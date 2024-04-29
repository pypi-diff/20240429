# Comparing `tmp/pyunifiprotect-5.1.3.tar.gz` & `tmp/pyunifiprotect-5.2.0.tar.gz`

## Comparing `pyunifiprotect-5.1.3.tar` & `pyunifiprotect-5.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/__main__.py
--rw-r--r--   0        0        0    61141 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/api.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/py.typed
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/stream.py
--rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/utils.py
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/websocket.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/__init__.py
--rw-r--r--   0        0        0    36594 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/backup.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/base.py
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/cameras.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/chimes.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/events.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/lights.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/nvr.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/sensors.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/cli/viewers.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/__init__.py
--rw-r--r--   0        0        0    37904 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/base.py
--rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/convert.py
--rw-r--r--   0        0        0   101900 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/devices.py
--rw-r--r--   0        0        0    38059 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/nvr.py
--rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/types.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/user.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/data/websocket.py
--rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/LICENSE
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/README.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/pyproject.toml
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 pyunifiprotect-5.1.3/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/__main__.py
+-rw-r--r--   0        0        0    65682 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/api.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/py.typed
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/stream.py
+-rw-r--r--   0        0        0    17948 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/utils.py
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/websocket.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0        0        0    36594 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/backup.py
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/base.py
+-rw-r--r--   0        0        0    17030 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/events.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/lights.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/cli/viewers.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/__init__.py
+-rw-r--r--   0        0        0    37567 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/base.py
+-rw-r--r--   0        0        0    21842 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/convert.py
+-rw-r--r--   0        0        0   113370 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/devices.py
+-rw-r--r--   0        0        0    47904 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/nvr.py
+-rw-r--r--   0        0        0    15445 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/types.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/user.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/data/websocket.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/LICENSE
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/README.md
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 pyunifiprotect-5.2.0/PKG-INFO
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/api.py` & `pyunifiprotect-5.2.0/pyunifiprotect/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     EventCategories,
     EventType,
     Light,
     Liveview,
     ModelType,
     ProtectAdoptableDeviceModel,
     ProtectModel,
+    PTZPosition,
+    PTZPreset,
     Sensor,
     SmartDetectObjectType,
     SmartDetectTrack,
     Version,
     Viewer,
     WSPacket,
     WSSubscriptionMessage,
@@ -1785,7 +1787,159 @@
         for url in PROTECT_APT_URLS:
             try:
                 versions |= await self._get_versions_from_api(url)
             except NvrError:
                 _LOGGER.warning("Failed to retrieve release versions from online.")
 
         return versions
+
+    async def relative_move_ptz_camera(
+        self,
+        device_id: str,
+        *,
+        pan: float,
+        tilt: float,
+        pan_speed: int = 10,
+        tilt_speed: int = 10,
+        scale: int = 0,
+    ) -> None:
+        """Move PTZ Camera relatively.
+
+        Pan/tilt values vary from camera to camera, but for G4 PTZ:
+            * Pan values range from 1 (0°) to 35200 (360°/0°).
+            * Tilt values range from 1 (-20°) to 9777 (90°).
+
+        Relative positions cannot move more then 4095 units in either direction at a time.
+
+        Camera objects have ptz values in feature flags and the methods on them provide better
+        control.
+        """
+
+        data = {
+            "type": "relative",
+            "payload": {
+                "panPos": pan,
+                "tiltPos": tilt,
+                "panSpeed": pan_speed,
+                "tiltSpeed": tilt_speed,
+                "scale": scale,
+            },
+        }
+
+        await self.api_request(f"cameras/{device_id}/move", method="post", json=data)
+
+    async def center_ptz_camera(
+        self,
+        device_id: str,
+        *,
+        x: int,
+        y: int,
+        z: int,
+    ) -> None:
+        """Center PTZ Camera on point in viewport.
+
+        x, y, z values range from 0 to 1000.
+
+        x, y are relative coords for the current viewport:
+            * (0, 0) is top left
+            * (500, 500) is the center
+            * (1000, 1000) is the bottom right
+
+        z value is zoom, but since it is capped at 1000, probably better to use `ptz_zoom_camera`.
+        """
+
+        data = {
+            "type": "center",
+            "payload": {
+                "x": x,
+                "y": y,
+                "z": z,
+            },
+        }
+
+        await self.api_request(f"cameras/{device_id}/move", method="post", json=data)
+
+    async def zoom_ptz_camera(
+        self,
+        device_id: str,
+        *,
+        zoom: float,
+        speed: int = 10,
+    ) -> None:
+        """Zoom PTZ Camera.
+
+        Zoom levels vary from camera to camera, but for G4 PTZ it goes from 0 (1x) to 2010 (22x).
+
+        Zoom speed does not seem to do much, if anything.
+
+        Camera objects have ptz values in feature flags and the methods on them provide better
+        control.
+        """
+
+        data = {
+            "type": "zoom",
+            "payload": {
+                "zoomPos": zoom,
+                "zoomSpeed": speed,
+            },
+        }
+
+        await self.api_request(f"cameras/{device_id}/move", method="post", json=data)
+
+    async def get_position_ptz_camera(self, device_id: str) -> PTZPosition:
+        """Get current PTZ camera position."""
+
+        pos = await self.api_request_obj(f"cameras/{device_id}/ptz/position")
+        return PTZPosition(**pos)
+
+    async def goto_ptz_camera(self, device_id: str, *, slot: int = -1) -> None:
+        """Goto PTZ slot position.
+
+        -1 is Home slot.
+        """
+
+        await self.api_request(f"cameras/{device_id}/ptz/goto/{slot}", method="post")
+
+    async def create_preset_ptz_camera(self, device_id: str, *, name: str) -> PTZPreset:
+        """Create PTZ Preset for camera based on current camera settings."""
+
+        preset = await self.api_request_obj(
+            f"cameras/{device_id}/ptz/preset",
+            method="post",
+            json={"name": name},
+        )
+
+        return PTZPreset(**preset)
+
+    async def get_presets_ptz_camera(self, device_id: str) -> list[PTZPreset]:
+        """Get PTZ Presets for camera."""
+
+        presets = await self.api_request(f"cameras/{device_id}/ptz/preset")
+
+        if not presets:
+            return []
+
+        presets = cast(list[dict[str, Any]], presets)
+        return [PTZPreset(**p) for p in presets]
+
+    async def delete_preset_ptz_camera(self, device_id: str, *, slot: int) -> None:
+        """Delete PTZ preset for camera."""
+
+        await self.api_request(
+            f"cameras/{device_id}/ptz/preset/{slot}",
+            method="delete",
+        )
+
+    async def get_home_ptz_camera(self, device_id: str) -> PTZPreset:
+        """Get PTZ home preset (-1)."""
+
+        preset = await self.api_request_obj(f"cameras/{device_id}/ptz/home")
+        return PTZPreset(**preset)
+
+    async def set_home_ptz_camera(self, device_id: str) -> PTZPreset:
+        """Set PTZ home preset (-1) to current position."""
+
+        preset = await self.api_request_obj(
+            f"cameras/{device_id}/ptz/home",
+            method="post",
+        )
+        return PTZPreset(**preset)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/exceptions.py` & `pyunifiprotect-5.2.0/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/stream.py` & `pyunifiprotect-5.2.0/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/utils.py` & `pyunifiprotect-5.2.0/pyunifiprotect/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,36 +24,26 @@
 import time
 from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union, overload
 from uuid import UUID
 import zoneinfo
 
 from aiohttp import ClientResponse
 import jwt
+from pydantic.v1.fields import SHAPE_DICT, SHAPE_LIST, SHAPE_SET, ModelField
+from pydantic.v1.utils import to_camel
 
 from pyunifiprotect.data.types import (
     Color,
     SmartDetectAudioType,
     SmartDetectObjectType,
     Version,
     VideoMode,
 )
 from pyunifiprotect.exceptions import NvrError
 
-try:
-    from pydantic.v1.fields import SHAPE_DICT, SHAPE_LIST, SHAPE_SET, ModelField
-    from pydantic.v1.utils import to_camel
-except ImportError:
-    from pydantic.fields import (  # type: ignore[attr-defined]
-        SHAPE_DICT,
-        SHAPE_LIST,
-        SHAPE_SET,
-        ModelField,
-    )
-    from pydantic.utils import to_camel
-
 if TYPE_CHECKING:
     from pyunifiprotect.api import ProtectApiClient
     from pyunifiprotect.data import CoordType, Event
     from pyunifiprotect.data.bootstrap import WSStat
 
 if sys.version_info[:2] < (3, 11):
     from async_timeout import timeout as asyncio_timeout
@@ -622,7 +612,14 @@
 def run_async(callback: Coroutine[Any, Any, T]) -> T:
     """Run async coroutine."""
 
     if sys.version_info >= (3, 11):
         return asyncio.run(callback)
     loop = asyncio.get_event_loop()
     return loop.run_until_complete(callback)
+
+
+def clamp_value(value: float, step_size: float) -> float:
+    """Clamps value to multiples of step size."""
+
+    ratio = 1 / step_size
+    return int(value * ratio) / ratio
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/websocket.py` & `pyunifiprotect-5.2.0/pyunifiprotect/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,11 +312,9 @@
         return versions
 
     _setup_logger()
 
     versions = run_async(callback())
     output = orjson.dumps(sorted([str(v) for v in versions]))
 
-    with open(RELEASE_CACHE, "wb") as cache_file:
-        cache_file.write(output)
-
+    Path(RELEASE_CACHE).write_bytes(output)
     typer.echo(output.decode("utf-8"))
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/backup.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/base.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,22 @@
 
 from collections.abc import Callable, Coroutine, Mapping, Sequence
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Optional, TypeVar
 
 import orjson
+from pydantic.v1 import ValidationError
 import typer
 
 from pyunifiprotect.api import ProtectApiClient
 from pyunifiprotect.data import NVR, ProtectAdoptableDeviceModel, ProtectBaseObject
 from pyunifiprotect.exceptions import BadRequest, NvrError, StreamError
 from pyunifiprotect.utils import run_async
 
-try:
-    from pydantic.v1 import ValidationError
-except ImportError:
-    from pydantic import ValidationError  # type: ignore[assignment]
-
 T = TypeVar("T")
 
 OPTION_FORCE = typer.Option(False, "-f", "--force", help="Skip confirmation prompt")
 
 
 class OutputFormatEnum(str, Enum):
     JSON = "json"
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,16 +170,15 @@
     else:
         snapshot = base.run(ctx, obj.get_snapshot(width, height, dt=dt))
 
     if snapshot is None:
         typer.secho("Could not get snapshot", fg="red")
         raise typer.Exit(1)
 
-    with open(output_path, "wb") as f:
-        f.write(snapshot)
+    Path(output_path).write_bytes(snapshot)
 
 
 @app.command()
 def save_video(
     ctx: typer.Context,
     output_path: Path = typer.Argument(..., help="MP4 format"),
     start: datetime = typer.Argument(...),
@@ -220,15 +219,15 @@
     if channel == 4 and not obj.feature_flags.has_package_camera:
         typer.secho("Camera does not have package camera", fg="red")
         raise typer.Exit(1)
 
     with Progress() as pb:
         task_id = pb.add_task("(1/2) Exporting", total=100)
 
-        async def callback(step: int, current: int, total: int) -> None:
+        async def callback(step: int, current: int, total: int) -> None:  # noqa: RUF029
             pb.update(
                 task_id,
                 total=total,
                 completed=current,
                 description="(2/2) Downloading",
             )
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/events.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,16 +135,15 @@
     for obj in objs.values():
         event_type = obj.type.value
         if event_type in {
             d.EventType.SMART_DETECT.value,
             d.EventType.SMART_DETECT_LINE.value,
         }:
             event_type = f"{event_type}[{','.join(obj.smart_detect_types)}]"
-        if len(event_type) > longest_event:
-            longest_event = len(event_type)
+        longest_event = max(len(event_type), longest_event)
         dt = obj.timestamp or obj.start
         dt = local_datetime(dt)
 
         to_print.append((obj.id, event_type, dt))
 
     if ctx.obj.output_format == base.OutputFormatEnum.JSON:
         base.json_output(to_print)
@@ -170,16 +169,15 @@
     event: d.Event = ctx.obj.event
 
     thumbnail = base.run(ctx, event.get_thumbnail())
     if thumbnail is None:
         typer.secho("Could not get thumbnail", fg="red")
         raise typer.Exit(1)
 
-    with open(output_path, "wb") as f:
-        f.write(thumbnail)
+    Path(output_path).write_bytes(thumbnail)
 
 
 @app.command()
 def save_animated_thumbnail(
     ctx: typer.Context,
     output_path: Path = typer.Argument(..., help="GIF format"),
 ) -> None:
@@ -192,16 +190,15 @@
     event: d.Event = ctx.obj.event
 
     thumbnail = base.run(ctx, event.get_animated_thumbnail())
     if thumbnail is None:
         typer.secho("Could not get thumbnail", fg="red")
         raise typer.Exit(1)
 
-    with open(output_path, "wb") as f:
-        f.write(thumbnail)
+    Path(output_path).write_bytes(thumbnail)
 
 
 @app.command()
 def save_heatmap(
     ctx: typer.Context,
     output_path: Path = typer.Argument(..., help="PNG format"),
 ) -> None:
@@ -214,16 +211,15 @@
     event: d.Event = ctx.obj.event
 
     heatmap = base.run(ctx, event.get_heatmap())
     if heatmap is None:
         typer.secho("Could not get heatmap", fg="red")
         raise typer.Exit(1)
 
-    with open(output_path, "wb") as f:
-        f.write(heatmap)
+    Path(output_path).write_bytes(heatmap)
 
 
 @app.command()
 def save_video(
     ctx: typer.Context,
     output_path: Path = typer.Argument(..., help="MP4 format"),
     channel: int = typer.Option(
@@ -242,15 +238,15 @@
 
     require_event_id(ctx)
     event: d.Event = ctx.obj.event
 
     with Progress() as pb:
         task_id = pb.add_task("(1/2) Exporting", total=100)
 
-        async def callback(step: int, current: int, total: int) -> None:
+        async def callback(step: int, current: int, total: int) -> None:  # noqa: RUF029
             pb.update(
                 task_id,
                 total=total,
                 completed=current,
                 description="(2/2) Downloading",
             )
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/lights.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-5.2.0/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/__init__.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     LightModeType,
     LockStatusType,
     ModelType,
     MountType,
     Percent,
     PermissionNode,
     ProtectWSPayloadFormat,
+    PTZPosition,
+    PTZPreset,
     RecordingMode,
     SensorStatusType,
     SensorType,
     SmartDetectAudioType,
     SmartDetectObjectType,
     StateType,
     StorageType,
@@ -113,14 +115,16 @@
     "LightModeEnableType",
     "LightModeType",
     "Liveview",
     "LockStatusType",
     "ModelType",
     "MountType",
     "NVRLocation",
+    "PTZPosition",
+    "PTZPreset",
     "Percent",
     "Permission",
     "PermissionNode",
     "ProtectAdoptableDeviceModel",
     "ProtectBaseObject",
     "ProtectDeviceModel",
     "ProtectModel",
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/base.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from datetime import datetime, timedelta
 from functools import cache
 from ipaddress import IPv4Address
 import logging
 from typing import TYPE_CHECKING, Any, ClassVar, Optional, TypeVar, Union
 from uuid import UUID
 
+from pydantic.v1 import BaseModel
+from pydantic.v1.fields import SHAPE_DICT, SHAPE_LIST, PrivateAttr
+
 from pyunifiprotect.data.types import (
     ModelType,
     PercentFloat,
     PermissionNode,
     ProtectWSPayloadFormat,
     StateType,
 )
@@ -30,35 +33,20 @@
     dict_diff,
     is_debug,
     process_datetime,
     serialize_unifi_obj,
     to_snake_case,
 )
 
-try:
-    from pydantic.v1 import BaseModel
-    from pydantic.v1.fields import SHAPE_DICT, SHAPE_LIST, PrivateAttr
-except ImportError:
-    from pydantic import BaseModel  # type: ignore[assignment]
-    from pydantic.fields import (  # type: ignore[attr-defined]
-        SHAPE_DICT,
-        SHAPE_LIST,
-        PrivateAttr,
-    )
-
 if TYPE_CHECKING:
     from asyncio.events import TimerHandle
 
+    from pydantic.v1.typing import DictStrAny, SetStr
     from typing_extensions import Self  # requires Python 3.11+
 
-    try:
-        from pydantic.v1.typing import DictStrAny, SetStr
-    except ImportError:
-        from pydantic.typing import DictStrAny, SetStr
-
     from pyunifiprotect.api import ProtectApiClient
     from pyunifiprotect.data.devices import Bridge
     from pyunifiprotect.data.nvr import Event
     from pyunifiprotect.data.user import User
 
 
 ProtectObject = TypeVar("ProtectObject", bound="ProtectBaseObject")
@@ -465,15 +453,15 @@
 
         use_obj = False
         if data is None:
             excluded_fields = (
                 self._get_protect_objs_set() | self._get_protect_lists_set()
             )
             if exclude is not None:
-                excluded_fields = excluded_fields | exclude
+                excluded_fields |= exclude
             data = self.dict(exclude=excluded_fields)
             use_obj = True
 
         for key, klass in self._get_protect_objs().items():
             if use_obj or key in data:
                 data[key] = self._unifi_dict_protect_obj(data, key, use_obj, klass)
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 import logging
 from typing import Any, Optional, cast
 from uuid import UUID
 
 from aiohttp.client_exceptions import ServerDisconnectedError
-
-try:
-    from pydantic.v1 import PrivateAttr, ValidationError
-except ImportError:
-    from pydantic import PrivateAttr, ValidationError  # type: ignore[assignment]
+from pydantic.v1 import PrivateAttr, ValidationError
 
 from pyunifiprotect.data.base import (
     RECENT_EVENT_MAX,
     ProtectBaseObject,
     ProtectModel,
     ProtectModelWithId,
 )
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/convert.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/devices.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,6355 +15,7072 @@
 000000e0: 206c 6f67 6769 6e67 0a66 726f 6d20 7061   logging.from pa
 000000f0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
 00000100: 680a 6672 6f6d 2074 7970 696e 6720 696d  h.from typing im
 00000110: 706f 7274 2054 5950 455f 4348 4543 4b49  port TYPE_CHECKI
 00000120: 4e47 2c20 416e 792c 204c 6974 6572 616c  NG, Any, Literal
 00000130: 2c20 4f70 7469 6f6e 616c 2c20 556e 696f  , Optional, Unio
 00000140: 6e2c 2063 6173 740a 696d 706f 7274 2077  n, cast.import w
-00000150: 6172 6e69 6e67 730a 0a74 7279 3a0a 2020  arnings..try:.  
-00000160: 2020 6672 6f6d 2070 7964 616e 7469 632e    from pydantic.
-00000170: 7631 2e66 6965 6c64 7320 696d 706f 7274  v1.fields import
-00000180: 2050 7269 7661 7465 4174 7472 0a65 7863   PrivateAttr.exc
-00000190: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
-000001a0: 0a20 2020 2066 726f 6d20 7079 6461 6e74  .    from pydant
-000001b0: 6963 2e66 6965 6c64 7320 696d 706f 7274  ic.fields import
-000001c0: 2050 7269 7661 7465 4174 7472 0a0a 6672   PrivateAttr..fr
-000001d0: 6f6d 2070 7975 6e69 6669 7072 6f74 6563  om pyunifiprotec
-000001e0: 742e 6461 7461 2e62 6173 6520 696d 706f  t.data.base impo
-000001f0: 7274 2028 0a20 2020 2045 5645 4e54 5f50  rt (.    EVENT_P
-00000200: 494e 475f 494e 5445 5256 414c 2c0a 2020  ING_INTERVAL,.  
-00000210: 2020 5072 6f74 6563 7441 646f 7074 6162    ProtectAdoptab
-00000220: 6c65 4465 7669 6365 4d6f 6465 6c2c 0a20  leDeviceModel,. 
-00000230: 2020 2050 726f 7465 6374 4261 7365 4f62     ProtectBaseOb
-00000240: 6a65 6374 2c0a 2020 2020 5072 6f74 6563  ject,.    Protec
-00000250: 744d 6f74 696f 6e44 6576 6963 654d 6f64  tMotionDeviceMod
-00000260: 656c 2c0a 290a 6672 6f6d 2070 7975 6e69  el,.).from pyuni
-00000270: 6669 7072 6f74 6563 742e 6461 7461 2e74  fiprotect.data.t
-00000280: 7970 6573 2069 6d70 6f72 7420 280a 2020  ypes import (.  
-00000290: 2020 4445 4641 554c 542c 0a20 2020 2044    DEFAULT,.    D
-000002a0: 4546 4155 4c54 5f54 5950 452c 0a20 2020  EFAULT_TYPE,.   
-000002b0: 2041 7564 696f 436f 6465 6373 2c0a 2020   AudioCodecs,.  
-000002c0: 2020 4175 6469 6f53 7479 6c65 2c0a 2020    AudioStyle,.  
-000002d0: 2020 4175 746f 4578 706f 7375 7265 4d6f    AutoExposureMo
-000002e0: 6465 2c0a 2020 2020 4368 696d 6554 7970  de,.    ChimeTyp
-000002f0: 652c 0a20 2020 2043 6f6c 6f72 2c0a 2020  e,.    Color,.  
-00000300: 2020 446f 6f72 6265 6c6c 4d65 7373 6167    DoorbellMessag
-00000310: 6554 7970 652c 0a20 2020 2046 6f63 7573  eType,.    Focus
-00000320: 4d6f 6465 2c0a 2020 2020 4765 6f66 656e  Mode,.    Geofen
-00000330: 6369 6e67 5365 7474 696e 672c 0a20 2020  cingSetting,.   
-00000340: 2048 4452 4d6f 6465 2c0a 2020 2020 4943   HDRMode,.    IC
-00000350: 5243 7573 746f 6d56 616c 7565 2c0a 2020  RCustomValue,.  
-00000360: 2020 4943 524c 7578 5661 6c75 652c 0a20    ICRLuxValue,. 
-00000370: 2020 2049 4352 5365 6e73 6974 6976 6974     ICRSensitivit
-00000380: 792c 0a20 2020 2049 524c 4544 4d6f 6465  y,.    IRLEDMode
-00000390: 2c0a 2020 2020 4974 6572 6174 6f72 4361  ,.    IteratorCa
-000003a0: 6c6c 6261 636b 2c0a 2020 2020 4c45 444c  llback,.    LEDL
-000003b0: 6576 656c 2c0a 2020 2020 4c65 6e73 5479  evel,.    LensTy
-000003c0: 7065 2c0a 2020 2020 4c69 6768 744d 6f64  pe,.    LightMod
-000003d0: 6545 6e61 626c 6554 7970 652c 0a20 2020  eEnableType,.   
-000003e0: 204c 6967 6874 4d6f 6465 5479 7065 2c0a   LightModeType,.
-000003f0: 2020 2020 4c6f 636b 5374 6174 7573 5479      LockStatusTy
-00000400: 7065 2c0a 2020 2020 4c6f 774d 6564 4869  pe,.    LowMedHi
-00000410: 6768 2c0a 2020 2020 4d6f 6465 6c54 7970  gh,.    ModelTyp
-00000420: 652c 0a20 2020 204d 6f74 696f 6e41 6c67  e,.    MotionAlg
-00000430: 6f72 6974 686d 2c0a 2020 2020 4d6f 756e  orithm,.    Moun
-00000440: 7450 6f73 6974 696f 6e2c 0a20 2020 204d  tPosition,.    M
-00000450: 6f75 6e74 5479 7065 2c0a 2020 2020 5065  ountType,.    Pe
-00000460: 7263 656e 742c 0a20 2020 2050 6572 6365  rcent,.    Perce
-00000470: 6e74 496e 742c 0a20 2020 2050 6572 6d69  ntInt,.    Permi
-00000480: 7373 696f 6e4e 6f64 652c 0a20 2020 2050  ssionNode,.    P
-00000490: 726f 6772 6573 7343 616c 6c62 6163 6b2c  rogressCallback,
-000004a0: 0a20 2020 2052 6563 6f72 6469 6e67 4d6f  .    RecordingMo
-000004b0: 6465 2c0a 2020 2020 5265 7065 6174 5469  de,.    RepeatTi
-000004c0: 6d65 732c 0a20 2020 2053 656e 736f 7253  mes,.    SensorS
-000004d0: 7461 7475 7354 7970 652c 0a20 2020 2053  tatusType,.    S
-000004e0: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
-000004f0: 7970 652c 0a20 2020 2053 6d61 7274 4465  ype,.    SmartDe
-00000500: 7465 6374 4f62 6a65 6374 5479 7065 2c0a  tectObjectType,.
-00000510: 2020 2020 5477 6f42 7974 6549 6e74 2c0a      TwoByteInt,.
-00000520: 2020 2020 5669 6465 6f4d 6f64 652c 0a20      VideoMode,. 
-00000530: 2020 2057 4452 4c65 7665 6c2c 0a29 0a66     WDRLevel,.).f
-00000540: 726f 6d20 7079 756e 6966 6970 726f 7465  rom pyunifiprote
-00000550: 6374 2e64 6174 612e 7573 6572 2069 6d70  ct.data.user imp
-00000560: 6f72 7420 5573 6572 0a66 726f 6d20 7079  ort User.from py
-00000570: 756e 6966 6970 726f 7465 6374 2e65 7863  unifiprotect.exc
-00000580: 6570 7469 6f6e 7320 696d 706f 7274 2042  eptions import B
-00000590: 6164 5265 7175 6573 742c 204e 6f74 4175  adRequest, NotAu
-000005a0: 7468 6f72 697a 6564 2c20 5374 7265 616d  thorized, Stream
-000005b0: 4572 726f 720a 6672 6f6d 2070 7975 6e69  Error.from pyuni
-000005c0: 6669 7072 6f74 6563 742e 7374 7265 616d  fiprotect.stream
-000005d0: 2069 6d70 6f72 7420 5461 6c6b 6261 636b   import Talkback
-000005e0: 5374 7265 616d 0a66 726f 6d20 7079 756e  Stream.from pyun
-000005f0: 6966 6970 726f 7465 6374 2e75 7469 6c73  ifiprotect.utils
-00000600: 2069 6d70 6f72 7420 280a 2020 2020 636f   import (.    co
-00000610: 6e76 6572 745f 736d 6172 745f 6175 6469  nvert_smart_audi
-00000620: 6f5f 7479 7065 732c 0a20 2020 2063 6f6e  o_types,.    con
-00000630: 7665 7274 5f73 6d61 7274 5f74 7970 6573  vert_smart_types
-00000640: 2c0a 2020 2020 636f 6e76 6572 745f 7669  ,.    convert_vi
-00000650: 6465 6f5f 6d6f 6465 732c 0a20 2020 2066  deo_modes,.    f
-00000660: 726f 6d5f 6a73 5f74 696d 652c 0a20 2020  rom_js_time,.   
-00000670: 2070 726f 6365 7373 5f64 6174 6574 696d   process_datetim
-00000680: 652c 0a20 2020 2073 6572 6961 6c69 7a65  e,.    serialize
-00000690: 5f70 6f69 6e74 2c0a 2020 2020 746f 5f6a  _point,.    to_j
-000006a0: 735f 7469 6d65 2c0a 2020 2020 7574 635f  s_time,.    utc_
-000006b0: 6e6f 772c 0a29 0a0a 6966 2054 5950 455f  now,.)..if TYPE_
-000006c0: 4348 4543 4b49 4e47 3a0a 2020 2020 6672  CHECKING:.    fr
-000006d0: 6f6d 2070 7975 6e69 6669 7072 6f74 6563  om pyunifiprotec
-000006e0: 742e 6461 7461 2e6e 7672 2069 6d70 6f72  t.data.nvr impor
-000006f0: 7420 4576 656e 742c 204c 6976 6576 6965  t Event, Livevie
-00000700: 770a 0a50 5249 5641 4359 5f5a 4f4e 455f  w..PRIVACY_ZONE_
-00000710: 4e41 4d45 203d 2022 7079 7566 705f 7072  NAME = "pyufp_pr
-00000720: 6976 6163 795f 7a6f 6e65 220a 4c55 585f  ivacy_zone".LUX_
-00000730: 4d41 5050 494e 475f 5641 4c55 4553 203d  MAPPING_VALUES =
-00000740: 205b 0a20 2020 2033 302c 0a20 2020 2032   [.    30,.    2
-00000750: 352c 0a20 2020 2032 302c 0a20 2020 2031  5,.    20,.    1
-00000760: 352c 0a20 2020 2031 322c 0a20 2020 2031  5,.    12,.    1
-00000770: 302c 0a20 2020 2037 2c0a 2020 2020 352c  0,.    7,.    5,
-00000780: 0a20 2020 2033 2c0a 2020 2020 312c 0a5d  .    3,.    1,.]
-00000790: 0a0a 5f4c 4f47 4745 5220 3d20 6c6f 6767  .._LOGGER = logg
-000007a0: 696e 672e 6765 744c 6f67 6765 7228 5f5f  ing.getLogger(__
-000007b0: 6e61 6d65 5f5f 290a 0a0a 636c 6173 7320  name__)...class 
-000007c0: 4c69 6768 7444 6576 6963 6553 6574 7469  LightDeviceSetti
-000007d0: 6e67 7328 5072 6f74 6563 7442 6173 654f  ngs(ProtectBaseO
-000007e0: 626a 6563 7429 3a0a 2020 2020 2320 5374  bject):.    # St
-000007f0: 6174 7573 204c 4544 0a20 2020 2069 735f  atus LED.    is_
-00000800: 696e 6469 6361 746f 725f 656e 6162 6c65  indicator_enable
-00000810: 643a 2062 6f6f 6c0a 2020 2020 2320 4272  d: bool.    # Br
-00000820: 6967 6874 6e65 7373 0a20 2020 206c 6564  ightness.    led
-00000830: 5f6c 6576 656c 3a20 4c45 444c 6576 656c  _level: LEDLevel
-00000840: 0a20 2020 206c 7578 5f73 656e 7369 7469  .    lux_sensiti
-00000850: 7669 7479 3a20 4c6f 774d 6564 4869 6768  vity: LowMedHigh
-00000860: 0a20 2020 2070 6972 5f64 7572 6174 696f  .    pir_duratio
-00000870: 6e3a 2074 696d 6564 656c 7461 0a20 2020  n: timedelta.   
-00000880: 2070 6972 5f73 656e 7369 7469 7669 7479   pir_sensitivity
-00000890: 3a20 5065 7263 656e 7449 6e74 0a0a 2020  : PercentInt..  
-000008a0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-000008b0: 2020 2064 6566 2075 6e69 6669 5f64 6963     def unifi_dic
-000008c0: 745f 746f 5f64 6963 7428 636c 732c 2064  t_to_dict(cls, d
-000008d0: 6174 613a 2064 6963 745b 7374 722c 2041  ata: dict[str, A
-000008e0: 6e79 5d29 202d 3e20 6469 6374 5b73 7472  ny]) -> dict[str
-000008f0: 2c20 416e 795d 3a0a 2020 2020 2020 2020  , Any]:.        
-00000900: 6966 2022 7069 7244 7572 6174 696f 6e22  if "pirDuration"
-00000910: 2069 6e20 6461 7461 2061 6e64 206e 6f74   in data and not
-00000920: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-00000930: 5b22 7069 7244 7572 6174 696f 6e22 5d2c  ["pirDuration"],
-00000940: 2074 696d 6564 656c 7461 293a 0a20 2020   timedelta):.   
-00000950: 2020 2020 2020 2020 2064 6174 615b 2270           data["p
-00000960: 6972 4475 7261 7469 6f6e 225d 203d 2074  irDuration"] = t
-00000970: 696d 6564 656c 7461 286d 696c 6c69 7365  imedelta(millise
-00000980: 636f 6e64 733d 6461 7461 5b22 7069 7244  conds=data["pirD
-00000990: 7572 6174 696f 6e22 5d29 0a0a 2020 2020  uration"])..    
-000009a0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-000009b0: 2829 2e75 6e69 6669 5f64 6963 745f 746f  ().unifi_dict_to
-000009c0: 5f64 6963 7428 6461 7461 290a 0a0a 636c  _dict(data)...cl
-000009d0: 6173 7320 4c69 6768 744f 6e53 6574 7469  ass LightOnSetti
-000009e0: 6e67 7328 5072 6f74 6563 7442 6173 654f  ngs(ProtectBaseO
-000009f0: 626a 6563 7429 3a0a 2020 2020 2320 4d61  bject):.    # Ma
-00000a00: 6e75 616c 2074 6f67 676c 6520 696e 2055  nual toggle in U
-00000a10: 490a 2020 2020 6973 5f6c 6564 5f66 6f72  I.    is_led_for
-00000a20: 6365 5f6f 6e3a 2062 6f6f 6c0a 0a0a 636c  ce_on: bool...cl
-00000a30: 6173 7320 4c69 6768 744d 6f64 6553 6574  ass LightModeSet
-00000a40: 7469 6e67 7328 5072 6f74 6563 7442 6173  tings(ProtectBas
-00000a50: 654f 626a 6563 7429 3a0a 2020 2020 2320  eObject):.    # 
-00000a60: 6d61 696e 2022 4c69 6768 7469 6e67 2220  main "Lighting" 
-00000a70: 7365 7474 696e 6773 0a20 2020 206d 6f64  settings.    mod
-00000a80: 653a 204c 6967 6874 4d6f 6465 5479 7065  e: LightModeType
-00000a90: 0a20 2020 2065 6e61 626c 655f 6174 3a20  .    enable_at: 
-00000aa0: 4c69 6768 744d 6f64 6545 6e61 626c 6554  LightModeEnableT
-00000ab0: 7970 650a 0a0a 636c 6173 7320 4c69 6768  ype...class Ligh
-00000ac0: 7428 5072 6f74 6563 744d 6f74 696f 6e44  t(ProtectMotionD
-00000ad0: 6576 6963 654d 6f64 656c 293a 0a20 2020  eviceModel):.   
-00000ae0: 2069 735f 7069 725f 6d6f 7469 6f6e 5f64   is_pir_motion_d
-00000af0: 6574 6563 7465 643a 2062 6f6f 6c0a 2020  etected: bool.  
-00000b00: 2020 6973 5f6c 6967 6874 5f6f 6e3a 2062    is_light_on: b
-00000b10: 6f6f 6c0a 2020 2020 6973 5f6c 6f63 6174  ool.    is_locat
-00000b20: 696e 673a 2062 6f6f 6c0a 2020 2020 6c69  ing: bool.    li
-00000b30: 6768 745f 6465 7669 6365 5f73 6574 7469  ght_device_setti
-00000b40: 6e67 733a 204c 6967 6874 4465 7669 6365  ngs: LightDevice
-00000b50: 5365 7474 696e 6773 0a20 2020 206c 6967  Settings.    lig
-00000b60: 6874 5f6f 6e5f 7365 7474 696e 6773 3a20  ht_on_settings: 
-00000b70: 4c69 6768 744f 6e53 6574 7469 6e67 730a  LightOnSettings.
-00000b80: 2020 2020 6c69 6768 745f 6d6f 6465 5f73      light_mode_s
-00000b90: 6574 7469 6e67 733a 204c 6967 6874 4d6f  ettings: LightMo
-00000ba0: 6465 5365 7474 696e 6773 0a20 2020 2063  deSettings.    c
-00000bb0: 616d 6572 615f 6964 3a20 4f70 7469 6f6e  amera_id: Option
-00000bc0: 616c 5b73 7472 5d0a 2020 2020 6973 5f63  al[str].    is_c
-00000bd0: 616d 6572 615f 7061 6972 6564 3a20 626f  amera_paired: bo
-00000be0: 6f6c 0a0a 2020 2020 4063 6c61 7373 6d65  ol..    @classme
-00000bf0: 7468 6f64 0a20 2020 2040 6361 6368 650a  thod.    @cache.
-00000c00: 2020 2020 6465 6620 5f67 6574 5f75 6e69      def _get_uni
-00000c10: 6669 5f72 656d 6170 7328 636c 7329 202d  fi_remaps(cls) -
-00000c20: 3e20 6469 6374 5b73 7472 2c20 7374 725d  > dict[str, str]
-00000c30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000c40: 207b 2a2a 7375 7065 7228 292e 5f67 6574   {**super()._get
-00000c50: 5f75 6e69 6669 5f72 656d 6170 7328 292c  _unifi_remaps(),
-00000c60: 2022 6361 6d65 7261 223a 2022 6361 6d65   "camera": "came
-00000c70: 7261 4964 227d 0a0a 2020 2020 4063 6c61  raId"}..    @cla
-00000c80: 7373 6d65 7468 6f64 0a20 2020 2040 6361  ssmethod.    @ca
-00000c90: 6368 650a 2020 2020 6465 6620 5f67 6574  che.    def _get
-00000ca0: 5f72 6561 645f 6f6e 6c79 5f66 6965 6c64  _read_only_field
-00000cb0: 7328 636c 7329 202d 3e20 7365 745b 7374  s(cls) -> set[st
-00000cc0: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
-00000cd0: 726e 2073 7570 6572 2829 2e5f 6765 745f  rn super()._get_
-00000ce0: 7265 6164 5f6f 6e6c 795f 6669 656c 6473  read_only_fields
-00000cf0: 2829 207c 207b 0a20 2020 2020 2020 2020  () | {.         
-00000d00: 2020 2022 6973 5069 724d 6f74 696f 6e44     "isPirMotionD
-00000d10: 6574 6563 7465 6422 2c0a 2020 2020 2020  etected",.      
-00000d20: 2020 2020 2020 2269 734c 6967 6874 4f6e        "isLightOn
-00000d30: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000d40: 6973 4c6f 6361 7469 6e67 222c 0a20 2020  isLocating",.   
-00000d50: 2020 2020 207d 0a0a 2020 2020 4070 726f       }..    @pro
-00000d60: 7065 7274 790a 2020 2020 6465 6620 6361  perty.    def ca
-00000d70: 6d65 7261 2873 656c 6629 202d 3e20 4f70  mera(self) -> Op
-00000d80: 7469 6f6e 616c 5b43 616d 6572 615d 3a0a  tional[Camera]:.
-00000d90: 2020 2020 2020 2020 2222 2250 6169 7265          """Paire
-00000da0: 6420 4361 6d65 7261 2077 696c 6c20 616c  d Camera will al
-00000db0: 7761 7973 2062 6520 6e6f 6e65 2069 6620  ways be none if 
-00000dc0: 6e6f 2063 616d 6572 6120 6973 2070 6169  no camera is pai
-00000dd0: 7265 6422 2222 0a0a 2020 2020 2020 2020  red"""..        
-00000de0: 6966 2073 656c 662e 6361 6d65 7261 5f69  if self.camera_i
-00000df0: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
-00000e00: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00000e10: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
-00000e20: 726e 2073 656c 662e 6170 692e 626f 6f74  rn self.api.boot
-00000e30: 7374 7261 702e 6361 6d65 7261 735b 7365  strap.cameras[se
-00000e40: 6c66 2e63 616d 6572 615f 6964 5d0a 0a20  lf.camera_id].. 
-00000e50: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-00000e60: 5f70 6169 7265 645f 6361 6d65 7261 2873  _paired_camera(s
-00000e70: 656c 662c 2063 616d 6572 613a 204f 7074  elf, camera: Opt
-00000e80: 696f 6e61 6c5b 4361 6d65 7261 5d29 202d  ional[Camera]) -
-00000e90: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00000ea0: 2222 2253 6574 7320 7468 6520 6361 6d65  """Sets the came
-00000eb0: 7261 2070 6169 7265 6420 7769 7468 2074  ra paired with t
-00000ec0: 6865 206c 6967 6874 2222 220a 0a20 2020  he light"""..   
-00000ed0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00000ee0: 7365 6c66 2e5f 7570 6461 7465 5f6c 6f63  self._update_loc
-00000ef0: 6b3a 0a20 2020 2020 2020 2020 2020 2061  k:.            a
-00000f00: 7761 6974 2061 7379 6e63 696f 2e73 6c65  wait asyncio.sle
-00000f10: 6570 280a 2020 2020 2020 2020 2020 2020  ep(.            
-00000f20: 2020 2020 302c 0a20 2020 2020 2020 2020      0,.         
-00000f30: 2020 2029 2020 2320 7969 656c 6420 746f     )  # yield to
-00000f40: 2074 6865 2065 7665 6e74 206c 6f6f 7020   the event loop 
-00000f50: 6f6e 6365 2077 6520 6861 7665 2074 6865  once we have the
-00000f60: 206c 6f63 6b20 746f 2070 726f 6365 7373   lock to process
-00000f70: 2061 6e79 2070 656e 6469 6e67 2075 7064   any pending upd
-00000f80: 6174 6573 0a20 2020 2020 2020 2020 2020  ates.           
-00000f90: 2064 6174 615f 6265 666f 7265 5f63 6861   data_before_cha
-00000fa0: 6e67 6573 203d 2073 656c 662e 6469 6374  nges = self.dict
-00000fb0: 5f77 6974 685f 6578 636c 7564 6573 2829  _with_excludes()
-00000fc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000fd0: 6361 6d65 7261 2069 7320 4e6f 6e65 3a0a  camera is None:.
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 7365 6c66 2e63 616d 6572 615f 6964 203d  self.camera_id =
-00001000: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00001010: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001020: 2020 2020 2020 2020 7365 6c66 2e63 616d          self.cam
-00001030: 6572 615f 6964 203d 2063 616d 6572 612e  era_id = camera.
-00001040: 6964 0a20 2020 2020 2020 2020 2020 2061  id.            a
-00001050: 7761 6974 2073 656c 662e 7361 7665 5f64  wait self.save_d
-00001060: 6576 6963 6528 6461 7461 5f62 6566 6f72  evice(data_befor
-00001070: 655f 6368 616e 6765 732c 2066 6f72 6365  e_changes, force
-00001080: 5f65 6d69 743d 5472 7565 290a 0a20 2020  _emit=True)..   
-00001090: 2061 7379 6e63 2064 6566 2073 6574 5f73   async def set_s
-000010a0: 7461 7475 735f 6c69 6768 7428 7365 6c66  tatus_light(self
-000010b0: 2c20 656e 6162 6c65 643a 2062 6f6f 6c29  , enabled: bool)
-000010c0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000010d0: 2020 2222 2253 6574 7320 7468 6520 7374    """Sets the st
-000010e0: 6174 7573 2069 6e64 6963 6174 6f72 206c  atus indicator l
-000010f0: 6967 6874 2066 6f72 2074 6865 206c 6967  ight for the lig
-00001100: 6874 2222 220a 0a20 2020 2020 2020 2064  ht"""..        d
-00001110: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
-00001120: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00001130: 2020 2073 656c 662e 6c69 6768 745f 6465     self.light_de
-00001140: 7669 6365 5f73 6574 7469 6e67 732e 6973  vice_settings.is
-00001150: 5f69 6e64 6963 6174 6f72 5f65 6e61 626c  _indicator_enabl
-00001160: 6564 203d 2065 6e61 626c 6564 0a0a 2020  ed = enabled..  
-00001170: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-00001180: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
-00001190: 6c6c 6261 636b 290a 0a20 2020 2061 7379  llback)..    asy
-000011a0: 6e63 2064 6566 2073 6574 5f6c 6564 5f6c  nc def set_led_l
-000011b0: 6576 656c 2873 656c 662c 206c 6564 5f6c  evel(self, led_l
-000011c0: 6576 656c 3a20 696e 7429 202d 3e20 4e6f  evel: int) -> No
-000011d0: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
-000011e0: 6574 7320 7468 6520 4c45 4420 6c65 7665  ets the LED leve
-000011f0: 6c20 666f 7220 7468 6520 6c69 6768 7422  l for the light"
-00001200: 2222 0a0a 2020 2020 2020 2020 6465 6620  ""..        def 
-00001210: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
-00001220: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001230: 7365 6c66 2e6c 6967 6874 5f64 6576 6963  self.light_devic
-00001240: 655f 7365 7474 696e 6773 2e6c 6564 5f6c  e_settings.led_l
-00001250: 6576 656c 203d 204c 4544 4c65 7665 6c28  evel = LEDLevel(
-00001260: 6c65 645f 6c65 7665 6c29 0a0a 2020 2020  led_level)..    
-00001270: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00001280: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00001290: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-000012a0: 2064 6566 2073 6574 5f6c 6967 6874 2873   def set_light(s
-000012b0: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
-000012c0: 6f6c 2c20 6c65 645f 6c65 7665 6c3a 204f  ol, led_level: O
-000012d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000012e0: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
-000012f0: 2020 2020 2020 2222 2246 6f72 6365 2074        """Force t
-00001300: 7572 6e73 206f 6e2f 6f66 6620 7468 6520  urns on/off the 
-00001310: 6c69 6768 7422 2222 0a0a 2020 2020 2020  light"""..      
-00001320: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
-00001330: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00001340: 2020 2020 2020 7365 6c66 2e6c 6967 6874        self.light
-00001350: 5f6f 6e5f 7365 7474 696e 6773 2e69 735f  _on_settings.is_
-00001360: 6c65 645f 666f 7263 655f 6f6e 203d 2065  led_force_on = e
-00001370: 6e61 626c 6564 0a20 2020 2020 2020 2020  nabled.         
-00001380: 2020 2069 6620 6c65 645f 6c65 7665 6c20     if led_level 
-00001390: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000013a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000013b0: 662e 6c69 6768 745f 6465 7669 6365 5f73  f.light_device_s
-000013c0: 6574 7469 6e67 732e 6c65 645f 6c65 7665  ettings.led_leve
-000013d0: 6c20 3d20 4c45 444c 6576 656c 286c 6564  l = LEDLevel(led
-000013e0: 5f6c 6576 656c 290a 0a20 2020 2020 2020  _level)..       
-000013f0: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
-00001400: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
-00001410: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
-00001420: 6620 7365 745f 7365 6e73 6974 6976 6974  f set_sensitivit
-00001430: 7928 7365 6c66 2c20 7365 6e73 6974 6976  y(self, sensitiv
-00001440: 6974 793a 2069 6e74 2920 2d3e 204e 6f6e  ity: int) -> Non
-00001450: 653a 0a20 2020 2020 2020 2022 2222 5365  e:.        """Se
-00001460: 7473 206d 6f74 696f 6e20 7365 6e73 6974  ts motion sensit
-00001470: 6976 6974 7922 2222 0a0a 2020 2020 2020  ivity"""..      
-00001480: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
-00001490: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000014a0: 2020 2020 2020 7365 6c66 2e6c 6967 6874        self.light
-000014b0: 5f64 6576 6963 655f 7365 7474 696e 6773  _device_settings
-000014c0: 2e70 6972 5f73 656e 7369 7469 7669 7479  .pir_sensitivity
-000014d0: 203d 2050 6572 6365 6e74 496e 7428 7365   = PercentInt(se
-000014e0: 6e73 6974 6976 6974 7929 0a0a 2020 2020  nsitivity)..    
-000014f0: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00001500: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00001510: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-00001520: 2064 6566 2073 6574 5f64 7572 6174 696f   def set_duratio
-00001530: 6e28 7365 6c66 2c20 6475 7261 7469 6f6e  n(self, duration
-00001540: 3a20 7469 6d65 6465 6c74 6129 202d 3e20  : timedelta) -> 
-00001550: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00001560: 2253 6574 7320 6d6f 7469 6f6e 2073 656e  "Sets motion sen
-00001570: 7369 7469 7669 7479 2222 220a 0a20 2020  sitivity"""..   
-00001580: 2020 2020 2069 6620 6475 7261 7469 6f6e       if duration
-00001590: 2e74 6f74 616c 5f73 6563 6f6e 6473 2829  .total_seconds()
-000015a0: 203c 2031 3520 6f72 2064 7572 6174 696f   < 15 or duratio
-000015b0: 6e2e 746f 7461 6c5f 7365 636f 6e64 7328  n.total_seconds(
-000015c0: 2920 3e20 3930 303a 0a20 2020 2020 2020  ) > 900:.       
-000015d0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-000015e0: 7175 6573 7428 2244 7572 6174 696f 6e20  quest("Duration 
-000015f0: 6f75 7473 6964 6520 6f66 2031 3573 2074  outside of 15s t
-00001600: 6f20 3930 3073 2072 616e 6765 2229 0a0a  o 900s range")..
-00001610: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
-00001620: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
-00001630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001640: 2e6c 6967 6874 5f64 6576 6963 655f 7365  .light_device_se
-00001650: 7474 696e 6773 2e70 6972 5f64 7572 6174  ttings.pir_durat
-00001660: 696f 6e20 3d20 6475 7261 7469 6f6e 0a0a  ion = duration..
-00001670: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00001680: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
-00001690: 6361 6c6c 6261 636b 290a 0a20 2020 2061  callback)..    a
-000016a0: 7379 6e63 2064 6566 2073 6574 5f6c 6967  sync def set_lig
-000016b0: 6874 5f73 6574 7469 6e67 7328 0a20 2020  ht_settings(.   
-000016c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000016d0: 2020 206d 6f64 653a 204c 6967 6874 4d6f     mode: LightMo
-000016e0: 6465 5479 7065 2c0a 2020 2020 2020 2020  deType,.        
-000016f0: 656e 6162 6c65 5f61 743a 204f 7074 696f  enable_at: Optio
-00001700: 6e61 6c5b 4c69 6768 744d 6f64 6545 6e61  nal[LightModeEna
-00001710: 626c 6554 7970 655d 203d 204e 6f6e 652c  bleType] = None,
-00001720: 0a20 2020 2020 2020 2064 7572 6174 696f  .        duratio
-00001730: 6e3a 204f 7074 696f 6e61 6c5b 7469 6d65  n: Optional[time
-00001740: 6465 6c74 615d 203d 204e 6f6e 652c 0a20  delta] = None,. 
-00001750: 2020 2020 2020 2073 656e 7369 7469 7669         sensitivi
-00001760: 7479 3a20 4f70 7469 6f6e 616c 5b69 6e74  ty: Optional[int
-00001770: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
-00001780: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00001790: 2022 2222 5570 6461 7465 7320 7661 7269   """Updates vari
-000017a0: 6f75 7320 4c69 6768 7420 7365 7474 696e  ous Light settin
-000017b0: 6773 2e0a 0a20 2020 2020 2020 2041 7267  gs...        Arg
-000017c0: 733a 0a20 2020 2020 2020 202d 2d2d 2d0a  s:.        ----.
-000017d0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000017e0: 3a20 4c69 6768 7420 7472 6967 6765 7220  : Light trigger 
-000017f0: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
-00001800: 2065 6e61 626c 655f 6174 3a20 5468 656e   enable_at: Then
-00001810: 2074 6865 206c 6967 6874 2061 7574 6f6d   the light autom
-00001820: 6174 6963 616c 6c79 2074 7572 6e73 206f  atically turns o
-00001830: 6e20 6279 2069 7473 656c 660a 2020 2020  n by itself.    
-00001840: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
-00001850: 3a20 486f 7720 6c6f 6e67 2074 6865 206c  : How long the l
-00001860: 6967 6874 2073 686f 756c 6420 7265 6d61  ight should rema
-00001870: 696e 206f 6e20 6166 7465 7220 6d6f 7469  in on after moti
-00001880: 6f6e 2c20 6d75 7374 2062 6520 7469 6d65  on, must be time
-00001890: 6465 6c74 6120 6265 7477 6565 6e20 3135  delta between 15
-000018a0: 7320 616e 6420 3930 3073 0a20 2020 2020  s and 900s.     
-000018b0: 2020 2020 2020 2073 656e 7369 7469 7669         sensitivi
-000018c0: 7479 3a20 5049 5220 4d6f 7469 6f6e 2073  ty: PIR Motion s
-000018d0: 656e 7369 7469 7669 7479 0a20 2020 2020  ensitivity.     
-000018e0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000018f0: 6966 2064 7572 6174 696f 6e20 6973 206e  if duration is n
-00001900: 6f74 204e 6f6e 6520 616e 6420 280a 2020  ot None and (.  
-00001910: 2020 2020 2020 2020 2020 6475 7261 7469            durati
-00001920: 6f6e 2e74 6f74 616c 5f73 6563 6f6e 6473  on.total_seconds
-00001930: 2829 203c 2031 3520 6f72 2064 7572 6174  () < 15 or durat
-00001940: 696f 6e2e 746f 7461 6c5f 7365 636f 6e64  ion.total_second
-00001950: 7328 2920 3e20 3930 300a 2020 2020 2020  s() > 900.      
-00001960: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00001970: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-00001980: 7428 2244 7572 6174 696f 6e20 6f75 7473  t("Duration outs
-00001990: 6964 6520 6f66 2031 3573 2074 6f20 3930  ide of 15s to 90
-000019a0: 3073 2072 616e 6765 2229 0a0a 2020 2020  0s range")..    
-000019b0: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
-000019c0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-000019d0: 2020 2020 2020 2020 7365 6c66 2e6c 6967          self.lig
-000019e0: 6874 5f6d 6f64 655f 7365 7474 696e 6773  ht_mode_settings
-000019f0: 2e6d 6f64 6520 3d20 6d6f 6465 0a20 2020  .mode = mode.   
-00001a00: 2020 2020 2020 2020 2069 6620 656e 6162           if enab
-00001a10: 6c65 5f61 7420 6973 206e 6f74 204e 6f6e  le_at is not Non
-00001a20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00001a30: 2020 2073 656c 662e 6c69 6768 745f 6d6f     self.light_mo
-00001a40: 6465 5f73 6574 7469 6e67 732e 656e 6162  de_settings.enab
-00001a50: 6c65 5f61 7420 3d20 656e 6162 6c65 5f61  le_at = enable_a
-00001a60: 740a 2020 2020 2020 2020 2020 2020 6966  t.            if
-00001a70: 2064 7572 6174 696f 6e20 6973 206e 6f74   duration is not
-00001a80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00001a90: 2020 2020 2020 2073 656c 662e 6c69 6768         self.ligh
-00001aa0: 745f 6465 7669 6365 5f73 6574 7469 6e67  t_device_setting
-00001ab0: 732e 7069 725f 6475 7261 7469 6f6e 203d  s.pir_duration =
-00001ac0: 2064 7572 6174 696f 6e0a 2020 2020 2020   duration.      
-00001ad0: 2020 2020 2020 6966 2073 656e 7369 7469        if sensiti
-00001ae0: 7669 7479 2069 7320 6e6f 7420 4e6f 6e65  vity is not None
-00001af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001b00: 2020 7365 6c66 2e6c 6967 6874 5f64 6576    self.light_dev
-00001b10: 6963 655f 7365 7474 696e 6773 2e70 6972  ice_settings.pir
-00001b20: 5f73 656e 7369 7469 7669 7479 203d 2050  _sensitivity = P
-00001b30: 6572 6365 6e74 496e 7428 7365 6e73 6974  ercentInt(sensit
-00001b40: 6976 6974 7929 0a0a 2020 2020 2020 2020  ivity)..        
-00001b50: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
-00001b60: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
-00001b70: 290a 0a0a 636c 6173 7320 4361 6d65 7261  )...class Camera
-00001b80: 4368 616e 6e65 6c28 5072 6f74 6563 7442  Channel(ProtectB
-00001b90: 6173 654f 626a 6563 7429 3a0a 2020 2020  aseObject):.    
-00001ba0: 6964 3a20 696e 7420 2023 2072 6561 6420  id: int  # read 
-00001bb0: 6f6e 6c79 0a20 2020 2076 6964 656f 5f69  only.    video_i
-00001bc0: 643a 2073 7472 2020 2320 7265 6164 206f  d: str  # read o
-00001bd0: 6e6c 790a 2020 2020 6e61 6d65 3a20 7374  nly.    name: st
-00001be0: 7220 2023 2072 6561 6420 6f6e 6c79 0a20  r  # read only. 
-00001bf0: 2020 2065 6e61 626c 6564 3a20 626f 6f6c     enabled: bool
-00001c00: 2020 2320 7265 6164 206f 6e6c 790a 2020    # read only.  
-00001c10: 2020 6973 5f72 7473 705f 656e 6162 6c65    is_rtsp_enable
-00001c20: 643a 2062 6f6f 6c0a 2020 2020 7274 7370  d: bool.    rtsp
-00001c30: 5f61 6c69 6173 3a20 4f70 7469 6f6e 616c  _alias: Optional
-00001c40: 5b73 7472 5d20 2023 2072 6561 6420 6f6e  [str]  # read on
-00001c50: 6c79 0a20 2020 2077 6964 7468 3a20 696e  ly.    width: in
-00001c60: 740a 2020 2020 6865 6967 6874 3a20 696e  t.    height: in
-00001c70: 740a 2020 2020 6670 733a 2069 6e74 0a20  t.    fps: int. 
-00001c80: 2020 2062 6974 7261 7465 3a20 696e 740a     bitrate: int.
-00001c90: 2020 2020 6d69 6e5f 6269 7472 6174 653a      min_bitrate:
-00001ca0: 2069 6e74 2020 2320 7265 6164 206f 6e6c   int  # read onl
-00001cb0: 790a 2020 2020 6d61 785f 6269 7472 6174  y.    max_bitrat
-00001cc0: 653a 2069 6e74 2020 2320 7265 6164 206f  e: int  # read o
-00001cd0: 6e6c 790a 2020 2020 6d69 6e5f 636c 6965  nly.    min_clie
-00001ce0: 6e74 5f61 6461 7074 6976 655f 6269 745f  nt_adaptive_bit_
-00001cf0: 7261 7465 3a20 4f70 7469 6f6e 616c 5b69  rate: Optional[i
-00001d00: 6e74 5d20 2023 2072 6561 6420 6f6e 6c79  nt]  # read only
-00001d10: 0a20 2020 206d 696e 5f6d 6f74 696f 6e5f  .    min_motion_
-00001d20: 6164 6170 7469 7665 5f62 6974 5f72 6174  adaptive_bit_rat
-00001d30: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-00001d40: 2020 2320 7265 6164 206f 6e6c 790a 2020    # read only.  
-00001d50: 2020 6670 735f 7661 6c75 6573 3a20 6c69    fps_values: li
-00001d60: 7374 5b69 6e74 5d20 2023 2072 6561 6420  st[int]  # read 
-00001d70: 6f6e 6c79 0a20 2020 2069 6472 5f69 6e74  only.    idr_int
-00001d80: 6572 7661 6c3a 2069 6e74 0a20 2020 2023  erval: int.    #
-00001d90: 2033 2e30 2e32 322b 0a20 2020 2061 7574   3.0.22+.    aut
-00001da0: 6f5f 6269 7472 6174 653a 204f 7074 696f  o_bitrate: Optio
-00001db0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00001dc0: 0a20 2020 2061 7574 6f5f 6670 733a 204f  .    auto_fps: O
-00001dd0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00001de0: 4e6f 6e65 0a0a 2020 2020 5f72 7473 705f  None..    _rtsp_
-00001df0: 7572 6c3a 204f 7074 696f 6e61 6c5b 7374  url: Optional[st
-00001e00: 725d 203d 2050 7269 7661 7465 4174 7472  r] = PrivateAttr
-00001e10: 284e 6f6e 6529 0a20 2020 205f 7274 7370  (None).    _rtsp
-00001e20: 735f 7572 6c3a 204f 7074 696f 6e61 6c5b  s_url: Optional[
-00001e30: 7374 725d 203d 2050 7269 7661 7465 4174  str] = PrivateAt
-00001e40: 7472 284e 6f6e 6529 0a0a 2020 2020 4070  tr(None)..    @p
-00001e50: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00001e60: 7274 7370 5f75 726c 2873 656c 6629 202d  rtsp_url(self) -
-00001e70: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
-00001e80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001e90: 7365 6c66 2e69 735f 7274 7370 5f65 6e61  self.is_rtsp_ena
-00001ea0: 626c 6564 206f 7220 7365 6c66 2e72 7473  bled or self.rts
-00001eb0: 705f 616c 6961 7320 6973 204e 6f6e 653a  p_alias is None:
-00001ec0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001ed0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-00001ee0: 2020 6966 2073 656c 662e 5f72 7473 705f    if self._rtsp_
-00001ef0: 7572 6c20 6973 206e 6f74 204e 6f6e 653a  url is not None:
-00001f00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001f10: 7572 6e20 7365 6c66 2e5f 7274 7370 5f75  urn self._rtsp_u
-00001f20: 726c 0a20 2020 2020 2020 2073 656c 662e  rl.        self.
-00001f30: 5f72 7473 705f 7572 6c20 3d20 6622 7274  _rtsp_url = f"rt
-00001f40: 7370 3a2f 2f7b 7365 6c66 2e61 7069 2e63  sp://{self.api.c
-00001f50: 6f6e 6e65 6374 696f 6e5f 686f 7374 7d3a  onnection_host}:
-00001f60: 7b73 656c 662e 6170 692e 626f 6f74 7374  {self.api.bootst
-00001f70: 7261 702e 6e76 722e 706f 7274 732e 7274  rap.nvr.ports.rt
-00001f80: 7370 7d2f 7b73 656c 662e 7274 7370 5f61  sp}/{self.rtsp_a
-00001f90: 6c69 6173 7d22 0a20 2020 2020 2020 2072  lias}".        r
-00001fa0: 6574 7572 6e20 7365 6c66 2e5f 7274 7370  eturn self._rtsp
-00001fb0: 5f75 726c 0a0a 2020 2020 4070 726f 7065  _url..    @prope
-00001fc0: 7274 790a 2020 2020 6465 6620 7274 7370  rty.    def rtsp
-00001fd0: 735f 7572 6c28 7365 6c66 2920 2d3e 204f  s_url(self) -> O
-00001fe0: 7074 696f 6e61 6c5b 7374 725d 3a0a 2020  ptional[str]:.  
-00001ff0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00002000: 662e 6973 5f72 7473 705f 656e 6162 6c65  f.is_rtsp_enable
-00002010: 6420 6f72 2073 656c 662e 7274 7370 5f61  d or self.rtsp_a
-00002020: 6c69 6173 2069 7320 4e6f 6e65 3a0a 2020  lias is None:.  
-00002030: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002040: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-00002050: 6620 7365 6c66 2e5f 7274 7370 735f 7572  f self._rtsps_ur
-00002060: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-00002070: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002080: 6e20 7365 6c66 2e5f 7274 7370 735f 7572  n self._rtsps_ur
-00002090: 6c0a 2020 2020 2020 2020 7365 6c66 2e5f  l.        self._
-000020a0: 7274 7370 735f 7572 6c20 3d20 6622 7274  rtsps_url = f"rt
-000020b0: 7370 733a 2f2f 7b73 656c 662e 6170 692e  sps://{self.api.
-000020c0: 636f 6e6e 6563 7469 6f6e 5f68 6f73 747d  connection_host}
-000020d0: 3a7b 7365 6c66 2e61 7069 2e62 6f6f 7473  :{self.api.boots
-000020e0: 7472 6170 2e6e 7672 2e70 6f72 7473 2e72  trap.nvr.ports.r
-000020f0: 7473 7073 7d2f 7b73 656c 662e 7274 7370  tsps}/{self.rtsp
-00002100: 5f61 6c69 6173 7d3f 656e 6162 6c65 5372  _alias}?enableSr
-00002110: 7470 220a 2020 2020 2020 2020 7265 7475  tp".        retu
-00002120: 726e 2073 656c 662e 5f72 7473 7073 5f75  rn self._rtsps_u
-00002130: 726c 0a0a 2020 2020 4070 726f 7065 7274  rl..    @propert
-00002140: 790a 2020 2020 6465 6620 6973 5f70 6163  y.    def is_pac
-00002150: 6b61 6765 2873 656c 6629 202d 3e20 626f  kage(self) -> bo
-00002160: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-00002170: 726e 2073 656c 662e 6670 7320 3c3d 2032  rn self.fps <= 2
-00002180: 0a0a 0a63 6c61 7373 2049 5350 5365 7474  ...class ISPSett
-00002190: 696e 6773 2850 726f 7465 6374 4261 7365  ings(ProtectBase
-000021a0: 4f62 6a65 6374 293a 0a20 2020 2061 655f  Object):.    ae_
-000021b0: 6d6f 6465 3a20 4175 746f 4578 706f 7375  mode: AutoExposu
-000021c0: 7265 4d6f 6465 0a20 2020 2069 725f 6c65  reMode.    ir_le
-000021d0: 645f 6d6f 6465 3a20 4952 4c45 444d 6f64  d_mode: IRLEDMod
-000021e0: 650a 2020 2020 6972 5f6c 6564 5f6c 6576  e.    ir_led_lev
-000021f0: 656c 3a20 5477 6f42 7974 6549 6e74 0a20  el: TwoByteInt. 
-00002200: 2020 2077 6472 3a20 5744 524c 6576 656c     wdr: WDRLevel
-00002210: 0a20 2020 2069 6372 5f73 656e 7369 7469  .    icr_sensiti
-00002220: 7669 7479 3a20 4943 5253 656e 7369 7469  vity: ICRSensiti
-00002230: 7669 7479 0a20 2020 2062 7269 6768 746e  vity.    brightn
-00002240: 6573 733a 2069 6e74 0a20 2020 2063 6f6e  ess: int.    con
-00002250: 7472 6173 743a 2069 6e74 0a20 2020 2068  trast: int.    h
-00002260: 7565 3a20 696e 740a 2020 2020 7361 7475  ue: int.    satu
-00002270: 7261 7469 6f6e 3a20 696e 740a 2020 2020  ration: int.    
-00002280: 7368 6172 706e 6573 733a 2069 6e74 0a20  sharpness: int. 
-00002290: 2020 2064 656e 6f69 7365 3a20 696e 740a     denoise: int.
-000022a0: 2020 2020 6973 5f66 6c69 7070 6564 5f76      is_flipped_v
-000022b0: 6572 7469 6361 6c3a 2062 6f6f 6c0a 2020  ertical: bool.  
-000022c0: 2020 6973 5f66 6c69 7070 6564 5f68 6f72    is_flipped_hor
-000022d0: 697a 6f6e 7461 6c3a 2062 6f6f 6c0a 2020  izontal: bool.  
-000022e0: 2020 6973 5f61 7574 6f5f 726f 7461 7465    is_auto_rotate
-000022f0: 5f65 6e61 626c 6564 3a20 626f 6f6c 0a20  _enabled: bool. 
-00002300: 2020 2069 735f 6c64 635f 656e 6162 6c65     is_ldc_enable
-00002310: 643a 2062 6f6f 6c0a 2020 2020 6973 5f33  d: bool.    is_3
-00002320: 646e 725f 656e 6162 6c65 643a 2062 6f6f  dnr_enabled: boo
-00002330: 6c0a 2020 2020 6973 5f65 7874 6572 6e61  l.    is_externa
-00002340: 6c5f 6972 5f65 6e61 626c 6564 3a20 626f  l_ir_enabled: bo
-00002350: 6f6c 0a20 2020 2069 735f 6167 6772 6573  ol.    is_aggres
-00002360: 7369 7665 5f61 6e74 695f 666c 6963 6b65  sive_anti_flicke
-00002370: 725f 656e 6162 6c65 643a 2062 6f6f 6c0a  r_enabled: bool.
-00002380: 2020 2020 6973 5f70 6175 7365 5f6d 6f74      is_pause_mot
-00002390: 696f 6e5f 656e 6162 6c65 643a 2062 6f6f  ion_enabled: boo
-000023a0: 6c0a 2020 2020 645f 7a6f 6f6d 5f63 656e  l.    d_zoom_cen
-000023b0: 7465 725f 783a 2069 6e74 0a20 2020 2064  ter_x: int.    d
-000023c0: 5f7a 6f6f 6d5f 6365 6e74 6572 5f79 3a20  _zoom_center_y: 
-000023d0: 696e 740a 2020 2020 645f 7a6f 6f6d 5f73  int.    d_zoom_s
-000023e0: 6361 6c65 3a20 696e 740a 2020 2020 645f  cale: int.    d_
-000023f0: 7a6f 6f6d 5f73 7472 6561 6d5f 6964 3a20  zoom_stream_id: 
-00002400: 696e 740a 2020 2020 666f 6375 735f 6d6f  int.    focus_mo
-00002410: 6465 3a20 4f70 7469 6f6e 616c 5b46 6f63  de: Optional[Foc
-00002420: 7573 4d6f 6465 5d20 3d20 4e6f 6e65 0a20  usMode] = None. 
-00002430: 2020 2066 6f63 7573 5f70 6f73 6974 696f     focus_positio
-00002440: 6e3a 2069 6e74 0a20 2020 2074 6f75 6368  n: int.    touch
-00002450: 5f66 6f63 7573 5f78 3a20 4f70 7469 6f6e  _focus_x: Option
-00002460: 616c 5b69 6e74 5d0a 2020 2020 746f 7563  al[int].    touc
-00002470: 685f 666f 6375 735f 793a 204f 7074 696f  h_focus_y: Optio
-00002480: 6e61 6c5b 696e 745d 0a20 2020 207a 6f6f  nal[int].    zoo
-00002490: 6d5f 706f 7369 7469 6f6e 3a20 5065 7263  m_position: Perc
-000024a0: 656e 7449 6e74 0a20 2020 206d 6f75 6e74  entInt.    mount
-000024b0: 5f70 6f73 6974 696f 6e3a 204f 7074 696f  _position: Optio
-000024c0: 6e61 6c5b 4d6f 756e 7450 6f73 6974 696f  nal[MountPositio
-000024d0: 6e5d 203d 204e 6f6e 650a 2020 2020 2320  n] = None.    # 
-000024e0: 7265 7175 6972 6573 2032 2e38 2e31 342b  requires 2.8.14+
-000024f0: 0a20 2020 2069 735f 636f 6c6f 725f 6e69  .    is_color_ni
-00002500: 6768 745f 7669 7369 6f6e 5f65 6e61 626c  ght_vision_enabl
-00002510: 6564 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ed: Optional[boo
-00002520: 6c5d 203d 204e 6f6e 650a 2020 2020 2320  l] = None.    # 
-00002530: 332e 302e 3232 2b0a 2020 2020 6864 725f  3.0.22+.    hdr_
-00002540: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b48  mode: Optional[H
-00002550: 4452 4d6f 6465 5d20 3d20 4e6f 6e65 0a20  DRMode] = None. 
-00002560: 2020 2069 6372 5f63 7573 746f 6d5f 7661     icr_custom_va
-00002570: 6c75 653a 204f 7074 696f 6e61 6c5b 4943  lue: Optional[IC
-00002580: 5243 7573 746f 6d56 616c 7565 5d20 3d20  RCustomValue] = 
-00002590: 4e6f 6e65 0a20 2020 2069 6372 5f73 7769  None.    icr_swi
-000025a0: 7463 685f 6d6f 6465 3a20 4f70 7469 6f6e  tch_mode: Option
-000025b0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-000025c0: 2020 2073 706f 746c 6967 6874 5f64 7572     spotlight_dur
-000025d0: 6174 696f 6e3a 204f 7074 696f 6e61 6c5b  ation: Optional[
-000025e0: 696e 745d 203d 204e 6f6e 650a 0a20 2020  int] = None..   
-000025f0: 2064 6566 2075 6e69 6669 5f64 6963 7428   def unifi_dict(
-00002600: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00002610: 2020 2020 2020 2064 6174 613a 204f 7074         data: Opt
-00002620: 696f 6e61 6c5b 6469 6374 5b73 7472 2c20  ional[dict[str, 
-00002630: 416e 795d 5d20 3d20 4e6f 6e65 2c0a 2020  Any]] = None,.  
-00002640: 2020 2020 2020 6578 636c 7564 653a 204f        exclude: O
-00002650: 7074 696f 6e61 6c5b 7365 745b 7374 725d  ptional[set[str]
-00002660: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
-00002670: 2d3e 2064 6963 745b 7374 722c 2041 6e79  -> dict[str, Any
-00002680: 5d3a 0a20 2020 2020 2020 2064 6174 6120  ]:.        data 
-00002690: 3d20 7375 7065 7228 292e 756e 6966 695f  = super().unifi_
-000026a0: 6469 6374 2864 6174 613d 6461 7461 2c20  dict(data=data, 
-000026b0: 6578 636c 7564 653d 6578 636c 7564 6529  exclude=exclude)
-000026c0: 0a0a 2020 2020 2020 2020 6966 2022 666f  ..        if "fo
-000026d0: 6375 734d 6f64 6522 2069 6e20 6461 7461  cusMode" in data
-000026e0: 2061 6e64 2064 6174 615b 2266 6f63 7573   and data["focus
-000026f0: 4d6f 6465 225d 2069 7320 4e6f 6e65 3a0a  Mode"] is None:.
-00002700: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00002710: 6461 7461 5b22 666f 6375 734d 6f64 6522  data["focusMode"
-00002720: 5d0a 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-00002730: 6e20 6461 7461 0a0a 0a63 6c61 7373 204f  n data...class O
-00002740: 5344 5365 7474 696e 6773 2850 726f 7465  SDSettings(Prote
-00002750: 6374 4261 7365 4f62 6a65 6374 293a 0a20  ctBaseObject):. 
-00002760: 2020 2023 204f 7665 726c 6179 2049 6e66     # Overlay Inf
-00002770: 6f72 6d61 7469 6f6e 0a20 2020 2069 735f  ormation.    is_
-00002780: 6e61 6d65 5f65 6e61 626c 6564 3a20 626f  name_enabled: bo
-00002790: 6f6c 0a20 2020 2069 735f 6461 7465 5f65  ol.    is_date_e
-000027a0: 6e61 626c 6564 3a20 626f 6f6c 0a20 2020  nabled: bool.   
-000027b0: 2069 735f 6c6f 676f 5f65 6e61 626c 6564   is_logo_enabled
-000027c0: 3a20 626f 6f6c 0a20 2020 2069 735f 6465  : bool.    is_de
-000027d0: 6275 675f 656e 6162 6c65 643a 2062 6f6f  bug_enabled: boo
-000027e0: 6c0a 0a0a 636c 6173 7320 4c45 4453 6574  l...class LEDSet
-000027f0: 7469 6e67 7328 5072 6f74 6563 7442 6173  tings(ProtectBas
-00002800: 654f 626a 6563 7429 3a0a 2020 2020 2320  eObject):.    # 
-00002810: 5374 6174 7573 204c 6967 6874 0a20 2020  Status Light.   
-00002820: 2069 735f 656e 6162 6c65 643a 2062 6f6f   is_enabled: boo
-00002830: 6c0a 2020 2020 626c 696e 6b5f 7261 7465  l.    blink_rate
-00002840: 3a20 696e 7420 2023 2069 6e20 6d69 6c6c  : int  # in mill
-00002850: 6973 6563 6f6e 6473 2062 6574 7765 6565  iseconds betweee
-00002860: 6e20 626c 696e 6b73 2c20 3020 3d20 736f  n blinks, 0 = so
-00002870: 6c69 640a 0a0a 636c 6173 7320 5370 6561  lid...class Spea
-00002880: 6b65 7253 6574 7469 6e67 7328 5072 6f74  kerSettings(Prot
-00002890: 6563 7442 6173 654f 626a 6563 7429 3a0a  ectBaseObject):.
-000028a0: 2020 2020 6973 5f65 6e61 626c 6564 3a20      is_enabled: 
-000028b0: 626f 6f6c 0a20 2020 2023 2053 7461 7475  bool.    # Statu
-000028c0: 7320 536f 756e 6473 0a20 2020 2061 7265  s Sounds.    are
-000028d0: 5f73 7973 7465 6d5f 736f 756e 6473 5f65  _system_sounds_e
-000028e0: 6e61 626c 6564 3a20 626f 6f6c 0a20 2020  nabled: bool.   
-000028f0: 2076 6f6c 756d 653a 2050 6572 6365 6e74   volume: Percent
-00002900: 496e 740a 0a0a 636c 6173 7320 5265 636f  Int...class Reco
-00002910: 7264 696e 6753 6574 7469 6e67 7328 5072  rdingSettings(Pr
-00002920: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
-00002930: 3a0a 2020 2020 2320 5365 636f 6e64 7320  :.    # Seconds 
-00002940: 746f 2072 6563 6f72 6420 6265 666f 7265  to record before
-00002950: 204d 6f74 696f 6e0a 2020 2020 7072 655f   Motion.    pre_
-00002960: 7061 6464 696e 673a 2074 696d 6564 656c  padding: timedel
-00002970: 7461 0a20 2020 2023 2053 6563 6f6e 6473  ta.    # Seconds
-00002980: 2074 6f20 7265 636f 7264 2061 6674 6572   to record after
-00002990: 204d 6f74 696f 6e0a 2020 2020 706f 7374   Motion.    post
-000029a0: 5f70 6164 6469 6e67 3a20 7469 6d65 6465  _padding: timede
-000029b0: 6c74 610a 2020 2020 2320 5365 636f 6e64  lta.    # Second
-000029c0: 7320 6f66 204d 6f74 696f 6e20 4e65 6564  s of Motion Need
-000029d0: 6564 0a20 2020 206d 696e 5f6d 6f74 696f  ed.    min_motio
-000029e0: 6e5f 6576 656e 745f 7472 6967 6765 723a  n_event_trigger:
-000029f0: 2074 696d 6564 656c 7461 0a20 2020 2065   timedelta.    e
-00002a00: 6e64 5f6d 6f74 696f 6e5f 6576 656e 745f  nd_motion_event_
-00002a10: 6465 6c61 793a 2074 696d 6564 656c 7461  delay: timedelta
-00002a20: 0a20 2020 2073 7570 7072 6573 735f 696c  .    suppress_il
-00002a30: 6c75 6d69 6e61 7469 6f6e 5f73 7572 6765  lumination_surge
-00002a40: 3a20 626f 6f6c 0a20 2020 2023 2048 6967  : bool.    # Hig
-00002a50: 6820 4672 616d 6520 5261 7465 204d 6f64  h Frame Rate Mod
-00002a60: 650a 2020 2020 6d6f 6465 3a20 5265 636f  e.    mode: Reco
-00002a70: 7264 696e 674d 6f64 650a 2020 2020 6765  rdingMode.    ge
-00002a80: 6f66 656e 6369 6e67 3a20 4765 6f66 656e  ofencing: Geofen
-00002a90: 6369 6e67 5365 7474 696e 670a 2020 2020  cingSetting.    
-00002aa0: 6d6f 7469 6f6e 5f61 6c67 6f72 6974 686d  motion_algorithm
-00002ab0: 3a20 4d6f 7469 6f6e 416c 676f 7269 7468  : MotionAlgorith
-00002ac0: 6d0a 2020 2020 656e 6162 6c65 5f6d 6f74  m.    enable_mot
-00002ad0: 696f 6e5f 6465 7465 6374 696f 6e3a 204f  ion_detection: O
-00002ae0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00002af0: 4e6f 6e65 0a20 2020 2075 7365 5f6e 6577  None.    use_new
-00002b00: 5f6d 6f74 696f 6e5f 616c 676f 7269 7468  _motion_algorith
-00002b10: 6d3a 2062 6f6f 6c0a 2020 2020 2320 7265  m: bool.    # re
-00002b20: 7175 6972 6573 2032 2e39 2e32 302b 0a20  quires 2.9.20+. 
-00002b30: 2020 2069 6e5f 7363 6865 6475 6c65 5f6d     in_schedule_m
-00002b40: 6f64 653a 204f 7074 696f 6e61 6c5b 7374  ode: Optional[st
-00002b50: 725d 203d 204e 6f6e 650a 2020 2020 6f75  r] = None.    ou
-00002b60: 745f 7363 6865 6475 6c65 5f6d 6f64 653a  t_schedule_mode:
-00002b70: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00002b80: 204e 6f6e 650a 2020 2020 2320 322e 3131   None.    # 2.11
-00002b90: 2e31 332b 0a20 2020 2072 6574 656e 7469  .13+.    retenti
-00002ba0: 6f6e 5f64 7572 6174 696f 6e3a 204f 7074  on_duration: Opt
-00002bb0: 696f 6e61 6c5b 6461 7465 7469 6d65 5d20  ional[datetime] 
-00002bc0: 3d20 4e6f 6e65 0a20 2020 2073 6d61 7274  = None.    smart
-00002bd0: 5f64 6574 6563 745f 706f 7374 5f70 6164  _detect_post_pad
-00002be0: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b74  ding: Optional[t
-00002bf0: 696d 6564 656c 7461 5d20 3d20 4e6f 6e65  imedelta] = None
-00002c00: 0a20 2020 2073 6d61 7274 5f64 6574 6563  .    smart_detec
-00002c10: 745f 7072 655f 7061 6464 696e 673a 204f  t_pre_padding: O
-00002c20: 7074 696f 6e61 6c5b 7469 6d65 6465 6c74  ptional[timedelt
-00002c30: 615d 203d 204e 6f6e 650a 0a20 2020 2040  a] = None..    @
-00002c40: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00002c50: 4063 6163 6865 0a20 2020 2064 6566 205f  @cache.    def _
-00002c60: 6765 745f 756e 6966 695f 7265 6d61 7073  get_unifi_remaps
-00002c70: 2863 6c73 2920 2d3e 2064 6963 745b 7374  (cls) -> dict[st
-00002c80: 722c 2073 7472 5d3a 0a20 2020 2020 2020  r, str]:.       
-00002c90: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00002ca0: 2020 2020 2020 2a2a 7375 7065 7228 292e        **super().
-00002cb0: 5f67 6574 5f75 6e69 6669 5f72 656d 6170  _get_unifi_remap
-00002cc0: 7328 292c 0a20 2020 2020 2020 2020 2020  s(),.           
-00002cd0: 2022 7265 7465 6e74 696f 6e44 7572 6174   "retentionDurat
-00002ce0: 696f 6e4d 7322 3a20 2272 6574 656e 7469  ionMs": "retenti
-00002cf0: 6f6e 4475 7261 7469 6f6e 222c 0a20 2020  onDuration",.   
-00002d00: 2020 2020 207d 0a0a 2020 2020 4063 6c61       }..    @cla
-00002d10: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00002d20: 2075 6e69 6669 5f64 6963 745f 746f 5f64   unifi_dict_to_d
-00002d30: 6963 7428 636c 732c 2064 6174 613a 2064  ict(cls, data: d
-00002d40: 6963 745b 7374 722c 2041 6e79 5d29 202d  ict[str, Any]) -
-00002d50: 3e20 6469 6374 5b73 7472 2c20 416e 795d  > dict[str, Any]
-00002d60: 3a0a 2020 2020 2020 2020 6966 2022 7072  :.        if "pr
-00002d70: 6550 6164 6469 6e67 5365 6373 2220 696e  ePaddingSecs" in
-00002d80: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00002d90: 2020 2064 6174 615b 2270 7265 5061 6464     data["prePadd
-00002da0: 696e 6722 5d20 3d20 7469 6d65 6465 6c74  ing"] = timedelt
-00002db0: 6128 7365 636f 6e64 733d 6461 7461 2e70  a(seconds=data.p
-00002dc0: 6f70 2822 7072 6550 6164 6469 6e67 5365  op("prePaddingSe
-00002dd0: 6373 2229 290a 2020 2020 2020 2020 6966  cs")).        if
-00002de0: 2022 706f 7374 5061 6464 696e 6753 6563   "postPaddingSec
-00002df0: 7322 2069 6e20 6461 7461 3a0a 2020 2020  s" in data:.    
-00002e00: 2020 2020 2020 2020 6461 7461 5b22 706f          data["po
-00002e10: 7374 5061 6464 696e 6722 5d20 3d20 7469  stPadding"] = ti
-00002e20: 6d65 6465 6c74 6128 7365 636f 6e64 733d  medelta(seconds=
-00002e30: 6461 7461 2e70 6f70 2822 706f 7374 5061  data.pop("postPa
-00002e40: 6464 696e 6753 6563 7322 2929 0a20 2020  ddingSecs")).   
-00002e50: 2020 2020 2069 6620 2273 6d61 7274 4465       if "smartDe
-00002e60: 7465 6374 5072 6550 6164 6469 6e67 5365  tectPrePaddingSe
-00002e70: 6373 2220 696e 2064 6174 613a 0a20 2020  cs" in data:.   
-00002e80: 2020 2020 2020 2020 2064 6174 615b 2273           data["s
-00002e90: 6d61 7274 4465 7465 6374 5072 6550 6164  martDetectPrePad
-00002ea0: 6469 6e67 225d 203d 2074 696d 6564 656c  ding"] = timedel
-00002eb0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
-00002ec0: 2020 2020 7365 636f 6e64 733d 6461 7461      seconds=data
-00002ed0: 2e70 6f70 2822 736d 6172 7444 6574 6563  .pop("smartDetec
-00002ee0: 7450 7265 5061 6464 696e 6753 6563 7322  tPrePaddingSecs"
-00002ef0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-00002f00: 0a20 2020 2020 2020 2069 6620 2273 6d61  .        if "sma
-00002f10: 7274 4465 7465 6374 506f 7374 5061 6464  rtDetectPostPadd
-00002f20: 696e 6753 6563 7322 2069 6e20 6461 7461  ingSecs" in data
-00002f30: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-00002f40: 7461 5b22 736d 6172 7444 6574 6563 7450  ta["smartDetectP
-00002f50: 6f73 7450 6164 6469 6e67 225d 203d 2074  ostPadding"] = t
-00002f60: 696d 6564 656c 7461 280a 2020 2020 2020  imedelta(.      
-00002f70: 2020 2020 2020 2020 2020 7365 636f 6e64            second
-00002f80: 733d 6461 7461 2e70 6f70 2822 736d 6172  s=data.pop("smar
-00002f90: 7444 6574 6563 7450 6f73 7450 6164 6469  tDetectPostPaddi
-00002fa0: 6e67 5365 6373 2229 2c0a 2020 2020 2020  ngSecs"),.      
-00002fb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002fc0: 6966 2022 6d69 6e4d 6f74 696f 6e45 7665  if "minMotionEve
-00002fd0: 6e74 5472 6967 6765 7222 2069 6e20 6461  ntTrigger" in da
-00002fe0: 7461 2061 6e64 206e 6f74 2069 7369 6e73  ta and not isins
-00002ff0: 7461 6e63 6528 0a20 2020 2020 2020 2020  tance(.         
-00003000: 2020 2064 6174 615b 226d 696e 4d6f 7469     data["minMoti
-00003010: 6f6e 4576 656e 7454 7269 6767 6572 225d  onEventTrigger"]
-00003020: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00003030: 6d65 6465 6c74 612c 0a20 2020 2020 2020  medelta,.       
-00003040: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00003050: 6461 7461 5b22 6d69 6e4d 6f74 696f 6e45  data["minMotionE
-00003060: 7665 6e74 5472 6967 6765 7222 5d20 3d20  ventTrigger"] = 
-00003070: 7469 6d65 6465 6c74 6128 0a20 2020 2020  timedelta(.     
-00003080: 2020 2020 2020 2020 2020 2073 6563 6f6e             secon
-00003090: 6473 3d64 6174 615b 226d 696e 4d6f 7469  ds=data["minMoti
-000030a0: 6f6e 4576 656e 7454 7269 6767 6572 225d  onEventTrigger"]
-000030b0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-000030c0: 2020 2020 2020 2020 6966 2022 656e 644d          if "endM
-000030d0: 6f74 696f 6e45 7665 6e74 4465 6c61 7922  otionEventDelay"
-000030e0: 2069 6e20 6461 7461 2061 6e64 206e 6f74   in data and not
-000030f0: 2069 7369 6e73 7461 6e63 6528 0a20 2020   isinstance(.   
-00003100: 2020 2020 2020 2020 2064 6174 615b 2265           data["e
-00003110: 6e64 4d6f 7469 6f6e 4576 656e 7444 656c  ndMotionEventDel
-00003120: 6179 225d 2c0a 2020 2020 2020 2020 2020  ay"],.          
-00003130: 2020 7469 6d65 6465 6c74 612c 0a20 2020    timedelta,.   
-00003140: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00003150: 2020 2020 6461 7461 5b22 656e 644d 6f74      data["endMot
-00003160: 696f 6e45 7665 6e74 4465 6c61 7922 5d20  ionEventDelay"] 
-00003170: 3d20 7469 6d65 6465 6c74 6128 7365 636f  = timedelta(seco
-00003180: 6e64 733d 6461 7461 5b22 656e 644d 6f74  nds=data["endMot
-00003190: 696f 6e45 7665 6e74 4465 6c61 7922 5d29  ionEventDelay"])
-000031a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000031b0: 2073 7570 6572 2829 2e75 6e69 6669 5f64   super().unifi_d
-000031c0: 6963 745f 746f 5f64 6963 7428 6461 7461  ict_to_dict(data
-000031d0: 290a 0a20 2020 2064 6566 2075 6e69 6669  )..    def unifi
-000031e0: 5f64 6963 7428 0a20 2020 2020 2020 2073  _dict(.        s
-000031f0: 656c 662c 0a20 2020 2020 2020 2064 6174  elf,.        dat
-00003200: 613a 204f 7074 696f 6e61 6c5b 6469 6374  a: Optional[dict
-00003210: 5b73 7472 2c20 416e 795d 5d20 3d20 4e6f  [str, Any]] = No
-00003220: 6e65 2c0a 2020 2020 2020 2020 6578 636c  ne,.        excl
-00003230: 7564 653a 204f 7074 696f 6e61 6c5b 7365  ude: Optional[se
-00003240: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  t[str]] = None,.
-00003250: 2020 2020 2920 2d3e 2064 6963 745b 7374      ) -> dict[st
-00003260: 722c 2041 6e79 5d3a 0a20 2020 2020 2020  r, Any]:.       
-00003270: 2064 6174 6120 3d20 7375 7065 7228 292e   data = super().
-00003280: 756e 6966 695f 6469 6374 2864 6174 613d  unifi_dict(data=
-00003290: 6461 7461 2c20 6578 636c 7564 653d 6578  data, exclude=ex
-000032a0: 636c 7564 6529 0a0a 2020 2020 2020 2020  clude)..        
-000032b0: 6966 2022 7072 6550 6164 6469 6e67 2220  if "prePadding" 
-000032c0: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
-000032d0: 2020 2020 2064 6174 615b 2270 7265 5061       data["prePa
-000032e0: 6464 696e 6753 6563 7322 5d20 3d20 6461  ddingSecs"] = da
-000032f0: 7461 2e70 6f70 2822 7072 6550 6164 6469  ta.pop("prePaddi
-00003300: 6e67 2229 202f 2f20 3130 3030 0a20 2020  ng") // 1000.   
-00003310: 2020 2020 2069 6620 2270 6f73 7450 6164       if "postPad
-00003320: 6469 6e67 2220 696e 2064 6174 613a 0a20  ding" in data:. 
-00003330: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00003340: 2270 6f73 7450 6164 6469 6e67 5365 6373  "postPaddingSecs
-00003350: 225d 203d 2064 6174 612e 706f 7028 2270  "] = data.pop("p
-00003360: 6f73 7450 6164 6469 6e67 2229 202f 2f20  ostPadding") // 
-00003370: 3130 3030 0a20 2020 2020 2020 2069 6620  1000.        if 
-00003380: 280a 2020 2020 2020 2020 2020 2020 2273  (.            "s
-00003390: 6d61 7274 4465 7465 6374 5072 6550 6164  martDetectPrePad
-000033a0: 6469 6e67 2220 696e 2064 6174 610a 2020  ding" in data.  
-000033b0: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-000033c0: 7461 5b22 736d 6172 7444 6574 6563 7450  ta["smartDetectP
-000033d0: 7265 5061 6464 696e 6722 5d20 6973 206e  rePadding"] is n
-000033e0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-000033f0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00003400: 6174 615b 2273 6d61 7274 4465 7465 6374  ata["smartDetect
-00003410: 5072 6550 6164 6469 6e67 5365 6373 225d  PrePaddingSecs"]
-00003420: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00003430: 2020 2020 2064 6174 612e 706f 7028 2273       data.pop("s
-00003440: 6d61 7274 4465 7465 6374 5072 6550 6164  martDetectPrePad
-00003450: 6469 6e67 2229 202f 2f20 3130 3030 0a20  ding") // 1000. 
-00003460: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00003470: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00003480: 2020 2020 2020 2273 6d61 7274 4465 7465        "smartDete
-00003490: 6374 506f 7374 5061 6464 696e 6722 2069  ctPostPadding" i
-000034a0: 6e20 6461 7461 0a20 2020 2020 2020 2020  n data.         
-000034b0: 2020 2061 6e64 2064 6174 615b 2273 6d61     and data["sma
-000034c0: 7274 4465 7465 6374 506f 7374 5061 6464  rtDetectPostPadd
-000034d0: 696e 6722 5d20 6973 206e 6f74 204e 6f6e  ing"] is not Non
-000034e0: 650a 2020 2020 2020 2020 293a 0a20 2020  e.        ):.   
-000034f0: 2020 2020 2020 2020 2064 6174 615b 2273           data["s
-00003500: 6d61 7274 4465 7465 6374 506f 7374 5061  martDetectPostPa
-00003510: 6464 696e 6753 6563 7322 5d20 3d20 280a  ddingSecs"] = (.
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 6461 7461 2e70 6f70 2822 736d 6172 7444  data.pop("smartD
-00003540: 6574 6563 7450 6f73 7450 6164 6469 6e67  etectPostPadding
-00003550: 2229 202f 2f20 3130 3030 0a20 2020 2020  ") // 1000.     
-00003560: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00003570: 2069 6620 226d 696e 4d6f 7469 6f6e 4576   if "minMotionEv
-00003580: 656e 7454 7269 6767 6572 2220 696e 2064  entTrigger" in d
-00003590: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-000035a0: 2064 6174 615b 226d 696e 4d6f 7469 6f6e   data["minMotion
-000035b0: 4576 656e 7454 7269 6767 6572 225d 203d  EventTrigger"] =
-000035c0: 2064 6174 612e 706f 7028 226d 696e 4d6f   data.pop("minMo
-000035d0: 7469 6f6e 4576 656e 7454 7269 6767 6572  tionEventTrigger
-000035e0: 2229 202f 2f20 3130 3030 0a20 2020 2020  ") // 1000.     
-000035f0: 2020 2069 6620 2265 6e64 4d6f 7469 6f6e     if "endMotion
-00003600: 4576 656e 7444 656c 6179 2220 696e 2064  EventDelay" in d
-00003610: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00003620: 2064 6174 615b 2265 6e64 4d6f 7469 6f6e   data["endMotion
-00003630: 4576 656e 7444 656c 6179 225d 203d 2064  EventDelay"] = d
-00003640: 6174 612e 706f 7028 2265 6e64 4d6f 7469  ata.pop("endMoti
-00003650: 6f6e 4576 656e 7444 656c 6179 2229 202f  onEventDelay") /
-00003660: 2f20 3130 3030 0a0a 2020 2020 2020 2020  / 1000..        
-00003670: 7265 7475 726e 2064 6174 610a 0a0a 636c  return data...cl
-00003680: 6173 7320 536d 6172 7444 6574 6563 7453  ass SmartDetectS
-00003690: 6574 7469 6e67 7328 5072 6f74 6563 7442  ettings(ProtectB
-000036a0: 6173 654f 626a 6563 7429 3a0a 2020 2020  aseObject):.    
-000036b0: 6f62 6a65 6374 5f74 7970 6573 3a20 6c69  object_types: li
-000036c0: 7374 5b53 6d61 7274 4465 7465 6374 4f62  st[SmartDetectOb
-000036d0: 6a65 6374 5479 7065 5d0a 2020 2020 6175  jectType].    au
-000036e0: 6469 6f5f 7479 7065 733a 204f 7074 696f  dio_types: Optio
-000036f0: 6e61 6c5b 6c69 7374 5b53 6d61 7274 4465  nal[list[SmartDe
-00003700: 7465 6374 4175 6469 6f54 7970 655d 5d20  tectAudioType]] 
-00003710: 3d20 4e6f 6e65 0a20 2020 2023 2072 6571  = None.    # req
-00003720: 7569 7265 7320 322e 382e 3232 2b0a 2020  uires 2.8.22+.  
-00003730: 2020 6175 746f 5f74 7261 636b 696e 675f    auto_tracking_
-00003740: 6f62 6a65 6374 5f74 7970 6573 3a20 4f70  object_types: Op
-00003750: 7469 6f6e 616c 5b6c 6973 745b 536d 6172  tional[list[Smar
-00003760: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-00003770: 655d 5d20 3d20 4e6f 6e65 0a0a 2020 2020  e]] = None..    
-00003780: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00003790: 2064 6566 2075 6e69 6669 5f64 6963 745f   def unifi_dict_
-000037a0: 746f 5f64 6963 7428 636c 732c 2064 6174  to_dict(cls, dat
-000037b0: 613a 2064 6963 745b 7374 722c 2041 6e79  a: dict[str, Any
-000037c0: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
-000037d0: 416e 795d 3a0a 2020 2020 2020 2020 6966  Any]:.        if
-000037e0: 2022 6f62 6a65 6374 5479 7065 7322 2069   "objectTypes" i
-000037f0: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
-00003800: 2020 2020 6461 7461 5b22 6f62 6a65 6374      data["object
-00003810: 5479 7065 7322 5d20 3d20 636f 6e76 6572  Types"] = conver
-00003820: 745f 736d 6172 745f 7479 7065 7328 6461  t_smart_types(da
-00003830: 7461 2e70 6f70 2822 6f62 6a65 6374 5479  ta.pop("objectTy
-00003840: 7065 7322 2929 0a20 2020 2020 2020 2069  pes")).        i
-00003850: 6620 2261 7564 696f 5479 7065 7322 2069  f "audioTypes" i
-00003860: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
-00003870: 2020 2020 6461 7461 5b22 6175 6469 6f54      data["audioT
-00003880: 7970 6573 225d 203d 2063 6f6e 7665 7274  ypes"] = convert
-00003890: 5f73 6d61 7274 5f61 7564 696f 5f74 7970  _smart_audio_typ
-000038a0: 6573 2864 6174 612e 706f 7028 2261 7564  es(data.pop("aud
-000038b0: 696f 5479 7065 7322 2929 0a20 2020 2020  ioTypes")).     
-000038c0: 2020 2069 6620 2261 7574 6f54 7261 636b     if "autoTrack
-000038d0: 696e 674f 626a 6563 7454 7970 6573 2220  ingObjectTypes" 
-000038e0: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
-000038f0: 2020 2020 2064 6174 615b 2261 7574 6f54       data["autoT
-00003900: 7261 636b 696e 674f 626a 6563 7454 7970  rackingObjectTyp
-00003910: 6573 225d 203d 2063 6f6e 7665 7274 5f73  es"] = convert_s
-00003920: 6d61 7274 5f74 7970 6573 280a 2020 2020  mart_types(.    
-00003930: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00003940: 2e70 6f70 2822 6175 746f 5472 6163 6b69  .pop("autoTracki
-00003950: 6e67 4f62 6a65 6374 5479 7065 7322 292c  ngObjectTypes"),
-00003960: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00003970: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003980: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
-00003990: 745f 746f 5f64 6963 7428 6461 7461 290a  t_to_dict(data).
-000039a0: 0a0a 636c 6173 7320 4c43 444d 6573 7361  ..class LCDMessa
-000039b0: 6765 2850 726f 7465 6374 4261 7365 4f62  ge(ProtectBaseOb
-000039c0: 6a65 6374 293a 0a20 2020 2074 7970 653a  ject):.    type:
-000039d0: 2044 6f6f 7262 656c 6c4d 6573 7361 6765   DoorbellMessage
-000039e0: 5479 7065 0a20 2020 2074 6578 743a 2073  Type.    text: s
-000039f0: 7472 0a20 2020 2072 6573 6574 5f61 743a  tr.    reset_at:
-00003a00: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00003a10: 6d65 5d20 3d20 4e6f 6e65 0a0a 2020 2020  me] = None..    
-00003a20: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00003a30: 2064 6566 2075 6e69 6669 5f64 6963 745f   def unifi_dict_
-00003a40: 746f 5f64 6963 7428 636c 732c 2064 6174  to_dict(cls, dat
-00003a50: 613a 2064 6963 745b 7374 722c 2041 6e79  a: dict[str, Any
-00003a60: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
-00003a70: 416e 795d 3a0a 2020 2020 2020 2020 6966  Any]:.        if
-00003a80: 2022 7265 7365 7441 7422 2069 6e20 6461   "resetAt" in da
-00003a90: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00003aa0: 6461 7461 5b22 7265 7365 7441 7422 5d20  data["resetAt"] 
-00003ab0: 3d20 7072 6f63 6573 735f 6461 7465 7469  = process_dateti
-00003ac0: 6d65 2864 6174 612c 2022 7265 7365 7441  me(data, "resetA
-00003ad0: 7422 290a 2020 2020 2020 2020 6966 2022  t").        if "
-00003ae0: 7465 7874 2220 696e 2064 6174 613a 0a20  text" in data:. 
-00003af0: 2020 2020 2020 2020 2020 2023 2055 6e69             # Uni
-00003b00: 4669 2050 726f 7465 6374 2062 7567 3a20  Fi Protect bug: 
-00003b10: 736f 6d65 2074 696d 6573 204c 4344 206d  some times LCD m
-00003b20: 6573 7361 6765 7320 6361 6e20 6765 7420  essages can get 
-00003b30: 696e 746f 2061 2062 6164 2073 7461 7465  into a bad state
-00003b40: 2077 6865 7265 206d 6573 7361 6765 203d   where message =
-00003b50: 2044 4546 4155 4c54 204d 4553 5341 4745   DEFAULT MESSAGE
-00003b60: 2c20 6275 7420 6e6f 2074 7970 650a 2020  , but no type.  
-00003b70: 2020 2020 2020 2020 2020 6966 2022 7479            if "ty
-00003b80: 7065 2220 6e6f 7420 696e 2064 6174 613a  pe" not in data:
-00003b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ba0: 2064 6174 615b 2274 7970 6522 5d20 3d20   data["type"] = 
-00003bb0: 446f 6f72 6265 6c6c 4d65 7373 6167 6554  DoorbellMessageT
-00003bc0: 7970 652e 4355 5354 4f4d 5f4d 4553 5341  ype.CUSTOM_MESSA
-00003bd0: 4745 2e76 616c 7565 0a0a 2020 2020 2020  GE.value..      
-00003be0: 2020 2020 2020 6461 7461 5b22 7465 7874        data["text
-00003bf0: 225d 203d 2063 6c73 2e5f 6669 785f 7465  "] = cls._fix_te
-00003c00: 7874 2864 6174 615b 2274 6578 7422 5d2c  xt(data["text"],
-00003c10: 2064 6174 615b 2274 7970 6522 5d29 0a0a   data["type"])..
-00003c20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003c30: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
-00003c40: 745f 746f 5f64 6963 7428 6461 7461 290a  t_to_dict(data).
-00003c50: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00003c60: 640a 2020 2020 6465 6620 5f66 6978 5f74  d.    def _fix_t
-00003c70: 6578 7428 636c 732c 2074 6578 743a 2073  ext(cls, text: s
-00003c80: 7472 2c20 7465 7874 5f74 7970 653a 204f  tr, text_type: O
-00003c90: 7074 696f 6e61 6c5b 7374 725d 2920 2d3e  ptional[str]) ->
-00003ca0: 2073 7472 3a0a 2020 2020 2020 2020 6966   str:.        if
-00003cb0: 2074 6578 745f 7479 7065 2069 7320 4e6f   text_type is No
-00003cc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003cd0: 7465 7874 5f74 7970 6520 3d20 636c 732e  text_type = cls.
-00003ce0: 7479 7065 2e76 616c 7565 0a0a 2020 2020  type.value..    
-00003cf0: 2020 2020 6966 2074 6578 745f 7479 7065      if text_type
-00003d00: 2021 3d20 446f 6f72 6265 6c6c 4d65 7373   != DoorbellMess
-00003d10: 6167 6554 7970 652e 4355 5354 4f4d 5f4d  ageType.CUSTOM_M
-00003d20: 4553 5341 4745 2e76 616c 7565 3a0a 2020  ESSAGE.value:.  
-00003d30: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00003d40: 2074 6578 745f 7479 7065 2e72 6570 6c61   text_type.repla
-00003d50: 6365 2822 5f22 2c20 2220 2229 0a0a 2020  ce("_", " ")..  
-00003d60: 2020 2020 2020 7265 7475 726e 2074 6578        return tex
-00003d70: 740a 0a20 2020 2064 6566 2075 6e69 6669  t..    def unifi
-00003d80: 5f64 6963 7428 0a20 2020 2020 2020 2073  _dict(.        s
-00003d90: 656c 662c 0a20 2020 2020 2020 2064 6174  elf,.        dat
-00003da0: 613a 204f 7074 696f 6e61 6c5b 6469 6374  a: Optional[dict
-00003db0: 5b73 7472 2c20 416e 795d 5d20 3d20 4e6f  [str, Any]] = No
-00003dc0: 6e65 2c0a 2020 2020 2020 2020 6578 636c  ne,.        excl
-00003dd0: 7564 653a 204f 7074 696f 6e61 6c5b 7365  ude: Optional[se
-00003de0: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  t[str]] = None,.
-00003df0: 2020 2020 2920 2d3e 2064 6963 745b 7374      ) -> dict[st
-00003e00: 722c 2041 6e79 5d3a 0a20 2020 2020 2020  r, Any]:.       
-00003e10: 2064 6174 6120 3d20 7375 7065 7228 292e   data = super().
-00003e20: 756e 6966 695f 6469 6374 2864 6174 613d  unifi_dict(data=
-00003e30: 6461 7461 2c20 6578 636c 7564 653d 6578  data, exclude=ex
-00003e40: 636c 7564 6529 0a0a 2020 2020 2020 2020  clude)..        
-00003e50: 6966 2022 7465 7874 2220 696e 2064 6174  if "text" in dat
-00003e60: 613a 0a20 2020 2020 2020 2020 2020 2074  a:.            t
-00003e70: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00003e80: 2020 2020 6d73 675f 7479 7065 203d 2073      msg_type = s
-00003e90: 656c 662e 7479 7065 2e76 616c 7565 0a20  elf.type.value. 
-00003ea0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00003eb0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
-00003ec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ed0: 2020 6d73 675f 7479 7065 203d 204e 6f6e    msg_type = Non
-00003ee0: 650a 0a20 2020 2020 2020 2020 2020 2064  e..            d
-00003ef0: 6174 615b 2274 6578 7422 5d20 3d20 7365  ata["text"] = se
-00003f00: 6c66 2e5f 6669 785f 7465 7874 2864 6174  lf._fix_text(dat
-00003f10: 615b 2274 6578 7422 5d2c 2064 6174 612e  a["text"], data.
-00003f20: 6765 7428 2274 7970 6522 2c20 6d73 675f  get("type", msg_
-00003f30: 7479 7065 2929 0a20 2020 2020 2020 2069  type)).        i
-00003f40: 6620 2272 6573 6574 4174 2220 696e 2064  f "resetAt" in d
-00003f50: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00003f60: 2064 6174 615b 2272 6573 6574 4174 225d   data["resetAt"]
-00003f70: 203d 2074 6f5f 6a73 5f74 696d 6528 6461   = to_js_time(da
-00003f80: 7461 5b22 7265 7365 7441 7422 5d29 0a0a  ta["resetAt"])..
-00003f90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00003fa0: 6174 610a 0a0a 636c 6173 7320 5461 6c6b  ata...class Talk
-00003fb0: 6261 636b 5365 7474 696e 6773 2850 726f  backSettings(Pro
-00003fc0: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
-00003fd0: 0a20 2020 2074 7970 655f 666d 743a 2041  .    type_fmt: A
-00003fe0: 7564 696f 436f 6465 6373 0a20 2020 2074  udioCodecs.    t
-00003ff0: 7970 655f 696e 3a20 7374 720a 2020 2020  ype_in: str.    
-00004000: 6269 6e64 5f61 6464 723a 2049 5076 3441  bind_addr: IPv4A
-00004010: 6464 7265 7373 0a20 2020 2062 696e 645f  ddress.    bind_
-00004020: 706f 7274 3a20 696e 740a 2020 2020 6669  port: int.    fi
-00004030: 6c74 6572 5f61 6464 723a 204f 7074 696f  lter_addr: Optio
-00004040: 6e61 6c5b 7374 725d 2020 2320 6361 6e20  nal[str]  # can 
-00004050: 6265 2075 7365 6420 746f 2072 6573 7472  be used to restr
-00004060: 6963 7420 7365 6e64 6572 2061 6464 7265  ict sender addre
-00004070: 7373 0a20 2020 2066 696c 7465 725f 706f  ss.    filter_po
-00004080: 7274 3a20 4f70 7469 6f6e 616c 5b69 6e74  rt: Optional[int
-00004090: 5d20 2023 2063 616e 2062 6520 7573 6564  ]  # can be used
-000040a0: 2074 6f20 7265 7374 7269 6374 2073 656e   to restrict sen
-000040b0: 6465 7220 706f 7274 0a20 2020 2063 6861  der port.    cha
-000040c0: 6e6e 656c 733a 2069 6e74 2020 2320 3120  nnels: int  # 1 
-000040d0: 6f72 2032 0a20 2020 2073 616d 706c 696e  or 2.    samplin
-000040e0: 675f 7261 7465 3a20 696e 7420 2023 2038  g_rate: int  # 8
-000040f0: 3030 302c 2031 3130 3235 2c20 3232 3035  000, 11025, 2205
-00004100: 302c 2034 3431 3030 2c20 3438 3030 300a  0, 44100, 48000.
-00004110: 2020 2020 6269 7473 5f70 6572 5f73 616d      bits_per_sam
-00004120: 706c 653a 2069 6e74 0a20 2020 2071 7561  ple: int.    qua
-00004130: 6c69 7479 3a20 5065 7263 656e 7449 6e74  lity: PercentInt
-00004140: 2020 2320 6f6e 6c79 2066 6f72 2076 6f72    # only for vor
-00004150: 6269 730a 0a0a 636c 6173 7320 5769 6669  bis...class Wifi
-00004160: 5374 6174 7328 5072 6f74 6563 7442 6173  Stats(ProtectBas
-00004170: 654f 626a 6563 7429 3a0a 2020 2020 6368  eObject):.    ch
-00004180: 616e 6e65 6c3a 204f 7074 696f 6e61 6c5b  annel: Optional[
-00004190: 696e 745d 0a20 2020 2066 7265 7175 656e  int].    frequen
-000041a0: 6379 3a20 4f70 7469 6f6e 616c 5b69 6e74  cy: Optional[int
-000041b0: 5d0a 2020 2020 6c69 6e6b 5f73 7065 6564  ].    link_speed
-000041c0: 5f6d 6270 733a 204f 7074 696f 6e61 6c5b  _mbps: Optional[
-000041d0: 7374 725d 0a20 2020 2073 6967 6e61 6c5f  str].    signal_
-000041e0: 7175 616c 6974 793a 2050 6572 6365 6e74  quality: Percent
-000041f0: 496e 740a 2020 2020 7369 676e 616c 5f73  Int.    signal_s
-00004200: 7472 656e 6774 683a 2069 6e74 0a0a 0a63  trength: int...c
-00004210: 6c61 7373 2056 6964 656f 5374 6174 7328  lass VideoStats(
-00004220: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
-00004230: 7429 3a0a 2020 2020 7265 636f 7264 696e  t):.    recordin
-00004240: 675f 7374 6172 743a 204f 7074 696f 6e61  g_start: Optiona
-00004250: 6c5b 6461 7465 7469 6d65 5d0a 2020 2020  l[datetime].    
-00004260: 7265 636f 7264 696e 675f 656e 643a 204f  recording_end: O
-00004270: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
-00004280: 5d0a 2020 2020 7265 636f 7264 696e 675f  ].    recording_
-00004290: 7374 6172 745f 6c71 3a20 4f70 7469 6f6e  start_lq: Option
-000042a0: 616c 5b64 6174 6574 696d 655d 0a20 2020  al[datetime].   
-000042b0: 2072 6563 6f72 6469 6e67 5f65 6e64 5f6c   recording_end_l
-000042c0: 713a 204f 7074 696f 6e61 6c5b 6461 7465  q: Optional[date
-000042d0: 7469 6d65 5d0a 2020 2020 7469 6d65 6c61  time].    timela
-000042e0: 7073 655f 7374 6172 743a 204f 7074 696f  pse_start: Optio
-000042f0: 6e61 6c5b 6461 7465 7469 6d65 5d0a 2020  nal[datetime].  
-00004300: 2020 7469 6d65 6c61 7073 655f 656e 643a    timelapse_end:
-00004310: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00004320: 6d65 5d0a 2020 2020 7469 6d65 6c61 7073  me].    timelaps
-00004330: 655f 7374 6172 745f 6c71 3a20 4f70 7469  e_start_lq: Opti
-00004340: 6f6e 616c 5b64 6174 6574 696d 655d 0a20  onal[datetime]. 
-00004350: 2020 2074 696d 656c 6170 7365 5f65 6e64     timelapse_end
-00004360: 5f6c 713a 204f 7074 696f 6e61 6c5b 6461  _lq: Optional[da
-00004370: 7465 7469 6d65 5d0a 0a20 2020 2040 636c  tetime]..    @cl
-00004380: 6173 736d 6574 686f 640a 2020 2020 4063  assmethod.    @c
-00004390: 6163 6865 0a20 2020 2064 6566 205f 6765  ache.    def _ge
-000043a0: 745f 756e 6966 695f 7265 6d61 7073 2863  t_unifi_remaps(c
-000043b0: 6c73 2920 2d3e 2064 6963 745b 7374 722c  ls) -> dict[str,
-000043c0: 2073 7472 5d3a 0a20 2020 2020 2020 2072   str]:.        r
-000043d0: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
-000043e0: 2020 2020 2a2a 7375 7065 7228 292e 5f67      **super()._g
-000043f0: 6574 5f75 6e69 6669 5f72 656d 6170 7328  et_unifi_remaps(
-00004400: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00004410: 7265 636f 7264 696e 6753 7461 7274 4c51  recordingStartLQ
-00004420: 223a 2022 7265 636f 7264 696e 6753 7461  ": "recordingSta
-00004430: 7274 4c71 222c 0a20 2020 2020 2020 2020  rtLq",.         
-00004440: 2020 2022 7265 636f 7264 696e 6745 6e64     "recordingEnd
-00004450: 4c51 223a 2022 7265 636f 7264 696e 6745  LQ": "recordingE
-00004460: 6e64 4c71 222c 0a20 2020 2020 2020 2020  ndLq",.         
-00004470: 2020 2022 7469 6d65 6c61 7073 6553 7461     "timelapseSta
-00004480: 7274 4c51 223a 2022 7469 6d65 6c61 7073  rtLQ": "timelaps
-00004490: 6553 7461 7274 4c71 222c 0a20 2020 2020  eStartLq",.     
-000044a0: 2020 2020 2020 2022 7469 6d65 6c61 7073         "timelaps
-000044b0: 6545 6e64 4c51 223a 2022 7469 6d65 6c61  eEndLQ": "timela
-000044c0: 7073 6545 6e64 4c71 222c 0a20 2020 2020  pseEndLq",.     
-000044d0: 2020 207d 0a0a 2020 2020 4063 6c61 7373     }..    @class
-000044e0: 6d65 7468 6f64 0a20 2020 2064 6566 2075  method.    def u
-000044f0: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
-00004500: 7428 636c 732c 2064 6174 613a 2064 6963  t(cls, data: dic
-00004510: 745b 7374 722c 2041 6e79 5d29 202d 3e20  t[str, Any]) -> 
-00004520: 6469 6374 5b73 7472 2c20 416e 795d 3a0a  dict[str, Any]:.
-00004530: 2020 2020 2020 2020 6966 2022 7265 636f          if "reco
-00004540: 7264 696e 6753 7461 7274 2220 696e 2064  rdingStart" in d
-00004550: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00004560: 2064 6174 615b 2272 6563 6f72 6469 6e67   data["recording
-00004570: 5374 6172 7422 5d20 3d20 7072 6f63 6573  Start"] = proces
-00004580: 735f 6461 7465 7469 6d65 2864 6174 612c  s_datetime(data,
-00004590: 2022 7265 636f 7264 696e 6753 7461 7274   "recordingStart
-000045a0: 2229 0a20 2020 2020 2020 2069 6620 2272  ").        if "r
-000045b0: 6563 6f72 6469 6e67 456e 6422 2069 6e20  ecordingEnd" in 
-000045c0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-000045d0: 2020 6461 7461 5b22 7265 636f 7264 696e    data["recordin
-000045e0: 6745 6e64 225d 203d 2070 726f 6365 7373  gEnd"] = process
-000045f0: 5f64 6174 6574 696d 6528 6461 7461 2c20  _datetime(data, 
-00004600: 2272 6563 6f72 6469 6e67 456e 6422 290a  "recordingEnd").
-00004610: 2020 2020 2020 2020 6966 2022 7265 636f          if "reco
-00004620: 7264 696e 6753 7461 7274 4c51 2220 696e  rdingStartLQ" in
-00004630: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00004640: 2020 2064 6174 615b 2272 6563 6f72 6469     data["recordi
-00004650: 6e67 5374 6172 744c 5122 5d20 3d20 7072  ngStartLQ"] = pr
-00004660: 6f63 6573 735f 6461 7465 7469 6d65 2864  ocess_datetime(d
-00004670: 6174 612c 2022 7265 636f 7264 696e 6753  ata, "recordingS
-00004680: 7461 7274 4c51 2229 0a20 2020 2020 2020  tartLQ").       
-00004690: 2069 6620 2272 6563 6f72 6469 6e67 456e   if "recordingEn
-000046a0: 644c 5122 2069 6e20 6461 7461 3a0a 2020  dLQ" in data:.  
-000046b0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-000046c0: 7265 636f 7264 696e 6745 6e64 4c51 225d  recordingEndLQ"]
-000046d0: 203d 2070 726f 6365 7373 5f64 6174 6574   = process_datet
-000046e0: 696d 6528 6461 7461 2c20 2272 6563 6f72  ime(data, "recor
-000046f0: 6469 6e67 456e 644c 5122 290a 2020 2020  dingEndLQ").    
-00004700: 2020 2020 6966 2022 7469 6d65 6c61 7073      if "timelaps
-00004710: 6553 7461 7274 2220 696e 2064 6174 613a  eStart" in data:
-00004720: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00004730: 615b 2274 696d 656c 6170 7365 5374 6172  a["timelapseStar
-00004740: 7422 5d20 3d20 7072 6f63 6573 735f 6461  t"] = process_da
-00004750: 7465 7469 6d65 2864 6174 612c 2022 7469  tetime(data, "ti
-00004760: 6d65 6c61 7073 6553 7461 7274 2229 0a20  melapseStart"). 
-00004770: 2020 2020 2020 2069 6620 2274 696d 656c         if "timel
-00004780: 6170 7365 456e 6422 2069 6e20 6461 7461  apseEnd" in data
-00004790: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-000047a0: 7461 5b22 7469 6d65 6c61 7073 6545 6e64  ta["timelapseEnd
-000047b0: 225d 203d 2070 726f 6365 7373 5f64 6174  "] = process_dat
-000047c0: 6574 696d 6528 6461 7461 2c20 2274 696d  etime(data, "tim
-000047d0: 656c 6170 7365 456e 6422 290a 2020 2020  elapseEnd").    
-000047e0: 2020 2020 6966 2022 7469 6d65 6c61 7073      if "timelaps
-000047f0: 6553 7461 7274 4c51 2220 696e 2064 6174  eStartLQ" in dat
-00004800: 613a 0a20 2020 2020 2020 2020 2020 2064  a:.            d
-00004810: 6174 615b 2274 696d 656c 6170 7365 5374  ata["timelapseSt
-00004820: 6172 744c 5122 5d20 3d20 7072 6f63 6573  artLQ"] = proces
-00004830: 735f 6461 7465 7469 6d65 2864 6174 612c  s_datetime(data,
-00004840: 2022 7469 6d65 6c61 7073 6553 7461 7274   "timelapseStart
-00004850: 4c51 2229 0a20 2020 2020 2020 2069 6620  LQ").        if 
-00004860: 2274 696d 656c 6170 7365 456e 644c 5122  "timelapseEndLQ"
-00004870: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-00004880: 2020 2020 2020 6461 7461 5b22 7469 6d65        data["time
-00004890: 6c61 7073 6545 6e64 4c51 225d 203d 2070  lapseEndLQ"] = p
-000048a0: 726f 6365 7373 5f64 6174 6574 696d 6528  rocess_datetime(
-000048b0: 6461 7461 2c20 2274 696d 656c 6170 7365  data, "timelapse
-000048c0: 456e 644c 5122 290a 0a20 2020 2020 2020  EndLQ")..       
-000048d0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-000048e0: 756e 6966 695f 6469 6374 5f74 6f5f 6469  unifi_dict_to_di
-000048f0: 6374 2864 6174 6129 0a0a 0a63 6c61 7373  ct(data)...class
-00004900: 2053 746f 7261 6765 5374 6174 7328 5072   StorageStats(Pr
-00004910: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
-00004920: 3a0a 2020 2020 7573 6564 3a20 4f70 7469  :.    used: Opti
-00004930: 6f6e 616c 5b69 6e74 5d20 2023 2062 7974  onal[int]  # byt
-00004940: 6573 0a20 2020 2072 6174 653a 204f 7074  es.    rate: Opt
-00004950: 696f 6e61 6c5b 666c 6f61 745d 2020 2320  ional[float]  # 
-00004960: 6279 7465 7320 2f20 6d69 6c6c 6973 6563  bytes / millisec
-00004970: 6f6e 640a 0a20 2020 2040 7072 6f70 6572  ond..    @proper
-00004980: 7479 0a20 2020 2064 6566 2072 6174 655f  ty.    def rate_
-00004990: 7065 725f 7365 636f 6e64 2873 656c 6629  per_second(self)
-000049a0: 202d 3e20 4f70 7469 6f6e 616c 5b66 6c6f   -> Optional[flo
-000049b0: 6174 5d3a 0a20 2020 2020 2020 2069 6620  at]:.        if 
-000049c0: 7365 6c66 2e72 6174 6520 6973 204e 6f6e  self.rate is Non
-000049d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000049e0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-000049f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00004a00: 7261 7465 202a 2031 3030 300a 0a20 2020  rate * 1000..   
-00004a10: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00004a20: 2020 6465 6620 756e 6966 695f 6469 6374    def unifi_dict
-00004a30: 5f74 6f5f 6469 6374 2863 6c73 2c20 6461  _to_dict(cls, da
-00004a40: 7461 3a20 6469 6374 5b73 7472 2c20 416e  ta: dict[str, An
-00004a50: 795d 2920 2d3e 2064 6963 745b 7374 722c  y]) -> dict[str,
-00004a60: 2041 6e79 5d3a 0a20 2020 2020 2020 2069   Any]:.        i
-00004a70: 6620 2272 6174 6522 206e 6f74 2069 6e20  f "rate" not in 
-00004a80: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00004a90: 2020 6461 7461 5b22 7261 7465 225d 203d    data["rate"] =
-00004aa0: 204e 6f6e 650a 0a20 2020 2020 2020 2072   None..        r
-00004ab0: 6574 7572 6e20 7375 7065 7228 292e 756e  eturn super().un
-00004ac0: 6966 695f 6469 6374 5f74 6f5f 6469 6374  ifi_dict_to_dict
-00004ad0: 2864 6174 6129 0a0a 2020 2020 6465 6620  (data)..    def 
-00004ae0: 756e 6966 695f 6469 6374 280a 2020 2020  unifi_dict(.    
-00004af0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00004b00: 2020 6461 7461 3a20 4f70 7469 6f6e 616c    data: Optional
-00004b10: 5b64 6963 745b 7374 722c 2041 6e79 5d5d  [dict[str, Any]]
-00004b20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00004b30: 2065 7863 6c75 6465 3a20 4f70 7469 6f6e   exclude: Option
-00004b40: 616c 5b73 6574 5b73 7472 5d5d 203d 204e  al[set[str]] = N
-00004b50: 6f6e 652c 0a20 2020 2029 202d 3e20 6469  one,.    ) -> di
-00004b60: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
-00004b70: 2020 2020 2020 6461 7461 203d 2073 7570        data = sup
-00004b80: 6572 2829 2e75 6e69 6669 5f64 6963 7428  er().unifi_dict(
-00004b90: 6461 7461 3d64 6174 612c 2065 7863 6c75  data=data, exclu
-00004ba0: 6465 3d65 7863 6c75 6465 290a 0a20 2020  de=exclude)..   
-00004bb0: 2020 2020 2069 6620 2272 6174 6522 2069       if "rate" i
-00004bc0: 6e20 6461 7461 2061 6e64 2064 6174 615b  n data and data[
-00004bd0: 2272 6174 6522 5d20 6973 204e 6f6e 653a  "rate"] is None:
-00004be0: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00004bf0: 2064 6174 615b 2272 6174 6522 5d0a 0a20   data["rate"].. 
-00004c00: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00004c10: 7461 0a0a 0a63 6c61 7373 2043 616d 6572  ta...class Camer
-00004c20: 6153 7461 7473 2850 726f 7465 6374 4261  aStats(ProtectBa
-00004c30: 7365 4f62 6a65 6374 293a 0a20 2020 2072  seObject):.    r
-00004c40: 785f 6279 7465 733a 2069 6e74 0a20 2020  x_bytes: int.   
-00004c50: 2074 785f 6279 7465 733a 2069 6e74 0a20   tx_bytes: int. 
-00004c60: 2020 2077 6966 693a 2057 6966 6953 7461     wifi: WifiSta
-00004c70: 7473 0a20 2020 2076 6964 656f 3a20 5669  ts.    video: Vi
-00004c80: 6465 6f53 7461 7473 0a20 2020 2073 746f  deoStats.    sto
-00004c90: 7261 6765 3a20 4f70 7469 6f6e 616c 5b53  rage: Optional[S
-00004ca0: 746f 7261 6765 5374 6174 735d 0a20 2020  torageStats].   
-00004cb0: 2077 6966 695f 7175 616c 6974 793a 2050   wifi_quality: P
-00004cc0: 6572 6365 6e74 496e 740a 2020 2020 7769  ercentInt.    wi
-00004cd0: 6669 5f73 7472 656e 6774 683a 2069 6e74  fi_strength: int
-00004ce0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00004cf0: 6f64 0a20 2020 2064 6566 2075 6e69 6669  od.    def unifi
-00004d00: 5f64 6963 745f 746f 5f64 6963 7428 636c  _dict_to_dict(cl
-00004d10: 732c 2064 6174 613a 2064 6963 745b 7374  s, data: dict[st
-00004d20: 722c 2041 6e79 5d29 202d 3e20 6469 6374  r, Any]) -> dict
-00004d30: 5b73 7472 2c20 416e 795d 3a0a 2020 2020  [str, Any]:.    
-00004d40: 2020 2020 6966 2022 7374 6f72 6167 6522      if "storage"
-00004d50: 2069 6e20 6461 7461 2061 6e64 2064 6174   in data and dat
-00004d60: 615b 2273 746f 7261 6765 225d 203d 3d20  a["storage"] == 
-00004d70: 7b7d 3a0a 2020 2020 2020 2020 2020 2020  {}:.            
-00004d80: 6465 6c20 6461 7461 5b22 7374 6f72 6167  del data["storag
-00004d90: 6522 5d0a 0a20 2020 2020 2020 2072 6574  e"]..        ret
-00004da0: 7572 6e20 7375 7065 7228 292e 756e 6966  urn super().unif
-00004db0: 695f 6469 6374 5f74 6f5f 6469 6374 2864  i_dict_to_dict(d
-00004dc0: 6174 6129 0a0a 2020 2020 6465 6620 756e  ata)..    def un
-00004dd0: 6966 695f 6469 6374 280a 2020 2020 2020  ifi_dict(.      
-00004de0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00004df0: 6461 7461 3a20 4f70 7469 6f6e 616c 5b64  data: Optional[d
-00004e00: 6963 745b 7374 722c 2041 6e79 5d5d 203d  ict[str, Any]] =
-00004e10: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00004e20: 7863 6c75 6465 3a20 4f70 7469 6f6e 616c  xclude: Optional
-00004e30: 5b73 6574 5b73 7472 5d5d 203d 204e 6f6e  [set[str]] = Non
-00004e40: 652c 0a20 2020 2029 202d 3e20 6469 6374  e,.    ) -> dict
-00004e50: 5b73 7472 2c20 416e 795d 3a0a 2020 2020  [str, Any]:.    
-00004e60: 2020 2020 6461 7461 203d 2073 7570 6572      data = super
-00004e70: 2829 2e75 6e69 6669 5f64 6963 7428 6461  ().unifi_dict(da
-00004e80: 7461 3d64 6174 612c 2065 7863 6c75 6465  ta=data, exclude
-00004e90: 3d65 7863 6c75 6465 290a 0a20 2020 2020  =exclude)..     
-00004ea0: 2020 2069 6620 2273 746f 7261 6765 2220     if "storage" 
-00004eb0: 696e 2064 6174 6120 616e 6420 6461 7461  in data and data
-00004ec0: 5b22 7374 6f72 6167 6522 5d20 6973 204e  ["storage"] is N
-00004ed0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00004ee0: 2064 6174 615b 2273 746f 7261 6765 225d   data["storage"]
-00004ef0: 203d 207b 7d0a 0a20 2020 2020 2020 2072   = {}..        r
-00004f00: 6574 7572 6e20 6461 7461 0a0a 0a63 6c61  eturn data...cla
-00004f10: 7373 2043 616d 6572 615a 6f6e 6528 5072  ss CameraZone(Pr
-00004f20: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
-00004f30: 3a0a 2020 2020 6964 3a20 696e 740a 2020  :.    id: int.  
-00004f40: 2020 6e61 6d65 3a20 7374 720a 2020 2020    name: str.    
-00004f50: 636f 6c6f 723a 2043 6f6c 6f72 0a20 2020  color: Color.   
-00004f60: 2070 6f69 6e74 733a 206c 6973 745b 7475   points: list[tu
-00004f70: 706c 655b 5065 7263 656e 742c 2050 6572  ple[Percent, Per
-00004f80: 6365 6e74 5d5d 0a0a 2020 2020 4063 6c61  cent]]..    @cla
-00004f90: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00004fa0: 2075 6e69 6669 5f64 6963 745f 746f 5f64   unifi_dict_to_d
-00004fb0: 6963 7428 636c 732c 2064 6174 613a 2064  ict(cls, data: d
-00004fc0: 6963 745b 7374 722c 2041 6e79 5d29 202d  ict[str, Any]) -
-00004fd0: 3e20 6469 6374 5b73 7472 2c20 416e 795d  > dict[str, Any]
-00004fe0: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-00004ff0: 2073 7570 6572 2829 2e75 6e69 6669 5f64   super().unifi_d
-00005000: 6963 745f 746f 5f64 6963 7428 6461 7461  ict_to_dict(data
-00005010: 290a 2020 2020 2020 2020 6966 2022 706f  ).        if "po
-00005020: 696e 7473 2220 696e 2064 6174 6120 616e  ints" in data an
-00005030: 6420 6973 696e 7374 616e 6365 2864 6174  d isinstance(dat
-00005040: 615b 2270 6f69 6e74 7322 5d2c 2049 7465  a["points"], Ite
-00005050: 7261 626c 6529 3a0a 2020 2020 2020 2020  rable):.        
-00005060: 2020 2020 6461 7461 5b22 706f 696e 7473      data["points
-00005070: 225d 203d 205b 2870 5b30 5d2c 2070 5b31  "] = [(p[0], p[1
-00005080: 5d29 2066 6f72 2070 2069 6e20 6461 7461  ]) for p in data
-00005090: 5b22 706f 696e 7473 225d 5d0a 0a20 2020  ["points"]]..   
-000050a0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-000050b0: 0a0a 2020 2020 6465 6620 756e 6966 695f  ..    def unifi_
-000050c0: 6469 6374 280a 2020 2020 2020 2020 7365  dict(.        se
-000050d0: 6c66 2c0a 2020 2020 2020 2020 6461 7461  lf,.        data
-000050e0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745b  : Optional[dict[
-000050f0: 7374 722c 2041 6e79 5d5d 203d 204e 6f6e  str, Any]] = Non
-00005100: 652c 0a20 2020 2020 2020 2065 7863 6c75  e,.        exclu
-00005110: 6465 3a20 4f70 7469 6f6e 616c 5b73 6574  de: Optional[set
-00005120: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
-00005130: 2020 2029 202d 3e20 6469 6374 5b73 7472     ) -> dict[str
-00005140: 2c20 416e 795d 3a0a 2020 2020 2020 2020  , Any]:.        
-00005150: 6461 7461 203d 2073 7570 6572 2829 2e75  data = super().u
-00005160: 6e69 6669 5f64 6963 7428 6461 7461 3d64  nifi_dict(data=d
-00005170: 6174 612c 2065 7863 6c75 6465 3d65 7863  ata, exclude=exc
-00005180: 6c75 6465 290a 0a20 2020 2020 2020 2069  lude)..        i
-00005190: 6620 2270 6f69 6e74 7322 2069 6e20 6461  f "points" in da
-000051a0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-000051b0: 6461 7461 5b22 706f 696e 7473 225d 203d  data["points"] =
-000051c0: 205b 7365 7269 616c 697a 655f 706f 696e   [serialize_poin
-000051d0: 7428 7029 2066 6f72 2070 2069 6e20 6461  t(p) for p in da
-000051e0: 7461 5b22 706f 696e 7473 225d 5d0a 0a20  ta["points"]].. 
-000051f0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00005200: 7461 0a0a 2020 2020 4073 7461 7469 636d  ta..    @staticm
-00005210: 6574 686f 640a 2020 2020 6465 6620 6372  ethod.    def cr
-00005220: 6561 7465 5f70 7269 7661 6379 5f7a 6f6e  eate_privacy_zon
-00005230: 6528 7a6f 6e65 5f69 643a 2069 6e74 2920  e(zone_id: int) 
-00005240: 2d3e 2043 616d 6572 615a 6f6e 653a 0a20  -> CameraZone:. 
-00005250: 2020 2020 2020 2072 6574 7572 6e20 4361         return Ca
-00005260: 6d65 7261 5a6f 6e65 280a 2020 2020 2020  meraZone(.      
-00005270: 2020 2020 2020 6964 3d7a 6f6e 655f 6964        id=zone_id
-00005280: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
-00005290: 6d65 3d50 5249 5641 4359 5f5a 4f4e 455f  me=PRIVACY_ZONE_
-000052a0: 4e41 4d45 2c0a 2020 2020 2020 2020 2020  NAME,.          
-000052b0: 2020 636f 6c6f 723d 436f 6c6f 7228 2223    color=Color("#
-000052c0: 3835 4243 4543 2229 2c0a 2020 2020 2020  85BCEC"),.      
-000052d0: 2020 2020 2020 706f 696e 7473 3d5b 5b30        points=[[0
-000052e0: 2c20 305d 2c20 5b31 2c20 305d 2c20 5b31  , 0], [1, 0], [1
-000052f0: 2c20 315d 2c20 5b30 2c20 315d 5d2c 2020  , 1], [0, 1]],  
-00005300: 2320 7479 7065 3a20 6967 6e6f 7265 5b6c  # type: ignore[l
-00005310: 6973 742d 6974 656d 5d0a 2020 2020 2020  ist-item].      
-00005320: 2020 290a 0a0a 636c 6173 7320 4d6f 7469    )...class Moti
-00005330: 6f6e 5a6f 6e65 2843 616d 6572 615a 6f6e  onZone(CameraZon
-00005340: 6529 3a0a 2020 2020 7365 6e73 6974 6976  e):.    sensitiv
-00005350: 6974 793a 2050 6572 6365 6e74 496e 740a  ity: PercentInt.
-00005360: 0a0a 636c 6173 7320 536d 6172 744d 6f74  ..class SmartMot
-00005370: 696f 6e5a 6f6e 6528 4d6f 7469 6f6e 5a6f  ionZone(MotionZo
-00005380: 6e65 293a 0a20 2020 206f 626a 6563 745f  ne):.    object_
-00005390: 7479 7065 733a 206c 6973 745b 536d 6172  types: list[Smar
-000053a0: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-000053b0: 655d 0a0a 2020 2020 4063 6c61 7373 6d65  e]..    @classme
-000053c0: 7468 6f64 0a20 2020 2064 6566 2075 6e69  thod.    def uni
-000053d0: 6669 5f64 6963 745f 746f 5f64 6963 7428  fi_dict_to_dict(
-000053e0: 636c 732c 2064 6174 613a 2064 6963 745b  cls, data: dict[
-000053f0: 7374 722c 2041 6e79 5d29 202d 3e20 6469  str, Any]) -> di
-00005400: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
-00005410: 2020 2020 2020 6966 2022 6f62 6a65 6374        if "object
-00005420: 5479 7065 7322 2069 6e20 6461 7461 3a0a  Types" in data:.
-00005430: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00005440: 5b22 6f62 6a65 6374 5479 7065 7322 5d20  ["objectTypes"] 
-00005450: 3d20 636f 6e76 6572 745f 736d 6172 745f  = convert_smart_
-00005460: 7479 7065 7328 6461 7461 2e70 6f70 2822  types(data.pop("
-00005470: 6f62 6a65 6374 5479 7065 7322 2929 0a0a  objectTypes"))..
-00005480: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005490: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
-000054a0: 745f 746f 5f64 6963 7428 6461 7461 290a  t_to_dict(data).
-000054b0: 0a0a 636c 6173 7320 5072 6976 6163 794d  ..class PrivacyM
-000054c0: 6173 6b43 6170 6162 696c 6974 7928 5072  askCapability(Pr
-000054d0: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
-000054e0: 3a0a 2020 2020 6d61 785f 6d61 736b 733a  :.    max_masks:
-000054f0: 204f 7074 696f 6e61 6c5b 696e 745d 0a20   Optional[int]. 
-00005500: 2020 2072 6563 7461 6e67 6c65 5f6f 6e6c     rectangle_onl
-00005510: 793a 2062 6f6f 6c0a 0a0a 636c 6173 7320  y: bool...class 
-00005520: 486f 7470 6c75 6745 7874 656e 6465 7228  HotplugExtender(
-00005530: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
-00005540: 7429 3a0a 2020 2020 6861 735f 666c 6173  t):.    has_flas
-00005550: 683a 204f 7074 696f 6e61 6c5b 626f 6f6c  h: Optional[bool
-00005560: 5d20 3d20 4e6f 6e65 0a20 2020 2068 6173  ] = None.    has
-00005570: 5f69 723a 204f 7074 696f 6e61 6c5b 626f  _ir: Optional[bo
-00005580: 6f6c 5d20 3d20 4e6f 6e65 0a20 2020 2068  ol] = None.    h
-00005590: 6173 5f72 6164 6172 3a20 4f70 7469 6f6e  as_radar: Option
-000055a0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-000055b0: 2020 2020 6973 5f61 7474 6163 6865 643a      is_attached:
-000055c0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-000055d0: 3d20 4e6f 6e65 0a20 2020 2023 2033 2e30  = None.    # 3.0
-000055e0: 2e32 322b 0a20 2020 2066 6c61 7368 5f72  .22+.    flash_r
-000055f0: 616e 6765 3a20 4f70 7469 6f6e 616c 5b41  ange: Optional[A
-00005600: 6e79 5d20 3d20 4e6f 6e65 0a0a 2020 2020  ny] = None..    
-00005610: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00005620: 2040 6361 6368 650a 2020 2020 6465 6620   @cache.    def 
-00005630: 5f67 6574 5f75 6e69 6669 5f72 656d 6170  _get_unifi_remap
-00005640: 7328 636c 7329 202d 3e20 6469 6374 5b73  s(cls) -> dict[s
-00005650: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
-00005660: 2020 7265 7475 726e 207b 2a2a 7375 7065    return {**supe
-00005670: 7228 292e 5f67 6574 5f75 6e69 6669 5f72  r()._get_unifi_r
-00005680: 656d 6170 7328 292c 2022 6861 7349 5222  emaps(), "hasIR"
-00005690: 3a20 2268 6173 4972 227d 0a0a 0a63 6c61  : "hasIr"}...cla
-000056a0: 7373 2048 6f74 706c 7567 2850 726f 7465  ss Hotplug(Prote
-000056b0: 6374 4261 7365 4f62 6a65 6374 293a 0a20  ctBaseObject):. 
-000056c0: 2020 2061 7564 696f 3a20 4f70 7469 6f6e     audio: Option
-000056d0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-000056e0: 2020 2020 7669 6465 6f3a 204f 7074 696f      video: Optio
-000056f0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00005700: 0a20 2020 2065 7874 656e 6465 723a 204f  .    extender: O
-00005710: 7074 696f 6e61 6c5b 486f 7470 6c75 6745  ptional[HotplugE
-00005720: 7874 656e 6465 725d 203d 204e 6f6e 650a  xtender] = None.
-00005730: 2020 2020 2320 322e 382e 3335 2b0a 2020      # 2.8.35+.  
-00005740: 2020 7374 616e 6461 6c6f 6e65 5f61 646f    standalone_ado
-00005750: 7074 696f 6e3a 204f 7074 696f 6e61 6c5b  ption: Optional[
-00005760: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 0a63  bool] = None...c
-00005770: 6c61 7373 2043 616d 6572 6146 6561 7475  lass CameraFeatu
-00005780: 7265 466c 6167 7328 5072 6f74 6563 7442  reFlags(ProtectB
-00005790: 6173 654f 626a 6563 7429 3a0a 2020 2020  aseObject):.    
-000057a0: 6361 6e5f 6164 6a75 7374 5f69 725f 6c65  can_adjust_ir_le
-000057b0: 645f 6c65 7665 6c3a 2062 6f6f 6c0a 2020  d_level: bool.  
-000057c0: 2020 6361 6e5f 6d61 6769 635f 7a6f 6f6d    can_magic_zoom
-000057d0: 3a20 626f 6f6c 0a20 2020 2063 616e 5f6f  : bool.    can_o
-000057e0: 7074 6963 616c 5f7a 6f6f 6d3a 2062 6f6f  ptical_zoom: boo
-000057f0: 6c0a 2020 2020 6361 6e5f 746f 7563 685f  l.    can_touch_
-00005800: 666f 6375 733a 2062 6f6f 6c0a 2020 2020  focus: bool.    
-00005810: 6861 735f 6163 6365 6c65 726f 6d65 7465  has_acceleromete
-00005820: 723a 2062 6f6f 6c0a 2020 2020 6861 735f  r: bool.    has_
-00005830: 6165 633a 2062 6f6f 6c0a 2020 2020 6861  aec: bool.    ha
-00005840: 735f 626c 7565 746f 6f74 683a 2062 6f6f  s_bluetooth: boo
-00005850: 6c0a 2020 2020 6861 735f 6368 696d 653a  l.    has_chime:
-00005860: 2062 6f6f 6c0a 2020 2020 6861 735f 6578   bool.    has_ex
-00005870: 7465 726e 616c 5f69 723a 2062 6f6f 6c0a  ternal_ir: bool.
-00005880: 2020 2020 6861 735f 6963 725f 7365 6e73      has_icr_sens
-00005890: 6974 6976 6974 793a 2062 6f6f 6c0a 2020  itivity: bool.  
-000058a0: 2020 6861 735f 6c64 633a 2062 6f6f 6c0a    has_ldc: bool.
-000058b0: 2020 2020 6861 735f 6c65 645f 6972 3a20      has_led_ir: 
-000058c0: 626f 6f6c 0a20 2020 2068 6173 5f6c 6564  bool.    has_led
-000058d0: 5f73 7461 7475 733a 2062 6f6f 6c0a 2020  _status: bool.  
-000058e0: 2020 6861 735f 6c69 6e65 5f69 6e3a 2062    has_line_in: b
-000058f0: 6f6f 6c0a 2020 2020 6861 735f 6d69 633a  ool.    has_mic:
-00005900: 2062 6f6f 6c0a 2020 2020 6861 735f 7072   bool.    has_pr
-00005910: 6976 6163 795f 6d61 736b 3a20 626f 6f6c  ivacy_mask: bool
-00005920: 0a20 2020 2068 6173 5f72 7463 3a20 626f  .    has_rtc: bo
-00005930: 6f6c 0a20 2020 2068 6173 5f73 645f 6361  ol.    has_sd_ca
-00005940: 7264 3a20 626f 6f6c 0a20 2020 2068 6173  rd: bool.    has
-00005950: 5f73 7065 616b 6572 3a20 626f 6f6c 0a20  _speaker: bool. 
-00005960: 2020 2068 6173 5f77 6966 693a 2062 6f6f     has_wifi: boo
-00005970: 6c0a 2020 2020 6861 735f 6864 723a 2062  l.    has_hdr: b
-00005980: 6f6f 6c0a 2020 2020 6861 735f 6175 746f  ool.    has_auto
-00005990: 5f69 6372 5f6f 6e6c 793a 2062 6f6f 6c0a  _icr_only: bool.
-000059a0: 2020 2020 7669 6465 6f5f 6d6f 6465 733a      video_modes:
-000059b0: 206c 6973 745b 5669 6465 6f4d 6f64 655d   list[VideoMode]
-000059c0: 0a20 2020 2076 6964 656f 5f6d 6f64 655f  .    video_mode_
-000059d0: 6d61 785f 6670 733a 206c 6973 745b 696e  max_fps: list[in
-000059e0: 745d 0a20 2020 2068 6173 5f6d 6f74 696f  t].    has_motio
-000059f0: 6e5f 7a6f 6e65 733a 2062 6f6f 6c0a 2020  n_zones: bool.  
-00005a00: 2020 6861 735f 6c63 645f 7363 7265 656e    has_lcd_screen
-00005a10: 3a20 626f 6f6c 0a20 2020 2073 6d61 7274  : bool.    smart
-00005a20: 5f64 6574 6563 745f 7479 7065 733a 206c  _detect_types: l
-00005a30: 6973 745b 536d 6172 7444 6574 6563 744f  ist[SmartDetectO
-00005a40: 626a 6563 7454 7970 655d 0a20 2020 206d  bjectType].    m
-00005a50: 6f74 696f 6e5f 616c 676f 7269 7468 6d73  otion_algorithms
-00005a60: 3a20 6c69 7374 5b4d 6f74 696f 6e41 6c67  : list[MotionAlg
-00005a70: 6f72 6974 686d 5d0a 2020 2020 6861 735f  orithm].    has_
-00005a80: 7371 7561 7265 5f65 7665 6e74 5f74 6875  square_event_thu
-00005a90: 6d62 6e61 696c 3a20 626f 6f6c 0a20 2020  mbnail: bool.   
-00005aa0: 2068 6173 5f70 6163 6b61 6765 5f63 616d   has_package_cam
-00005ab0: 6572 613a 2062 6f6f 6c0a 2020 2020 7072  era: bool.    pr
-00005ac0: 6976 6163 795f 6d61 736b 5f63 6170 6162  ivacy_mask_capab
-00005ad0: 696c 6974 793a 2050 7269 7661 6379 4d61  ility: PrivacyMa
-00005ae0: 736b 4361 7061 6269 6c69 7479 0a20 2020  skCapability.   
-00005af0: 2068 6173 5f73 6d61 7274 5f64 6574 6563   has_smart_detec
-00005b00: 743a 2062 6f6f 6c0a 2020 2020 6175 6469  t: bool.    audi
-00005b10: 6f3a 206c 6973 745b 7374 725d 203d 205b  o: list[str] = [
-00005b20: 5d0a 2020 2020 6175 6469 6f5f 636f 6465  ].    audio_code
-00005b30: 6373 3a20 6c69 7374 5b41 7564 696f 436f  cs: list[AudioCo
-00005b40: 6465 6373 5d20 3d20 5b5d 0a20 2020 206d  decs] = [].    m
-00005b50: 6f75 6e74 5f70 6f73 6974 696f 6e73 3a20  ount_positions: 
-00005b60: 6c69 7374 5b4d 6f75 6e74 506f 7369 7469  list[MountPositi
-00005b70: 6f6e 5d20 3d20 5b5d 0a20 2020 2068 6173  on] = [].    has
-00005b80: 5f69 6e66 7261 7265 643a 204f 7074 696f  _infrared: Optio
-00005b90: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00005ba0: 0a20 2020 206c 656e 735f 7479 7065 3a20  .    lens_type: 
-00005bb0: 4f70 7469 6f6e 616c 5b4c 656e 7354 7970  Optional[LensTyp
-00005bc0: 655d 203d 204e 6f6e 650a 2020 2020 686f  e] = None.    ho
-00005bd0: 7470 6c75 673a 204f 7074 696f 6e61 6c5b  tplug: Optional[
-00005be0: 486f 7470 6c75 675d 203d 204e 6f6e 650a  Hotplug] = None.
-00005bf0: 2020 2020 736d 6172 745f 6465 7465 6374      smart_detect
-00005c00: 5f61 7564 696f 5f74 7970 6573 3a20 4f70  _audio_types: Op
-00005c10: 7469 6f6e 616c 5b6c 6973 745b 536d 6172  tional[list[Smar
-00005c20: 7444 6574 6563 7441 7564 696f 5479 7065  tDetectAudioType
-00005c30: 5d5d 203d 204e 6f6e 650a 2020 2020 2320  ]] = None.    # 
-00005c40: 322e 372e 3138 2b0a 2020 2020 6973 5f64  2.7.18+.    is_d
-00005c50: 6f6f 7262 656c 6c3a 2062 6f6f 6c0a 2020  oorbell: bool.  
-00005c60: 2020 2320 322e 382e 3232 2b0a 2020 2020    # 2.8.22+.    
-00005c70: 6c65 6e73 5f6d 6f64 656c 3a20 4f70 7469  lens_model: Opti
-00005c80: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00005c90: 0a20 2020 2023 2032 2e39 2e32 302b 0a20  .    # 2.9.20+. 
-00005ca0: 2020 2068 6173 5f63 6f6c 6f72 5f6c 6364     has_color_lcd
-00005cb0: 5f73 6372 6565 6e3a 204f 7074 696f 6e61  _screen: Optiona
-00005cc0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a20  l[bool] = None. 
-00005cd0: 2020 2068 6173 5f6c 696e 655f 6372 6f73     has_line_cros
-00005ce0: 7369 6e67 3a20 4f70 7469 6f6e 616c 5b62  sing: Optional[b
-00005cf0: 6f6f 6c5d 203d 204e 6f6e 650a 2020 2020  ool] = None.    
-00005d00: 6861 735f 6c69 6e65 5f63 726f 7373 696e  has_line_crossin
-00005d10: 675f 636f 756e 7469 6e67 3a20 4f70 7469  g_counting: Opti
-00005d20: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00005d30: 650a 2020 2020 6861 735f 6c69 7665 7669  e.    has_livevi
-00005d40: 6577 5f74 7261 636b 696e 673a 204f 7074  ew_tracking: Opt
-00005d50: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00005d60: 6e65 0a20 2020 2023 2032 2e31 302e 3130  ne.    # 2.10.10
-00005d70: 2b0a 2020 2020 6861 735f 666c 6173 683a  +.    has_flash:
-00005d80: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00005d90: 3d20 4e6f 6e65 0a20 2020 2069 735f 7074  = None.    is_pt
-00005da0: 7a3a 204f 7074 696f 6e61 6c5b 626f 6f6c  z: Optional[bool
-00005db0: 5d20 3d20 4e6f 6e65 0a20 2020 2023 2032  ] = None.    # 2
-00005dc0: 2e31 312e 3133 2b0a 2020 2020 6175 6469  .11.13+.    audi
-00005dd0: 6f5f 7374 796c 653a 204f 7074 696f 6e61  o_style: Optiona
-00005de0: 6c5b 6c69 7374 5b41 7564 696f 5374 796c  l[list[AudioStyl
-00005df0: 655d 5d20 3d20 4e6f 6e65 0a20 2020 2068  e]] = None.    h
-00005e00: 6173 5f76 6572 7469 6361 6c5f 666c 6970  as_vertical_flip
-00005e10: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00005e20: 203d 204e 6f6e 650a 2020 2020 2320 332e   = None.    # 3.
-00005e30: 302e 3232 2b0a 2020 2020 666c 6173 685f  0.22+.    flash_
-00005e40: 7261 6e67 653a 204f 7074 696f 6e61 6c5b  range: Optional[
-00005e50: 416e 795d 203d 204e 6f6e 650a 0a20 2020  Any] = None..   
-00005e60: 2023 2054 4f44 4f3a 0a20 2020 2023 2066   # TODO:.    # f
-00005e70: 6f63 7573 0a20 2020 2023 2070 616e 0a20  ocus.    # pan. 
-00005e80: 2020 2023 2074 696c 740a 2020 2020 2320     # tilt.    # 
-00005e90: 7a6f 6f6d 0a0a 2020 2020 4063 6c61 7373  zoom..    @class
-00005ea0: 6d65 7468 6f64 0a20 2020 2064 6566 2075  method.    def u
-00005eb0: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
-00005ec0: 7428 636c 732c 2064 6174 613a 2064 6963  t(cls, data: dic
-00005ed0: 745b 7374 722c 2041 6e79 5d29 202d 3e20  t[str, Any]) -> 
-00005ee0: 6469 6374 5b73 7472 2c20 416e 795d 3a0a  dict[str, Any]:.
-00005ef0: 2020 2020 2020 2020 6966 2022 736d 6172          if "smar
-00005f00: 7444 6574 6563 7454 7970 6573 2220 696e  tDetectTypes" in
-00005f10: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00005f20: 2020 2064 6174 615b 2273 6d61 7274 4465     data["smartDe
-00005f30: 7465 6374 5479 7065 7322 5d20 3d20 636f  tectTypes"] = co
-00005f40: 6e76 6572 745f 736d 6172 745f 7479 7065  nvert_smart_type
-00005f50: 7328 6461 7461 2e70 6f70 2822 736d 6172  s(data.pop("smar
-00005f60: 7444 6574 6563 7454 7970 6573 2229 290a  tDetectTypes")).
-00005f70: 2020 2020 2020 2020 6966 2022 736d 6172          if "smar
-00005f80: 7444 6574 6563 7441 7564 696f 5479 7065  tDetectAudioType
-00005f90: 7322 2069 6e20 6461 7461 3a0a 2020 2020  s" in data:.    
-00005fa0: 2020 2020 2020 2020 6461 7461 5b22 736d          data["sm
-00005fb0: 6172 7444 6574 6563 7441 7564 696f 5479  artDetectAudioTy
-00005fc0: 7065 7322 5d20 3d20 636f 6e76 6572 745f  pes"] = convert_
-00005fd0: 736d 6172 745f 6175 6469 6f5f 7479 7065  smart_audio_type
-00005fe0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00005ff0: 2020 2064 6174 612e 706f 7028 2273 6d61     data.pop("sma
-00006000: 7274 4465 7465 6374 4175 6469 6f54 7970  rtDetectAudioTyp
-00006010: 6573 2229 2c0a 2020 2020 2020 2020 2020  es"),.          
-00006020: 2020 290a 2020 2020 2020 2020 6966 2022    ).        if "
-00006030: 7669 6465 6f4d 6f64 6573 2220 696e 2064  videoModes" in d
-00006040: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00006050: 2064 6174 615b 2276 6964 656f 4d6f 6465   data["videoMode
-00006060: 7322 5d20 3d20 636f 6e76 6572 745f 7669  s"] = convert_vi
-00006070: 6465 6f5f 6d6f 6465 7328 6461 7461 2e70  deo_modes(data.p
-00006080: 6f70 2822 7669 6465 6f4d 6f64 6573 2229  op("videoModes")
-00006090: 290a 0a20 2020 2020 2020 2023 2062 6163  )..        # bac
-000060a0: 6b70 6f72 7420 7375 7070 6f72 7420 666f  kport support fo
-000060b0: 7220 6069 735f 646f 6f72 6265 6c6c 6020  r `is_doorbell` 
-000060c0: 746f 206f 6c64 6572 2076 6572 7369 6f6e  to older version
-000060d0: 7320 6f66 2050 726f 7465 6374 0a20 2020  s of Protect.   
-000060e0: 2020 2020 2069 6620 2268 6173 4368 696d       if "hasChim
-000060f0: 6522 2069 6e20 6461 7461 2061 6e64 2022  e" in data and "
-00006100: 6973 446f 6f72 6265 6c6c 2220 6e6f 7420  isDoorbell" not 
-00006110: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
-00006120: 2020 2020 2064 6174 615b 2269 7344 6f6f       data["isDoo
-00006130: 7262 656c 6c22 5d20 3d20 6461 7461 5b22  rbell"] = data["
-00006140: 6861 7343 6869 6d65 225d 0a0a 2020 2020  hasChime"]..    
-00006150: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00006160: 2829 2e75 6e69 6669 5f64 6963 745f 746f  ().unifi_dict_to
-00006170: 5f64 6963 7428 6461 7461 290a 0a20 2020  _dict(data)..   
-00006180: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00006190: 2020 4063 6163 6865 0a20 2020 2064 6566    @cache.    def
-000061a0: 205f 6765 745f 756e 6966 695f 7265 6d61   _get_unifi_rema
-000061b0: 7073 2863 6c73 2920 2d3e 2064 6963 745b  ps(cls) -> dict[
-000061c0: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-000061d0: 2020 2072 6574 7572 6e20 7b2a 2a73 7570     return {**sup
-000061e0: 6572 2829 2e5f 6765 745f 756e 6966 695f  er()._get_unifi_
-000061f0: 7265 6d61 7073 2829 2c20 2268 6173 4175  remaps(), "hasAu
-00006200: 746f 4943 524f 6e6c 7922 3a20 2268 6173  toICROnly": "has
-00006210: 4175 746f 4963 724f 6e6c 7922 7d0a 0a20  AutoIcrOnly"}.. 
-00006220: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00006230: 2064 6566 2068 6173 5f68 6967 6866 7073   def has_highfps
-00006240: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00006250: 2020 2020 2020 2020 7265 7475 726e 2056          return V
-00006260: 6964 656f 4d6f 6465 2e48 4947 485f 4650  ideoMode.HIGH_FP
-00006270: 5320 696e 2073 656c 662e 7669 6465 6f5f  S in self.video_
-00006280: 6d6f 6465 730a 0a20 2020 2040 7072 6f70  modes..    @prop
-00006290: 6572 7479 0a20 2020 2064 6566 2068 6173  erty.    def has
-000062a0: 5f77 6472 2873 656c 6629 202d 3e20 626f  _wdr(self) -> bo
-000062b0: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-000062c0: 726e 206e 6f74 2073 656c 662e 6861 735f  rn not self.has_
-000062d0: 6864 720a 0a0a 636c 6173 7320 4361 6d65  hdr...class Came
-000062e0: 7261 4c65 6e73 6573 2850 726f 7465 6374  raLenses(Protect
-000062f0: 4261 7365 4f62 6a65 6374 293a 0a20 2020  BaseObject):.   
-00006300: 2069 643a 2069 6e74 0a20 2020 2076 6964   id: int.    vid
-00006310: 656f 3a20 5669 6465 6f53 7461 7473 0a0a  eo: VideoStats..
-00006320: 0a63 6c61 7373 2043 616d 6572 6148 6f6d  .class CameraHom
-00006330: 656b 6974 5365 7474 696e 6773 2850 726f  ekitSettings(Pro
-00006340: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
-00006350: 0a20 2020 206d 6963 726f 7068 6f6e 655f  .    microphone_
-00006360: 6d75 7465 643a 2062 6f6f 6c0a 2020 2020  muted: bool.    
-00006370: 7370 6561 6b65 725f 6d75 7465 643a 2062  speaker_muted: b
-00006380: 6f6f 6c0a 2020 2020 7374 7265 616d 5f69  ool.    stream_i
-00006390: 6e5f 7072 6f67 7265 7373 3a20 626f 6f6c  n_progress: bool
-000063a0: 0a20 2020 2074 616c 6b62 6163 6b5f 7365  .    talkback_se
-000063b0: 7474 696e 6773 5f61 6374 6976 653a 2062  ttings_active: b
-000063c0: 6f6f 6c0a 0a0a 636c 6173 7320 4361 6d65  ool...class Came
-000063d0: 7261 4175 6469 6f53 6574 7469 6e67 7328  raAudioSettings(
-000063e0: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
-000063f0: 7429 3a0a 2020 2020 7374 796c 653a 206c  t):.    style: l
-00006400: 6973 745b 4175 6469 6f53 7479 6c65 5d0a  ist[AudioStyle].
-00006410: 0a0a 636c 6173 7320 4361 6d65 7261 2850  ..class Camera(P
-00006420: 726f 7465 6374 4d6f 7469 6f6e 4465 7669  rotectMotionDevi
-00006430: 6365 4d6f 6465 6c29 3a0a 2020 2020 6973  ceModel):.    is
-00006440: 5f64 656c 6574 696e 673a 2062 6f6f 6c0a  _deleting: bool.
-00006450: 2020 2020 2320 4d69 6372 6f70 686f 6e65      # Microphone
-00006460: 2053 656e 7369 7469 7669 7479 0a20 2020   Sensitivity.   
-00006470: 206d 6963 5f76 6f6c 756d 653a 2050 6572   mic_volume: Per
-00006480: 6365 6e74 496e 740a 2020 2020 6973 5f6d  centInt.    is_m
-00006490: 6963 5f65 6e61 626c 6564 3a20 626f 6f6c  ic_enabled: bool
-000064a0: 0a20 2020 2069 735f 7265 636f 7264 696e  .    is_recordin
-000064b0: 673a 2062 6f6f 6c0a 2020 2020 6973 5f6d  g: bool.    is_m
-000064c0: 6f74 696f 6e5f 6465 7465 6374 6564 3a20  otion_detected: 
-000064d0: 626f 6f6c 0a20 2020 2069 735f 736d 6172  bool.    is_smar
-000064e0: 745f 6465 7465 6374 6564 3a20 626f 6f6c  t_detected: bool
-000064f0: 0a20 2020 2070 6879 5f72 6174 653a 204f  .    phy_rate: O
-00006500: 7074 696f 6e61 6c5b 666c 6f61 745d 0a20  ptional[float]. 
-00006510: 2020 2068 6472 5f6d 6f64 653a 2062 6f6f     hdr_mode: boo
-00006520: 6c0a 2020 2020 2320 5265 636f 7264 696e  l.    # Recordin
-00006530: 6720 5175 616c 6974 7920 2d3e 2048 6967  g Quality -> Hig
-00006540: 6820 4672 616d 650a 2020 2020 7669 6465  h Frame.    vide
-00006550: 6f5f 6d6f 6465 3a20 5669 6465 6f4d 6f64  o_mode: VideoMod
-00006560: 650a 2020 2020 6973 5f70 726f 6269 6e67  e.    is_probing
-00006570: 5f66 6f72 5f77 6966 693a 2062 6f6f 6c0a  _for_wifi: bool.
-00006580: 2020 2020 6368 696d 655f 6475 7261 7469      chime_durati
-00006590: 6f6e 3a20 7469 6d65 6465 6c74 610a 2020  on: timedelta.  
-000065a0: 2020 6c61 7374 5f72 696e 673a 204f 7074    last_ring: Opt
-000065b0: 696f 6e61 6c5b 6461 7465 7469 6d65 5d0a  ional[datetime].
-000065c0: 2020 2020 6973 5f6c 6976 655f 6865 6174      is_live_heat
-000065d0: 6d61 705f 656e 6162 6c65 643a 2062 6f6f  map_enabled: boo
-000065e0: 6c0a 2020 2020 7669 6465 6f5f 7265 636f  l.    video_reco
-000065f0: 6e66 6967 7572 6174 696f 6e5f 696e 5f70  nfiguration_in_p
-00006600: 726f 6772 6573 733a 2062 6f6f 6c0a 2020  rogress: bool.  
-00006610: 2020 6368 616e 6e65 6c73 3a20 6c69 7374    channels: list
-00006620: 5b43 616d 6572 6143 6861 6e6e 656c 5d0a  [CameraChannel].
-00006630: 2020 2020 6973 705f 7365 7474 696e 6773      isp_settings
-00006640: 3a20 4953 5053 6574 7469 6e67 730a 2020  : ISPSettings.  
-00006650: 2020 7461 6c6b 6261 636b 5f73 6574 7469    talkback_setti
-00006660: 6e67 733a 2054 616c 6b62 6163 6b53 6574  ngs: TalkbackSet
-00006670: 7469 6e67 730a 2020 2020 6f73 645f 7365  tings.    osd_se
-00006680: 7474 696e 6773 3a20 4f53 4453 6574 7469  ttings: OSDSetti
-00006690: 6e67 730a 2020 2020 6c65 645f 7365 7474  ngs.    led_sett
-000066a0: 696e 6773 3a20 4c45 4453 6574 7469 6e67  ings: LEDSetting
-000066b0: 730a 2020 2020 7370 6561 6b65 725f 7365  s.    speaker_se
-000066c0: 7474 696e 6773 3a20 5370 6561 6b65 7253  ttings: SpeakerS
-000066d0: 6574 7469 6e67 730a 2020 2020 7265 636f  ettings.    reco
-000066e0: 7264 696e 675f 7365 7474 696e 6773 3a20  rding_settings: 
-000066f0: 5265 636f 7264 696e 6753 6574 7469 6e67  RecordingSetting
-00006700: 730a 2020 2020 736d 6172 745f 6465 7465  s.    smart_dete
-00006710: 6374 5f73 6574 7469 6e67 733a 2053 6d61  ct_settings: Sma
-00006720: 7274 4465 7465 6374 5365 7474 696e 6773  rtDetectSettings
-00006730: 0a20 2020 206d 6f74 696f 6e5f 7a6f 6e65  .    motion_zone
-00006740: 733a 206c 6973 745b 4d6f 7469 6f6e 5a6f  s: list[MotionZo
-00006750: 6e65 5d0a 2020 2020 7072 6976 6163 795f  ne].    privacy_
-00006760: 7a6f 6e65 733a 206c 6973 745b 4361 6d65  zones: list[Came
-00006770: 7261 5a6f 6e65 5d0a 2020 2020 736d 6172  raZone].    smar
-00006780: 745f 6465 7465 6374 5f7a 6f6e 6573 3a20  t_detect_zones: 
-00006790: 6c69 7374 5b53 6d61 7274 4d6f 7469 6f6e  list[SmartMotion
-000067a0: 5a6f 6e65 5d0a 2020 2020 7374 6174 733a  Zone].    stats:
-000067b0: 2043 616d 6572 6153 7461 7473 0a20 2020   CameraStats.   
-000067c0: 2066 6561 7475 7265 5f66 6c61 6773 3a20   feature_flags: 
-000067d0: 4361 6d65 7261 4665 6174 7572 6546 6c61  CameraFeatureFla
-000067e0: 6773 0a20 2020 206c 6364 5f6d 6573 7361  gs.    lcd_messa
-000067f0: 6765 3a20 4f70 7469 6f6e 616c 5b4c 4344  ge: Optional[LCD
-00006800: 4d65 7373 6167 655d 0a20 2020 206c 656e  Message].    len
-00006810: 7365 733a 206c 6973 745b 4361 6d65 7261  ses: list[Camera
-00006820: 4c65 6e73 6573 5d0a 2020 2020 706c 6174  Lenses].    plat
-00006830: 666f 726d 3a20 7374 720a 2020 2020 6861  form: str.    ha
-00006840: 735f 7370 6561 6b65 723a 2062 6f6f 6c0a  s_speaker: bool.
-00006850: 2020 2020 6861 735f 7769 6669 3a20 626f      has_wifi: bo
-00006860: 6f6c 0a20 2020 2061 7564 696f 5f62 6974  ol.    audio_bit
-00006870: 7261 7465 3a20 696e 740a 2020 2020 6361  rate: int.    ca
-00006880: 6e5f 6d61 6e61 6765 3a20 626f 6f6c 0a20  n_manage: bool. 
-00006890: 2020 2069 735f 6d61 6e61 6765 643a 2062     is_managed: b
-000068a0: 6f6f 6c0a 2020 2020 766f 6c74 6167 653a  ool.    voltage:
-000068b0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-000068c0: 0a20 2020 2023 2072 6571 7569 7265 7320  .    # requires 
-000068d0: 312e 3231 2b0a 2020 2020 6973 5f70 6f6f  1.21+.    is_poo
-000068e0: 725f 6e65 7477 6f72 6b3a 204f 7074 696f  r_network: Optio
-000068f0: 6e61 6c5b 626f 6f6c 5d0a 2020 2020 6973  nal[bool].    is
-00006900: 5f77 6972 656c 6573 735f 7570 6c69 6e6b  _wireless_uplink
-00006910: 5f65 6e61 626c 6564 3a20 4f70 7469 6f6e  _enabled: Option
-00006920: 616c 5b62 6f6f 6c5d 0a20 2020 2023 2072  al[bool].    # r
-00006930: 6571 7569 7265 7320 322e 362e 3133 2b0a  equires 2.6.13+.
-00006940: 2020 2020 686f 6d65 6b69 745f 7365 7474      homekit_sett
-00006950: 696e 6773 3a20 4f70 7469 6f6e 616c 5b43  ings: Optional[C
-00006960: 616d 6572 6148 6f6d 656b 6974 5365 7474  ameraHomekitSett
-00006970: 696e 6773 5d20 3d20 4e6f 6e65 0a20 2020  ings] = None.   
-00006980: 2023 2072 6571 7569 7265 7320 322e 362e   # requires 2.6.
-00006990: 3137 2b0a 2020 2020 6170 5f6d 676d 745f  17+.    ap_mgmt_
-000069a0: 6970 3a20 4f70 7469 6f6e 616c 5b49 5076  ip: Optional[IPv
-000069b0: 3441 6464 7265 7373 5d20 3d20 4e6f 6e65  4Address] = None
-000069c0: 0a20 2020 2023 2072 6571 7569 7265 7320  .    # requires 
-000069d0: 322e 372e 352b 0a20 2020 2069 735f 7761  2.7.5+.    is_wa
-000069e0: 7465 7270 726f 6f66 5f63 6173 655f 6174  terproof_case_at
-000069f0: 7461 6368 6564 3a20 4f70 7469 6f6e 616c  tached: Optional
-00006a00: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 2020  [bool] = None.  
-00006a10: 2020 6c61 7374 5f64 6973 636f 6e6e 6563    last_disconnec
-00006a20: 743a 204f 7074 696f 6e61 6c5b 6461 7465  t: Optional[date
-00006a30: 7469 6d65 5d20 3d20 4e6f 6e65 0a20 2020  time] = None.   
-00006a40: 2023 2072 6571 7569 7265 7320 322e 382e   # requires 2.8.
-00006a50: 3134 2b0a 2020 2020 6973 5f32 6b3a 204f  14+.    is_2k: O
-00006a60: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00006a70: 4e6f 6e65 0a20 2020 2069 735f 346b 3a20  None.    is_4k: 
-00006a80: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00006a90: 204e 6f6e 650a 2020 2020 7573 655f 676c   None.    use_gl
-00006aa0: 6f62 616c 3a20 4f70 7469 6f6e 616c 5b62  obal: Optional[b
-00006ab0: 6f6f 6c5d 203d 204e 6f6e 650a 2020 2020  ool] = None.    
-00006ac0: 2320 7265 7175 6972 6573 2032 2e38 2e32  # requires 2.8.2
-00006ad0: 322b 0a20 2020 2075 7365 725f 636f 6e66  2+.    user_conf
-00006ae0: 6967 7572 6564 5f61 703a 204f 7074 696f  igured_ap: Optio
-00006af0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00006b00: 0a20 2020 2023 2072 6571 7569 7265 7320  .    # requires 
-00006b10: 322e 392e 3230 2b0a 2020 2020 6861 735f  2.9.20+.    has_
-00006b20: 7265 636f 7264 696e 6773 3a20 4f70 7469  recordings: Opti
-00006b30: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00006b40: 650a 2020 2020 2320 7265 7175 6972 6573  e.    # requires
-00006b50: 2032 2e31 302e 3130 2b0a 2020 2020 6973   2.10.10+.    is
-00006b60: 5f70 747a 3a20 4f70 7469 6f6e 616c 5b62  _ptz: Optional[b
-00006b70: 6f6f 6c5d 203d 204e 6f6e 650a 2020 2020  ool] = None.    
-00006b80: 2320 7265 7175 6972 6573 2032 2e31 312e  # requires 2.11.
-00006b90: 3133 2b0a 2020 2020 6175 6469 6f5f 7365  13+.    audio_se
-00006ba0: 7474 696e 6773 3a20 4f70 7469 6f6e 616c  ttings: Optional
-00006bb0: 5b43 616d 6572 6141 7564 696f 5365 7474  [CameraAudioSett
-00006bc0: 696e 6773 5d20 3d20 4e6f 6e65 0a0a 2020  ings] = None..  
-00006bd0: 2020 2320 544f 444f 3a20 7573 6564 2066    # TODO: used f
-00006be0: 6f72 2061 646f 7074 696e 670a 2020 2020  or adopting.    
-00006bf0: 2320 6170 4d61 6320 7265 6164 206f 6e6c  # apMac read onl
-00006c00: 790a 2020 2020 2320 6170 5273 7369 2072  y.    # apRssi r
-00006c10: 6561 6420 6f6e 6c79 0a20 2020 2023 2065  ead only.    # e
-00006c20: 6c65 6d65 6e74 496e 666f 2072 6561 6420  lementInfo read 
-00006c30: 6f6e 6c79 0a0a 2020 2020 2320 544f 444f  only..    # TODO
-00006c40: 3a0a 2020 2020 2320 6c61 7374 5072 6976  :.    # lastPriv
-00006c50: 6163 795a 6f6e 6550 6f73 6974 696f 6e49  acyZonePositionI
-00006c60: 640a 2020 2020 2320 736d 6172 7444 6574  d.    # smartDet
-00006c70: 6563 744c 696e 6573 0a20 2020 2023 2073  ectLines.    # s
-00006c80: 7472 6561 6d53 6861 7269 6e67 2072 6561  treamSharing rea
-00006c90: 6420 6f6e 6c79 0a20 2020 2023 2073 746f  d only.    # sto
-00006ca0: 7053 7472 6561 6d4c 6576 656c 0a20 2020  pStreamLevel.   
-00006cb0: 2023 2075 706c 696e 6b44 6576 6963 650a   # uplinkDevice.
-00006cc0: 2020 2020 2320 7265 636f 7264 696e 6753      # recordingS
-00006cd0: 6368 6564 756c 6573 5632 0a0a 2020 2020  chedulesV2..    
-00006ce0: 2320 6e6f 7420 6469 7265 6374 6c79 2066  # not directly f
-00006cf0: 726f 6d20 556e 6946 690a 2020 2020 6c61  rom UniFi.    la
-00006d00: 7374 5f72 696e 675f 6576 656e 745f 6964  st_ring_event_id
-00006d10: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00006d20: 3d20 4e6f 6e65 0a20 2020 206c 6173 745f  = None.    last_
-00006d30: 736d 6172 745f 6465 7465 6374 3a20 4f70  smart_detect: Op
-00006d40: 7469 6f6e 616c 5b64 6174 6574 696d 655d  tional[datetime]
-00006d50: 203d 204e 6f6e 650a 2020 2020 6c61 7374   = None.    last
-00006d60: 5f73 6d61 7274 5f61 7564 696f 5f64 6574  _smart_audio_det
-00006d70: 6563 743a 204f 7074 696f 6e61 6c5b 6461  ect: Optional[da
-00006d80: 7465 7469 6d65 5d20 3d20 4e6f 6e65 0a20  tetime] = None. 
-00006d90: 2020 206c 6173 745f 736d 6172 745f 6465     last_smart_de
-00006da0: 7465 6374 5f65 7665 6e74 5f69 643a 204f  tect_event_id: O
-00006db0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00006dc0: 6f6e 650a 2020 2020 6c61 7374 5f73 6d61  one.    last_sma
-00006dd0: 7274 5f61 7564 696f 5f64 6574 6563 745f  rt_audio_detect_
-00006de0: 6576 656e 745f 6964 3a20 4f70 7469 6f6e  event_id: Option
-00006df0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-00006e00: 2020 206c 6173 745f 736d 6172 745f 6465     last_smart_de
-00006e10: 7465 6374 733a 2064 6963 745b 536d 6172  tects: dict[Smar
-00006e20: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-00006e30: 652c 2064 6174 6574 696d 655d 203d 207b  e, datetime] = {
-00006e40: 7d0a 2020 2020 6c61 7374 5f73 6d61 7274  }.    last_smart
-00006e50: 5f61 7564 696f 5f64 6574 6563 7473 3a20  _audio_detects: 
-00006e60: 6469 6374 5b53 6d61 7274 4465 7465 6374  dict[SmartDetect
-00006e70: 4175 6469 6f54 7970 652c 2064 6174 6574  AudioType, datet
-00006e80: 696d 655d 203d 207b 7d0a 2020 2020 6c61  ime] = {}.    la
-00006e90: 7374 5f73 6d61 7274 5f64 6574 6563 745f  st_smart_detect_
-00006ea0: 6576 656e 745f 6964 733a 2064 6963 745b  event_ids: dict[
-00006eb0: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
-00006ec0: 7454 7970 652c 2073 7472 5d20 3d20 7b7d  tType, str] = {}
-00006ed0: 0a20 2020 206c 6173 745f 736d 6172 745f  .    last_smart_
-00006ee0: 6175 6469 6f5f 6465 7465 6374 5f65 7665  audio_detect_eve
-00006ef0: 6e74 5f69 6473 3a20 6469 6374 5b53 6d61  nt_ids: dict[Sma
-00006f00: 7274 4465 7465 6374 4175 6469 6f54 7970  rtDetectAudioTyp
-00006f10: 652c 2073 7472 5d20 3d20 7b7d 0a20 2020  e, str] = {}.   
-00006f20: 2074 616c 6b62 6163 6b5f 7374 7265 616d   talkback_stream
-00006f30: 3a20 4f70 7469 6f6e 616c 5b54 616c 6b62  : Optional[Talkb
-00006f40: 6163 6b53 7472 6561 6d5d 203d 204e 6f6e  ackStream] = Non
-00006f50: 650a 2020 2020 5f6c 6173 745f 7269 6e67  e.    _last_ring
-00006f60: 5f74 696d 656f 7574 3a20 4f70 7469 6f6e  _timeout: Option
-00006f70: 616c 5b64 6174 6574 696d 655d 203d 2050  al[datetime] = P
-00006f80: 7269 7661 7465 4174 7472 284e 6f6e 6529  rivateAttr(None)
-00006f90: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00006fa0: 6f64 0a20 2020 2040 6361 6368 650a 2020  od.    @cache.  
-00006fb0: 2020 6465 6620 5f67 6574 5f75 6e69 6669    def _get_unifi
-00006fc0: 5f72 656d 6170 7328 636c 7329 202d 3e20  _remaps(cls) -> 
-00006fd0: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
-00006fe0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00006ff0: 2a2a 7375 7065 7228 292e 5f67 6574 5f75  **super()._get_u
-00007000: 6e69 6669 5f72 656d 6170 7328 292c 2022  nifi_remaps(), "
-00007010: 6973 324b 223a 2022 6973 326b 222c 2022  is2K": "is2k", "
-00007020: 6973 344b 223a 2022 6973 346b 227d 0a0a  is4K": "is4k"}..
-00007030: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00007040: 0a20 2020 2040 6361 6368 650a 2020 2020  .    @cache.    
-00007050: 6465 6620 5f67 6574 5f65 7863 6c75 6465  def _get_exclude
-00007060: 645f 6368 616e 6765 645f 6669 656c 6473  d_changed_fields
-00007070: 2863 6c73 2920 2d3e 2073 6574 5b73 7472  (cls) -> set[str
-00007080: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-00007090: 6e20 7375 7065 7228 292e 5f67 6574 5f65  n super()._get_e
-000070a0: 7863 6c75 6465 645f 6368 616e 6765 645f  xcluded_changed_
-000070b0: 6669 656c 6473 2829 207c 207b 0a20 2020  fields() | {.   
-000070c0: 2020 2020 2020 2020 2022 6c61 7374 5f72           "last_r
-000070d0: 696e 675f 6576 656e 745f 6964 222c 0a20  ing_event_id",. 
-000070e0: 2020 2020 2020 2020 2020 2022 6c61 7374             "last
-000070f0: 5f73 6d61 7274 5f64 6574 6563 7422 2c0a  _smart_detect",.
-00007100: 2020 2020 2020 2020 2020 2020 226c 6173              "las
-00007110: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
-00007120: 7465 6374 222c 0a20 2020 2020 2020 2020  tect",.         
-00007130: 2020 2022 6c61 7374 5f73 6d61 7274 5f64     "last_smart_d
-00007140: 6574 6563 745f 6576 656e 745f 6964 222c  etect_event_id",
-00007150: 0a20 2020 2020 2020 2020 2020 2022 6c61  .            "la
-00007160: 7374 5f73 6d61 7274 5f61 7564 696f 5f64  st_smart_audio_d
-00007170: 6574 6563 745f 6576 656e 745f 6964 222c  etect_event_id",
-00007180: 0a20 2020 2020 2020 2020 2020 2022 6c61  .            "la
-00007190: 7374 5f73 6d61 7274 5f64 6574 6563 7473  st_smart_detects
-000071a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000071b0: 6c61 7374 5f73 6d61 7274 5f61 7564 696f  last_smart_audio
-000071c0: 5f64 6574 6563 7473 222c 0a20 2020 2020  _detects",.     
-000071d0: 2020 2020 2020 2022 6c61 7374 5f73 6d61         "last_sma
-000071e0: 7274 5f64 6574 6563 745f 6576 656e 745f  rt_detect_event_
-000071f0: 6964 7322 2c0a 2020 2020 2020 2020 2020  ids",.          
-00007200: 2020 226c 6173 745f 736d 6172 745f 6175    "last_smart_au
-00007210: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
-00007220: 5f69 6473 222c 0a20 2020 2020 2020 2020  _ids",.         
-00007230: 2020 2022 7461 6c6b 6261 636b 5f73 7472     "talkback_str
-00007240: 6561 6d22 2c0a 2020 2020 2020 2020 7d0a  eam",.        }.
-00007250: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00007260: 640a 2020 2020 4063 6163 6865 0a20 2020  d.    @cache.   
-00007270: 2064 6566 205f 6765 745f 7265 6164 5f6f   def _get_read_o
-00007280: 6e6c 795f 6669 656c 6473 2863 6c73 2920  nly_fields(cls) 
-00007290: 2d3e 2073 6574 5b73 7472 5d3a 0a20 2020  -> set[str]:.   
-000072a0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000072b0: 7228 292e 5f67 6574 5f72 6561 645f 6f6e  r()._get_read_on
-000072c0: 6c79 5f66 6965 6c64 7328 2920 7c20 7b0a  ly_fields() | {.
-000072d0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-000072e0: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-000072f0: 2022 6973 4465 6c65 7469 6e67 222c 0a20   "isDeleting",. 
-00007300: 2020 2020 2020 2020 2020 2022 6973 5265             "isRe
-00007310: 636f 7264 696e 6722 2c0a 2020 2020 2020  cording",.      
-00007320: 2020 2020 2020 2269 734d 6f74 696f 6e44        "isMotionD
-00007330: 6574 6563 7465 6422 2c0a 2020 2020 2020  etected",.      
-00007340: 2020 2020 2020 2269 7353 6d61 7274 4465        "isSmartDe
-00007350: 7465 6374 6564 222c 0a20 2020 2020 2020  tected",.       
-00007360: 2020 2020 2022 7068 7952 6174 6522 2c0a       "phyRate",.
-00007370: 2020 2020 2020 2020 2020 2020 2269 7350              "isP
-00007380: 726f 6269 6e67 466f 7257 6966 6922 2c0a  robingForWifi",.
-00007390: 2020 2020 2020 2020 2020 2020 226c 6173              "las
-000073a0: 7452 696e 6722 2c0a 2020 2020 2020 2020  tRing",.        
-000073b0: 2020 2020 2269 734c 6976 6548 6561 746d      "isLiveHeatm
-000073c0: 6170 456e 6162 6c65 6422 2c0a 2020 2020  apEnabled",.    
-000073d0: 2020 2020 2020 2020 2276 6964 656f 5265          "videoRe
-000073e0: 636f 6e66 6967 7572 6174 696f 6e49 6e50  configurationInP
-000073f0: 726f 6772 6573 7322 2c0a 2020 2020 2020  rogress",.      
-00007400: 2020 2020 2020 226c 656e 7365 7322 2c0a        "lenses",.
-00007410: 2020 2020 2020 2020 2020 2020 2269 7350              "isP
-00007420: 6f6f 724e 6574 776f 726b 222c 0a20 2020  oorNetwork",.   
-00007430: 2020 2020 2020 2020 2022 6665 6174 7572           "featur
-00007440: 6546 6c61 6773 222c 0a20 2020 2020 2020  eFlags",.       
-00007450: 207d 0a0a 2020 2020 4063 6c61 7373 6d65   }..    @classme
-00007460: 7468 6f64 0a20 2020 2064 6566 2075 6e69  thod.    def uni
-00007470: 6669 5f64 6963 745f 746f 5f64 6963 7428  fi_dict_to_dict(
-00007480: 636c 732c 2064 6174 613a 2064 6963 745b  cls, data: dict[
-00007490: 7374 722c 2041 6e79 5d29 202d 3e20 6469  str, Any]) -> di
-000074a0: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
-000074b0: 2020 2020 2020 2320 4c43 4420 6d65 7373        # LCD mess
-000074c0: 6167 6573 2063 6f6d 6573 2062 6163 6b20  ages comes back 
-000074d0: 6173 2065 6d70 7479 2064 6963 7420 7b7d  as empty dict {}
-000074e0: 0a20 2020 2020 2020 2069 6620 226c 6364  .        if "lcd
-000074f0: 4d65 7373 6167 6522 2069 6e20 6461 7461  Message" in data
-00007500: 2061 6e64 206c 656e 2864 6174 615b 226c   and len(data["l
-00007510: 6364 4d65 7373 6167 6522 5d2e 6b65 7973  cdMessage"].keys
-00007520: 2829 2920 3d3d 2030 3a0a 2020 2020 2020  ()) == 0:.      
-00007530: 2020 2020 2020 6465 6c20 6461 7461 5b22        del data["
-00007540: 6c63 644d 6573 7361 6765 225d 0a20 2020  lcdMessage"].   
-00007550: 2020 2020 2069 6620 2263 6869 6d65 4475       if "chimeDu
-00007560: 7261 7469 6f6e 2220 696e 2064 6174 6120  ration" in data 
-00007570: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-00007580: 6365 2864 6174 615b 2263 6869 6d65 4475  ce(data["chimeDu
-00007590: 7261 7469 6f6e 225d 2c20 7469 6d65 6465  ration"], timede
-000075a0: 6c74 6129 3a0a 2020 2020 2020 2020 2020  lta):.          
-000075b0: 2020 6461 7461 5b22 6368 696d 6544 7572    data["chimeDur
-000075c0: 6174 696f 6e22 5d20 3d20 7469 6d65 6465  ation"] = timede
-000075d0: 6c74 6128 6d69 6c6c 6973 6563 6f6e 6473  lta(milliseconds
-000075e0: 3d64 6174 615b 2263 6869 6d65 4475 7261  =data["chimeDura
-000075f0: 7469 6f6e 225d 290a 0a20 2020 2020 2020  tion"])..       
-00007600: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00007610: 756e 6966 695f 6469 6374 5f74 6f5f 6469  unifi_dict_to_di
-00007620: 6374 2864 6174 6129 0a0a 2020 2020 6465  ct(data)..    de
-00007630: 6620 756e 6966 695f 6469 6374 280a 2020  f unifi_dict(.  
-00007640: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00007650: 2020 2020 6461 7461 3a20 4f70 7469 6f6e      data: Option
-00007660: 616c 5b64 6963 745b 7374 722c 2041 6e79  al[dict[str, Any
-00007670: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00007680: 2020 2065 7863 6c75 6465 3a20 4f70 7469     exclude: Opti
-00007690: 6f6e 616c 5b73 6574 5b73 7472 5d5d 203d  onal[set[str]] =
-000076a0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-000076b0: 6469 6374 5b73 7472 2c20 416e 795d 3a0a  dict[str, Any]:.
-000076c0: 2020 2020 2020 2020 6966 2064 6174 6120          if data 
-000076d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000076e0: 2020 2020 2020 2020 2069 6620 226d 6f74           if "mot
-000076f0: 696f 6e5f 7a6f 6e65 7322 2069 6e20 6461  ion_zones" in da
-00007700: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00007710: 2020 2020 6461 7461 5b22 6d6f 7469 6f6e      data["motion
-00007720: 5f7a 6f6e 6573 225d 203d 205b 0a20 2020  _zones"] = [.   
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 204d 6f74 696f 6e5a 6f6e 6528 2a2a 7a29   MotionZone(**z)
-00007750: 2e75 6e69 6669 5f64 6963 7428 2920 666f  .unifi_dict() fo
-00007760: 7220 7a20 696e 2064 6174 615b 226d 6f74  r z in data["mot
-00007770: 696f 6e5f 7a6f 6e65 7322 5d0a 2020 2020  ion_zones"].    
-00007780: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00007790: 2020 2020 2020 2020 2020 6966 2022 7072            if "pr
-000077a0: 6976 6163 795f 7a6f 6e65 7322 2069 6e20  ivacy_zones" in 
-000077b0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-000077c0: 2020 2020 2020 6461 7461 5b22 7072 6976        data["priv
-000077d0: 6163 795f 7a6f 6e65 7322 5d20 3d20 5b0a  acy_zones"] = [.
-000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077f0: 2020 2020 4361 6d65 7261 5a6f 6e65 282a      CameraZone(*
-00007800: 2a7a 292e 756e 6966 695f 6469 6374 2829  *z).unifi_dict()
-00007810: 2066 6f72 207a 2069 6e20 6461 7461 5b22   for z in data["
-00007820: 7072 6976 6163 795f 7a6f 6e65 7322 5d0a  privacy_zones"].
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-00007850: 2022 736d 6172 745f 6465 7465 6374 5f7a   "smart_detect_z
-00007860: 6f6e 6573 2220 696e 2064 6174 613a 0a20  ones" in data:. 
-00007870: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007880: 6174 615b 2273 6d61 7274 5f64 6574 6563  ata["smart_detec
-00007890: 745f 7a6f 6e65 7322 5d20 3d20 5b0a 2020  t_zones"] = [.  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 2020 536d 6172 744d 6f74 696f 6e5a 6f6e    SmartMotionZon
-000078c0: 6528 2a2a 7a29 2e75 6e69 6669 5f64 6963  e(**z).unifi_dic
-000078d0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000078e0: 2020 2020 2020 2020 666f 7220 7a20 696e          for z in
-000078f0: 2064 6174 615b 2273 6d61 7274 5f64 6574   data["smart_det
-00007900: 6563 745f 7a6f 6e65 7322 5d0a 2020 2020  ect_zones"].    
-00007910: 2020 2020 2020 2020 2020 2020 5d0a 0a20              ].. 
-00007920: 2020 2020 2020 2064 6174 6120 3d20 7375         data = su
-00007930: 7065 7228 292e 756e 6966 695f 6469 6374  per().unifi_dict
-00007940: 2864 6174 613d 6461 7461 2c20 6578 636c  (data=data, excl
-00007950: 7564 653d 6578 636c 7564 6529 0a0a 2020  ude=exclude)..  
-00007960: 2020 2020 2020 6966 2022 6c61 7374 5269        if "lastRi
-00007970: 6e67 4576 656e 7449 6422 2069 6e20 6461  ngEventId" in da
-00007980: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00007990: 6465 6c20 6461 7461 5b22 6c61 7374 5269  del data["lastRi
-000079a0: 6e67 4576 656e 7449 6422 5d0a 2020 2020  ngEventId"].    
-000079b0: 2020 2020 6966 2022 6c61 7374 536d 6172      if "lastSmar
-000079c0: 7444 6574 6563 7422 2069 6e20 6461 7461  tDetect" in data
-000079d0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000079e0: 6c20 6461 7461 5b22 6c61 7374 536d 6172  l data["lastSmar
-000079f0: 7444 6574 6563 7422 5d0a 2020 2020 2020  tDetect"].      
-00007a00: 2020 6966 2022 6c61 7374 536d 6172 7441    if "lastSmartA
-00007a10: 7564 696f 4465 7465 6374 2220 696e 2064  udioDetect" in d
-00007a20: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00007a30: 2064 656c 2064 6174 615b 226c 6173 7453   del data["lastS
-00007a40: 6d61 7274 4175 6469 6f44 6574 6563 7422  martAudioDetect"
-00007a50: 5d0a 2020 2020 2020 2020 6966 2022 6c61  ].        if "la
-00007a60: 7374 536d 6172 7444 6574 6563 7445 7665  stSmartDetectEve
-00007a70: 6e74 4964 2220 696e 2064 6174 613a 0a20  ntId" in data:. 
-00007a80: 2020 2020 2020 2020 2020 2064 656c 2064             del d
-00007a90: 6174 615b 226c 6173 7453 6d61 7274 4465  ata["lastSmartDe
-00007aa0: 7465 6374 4576 656e 7449 6422 5d0a 2020  tectEventId"].  
-00007ab0: 2020 2020 2020 6966 2022 6c61 7374 536d        if "lastSm
-00007ac0: 6172 7441 7564 696f 4465 7465 6374 4576  artAudioDetectEv
-00007ad0: 656e 7449 6422 2069 6e20 6461 7461 3a0a  entId" in data:.
-00007ae0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00007af0: 6461 7461 5b22 6c61 7374 536d 6172 7441  data["lastSmartA
-00007b00: 7564 696f 4465 7465 6374 4576 656e 7449  udioDetectEventI
-00007b10: 6422 5d0a 2020 2020 2020 2020 6966 2022  d"].        if "
-00007b20: 6c61 7374 536d 6172 7444 6574 6563 7473  lastSmartDetects
-00007b30: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
-00007b40: 2020 2020 2020 2064 656c 2064 6174 615b         del data[
-00007b50: 226c 6173 7453 6d61 7274 4465 7465 6374  "lastSmartDetect
-00007b60: 7322 5d0a 2020 2020 2020 2020 6966 2022  s"].        if "
-00007b70: 6c61 7374 536d 6172 7441 7564 696f 4465  lastSmartAudioDe
-00007b80: 7465 6374 7322 2069 6e20 6461 7461 3a0a  tects" in data:.
-00007b90: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00007ba0: 6461 7461 5b22 6c61 7374 536d 6172 7441  data["lastSmartA
-00007bb0: 7564 696f 4465 7465 6374 7322 5d0a 2020  udioDetects"].  
-00007bc0: 2020 2020 2020 6966 2022 6c61 7374 536d        if "lastSm
-00007bd0: 6172 7444 6574 6563 7445 7665 6e74 4964  artDetectEventId
-00007be0: 7322 2069 6e20 6461 7461 3a0a 2020 2020  s" in data:.    
-00007bf0: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
-00007c00: 5b22 6c61 7374 536d 6172 7444 6574 6563  ["lastSmartDetec
-00007c10: 7445 7665 6e74 4964 7322 5d0a 2020 2020  tEventIds"].    
-00007c20: 2020 2020 6966 2022 6c61 7374 536d 6172      if "lastSmar
-00007c30: 7441 7564 696f 4465 7465 6374 4576 656e  tAudioDetectEven
-00007c40: 7449 6473 2220 696e 2064 6174 613a 0a20  tIds" in data:. 
-00007c50: 2020 2020 2020 2020 2020 2064 656c 2064             del d
-00007c60: 6174 615b 226c 6173 7453 6d61 7274 4175  ata["lastSmartAu
-00007c70: 6469 6f44 6574 6563 7445 7665 6e74 4964  dioDetectEventId
-00007c80: 7322 5d0a 2020 2020 2020 2020 6966 2022  s"].        if "
-00007c90: 7461 6c6b 6261 636b 5374 7265 616d 2220  talkbackStream" 
-00007ca0: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
-00007cb0: 2020 2020 2064 656c 2064 6174 615b 2274       del data["t
-00007cc0: 616c 6b62 6163 6b53 7472 6561 6d22 5d0a  alkbackStream"].
-00007cd0: 2020 2020 2020 2020 6966 2022 6c63 644d          if "lcdM
-00007ce0: 6573 7361 6765 2220 696e 2064 6174 6120  essage" in data 
-00007cf0: 616e 6420 6461 7461 5b22 6c63 644d 6573  and data["lcdMes
-00007d00: 7361 6765 225d 2069 7320 4e6f 6e65 3a0a  sage"] is None:.
-00007d10: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00007d20: 5b22 6c63 644d 6573 7361 6765 225d 203d  ["lcdMessage"] =
-00007d30: 207b 7d0a 0a20 2020 2020 2020 2072 6574   {}..        ret
-00007d40: 7572 6e20 6461 7461 0a0a 2020 2020 6465  urn data..    de
-00007d50: 6620 6765 745f 6368 616e 6765 6428 7365  f get_changed(se
-00007d60: 6c66 2c20 6461 7461 5f62 6566 6f72 655f  lf, data_before_
-00007d70: 6368 616e 6765 733a 2064 6963 745b 7374  changes: dict[st
-00007d80: 722c 2041 6e79 5d29 202d 3e20 6469 6374  r, Any]) -> dict
-00007d90: 5b73 7472 2c20 416e 795d 3a0a 2020 2020  [str, Any]:.    
-00007da0: 2020 2020 7570 6461 7465 6420 3d20 7375      updated = su
-00007db0: 7065 7228 292e 6765 745f 6368 616e 6765  per().get_change
-00007dc0: 6428 6461 7461 5f62 6566 6f72 655f 6368  d(data_before_ch
-00007dd0: 616e 6765 7329 0a0a 2020 2020 2020 2020  anges)..        
-00007de0: 6966 2022 6c63 645f 6d65 7373 6167 6522  if "lcd_message"
-00007df0: 2069 6e20 7570 6461 7465 643a 0a20 2020   in updated:.   
-00007e00: 2020 2020 2020 2020 206c 6364 5f6d 6573           lcd_mes
-00007e10: 7361 6765 203d 2075 7064 6174 6564 5b22  sage = updated["
-00007e20: 6c63 645f 6d65 7373 6167 6522 5d0a 2020  lcd_message"].  
-00007e30: 2020 2020 2020 2020 2020 2320 746f 2022            # to "
-00007e40: 636c 6561 7222 204c 4344 206d 6573 7361  clear" LCD messa
-00007e50: 6765 2c20 7365 7420 7265 7365 745f 6174  ge, set reset_at
-00007e60: 2074 6f20 6120 7469 6d65 2069 6e20 7468   to a time in th
-00007e70: 6520 7061 7374 0a20 2020 2020 2020 2020  e past.         
-00007e80: 2020 2069 6620 6c63 645f 6d65 7373 6167     if lcd_messag
-00007e90: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00007ea0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-00007eb0: 6564 5b22 6c63 645f 6d65 7373 6167 6522  ed["lcd_message"
-00007ec0: 5d20 3d20 7b22 7265 7365 745f 6174 223a  ] = {"reset_at":
-00007ed0: 2075 7463 5f6e 6f77 2829 202d 2074 696d   utc_now() - tim
-00007ee0: 6564 656c 7461 2873 6563 6f6e 6473 3d31  edelta(seconds=1
-00007ef0: 3029 7d0a 2020 2020 2020 2020 2020 2020  0)}.            
-00007f00: 2320 6f74 6865 7277 6973 652c 2070 6173  # otherwise, pas
-00007f10: 7320 6675 6c6c 204c 4344 206d 6573 7361  s full LCD messa
-00007f20: 6765 2074 6f20 7072 6576 656e 7420 6973  ge to prevent is
-00007f30: 7375 6573 0a20 2020 2020 2020 2020 2020  sues.           
-00007f40: 2065 6c69 6620 7365 6c66 2e6c 6364 5f6d   elif self.lcd_m
-00007f50: 6573 7361 6765 2069 7320 6e6f 7420 4e6f  essage is not No
-00007f60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007f70: 2020 2020 7570 6461 7465 645b 226c 6364      updated["lcd
-00007f80: 5f6d 6573 7361 6765 225d 203d 2073 656c  _message"] = sel
-00007f90: 662e 6c63 645f 6d65 7373 6167 652e 6469  f.lcd_message.di
-00007fa0: 6374 2829 0a0a 2020 2020 2020 2020 2020  ct()..          
-00007fb0: 2020 2320 6966 2072 6573 6574 5f61 7420    # if reset_at 
-00007fc0: 6973 206e 6f74 2070 6173 7365 6420 696e  is not passed in
-00007fd0: 2c20 6974 2077 696c 6c20 6465 6661 756c  , it will defaul
-00007fe0: 7420 746f 2072 6573 6574 2069 6e20 3120  t to reset in 1 
-00007ff0: 6d69 6e75 7465 0a20 2020 2020 2020 2020  minute.         
-00008000: 2020 2069 6620 6c63 645f 6d65 7373 6167     if lcd_messag
-00008010: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-00008020: 6420 2272 6573 6574 5f61 7422 206e 6f74  d "reset_at" not
-00008030: 2069 6e20 6c63 645f 6d65 7373 6167 653a   in lcd_message:
-00008040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008050: 2069 6620 7365 6c66 2e6c 6364 5f6d 6573   if self.lcd_mes
-00008060: 7361 6765 2069 7320 4e6f 6e65 3a0a 2020  sage is None:.  
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 2020 7570 6461 7465 645b 226c 6364 5f6d    updated["lcd_m
-00008090: 6573 7361 6765 225d 5b22 7265 7365 745f  essage"]["reset_
-000080a0: 6174 225d 203d 204e 6f6e 650a 2020 2020  at"] = None.    
-000080b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000080c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000080d0: 2020 2020 2020 7570 6461 7465 645b 226c        updated["l
-000080e0: 6364 5f6d 6573 7361 6765 225d 5b22 7265  cd_message"]["re
-000080f0: 7365 745f 6174 225d 203d 2073 656c 662e  set_at"] = self.
-00008100: 6c63 645f 6d65 7373 6167 652e 7265 7365  lcd_message.rese
-00008110: 745f 6174 0a0a 2020 2020 2020 2020 7265  t_at..        re
-00008120: 7475 726e 2075 7064 6174 6564 0a0a 2020  turn updated..  
-00008130: 2020 6465 6620 7570 6461 7465 5f66 726f    def update_fro
-00008140: 6d5f 6469 6374 2873 656c 662c 2064 6174  m_dict(self, dat
-00008150: 613a 2064 6963 745b 7374 722c 2041 6e79  a: dict[str, Any
-00008160: 5d29 202d 3e20 4361 6d65 7261 3a0a 2020  ]) -> Camera:.  
-00008170: 2020 2020 2020 2320 6120 6d65 7373 6167        # a messag
-00008180: 6520 696e 2074 6865 2070 6173 7420 6973  e in the past is
-00008190: 2061 6374 7561 6c6c 7920 6120 7369 6e67   actually a sing
-000081a0: 616c 2074 6f20 7769 7065 2074 6865 206d  al to wipe the m
-000081b0: 6573 7361 6765 0a20 2020 2020 2020 2072  essage.        r
-000081c0: 6573 6574 5f61 7420 3d20 6461 7461 2e67  eset_at = data.g
-000081d0: 6574 2822 6c63 645f 6d65 7373 6167 6522  et("lcd_message"
-000081e0: 2c20 7b7d 292e 6765 7428 2272 6573 6574  , {}).get("reset
-000081f0: 5f61 7422 290a 2020 2020 2020 2020 6966  _at").        if
-00008200: 2072 6573 6574 5f61 7420 6973 206e 6f74   reset_at is not
-00008210: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008220: 2020 2072 6573 6574 5f61 7420 3d20 6672     reset_at = fr
-00008230: 6f6d 5f6a 735f 7469 6d65 2872 6573 6574  om_js_time(reset
-00008240: 5f61 7429 0a20 2020 2020 2020 2020 2020  _at).           
-00008250: 2069 6620 7574 635f 6e6f 7728 2920 3e20   if utc_now() > 
-00008260: 7265 7365 745f 6174 3a0a 2020 2020 2020  reset_at:.      
-00008270: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-00008280: 6c63 645f 6d65 7373 6167 6522 5d20 3d20  lcd_message"] = 
-00008290: 4e6f 6e65 0a0a 2020 2020 2020 2020 7265  None..        re
-000082a0: 7475 726e 2073 7570 6572 2829 2e75 7064  turn super().upd
-000082b0: 6174 655f 6672 6f6d 5f64 6963 7428 6461  ate_from_dict(da
-000082c0: 7461 290a 0a20 2020 2040 7072 6f70 6572  ta)..    @proper
-000082d0: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
-000082e0: 7269 6e67 5f65 7665 6e74 2873 656c 6629  ring_event(self)
-000082f0: 202d 3e20 4f70 7469 6f6e 616c 5b45 7665   -> Optional[Eve
-00008300: 6e74 5d3a 0a20 2020 2020 2020 2069 6620  nt]:.        if 
-00008310: 7365 6c66 2e6c 6173 745f 7269 6e67 5f65  self.last_ring_e
-00008320: 7665 6e74 5f69 6420 6973 204e 6f6e 653a  vent_id is None:
-00008330: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008340: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-00008350: 2020 7265 7475 726e 2073 656c 662e 6170    return self.ap
-00008360: 692e 626f 6f74 7374 7261 702e 6576 656e  i.bootstrap.even
-00008370: 7473 2e67 6574 2873 656c 662e 6c61 7374  ts.get(self.last
-00008380: 5f72 696e 675f 6576 656e 745f 6964 290a  _ring_event_id).
-00008390: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000083a0: 2020 2064 6566 206c 6173 745f 736d 6172     def last_smar
-000083b0: 745f 6465 7465 6374 5f65 7665 6e74 2873  t_detect_event(s
-000083c0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-000083d0: 5b45 7665 6e74 5d3a 0a20 2020 2020 2020  [Event]:.       
-000083e0: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
-000083f0: 2073 6d61 7274 2064 6574 6563 7420 6576   smart detect ev
-00008400: 656e 7420 6964 2e22 2222 0a0a 2020 2020  ent id."""..    
-00008410: 2020 2020 6966 2073 656c 662e 6c61 7374      if self.last
-00008420: 5f73 6d61 7274 5f64 6574 6563 745f 6576  _smart_detect_ev
-00008430: 656e 745f 6964 2069 7320 4e6f 6e65 3a0a  ent_id is None:.
-00008440: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008450: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-00008460: 2072 6574 7572 6e20 7365 6c66 2e61 7069   return self.api
-00008470: 2e62 6f6f 7473 7472 6170 2e65 7665 6e74  .bootstrap.event
-00008480: 732e 6765 7428 7365 6c66 2e6c 6173 745f  s.get(self.last_
-00008490: 736d 6172 745f 6465 7465 6374 5f65 7665  smart_detect_eve
-000084a0: 6e74 5f69 6429 0a0a 2020 2020 4070 726f  nt_id)..    @pro
-000084b0: 7065 7274 790a 2020 2020 6465 6620 6864  perty.    def hd
-000084c0: 725f 6d6f 6465 5f64 6973 706c 6179 2873  r_mode_display(s
-000084d0: 656c 6629 202d 3e20 4c69 7465 7261 6c5b  elf) -> Literal[
-000084e0: 2261 7574 6f22 2c20 226f 6666 222c 2022  "auto", "off", "
-000084f0: 616c 7761 7973 225d 3a0a 2020 2020 2020  always"]:.      
-00008500: 2020 2222 2247 6574 2048 4452 206d 6f64    """Get HDR mod
-00008510: 6520 7369 6d69 6c61 7220 746f 2068 6f77  e similar to how
-00008520: 2050 726f 7465 6374 2069 6e74 6572 6661   Protect interfa
-00008530: 6365 2077 6f72 6b73 2e22 2222 0a0a 2020  ce works."""..  
-00008540: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00008550: 662e 6864 725f 6d6f 6465 3a0a 2020 2020  f.hdr_mode:.    
-00008560: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00008570: 6f66 6622 0a20 2020 2020 2020 2069 6620  off".        if 
-00008580: 7365 6c66 2e69 7370 5f73 6574 7469 6e67  self.isp_setting
-00008590: 732e 6864 725f 6d6f 6465 203d 3d20 4844  s.hdr_mode == HD
-000085a0: 524d 6f64 652e 4e4f 524d 414c 3a0a 2020  RMode.NORMAL:.  
-000085b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000085c0: 2022 6175 746f 220a 2020 2020 2020 2020   "auto".        
-000085d0: 7265 7475 726e 2022 616c 7761 7973 220a  return "always".
-000085e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000085f0: 2020 2064 6566 2069 6372 5f6c 7578 5f64     def icr_lux_d
-00008600: 6973 706c 6179 2873 656c 6629 202d 3e20  isplay(self) -> 
-00008610: 696e 7420 7c20 4e6f 6e65 3a0a 2020 2020  int | None:.    
-00008620: 2020 2020 2222 2247 6574 2049 4352 2043      """Get ICR C
-00008630: 7573 746f 6d20 4c75 7820 7661 6c75 6520  ustom Lux value 
-00008640: 7369 6d69 6c61 7220 746f 2068 6f77 2074  similar to how t
-00008650: 6865 2050 726f 7465 6374 2069 6e74 6572  he Protect inter
-00008660: 6661 6365 2077 6f72 6b73 2e22 2222 0a0a  face works."""..
-00008670: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008680: 6973 705f 7365 7474 696e 6773 2e69 6372  isp_settings.icr
-00008690: 5f63 7573 746f 6d5f 7661 6c75 6520 6973  _custom_value is
-000086a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000086b0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-000086c0: 2020 2020 2020 2020 7265 7475 726e 204c          return L
-000086d0: 5558 5f4d 4150 5049 4e47 5f56 414c 5545  UX_MAPPING_VALUE
-000086e0: 535b 3130 202d 2073 656c 662e 6973 705f  S[10 - self.isp_
-000086f0: 7365 7474 696e 6773 2e69 6372 5f63 7573  settings.icr_cus
-00008700: 746f 6d5f 7661 6c75 655d 0a0a 2020 2020  tom_value]..    
-00008710: 6465 6620 6765 745f 6c61 7374 5f73 6d61  def get_last_sma
-00008720: 7274 5f64 6574 6563 745f 6576 656e 7428  rt_detect_event(
-00008730: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008740: 2020 2020 2020 2073 6d61 7274 5f74 7970         smart_typ
-00008750: 653a 2053 6d61 7274 4465 7465 6374 4f62  e: SmartDetectOb
-00008760: 6a65 6374 5479 7065 2c0a 2020 2020 2920  jectType,.    ) 
-00008770: 2d3e 204f 7074 696f 6e61 6c5b 4576 656e  -> Optional[Even
-00008780: 745d 3a0a 2020 2020 2020 2020 2222 2247  t]:.        """G
-00008790: 6574 2074 6865 206c 6173 7420 736d 6172  et the last smar
-000087a0: 7420 6465 7465 6374 2065 7665 6e74 2066  t detect event f
-000087b0: 6f72 2067 6976 656e 2074 7970 652e 2222  or given type.""
-000087c0: 220a 0a20 2020 2020 2020 2065 7665 6e74  "..        event
-000087d0: 5f69 6420 3d20 7365 6c66 2e6c 6173 745f  _id = self.last_
-000087e0: 736d 6172 745f 6465 7465 6374 5f65 7665  smart_detect_eve
-000087f0: 6e74 5f69 6473 2e67 6574 2873 6d61 7274  nt_ids.get(smart
-00008800: 5f74 7970 6529 0a20 2020 2020 2020 2069  _type).        i
-00008810: 6620 6576 656e 745f 6964 2069 7320 4e6f  f event_id is No
-00008820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008830: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00008840: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008850: 2e61 7069 2e62 6f6f 7473 7472 6170 2e65  .api.bootstrap.e
-00008860: 7665 6e74 732e 6765 7428 6576 656e 745f  vents.get(event_
-00008870: 6964 290a 0a20 2020 2040 7072 6f70 6572  id)..    @proper
-00008880: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
-00008890: 736d 6172 745f 6175 6469 6f5f 6465 7465  smart_audio_dete
-000088a0: 6374 5f65 7665 6e74 2873 656c 6629 202d  ct_event(self) -
-000088b0: 3e20 4f70 7469 6f6e 616c 5b45 7665 6e74  > Optional[Event
-000088c0: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-000088d0: 7420 7468 6520 6c61 7374 2073 6d61 7274  t the last smart
-000088e0: 2061 7564 696f 2064 6574 6563 7420 6576   audio detect ev
-000088f0: 656e 7420 6964 2e22 2222 0a0a 2020 2020  ent id."""..    
-00008900: 2020 2020 6966 2073 656c 662e 6c61 7374      if self.last
-00008910: 5f73 6d61 7274 5f61 7564 696f 5f64 6574  _smart_audio_det
-00008920: 6563 745f 6576 656e 745f 6964 2069 7320  ect_event_id is 
-00008930: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008940: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-00008950: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00008960: 6c66 2e61 7069 2e62 6f6f 7473 7472 6170  lf.api.bootstrap
-00008970: 2e65 7665 6e74 732e 6765 7428 7365 6c66  .events.get(self
-00008980: 2e6c 6173 745f 736d 6172 745f 6175 6469  .last_smart_audi
-00008990: 6f5f 6465 7465 6374 5f65 7665 6e74 5f69  o_detect_event_i
-000089a0: 6429 0a0a 2020 2020 6465 6620 6765 745f  d)..    def get_
-000089b0: 6c61 7374 5f73 6d61 7274 5f61 7564 696f  last_smart_audio
-000089c0: 5f64 6574 6563 745f 6576 656e 7428 0a20  _detect_event(. 
-000089d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000089e0: 2020 2020 2073 6d61 7274 5f74 7970 653a       smart_type:
-000089f0: 2053 6d61 7274 4465 7465 6374 4175 6469   SmartDetectAudi
-00008a00: 6f54 7970 652c 0a20 2020 2029 202d 3e20  oType,.    ) -> 
-00008a10: 4f70 7469 6f6e 616c 5b45 7665 6e74 5d3a  Optional[Event]:
-00008a20: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-00008a30: 7468 6520 6c61 7374 2073 6d61 7274 2061  the last smart a
-00008a40: 7564 696f 2064 6574 6563 7420 6576 656e  udio detect even
-00008a50: 7420 666f 7220 6769 7665 6e20 7479 7065  t for given type
-00008a60: 2e22 2222 0a0a 2020 2020 2020 2020 6576  ."""..        ev
-00008a70: 656e 745f 6964 203d 2073 656c 662e 6c61  ent_id = self.la
-00008a80: 7374 5f73 6d61 7274 5f61 7564 696f 5f64  st_smart_audio_d
-00008a90: 6574 6563 745f 6576 656e 745f 6964 732e  etect_event_ids.
-00008aa0: 6765 7428 736d 6172 745f 7479 7065 290a  get(smart_type).
-00008ab0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00008ac0: 5f69 6420 6973 204e 6f6e 653a 0a20 2020  _id is None:.   
-00008ad0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008ae0: 4e6f 6e65 0a0a 2020 2020 2020 2020 7265  None..        re
-00008af0: 7475 726e 2073 656c 662e 6170 692e 626f  turn self.api.bo
-00008b00: 6f74 7374 7261 702e 6576 656e 7473 2e67  otstrap.events.g
-00008b10: 6574 2865 7665 6e74 5f69 6429 0a0a 2020  et(event_id)..  
-00008b20: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00008b30: 6465 6620 7469 6d65 6c61 7073 655f 7572  def timelapse_ur
-00008b40: 6c28 7365 6c66 2920 2d3e 2073 7472 3a0a  l(self) -> str:.
-00008b50: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00008b60: 227b 7365 6c66 2e61 7069 2e62 6173 655f  "{self.api.base_
-00008b70: 7572 6c7d 2f70 726f 7465 6374 2f74 696d  url}/protect/tim
-00008b80: 656c 6170 7365 2f7b 7365 6c66 2e69 647d  elapse/{self.id}
-00008b90: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-00008ba0: 0a20 2020 2064 6566 2069 735f 7072 6976  .    def is_priv
-00008bb0: 6163 795f 6f6e 2873 656c 6629 202d 3e20  acy_on(self) -> 
-00008bc0: 626f 6f6c 3a0a 2020 2020 2020 2020 696e  bool:.        in
-00008bd0: 6465 782c 205f 203d 2073 656c 662e 6765  dex, _ = self.ge
-00008be0: 745f 7072 6976 6163 795f 7a6f 6e65 2829  t_privacy_zone()
-00008bf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008c00: 696e 6465 7820 6973 206e 6f74 204e 6f6e  index is not Non
-00008c10: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00008c20: 0a20 2020 2064 6566 2069 735f 7265 636f  .    def is_reco
-00008c30: 7264 696e 675f 656e 6162 6c65 6428 7365  rding_enabled(se
-00008c40: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00008c50: 2020 2020 2022 2222 4973 2072 6563 6f72       """Is recor
-00008c60: 6469 6e67 2066 6f6f 7461 6765 2f65 7665  ding footage/eve
-00008c70: 6e74 7320 6672 6f6d 2074 6865 2063 616d  nts from the cam
-00008c80: 6572 6120 656e 6162 6c65 643f 0a0a 2020  era enabled?..  
-00008c90: 2020 2020 2020 4966 2072 6563 6f72 6469        If recordi
-00008ca0: 6e67 2069 7320 6e6f 7420 656e 6162 6c65  ng is not enable
-00008cb0: 642c 2063 616d 6572 6173 2077 696c 6c20  d, cameras will 
-00008cc0: 6e6f 7420 7072 6f64 7563 6520 616e 7920  not produce any 
-00008cd0: 666f 6f74 6167 652c 2074 6875 6d62 6e61  footage, thumbna
-00008ce0: 696c 732c 0a20 2020 2020 2020 206d 6f74  ils,.        mot
-00008cf0: 696f 6e2f 736d 6172 7420 6465 7465 6374  ion/smart detect
-00008d00: 696f 6e20 6576 656e 7473 2e0a 2020 2020  ion events..    
-00008d10: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00008d20: 2072 6574 7572 6e20 7365 6c66 2e72 6563   return self.rec
-00008d30: 6f72 6469 6e67 5f73 6574 7469 6e67 732e  ording_settings.
-00008d40: 6d6f 6465 2021 3d20 5265 636f 7264 696e  mode != Recordin
-00008d50: 674d 6f64 652e 4e45 5645 520a 0a20 2020  gMode.NEVER..   
-00008d60: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00008d70: 6566 2069 735f 6d6f 7469 6f6e 5f64 6574  ef is_motion_det
-00008d80: 6563 7469 6f6e 5f6f 6e28 7365 6c66 2920  ection_on(self) 
-00008d90: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00008da0: 2022 2222 4973 204d 6f74 696f 6e20 4465   """Is Motion De
-00008db0: 7465 6374 696f 6e20 6176 6169 6c61 626c  tection availabl
-00008dc0: 6520 616e 6420 656e 6162 6c65 6420 2863  e and enabled (c
-00008dd0: 616d 6572 6120 7769 6c6c 2070 726f 6475  amera will produ
-00008de0: 6365 206d 6f74 696f 6e20 6576 656e 7473  ce motion events
-00008df0: 293f 2222 220a 0a20 2020 2020 2020 2072  )?"""..        r
-00008e00: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
-00008e10: 2020 2020 7365 6c66 2e69 735f 7265 636f      self.is_reco
-00008e20: 7264 696e 675f 656e 6162 6c65 640a 2020  rding_enabled.  
-00008e30: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-00008e40: 6c66 2e72 6563 6f72 6469 6e67 5f73 6574  lf.recording_set
-00008e50: 7469 6e67 732e 656e 6162 6c65 5f6d 6f74  tings.enable_mot
-00008e60: 696f 6e5f 6465 7465 6374 696f 6e20 6973  ion_detection is
-00008e70: 206e 6f74 2046 616c 7365 0a20 2020 2020   not False.     
-00008e80: 2020 2029 0a0a 2020 2020 4070 726f 7065     )..    @prope
-00008e90: 7274 790a 2020 2020 6465 6620 6973 5f6d  rty.    def is_m
-00008ea0: 6f74 696f 6e5f 6375 7272 656e 746c 795f  otion_currently_
-00008eb0: 6465 7465 6374 6564 2873 656c 6629 202d  detected(self) -
-00008ec0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00008ed0: 2222 2249 7320 6d6f 7469 6f6e 2063 7572  """Is motion cur
-00008ee0: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
-00008ef0: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
-00008f00: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-00008f10: 2020 2020 2020 2073 656c 662e 6973 5f6d         self.is_m
-00008f20: 6f74 696f 6e5f 6465 7465 6374 696f 6e5f  otion_detection_
-00008f30: 6f6e 0a20 2020 2020 2020 2020 2020 2061  on.            a
-00008f40: 6e64 2073 656c 662e 6973 5f6d 6f74 696f  nd self.is_motio
-00008f50: 6e5f 6465 7465 6374 6564 0a20 2020 2020  n_detected.     
-00008f60: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-00008f70: 6c61 7374 5f6d 6f74 696f 6e5f 6576 656e  last_motion_even
-00008f80: 7420 6973 206e 6f74 204e 6f6e 650a 2020  t is not None.  
-00008f90: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-00008fa0: 6c66 2e6c 6173 745f 6d6f 7469 6f6e 5f65  lf.last_motion_e
-00008fb0: 7665 6e74 2e65 6e64 2069 7320 4e6f 6e65  vent.end is None
-00008fc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00008fd0: 6173 796e 6320 6465 6620 7365 745f 6d6f  async def set_mo
-00008fe0: 7469 6f6e 5f64 6574 6563 7469 6f6e 2873  tion_detection(s
-00008ff0: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
-00009000: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-00009010: 2020 2020 2022 2222 5365 7473 206d 6f74       """Sets mot
-00009020: 696f 6e20 6465 7465 6374 696f 6e20 6f6e  ion detection on
-00009030: 2063 616d 6572 6122 2222 0a0a 2020 2020   camera"""..    
-00009040: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
-00009050: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00009060: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00009070: 6f72 6469 6e67 5f73 6574 7469 6e67 732e  ording_settings.
-00009080: 656e 6162 6c65 5f6d 6f74 696f 6e5f 6465  enable_motion_de
-00009090: 7465 6374 696f 6e20 3d20 656e 6162 6c65  tection = enable
-000090a0: 640a 0a20 2020 2020 2020 2061 7761 6974  d..        await
-000090b0: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
-000090c0: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
-000090d0: 2020 2320 6f62 6a65 6374 2073 6d61 7274    # object smart
-000090e0: 2064 6574 6563 7469 6f6e 730a 0a20 2020   detections..   
-000090f0: 2064 6566 205f 6973 5f73 6d61 7274 5f65   def _is_smart_e
-00009100: 6e61 626c 6564 2873 656c 662c 2073 6d61  nabled(self, sma
-00009110: 7274 5f74 7970 653a 2053 6d61 7274 4465  rt_type: SmartDe
-00009120: 7465 6374 4f62 6a65 6374 5479 7065 2920  tectObjectType) 
-00009130: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00009140: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00009150: 2020 2020 2020 7365 6c66 2e69 735f 7265        self.is_re
-00009160: 636f 7264 696e 675f 656e 6162 6c65 640a  cording_enabled.
-00009170: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00009180: 736d 6172 745f 7479 7065 2069 6e20 7365  smart_type in se
-00009190: 6c66 2e73 6d61 7274 5f64 6574 6563 745f  lf.smart_detect_
-000091a0: 7365 7474 696e 6773 2e6f 626a 6563 745f  settings.object_
-000091b0: 7479 7065 730a 2020 2020 2020 2020 290a  types.        ).
-000091c0: 0a20 2020 2064 6566 205f 6973 5f73 6d61  .    def _is_sma
-000091d0: 7274 5f64 6574 6563 7465 6428 7365 6c66  rt_detected(self
-000091e0: 2c20 736d 6172 745f 7479 7065 3a20 536d  , smart_type: Sm
-000091f0: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
-00009200: 7970 6529 202d 3e20 626f 6f6c 3a0a 2020  ype) -> bool:.  
-00009210: 2020 2020 2020 6576 656e 7420 3d20 7365        event = se
-00009220: 6c66 2e67 6574 5f6c 6173 745f 736d 6172  lf.get_last_smar
-00009230: 745f 6465 7465 6374 5f65 7665 6e74 2873  t_detect_event(s
-00009240: 6d61 7274 5f74 7970 6529 0a20 2020 2020  mart_type).     
-00009250: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-00009260: 2020 2020 2020 2020 7365 6c66 2e5f 6973          self._is
-00009270: 5f73 6d61 7274 5f65 6e61 626c 6564 2873  _smart_enabled(s
-00009280: 6d61 7274 5f74 7970 6529 0a20 2020 2020  mart_type).     
-00009290: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-000092a0: 6973 5f73 6d61 7274 5f64 6574 6563 7465  is_smart_detecte
-000092b0: 640a 2020 2020 2020 2020 2020 2020 616e  d.            an
-000092c0: 6420 6576 656e 7420 6973 206e 6f74 204e  d event is not N
-000092d0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000092e0: 616e 6420 6576 656e 742e 656e 6420 6973  and event.end is
-000092f0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00009300: 2020 616e 6420 736d 6172 745f 7479 7065    and smart_type
-00009310: 2069 6e20 6576 656e 742e 736d 6172 745f   in event.smart_
-00009320: 6465 7465 6374 5f74 7970 6573 0a20 2020  detect_types.   
-00009330: 2020 2020 2029 0a0a 2020 2020 4070 726f       )..    @pro
-00009340: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
-00009350: 5f73 6d61 7274 5f63 7572 7265 6e74 6c79  _smart_currently
-00009360: 5f64 6574 6563 7465 6428 7365 6c66 2920  _detected(self) 
-00009370: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00009380: 2022 2222 4973 2073 6d61 7274 2064 6574   """Is smart det
-00009390: 6563 7469 6f6e 2063 7572 7265 6e74 6c79  ection currently
-000093a0: 2062 6569 6e67 2064 6574 6563 7465 6422   being detected"
-000093b0: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-000093c0: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
-000093d0: 2073 656c 662e 6973 5f72 6563 6f72 6469   self.is_recordi
-000093e0: 6e67 5f65 6e61 626c 6564 0a20 2020 2020  ng_enabled.     
-000093f0: 2020 2020 2020 2061 6e64 2062 6f6f 6c28         and bool(
-00009400: 7365 6c66 2e73 6d61 7274 5f64 6574 6563  self.smart_detec
-00009410: 745f 7365 7474 696e 6773 2e6f 626a 6563  t_settings.objec
-00009420: 745f 7479 7065 7329 0a20 2020 2020 2020  t_types).       
-00009430: 2020 2020 2061 6e64 2073 656c 662e 6973       and self.is
-00009440: 5f73 6d61 7274 5f64 6574 6563 7465 640a  _smart_detected.
-00009450: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00009460: 7365 6c66 2e6c 6173 745f 736d 6172 745f  self.last_smart_
-00009470: 6465 7465 6374 5f65 7665 6e74 2069 7320  detect_event is 
-00009480: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00009490: 2020 2020 2061 6e64 2073 656c 662e 6c61       and self.la
-000094a0: 7374 5f73 6d61 7274 5f64 6574 6563 745f  st_smart_detect_
-000094b0: 6576 656e 742e 656e 6420 6973 204e 6f6e  event.end is Non
-000094c0: 650a 2020 2020 2020 2020 290a 0a20 2020  e.        )..   
-000094d0: 2023 2070 6572 736f 6e0a 0a20 2020 2040   # person..    @
+00000150: 6172 6e69 6e67 730a 0a66 726f 6d20 7079  arnings..from py
+00000160: 6461 6e74 6963 2e76 312e 6669 656c 6473  dantic.v1.fields
+00000170: 2069 6d70 6f72 7420 5072 6976 6174 6541   import PrivateA
+00000180: 7474 720a 0a66 726f 6d20 7079 756e 6966  ttr..from pyunif
+00000190: 6970 726f 7465 6374 2e64 6174 612e 6261  iprotect.data.ba
+000001a0: 7365 2069 6d70 6f72 7420 280a 2020 2020  se import (.    
+000001b0: 4556 454e 545f 5049 4e47 5f49 4e54 4552  EVENT_PING_INTER
+000001c0: 5641 4c2c 0a20 2020 2050 726f 7465 6374  VAL,.    Protect
+000001d0: 4164 6f70 7461 626c 6544 6576 6963 654d  AdoptableDeviceM
+000001e0: 6f64 656c 2c0a 2020 2020 5072 6f74 6563  odel,.    Protec
+000001f0: 7442 6173 654f 626a 6563 742c 0a20 2020  tBaseObject,.   
+00000200: 2050 726f 7465 6374 4d6f 7469 6f6e 4465   ProtectMotionDe
+00000210: 7669 6365 4d6f 6465 6c2c 0a29 0a66 726f  viceModel,.).fro
+00000220: 6d20 7079 756e 6966 6970 726f 7465 6374  m pyunifiprotect
+00000230: 2e64 6174 612e 7479 7065 7320 696d 706f  .data.types impo
+00000240: 7274 2028 0a20 2020 2044 4546 4155 4c54  rt (.    DEFAULT
+00000250: 2c0a 2020 2020 4445 4641 554c 545f 5459  ,.    DEFAULT_TY
+00000260: 5045 2c0a 2020 2020 4175 6469 6f43 6f64  PE,.    AudioCod
+00000270: 6563 732c 0a20 2020 2041 7564 696f 5374  ecs,.    AudioSt
+00000280: 796c 652c 0a20 2020 2041 7574 6f45 7870  yle,.    AutoExp
+00000290: 6f73 7572 654d 6f64 652c 0a20 2020 2043  osureMode,.    C
+000002a0: 6869 6d65 5479 7065 2c0a 2020 2020 436f  himeType,.    Co
+000002b0: 6c6f 722c 0a20 2020 2044 6f6f 7262 656c  lor,.    Doorbel
+000002c0: 6c4d 6573 7361 6765 5479 7065 2c0a 2020  lMessageType,.  
+000002d0: 2020 466f 6375 734d 6f64 652c 0a20 2020    FocusMode,.   
+000002e0: 2047 656f 6665 6e63 696e 6753 6574 7469   GeofencingSetti
+000002f0: 6e67 2c0a 2020 2020 4844 524d 6f64 652c  ng,.    HDRMode,
+00000300: 0a20 2020 2049 4352 4375 7374 6f6d 5661  .    ICRCustomVa
+00000310: 6c75 652c 0a20 2020 2049 4352 4c75 7856  lue,.    ICRLuxV
+00000320: 616c 7565 2c0a 2020 2020 4943 5253 656e  alue,.    ICRSen
+00000330: 7369 7469 7669 7479 2c0a 2020 2020 4952  sitivity,.    IR
+00000340: 4c45 444d 6f64 652c 0a20 2020 2049 7465  LEDMode,.    Ite
+00000350: 7261 746f 7243 616c 6c62 6163 6b2c 0a20  ratorCallback,. 
+00000360: 2020 204c 4544 4c65 7665 6c2c 0a20 2020     LEDLevel,.   
+00000370: 204c 656e 7354 7970 652c 0a20 2020 204c   LensType,.    L
+00000380: 6967 6874 4d6f 6465 456e 6162 6c65 5479  ightModeEnableTy
+00000390: 7065 2c0a 2020 2020 4c69 6768 744d 6f64  pe,.    LightMod
+000003a0: 6554 7970 652c 0a20 2020 204c 6f63 6b53  eType,.    LockS
+000003b0: 7461 7475 7354 7970 652c 0a20 2020 204c  tatusType,.    L
+000003c0: 6f77 4d65 6448 6967 682c 0a20 2020 204d  owMedHigh,.    M
+000003d0: 6f64 656c 5479 7065 2c0a 2020 2020 4d6f  odelType,.    Mo
+000003e0: 7469 6f6e 416c 676f 7269 7468 6d2c 0a20  tionAlgorithm,. 
+000003f0: 2020 204d 6f75 6e74 506f 7369 7469 6f6e     MountPosition
+00000400: 2c0a 2020 2020 4d6f 756e 7454 7970 652c  ,.    MountType,
+00000410: 0a20 2020 2050 6572 6365 6e74 2c0a 2020  .    Percent,.  
+00000420: 2020 5065 7263 656e 7449 6e74 2c0a 2020    PercentInt,.  
+00000430: 2020 5065 726d 6973 7369 6f6e 4e6f 6465    PermissionNode
+00000440: 2c0a 2020 2020 5072 6f67 7265 7373 4361  ,.    ProgressCa
+00000450: 6c6c 6261 636b 2c0a 2020 2020 5054 5a50  llback,.    PTZP
+00000460: 6f73 6974 696f 6e2c 0a20 2020 2050 545a  osition,.    PTZ
+00000470: 5072 6573 6574 2c0a 2020 2020 5265 636f  Preset,.    Reco
+00000480: 7264 696e 674d 6f64 652c 0a20 2020 2052  rdingMode,.    R
+00000490: 6570 6561 7454 696d 6573 2c0a 2020 2020  epeatTimes,.    
+000004a0: 5365 6e73 6f72 5374 6174 7573 5479 7065  SensorStatusType
+000004b0: 2c0a 2020 2020 536d 6172 7444 6574 6563  ,.    SmartDetec
+000004c0: 7441 7564 696f 5479 7065 2c0a 2020 2020  tAudioType,.    
+000004d0: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
+000004e0: 7454 7970 652c 0a20 2020 2054 776f 4279  tType,.    TwoBy
+000004f0: 7465 496e 742c 0a20 2020 2056 6964 656f  teInt,.    Video
+00000500: 4d6f 6465 2c0a 2020 2020 5744 524c 6576  Mode,.    WDRLev
+00000510: 656c 2c0a 290a 6672 6f6d 2070 7975 6e69  el,.).from pyuni
+00000520: 6669 7072 6f74 6563 742e 6461 7461 2e75  fiprotect.data.u
+00000530: 7365 7220 696d 706f 7274 2055 7365 720a  ser import User.
+00000540: 6672 6f6d 2070 7975 6e69 6669 7072 6f74  from pyunifiprot
+00000550: 6563 742e 6578 6365 7074 696f 6e73 2069  ect.exceptions i
+00000560: 6d70 6f72 7420 4261 6452 6571 7565 7374  mport BadRequest
+00000570: 2c20 4e6f 7441 7574 686f 7269 7a65 642c  , NotAuthorized,
+00000580: 2053 7472 6561 6d45 7272 6f72 0a66 726f   StreamError.fro
+00000590: 6d20 7079 756e 6966 6970 726f 7465 6374  m pyunifiprotect
+000005a0: 2e73 7472 6561 6d20 696d 706f 7274 2054  .stream import T
+000005b0: 616c 6b62 6163 6b53 7472 6561 6d0a 6672  alkbackStream.fr
+000005c0: 6f6d 2070 7975 6e69 6669 7072 6f74 6563  om pyunifiprotec
+000005d0: 742e 7574 696c 7320 696d 706f 7274 2028  t.utils import (
+000005e0: 0a20 2020 2063 6c61 6d70 5f76 616c 7565  .    clamp_value
+000005f0: 2c0a 2020 2020 636f 6e76 6572 745f 736d  ,.    convert_sm
+00000600: 6172 745f 6175 6469 6f5f 7479 7065 732c  art_audio_types,
+00000610: 0a20 2020 2063 6f6e 7665 7274 5f73 6d61  .    convert_sma
+00000620: 7274 5f74 7970 6573 2c0a 2020 2020 636f  rt_types,.    co
+00000630: 6e76 6572 745f 7669 6465 6f5f 6d6f 6465  nvert_video_mode
+00000640: 732c 0a20 2020 2066 726f 6d5f 6a73 5f74  s,.    from_js_t
+00000650: 696d 652c 0a20 2020 2070 726f 6365 7373  ime,.    process
+00000660: 5f64 6174 6574 696d 652c 0a20 2020 2073  _datetime,.    s
+00000670: 6572 6961 6c69 7a65 5f70 6f69 6e74 2c0a  erialize_point,.
+00000680: 2020 2020 746f 5f6a 735f 7469 6d65 2c0a      to_js_time,.
+00000690: 2020 2020 7574 635f 6e6f 772c 0a29 0a0a      utc_now,.)..
+000006a0: 6966 2054 5950 455f 4348 4543 4b49 4e47  if TYPE_CHECKING
+000006b0: 3a0a 2020 2020 6672 6f6d 2070 7975 6e69  :.    from pyuni
+000006c0: 6669 7072 6f74 6563 742e 6461 7461 2e6e  fiprotect.data.n
+000006d0: 7672 2069 6d70 6f72 7420 4576 656e 742c  vr import Event,
+000006e0: 204c 6976 6576 6965 770a 0a50 5249 5641   Liveview..PRIVA
+000006f0: 4359 5f5a 4f4e 455f 4e41 4d45 203d 2022  CY_ZONE_NAME = "
+00000700: 7079 7566 705f 7072 6976 6163 795f 7a6f  pyufp_privacy_zo
+00000710: 6e65 220a 4c55 585f 4d41 5050 494e 475f  ne".LUX_MAPPING_
+00000720: 5641 4c55 4553 203d 205b 0a20 2020 2033  VALUES = [.    3
+00000730: 302c 0a20 2020 2032 352c 0a20 2020 2032  0,.    25,.    2
+00000740: 302c 0a20 2020 2031 352c 0a20 2020 2031  0,.    15,.    1
+00000750: 322c 0a20 2020 2031 302c 0a20 2020 2037  2,.    10,.    7
+00000760: 2c0a 2020 2020 352c 0a20 2020 2033 2c0a  ,.    5,.    3,.
+00000770: 2020 2020 312c 0a5d 0a0a 5f4c 4f47 4745      1,.].._LOGGE
+00000780: 5220 3d20 6c6f 6767 696e 672e 6765 744c  R = logging.getL
+00000790: 6f67 6765 7228 5f5f 6e61 6d65 5f5f 290a  ogger(__name__).
+000007a0: 0a0a 636c 6173 7320 4c69 6768 7444 6576  ..class LightDev
+000007b0: 6963 6553 6574 7469 6e67 7328 5072 6f74  iceSettings(Prot
+000007c0: 6563 7442 6173 654f 626a 6563 7429 3a0a  ectBaseObject):.
+000007d0: 2020 2020 2320 5374 6174 7573 204c 4544      # Status LED
+000007e0: 0a20 2020 2069 735f 696e 6469 6361 746f  .    is_indicato
+000007f0: 725f 656e 6162 6c65 643a 2062 6f6f 6c0a  r_enabled: bool.
+00000800: 2020 2020 2320 4272 6967 6874 6e65 7373      # Brightness
+00000810: 0a20 2020 206c 6564 5f6c 6576 656c 3a20  .    led_level: 
+00000820: 4c45 444c 6576 656c 0a20 2020 206c 7578  LEDLevel.    lux
+00000830: 5f73 656e 7369 7469 7669 7479 3a20 4c6f  _sensitivity: Lo
+00000840: 774d 6564 4869 6768 0a20 2020 2070 6972  wMedHigh.    pir
+00000850: 5f64 7572 6174 696f 6e3a 2074 696d 6564  _duration: timed
+00000860: 656c 7461 0a20 2020 2070 6972 5f73 656e  elta.    pir_sen
+00000870: 7369 7469 7669 7479 3a20 5065 7263 656e  sitivity: Percen
+00000880: 7449 6e74 0a0a 2020 2020 4063 6c61 7373  tInt..    @class
+00000890: 6d65 7468 6f64 0a20 2020 2064 6566 2075  method.    def u
+000008a0: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
+000008b0: 7428 636c 732c 2064 6174 613a 2064 6963  t(cls, data: dic
+000008c0: 745b 7374 722c 2041 6e79 5d29 202d 3e20  t[str, Any]) -> 
+000008d0: 6469 6374 5b73 7472 2c20 416e 795d 3a0a  dict[str, Any]:.
+000008e0: 2020 2020 2020 2020 6966 2022 7069 7244          if "pirD
+000008f0: 7572 6174 696f 6e22 2069 6e20 6461 7461  uration" in data
+00000900: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
+00000910: 6e63 6528 6461 7461 5b22 7069 7244 7572  nce(data["pirDur
+00000920: 6174 696f 6e22 5d2c 2074 696d 6564 656c  ation"], timedel
+00000930: 7461 293a 0a20 2020 2020 2020 2020 2020  ta):.           
+00000940: 2064 6174 615b 2270 6972 4475 7261 7469   data["pirDurati
+00000950: 6f6e 225d 203d 2074 696d 6564 656c 7461  on"] = timedelta
+00000960: 286d 696c 6c69 7365 636f 6e64 733d 6461  (milliseconds=da
+00000970: 7461 5b22 7069 7244 7572 6174 696f 6e22  ta["pirDuration"
+00000980: 5d29 0a0a 2020 2020 2020 2020 7265 7475  ])..        retu
+00000990: 726e 2073 7570 6572 2829 2e75 6e69 6669  rn super().unifi
+000009a0: 5f64 6963 745f 746f 5f64 6963 7428 6461  _dict_to_dict(da
+000009b0: 7461 290a 0a0a 636c 6173 7320 4c69 6768  ta)...class Ligh
+000009c0: 744f 6e53 6574 7469 6e67 7328 5072 6f74  tOnSettings(Prot
+000009d0: 6563 7442 6173 654f 626a 6563 7429 3a0a  ectBaseObject):.
+000009e0: 2020 2020 2320 4d61 6e75 616c 2074 6f67      # Manual tog
+000009f0: 676c 6520 696e 2055 490a 2020 2020 6973  gle in UI.    is
+00000a00: 5f6c 6564 5f66 6f72 6365 5f6f 6e3a 2062  _led_force_on: b
+00000a10: 6f6f 6c0a 0a0a 636c 6173 7320 4c69 6768  ool...class Ligh
+00000a20: 744d 6f64 6553 6574 7469 6e67 7328 5072  tModeSettings(Pr
+00000a30: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
+00000a40: 3a0a 2020 2020 2320 6d61 696e 2022 4c69  :.    # main "Li
+00000a50: 6768 7469 6e67 2220 7365 7474 696e 6773  ghting" settings
+00000a60: 0a20 2020 206d 6f64 653a 204c 6967 6874  .    mode: Light
+00000a70: 4d6f 6465 5479 7065 0a20 2020 2065 6e61  ModeType.    ena
+00000a80: 626c 655f 6174 3a20 4c69 6768 744d 6f64  ble_at: LightMod
+00000a90: 6545 6e61 626c 6554 7970 650a 0a0a 636c  eEnableType...cl
+00000aa0: 6173 7320 4c69 6768 7428 5072 6f74 6563  ass Light(Protec
+00000ab0: 744d 6f74 696f 6e44 6576 6963 654d 6f64  tMotionDeviceMod
+00000ac0: 656c 293a 0a20 2020 2069 735f 7069 725f  el):.    is_pir_
+00000ad0: 6d6f 7469 6f6e 5f64 6574 6563 7465 643a  motion_detected:
+00000ae0: 2062 6f6f 6c0a 2020 2020 6973 5f6c 6967   bool.    is_lig
+00000af0: 6874 5f6f 6e3a 2062 6f6f 6c0a 2020 2020  ht_on: bool.    
+00000b00: 6973 5f6c 6f63 6174 696e 673a 2062 6f6f  is_locating: boo
+00000b10: 6c0a 2020 2020 6c69 6768 745f 6465 7669  l.    light_devi
+00000b20: 6365 5f73 6574 7469 6e67 733a 204c 6967  ce_settings: Lig
+00000b30: 6874 4465 7669 6365 5365 7474 696e 6773  htDeviceSettings
+00000b40: 0a20 2020 206c 6967 6874 5f6f 6e5f 7365  .    light_on_se
+00000b50: 7474 696e 6773 3a20 4c69 6768 744f 6e53  ttings: LightOnS
+00000b60: 6574 7469 6e67 730a 2020 2020 6c69 6768  ettings.    ligh
+00000b70: 745f 6d6f 6465 5f73 6574 7469 6e67 733a  t_mode_settings:
+00000b80: 204c 6967 6874 4d6f 6465 5365 7474 696e   LightModeSettin
+00000b90: 6773 0a20 2020 2063 616d 6572 615f 6964  gs.    camera_id
+00000ba0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0a  : Optional[str].
+00000bb0: 2020 2020 6973 5f63 616d 6572 615f 7061      is_camera_pa
+00000bc0: 6972 6564 3a20 626f 6f6c 0a0a 2020 2020  ired: bool..    
+00000bd0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00000be0: 2040 6361 6368 650a 2020 2020 6465 6620   @cache.    def 
+00000bf0: 5f67 6574 5f75 6e69 6669 5f72 656d 6170  _get_unifi_remap
+00000c00: 7328 636c 7329 202d 3e20 6469 6374 5b73  s(cls) -> dict[s
+00000c10: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
+00000c20: 2020 7265 7475 726e 207b 2a2a 7375 7065    return {**supe
+00000c30: 7228 292e 5f67 6574 5f75 6e69 6669 5f72  r()._get_unifi_r
+00000c40: 656d 6170 7328 292c 2022 6361 6d65 7261  emaps(), "camera
+00000c50: 223a 2022 6361 6d65 7261 4964 227d 0a0a  ": "cameraId"}..
+00000c60: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00000c70: 0a20 2020 2040 6361 6368 650a 2020 2020  .    @cache.    
+00000c80: 6465 6620 5f67 6574 5f72 6561 645f 6f6e  def _get_read_on
+00000c90: 6c79 5f66 6965 6c64 7328 636c 7329 202d  ly_fields(cls) -
+00000ca0: 3e20 7365 745b 7374 725d 3a0a 2020 2020  > set[str]:.    
+00000cb0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00000cc0: 2829 2e5f 6765 745f 7265 6164 5f6f 6e6c  ()._get_read_onl
+00000cd0: 795f 6669 656c 6473 2829 207c 207b 0a20  y_fields() | {. 
+00000ce0: 2020 2020 2020 2020 2020 2022 6973 5069             "isPi
+00000cf0: 724d 6f74 696f 6e44 6574 6563 7465 6422  rMotionDetected"
+00000d00: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+00000d10: 734c 6967 6874 4f6e 222c 0a20 2020 2020  sLightOn",.     
+00000d20: 2020 2020 2020 2022 6973 4c6f 6361 7469         "isLocati
+00000d30: 6e67 222c 0a20 2020 2020 2020 207d 0a0a  ng",.        }..
+00000d40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00000d50: 2020 6465 6620 6361 6d65 7261 2873 656c    def camera(sel
+00000d60: 6629 202d 3e20 4f70 7469 6f6e 616c 5b43  f) -> Optional[C
+00000d70: 616d 6572 615d 3a0a 2020 2020 2020 2020  amera]:.        
+00000d80: 2222 2250 6169 7265 6420 4361 6d65 7261  """Paired Camera
+00000d90: 2077 696c 6c20 616c 7761 7973 2062 6520   will always be 
+00000da0: 6e6f 6e65 2069 6620 6e6f 2063 616d 6572  none if no camer
+00000db0: 6120 6973 2070 6169 7265 6422 2222 0a0a  a is paired"""..
+00000dc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000dd0: 6361 6d65 7261 5f69 6420 6973 204e 6f6e  camera_id is Non
+00000de0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00000df0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00000e00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000e10: 6170 692e 626f 6f74 7374 7261 702e 6361  api.bootstrap.ca
+00000e20: 6d65 7261 735b 7365 6c66 2e63 616d 6572  meras[self.camer
+00000e30: 615f 6964 5d0a 0a20 2020 2061 7379 6e63  a_id]..    async
+00000e40: 2064 6566 2073 6574 5f70 6169 7265 645f   def set_paired_
+00000e50: 6361 6d65 7261 2873 656c 662c 2063 616d  camera(self, cam
+00000e60: 6572 613a 204f 7074 696f 6e61 6c5b 4361  era: Optional[Ca
+00000e70: 6d65 7261 5d29 202d 3e20 4e6f 6e65 3a0a  mera]) -> None:.
+00000e80: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00000e90: 7468 6520 6361 6d65 7261 2070 6169 7265  the camera paire
+00000ea0: 6420 7769 7468 2074 6865 206c 6967 6874  d with the light
+00000eb0: 2222 220a 0a20 2020 2020 2020 2061 7379  """..        asy
+00000ec0: 6e63 2077 6974 6820 7365 6c66 2e5f 7570  nc with self._up
+00000ed0: 6461 7465 5f6c 6f63 6b3a 0a20 2020 2020  date_lock:.     
+00000ee0: 2020 2020 2020 2061 7761 6974 2061 7379         await asy
+00000ef0: 6e63 696f 2e73 6c65 6570 280a 2020 2020  ncio.sleep(.    
+00000f00: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
+00000f10: 2020 2020 2020 2020 2020 2029 2020 2320             )  # 
+00000f20: 7969 656c 6420 746f 2074 6865 2065 7665  yield to the eve
+00000f30: 6e74 206c 6f6f 7020 6f6e 6365 2077 6520  nt loop once we 
+00000f40: 6861 7665 2074 6865 206c 6f63 6b20 746f  have the lock to
+00000f50: 2070 726f 6365 7373 2061 6e79 2070 656e   process any pen
+00000f60: 6469 6e67 2075 7064 6174 6573 0a20 2020  ding updates.   
+00000f70: 2020 2020 2020 2020 2064 6174 615f 6265           data_be
+00000f80: 666f 7265 5f63 6861 6e67 6573 203d 2073  fore_changes = s
+00000f90: 656c 662e 6469 6374 5f77 6974 685f 6578  elf.dict_with_ex
+00000fa0: 636c 7564 6573 2829 0a20 2020 2020 2020  cludes().       
+00000fb0: 2020 2020 2069 6620 6361 6d65 7261 2069       if camera i
+00000fc0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00000fd0: 2020 2020 2020 2020 7365 6c66 2e63 616d          self.cam
+00000fe0: 6572 615f 6964 203d 204e 6f6e 650a 2020  era_id = None.  
+00000ff0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 7365 6c66 2e63 616d 6572 615f 6964 203d  self.camera_id =
+00001020: 2063 616d 6572 612e 6964 0a20 2020 2020   camera.id.     
+00001030: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00001040: 662e 7361 7665 5f64 6576 6963 6528 6461  f.save_device(da
+00001050: 7461 5f62 6566 6f72 655f 6368 616e 6765  ta_before_change
+00001060: 732c 2066 6f72 6365 5f65 6d69 743d 5472  s, force_emit=Tr
+00001070: 7565 290a 0a20 2020 2061 7379 6e63 2064  ue)..    async d
+00001080: 6566 2073 6574 5f73 7461 7475 735f 6c69  ef set_status_li
+00001090: 6768 7428 7365 6c66 2c20 656e 6162 6c65  ght(self, enable
+000010a0: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
+000010b0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+000010c0: 7320 7468 6520 7374 6174 7573 2069 6e64  s the status ind
+000010d0: 6963 6174 6f72 206c 6967 6874 2066 6f72  icator light for
+000010e0: 2074 6865 206c 6967 6874 2222 220a 0a20   the light""".. 
+000010f0: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
+00001100: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
+00001110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001120: 6c69 6768 745f 6465 7669 6365 5f73 6574  light_device_set
+00001130: 7469 6e67 732e 6973 5f69 6e64 6963 6174  tings.is_indicat
+00001140: 6f72 5f65 6e61 626c 6564 203d 2065 6e61  or_enabled = ena
+00001150: 626c 6564 0a0a 2020 2020 2020 2020 6177  bled..        aw
+00001160: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
+00001170: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
+00001180: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
+00001190: 6574 5f6c 6564 5f6c 6576 656c 2873 656c  et_led_level(sel
+000011a0: 662c 206c 6564 5f6c 6576 656c 3a20 696e  f, led_level: in
+000011b0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+000011c0: 2020 2020 2222 2253 6574 7320 7468 6520      """Sets the 
+000011d0: 4c45 4420 6c65 7665 6c20 666f 7220 7468  LED level for th
+000011e0: 6520 6c69 6768 7422 2222 0a0a 2020 2020  e light"""..    
+000011f0: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
+00001200: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
+00001210: 2020 2020 2020 2020 7365 6c66 2e6c 6967          self.lig
+00001220: 6874 5f64 6576 6963 655f 7365 7474 696e  ht_device_settin
+00001230: 6773 2e6c 6564 5f6c 6576 656c 203d 204c  gs.led_level = L
+00001240: 4544 4c65 7665 6c28 6c65 645f 6c65 7665  EDLevel(led_leve
+00001250: 6c29 0a0a 2020 2020 2020 2020 6177 6169  l)..        awai
+00001260: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
+00001270: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
+00001280: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+00001290: 5f6c 6967 6874 2873 656c 662c 2065 6e61  _light(self, ena
+000012a0: 626c 6564 3a20 626f 6f6c 2c20 6c65 645f  bled: bool, led_
+000012b0: 6c65 7665 6c3a 204f 7074 696f 6e61 6c5b  level: Optional[
+000012c0: 696e 745d 203d 204e 6f6e 6529 202d 3e20  int] = None) -> 
+000012d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000012e0: 2246 6f72 6365 2074 7572 6e73 206f 6e2f  "Force turns on/
+000012f0: 6f66 6620 7468 6520 6c69 6768 7422 2222  off the light"""
+00001300: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
+00001310: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
+00001320: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00001330: 6c66 2e6c 6967 6874 5f6f 6e5f 7365 7474  lf.light_on_sett
+00001340: 696e 6773 2e69 735f 6c65 645f 666f 7263  ings.is_led_forc
+00001350: 655f 6f6e 203d 2065 6e61 626c 6564 0a20  e_on = enabled. 
+00001360: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00001370: 645f 6c65 7665 6c20 6973 206e 6f74 204e  d_level is not N
+00001380: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001390: 2020 2020 2073 656c 662e 6c69 6768 745f       self.light_
+000013a0: 6465 7669 6365 5f73 6574 7469 6e67 732e  device_settings.
+000013b0: 6c65 645f 6c65 7665 6c20 3d20 4c45 444c  led_level = LEDL
+000013c0: 6576 656c 286c 6564 5f6c 6576 656c 290a  evel(led_level).
+000013d0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+000013e0: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
+000013f0: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
+00001400: 6173 796e 6320 6465 6620 7365 745f 7365  async def set_se
+00001410: 6e73 6974 6976 6974 7928 7365 6c66 2c20  nsitivity(self, 
+00001420: 7365 6e73 6974 6976 6974 793a 2069 6e74  sensitivity: int
+00001430: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00001440: 2020 2022 2222 5365 7473 206d 6f74 696f     """Sets motio
+00001450: 6e20 7365 6e73 6974 6976 6974 7922 2222  n sensitivity"""
+00001460: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
+00001470: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
+00001480: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00001490: 6c66 2e6c 6967 6874 5f64 6576 6963 655f  lf.light_device_
+000014a0: 7365 7474 696e 6773 2e70 6972 5f73 656e  settings.pir_sen
+000014b0: 7369 7469 7669 7479 203d 2050 6572 6365  sitivity = Perce
+000014c0: 6e74 496e 7428 7365 6e73 6974 6976 6974  ntInt(sensitivit
+000014d0: 7929 0a0a 2020 2020 2020 2020 6177 6169  y)..        awai
+000014e0: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
+000014f0: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
+00001500: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+00001510: 5f64 7572 6174 696f 6e28 7365 6c66 2c20  _duration(self, 
+00001520: 6475 7261 7469 6f6e 3a20 7469 6d65 6465  duration: timede
+00001530: 6c74 6129 202d 3e20 4e6f 6e65 3a0a 2020  lta) -> None:.  
+00001540: 2020 2020 2020 2222 2253 6574 7320 6d6f        """Sets mo
+00001550: 7469 6f6e 2073 656e 7369 7469 7669 7479  tion sensitivity
+00001560: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00001570: 6475 7261 7469 6f6e 2e74 6f74 616c 5f73  duration.total_s
+00001580: 6563 6f6e 6473 2829 203c 2031 3520 6f72  econds() < 15 or
+00001590: 2064 7572 6174 696f 6e2e 746f 7461 6c5f   duration.total_
+000015a0: 7365 636f 6e64 7328 2920 3e20 3930 303a  seconds() > 900:
+000015b0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000015c0: 7365 2042 6164 5265 7175 6573 7428 2244  se BadRequest("D
+000015d0: 7572 6174 696f 6e20 6f75 7473 6964 6520  uration outside 
+000015e0: 6f66 2031 3573 2074 6f20 3930 3073 2072  of 15s to 900s r
+000015f0: 616e 6765 2229 0a0a 2020 2020 2020 2020  ange")..        
+00001600: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
+00001610: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001620: 2020 2020 7365 6c66 2e6c 6967 6874 5f64      self.light_d
+00001630: 6576 6963 655f 7365 7474 696e 6773 2e70  evice_settings.p
+00001640: 6972 5f64 7572 6174 696f 6e20 3d20 6475  ir_duration = du
+00001650: 7261 7469 6f6e 0a0a 2020 2020 2020 2020  ration..        
+00001660: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+00001670: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+00001680: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00001690: 2073 6574 5f6c 6967 6874 5f73 6574 7469   set_light_setti
+000016a0: 6e67 7328 0a20 2020 2020 2020 2073 656c  ngs(.        sel
+000016b0: 662c 0a20 2020 2020 2020 206d 6f64 653a  f,.        mode:
+000016c0: 204c 6967 6874 4d6f 6465 5479 7065 2c0a   LightModeType,.
+000016d0: 2020 2020 2020 2020 656e 6162 6c65 5f61          enable_a
+000016e0: 743a 204f 7074 696f 6e61 6c5b 4c69 6768  t: Optional[Ligh
+000016f0: 744d 6f64 6545 6e61 626c 6554 7970 655d  tModeEnableType]
+00001700: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00001710: 2064 7572 6174 696f 6e3a 204f 7074 696f   duration: Optio
+00001720: 6e61 6c5b 7469 6d65 6465 6c74 615d 203d  nal[timedelta] =
+00001730: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00001740: 656e 7369 7469 7669 7479 3a20 4f70 7469  ensitivity: Opti
+00001750: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00001760: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00001770: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
+00001780: 7465 7320 7661 7269 6f75 7320 4c69 6768  tes various Ligh
+00001790: 7420 7365 7474 696e 6773 2e0a 0a20 2020  t settings...   
+000017a0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000017b0: 2020 202d 2d2d 2d0a 2020 2020 2020 2020     ----.        
+000017c0: 2020 2020 6d6f 6465 3a20 4c69 6768 7420      mode: Light 
+000017d0: 7472 6967 6765 7220 6d6f 6465 0a20 2020  trigger mode.   
+000017e0: 2020 2020 2020 2020 2065 6e61 626c 655f           enable_
+000017f0: 6174 3a20 5468 656e 2074 6865 206c 6967  at: Then the lig
+00001800: 6874 2061 7574 6f6d 6174 6963 616c 6c79  ht automatically
+00001810: 2074 7572 6e73 206f 6e20 6279 2069 7473   turns on by its
+00001820: 656c 660a 2020 2020 2020 2020 2020 2020  elf.            
+00001830: 6475 7261 7469 6f6e 3a20 486f 7720 6c6f  duration: How lo
+00001840: 6e67 2074 6865 206c 6967 6874 2073 686f  ng the light sho
+00001850: 756c 6420 7265 6d61 696e 206f 6e20 6166  uld remain on af
+00001860: 7465 7220 6d6f 7469 6f6e 2c20 6d75 7374  ter motion, must
+00001870: 2062 6520 7469 6d65 6465 6c74 6120 6265   be timedelta be
+00001880: 7477 6565 6e20 3135 7320 616e 6420 3930  tween 15s and 90
+00001890: 3073 0a20 2020 2020 2020 2020 2020 2073  0s.            s
+000018a0: 656e 7369 7469 7669 7479 3a20 5049 5220  ensitivity: PIR 
+000018b0: 4d6f 7469 6f6e 2073 656e 7369 7469 7669  Motion sensitivi
+000018c0: 7479 0a20 2020 2020 2020 2022 2222 0a0a  ty.        """..
+000018d0: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
+000018e0: 696f 6e20 6973 206e 6f74 204e 6f6e 6520  ion is not None 
+000018f0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+00001900: 2020 6475 7261 7469 6f6e 2e74 6f74 616c    duration.total
+00001910: 5f73 6563 6f6e 6473 2829 203c 2031 3520  _seconds() < 15 
+00001920: 6f72 2064 7572 6174 696f 6e2e 746f 7461  or duration.tota
+00001930: 6c5f 7365 636f 6e64 7328 2920 3e20 3930  l_seconds() > 90
+00001940: 300a 2020 2020 2020 2020 293a 0a20 2020  0.        ):.   
+00001950: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+00001960: 6164 5265 7175 6573 7428 2244 7572 6174  adRequest("Durat
+00001970: 696f 6e20 6f75 7473 6964 6520 6f66 2031  ion outside of 1
+00001980: 3573 2074 6f20 3930 3073 2072 616e 6765  5s to 900s range
+00001990: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
+000019a0: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
+000019b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000019c0: 7365 6c66 2e6c 6967 6874 5f6d 6f64 655f  self.light_mode_
+000019d0: 7365 7474 696e 6773 2e6d 6f64 6520 3d20  settings.mode = 
+000019e0: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
+000019f0: 2069 6620 656e 6162 6c65 5f61 7420 6973   if enable_at is
+00001a00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00001a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001a20: 6c69 6768 745f 6d6f 6465 5f73 6574 7469  light_mode_setti
+00001a30: 6e67 732e 656e 6162 6c65 5f61 7420 3d20  ngs.enable_at = 
+00001a40: 656e 6162 6c65 5f61 740a 2020 2020 2020  enable_at.      
+00001a50: 2020 2020 2020 6966 2064 7572 6174 696f        if duratio
+00001a60: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001a80: 656c 662e 6c69 6768 745f 6465 7669 6365  elf.light_device
+00001a90: 5f73 6574 7469 6e67 732e 7069 725f 6475  _settings.pir_du
+00001aa0: 7261 7469 6f6e 203d 2064 7572 6174 696f  ration = duratio
+00001ab0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+00001ac0: 2073 656e 7369 7469 7669 7479 2069 7320   sensitivity is 
+00001ad0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00001ae0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00001af0: 6967 6874 5f64 6576 6963 655f 7365 7474  ight_device_sett
+00001b00: 696e 6773 2e70 6972 5f73 656e 7369 7469  ings.pir_sensiti
+00001b10: 7669 7479 203d 2050 6572 6365 6e74 496e  vity = PercentIn
+00001b20: 7428 7365 6e73 6974 6976 6974 7929 0a0a  t(sensitivity)..
+00001b30: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+00001b40: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
+00001b50: 6361 6c6c 6261 636b 290a 0a0a 636c 6173  callback)...clas
+00001b60: 7320 4361 6d65 7261 4368 616e 6e65 6c28  s CameraChannel(
+00001b70: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
+00001b80: 7429 3a0a 2020 2020 6964 3a20 696e 7420  t):.    id: int 
+00001b90: 2023 2072 6561 6420 6f6e 6c79 0a20 2020   # read only.   
+00001ba0: 2076 6964 656f 5f69 643a 2073 7472 2020   video_id: str  
+00001bb0: 2320 7265 6164 206f 6e6c 790a 2020 2020  # read only.    
+00001bc0: 6e61 6d65 3a20 7374 7220 2023 2072 6561  name: str  # rea
+00001bd0: 6420 6f6e 6c79 0a20 2020 2065 6e61 626c  d only.    enabl
+00001be0: 6564 3a20 626f 6f6c 2020 2320 7265 6164  ed: bool  # read
+00001bf0: 206f 6e6c 790a 2020 2020 6973 5f72 7473   only.    is_rts
+00001c00: 705f 656e 6162 6c65 643a 2062 6f6f 6c0a  p_enabled: bool.
+00001c10: 2020 2020 7274 7370 5f61 6c69 6173 3a20      rtsp_alias: 
+00001c20: 4f70 7469 6f6e 616c 5b73 7472 5d20 2023  Optional[str]  #
+00001c30: 2072 6561 6420 6f6e 6c79 0a20 2020 2077   read only.    w
+00001c40: 6964 7468 3a20 696e 740a 2020 2020 6865  idth: int.    he
+00001c50: 6967 6874 3a20 696e 740a 2020 2020 6670  ight: int.    fp
+00001c60: 733a 2069 6e74 0a20 2020 2062 6974 7261  s: int.    bitra
+00001c70: 7465 3a20 696e 740a 2020 2020 6d69 6e5f  te: int.    min_
+00001c80: 6269 7472 6174 653a 2069 6e74 2020 2320  bitrate: int  # 
+00001c90: 7265 6164 206f 6e6c 790a 2020 2020 6d61  read only.    ma
+00001ca0: 785f 6269 7472 6174 653a 2069 6e74 2020  x_bitrate: int  
+00001cb0: 2320 7265 6164 206f 6e6c 790a 2020 2020  # read only.    
+00001cc0: 6d69 6e5f 636c 6965 6e74 5f61 6461 7074  min_client_adapt
+00001cd0: 6976 655f 6269 745f 7261 7465 3a20 4f70  ive_bit_rate: Op
+00001ce0: 7469 6f6e 616c 5b69 6e74 5d20 2023 2072  tional[int]  # r
+00001cf0: 6561 6420 6f6e 6c79 0a20 2020 206d 696e  ead only.    min
+00001d00: 5f6d 6f74 696f 6e5f 6164 6170 7469 7665  _motion_adaptive
+00001d10: 5f62 6974 5f72 6174 653a 204f 7074 696f  _bit_rate: Optio
+00001d20: 6e61 6c5b 696e 745d 2020 2320 7265 6164  nal[int]  # read
+00001d30: 206f 6e6c 790a 2020 2020 6670 735f 7661   only.    fps_va
+00001d40: 6c75 6573 3a20 6c69 7374 5b69 6e74 5d20  lues: list[int] 
+00001d50: 2023 2072 6561 6420 6f6e 6c79 0a20 2020   # read only.   
+00001d60: 2069 6472 5f69 6e74 6572 7661 6c3a 2069   idr_interval: i
+00001d70: 6e74 0a20 2020 2023 2033 2e30 2e32 322b  nt.    # 3.0.22+
+00001d80: 0a20 2020 2061 7574 6f5f 6269 7472 6174  .    auto_bitrat
+00001d90: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+00001da0: 5d20 3d20 4e6f 6e65 0a20 2020 2061 7574  ] = None.    aut
+00001db0: 6f5f 6670 733a 204f 7074 696f 6e61 6c5b  o_fps: Optional[
+00001dc0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 2020  bool] = None..  
+00001dd0: 2020 5f72 7473 705f 7572 6c3a 204f 7074    _rtsp_url: Opt
+00001de0: 696f 6e61 6c5b 7374 725d 203d 2050 7269  ional[str] = Pri
+00001df0: 7661 7465 4174 7472 284e 6f6e 6529 0a20  vateAttr(None). 
+00001e00: 2020 205f 7274 7370 735f 7572 6c3a 204f     _rtsps_url: O
+00001e10: 7074 696f 6e61 6c5b 7374 725d 203d 2050  ptional[str] = P
+00001e20: 7269 7661 7465 4174 7472 284e 6f6e 6529  rivateAttr(None)
+00001e30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00001e40: 2020 2020 6465 6620 7274 7370 5f75 726c      def rtsp_url
+00001e50: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00001e60: 616c 5b73 7472 5d3a 0a20 2020 2020 2020  al[str]:.       
+00001e70: 2069 6620 6e6f 7420 7365 6c66 2e69 735f   if not self.is_
+00001e80: 7274 7370 5f65 6e61 626c 6564 206f 7220  rtsp_enabled or 
+00001e90: 7365 6c66 2e72 7473 705f 616c 6961 7320  self.rtsp_alias 
+00001ea0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00001eb0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00001ec0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00001ed0: 662e 5f72 7473 705f 7572 6c20 6973 206e  f._rtsp_url is n
+00001ee0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001ef0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00001f00: 2e5f 7274 7370 5f75 726c 0a20 2020 2020  ._rtsp_url.     
+00001f10: 2020 2073 656c 662e 5f72 7473 705f 7572     self._rtsp_ur
+00001f20: 6c20 3d20 6622 7274 7370 3a2f 2f7b 7365  l = f"rtsp://{se
+00001f30: 6c66 2e61 7069 2e63 6f6e 6e65 6374 696f  lf.api.connectio
+00001f40: 6e5f 686f 7374 7d3a 7b73 656c 662e 6170  n_host}:{self.ap
+00001f50: 692e 626f 6f74 7374 7261 702e 6e76 722e  i.bootstrap.nvr.
+00001f60: 706f 7274 732e 7274 7370 7d2f 7b73 656c  ports.rtsp}/{sel
+00001f70: 662e 7274 7370 5f61 6c69 6173 7d22 0a20  f.rtsp_alias}". 
+00001f80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001f90: 6c66 2e5f 7274 7370 5f75 726c 0a0a 2020  lf._rtsp_url..  
+00001fa0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00001fb0: 6465 6620 7274 7370 735f 7572 6c28 7365  def rtsps_url(se
+00001fc0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+00001fd0: 7374 725d 3a0a 2020 2020 2020 2020 6966  str]:.        if
+00001fe0: 206e 6f74 2073 656c 662e 6973 5f72 7473   not self.is_rts
+00001ff0: 705f 656e 6162 6c65 6420 6f72 2073 656c  p_enabled or sel
+00002000: 662e 7274 7370 5f61 6c69 6173 2069 7320  f.rtsp_alias is 
+00002010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002020: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+00002030: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00002040: 7274 7370 735f 7572 6c20 6973 206e 6f74  rtsps_url is not
+00002050: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002060: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002070: 7274 7370 735f 7572 6c0a 2020 2020 2020  rtsps_url.      
+00002080: 2020 7365 6c66 2e5f 7274 7370 735f 7572    self._rtsps_ur
+00002090: 6c20 3d20 6622 7274 7370 733a 2f2f 7b73  l = f"rtsps://{s
+000020a0: 656c 662e 6170 692e 636f 6e6e 6563 7469  elf.api.connecti
+000020b0: 6f6e 5f68 6f73 747d 3a7b 7365 6c66 2e61  on_host}:{self.a
+000020c0: 7069 2e62 6f6f 7473 7472 6170 2e6e 7672  pi.bootstrap.nvr
+000020d0: 2e70 6f72 7473 2e72 7473 7073 7d2f 7b73  .ports.rtsps}/{s
+000020e0: 656c 662e 7274 7370 5f61 6c69 6173 7d3f  elf.rtsp_alias}?
+000020f0: 656e 6162 6c65 5372 7470 220a 2020 2020  enableSrtp".    
+00002100: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002110: 5f72 7473 7073 5f75 726c 0a0a 2020 2020  _rtsps_url..    
+00002120: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00002130: 6620 6973 5f70 6163 6b61 6765 2873 656c  f is_package(sel
+00002140: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+00002150: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002160: 6670 7320 3c3d 2032 0a0a 0a63 6c61 7373  fps <= 2...class
+00002170: 2049 5350 5365 7474 696e 6773 2850 726f   ISPSettings(Pro
+00002180: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
+00002190: 0a20 2020 2061 655f 6d6f 6465 3a20 4175  .    ae_mode: Au
+000021a0: 746f 4578 706f 7375 7265 4d6f 6465 0a20  toExposureMode. 
+000021b0: 2020 2069 725f 6c65 645f 6d6f 6465 3a20     ir_led_mode: 
+000021c0: 4952 4c45 444d 6f64 650a 2020 2020 6972  IRLEDMode.    ir
+000021d0: 5f6c 6564 5f6c 6576 656c 3a20 5477 6f42  _led_level: TwoB
+000021e0: 7974 6549 6e74 0a20 2020 2077 6472 3a20  yteInt.    wdr: 
+000021f0: 5744 524c 6576 656c 0a20 2020 2069 6372  WDRLevel.    icr
+00002200: 5f73 656e 7369 7469 7669 7479 3a20 4943  _sensitivity: IC
+00002210: 5253 656e 7369 7469 7669 7479 0a20 2020  RSensitivity.   
+00002220: 2062 7269 6768 746e 6573 733a 2069 6e74   brightness: int
+00002230: 0a20 2020 2063 6f6e 7472 6173 743a 2069  .    contrast: i
+00002240: 6e74 0a20 2020 2068 7565 3a20 696e 740a  nt.    hue: int.
+00002250: 2020 2020 7361 7475 7261 7469 6f6e 3a20      saturation: 
+00002260: 696e 740a 2020 2020 7368 6172 706e 6573  int.    sharpnes
+00002270: 733a 2069 6e74 0a20 2020 2064 656e 6f69  s: int.    denoi
+00002280: 7365 3a20 696e 740a 2020 2020 6973 5f66  se: int.    is_f
+00002290: 6c69 7070 6564 5f76 6572 7469 6361 6c3a  lipped_vertical:
+000022a0: 2062 6f6f 6c0a 2020 2020 6973 5f66 6c69   bool.    is_fli
+000022b0: 7070 6564 5f68 6f72 697a 6f6e 7461 6c3a  pped_horizontal:
+000022c0: 2062 6f6f 6c0a 2020 2020 6973 5f61 7574   bool.    is_aut
+000022d0: 6f5f 726f 7461 7465 5f65 6e61 626c 6564  o_rotate_enabled
+000022e0: 3a20 626f 6f6c 0a20 2020 2069 735f 6c64  : bool.    is_ld
+000022f0: 635f 656e 6162 6c65 643a 2062 6f6f 6c0a  c_enabled: bool.
+00002300: 2020 2020 6973 5f33 646e 725f 656e 6162      is_3dnr_enab
+00002310: 6c65 643a 2062 6f6f 6c0a 2020 2020 6973  led: bool.    is
+00002320: 5f65 7874 6572 6e61 6c5f 6972 5f65 6e61  _external_ir_ena
+00002330: 626c 6564 3a20 626f 6f6c 0a20 2020 2069  bled: bool.    i
+00002340: 735f 6167 6772 6573 7369 7665 5f61 6e74  s_aggressive_ant
+00002350: 695f 666c 6963 6b65 725f 656e 6162 6c65  i_flicker_enable
+00002360: 643a 2062 6f6f 6c0a 2020 2020 6973 5f70  d: bool.    is_p
+00002370: 6175 7365 5f6d 6f74 696f 6e5f 656e 6162  ause_motion_enab
+00002380: 6c65 643a 2062 6f6f 6c0a 2020 2020 645f  led: bool.    d_
+00002390: 7a6f 6f6d 5f63 656e 7465 725f 783a 2069  zoom_center_x: i
+000023a0: 6e74 0a20 2020 2064 5f7a 6f6f 6d5f 6365  nt.    d_zoom_ce
+000023b0: 6e74 6572 5f79 3a20 696e 740a 2020 2020  nter_y: int.    
+000023c0: 645f 7a6f 6f6d 5f73 6361 6c65 3a20 696e  d_zoom_scale: in
+000023d0: 740a 2020 2020 645f 7a6f 6f6d 5f73 7472  t.    d_zoom_str
+000023e0: 6561 6d5f 6964 3a20 696e 740a 2020 2020  eam_id: int.    
+000023f0: 666f 6375 735f 6d6f 6465 3a20 4f70 7469  focus_mode: Opti
+00002400: 6f6e 616c 5b46 6f63 7573 4d6f 6465 5d20  onal[FocusMode] 
+00002410: 3d20 4e6f 6e65 0a20 2020 2066 6f63 7573  = None.    focus
+00002420: 5f70 6f73 6974 696f 6e3a 2069 6e74 0a20  _position: int. 
+00002430: 2020 2074 6f75 6368 5f66 6f63 7573 5f78     touch_focus_x
+00002440: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0a  : Optional[int].
+00002450: 2020 2020 746f 7563 685f 666f 6375 735f      touch_focus_
+00002460: 793a 204f 7074 696f 6e61 6c5b 696e 745d  y: Optional[int]
+00002470: 0a20 2020 207a 6f6f 6d5f 706f 7369 7469  .    zoom_positi
+00002480: 6f6e 3a20 5065 7263 656e 7449 6e74 0a20  on: PercentInt. 
+00002490: 2020 206d 6f75 6e74 5f70 6f73 6974 696f     mount_positio
+000024a0: 6e3a 204f 7074 696f 6e61 6c5b 4d6f 756e  n: Optional[Moun
+000024b0: 7450 6f73 6974 696f 6e5d 203d 204e 6f6e  tPosition] = Non
+000024c0: 650a 2020 2020 2320 7265 7175 6972 6573  e.    # requires
+000024d0: 2032 2e38 2e31 342b 0a20 2020 2069 735f   2.8.14+.    is_
+000024e0: 636f 6c6f 725f 6e69 6768 745f 7669 7369  color_night_visi
+000024f0: 6f6e 5f65 6e61 626c 6564 3a20 4f70 7469  on_enabled: Opti
+00002500: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00002510: 650a 2020 2020 2320 332e 302e 3232 2b0a  e.    # 3.0.22+.
+00002520: 2020 2020 6864 725f 6d6f 6465 3a20 4f70      hdr_mode: Op
+00002530: 7469 6f6e 616c 5b48 4452 4d6f 6465 5d20  tional[HDRMode] 
+00002540: 3d20 4e6f 6e65 0a20 2020 2069 6372 5f63  = None.    icr_c
+00002550: 7573 746f 6d5f 7661 6c75 653a 204f 7074  ustom_value: Opt
+00002560: 696f 6e61 6c5b 4943 5243 7573 746f 6d56  ional[ICRCustomV
+00002570: 616c 7565 5d20 3d20 4e6f 6e65 0a20 2020  alue] = None.   
+00002580: 2069 6372 5f73 7769 7463 685f 6d6f 6465   icr_switch_mode
+00002590: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000025a0: 3d20 4e6f 6e65 0a20 2020 2073 706f 746c  = None.    spotl
+000025b0: 6967 6874 5f64 7572 6174 696f 6e3a 204f  ight_duration: O
+000025c0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000025d0: 6f6e 650a 0a20 2020 2064 6566 2075 6e69  one..    def uni
+000025e0: 6669 5f64 6963 7428 0a20 2020 2020 2020  fi_dict(.       
+000025f0: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+00002600: 6174 613a 204f 7074 696f 6e61 6c5b 6469  ata: Optional[di
+00002610: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
+00002620: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
+00002630: 636c 7564 653a 204f 7074 696f 6e61 6c5b  clude: Optional[
+00002640: 7365 745b 7374 725d 5d20 3d20 4e6f 6e65  set[str]] = None
+00002650: 2c0a 2020 2020 2920 2d3e 2064 6963 745b  ,.    ) -> dict[
+00002660: 7374 722c 2041 6e79 5d3a 0a20 2020 2020  str, Any]:.     
+00002670: 2020 2064 6174 6120 3d20 7375 7065 7228     data = super(
+00002680: 292e 756e 6966 695f 6469 6374 2864 6174  ).unifi_dict(dat
+00002690: 613d 6461 7461 2c20 6578 636c 7564 653d  a=data, exclude=
+000026a0: 6578 636c 7564 6529 0a0a 2020 2020 2020  exclude)..      
+000026b0: 2020 6966 2022 666f 6375 734d 6f64 6522    if "focusMode"
+000026c0: 2069 6e20 6461 7461 2061 6e64 2064 6174   in data and dat
+000026d0: 615b 2266 6f63 7573 4d6f 6465 225d 2069  a["focusMode"] i
+000026e0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000026f0: 2020 2020 6465 6c20 6461 7461 5b22 666f      del data["fo
+00002700: 6375 734d 6f64 6522 5d0a 0a20 2020 2020  cusMode"]..     
+00002710: 2020 2072 6574 7572 6e20 6461 7461 0a0a     return data..
+00002720: 0a63 6c61 7373 204f 5344 5365 7474 696e  .class OSDSettin
+00002730: 6773 2850 726f 7465 6374 4261 7365 4f62  gs(ProtectBaseOb
+00002740: 6a65 6374 293a 0a20 2020 2023 204f 7665  ject):.    # Ove
+00002750: 726c 6179 2049 6e66 6f72 6d61 7469 6f6e  rlay Information
+00002760: 0a20 2020 2069 735f 6e61 6d65 5f65 6e61  .    is_name_ena
+00002770: 626c 6564 3a20 626f 6f6c 0a20 2020 2069  bled: bool.    i
+00002780: 735f 6461 7465 5f65 6e61 626c 6564 3a20  s_date_enabled: 
+00002790: 626f 6f6c 0a20 2020 2069 735f 6c6f 676f  bool.    is_logo
+000027a0: 5f65 6e61 626c 6564 3a20 626f 6f6c 0a20  _enabled: bool. 
+000027b0: 2020 2069 735f 6465 6275 675f 656e 6162     is_debug_enab
+000027c0: 6c65 643a 2062 6f6f 6c0a 0a0a 636c 6173  led: bool...clas
+000027d0: 7320 4c45 4453 6574 7469 6e67 7328 5072  s LEDSettings(Pr
+000027e0: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
+000027f0: 3a0a 2020 2020 2320 5374 6174 7573 204c  :.    # Status L
+00002800: 6967 6874 0a20 2020 2069 735f 656e 6162  ight.    is_enab
+00002810: 6c65 643a 2062 6f6f 6c0a 2020 2020 626c  led: bool.    bl
+00002820: 696e 6b5f 7261 7465 3a20 696e 7420 2023  ink_rate: int  #
+00002830: 2069 6e20 6d69 6c6c 6973 6563 6f6e 6473   in milliseconds
+00002840: 2062 6574 7765 6565 6e20 626c 696e 6b73   betweeen blinks
+00002850: 2c20 3020 3d20 736f 6c69 640a 0a0a 636c  , 0 = solid...cl
+00002860: 6173 7320 5370 6561 6b65 7253 6574 7469  ass SpeakerSetti
+00002870: 6e67 7328 5072 6f74 6563 7442 6173 654f  ngs(ProtectBaseO
+00002880: 626a 6563 7429 3a0a 2020 2020 6973 5f65  bject):.    is_e
+00002890: 6e61 626c 6564 3a20 626f 6f6c 0a20 2020  nabled: bool.   
+000028a0: 2023 2053 7461 7475 7320 536f 756e 6473   # Status Sounds
+000028b0: 0a20 2020 2061 7265 5f73 7973 7465 6d5f  .    are_system_
+000028c0: 736f 756e 6473 5f65 6e61 626c 6564 3a20  sounds_enabled: 
+000028d0: 626f 6f6c 0a20 2020 2076 6f6c 756d 653a  bool.    volume:
+000028e0: 2050 6572 6365 6e74 496e 740a 0a0a 636c   PercentInt...cl
+000028f0: 6173 7320 5265 636f 7264 696e 6753 6574  ass RecordingSet
+00002900: 7469 6e67 7328 5072 6f74 6563 7442 6173  tings(ProtectBas
+00002910: 654f 626a 6563 7429 3a0a 2020 2020 2320  eObject):.    # 
+00002920: 5365 636f 6e64 7320 746f 2072 6563 6f72  Seconds to recor
+00002930: 6420 6265 666f 7265 204d 6f74 696f 6e0a  d before Motion.
+00002940: 2020 2020 7072 655f 7061 6464 696e 673a      pre_padding:
+00002950: 2074 696d 6564 656c 7461 0a20 2020 2023   timedelta.    #
+00002960: 2053 6563 6f6e 6473 2074 6f20 7265 636f   Seconds to reco
+00002970: 7264 2061 6674 6572 204d 6f74 696f 6e0a  rd after Motion.
+00002980: 2020 2020 706f 7374 5f70 6164 6469 6e67      post_padding
+00002990: 3a20 7469 6d65 6465 6c74 610a 2020 2020  : timedelta.    
+000029a0: 2320 5365 636f 6e64 7320 6f66 204d 6f74  # Seconds of Mot
+000029b0: 696f 6e20 4e65 6564 6564 0a20 2020 206d  ion Needed.    m
+000029c0: 696e 5f6d 6f74 696f 6e5f 6576 656e 745f  in_motion_event_
+000029d0: 7472 6967 6765 723a 2074 696d 6564 656c  trigger: timedel
+000029e0: 7461 0a20 2020 2065 6e64 5f6d 6f74 696f  ta.    end_motio
+000029f0: 6e5f 6576 656e 745f 6465 6c61 793a 2074  n_event_delay: t
+00002a00: 696d 6564 656c 7461 0a20 2020 2073 7570  imedelta.    sup
+00002a10: 7072 6573 735f 696c 6c75 6d69 6e61 7469  press_illuminati
+00002a20: 6f6e 5f73 7572 6765 3a20 626f 6f6c 0a20  on_surge: bool. 
+00002a30: 2020 2023 2048 6967 6820 4672 616d 6520     # High Frame 
+00002a40: 5261 7465 204d 6f64 650a 2020 2020 6d6f  Rate Mode.    mo
+00002a50: 6465 3a20 5265 636f 7264 696e 674d 6f64  de: RecordingMod
+00002a60: 650a 2020 2020 6765 6f66 656e 6369 6e67  e.    geofencing
+00002a70: 3a20 4765 6f66 656e 6369 6e67 5365 7474  : GeofencingSett
+00002a80: 696e 670a 2020 2020 6d6f 7469 6f6e 5f61  ing.    motion_a
+00002a90: 6c67 6f72 6974 686d 3a20 4d6f 7469 6f6e  lgorithm: Motion
+00002aa0: 416c 676f 7269 7468 6d0a 2020 2020 656e  Algorithm.    en
+00002ab0: 6162 6c65 5f6d 6f74 696f 6e5f 6465 7465  able_motion_dete
+00002ac0: 6374 696f 6e3a 204f 7074 696f 6e61 6c5b  ction: Optional[
+00002ad0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a20 2020  bool] = None.   
+00002ae0: 2075 7365 5f6e 6577 5f6d 6f74 696f 6e5f   use_new_motion_
+00002af0: 616c 676f 7269 7468 6d3a 2062 6f6f 6c0a  algorithm: bool.
+00002b00: 2020 2020 2320 7265 7175 6972 6573 2032      # requires 2
+00002b10: 2e39 2e32 302b 0a20 2020 2069 6e5f 7363  .9.20+.    in_sc
+00002b20: 6865 6475 6c65 5f6d 6f64 653a 204f 7074  hedule_mode: Opt
+00002b30: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00002b40: 650a 2020 2020 6f75 745f 7363 6865 6475  e.    out_schedu
+00002b50: 6c65 5f6d 6f64 653a 204f 7074 696f 6e61  le_mode: Optiona
+00002b60: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
+00002b70: 2020 2320 322e 3131 2e31 332b 0a20 2020    # 2.11.13+.   
+00002b80: 2072 6574 656e 7469 6f6e 5f64 7572 6174   retention_durat
+00002b90: 696f 6e3a 204f 7074 696f 6e61 6c5b 6461  ion: Optional[da
+00002ba0: 7465 7469 6d65 5d20 3d20 4e6f 6e65 0a20  tetime] = None. 
+00002bb0: 2020 2073 6d61 7274 5f64 6574 6563 745f     smart_detect_
+00002bc0: 706f 7374 5f70 6164 6469 6e67 3a20 4f70  post_padding: Op
+00002bd0: 7469 6f6e 616c 5b74 696d 6564 656c 7461  tional[timedelta
+00002be0: 5d20 3d20 4e6f 6e65 0a20 2020 2073 6d61  ] = None.    sma
+00002bf0: 7274 5f64 6574 6563 745f 7072 655f 7061  rt_detect_pre_pa
+00002c00: 6464 696e 673a 204f 7074 696f 6e61 6c5b  dding: Optional[
+00002c10: 7469 6d65 6465 6c74 615d 203d 204e 6f6e  timedelta] = Non
+00002c20: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
+00002c30: 686f 640a 2020 2020 4063 6163 6865 0a20  hod.    @cache. 
+00002c40: 2020 2064 6566 205f 6765 745f 756e 6966     def _get_unif
+00002c50: 695f 7265 6d61 7073 2863 6c73 2920 2d3e  i_remaps(cls) ->
+00002c60: 2064 6963 745b 7374 722c 2073 7472 5d3a   dict[str, str]:
+00002c70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002c80: 7b0a 2020 2020 2020 2020 2020 2020 2a2a  {.            **
+00002c90: 7375 7065 7228 292e 5f67 6574 5f75 6e69  super()._get_uni
+00002ca0: 6669 5f72 656d 6170 7328 292c 0a20 2020  fi_remaps(),.   
+00002cb0: 2020 2020 2020 2020 2022 7265 7465 6e74           "retent
+00002cc0: 696f 6e44 7572 6174 696f 6e4d 7322 3a20  ionDurationMs": 
+00002cd0: 2272 6574 656e 7469 6f6e 4475 7261 7469  "retentionDurati
+00002ce0: 6f6e 222c 0a20 2020 2020 2020 207d 0a0a  on",.        }..
+00002cf0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00002d00: 0a20 2020 2064 6566 2075 6e69 6669 5f64  .    def unifi_d
+00002d10: 6963 745f 746f 5f64 6963 7428 636c 732c  ict_to_dict(cls,
+00002d20: 2064 6174 613a 2064 6963 745b 7374 722c   data: dict[str,
+00002d30: 2041 6e79 5d29 202d 3e20 6469 6374 5b73   Any]) -> dict[s
+00002d40: 7472 2c20 416e 795d 3a0a 2020 2020 2020  tr, Any]:.      
+00002d50: 2020 6966 2022 7072 6550 6164 6469 6e67    if "prePadding
+00002d60: 5365 6373 2220 696e 2064 6174 613a 0a20  Secs" in data:. 
+00002d70: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00002d80: 2270 7265 5061 6464 696e 6722 5d20 3d20  "prePadding"] = 
+00002d90: 7469 6d65 6465 6c74 6128 7365 636f 6e64  timedelta(second
+00002da0: 733d 6461 7461 2e70 6f70 2822 7072 6550  s=data.pop("preP
+00002db0: 6164 6469 6e67 5365 6373 2229 290a 2020  addingSecs")).  
+00002dc0: 2020 2020 2020 6966 2022 706f 7374 5061        if "postPa
+00002dd0: 6464 696e 6753 6563 7322 2069 6e20 6461  ddingSecs" in da
+00002de0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00002df0: 6461 7461 5b22 706f 7374 5061 6464 696e  data["postPaddin
+00002e00: 6722 5d20 3d20 7469 6d65 6465 6c74 6128  g"] = timedelta(
+00002e10: 7365 636f 6e64 733d 6461 7461 2e70 6f70  seconds=data.pop
+00002e20: 2822 706f 7374 5061 6464 696e 6753 6563  ("postPaddingSec
+00002e30: 7322 2929 0a20 2020 2020 2020 2069 6620  s")).        if 
+00002e40: 2273 6d61 7274 4465 7465 6374 5072 6550  "smartDetectPreP
+00002e50: 6164 6469 6e67 5365 6373 2220 696e 2064  addingSecs" in d
+00002e60: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00002e70: 2064 6174 615b 2273 6d61 7274 4465 7465   data["smartDete
+00002e80: 6374 5072 6550 6164 6469 6e67 225d 203d  ctPrePadding"] =
+00002e90: 2074 696d 6564 656c 7461 280a 2020 2020   timedelta(.    
+00002ea0: 2020 2020 2020 2020 2020 2020 7365 636f              seco
+00002eb0: 6e64 733d 6461 7461 2e70 6f70 2822 736d  nds=data.pop("sm
+00002ec0: 6172 7444 6574 6563 7450 7265 5061 6464  artDetectPrePadd
+00002ed0: 696e 6753 6563 7322 292c 0a20 2020 2020  ingSecs"),.     
+00002ee0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00002ef0: 2069 6620 2273 6d61 7274 4465 7465 6374   if "smartDetect
+00002f00: 506f 7374 5061 6464 696e 6753 6563 7322  PostPaddingSecs"
+00002f10: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
+00002f20: 2020 2020 2020 6461 7461 5b22 736d 6172        data["smar
+00002f30: 7444 6574 6563 7450 6f73 7450 6164 6469  tDetectPostPaddi
+00002f40: 6e67 225d 203d 2074 696d 6564 656c 7461  ng"] = timedelta
+00002f50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002f60: 2020 7365 636f 6e64 733d 6461 7461 2e70    seconds=data.p
+00002f70: 6f70 2822 736d 6172 7444 6574 6563 7450  op("smartDetectP
+00002f80: 6f73 7450 6164 6469 6e67 5365 6373 2229  ostPaddingSecs")
+00002f90: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00002fa0: 2020 2020 2020 2020 6966 2022 6d69 6e4d          if "minM
+00002fb0: 6f74 696f 6e45 7665 6e74 5472 6967 6765  otionEventTrigge
+00002fc0: 7222 2069 6e20 6461 7461 2061 6e64 206e  r" in data and n
+00002fd0: 6f74 2069 7369 6e73 7461 6e63 6528 0a20  ot isinstance(. 
+00002fe0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00002ff0: 226d 696e 4d6f 7469 6f6e 4576 656e 7454  "minMotionEventT
+00003000: 7269 6767 6572 225d 2c0a 2020 2020 2020  rigger"],.      
+00003010: 2020 2020 2020 7469 6d65 6465 6c74 612c        timedelta,
+00003020: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+00003030: 2020 2020 2020 2020 6461 7461 5b22 6d69          data["mi
+00003040: 6e4d 6f74 696f 6e45 7665 6e74 5472 6967  nMotionEventTrig
+00003050: 6765 7222 5d20 3d20 7469 6d65 6465 6c74  ger"] = timedelt
+00003060: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
+00003070: 2020 2073 6563 6f6e 6473 3d64 6174 615b     seconds=data[
+00003080: 226d 696e 4d6f 7469 6f6e 4576 656e 7454  "minMotionEventT
+00003090: 7269 6767 6572 225d 2c0a 2020 2020 2020  rigger"],.      
+000030a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000030b0: 6966 2022 656e 644d 6f74 696f 6e45 7665  if "endMotionEve
+000030c0: 6e74 4465 6c61 7922 2069 6e20 6461 7461  ntDelay" in data
+000030d0: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
+000030e0: 6e63 6528 0a20 2020 2020 2020 2020 2020  nce(.           
+000030f0: 2064 6174 615b 2265 6e64 4d6f 7469 6f6e   data["endMotion
+00003100: 4576 656e 7444 656c 6179 225d 2c0a 2020  EventDelay"],.  
+00003110: 2020 2020 2020 2020 2020 7469 6d65 6465            timede
+00003120: 6c74 612c 0a20 2020 2020 2020 2029 3a0a  lta,.        ):.
+00003130: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00003140: 5b22 656e 644d 6f74 696f 6e45 7665 6e74  ["endMotionEvent
+00003150: 4465 6c61 7922 5d20 3d20 7469 6d65 6465  Delay"] = timede
+00003160: 6c74 6128 7365 636f 6e64 733d 6461 7461  lta(seconds=data
+00003170: 5b22 656e 644d 6f74 696f 6e45 7665 6e74  ["endMotionEvent
+00003180: 4465 6c61 7922 5d29 0a0a 2020 2020 2020  Delay"])..      
+00003190: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000031a0: 2e75 6e69 6669 5f64 6963 745f 746f 5f64  .unifi_dict_to_d
+000031b0: 6963 7428 6461 7461 290a 0a20 2020 2064  ict(data)..    d
+000031c0: 6566 2075 6e69 6669 5f64 6963 7428 0a20  ef unifi_dict(. 
+000031d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000031e0: 2020 2020 2064 6174 613a 204f 7074 696f       data: Optio
+000031f0: 6e61 6c5b 6469 6374 5b73 7472 2c20 416e  nal[dict[str, An
+00003200: 795d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  y]] = None,.    
+00003210: 2020 2020 6578 636c 7564 653a 204f 7074      exclude: Opt
+00003220: 696f 6e61 6c5b 7365 745b 7374 725d 5d20  ional[set[str]] 
+00003230: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
+00003240: 2064 6963 745b 7374 722c 2041 6e79 5d3a   dict[str, Any]:
+00003250: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00003260: 7375 7065 7228 292e 756e 6966 695f 6469  super().unifi_di
+00003270: 6374 2864 6174 613d 6461 7461 2c20 6578  ct(data=data, ex
+00003280: 636c 7564 653d 6578 636c 7564 6529 0a0a  clude=exclude)..
+00003290: 2020 2020 2020 2020 6966 2022 7072 6550          if "preP
+000032a0: 6164 6469 6e67 2220 696e 2064 6174 613a  adding" in data:
+000032b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000032c0: 615b 2270 7265 5061 6464 696e 6753 6563  a["prePaddingSec
+000032d0: 7322 5d20 3d20 6461 7461 2e70 6f70 2822  s"] = data.pop("
+000032e0: 7072 6550 6164 6469 6e67 2229 202f 2f20  prePadding") // 
+000032f0: 3130 3030 0a20 2020 2020 2020 2069 6620  1000.        if 
+00003300: 2270 6f73 7450 6164 6469 6e67 2220 696e  "postPadding" in
+00003310: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+00003320: 2020 2064 6174 615b 2270 6f73 7450 6164     data["postPad
+00003330: 6469 6e67 5365 6373 225d 203d 2064 6174  dingSecs"] = dat
+00003340: 612e 706f 7028 2270 6f73 7450 6164 6469  a.pop("postPaddi
+00003350: 6e67 2229 202f 2f20 3130 3030 0a20 2020  ng") // 1000.   
+00003360: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00003370: 2020 2020 2020 2273 6d61 7274 4465 7465        "smartDete
+00003380: 6374 5072 6550 6164 6469 6e67 2220 696e  ctPrePadding" in
+00003390: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+000033a0: 2020 616e 6420 6461 7461 5b22 736d 6172    and data["smar
+000033b0: 7444 6574 6563 7450 7265 5061 6464 696e  tDetectPrePaddin
+000033c0: 6722 5d20 6973 206e 6f74 204e 6f6e 650a  g"] is not None.
+000033d0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+000033e0: 2020 2020 2020 2064 6174 615b 2273 6d61         data["sma
+000033f0: 7274 4465 7465 6374 5072 6550 6164 6469  rtDetectPrePaddi
+00003400: 6e67 5365 6373 225d 203d 2028 0a20 2020  ngSecs"] = (.   
+00003410: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00003420: 612e 706f 7028 2273 6d61 7274 4465 7465  a.pop("smartDete
+00003430: 6374 5072 6550 6164 6469 6e67 2229 202f  ctPrePadding") /
+00003440: 2f20 3130 3030 0a20 2020 2020 2020 2020  / 1000.         
+00003450: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00003460: 280a 2020 2020 2020 2020 2020 2020 2273  (.            "s
+00003470: 6d61 7274 4465 7465 6374 506f 7374 5061  martDetectPostPa
+00003480: 6464 696e 6722 2069 6e20 6461 7461 0a20  dding" in data. 
+00003490: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
+000034a0: 6174 615b 2273 6d61 7274 4465 7465 6374  ata["smartDetect
+000034b0: 506f 7374 5061 6464 696e 6722 5d20 6973  PostPadding"] is
+000034c0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+000034d0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000034e0: 2064 6174 615b 2273 6d61 7274 4465 7465   data["smartDete
+000034f0: 6374 506f 7374 5061 6464 696e 6753 6563  ctPostPaddingSec
+00003500: 7322 5d20 3d20 280a 2020 2020 2020 2020  s"] = (.        
+00003510: 2020 2020 2020 2020 6461 7461 2e70 6f70          data.pop
+00003520: 2822 736d 6172 7444 6574 6563 7450 6f73  ("smartDetectPos
+00003530: 7450 6164 6469 6e67 2229 202f 2f20 3130  tPadding") // 10
+00003540: 3030 0a20 2020 2020 2020 2020 2020 2029  00.            )
+00003550: 0a20 2020 2020 2020 2069 6620 226d 696e  .        if "min
+00003560: 4d6f 7469 6f6e 4576 656e 7454 7269 6767  MotionEventTrigg
+00003570: 6572 2220 696e 2064 6174 613a 0a20 2020  er" in data:.   
+00003580: 2020 2020 2020 2020 2064 6174 615b 226d           data["m
+00003590: 696e 4d6f 7469 6f6e 4576 656e 7454 7269  inMotionEventTri
+000035a0: 6767 6572 225d 203d 2064 6174 612e 706f  gger"] = data.po
+000035b0: 7028 226d 696e 4d6f 7469 6f6e 4576 656e  p("minMotionEven
+000035c0: 7454 7269 6767 6572 2229 202f 2f20 3130  tTrigger") // 10
+000035d0: 3030 0a20 2020 2020 2020 2069 6620 2265  00.        if "e
+000035e0: 6e64 4d6f 7469 6f6e 4576 656e 7444 656c  ndMotionEventDel
+000035f0: 6179 2220 696e 2064 6174 613a 0a20 2020  ay" in data:.   
+00003600: 2020 2020 2020 2020 2064 6174 615b 2265           data["e
+00003610: 6e64 4d6f 7469 6f6e 4576 656e 7444 656c  ndMotionEventDel
+00003620: 6179 225d 203d 2064 6174 612e 706f 7028  ay"] = data.pop(
+00003630: 2265 6e64 4d6f 7469 6f6e 4576 656e 7444  "endMotionEventD
+00003640: 656c 6179 2229 202f 2f20 3130 3030 0a0a  elay") // 1000..
+00003650: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00003660: 6174 610a 0a0a 636c 6173 7320 536d 6172  ata...class Smar
+00003670: 7444 6574 6563 7453 6574 7469 6e67 7328  tDetectSettings(
+00003680: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
+00003690: 7429 3a0a 2020 2020 6f62 6a65 6374 5f74  t):.    object_t
+000036a0: 7970 6573 3a20 6c69 7374 5b53 6d61 7274  ypes: list[Smart
+000036b0: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+000036c0: 5d0a 2020 2020 6175 6469 6f5f 7479 7065  ].    audio_type
+000036d0: 733a 204f 7074 696f 6e61 6c5b 6c69 7374  s: Optional[list
+000036e0: 5b53 6d61 7274 4465 7465 6374 4175 6469  [SmartDetectAudi
+000036f0: 6f54 7970 655d 5d20 3d20 4e6f 6e65 0a20  oType]] = None. 
+00003700: 2020 2023 2072 6571 7569 7265 7320 322e     # requires 2.
+00003710: 382e 3232 2b0a 2020 2020 6175 746f 5f74  8.22+.    auto_t
+00003720: 7261 636b 696e 675f 6f62 6a65 6374 5f74  racking_object_t
+00003730: 7970 6573 3a20 4f70 7469 6f6e 616c 5b6c  ypes: Optional[l
+00003740: 6973 745b 536d 6172 7444 6574 6563 744f  ist[SmartDetectO
+00003750: 626a 6563 7454 7970 655d 5d20 3d20 4e6f  bjectType]] = No
+00003760: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
+00003770: 7468 6f64 0a20 2020 2064 6566 2075 6e69  thod.    def uni
+00003780: 6669 5f64 6963 745f 746f 5f64 6963 7428  fi_dict_to_dict(
+00003790: 636c 732c 2064 6174 613a 2064 6963 745b  cls, data: dict[
+000037a0: 7374 722c 2041 6e79 5d29 202d 3e20 6469  str, Any]) -> di
+000037b0: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
+000037c0: 2020 2020 2020 6966 2022 6f62 6a65 6374        if "object
+000037d0: 5479 7065 7322 2069 6e20 6461 7461 3a0a  Types" in data:.
+000037e0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000037f0: 5b22 6f62 6a65 6374 5479 7065 7322 5d20  ["objectTypes"] 
+00003800: 3d20 636f 6e76 6572 745f 736d 6172 745f  = convert_smart_
+00003810: 7479 7065 7328 6461 7461 2e70 6f70 2822  types(data.pop("
+00003820: 6f62 6a65 6374 5479 7065 7322 2929 0a20  objectTypes")). 
+00003830: 2020 2020 2020 2069 6620 2261 7564 696f         if "audio
+00003840: 5479 7065 7322 2069 6e20 6461 7461 3a0a  Types" in data:.
+00003850: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00003860: 5b22 6175 6469 6f54 7970 6573 225d 203d  ["audioTypes"] =
+00003870: 2063 6f6e 7665 7274 5f73 6d61 7274 5f61   convert_smart_a
+00003880: 7564 696f 5f74 7970 6573 2864 6174 612e  udio_types(data.
+00003890: 706f 7028 2261 7564 696f 5479 7065 7322  pop("audioTypes"
+000038a0: 2929 0a20 2020 2020 2020 2069 6620 2261  )).        if "a
+000038b0: 7574 6f54 7261 636b 696e 674f 626a 6563  utoTrackingObjec
+000038c0: 7454 7970 6573 2220 696e 2064 6174 613a  tTypes" in data:
+000038d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000038e0: 615b 2261 7574 6f54 7261 636b 696e 674f  a["autoTrackingO
+000038f0: 626a 6563 7454 7970 6573 225d 203d 2063  bjectTypes"] = c
+00003900: 6f6e 7665 7274 5f73 6d61 7274 5f74 7970  onvert_smart_typ
+00003910: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00003920: 2020 2020 6461 7461 2e70 6f70 2822 6175      data.pop("au
+00003930: 746f 5472 6163 6b69 6e67 4f62 6a65 6374  toTrackingObject
+00003940: 5479 7065 7322 292c 0a20 2020 2020 2020  Types"),.       
+00003950: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00003960: 7265 7475 726e 2073 7570 6572 2829 2e75  return super().u
+00003970: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
+00003980: 7428 6461 7461 290a 0a0a 636c 6173 7320  t(data)...class 
+00003990: 4c43 444d 6573 7361 6765 2850 726f 7465  LCDMessage(Prote
+000039a0: 6374 4261 7365 4f62 6a65 6374 293a 0a20  ctBaseObject):. 
+000039b0: 2020 2074 7970 653a 2044 6f6f 7262 656c     type: Doorbel
+000039c0: 6c4d 6573 7361 6765 5479 7065 0a20 2020  lMessageType.   
+000039d0: 2074 6578 743a 2073 7472 0a20 2020 2072   text: str.    r
+000039e0: 6573 6574 5f61 743a 204f 7074 696f 6e61  eset_at: Optiona
+000039f0: 6c5b 6461 7465 7469 6d65 5d20 3d20 4e6f  l[datetime] = No
+00003a00: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
+00003a10: 7468 6f64 0a20 2020 2064 6566 2075 6e69  thod.    def uni
+00003a20: 6669 5f64 6963 745f 746f 5f64 6963 7428  fi_dict_to_dict(
+00003a30: 636c 732c 2064 6174 613a 2064 6963 745b  cls, data: dict[
+00003a40: 7374 722c 2041 6e79 5d29 202d 3e20 6469  str, Any]) -> di
+00003a50: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
+00003a60: 2020 2020 2020 6966 2022 7265 7365 7441        if "resetA
+00003a70: 7422 2069 6e20 6461 7461 3a0a 2020 2020  t" in data:.    
+00003a80: 2020 2020 2020 2020 6461 7461 5b22 7265          data["re
+00003a90: 7365 7441 7422 5d20 3d20 7072 6f63 6573  setAt"] = proces
+00003aa0: 735f 6461 7465 7469 6d65 2864 6174 612c  s_datetime(data,
+00003ab0: 2022 7265 7365 7441 7422 290a 2020 2020   "resetAt").    
+00003ac0: 2020 2020 6966 2022 7465 7874 2220 696e      if "text" in
+00003ad0: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+00003ae0: 2020 2023 2055 6e69 4669 2050 726f 7465     # UniFi Prote
+00003af0: 6374 2062 7567 3a20 736f 6d65 2074 696d  ct bug: some tim
+00003b00: 6573 204c 4344 206d 6573 7361 6765 7320  es LCD messages 
+00003b10: 6361 6e20 6765 7420 696e 746f 2061 2062  can get into a b
+00003b20: 6164 2073 7461 7465 2077 6865 7265 206d  ad state where m
+00003b30: 6573 7361 6765 203d 2044 4546 4155 4c54  essage = DEFAULT
+00003b40: 204d 4553 5341 4745 2c20 6275 7420 6e6f   MESSAGE, but no
+00003b50: 2074 7970 650a 2020 2020 2020 2020 2020   type.          
+00003b60: 2020 6966 2022 7479 7065 2220 6e6f 7420    if "type" not 
+00003b70: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
+00003b80: 2020 2020 2020 2020 2064 6174 615b 2274           data["t
+00003b90: 7970 6522 5d20 3d20 446f 6f72 6265 6c6c  ype"] = Doorbell
+00003ba0: 4d65 7373 6167 6554 7970 652e 4355 5354  MessageType.CUST
+00003bb0: 4f4d 5f4d 4553 5341 4745 2e76 616c 7565  OM_MESSAGE.value
+00003bc0: 0a0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00003bd0: 7461 5b22 7465 7874 225d 203d 2063 6c73  ta["text"] = cls
+00003be0: 2e5f 6669 785f 7465 7874 2864 6174 615b  ._fix_text(data[
+00003bf0: 2274 6578 7422 5d2c 2064 6174 615b 2274  "text"], data["t
+00003c00: 7970 6522 5d29 0a0a 2020 2020 2020 2020  ype"])..        
+00003c10: 7265 7475 726e 2073 7570 6572 2829 2e75  return super().u
+00003c20: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
+00003c30: 7428 6461 7461 290a 0a20 2020 2040 636c  t(data)..    @cl
+00003c40: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00003c50: 6620 5f66 6978 5f74 6578 7428 636c 732c  f _fix_text(cls,
+00003c60: 2074 6578 743a 2073 7472 2c20 7465 7874   text: str, text
+00003c70: 5f74 7970 653a 204f 7074 696f 6e61 6c5b  _type: Optional[
+00003c80: 7374 725d 2920 2d3e 2073 7472 3a0a 2020  str]) -> str:.  
+00003c90: 2020 2020 2020 6966 2074 6578 745f 7479        if text_ty
+00003ca0: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00003cb0: 2020 2020 2020 2020 7465 7874 5f74 7970          text_typ
+00003cc0: 6520 3d20 636c 732e 7479 7065 2e76 616c  e = cls.type.val
+00003cd0: 7565 0a0a 2020 2020 2020 2020 6966 2074  ue..        if t
+00003ce0: 6578 745f 7479 7065 2021 3d20 446f 6f72  ext_type != Door
+00003cf0: 6265 6c6c 4d65 7373 6167 6554 7970 652e  bellMessageType.
+00003d00: 4355 5354 4f4d 5f4d 4553 5341 4745 2e76  CUSTOM_MESSAGE.v
+00003d10: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
+00003d20: 2020 7465 7874 203d 2074 6578 745f 7479    text = text_ty
+00003d30: 7065 2e72 6570 6c61 6365 2822 5f22 2c20  pe.replace("_", 
+00003d40: 2220 2229 0a0a 2020 2020 2020 2020 7265  " ")..        re
+00003d50: 7475 726e 2074 6578 740a 0a20 2020 2064  turn text..    d
+00003d60: 6566 2075 6e69 6669 5f64 6963 7428 0a20  ef unifi_dict(. 
+00003d70: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00003d80: 2020 2020 2064 6174 613a 204f 7074 696f       data: Optio
+00003d90: 6e61 6c5b 6469 6374 5b73 7472 2c20 416e  nal[dict[str, An
+00003da0: 795d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  y]] = None,.    
+00003db0: 2020 2020 6578 636c 7564 653a 204f 7074      exclude: Opt
+00003dc0: 696f 6e61 6c5b 7365 745b 7374 725d 5d20  ional[set[str]] 
+00003dd0: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
+00003de0: 2064 6963 745b 7374 722c 2041 6e79 5d3a   dict[str, Any]:
+00003df0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00003e00: 7375 7065 7228 292e 756e 6966 695f 6469  super().unifi_di
+00003e10: 6374 2864 6174 613d 6461 7461 2c20 6578  ct(data=data, ex
+00003e20: 636c 7564 653d 6578 636c 7564 6529 0a0a  clude=exclude)..
+00003e30: 2020 2020 2020 2020 6966 2022 7465 7874          if "text
+00003e40: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
+00003e50: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00003e60: 2020 2020 2020 2020 2020 2020 6d73 675f              msg_
+00003e70: 7479 7065 203d 2073 656c 662e 7479 7065  type = self.type
+00003e80: 2e76 616c 7565 0a20 2020 2020 2020 2020  .value.         
+00003e90: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
+00003ea0: 7574 6545 7272 6f72 3a0a 2020 2020 2020  uteError:.      
+00003eb0: 2020 2020 2020 2020 2020 6d73 675f 7479            msg_ty
+00003ec0: 7065 203d 204e 6f6e 650a 0a20 2020 2020  pe = None..     
+00003ed0: 2020 2020 2020 2064 6174 615b 2274 6578         data["tex
+00003ee0: 7422 5d20 3d20 7365 6c66 2e5f 6669 785f  t"] = self._fix_
+00003ef0: 7465 7874 2864 6174 615b 2274 6578 7422  text(data["text"
+00003f00: 5d2c 2064 6174 612e 6765 7428 2274 7970  ], data.get("typ
+00003f10: 6522 2c20 6d73 675f 7479 7065 2929 0a20  e", msg_type)). 
+00003f20: 2020 2020 2020 2069 6620 2272 6573 6574         if "reset
+00003f30: 4174 2220 696e 2064 6174 613a 0a20 2020  At" in data:.   
+00003f40: 2020 2020 2020 2020 2064 6174 615b 2272           data["r
+00003f50: 6573 6574 4174 225d 203d 2074 6f5f 6a73  esetAt"] = to_js
+00003f60: 5f74 696d 6528 6461 7461 5b22 7265 7365  _time(data["rese
+00003f70: 7441 7422 5d29 0a0a 2020 2020 2020 2020  tAt"])..        
+00003f80: 7265 7475 726e 2064 6174 610a 0a0a 636c  return data...cl
+00003f90: 6173 7320 5461 6c6b 6261 636b 5365 7474  ass TalkbackSett
+00003fa0: 696e 6773 2850 726f 7465 6374 4261 7365  ings(ProtectBase
+00003fb0: 4f62 6a65 6374 293a 0a20 2020 2074 7970  Object):.    typ
+00003fc0: 655f 666d 743a 2041 7564 696f 436f 6465  e_fmt: AudioCode
+00003fd0: 6373 0a20 2020 2074 7970 655f 696e 3a20  cs.    type_in: 
+00003fe0: 7374 720a 2020 2020 6269 6e64 5f61 6464  str.    bind_add
+00003ff0: 723a 2049 5076 3441 6464 7265 7373 0a20  r: IPv4Address. 
+00004000: 2020 2062 696e 645f 706f 7274 3a20 696e     bind_port: in
+00004010: 740a 2020 2020 6669 6c74 6572 5f61 6464  t.    filter_add
+00004020: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
+00004030: 2020 2320 6361 6e20 6265 2075 7365 6420    # can be used 
+00004040: 746f 2072 6573 7472 6963 7420 7365 6e64  to restrict send
+00004050: 6572 2061 6464 7265 7373 0a20 2020 2066  er address.    f
+00004060: 696c 7465 725f 706f 7274 3a20 4f70 7469  ilter_port: Opti
+00004070: 6f6e 616c 5b69 6e74 5d20 2023 2063 616e  onal[int]  # can
+00004080: 2062 6520 7573 6564 2074 6f20 7265 7374   be used to rest
+00004090: 7269 6374 2073 656e 6465 7220 706f 7274  rict sender port
+000040a0: 0a20 2020 2063 6861 6e6e 656c 733a 2069  .    channels: i
+000040b0: 6e74 2020 2320 3120 6f72 2032 0a20 2020  nt  # 1 or 2.   
+000040c0: 2073 616d 706c 696e 675f 7261 7465 3a20   sampling_rate: 
+000040d0: 696e 7420 2023 2038 3030 302c 2031 3130  int  # 8000, 110
+000040e0: 3235 2c20 3232 3035 302c 2034 3431 3030  25, 22050, 44100
+000040f0: 2c20 3438 3030 300a 2020 2020 6269 7473  , 48000.    bits
+00004100: 5f70 6572 5f73 616d 706c 653a 2069 6e74  _per_sample: int
+00004110: 0a20 2020 2071 7561 6c69 7479 3a20 5065  .    quality: Pe
+00004120: 7263 656e 7449 6e74 2020 2320 6f6e 6c79  rcentInt  # only
+00004130: 2066 6f72 2076 6f72 6269 730a 0a0a 636c   for vorbis...cl
+00004140: 6173 7320 5769 6669 5374 6174 7328 5072  ass WifiStats(Pr
+00004150: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
+00004160: 3a0a 2020 2020 6368 616e 6e65 6c3a 204f  :.    channel: O
+00004170: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
+00004180: 2066 7265 7175 656e 6379 3a20 4f70 7469   frequency: Opti
+00004190: 6f6e 616c 5b69 6e74 5d0a 2020 2020 6c69  onal[int].    li
+000041a0: 6e6b 5f73 7065 6564 5f6d 6270 733a 204f  nk_speed_mbps: O
+000041b0: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
+000041c0: 2073 6967 6e61 6c5f 7175 616c 6974 793a   signal_quality:
+000041d0: 2050 6572 6365 6e74 496e 740a 2020 2020   PercentInt.    
+000041e0: 7369 676e 616c 5f73 7472 656e 6774 683a  signal_strength:
+000041f0: 2069 6e74 0a0a 0a63 6c61 7373 2056 6964   int...class Vid
+00004200: 656f 5374 6174 7328 5072 6f74 6563 7442  eoStats(ProtectB
+00004210: 6173 654f 626a 6563 7429 3a0a 2020 2020  aseObject):.    
+00004220: 7265 636f 7264 696e 675f 7374 6172 743a  recording_start:
+00004230: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
+00004240: 6d65 5d0a 2020 2020 7265 636f 7264 696e  me].    recordin
+00004250: 675f 656e 643a 204f 7074 696f 6e61 6c5b  g_end: Optional[
+00004260: 6461 7465 7469 6d65 5d0a 2020 2020 7265  datetime].    re
+00004270: 636f 7264 696e 675f 7374 6172 745f 6c71  cording_start_lq
+00004280: 3a20 4f70 7469 6f6e 616c 5b64 6174 6574  : Optional[datet
+00004290: 696d 655d 0a20 2020 2072 6563 6f72 6469  ime].    recordi
+000042a0: 6e67 5f65 6e64 5f6c 713a 204f 7074 696f  ng_end_lq: Optio
+000042b0: 6e61 6c5b 6461 7465 7469 6d65 5d0a 2020  nal[datetime].  
+000042c0: 2020 7469 6d65 6c61 7073 655f 7374 6172    timelapse_star
+000042d0: 743a 204f 7074 696f 6e61 6c5b 6461 7465  t: Optional[date
+000042e0: 7469 6d65 5d0a 2020 2020 7469 6d65 6c61  time].    timela
+000042f0: 7073 655f 656e 643a 204f 7074 696f 6e61  pse_end: Optiona
+00004300: 6c5b 6461 7465 7469 6d65 5d0a 2020 2020  l[datetime].    
+00004310: 7469 6d65 6c61 7073 655f 7374 6172 745f  timelapse_start_
+00004320: 6c71 3a20 4f70 7469 6f6e 616c 5b64 6174  lq: Optional[dat
+00004330: 6574 696d 655d 0a20 2020 2074 696d 656c  etime].    timel
+00004340: 6170 7365 5f65 6e64 5f6c 713a 204f 7074  apse_end_lq: Opt
+00004350: 696f 6e61 6c5b 6461 7465 7469 6d65 5d0a  ional[datetime].
+00004360: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00004370: 640a 2020 2020 4063 6163 6865 0a20 2020  d.    @cache.   
+00004380: 2064 6566 205f 6765 745f 756e 6966 695f   def _get_unifi_
+00004390: 7265 6d61 7073 2863 6c73 2920 2d3e 2064  remaps(cls) -> d
+000043a0: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
+000043b0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+000043c0: 2020 2020 2020 2020 2020 2020 2a2a 7375              **su
+000043d0: 7065 7228 292e 5f67 6574 5f75 6e69 6669  per()._get_unifi
+000043e0: 5f72 656d 6170 7328 292c 0a20 2020 2020  _remaps(),.     
+000043f0: 2020 2020 2020 2022 7265 636f 7264 696e         "recordin
+00004400: 6753 7461 7274 4c51 223a 2022 7265 636f  gStartLQ": "reco
+00004410: 7264 696e 6753 7461 7274 4c71 222c 0a20  rdingStartLq",. 
+00004420: 2020 2020 2020 2020 2020 2022 7265 636f             "reco
+00004430: 7264 696e 6745 6e64 4c51 223a 2022 7265  rdingEndLQ": "re
+00004440: 636f 7264 696e 6745 6e64 4c71 222c 0a20  cordingEndLq",. 
+00004450: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
+00004460: 6c61 7073 6553 7461 7274 4c51 223a 2022  lapseStartLQ": "
+00004470: 7469 6d65 6c61 7073 6553 7461 7274 4c71  timelapseStartLq
+00004480: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00004490: 7469 6d65 6c61 7073 6545 6e64 4c51 223a  timelapseEndLQ":
+000044a0: 2022 7469 6d65 6c61 7073 6545 6e64 4c71   "timelapseEndLq
+000044b0: 222c 0a20 2020 2020 2020 207d 0a0a 2020  ",.        }..  
+000044c0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000044d0: 2020 2064 6566 2075 6e69 6669 5f64 6963     def unifi_dic
+000044e0: 745f 746f 5f64 6963 7428 636c 732c 2064  t_to_dict(cls, d
+000044f0: 6174 613a 2064 6963 745b 7374 722c 2041  ata: dict[str, A
+00004500: 6e79 5d29 202d 3e20 6469 6374 5b73 7472  ny]) -> dict[str
+00004510: 2c20 416e 795d 3a0a 2020 2020 2020 2020  , Any]:.        
+00004520: 6966 2022 7265 636f 7264 696e 6753 7461  if "recordingSta
+00004530: 7274 2220 696e 2064 6174 613a 0a20 2020  rt" in data:.   
+00004540: 2020 2020 2020 2020 2064 6174 615b 2272           data["r
+00004550: 6563 6f72 6469 6e67 5374 6172 7422 5d20  ecordingStart"] 
+00004560: 3d20 7072 6f63 6573 735f 6461 7465 7469  = process_dateti
+00004570: 6d65 2864 6174 612c 2022 7265 636f 7264  me(data, "record
+00004580: 696e 6753 7461 7274 2229 0a20 2020 2020  ingStart").     
+00004590: 2020 2069 6620 2272 6563 6f72 6469 6e67     if "recording
+000045a0: 456e 6422 2069 6e20 6461 7461 3a0a 2020  End" in data:.  
+000045b0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+000045c0: 7265 636f 7264 696e 6745 6e64 225d 203d  recordingEnd"] =
+000045d0: 2070 726f 6365 7373 5f64 6174 6574 696d   process_datetim
+000045e0: 6528 6461 7461 2c20 2272 6563 6f72 6469  e(data, "recordi
+000045f0: 6e67 456e 6422 290a 2020 2020 2020 2020  ngEnd").        
+00004600: 6966 2022 7265 636f 7264 696e 6753 7461  if "recordingSta
+00004610: 7274 4c51 2220 696e 2064 6174 613a 0a20  rtLQ" in data:. 
+00004620: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00004630: 2272 6563 6f72 6469 6e67 5374 6172 744c  "recordingStartL
+00004640: 5122 5d20 3d20 7072 6f63 6573 735f 6461  Q"] = process_da
+00004650: 7465 7469 6d65 2864 6174 612c 2022 7265  tetime(data, "re
+00004660: 636f 7264 696e 6753 7461 7274 4c51 2229  cordingStartLQ")
+00004670: 0a20 2020 2020 2020 2069 6620 2272 6563  .        if "rec
+00004680: 6f72 6469 6e67 456e 644c 5122 2069 6e20  ordingEndLQ" in 
+00004690: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+000046a0: 2020 6461 7461 5b22 7265 636f 7264 696e    data["recordin
+000046b0: 6745 6e64 4c51 225d 203d 2070 726f 6365  gEndLQ"] = proce
+000046c0: 7373 5f64 6174 6574 696d 6528 6461 7461  ss_datetime(data
+000046d0: 2c20 2272 6563 6f72 6469 6e67 456e 644c  , "recordingEndL
+000046e0: 5122 290a 2020 2020 2020 2020 6966 2022  Q").        if "
+000046f0: 7469 6d65 6c61 7073 6553 7461 7274 2220  timelapseStart" 
+00004700: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
+00004710: 2020 2020 2064 6174 615b 2274 696d 656c       data["timel
+00004720: 6170 7365 5374 6172 7422 5d20 3d20 7072  apseStart"] = pr
+00004730: 6f63 6573 735f 6461 7465 7469 6d65 2864  ocess_datetime(d
+00004740: 6174 612c 2022 7469 6d65 6c61 7073 6553  ata, "timelapseS
+00004750: 7461 7274 2229 0a20 2020 2020 2020 2069  tart").        i
+00004760: 6620 2274 696d 656c 6170 7365 456e 6422  f "timelapseEnd"
+00004770: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
+00004780: 2020 2020 2020 6461 7461 5b22 7469 6d65        data["time
+00004790: 6c61 7073 6545 6e64 225d 203d 2070 726f  lapseEnd"] = pro
+000047a0: 6365 7373 5f64 6174 6574 696d 6528 6461  cess_datetime(da
+000047b0: 7461 2c20 2274 696d 656c 6170 7365 456e  ta, "timelapseEn
+000047c0: 6422 290a 2020 2020 2020 2020 6966 2022  d").        if "
+000047d0: 7469 6d65 6c61 7073 6553 7461 7274 4c51  timelapseStartLQ
+000047e0: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
+000047f0: 2020 2020 2020 2064 6174 615b 2274 696d         data["tim
+00004800: 656c 6170 7365 5374 6172 744c 5122 5d20  elapseStartLQ"] 
+00004810: 3d20 7072 6f63 6573 735f 6461 7465 7469  = process_dateti
+00004820: 6d65 2864 6174 612c 2022 7469 6d65 6c61  me(data, "timela
+00004830: 7073 6553 7461 7274 4c51 2229 0a20 2020  pseStartLQ").   
+00004840: 2020 2020 2069 6620 2274 696d 656c 6170       if "timelap
+00004850: 7365 456e 644c 5122 2069 6e20 6461 7461  seEndLQ" in data
+00004860: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+00004870: 7461 5b22 7469 6d65 6c61 7073 6545 6e64  ta["timelapseEnd
+00004880: 4c51 225d 203d 2070 726f 6365 7373 5f64  LQ"] = process_d
+00004890: 6174 6574 696d 6528 6461 7461 2c20 2274  atetime(data, "t
+000048a0: 696d 656c 6170 7365 456e 644c 5122 290a  imelapseEndLQ").
+000048b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000048c0: 7375 7065 7228 292e 756e 6966 695f 6469  super().unifi_di
+000048d0: 6374 5f74 6f5f 6469 6374 2864 6174 6129  ct_to_dict(data)
+000048e0: 0a0a 0a63 6c61 7373 2053 746f 7261 6765  ...class Storage
+000048f0: 5374 6174 7328 5072 6f74 6563 7442 6173  Stats(ProtectBas
+00004900: 654f 626a 6563 7429 3a0a 2020 2020 7573  eObject):.    us
+00004910: 6564 3a20 4f70 7469 6f6e 616c 5b69 6e74  ed: Optional[int
+00004920: 5d20 2023 2062 7974 6573 0a20 2020 2072  ]  # bytes.    r
+00004930: 6174 653a 204f 7074 696f 6e61 6c5b 666c  ate: Optional[fl
+00004940: 6f61 745d 2020 2320 6279 7465 7320 2f20  oat]  # bytes / 
+00004950: 6d69 6c6c 6973 6563 6f6e 640a 0a20 2020  millisecond..   
+00004960: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00004970: 6566 2072 6174 655f 7065 725f 7365 636f  ef rate_per_seco
+00004980: 6e64 2873 656c 6629 202d 3e20 4f70 7469  nd(self) -> Opti
+00004990: 6f6e 616c 5b66 6c6f 6174 5d3a 0a20 2020  onal[float]:.   
+000049a0: 2020 2020 2069 6620 7365 6c66 2e72 6174       if self.rat
+000049b0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+000049c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000049d0: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
+000049e0: 726e 2073 656c 662e 7261 7465 202a 2031  rn self.rate * 1
+000049f0: 3030 300a 0a20 2020 2040 636c 6173 736d  000..    @classm
+00004a00: 6574 686f 640a 2020 2020 6465 6620 756e  ethod.    def un
+00004a10: 6966 695f 6469 6374 5f74 6f5f 6469 6374  ifi_dict_to_dict
+00004a20: 2863 6c73 2c20 6461 7461 3a20 6469 6374  (cls, data: dict
+00004a30: 5b73 7472 2c20 416e 795d 2920 2d3e 2064  [str, Any]) -> d
+00004a40: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
+00004a50: 2020 2020 2020 2069 6620 2272 6174 6522         if "rate"
+00004a60: 206e 6f74 2069 6e20 6461 7461 3a0a 2020   not in data:.  
+00004a70: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+00004a80: 7261 7465 225d 203d 204e 6f6e 650a 0a20  rate"] = None.. 
+00004a90: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+00004aa0: 7065 7228 292e 756e 6966 695f 6469 6374  per().unifi_dict
+00004ab0: 5f74 6f5f 6469 6374 2864 6174 6129 0a0a  _to_dict(data)..
+00004ac0: 2020 2020 6465 6620 756e 6966 695f 6469      def unifi_di
+00004ad0: 6374 280a 2020 2020 2020 2020 7365 6c66  ct(.        self
+00004ae0: 2c0a 2020 2020 2020 2020 6461 7461 3a20  ,.        data: 
+00004af0: 4f70 7469 6f6e 616c 5b64 6963 745b 7374  Optional[dict[st
+00004b00: 722c 2041 6e79 5d5d 203d 204e 6f6e 652c  r, Any]] = None,
+00004b10: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+00004b20: 3a20 4f70 7469 6f6e 616c 5b73 6574 5b73  : Optional[set[s
+00004b30: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00004b40: 2029 202d 3e20 6469 6374 5b73 7472 2c20   ) -> dict[str, 
+00004b50: 416e 795d 3a0a 2020 2020 2020 2020 6461  Any]:.        da
+00004b60: 7461 203d 2073 7570 6572 2829 2e75 6e69  ta = super().uni
+00004b70: 6669 5f64 6963 7428 6461 7461 3d64 6174  fi_dict(data=dat
+00004b80: 612c 2065 7863 6c75 6465 3d65 7863 6c75  a, exclude=exclu
+00004b90: 6465 290a 0a20 2020 2020 2020 2069 6620  de)..        if 
+00004ba0: 2272 6174 6522 2069 6e20 6461 7461 2061  "rate" in data a
+00004bb0: 6e64 2064 6174 615b 2272 6174 6522 5d20  nd data["rate"] 
+00004bc0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00004bd0: 2020 2020 2064 656c 2064 6174 615b 2272       del data["r
+00004be0: 6174 6522 5d0a 0a20 2020 2020 2020 2072  ate"]..        r
+00004bf0: 6574 7572 6e20 6461 7461 0a0a 0a63 6c61  eturn data...cla
+00004c00: 7373 2043 616d 6572 6153 7461 7473 2850  ss CameraStats(P
+00004c10: 726f 7465 6374 4261 7365 4f62 6a65 6374  rotectBaseObject
+00004c20: 293a 0a20 2020 2072 785f 6279 7465 733a  ):.    rx_bytes:
+00004c30: 2069 6e74 0a20 2020 2074 785f 6279 7465   int.    tx_byte
+00004c40: 733a 2069 6e74 0a20 2020 2077 6966 693a  s: int.    wifi:
+00004c50: 2057 6966 6953 7461 7473 0a20 2020 2076   WifiStats.    v
+00004c60: 6964 656f 3a20 5669 6465 6f53 7461 7473  ideo: VideoStats
+00004c70: 0a20 2020 2073 746f 7261 6765 3a20 4f70  .    storage: Op
+00004c80: 7469 6f6e 616c 5b53 746f 7261 6765 5374  tional[StorageSt
+00004c90: 6174 735d 0a20 2020 2077 6966 695f 7175  ats].    wifi_qu
+00004ca0: 616c 6974 793a 2050 6572 6365 6e74 496e  ality: PercentIn
+00004cb0: 740a 2020 2020 7769 6669 5f73 7472 656e  t.    wifi_stren
+00004cc0: 6774 683a 2069 6e74 0a0a 2020 2020 4063  gth: int..    @c
+00004cd0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00004ce0: 6566 2075 6e69 6669 5f64 6963 745f 746f  ef unifi_dict_to
+00004cf0: 5f64 6963 7428 636c 732c 2064 6174 613a  _dict(cls, data:
+00004d00: 2064 6963 745b 7374 722c 2041 6e79 5d29   dict[str, Any])
+00004d10: 202d 3e20 6469 6374 5b73 7472 2c20 416e   -> dict[str, An
+00004d20: 795d 3a0a 2020 2020 2020 2020 6966 2022  y]:.        if "
+00004d30: 7374 6f72 6167 6522 2069 6e20 6461 7461  storage" in data
+00004d40: 2061 6e64 2064 6174 615b 2273 746f 7261   and data["stora
+00004d50: 6765 225d 203d 3d20 7b7d 3a0a 2020 2020  ge"] == {}:.    
+00004d60: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
+00004d70: 5b22 7374 6f72 6167 6522 5d0a 0a20 2020  ["storage"]..   
+00004d80: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00004d90: 7228 292e 756e 6966 695f 6469 6374 5f74  r().unifi_dict_t
+00004da0: 6f5f 6469 6374 2864 6174 6129 0a0a 2020  o_dict(data)..  
+00004db0: 2020 6465 6620 756e 6966 695f 6469 6374    def unifi_dict
+00004dc0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00004dd0: 2020 2020 2020 2020 6461 7461 3a20 4f70          data: Op
+00004de0: 7469 6f6e 616c 5b64 6963 745b 7374 722c  tional[dict[str,
+00004df0: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
+00004e00: 2020 2020 2020 2065 7863 6c75 6465 3a20         exclude: 
+00004e10: 4f70 7469 6f6e 616c 5b73 6574 5b73 7472  Optional[set[str
+00004e20: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
+00004e30: 202d 3e20 6469 6374 5b73 7472 2c20 416e   -> dict[str, An
+00004e40: 795d 3a0a 2020 2020 2020 2020 6461 7461  y]:.        data
+00004e50: 203d 2073 7570 6572 2829 2e75 6e69 6669   = super().unifi
+00004e60: 5f64 6963 7428 6461 7461 3d64 6174 612c  _dict(data=data,
+00004e70: 2065 7863 6c75 6465 3d65 7863 6c75 6465   exclude=exclude
+00004e80: 290a 0a20 2020 2020 2020 2069 6620 2273  )..        if "s
+00004e90: 746f 7261 6765 2220 696e 2064 6174 6120  torage" in data 
+00004ea0: 616e 6420 6461 7461 5b22 7374 6f72 6167  and data["storag
+00004eb0: 6522 5d20 6973 204e 6f6e 653a 0a20 2020  e"] is None:.   
+00004ec0: 2020 2020 2020 2020 2064 6174 615b 2273           data["s
+00004ed0: 746f 7261 6765 225d 203d 207b 7d0a 0a20  torage"] = {}.. 
+00004ee0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+00004ef0: 7461 0a0a 0a63 6c61 7373 2043 616d 6572  ta...class Camer
+00004f00: 615a 6f6e 6528 5072 6f74 6563 7442 6173  aZone(ProtectBas
+00004f10: 654f 626a 6563 7429 3a0a 2020 2020 6964  eObject):.    id
+00004f20: 3a20 696e 740a 2020 2020 6e61 6d65 3a20  : int.    name: 
+00004f30: 7374 720a 2020 2020 636f 6c6f 723a 2043  str.    color: C
+00004f40: 6f6c 6f72 0a20 2020 2070 6f69 6e74 733a  olor.    points:
+00004f50: 206c 6973 745b 7475 706c 655b 5065 7263   list[tuple[Perc
+00004f60: 656e 742c 2050 6572 6365 6e74 5d5d 0a0a  ent, Percent]]..
+00004f70: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00004f80: 0a20 2020 2064 6566 2075 6e69 6669 5f64  .    def unifi_d
+00004f90: 6963 745f 746f 5f64 6963 7428 636c 732c  ict_to_dict(cls,
+00004fa0: 2064 6174 613a 2064 6963 745b 7374 722c   data: dict[str,
+00004fb0: 2041 6e79 5d29 202d 3e20 6469 6374 5b73   Any]) -> dict[s
+00004fc0: 7472 2c20 416e 795d 3a0a 2020 2020 2020  tr, Any]:.      
+00004fd0: 2020 6461 7461 203d 2073 7570 6572 2829    data = super()
+00004fe0: 2e75 6e69 6669 5f64 6963 745f 746f 5f64  .unifi_dict_to_d
+00004ff0: 6963 7428 6461 7461 290a 2020 2020 2020  ict(data).      
+00005000: 2020 6966 2022 706f 696e 7473 2220 696e    if "points" in
+00005010: 2064 6174 6120 616e 6420 6973 696e 7374   data and isinst
+00005020: 616e 6365 2864 6174 615b 2270 6f69 6e74  ance(data["point
+00005030: 7322 5d2c 2049 7465 7261 626c 6529 3a0a  s"], Iterable):.
+00005040: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00005050: 5b22 706f 696e 7473 225d 203d 205b 2870  ["points"] = [(p
+00005060: 5b30 5d2c 2070 5b31 5d29 2066 6f72 2070  [0], p[1]) for p
+00005070: 2069 6e20 6461 7461 5b22 706f 696e 7473   in data["points
+00005080: 225d 5d0a 0a20 2020 2020 2020 2072 6574  "]]..        ret
+00005090: 7572 6e20 6461 7461 0a0a 2020 2020 6465  urn data..    de
+000050a0: 6620 756e 6966 695f 6469 6374 280a 2020  f unifi_dict(.  
+000050b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000050c0: 2020 2020 6461 7461 3a20 4f70 7469 6f6e      data: Option
+000050d0: 616c 5b64 6963 745b 7374 722c 2041 6e79  al[dict[str, Any
+000050e0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+000050f0: 2020 2065 7863 6c75 6465 3a20 4f70 7469     exclude: Opti
+00005100: 6f6e 616c 5b73 6574 5b73 7472 5d5d 203d  onal[set[str]] =
+00005110: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+00005120: 6469 6374 5b73 7472 2c20 416e 795d 3a0a  dict[str, Any]:.
+00005130: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+00005140: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
+00005150: 7428 6461 7461 3d64 6174 612c 2065 7863  t(data=data, exc
+00005160: 6c75 6465 3d65 7863 6c75 6465 290a 0a20  lude=exclude).. 
+00005170: 2020 2020 2020 2069 6620 2270 6f69 6e74         if "point
+00005180: 7322 2069 6e20 6461 7461 3a0a 2020 2020  s" in data:.    
+00005190: 2020 2020 2020 2020 6461 7461 5b22 706f          data["po
+000051a0: 696e 7473 225d 203d 205b 7365 7269 616c  ints"] = [serial
+000051b0: 697a 655f 706f 696e 7428 7029 2066 6f72  ize_point(p) for
+000051c0: 2070 2069 6e20 6461 7461 5b22 706f 696e   p in data["poin
+000051d0: 7473 225d 5d0a 0a20 2020 2020 2020 2072  ts"]]..        r
+000051e0: 6574 7572 6e20 6461 7461 0a0a 2020 2020  eturn data..    
+000051f0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00005200: 2020 6465 6620 6372 6561 7465 5f70 7269    def create_pri
+00005210: 7661 6379 5f7a 6f6e 6528 7a6f 6e65 5f69  vacy_zone(zone_i
+00005220: 643a 2069 6e74 2920 2d3e 2043 616d 6572  d: int) -> Camer
+00005230: 615a 6f6e 653a 0a20 2020 2020 2020 2072  aZone:.        r
+00005240: 6574 7572 6e20 4361 6d65 7261 5a6f 6e65  eturn CameraZone
+00005250: 280a 2020 2020 2020 2020 2020 2020 6964  (.            id
+00005260: 3d7a 6f6e 655f 6964 2c0a 2020 2020 2020  =zone_id,.      
+00005270: 2020 2020 2020 6e61 6d65 3d50 5249 5641        name=PRIVA
+00005280: 4359 5f5a 4f4e 455f 4e41 4d45 2c0a 2020  CY_ZONE_NAME,.  
+00005290: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+000052a0: 436f 6c6f 7228 2223 3835 4243 4543 2229  Color("#85BCEC")
+000052b0: 2c0a 2020 2020 2020 2020 2020 2020 706f  ,.            po
+000052c0: 696e 7473 3d5b 5b30 2c20 305d 2c20 5b31  ints=[[0, 0], [1
+000052d0: 2c20 305d 2c20 5b31 2c20 315d 2c20 5b30  , 0], [1, 1], [0
+000052e0: 2c20 315d 5d2c 2020 2320 7479 7065 3a20  , 1]],  # type: 
+000052f0: 6967 6e6f 7265 5b6c 6973 742d 6974 656d  ignore[list-item
+00005300: 5d0a 2020 2020 2020 2020 290a 0a0a 636c  ].        )...cl
+00005310: 6173 7320 4d6f 7469 6f6e 5a6f 6e65 2843  ass MotionZone(C
+00005320: 616d 6572 615a 6f6e 6529 3a0a 2020 2020  ameraZone):.    
+00005330: 7365 6e73 6974 6976 6974 793a 2050 6572  sensitivity: Per
+00005340: 6365 6e74 496e 740a 0a0a 636c 6173 7320  centInt...class 
+00005350: 536d 6172 744d 6f74 696f 6e5a 6f6e 6528  SmartMotionZone(
+00005360: 4d6f 7469 6f6e 5a6f 6e65 293a 0a20 2020  MotionZone):.   
+00005370: 206f 626a 6563 745f 7479 7065 733a 206c   object_types: l
+00005380: 6973 745b 536d 6172 7444 6574 6563 744f  ist[SmartDetectO
+00005390: 626a 6563 7454 7970 655d 0a0a 2020 2020  bjectType]..    
+000053a0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+000053b0: 2064 6566 2075 6e69 6669 5f64 6963 745f   def unifi_dict_
+000053c0: 746f 5f64 6963 7428 636c 732c 2064 6174  to_dict(cls, dat
+000053d0: 613a 2064 6963 745b 7374 722c 2041 6e79  a: dict[str, Any
+000053e0: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
+000053f0: 416e 795d 3a0a 2020 2020 2020 2020 6966  Any]:.        if
+00005400: 2022 6f62 6a65 6374 5479 7065 7322 2069   "objectTypes" i
+00005410: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
+00005420: 2020 2020 6461 7461 5b22 6f62 6a65 6374      data["object
+00005430: 5479 7065 7322 5d20 3d20 636f 6e76 6572  Types"] = conver
+00005440: 745f 736d 6172 745f 7479 7065 7328 6461  t_smart_types(da
+00005450: 7461 2e70 6f70 2822 6f62 6a65 6374 5479  ta.pop("objectTy
+00005460: 7065 7322 2929 0a0a 2020 2020 2020 2020  pes"))..        
+00005470: 7265 7475 726e 2073 7570 6572 2829 2e75  return super().u
+00005480: 6e69 6669 5f64 6963 745f 746f 5f64 6963  nifi_dict_to_dic
+00005490: 7428 6461 7461 290a 0a0a 636c 6173 7320  t(data)...class 
+000054a0: 5072 6976 6163 794d 6173 6b43 6170 6162  PrivacyMaskCapab
+000054b0: 696c 6974 7928 5072 6f74 6563 7442 6173  ility(ProtectBas
+000054c0: 654f 626a 6563 7429 3a0a 2020 2020 6d61  eObject):.    ma
+000054d0: 785f 6d61 736b 733a 204f 7074 696f 6e61  x_masks: Optiona
+000054e0: 6c5b 696e 745d 0a20 2020 2072 6563 7461  l[int].    recta
+000054f0: 6e67 6c65 5f6f 6e6c 793a 2062 6f6f 6c0a  ngle_only: bool.
+00005500: 0a0a 636c 6173 7320 486f 7470 6c75 6745  ..class HotplugE
+00005510: 7874 656e 6465 7228 5072 6f74 6563 7442  xtender(ProtectB
+00005520: 6173 654f 626a 6563 7429 3a0a 2020 2020  aseObject):.    
+00005530: 6861 735f 666c 6173 683a 204f 7074 696f  has_flash: Optio
+00005540: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00005550: 0a20 2020 2068 6173 5f69 723a 204f 7074  .    has_ir: Opt
+00005560: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00005570: 6e65 0a20 2020 2068 6173 5f72 6164 6172  ne.    has_radar
+00005580: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00005590: 203d 204e 6f6e 650a 2020 2020 6973 5f61   = None.    is_a
+000055a0: 7474 6163 6865 643a 204f 7074 696f 6e61  ttached: Optiona
+000055b0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a20  l[bool] = None. 
+000055c0: 2020 2023 2033 2e30 2e32 322b 0a20 2020     # 3.0.22+.   
+000055d0: 2066 6c61 7368 5f72 616e 6765 3a20 4f70   flash_range: Op
+000055e0: 7469 6f6e 616c 5b41 6e79 5d20 3d20 4e6f  tional[Any] = No
+000055f0: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
+00005600: 7468 6f64 0a20 2020 2040 6361 6368 650a  thod.    @cache.
+00005610: 2020 2020 6465 6620 5f67 6574 5f75 6e69      def _get_uni
+00005620: 6669 5f72 656d 6170 7328 636c 7329 202d  fi_remaps(cls) -
+00005630: 3e20 6469 6374 5b73 7472 2c20 7374 725d  > dict[str, str]
+00005640: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00005650: 207b 2a2a 7375 7065 7228 292e 5f67 6574   {**super()._get
+00005660: 5f75 6e69 6669 5f72 656d 6170 7328 292c  _unifi_remaps(),
+00005670: 2022 6861 7349 5222 3a20 2268 6173 4972   "hasIR": "hasIr
+00005680: 227d 0a0a 0a63 6c61 7373 2048 6f74 706c  "}...class Hotpl
+00005690: 7567 2850 726f 7465 6374 4261 7365 4f62  ug(ProtectBaseOb
+000056a0: 6a65 6374 293a 0a20 2020 2061 7564 696f  ject):.    audio
+000056b0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+000056c0: 203d 204e 6f6e 650a 2020 2020 7669 6465   = None.    vide
+000056d0: 6f3a 204f 7074 696f 6e61 6c5b 626f 6f6c  o: Optional[bool
+000056e0: 5d20 3d20 4e6f 6e65 0a20 2020 2065 7874  ] = None.    ext
+000056f0: 656e 6465 723a 204f 7074 696f 6e61 6c5b  ender: Optional[
+00005700: 486f 7470 6c75 6745 7874 656e 6465 725d  HotplugExtender]
+00005710: 203d 204e 6f6e 650a 2020 2020 2320 322e   = None.    # 2.
+00005720: 382e 3335 2b0a 2020 2020 7374 616e 6461  8.35+.    standa
+00005730: 6c6f 6e65 5f61 646f 7074 696f 6e3a 204f  lone_adoption: O
+00005740: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00005750: 4e6f 6e65 0a0a 0a63 6c61 7373 2050 545a  None...class PTZ
+00005760: 5261 6e67 6553 696e 676c 6528 5072 6f74  RangeSingle(Prot
+00005770: 6563 7442 6173 654f 626a 6563 7429 3a0a  ectBaseObject):.
+00005780: 2020 2020 6d61 783a 204f 7074 696f 6e61      max: Optiona
+00005790: 6c5b 666c 6f61 745d 0a20 2020 206d 696e  l[float].    min
+000057a0: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+000057b0: 5d0a 2020 2020 7374 6570 3a20 4f70 7469  ].    step: Opti
+000057c0: 6f6e 616c 5b66 6c6f 6174 5d0a 0a0a 636c  onal[float]...cl
+000057d0: 6173 7320 5054 5a52 616e 6765 2850 726f  ass PTZRange(Pro
+000057e0: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
+000057f0: 0a20 2020 2073 7465 7073 3a20 5054 5a52  .    steps: PTZR
+00005800: 616e 6765 5369 6e67 6c65 0a20 2020 2064  angeSingle.    d
+00005810: 6567 7265 6573 3a20 5054 5a52 616e 6765  egrees: PTZRange
+00005820: 5369 6e67 6c65 0a0a 2020 2020 6465 6620  Single..    def 
+00005830: 746f 5f6e 6174 6976 655f 7661 6c75 6528  to_native_value(
+00005840: 7365 6c66 2c20 6465 6772 6565 5f76 616c  self, degree_val
+00005850: 7565 3a20 666c 6f61 742c 2069 735f 7265  ue: float, is_re
+00005860: 6c61 7469 7665 3a20 626f 6f6c 203d 2046  lative: bool = F
+00005870: 616c 7365 2920 2d3e 2066 6c6f 6174 3a0a  alse) -> float:.
+00005880: 2020 2020 2020 2020 2222 2243 6f6e 7665          """Conve
+00005890: 7274 2064 6567 7265 6520 7661 6c75 6573  rt degree values
+000058a0: 2074 6f20 7374 6570 2076 616c 7565 732e   to step values.
+000058b0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+000058c0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+000058d0: 6c66 2e64 6567 7265 6573 2e6d 6178 2069  lf.degrees.max i
+000058e0: 7320 4e6f 6e65 2020 2320 6e6f 7161 3a20  s None  # noqa: 
+000058f0: 504c 5230 3931 360a 2020 2020 2020 2020  PLR0916.        
+00005900: 2020 2020 6f72 2073 656c 662e 6465 6772      or self.degr
+00005910: 6565 732e 6d69 6e20 6973 204e 6f6e 650a  ees.min is None.
+00005920: 2020 2020 2020 2020 2020 2020 6f72 2073              or s
+00005930: 656c 662e 6465 6772 6565 732e 7374 6570  elf.degrees.step
+00005940: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
+00005950: 2020 2020 206f 7220 7365 6c66 2e73 7465       or self.ste
+00005960: 7073 2e6d 6178 2069 7320 4e6f 6e65 0a20  ps.max is None. 
+00005970: 2020 2020 2020 2020 2020 206f 7220 7365             or se
+00005980: 6c66 2e73 7465 7073 2e6d 696e 2069 7320  lf.steps.min is 
+00005990: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+000059a0: 206f 7220 7365 6c66 2e73 7465 7073 2e73   or self.steps.s
+000059b0: 7465 7020 6973 204e 6f6e 650a 2020 2020  tep is None.    
+000059c0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000059d0: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+000059e0: 6573 7428 2264 6567 7265 6520 746f 2073  est("degree to s
+000059f0: 7465 7020 636f 6e76 6572 7369 6f6e 206e  tep conversion n
+00005a00: 6f74 2073 7570 706f 7274 6564 2e22 290a  ot supported.").
+00005a10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00005a20: 6973 5f72 656c 6174 6976 653a 0a20 2020  is_relative:.   
+00005a30: 2020 2020 2020 2020 2064 6567 7265 655f           degree_
+00005a40: 7661 6c75 6520 2d3d 2073 656c 662e 6465  value -= self.de
+00005a50: 6772 6565 732e 6d69 6e0a 0a20 2020 2020  grees.min..     
+00005a60: 2020 2073 7465 705f 7261 6e67 6520 3d20     step_range = 
+00005a70: 7365 6c66 2e73 7465 7073 2e6d 6178 202d  self.steps.max -
+00005a80: 2073 656c 662e 7374 6570 732e 6d69 6e0a   self.steps.min.
+00005a90: 2020 2020 2020 2020 6465 6772 6565 5f72          degree_r
+00005aa0: 616e 6765 203d 2073 656c 662e 6465 6772  ange = self.degr
+00005ab0: 6565 732e 6d61 7820 2d20 7365 6c66 2e64  ees.max - self.d
+00005ac0: 6567 7265 6573 2e6d 696e 0a20 2020 2020  egrees.min.     
+00005ad0: 2020 2072 6174 696f 203d 2073 7465 705f     ratio = step_
+00005ae0: 7261 6e67 6520 2f20 6465 6772 6565 5f72  range / degree_r
+00005af0: 616e 6765 0a0a 2020 2020 2020 2020 7374  ange..        st
+00005b00: 6570 5f76 616c 7565 203d 2063 6c61 6d70  ep_value = clamp
+00005b10: 5f76 616c 7565 2864 6567 7265 655f 7661  _value(degree_va
+00005b20: 6c75 6520 2a20 7261 7469 6f2c 2073 656c  lue * ratio, sel
+00005b30: 662e 7374 6570 732e 7374 6570 290a 2020  f.steps.step).  
+00005b40: 2020 2020 2020 6966 206e 6f74 2069 735f        if not is_
+00005b50: 7265 6c61 7469 7665 3a0a 2020 2020 2020  relative:.      
+00005b60: 2020 2020 2020 7374 6570 5f76 616c 7565        step_value
+00005b70: 203d 2073 656c 662e 7374 6570 732e 6d69   = self.steps.mi
+00005b80: 6e20 2b20 7374 6570 5f76 616c 7565 0a0a  n + step_value..
+00005b90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005ba0: 7465 705f 7661 6c75 650a 0a0a 636c 6173  tep_value...clas
+00005bb0: 7320 5054 5a5a 6f6f 6d52 616e 6765 2850  s PTZZoomRange(P
+00005bc0: 545a 5261 6e67 6529 3a0a 2020 2020 7261  TZRange):.    ra
+00005bd0: 7469 6f3a 2066 6c6f 6174 0a0a 2020 2020  tio: float..    
+00005be0: 6465 6620 746f 5f6e 6174 6976 655f 7661  def to_native_va
+00005bf0: 6c75 6528 7365 6c66 2c20 7a6f 6f6d 5f76  lue(self, zoom_v
+00005c00: 616c 7565 3a20 666c 6f61 742c 2069 735f  alue: float, is_
+00005c10: 7265 6c61 7469 7665 3a20 626f 6f6c 203d  relative: bool =
+00005c20: 2046 616c 7365 2920 2d3e 2066 6c6f 6174   False) -> float
+00005c30: 3a0a 2020 2020 2020 2020 2222 2243 6f6e  :.        """Con
+00005c40: 7665 7274 207a 6f6f 6d20 7661 6c75 6573  vert zoom values
+00005c50: 2074 6f20 7374 6570 2076 616c 7565 732e   to step values.
+00005c60: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00005c70: 7365 6c66 2e73 7465 7073 2e6d 6178 2069  self.steps.max i
+00005c80: 7320 4e6f 6e65 206f 7220 7365 6c66 2e73  s None or self.s
+00005c90: 7465 7073 2e6d 696e 2069 7320 4e6f 6e65  teps.min is None
+00005ca0: 206f 7220 7365 6c66 2e73 7465 7073 2e73   or self.steps.s
+00005cb0: 7465 7020 6973 204e 6f6e 653a 0a20 2020  tep is None:.   
+00005cc0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+00005cd0: 6164 5265 7175 6573 7428 2273 7465 7020  adRequest("step 
+00005ce0: 636f 6e76 6572 7369 6f6e 206e 6f74 2073  conversion not s
+00005cf0: 7570 706f 7274 6564 2e22 290a 0a20 2020  upported.")..   
+00005d00: 2020 2020 2073 7465 705f 7261 6e67 6520       step_range 
+00005d10: 3d20 7365 6c66 2e73 7465 7073 2e6d 6178  = self.steps.max
+00005d20: 202d 2073 656c 662e 7374 6570 732e 6d69   - self.steps.mi
+00005d30: 6e0a 2020 2020 2020 2020 2320 7a6f 6f6d  n.        # zoom
+00005d40: 206c 6576 656c 7320 7374 6172 7420 6174   levels start at
+00005d50: 2031 0a20 2020 2020 2020 2072 6174 696f   1.        ratio
+00005d60: 203d 2073 7465 705f 7261 6e67 6520 2f20   = step_range / 
+00005d70: 2873 656c 662e 7261 7469 6f20 2d20 3129  (self.ratio - 1)
+00005d80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00005d90: 6973 5f72 656c 6174 6976 653a 0a20 2020  is_relative:.   
+00005da0: 2020 2020 2020 2020 207a 6f6f 6d5f 7661           zoom_va
+00005db0: 6c75 6520 2d3d 2031 0a0a 2020 2020 2020  lue -= 1..      
+00005dc0: 2020 7374 6570 5f76 616c 7565 203d 2063    step_value = c
+00005dd0: 6c61 6d70 5f76 616c 7565 287a 6f6f 6d5f  lamp_value(zoom_
+00005de0: 7661 6c75 6520 2a20 7261 7469 6f2c 2073  value * ratio, s
+00005df0: 656c 662e 7374 6570 732e 7374 6570 290a  elf.steps.step).
+00005e00: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00005e10: 735f 7265 6c61 7469 7665 3a0a 2020 2020  s_relative:.    
+00005e20: 2020 2020 2020 2020 7374 6570 5f76 616c          step_val
+00005e30: 7565 203d 2073 656c 662e 7374 6570 732e  ue = self.steps.
+00005e40: 6d69 6e20 2b20 7374 6570 5f76 616c 7565  min + step_value
+00005e50: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005e60: 2073 7465 705f 7661 6c75 650a 0a0a 636c   step_value...cl
+00005e70: 6173 7320 4361 6d65 7261 4665 6174 7572  ass CameraFeatur
+00005e80: 6546 6c61 6773 2850 726f 7465 6374 4261  eFlags(ProtectBa
+00005e90: 7365 4f62 6a65 6374 293a 0a20 2020 2063  seObject):.    c
+00005ea0: 616e 5f61 646a 7573 745f 6972 5f6c 6564  an_adjust_ir_led
+00005eb0: 5f6c 6576 656c 3a20 626f 6f6c 0a20 2020  _level: bool.   
+00005ec0: 2063 616e 5f6d 6167 6963 5f7a 6f6f 6d3a   can_magic_zoom:
+00005ed0: 2062 6f6f 6c0a 2020 2020 6361 6e5f 6f70   bool.    can_op
+00005ee0: 7469 6361 6c5f 7a6f 6f6d 3a20 626f 6f6c  tical_zoom: bool
+00005ef0: 0a20 2020 2063 616e 5f74 6f75 6368 5f66  .    can_touch_f
+00005f00: 6f63 7573 3a20 626f 6f6c 0a20 2020 2068  ocus: bool.    h
+00005f10: 6173 5f61 6363 656c 6572 6f6d 6574 6572  as_accelerometer
+00005f20: 3a20 626f 6f6c 0a20 2020 2068 6173 5f61  : bool.    has_a
+00005f30: 6563 3a20 626f 6f6c 0a20 2020 2068 6173  ec: bool.    has
+00005f40: 5f62 6c75 6574 6f6f 7468 3a20 626f 6f6c  _bluetooth: bool
+00005f50: 0a20 2020 2068 6173 5f63 6869 6d65 3a20  .    has_chime: 
+00005f60: 626f 6f6c 0a20 2020 2068 6173 5f65 7874  bool.    has_ext
+00005f70: 6572 6e61 6c5f 6972 3a20 626f 6f6c 0a20  ernal_ir: bool. 
+00005f80: 2020 2068 6173 5f69 6372 5f73 656e 7369     has_icr_sensi
+00005f90: 7469 7669 7479 3a20 626f 6f6c 0a20 2020  tivity: bool.   
+00005fa0: 2068 6173 5f6c 6463 3a20 626f 6f6c 0a20   has_ldc: bool. 
+00005fb0: 2020 2068 6173 5f6c 6564 5f69 723a 2062     has_led_ir: b
+00005fc0: 6f6f 6c0a 2020 2020 6861 735f 6c65 645f  ool.    has_led_
+00005fd0: 7374 6174 7573 3a20 626f 6f6c 0a20 2020  status: bool.   
+00005fe0: 2068 6173 5f6c 696e 655f 696e 3a20 626f   has_line_in: bo
+00005ff0: 6f6c 0a20 2020 2068 6173 5f6d 6963 3a20  ol.    has_mic: 
+00006000: 626f 6f6c 0a20 2020 2068 6173 5f70 7269  bool.    has_pri
+00006010: 7661 6379 5f6d 6173 6b3a 2062 6f6f 6c0a  vacy_mask: bool.
+00006020: 2020 2020 6861 735f 7274 633a 2062 6f6f      has_rtc: boo
+00006030: 6c0a 2020 2020 6861 735f 7364 5f63 6172  l.    has_sd_car
+00006040: 643a 2062 6f6f 6c0a 2020 2020 6861 735f  d: bool.    has_
+00006050: 7370 6561 6b65 723a 2062 6f6f 6c0a 2020  speaker: bool.  
+00006060: 2020 6861 735f 7769 6669 3a20 626f 6f6c    has_wifi: bool
+00006070: 0a20 2020 2068 6173 5f68 6472 3a20 626f  .    has_hdr: bo
+00006080: 6f6c 0a20 2020 2068 6173 5f61 7574 6f5f  ol.    has_auto_
+00006090: 6963 725f 6f6e 6c79 3a20 626f 6f6c 0a20  icr_only: bool. 
+000060a0: 2020 2076 6964 656f 5f6d 6f64 6573 3a20     video_modes: 
+000060b0: 6c69 7374 5b56 6964 656f 4d6f 6465 5d0a  list[VideoMode].
+000060c0: 2020 2020 7669 6465 6f5f 6d6f 6465 5f6d      video_mode_m
+000060d0: 6178 5f66 7073 3a20 6c69 7374 5b69 6e74  ax_fps: list[int
+000060e0: 5d0a 2020 2020 6861 735f 6d6f 7469 6f6e  ].    has_motion
+000060f0: 5f7a 6f6e 6573 3a20 626f 6f6c 0a20 2020  _zones: bool.   
+00006100: 2068 6173 5f6c 6364 5f73 6372 6565 6e3a   has_lcd_screen:
+00006110: 2062 6f6f 6c0a 2020 2020 736d 6172 745f   bool.    smart_
+00006120: 6465 7465 6374 5f74 7970 6573 3a20 6c69  detect_types: li
+00006130: 7374 5b53 6d61 7274 4465 7465 6374 4f62  st[SmartDetectOb
+00006140: 6a65 6374 5479 7065 5d0a 2020 2020 6d6f  jectType].    mo
+00006150: 7469 6f6e 5f61 6c67 6f72 6974 686d 733a  tion_algorithms:
+00006160: 206c 6973 745b 4d6f 7469 6f6e 416c 676f   list[MotionAlgo
+00006170: 7269 7468 6d5d 0a20 2020 2068 6173 5f73  rithm].    has_s
+00006180: 7175 6172 655f 6576 656e 745f 7468 756d  quare_event_thum
+00006190: 626e 6169 6c3a 2062 6f6f 6c0a 2020 2020  bnail: bool.    
+000061a0: 6861 735f 7061 636b 6167 655f 6361 6d65  has_package_came
+000061b0: 7261 3a20 626f 6f6c 0a20 2020 2070 7269  ra: bool.    pri
+000061c0: 7661 6379 5f6d 6173 6b5f 6361 7061 6269  vacy_mask_capabi
+000061d0: 6c69 7479 3a20 5072 6976 6163 794d 6173  lity: PrivacyMas
+000061e0: 6b43 6170 6162 696c 6974 790a 2020 2020  kCapability.    
+000061f0: 6861 735f 736d 6172 745f 6465 7465 6374  has_smart_detect
+00006200: 3a20 626f 6f6c 0a20 2020 2061 7564 696f  : bool.    audio
+00006210: 3a20 6c69 7374 5b73 7472 5d20 3d20 5b5d  : list[str] = []
+00006220: 0a20 2020 2061 7564 696f 5f63 6f64 6563  .    audio_codec
+00006230: 733a 206c 6973 745b 4175 6469 6f43 6f64  s: list[AudioCod
+00006240: 6563 735d 203d 205b 5d0a 2020 2020 6d6f  ecs] = [].    mo
+00006250: 756e 745f 706f 7369 7469 6f6e 733a 206c  unt_positions: l
+00006260: 6973 745b 4d6f 756e 7450 6f73 6974 696f  ist[MountPositio
+00006270: 6e5d 203d 205b 5d0a 2020 2020 6861 735f  n] = [].    has_
+00006280: 696e 6672 6172 6564 3a20 4f70 7469 6f6e  infrared: Option
+00006290: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+000062a0: 2020 2020 6c65 6e73 5f74 7970 653a 204f      lens_type: O
+000062b0: 7074 696f 6e61 6c5b 4c65 6e73 5479 7065  ptional[LensType
+000062c0: 5d20 3d20 4e6f 6e65 0a20 2020 2068 6f74  ] = None.    hot
+000062d0: 706c 7567 3a20 4f70 7469 6f6e 616c 5b48  plug: Optional[H
+000062e0: 6f74 706c 7567 5d20 3d20 4e6f 6e65 0a20  otplug] = None. 
+000062f0: 2020 2073 6d61 7274 5f64 6574 6563 745f     smart_detect_
+00006300: 6175 6469 6f5f 7479 7065 733a 204f 7074  audio_types: Opt
+00006310: 696f 6e61 6c5b 6c69 7374 5b53 6d61 7274  ional[list[Smart
+00006320: 4465 7465 6374 4175 6469 6f54 7970 655d  DetectAudioType]
+00006330: 5d20 3d20 4e6f 6e65 0a20 2020 2023 2032  ] = None.    # 2
+00006340: 2e37 2e31 382b 0a20 2020 2069 735f 646f  .7.18+.    is_do
+00006350: 6f72 6265 6c6c 3a20 626f 6f6c 0a20 2020  orbell: bool.   
+00006360: 2023 2032 2e38 2e32 322b 0a20 2020 206c   # 2.8.22+.    l
+00006370: 656e 735f 6d6f 6465 6c3a 204f 7074 696f  ens_model: Optio
+00006380: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00006390: 2020 2020 2320 322e 392e 3230 2b0a 2020      # 2.9.20+.  
+000063a0: 2020 6861 735f 636f 6c6f 725f 6c63 645f    has_color_lcd_
+000063b0: 7363 7265 656e 3a20 4f70 7469 6f6e 616c  screen: Optional
+000063c0: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 2020  [bool] = None.  
+000063d0: 2020 6861 735f 6c69 6e65 5f63 726f 7373    has_line_cross
+000063e0: 696e 673a 204f 7074 696f 6e61 6c5b 626f  ing: Optional[bo
+000063f0: 6f6c 5d20 3d20 4e6f 6e65 0a20 2020 2068  ol] = None.    h
+00006400: 6173 5f6c 696e 655f 6372 6f73 7369 6e67  as_line_crossing
+00006410: 5f63 6f75 6e74 696e 673a 204f 7074 696f  _counting: Optio
+00006420: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00006430: 0a20 2020 2068 6173 5f6c 6976 6576 6965  .    has_livevie
+00006440: 775f 7472 6163 6b69 6e67 3a20 4f70 7469  w_tracking: Opti
+00006450: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00006460: 650a 2020 2020 2320 322e 3130 2e31 302b  e.    # 2.10.10+
+00006470: 0a20 2020 2068 6173 5f66 6c61 7368 3a20  .    has_flash: 
+00006480: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00006490: 204e 6f6e 650a 2020 2020 6973 5f70 747a   None.    is_ptz
+000064a0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+000064b0: 203d 204e 6f6e 650a 2020 2020 2320 322e   = None.    # 2.
+000064c0: 3131 2e31 332b 0a20 2020 2061 7564 696f  11.13+.    audio
+000064d0: 5f73 7479 6c65 3a20 4f70 7469 6f6e 616c  _style: Optional
+000064e0: 5b6c 6973 745b 4175 6469 6f53 7479 6c65  [list[AudioStyle
+000064f0: 5d5d 203d 204e 6f6e 650a 2020 2020 6861  ]] = None.    ha
+00006500: 735f 7665 7274 6963 616c 5f66 6c69 703a  s_vertical_flip:
+00006510: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00006520: 3d20 4e6f 6e65 0a20 2020 2023 2033 2e30  = None.    # 3.0
+00006530: 2e32 322b 0a20 2020 2066 6c61 7368 5f72  .22+.    flash_r
+00006540: 616e 6765 3a20 4f70 7469 6f6e 616c 5b41  ange: Optional[A
+00006550: 6e79 5d20 3d20 4e6f 6e65 0a0a 2020 2020  ny] = None..    
+00006560: 666f 6375 733a 2050 545a 5261 6e67 650a  focus: PTZRange.
+00006570: 2020 2020 7061 6e3a 2050 545a 5261 6e67      pan: PTZRang
+00006580: 650a 2020 2020 7469 6c74 3a20 5054 5a52  e.    tilt: PTZR
+00006590: 616e 6765 0a20 2020 207a 6f6f 6d3a 2050  ange.    zoom: P
+000065a0: 545a 5a6f 6f6d 5261 6e67 650a 0a20 2020  TZZoomRange..   
+000065b0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+000065c0: 2020 6465 6620 756e 6966 695f 6469 6374    def unifi_dict
+000065d0: 5f74 6f5f 6469 6374 2863 6c73 2c20 6461  _to_dict(cls, da
+000065e0: 7461 3a20 6469 6374 5b73 7472 2c20 416e  ta: dict[str, An
+000065f0: 795d 2920 2d3e 2064 6963 745b 7374 722c  y]) -> dict[str,
+00006600: 2041 6e79 5d3a 0a20 2020 2020 2020 2069   Any]:.        i
+00006610: 6620 2273 6d61 7274 4465 7465 6374 5479  f "smartDetectTy
+00006620: 7065 7322 2069 6e20 6461 7461 3a0a 2020  pes" in data:.  
+00006630: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+00006640: 736d 6172 7444 6574 6563 7454 7970 6573  smartDetectTypes
+00006650: 225d 203d 2063 6f6e 7665 7274 5f73 6d61  "] = convert_sma
+00006660: 7274 5f74 7970 6573 2864 6174 612e 706f  rt_types(data.po
+00006670: 7028 2273 6d61 7274 4465 7465 6374 5479  p("smartDetectTy
+00006680: 7065 7322 2929 0a20 2020 2020 2020 2069  pes")).        i
+00006690: 6620 2273 6d61 7274 4465 7465 6374 4175  f "smartDetectAu
+000066a0: 6469 6f54 7970 6573 2220 696e 2064 6174  dioTypes" in dat
+000066b0: 613a 0a20 2020 2020 2020 2020 2020 2064  a:.            d
+000066c0: 6174 615b 2273 6d61 7274 4465 7465 6374  ata["smartDetect
+000066d0: 4175 6469 6f54 7970 6573 225d 203d 2063  AudioTypes"] = c
+000066e0: 6f6e 7665 7274 5f73 6d61 7274 5f61 7564  onvert_smart_aud
+000066f0: 696f 5f74 7970 6573 280a 2020 2020 2020  io_types(.      
+00006700: 2020 2020 2020 2020 2020 6461 7461 2e70            data.p
+00006710: 6f70 2822 736d 6172 7444 6574 6563 7441  op("smartDetectA
+00006720: 7564 696f 5479 7065 7322 292c 0a20 2020  udioTypes"),.   
+00006730: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00006740: 2020 2069 6620 2276 6964 656f 4d6f 6465     if "videoMode
+00006750: 7322 2069 6e20 6461 7461 3a0a 2020 2020  s" in data:.    
+00006760: 2020 2020 2020 2020 6461 7461 5b22 7669          data["vi
+00006770: 6465 6f4d 6f64 6573 225d 203d 2063 6f6e  deoModes"] = con
+00006780: 7665 7274 5f76 6964 656f 5f6d 6f64 6573  vert_video_modes
+00006790: 2864 6174 612e 706f 7028 2276 6964 656f  (data.pop("video
+000067a0: 4d6f 6465 7322 2929 0a0a 2020 2020 2020  Modes"))..      
+000067b0: 2020 2320 6261 636b 706f 7274 2073 7570    # backport sup
+000067c0: 706f 7274 2066 6f72 2060 6973 5f64 6f6f  port for `is_doo
+000067d0: 7262 656c 6c60 2074 6f20 6f6c 6465 7220  rbell` to older 
+000067e0: 7665 7273 696f 6e73 206f 6620 5072 6f74  versions of Prot
+000067f0: 6563 740a 2020 2020 2020 2020 6966 2022  ect.        if "
+00006800: 6861 7343 6869 6d65 2220 696e 2064 6174  hasChime" in dat
+00006810: 6120 616e 6420 2269 7344 6f6f 7262 656c  a and "isDoorbel
+00006820: 6c22 206e 6f74 2069 6e20 6461 7461 3a0a  l" not in data:.
+00006830: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00006840: 5b22 6973 446f 6f72 6265 6c6c 225d 203d  ["isDoorbell"] =
+00006850: 2064 6174 615b 2268 6173 4368 696d 6522   data["hasChime"
+00006860: 5d0a 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+00006870: 6e20 7375 7065 7228 292e 756e 6966 695f  n super().unifi_
+00006880: 6469 6374 5f74 6f5f 6469 6374 2864 6174  dict_to_dict(dat
+00006890: 6129 0a0a 2020 2020 4063 6c61 7373 6d65  a)..    @classme
+000068a0: 7468 6f64 0a20 2020 2040 6361 6368 650a  thod.    @cache.
+000068b0: 2020 2020 6465 6620 5f67 6574 5f75 6e69      def _get_uni
+000068c0: 6669 5f72 656d 6170 7328 636c 7329 202d  fi_remaps(cls) -
+000068d0: 3e20 6469 6374 5b73 7472 2c20 7374 725d  > dict[str, str]
+000068e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000068f0: 207b 2a2a 7375 7065 7228 292e 5f67 6574   {**super()._get
+00006900: 5f75 6e69 6669 5f72 656d 6170 7328 292c  _unifi_remaps(),
+00006910: 2022 6861 7341 7574 6f49 4352 4f6e 6c79   "hasAutoICROnly
+00006920: 223a 2022 6861 7341 7574 6f49 6372 4f6e  ": "hasAutoIcrOn
+00006930: 6c79 227d 0a0a 2020 2020 4070 726f 7065  ly"}..    @prope
+00006940: 7274 790a 2020 2020 6465 6620 6861 735f  rty.    def has_
+00006950: 6869 6768 6670 7328 7365 6c66 2920 2d3e  highfps(self) ->
+00006960: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
+00006970: 6574 7572 6e20 5669 6465 6f4d 6f64 652e  eturn VideoMode.
+00006980: 4849 4748 5f46 5053 2069 6e20 7365 6c66  HIGH_FPS in self
+00006990: 2e76 6964 656f 5f6d 6f64 6573 0a0a 2020  .video_modes..  
+000069a0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000069b0: 6465 6620 6861 735f 7764 7228 7365 6c66  def has_wdr(self
+000069c0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+000069d0: 2020 2072 6574 7572 6e20 6e6f 7420 7365     return not se
+000069e0: 6c66 2e68 6173 5f68 6472 0a0a 0a63 6c61  lf.has_hdr...cla
+000069f0: 7373 2043 616d 6572 614c 656e 7365 7328  ss CameraLenses(
+00006a00: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
+00006a10: 7429 3a0a 2020 2020 6964 3a20 696e 740a  t):.    id: int.
+00006a20: 2020 2020 7669 6465 6f3a 2056 6964 656f      video: Video
+00006a30: 5374 6174 730a 0a0a 636c 6173 7320 4361  Stats...class Ca
+00006a40: 6d65 7261 486f 6d65 6b69 7453 6574 7469  meraHomekitSetti
+00006a50: 6e67 7328 5072 6f74 6563 7442 6173 654f  ngs(ProtectBaseO
+00006a60: 626a 6563 7429 3a0a 2020 2020 6d69 6372  bject):.    micr
+00006a70: 6f70 686f 6e65 5f6d 7574 6564 3a20 626f  ophone_muted: bo
+00006a80: 6f6c 0a20 2020 2073 7065 616b 6572 5f6d  ol.    speaker_m
+00006a90: 7574 6564 3a20 626f 6f6c 0a20 2020 2073  uted: bool.    s
+00006aa0: 7472 6561 6d5f 696e 5f70 726f 6772 6573  tream_in_progres
+00006ab0: 733a 2062 6f6f 6c0a 2020 2020 7461 6c6b  s: bool.    talk
+00006ac0: 6261 636b 5f73 6574 7469 6e67 735f 6163  back_settings_ac
+00006ad0: 7469 7665 3a20 626f 6f6c 0a0a 0a63 6c61  tive: bool...cla
+00006ae0: 7373 2043 616d 6572 6141 7564 696f 5365  ss CameraAudioSe
+00006af0: 7474 696e 6773 2850 726f 7465 6374 4261  ttings(ProtectBa
+00006b00: 7365 4f62 6a65 6374 293a 0a20 2020 2073  seObject):.    s
+00006b10: 7479 6c65 3a20 6c69 7374 5b41 7564 696f  tyle: list[Audio
+00006b20: 5374 796c 655d 0a0a 0a63 6c61 7373 2043  Style]...class C
+00006b30: 616d 6572 6128 5072 6f74 6563 744d 6f74  amera(ProtectMot
+00006b40: 696f 6e44 6576 6963 654d 6f64 656c 293a  ionDeviceModel):
+00006b50: 0a20 2020 2069 735f 6465 6c65 7469 6e67  .    is_deleting
+00006b60: 3a20 626f 6f6c 0a20 2020 2023 204d 6963  : bool.    # Mic
+00006b70: 726f 7068 6f6e 6520 5365 6e73 6974 6976  rophone Sensitiv
+00006b80: 6974 790a 2020 2020 6d69 635f 766f 6c75  ity.    mic_volu
+00006b90: 6d65 3a20 5065 7263 656e 7449 6e74 0a20  me: PercentInt. 
+00006ba0: 2020 2069 735f 6d69 635f 656e 6162 6c65     is_mic_enable
+00006bb0: 643a 2062 6f6f 6c0a 2020 2020 6973 5f72  d: bool.    is_r
+00006bc0: 6563 6f72 6469 6e67 3a20 626f 6f6c 0a20  ecording: bool. 
+00006bd0: 2020 2069 735f 6d6f 7469 6f6e 5f64 6574     is_motion_det
+00006be0: 6563 7465 643a 2062 6f6f 6c0a 2020 2020  ected: bool.    
+00006bf0: 6973 5f73 6d61 7274 5f64 6574 6563 7465  is_smart_detecte
+00006c00: 643a 2062 6f6f 6c0a 2020 2020 7068 795f  d: bool.    phy_
+00006c10: 7261 7465 3a20 4f70 7469 6f6e 616c 5b66  rate: Optional[f
+00006c20: 6c6f 6174 5d0a 2020 2020 6864 725f 6d6f  loat].    hdr_mo
+00006c30: 6465 3a20 626f 6f6c 0a20 2020 2023 2052  de: bool.    # R
+00006c40: 6563 6f72 6469 6e67 2051 7561 6c69 7479  ecording Quality
+00006c50: 202d 3e20 4869 6768 2046 7261 6d65 0a20   -> High Frame. 
+00006c60: 2020 2076 6964 656f 5f6d 6f64 653a 2056     video_mode: V
+00006c70: 6964 656f 4d6f 6465 0a20 2020 2069 735f  ideoMode.    is_
+00006c80: 7072 6f62 696e 675f 666f 725f 7769 6669  probing_for_wifi
+00006c90: 3a20 626f 6f6c 0a20 2020 2063 6869 6d65  : bool.    chime
+00006ca0: 5f64 7572 6174 696f 6e3a 2074 696d 6564  _duration: timed
+00006cb0: 656c 7461 0a20 2020 206c 6173 745f 7269  elta.    last_ri
+00006cc0: 6e67 3a20 4f70 7469 6f6e 616c 5b64 6174  ng: Optional[dat
+00006cd0: 6574 696d 655d 0a20 2020 2069 735f 6c69  etime].    is_li
+00006ce0: 7665 5f68 6561 746d 6170 5f65 6e61 626c  ve_heatmap_enabl
+00006cf0: 6564 3a20 626f 6f6c 0a20 2020 2076 6964  ed: bool.    vid
+00006d00: 656f 5f72 6563 6f6e 6669 6775 7261 7469  eo_reconfigurati
+00006d10: 6f6e 5f69 6e5f 7072 6f67 7265 7373 3a20  on_in_progress: 
+00006d20: 626f 6f6c 0a20 2020 2063 6861 6e6e 656c  bool.    channel
+00006d30: 733a 206c 6973 745b 4361 6d65 7261 4368  s: list[CameraCh
+00006d40: 616e 6e65 6c5d 0a20 2020 2069 7370 5f73  annel].    isp_s
+00006d50: 6574 7469 6e67 733a 2049 5350 5365 7474  ettings: ISPSett
+00006d60: 696e 6773 0a20 2020 2074 616c 6b62 6163  ings.    talkbac
+00006d70: 6b5f 7365 7474 696e 6773 3a20 5461 6c6b  k_settings: Talk
+00006d80: 6261 636b 5365 7474 696e 6773 0a20 2020  backSettings.   
+00006d90: 206f 7364 5f73 6574 7469 6e67 733a 204f   osd_settings: O
+00006da0: 5344 5365 7474 696e 6773 0a20 2020 206c  SDSettings.    l
+00006db0: 6564 5f73 6574 7469 6e67 733a 204c 4544  ed_settings: LED
+00006dc0: 5365 7474 696e 6773 0a20 2020 2073 7065  Settings.    spe
+00006dd0: 616b 6572 5f73 6574 7469 6e67 733a 2053  aker_settings: S
+00006de0: 7065 616b 6572 5365 7474 696e 6773 0a20  peakerSettings. 
+00006df0: 2020 2072 6563 6f72 6469 6e67 5f73 6574     recording_set
+00006e00: 7469 6e67 733a 2052 6563 6f72 6469 6e67  tings: Recording
+00006e10: 5365 7474 696e 6773 0a20 2020 2073 6d61  Settings.    sma
+00006e20: 7274 5f64 6574 6563 745f 7365 7474 696e  rt_detect_settin
+00006e30: 6773 3a20 536d 6172 7444 6574 6563 7453  gs: SmartDetectS
+00006e40: 6574 7469 6e67 730a 2020 2020 6d6f 7469  ettings.    moti
+00006e50: 6f6e 5f7a 6f6e 6573 3a20 6c69 7374 5b4d  on_zones: list[M
+00006e60: 6f74 696f 6e5a 6f6e 655d 0a20 2020 2070  otionZone].    p
+00006e70: 7269 7661 6379 5f7a 6f6e 6573 3a20 6c69  rivacy_zones: li
+00006e80: 7374 5b43 616d 6572 615a 6f6e 655d 0a20  st[CameraZone]. 
+00006e90: 2020 2073 6d61 7274 5f64 6574 6563 745f     smart_detect_
+00006ea0: 7a6f 6e65 733a 206c 6973 745b 536d 6172  zones: list[Smar
+00006eb0: 744d 6f74 696f 6e5a 6f6e 655d 0a20 2020  tMotionZone].   
+00006ec0: 2073 7461 7473 3a20 4361 6d65 7261 5374   stats: CameraSt
+00006ed0: 6174 730a 2020 2020 6665 6174 7572 655f  ats.    feature_
+00006ee0: 666c 6167 733a 2043 616d 6572 6146 6561  flags: CameraFea
+00006ef0: 7475 7265 466c 6167 730a 2020 2020 6c63  tureFlags.    lc
+00006f00: 645f 6d65 7373 6167 653a 204f 7074 696f  d_message: Optio
+00006f10: 6e61 6c5b 4c43 444d 6573 7361 6765 5d0a  nal[LCDMessage].
+00006f20: 2020 2020 6c65 6e73 6573 3a20 6c69 7374      lenses: list
+00006f30: 5b43 616d 6572 614c 656e 7365 735d 0a20  [CameraLenses]. 
+00006f40: 2020 2070 6c61 7466 6f72 6d3a 2073 7472     platform: str
+00006f50: 0a20 2020 2068 6173 5f73 7065 616b 6572  .    has_speaker
+00006f60: 3a20 626f 6f6c 0a20 2020 2068 6173 5f77  : bool.    has_w
+00006f70: 6966 693a 2062 6f6f 6c0a 2020 2020 6175  ifi: bool.    au
+00006f80: 6469 6f5f 6269 7472 6174 653a 2069 6e74  dio_bitrate: int
+00006f90: 0a20 2020 2063 616e 5f6d 616e 6167 653a  .    can_manage:
+00006fa0: 2062 6f6f 6c0a 2020 2020 6973 5f6d 616e   bool.    is_man
+00006fb0: 6167 6564 3a20 626f 6f6c 0a20 2020 2076  aged: bool.    v
+00006fc0: 6f6c 7461 6765 3a20 4f70 7469 6f6e 616c  oltage: Optional
+00006fd0: 5b66 6c6f 6174 5d0a 2020 2020 2320 7265  [float].    # re
+00006fe0: 7175 6972 6573 2031 2e32 312b 0a20 2020  quires 1.21+.   
+00006ff0: 2069 735f 706f 6f72 5f6e 6574 776f 726b   is_poor_network
+00007000: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00007010: 0a20 2020 2069 735f 7769 7265 6c65 7373  .    is_wireless
+00007020: 5f75 706c 696e 6b5f 656e 6162 6c65 643a  _uplink_enabled:
+00007030: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0a   Optional[bool].
+00007040: 2020 2020 2320 7265 7175 6972 6573 2032      # requires 2
+00007050: 2e36 2e31 332b 0a20 2020 2068 6f6d 656b  .6.13+.    homek
+00007060: 6974 5f73 6574 7469 6e67 733a 204f 7074  it_settings: Opt
+00007070: 696f 6e61 6c5b 4361 6d65 7261 486f 6d65  ional[CameraHome
+00007080: 6b69 7453 6574 7469 6e67 735d 203d 204e  kitSettings] = N
+00007090: 6f6e 650a 2020 2020 2320 7265 7175 6972  one.    # requir
+000070a0: 6573 2032 2e36 2e31 372b 0a20 2020 2061  es 2.6.17+.    a
+000070b0: 705f 6d67 6d74 5f69 703a 204f 7074 696f  p_mgmt_ip: Optio
+000070c0: 6e61 6c5b 4950 7634 4164 6472 6573 735d  nal[IPv4Address]
+000070d0: 203d 204e 6f6e 650a 2020 2020 2320 7265   = None.    # re
+000070e0: 7175 6972 6573 2032 2e37 2e35 2b0a 2020  quires 2.7.5+.  
+000070f0: 2020 6973 5f77 6174 6572 7072 6f6f 665f    is_waterproof_
+00007100: 6361 7365 5f61 7474 6163 6865 643a 204f  case_attached: O
+00007110: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00007120: 4e6f 6e65 0a20 2020 206c 6173 745f 6469  None.    last_di
+00007130: 7363 6f6e 6e65 6374 3a20 4f70 7469 6f6e  sconnect: Option
+00007140: 616c 5b64 6174 6574 696d 655d 203d 204e  al[datetime] = N
+00007150: 6f6e 650a 2020 2020 2320 7265 7175 6972  one.    # requir
+00007160: 6573 2032 2e38 2e31 342b 0a20 2020 2069  es 2.8.14+.    i
+00007170: 735f 326b 3a20 4f70 7469 6f6e 616c 5b62  s_2k: Optional[b
+00007180: 6f6f 6c5d 203d 204e 6f6e 650a 2020 2020  ool] = None.    
+00007190: 6973 5f34 6b3a 204f 7074 696f 6e61 6c5b  is_4k: Optional[
+000071a0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a20 2020  bool] = None.   
+000071b0: 2075 7365 5f67 6c6f 6261 6c3a 204f 7074   use_global: Opt
+000071c0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+000071d0: 6e65 0a20 2020 2023 2072 6571 7569 7265  ne.    # require
+000071e0: 7320 322e 382e 3232 2b0a 2020 2020 7573  s 2.8.22+.    us
+000071f0: 6572 5f63 6f6e 6669 6775 7265 645f 6170  er_configured_ap
+00007200: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00007210: 203d 204e 6f6e 650a 2020 2020 2320 7265   = None.    # re
+00007220: 7175 6972 6573 2032 2e39 2e32 302b 0a20  quires 2.9.20+. 
+00007230: 2020 2068 6173 5f72 6563 6f72 6469 6e67     has_recording
+00007240: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
+00007250: 5d20 3d20 4e6f 6e65 0a20 2020 2023 2072  ] = None.    # r
+00007260: 6571 7569 7265 7320 322e 3130 2e31 302b  equires 2.10.10+
+00007270: 0a20 2020 2069 735f 7074 7a3a 204f 7074  .    is_ptz: Opt
+00007280: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00007290: 6e65 0a20 2020 2023 2072 6571 7569 7265  ne.    # require
+000072a0: 7320 322e 3131 2e31 332b 0a20 2020 2061  s 2.11.13+.    a
+000072b0: 7564 696f 5f73 6574 7469 6e67 733a 204f  udio_settings: O
+000072c0: 7074 696f 6e61 6c5b 4361 6d65 7261 4175  ptional[CameraAu
+000072d0: 6469 6f53 6574 7469 6e67 735d 203d 204e  dioSettings] = N
+000072e0: 6f6e 650a 0a20 2020 2023 2054 4f44 4f3a  one..    # TODO:
+000072f0: 2075 7365 6420 666f 7220 6164 6f70 7469   used for adopti
+00007300: 6e67 0a20 2020 2023 2061 704d 6163 2072  ng.    # apMac r
+00007310: 6561 6420 6f6e 6c79 0a20 2020 2023 2061  ead only.    # a
+00007320: 7052 7373 6920 7265 6164 206f 6e6c 790a  pRssi read only.
+00007330: 2020 2020 2320 656c 656d 656e 7449 6e66      # elementInf
+00007340: 6f20 7265 6164 206f 6e6c 790a 0a20 2020  o read only..   
+00007350: 2023 2054 4f44 4f3a 0a20 2020 2023 206c   # TODO:.    # l
+00007360: 6173 7450 7269 7661 6379 5a6f 6e65 506f  astPrivacyZonePo
+00007370: 7369 7469 6f6e 4964 0a20 2020 2023 2073  sitionId.    # s
+00007380: 6d61 7274 4465 7465 6374 4c69 6e65 730a  martDetectLines.
+00007390: 2020 2020 2320 7374 7265 616d 5368 6172      # streamShar
+000073a0: 696e 6720 7265 6164 206f 6e6c 790a 2020  ing read only.  
+000073b0: 2020 2320 7374 6f70 5374 7265 616d 4c65    # stopStreamLe
+000073c0: 7665 6c0a 2020 2020 2320 7570 6c69 6e6b  vel.    # uplink
+000073d0: 4465 7669 6365 0a20 2020 2023 2072 6563  Device.    # rec
+000073e0: 6f72 6469 6e67 5363 6865 6475 6c65 7356  ordingSchedulesV
+000073f0: 320a 0a20 2020 2023 206e 6f74 2064 6972  2..    # not dir
+00007400: 6563 746c 7920 6672 6f6d 2055 6e69 4669  ectly from UniFi
+00007410: 0a20 2020 206c 6173 745f 7269 6e67 5f65  .    last_ring_e
+00007420: 7665 6e74 5f69 643a 204f 7074 696f 6e61  vent_id: Optiona
+00007430: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
+00007440: 2020 6c61 7374 5f73 6d61 7274 5f64 6574    last_smart_det
+00007450: 6563 743a 204f 7074 696f 6e61 6c5b 6461  ect: Optional[da
+00007460: 7465 7469 6d65 5d20 3d20 4e6f 6e65 0a20  tetime] = None. 
+00007470: 2020 206c 6173 745f 736d 6172 745f 6175     last_smart_au
+00007480: 6469 6f5f 6465 7465 6374 3a20 4f70 7469  dio_detect: Opti
+00007490: 6f6e 616c 5b64 6174 6574 696d 655d 203d  onal[datetime] =
+000074a0: 204e 6f6e 650a 2020 2020 6c61 7374 5f73   None.    last_s
+000074b0: 6d61 7274 5f64 6574 6563 745f 6576 656e  mart_detect_even
+000074c0: 745f 6964 3a20 4f70 7469 6f6e 616c 5b73  t_id: Optional[s
+000074d0: 7472 5d20 3d20 4e6f 6e65 0a20 2020 206c  tr] = None.    l
+000074e0: 6173 745f 736d 6172 745f 6175 6469 6f5f  ast_smart_audio_
+000074f0: 6465 7465 6374 5f65 7665 6e74 5f69 643a  detect_event_id:
+00007500: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00007510: 204e 6f6e 650a 2020 2020 6c61 7374 5f73   None.    last_s
+00007520: 6d61 7274 5f64 6574 6563 7473 3a20 6469  mart_detects: di
+00007530: 6374 5b53 6d61 7274 4465 7465 6374 4f62  ct[SmartDetectOb
+00007540: 6a65 6374 5479 7065 2c20 6461 7465 7469  jectType, dateti
+00007550: 6d65 5d20 3d20 7b7d 0a20 2020 206c 6173  me] = {}.    las
+00007560: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
+00007570: 7465 6374 733a 2064 6963 745b 536d 6172  tects: dict[Smar
+00007580: 7444 6574 6563 7441 7564 696f 5479 7065  tDetectAudioType
+00007590: 2c20 6461 7465 7469 6d65 5d20 3d20 7b7d  , datetime] = {}
+000075a0: 0a20 2020 206c 6173 745f 736d 6172 745f  .    last_smart_
+000075b0: 6465 7465 6374 5f65 7665 6e74 5f69 6473  detect_event_ids
+000075c0: 3a20 6469 6374 5b53 6d61 7274 4465 7465  : dict[SmartDete
+000075d0: 6374 4f62 6a65 6374 5479 7065 2c20 7374  ctObjectType, st
+000075e0: 725d 203d 207b 7d0a 2020 2020 6c61 7374  r] = {}.    last
+000075f0: 5f73 6d61 7274 5f61 7564 696f 5f64 6574  _smart_audio_det
+00007600: 6563 745f 6576 656e 745f 6964 733a 2064  ect_event_ids: d
+00007610: 6963 745b 536d 6172 7444 6574 6563 7441  ict[SmartDetectA
+00007620: 7564 696f 5479 7065 2c20 7374 725d 203d  udioType, str] =
+00007630: 207b 7d0a 2020 2020 7461 6c6b 6261 636b   {}.    talkback
+00007640: 5f73 7472 6561 6d3a 204f 7074 696f 6e61  _stream: Optiona
+00007650: 6c5b 5461 6c6b 6261 636b 5374 7265 616d  l[TalkbackStream
+00007660: 5d20 3d20 4e6f 6e65 0a20 2020 205f 6c61  ] = None.    _la
+00007670: 7374 5f72 696e 675f 7469 6d65 6f75 743a  st_ring_timeout:
+00007680: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
+00007690: 6d65 5d20 3d20 5072 6976 6174 6541 7474  me] = PrivateAtt
+000076a0: 7228 4e6f 6e65 290a 0a20 2020 2040 636c  r(None)..    @cl
+000076b0: 6173 736d 6574 686f 640a 2020 2020 4063  assmethod.    @c
+000076c0: 6163 6865 0a20 2020 2064 6566 205f 6765  ache.    def _ge
+000076d0: 745f 756e 6966 695f 7265 6d61 7073 2863  t_unifi_remaps(c
+000076e0: 6c73 2920 2d3e 2064 6963 745b 7374 722c  ls) -> dict[str,
+000076f0: 2073 7472 5d3a 0a20 2020 2020 2020 2072   str]:.        r
+00007700: 6574 7572 6e20 7b2a 2a73 7570 6572 2829  eturn {**super()
+00007710: 2e5f 6765 745f 756e 6966 695f 7265 6d61  ._get_unifi_rema
+00007720: 7073 2829 2c20 2269 7332 4b22 3a20 2269  ps(), "is2K": "i
+00007730: 7332 6b22 2c20 2269 7334 4b22 3a20 2269  s2k", "is4K": "i
+00007740: 7334 6b22 7d0a 0a20 2020 2040 636c 6173  s4k"}..    @clas
+00007750: 736d 6574 686f 640a 2020 2020 4063 6163  smethod.    @cac
+00007760: 6865 0a20 2020 2064 6566 205f 6765 745f  he.    def _get_
+00007770: 6578 636c 7564 6564 5f63 6861 6e67 6564  excluded_changed
+00007780: 5f66 6965 6c64 7328 636c 7329 202d 3e20  _fields(cls) -> 
+00007790: 7365 745b 7374 725d 3a0a 2020 2020 2020  set[str]:.      
+000077a0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000077b0: 2e5f 6765 745f 6578 636c 7564 6564 5f63  ._get_excluded_c
+000077c0: 6861 6e67 6564 5f66 6965 6c64 7328 2920  hanged_fields() 
+000077d0: 7c20 7b0a 2020 2020 2020 2020 2020 2020  | {.            
+000077e0: 226c 6173 745f 7269 6e67 5f65 7665 6e74  "last_ring_event
+000077f0: 5f69 6422 2c0a 2020 2020 2020 2020 2020  _id",.          
+00007800: 2020 226c 6173 745f 736d 6172 745f 6465    "last_smart_de
+00007810: 7465 6374 222c 0a20 2020 2020 2020 2020  tect",.         
+00007820: 2020 2022 6c61 7374 5f73 6d61 7274 5f61     "last_smart_a
+00007830: 7564 696f 5f64 6574 6563 7422 2c0a 2020  udio_detect",.  
+00007840: 2020 2020 2020 2020 2020 226c 6173 745f            "last_
+00007850: 736d 6172 745f 6465 7465 6374 5f65 7665  smart_detect_eve
+00007860: 6e74 5f69 6422 2c0a 2020 2020 2020 2020  nt_id",.        
+00007870: 2020 2020 226c 6173 745f 736d 6172 745f      "last_smart_
+00007880: 6175 6469 6f5f 6465 7465 6374 5f65 7665  audio_detect_eve
+00007890: 6e74 5f69 6422 2c0a 2020 2020 2020 2020  nt_id",.        
+000078a0: 2020 2020 226c 6173 745f 736d 6172 745f      "last_smart_
+000078b0: 6465 7465 6374 7322 2c0a 2020 2020 2020  detects",.      
+000078c0: 2020 2020 2020 226c 6173 745f 736d 6172        "last_smar
+000078d0: 745f 6175 6469 6f5f 6465 7465 6374 7322  t_audio_detects"
+000078e0: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
+000078f0: 6173 745f 736d 6172 745f 6465 7465 6374  ast_smart_detect
+00007900: 5f65 7665 6e74 5f69 6473 222c 0a20 2020  _event_ids",.   
+00007910: 2020 2020 2020 2020 2022 6c61 7374 5f73           "last_s
+00007920: 6d61 7274 5f61 7564 696f 5f64 6574 6563  mart_audio_detec
+00007930: 745f 6576 656e 745f 6964 7322 2c0a 2020  t_event_ids",.  
+00007940: 2020 2020 2020 2020 2020 2274 616c 6b62            "talkb
+00007950: 6163 6b5f 7374 7265 616d 222c 0a20 2020  ack_stream",.   
+00007960: 2020 2020 207d 0a0a 2020 2020 4063 6c61       }..    @cla
+00007970: 7373 6d65 7468 6f64 0a20 2020 2040 6361  ssmethod.    @ca
+00007980: 6368 650a 2020 2020 6465 6620 5f67 6574  che.    def _get
+00007990: 5f72 6561 645f 6f6e 6c79 5f66 6965 6c64  _read_only_field
+000079a0: 7328 636c 7329 202d 3e20 7365 745b 7374  s(cls) -> set[st
+000079b0: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
+000079c0: 726e 2073 7570 6572 2829 2e5f 6765 745f  rn super()._get_
+000079d0: 7265 6164 5f6f 6e6c 795f 6669 656c 6473  read_only_fields
+000079e0: 2829 207c 207b 0a20 2020 2020 2020 2020  () | {.         
+000079f0: 2020 2022 7374 6174 7322 2c0a 2020 2020     "stats",.    
+00007a00: 2020 2020 2020 2020 2269 7344 656c 6574          "isDelet
+00007a10: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
+00007a20: 2020 2269 7352 6563 6f72 6469 6e67 222c    "isRecording",
+00007a30: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+00007a40: 4d6f 7469 6f6e 4465 7465 6374 6564 222c  MotionDetected",
+00007a50: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+00007a60: 536d 6172 7444 6574 6563 7465 6422 2c0a  SmartDetected",.
+00007a70: 2020 2020 2020 2020 2020 2020 2270 6879              "phy
+00007a80: 5261 7465 222c 0a20 2020 2020 2020 2020  Rate",.         
+00007a90: 2020 2022 6973 5072 6f62 696e 6746 6f72     "isProbingFor
+00007aa0: 5769 6669 222c 0a20 2020 2020 2020 2020  Wifi",.         
+00007ab0: 2020 2022 6c61 7374 5269 6e67 222c 0a20     "lastRing",. 
+00007ac0: 2020 2020 2020 2020 2020 2022 6973 4c69             "isLi
+00007ad0: 7665 4865 6174 6d61 7045 6e61 626c 6564  veHeatmapEnabled
+00007ae0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00007af0: 7669 6465 6f52 6563 6f6e 6669 6775 7261  videoReconfigura
+00007b00: 7469 6f6e 496e 5072 6f67 7265 7373 222c  tionInProgress",
+00007b10: 0a20 2020 2020 2020 2020 2020 2022 6c65  .            "le
+00007b20: 6e73 6573 222c 0a20 2020 2020 2020 2020  nses",.         
+00007b30: 2020 2022 6973 506f 6f72 4e65 7477 6f72     "isPoorNetwor
+00007b40: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00007b50: 2266 6561 7475 7265 466c 6167 7322 2c0a  "featureFlags",.
+00007b60: 2020 2020 2020 2020 7d0a 0a20 2020 2040          }..    @
+00007b70: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00007b80: 6465 6620 756e 6966 695f 6469 6374 5f74  def unifi_dict_t
+00007b90: 6f5f 6469 6374 2863 6c73 2c20 6461 7461  o_dict(cls, data
+00007ba0: 3a20 6469 6374 5b73 7472 2c20 416e 795d  : dict[str, Any]
+00007bb0: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
+00007bc0: 6e79 5d3a 0a20 2020 2020 2020 2023 204c  ny]:.        # L
+00007bd0: 4344 206d 6573 7361 6765 7320 636f 6d65  CD messages come
+00007be0: 7320 6261 636b 2061 7320 656d 7074 7920  s back as empty 
+00007bf0: 6469 6374 207b 7d0a 2020 2020 2020 2020  dict {}.        
+00007c00: 6966 2022 6c63 644d 6573 7361 6765 2220  if "lcdMessage" 
+00007c10: 696e 2064 6174 6120 616e 6420 6c65 6e28  in data and len(
+00007c20: 6461 7461 5b22 6c63 644d 6573 7361 6765  data["lcdMessage
+00007c30: 225d 2e6b 6579 7328 2929 203d 3d20 303a  "].keys()) == 0:
+00007c40: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00007c50: 2064 6174 615b 226c 6364 4d65 7373 6167   data["lcdMessag
+00007c60: 6522 5d0a 2020 2020 2020 2020 6966 2022  e"].        if "
+00007c70: 6368 696d 6544 7572 6174 696f 6e22 2069  chimeDuration" i
+00007c80: 6e20 6461 7461 2061 6e64 206e 6f74 2069  n data and not i
+00007c90: 7369 6e73 7461 6e63 6528 6461 7461 5b22  sinstance(data["
+00007ca0: 6368 696d 6544 7572 6174 696f 6e22 5d2c  chimeDuration"],
+00007cb0: 2074 696d 6564 656c 7461 293a 0a20 2020   timedelta):.   
+00007cc0: 2020 2020 2020 2020 2064 6174 615b 2263           data["c
+00007cd0: 6869 6d65 4475 7261 7469 6f6e 225d 203d  himeDuration"] =
+00007ce0: 2074 696d 6564 656c 7461 286d 696c 6c69   timedelta(milli
+00007cf0: 7365 636f 6e64 733d 6461 7461 5b22 6368  seconds=data["ch
+00007d00: 696d 6544 7572 6174 696f 6e22 5d29 0a0a  imeDuration"])..
+00007d10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007d20: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
+00007d30: 745f 746f 5f64 6963 7428 6461 7461 290a  t_to_dict(data).
+00007d40: 0a20 2020 2064 6566 2075 6e69 6669 5f64  .    def unifi_d
+00007d50: 6963 7428 0a20 2020 2020 2020 2073 656c  ict(.        sel
+00007d60: 662c 0a20 2020 2020 2020 2064 6174 613a  f,.        data:
+00007d70: 204f 7074 696f 6e61 6c5b 6469 6374 5b73   Optional[dict[s
+00007d80: 7472 2c20 416e 795d 5d20 3d20 4e6f 6e65  tr, Any]] = None
+00007d90: 2c0a 2020 2020 2020 2020 6578 636c 7564  ,.        exclud
+00007da0: 653a 204f 7074 696f 6e61 6c5b 7365 745b  e: Optional[set[
+00007db0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00007dc0: 2020 2920 2d3e 2064 6963 745b 7374 722c    ) -> dict[str,
+00007dd0: 2041 6e79 5d3a 0a20 2020 2020 2020 2069   Any]:.        i
+00007de0: 6620 6461 7461 2069 7320 6e6f 7420 4e6f  f data is not No
+00007df0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007e00: 6966 2022 6d6f 7469 6f6e 5f7a 6f6e 6573  if "motion_zones
+00007e10: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
+00007e20: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00007e30: 226d 6f74 696f 6e5f 7a6f 6e65 7322 5d20  "motion_zones"] 
+00007e40: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00007e50: 2020 2020 2020 2020 4d6f 7469 6f6e 5a6f          MotionZo
+00007e60: 6e65 282a 2a7a 292e 756e 6966 695f 6469  ne(**z).unifi_di
+00007e70: 6374 2829 2066 6f72 207a 2069 6e20 6461  ct() for z in da
+00007e80: 7461 5b22 6d6f 7469 6f6e 5f7a 6f6e 6573  ta["motion_zones
+00007e90: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00007ea0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00007eb0: 2069 6620 2270 7269 7661 6379 5f7a 6f6e   if "privacy_zon
+00007ec0: 6573 2220 696e 2064 6174 613a 0a20 2020  es" in data:.   
+00007ed0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00007ee0: 615b 2270 7269 7661 6379 5f7a 6f6e 6573  a["privacy_zones
+00007ef0: 225d 203d 205b 0a20 2020 2020 2020 2020  "] = [.         
+00007f00: 2020 2020 2020 2020 2020 2043 616d 6572             Camer
+00007f10: 615a 6f6e 6528 2a2a 7a29 2e75 6e69 6669  aZone(**z).unifi
+00007f20: 5f64 6963 7428 2920 666f 7220 7a20 696e  _dict() for z in
+00007f30: 2064 6174 615b 2270 7269 7661 6379 5f7a   data["privacy_z
+00007f40: 6f6e 6573 225d 0a20 2020 2020 2020 2020  ones"].         
+00007f50: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00007f60: 2020 2020 2069 6620 2273 6d61 7274 5f64       if "smart_d
+00007f70: 6574 6563 745f 7a6f 6e65 7322 2069 6e20  etect_zones" in 
+00007f80: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+00007f90: 2020 2020 2020 6461 7461 5b22 736d 6172        data["smar
+00007fa0: 745f 6465 7465 6374 5f7a 6f6e 6573 225d  t_detect_zones"]
+00007fb0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00007fc0: 2020 2020 2020 2020 2053 6d61 7274 4d6f           SmartMo
+00007fd0: 7469 6f6e 5a6f 6e65 282a 2a7a 292e 756e  tionZone(**z).un
+00007fe0: 6966 695f 6469 6374 2829 0a20 2020 2020  ifi_dict().     
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00008000: 6f72 207a 2069 6e20 6461 7461 5b22 736d  or z in data["sm
+00008010: 6172 745f 6465 7465 6374 5f7a 6f6e 6573  art_detect_zones
+00008020: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00008030: 2020 205d 0a0a 2020 2020 2020 2020 6461     ]..        da
+00008040: 7461 203d 2073 7570 6572 2829 2e75 6e69  ta = super().uni
+00008050: 6669 5f64 6963 7428 6461 7461 3d64 6174  fi_dict(data=dat
+00008060: 612c 2065 7863 6c75 6465 3d65 7863 6c75  a, exclude=exclu
+00008070: 6465 290a 0a20 2020 2020 2020 2069 6620  de)..        if 
+00008080: 226c 6173 7452 696e 6745 7665 6e74 4964  "lastRingEventId
+00008090: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
+000080a0: 2020 2020 2020 2064 656c 2064 6174 615b         del data[
+000080b0: 226c 6173 7452 696e 6745 7665 6e74 4964  "lastRingEventId
+000080c0: 225d 0a20 2020 2020 2020 2069 6620 226c  "].        if "l
+000080d0: 6173 7453 6d61 7274 4465 7465 6374 2220  astSmartDetect" 
+000080e0: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
+000080f0: 2020 2020 2064 656c 2064 6174 615b 226c       del data["l
+00008100: 6173 7453 6d61 7274 4465 7465 6374 225d  astSmartDetect"]
+00008110: 0a20 2020 2020 2020 2069 6620 226c 6173  .        if "las
+00008120: 7453 6d61 7274 4175 6469 6f44 6574 6563  tSmartAudioDetec
+00008130: 7422 2069 6e20 6461 7461 3a0a 2020 2020  t" in data:.    
+00008140: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
+00008150: 5b22 6c61 7374 536d 6172 7441 7564 696f  ["lastSmartAudio
+00008160: 4465 7465 6374 225d 0a20 2020 2020 2020  Detect"].       
+00008170: 2069 6620 226c 6173 7453 6d61 7274 4465   if "lastSmartDe
+00008180: 7465 6374 4576 656e 7449 6422 2069 6e20  tectEventId" in 
+00008190: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+000081a0: 2020 6465 6c20 6461 7461 5b22 6c61 7374    del data["last
+000081b0: 536d 6172 7444 6574 6563 7445 7665 6e74  SmartDetectEvent
+000081c0: 4964 225d 0a20 2020 2020 2020 2069 6620  Id"].        if 
+000081d0: 226c 6173 7453 6d61 7274 4175 6469 6f44  "lastSmartAudioD
+000081e0: 6574 6563 7445 7665 6e74 4964 2220 696e  etectEventId" in
+000081f0: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+00008200: 2020 2064 656c 2064 6174 615b 226c 6173     del data["las
+00008210: 7453 6d61 7274 4175 6469 6f44 6574 6563  tSmartAudioDetec
+00008220: 7445 7665 6e74 4964 225d 0a20 2020 2020  tEventId"].     
+00008230: 2020 2069 6620 226c 6173 7453 6d61 7274     if "lastSmart
+00008240: 4465 7465 6374 7322 2069 6e20 6461 7461  Detects" in data
+00008250: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00008260: 6c20 6461 7461 5b22 6c61 7374 536d 6172  l data["lastSmar
+00008270: 7444 6574 6563 7473 225d 0a20 2020 2020  tDetects"].     
+00008280: 2020 2069 6620 226c 6173 7453 6d61 7274     if "lastSmart
+00008290: 4175 6469 6f44 6574 6563 7473 2220 696e  AudioDetects" in
+000082a0: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+000082b0: 2020 2064 656c 2064 6174 615b 226c 6173     del data["las
+000082c0: 7453 6d61 7274 4175 6469 6f44 6574 6563  tSmartAudioDetec
+000082d0: 7473 225d 0a20 2020 2020 2020 2069 6620  ts"].        if 
+000082e0: 226c 6173 7453 6d61 7274 4465 7465 6374  "lastSmartDetect
+000082f0: 4576 656e 7449 6473 2220 696e 2064 6174  EventIds" in dat
+00008300: 613a 0a20 2020 2020 2020 2020 2020 2064  a:.            d
+00008310: 656c 2064 6174 615b 226c 6173 7453 6d61  el data["lastSma
+00008320: 7274 4465 7465 6374 4576 656e 7449 6473  rtDetectEventIds
+00008330: 225d 0a20 2020 2020 2020 2069 6620 226c  "].        if "l
+00008340: 6173 7453 6d61 7274 4175 6469 6f44 6574  astSmartAudioDet
+00008350: 6563 7445 7665 6e74 4964 7322 2069 6e20  ectEventIds" in 
+00008360: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+00008370: 2020 6465 6c20 6461 7461 5b22 6c61 7374    del data["last
+00008380: 536d 6172 7441 7564 696f 4465 7465 6374  SmartAudioDetect
+00008390: 4576 656e 7449 6473 225d 0a20 2020 2020  EventIds"].     
+000083a0: 2020 2069 6620 2274 616c 6b62 6163 6b53     if "talkbackS
+000083b0: 7472 6561 6d22 2069 6e20 6461 7461 3a0a  tream" in data:.
+000083c0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+000083d0: 6461 7461 5b22 7461 6c6b 6261 636b 5374  data["talkbackSt
+000083e0: 7265 616d 225d 0a20 2020 2020 2020 2069  ream"].        i
+000083f0: 6620 226c 6364 4d65 7373 6167 6522 2069  f "lcdMessage" i
+00008400: 6e20 6461 7461 2061 6e64 2064 6174 615b  n data and data[
+00008410: 226c 6364 4d65 7373 6167 6522 5d20 6973  "lcdMessage"] is
+00008420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00008430: 2020 2064 6174 615b 226c 6364 4d65 7373     data["lcdMess
+00008440: 6167 6522 5d20 3d20 7b7d 0a0a 2020 2020  age"] = {}..    
+00008450: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
+00008460: 0a20 2020 2064 6566 2067 6574 5f63 6861  .    def get_cha
+00008470: 6e67 6564 2873 656c 662c 2064 6174 615f  nged(self, data_
+00008480: 6265 666f 7265 5f63 6861 6e67 6573 3a20  before_changes: 
+00008490: 6469 6374 5b73 7472 2c20 416e 795d 2920  dict[str, Any]) 
+000084a0: 2d3e 2064 6963 745b 7374 722c 2041 6e79  -> dict[str, Any
+000084b0: 5d3a 0a20 2020 2020 2020 2075 7064 6174  ]:.        updat
+000084c0: 6564 203d 2073 7570 6572 2829 2e67 6574  ed = super().get
+000084d0: 5f63 6861 6e67 6564 2864 6174 615f 6265  _changed(data_be
+000084e0: 666f 7265 5f63 6861 6e67 6573 290a 0a20  fore_changes).. 
+000084f0: 2020 2020 2020 2069 6620 226c 6364 5f6d         if "lcd_m
+00008500: 6573 7361 6765 2220 696e 2075 7064 6174  essage" in updat
+00008510: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00008520: 6c63 645f 6d65 7373 6167 6520 3d20 7570  lcd_message = up
+00008530: 6461 7465 645b 226c 6364 5f6d 6573 7361  dated["lcd_messa
+00008540: 6765 225d 0a20 2020 2020 2020 2020 2020  ge"].           
+00008550: 2023 2074 6f20 2263 6c65 6172 2220 4c43   # to "clear" LC
+00008560: 4420 6d65 7373 6167 652c 2073 6574 2072  D message, set r
+00008570: 6573 6574 5f61 7420 746f 2061 2074 696d  eset_at to a tim
+00008580: 6520 696e 2074 6865 2070 6173 740a 2020  e in the past.  
+00008590: 2020 2020 2020 2020 2020 6966 206c 6364            if lcd
+000085a0: 5f6d 6573 7361 6765 2069 7320 4e6f 6e65  _message is None
+000085b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000085c0: 2020 7570 6461 7465 645b 226c 6364 5f6d    updated["lcd_m
+000085d0: 6573 7361 6765 225d 203d 207b 2272 6573  essage"] = {"res
+000085e0: 6574 5f61 7422 3a20 7574 635f 6e6f 7728  et_at": utc_now(
+000085f0: 2920 2d20 7469 6d65 6465 6c74 6128 7365  ) - timedelta(se
+00008600: 636f 6e64 733d 3130 297d 0a20 2020 2020  conds=10)}.     
+00008610: 2020 2020 2020 2023 206f 7468 6572 7769         # otherwi
+00008620: 7365 2c20 7061 7373 2066 756c 6c20 4c43  se, pass full LC
+00008630: 4420 6d65 7373 6167 6520 746f 2070 7265  D message to pre
+00008640: 7665 6e74 2069 7373 7565 730a 2020 2020  vent issues.    
+00008650: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00008660: 662e 6c63 645f 6d65 7373 6167 6520 6973  f.lcd_message is
+00008670: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008680: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+00008690: 6564 5b22 6c63 645f 6d65 7373 6167 6522  ed["lcd_message"
+000086a0: 5d20 3d20 7365 6c66 2e6c 6364 5f6d 6573  ] = self.lcd_mes
+000086b0: 7361 6765 2e64 6963 7428 290a 0a20 2020  sage.dict()..   
+000086c0: 2020 2020 2020 2020 2023 2069 6620 7265           # if re
+000086d0: 7365 745f 6174 2069 7320 6e6f 7420 7061  set_at is not pa
+000086e0: 7373 6564 2069 6e2c 2069 7420 7769 6c6c  ssed in, it will
+000086f0: 2064 6566 6175 6c74 2074 6f20 7265 7365   default to rese
+00008700: 7420 696e 2031 206d 696e 7574 650a 2020  t in 1 minute.  
+00008710: 2020 2020 2020 2020 2020 6966 206c 6364            if lcd
+00008720: 5f6d 6573 7361 6765 2069 7320 6e6f 7420  _message is not 
+00008730: 4e6f 6e65 2061 6e64 2022 7265 7365 745f  None and "reset_
+00008740: 6174 2220 6e6f 7420 696e 206c 6364 5f6d  at" not in lcd_m
+00008750: 6573 7361 6765 3a0a 2020 2020 2020 2020  essage:.        
+00008760: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008770: 6c63 645f 6d65 7373 6167 6520 6973 204e  lcd_message is N
+00008780: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008790: 2020 2020 2020 2020 2075 7064 6174 6564           updated
+000087a0: 5b22 6c63 645f 6d65 7373 6167 6522 5d5b  ["lcd_message"][
+000087b0: 2272 6573 6574 5f61 7422 5d20 3d20 4e6f  "reset_at"] = No
+000087c0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+000087d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000087e0: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+000087f0: 6174 6564 5b22 6c63 645f 6d65 7373 6167  ated["lcd_messag
+00008800: 6522 5d5b 2272 6573 6574 5f61 7422 5d20  e"]["reset_at"] 
+00008810: 3d20 7365 6c66 2e6c 6364 5f6d 6573 7361  = self.lcd_messa
+00008820: 6765 2e72 6573 6574 5f61 740a 0a20 2020  ge.reset_at..   
+00008830: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
+00008840: 7465 640a 0a20 2020 2064 6566 2075 7064  ted..    def upd
+00008850: 6174 655f 6672 6f6d 5f64 6963 7428 7365  ate_from_dict(se
+00008860: 6c66 2c20 6461 7461 3a20 6469 6374 5b73  lf, data: dict[s
+00008870: 7472 2c20 416e 795d 2920 2d3e 2043 616d  tr, Any]) -> Cam
+00008880: 6572 613a 0a20 2020 2020 2020 2023 2061  era:.        # a
+00008890: 206d 6573 7361 6765 2069 6e20 7468 6520   message in the 
+000088a0: 7061 7374 2069 7320 6163 7475 616c 6c79  past is actually
+000088b0: 2061 2073 696e 6761 6c20 746f 2077 6970   a singal to wip
+000088c0: 6520 7468 6520 6d65 7373 6167 650a 2020  e the message.  
+000088d0: 2020 2020 2020 7265 7365 745f 6174 203d        reset_at =
+000088e0: 2064 6174 612e 6765 7428 226c 6364 5f6d   data.get("lcd_m
+000088f0: 6573 7361 6765 222c 207b 7d29 2e67 6574  essage", {}).get
+00008900: 2822 7265 7365 745f 6174 2229 0a20 2020  ("reset_at").   
+00008910: 2020 2020 2069 6620 7265 7365 745f 6174       if reset_at
+00008920: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00008930: 2020 2020 2020 2020 2020 7265 7365 745f            reset_
+00008940: 6174 203d 2066 726f 6d5f 6a73 5f74 696d  at = from_js_tim
+00008950: 6528 7265 7365 745f 6174 290a 2020 2020  e(reset_at).    
+00008960: 2020 2020 2020 2020 6966 2075 7463 5f6e          if utc_n
+00008970: 6f77 2829 203e 2072 6573 6574 5f61 743a  ow() > reset_at:
+00008980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008990: 2064 6174 615b 226c 6364 5f6d 6573 7361   data["lcd_messa
+000089a0: 6765 225d 203d 204e 6f6e 650a 0a20 2020  ge"] = None..   
+000089b0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+000089c0: 7228 292e 7570 6461 7465 5f66 726f 6d5f  r().update_from_
+000089d0: 6469 6374 2864 6174 6129 0a0a 2020 2020  dict(data)..    
+000089e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000089f0: 6620 6c61 7374 5f72 696e 675f 6576 656e  f last_ring_even
+00008a00: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
+00008a10: 6e61 6c5b 4576 656e 745d 3a0a 2020 2020  nal[Event]:.    
+00008a20: 2020 2020 6966 2073 656c 662e 6c61 7374      if self.last
+00008a30: 5f72 696e 675f 6576 656e 745f 6964 2069  _ring_event_id i
+00008a40: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00008a50: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00008a60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008a70: 7365 6c66 2e61 7069 2e62 6f6f 7473 7472  self.api.bootstr
+00008a80: 6170 2e65 7665 6e74 732e 6765 7428 7365  ap.events.get(se
+00008a90: 6c66 2e6c 6173 745f 7269 6e67 5f65 7665  lf.last_ring_eve
+00008aa0: 6e74 5f69 6429 0a0a 2020 2020 4070 726f  nt_id)..    @pro
+00008ab0: 7065 7274 790a 2020 2020 6465 6620 6c61  perty.    def la
+00008ac0: 7374 5f73 6d61 7274 5f64 6574 6563 745f  st_smart_detect_
+00008ad0: 6576 656e 7428 7365 6c66 2920 2d3e 204f  event(self) -> O
+00008ae0: 7074 696f 6e61 6c5b 4576 656e 745d 3a0a  ptional[Event]:.
+00008af0: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00008b00: 6865 206c 6173 7420 736d 6172 7420 6465  he last smart de
+00008b10: 7465 6374 2065 7665 6e74 2069 642e 2222  tect event id.""
+00008b20: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00008b30: 6c66 2e6c 6173 745f 736d 6172 745f 6465  lf.last_smart_de
+00008b40: 7465 6374 5f65 7665 6e74 5f69 6420 6973  tect_event_id is
+00008b50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00008b60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00008b70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008b80: 656c 662e 6170 692e 626f 6f74 7374 7261  elf.api.bootstra
+00008b90: 702e 6576 656e 7473 2e67 6574 2873 656c  p.events.get(sel
+00008ba0: 662e 6c61 7374 5f73 6d61 7274 5f64 6574  f.last_smart_det
+00008bb0: 6563 745f 6576 656e 745f 6964 290a 0a20  ect_event_id).. 
+00008bc0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00008bd0: 2064 6566 2068 6472 5f6d 6f64 655f 6469   def hdr_mode_di
+00008be0: 7370 6c61 7928 7365 6c66 2920 2d3e 204c  splay(self) -> L
+00008bf0: 6974 6572 616c 5b22 6175 746f 222c 2022  iteral["auto", "
+00008c00: 6f66 6622 2c20 2261 6c77 6179 7322 5d3a  off", "always"]:
+00008c10: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00008c20: 4844 5220 6d6f 6465 2073 696d 696c 6172  HDR mode similar
+00008c30: 2074 6f20 686f 7720 5072 6f74 6563 7420   to how Protect 
+00008c40: 696e 7465 7266 6163 6520 776f 726b 732e  interface works.
+00008c50: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00008c60: 6e6f 7420 7365 6c66 2e68 6472 5f6d 6f64  not self.hdr_mod
+00008c70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00008c80: 6574 7572 6e20 226f 6666 220a 2020 2020  eturn "off".    
+00008c90: 2020 2020 6966 2073 656c 662e 6973 705f      if self.isp_
+00008ca0: 7365 7474 696e 6773 2e68 6472 5f6d 6f64  settings.hdr_mod
+00008cb0: 6520 3d3d 2048 4452 4d6f 6465 2e4e 4f52  e == HDRMode.NOR
+00008cc0: 4d41 4c3a 0a20 2020 2020 2020 2020 2020  MAL:.           
+00008cd0: 2072 6574 7572 6e20 2261 7574 6f22 0a20   return "auto". 
+00008ce0: 2020 2020 2020 2072 6574 7572 6e20 2261         return "a
+00008cf0: 6c77 6179 7322 0a0a 2020 2020 4070 726f  lways"..    @pro
+00008d00: 7065 7274 790a 2020 2020 6465 6620 6963  perty.    def ic
+00008d10: 725f 6c75 785f 6469 7370 6c61 7928 7365  r_lux_display(se
+00008d20: 6c66 2920 2d3e 2069 6e74 207c 204e 6f6e  lf) -> int | Non
+00008d30: 653a 0a20 2020 2020 2020 2022 2222 4765  e:.        """Ge
+00008d40: 7420 4943 5220 4375 7374 6f6d 204c 7578  t ICR Custom Lux
+00008d50: 2076 616c 7565 2073 696d 696c 6172 2074   value similar t
+00008d60: 6f20 686f 7720 7468 6520 5072 6f74 6563  o how the Protec
+00008d70: 7420 696e 7465 7266 6163 6520 776f 726b  t interface work
+00008d80: 732e 2222 220a 0a20 2020 2020 2020 2069  s."""..        i
+00008d90: 6620 7365 6c66 2e69 7370 5f73 6574 7469  f self.isp_setti
+00008da0: 6e67 732e 6963 725f 6375 7374 6f6d 5f76  ngs.icr_custom_v
+00008db0: 616c 7565 2069 7320 4e6f 6e65 3a0a 2020  alue is None:.  
+00008dc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008dd0: 204e 6f6e 650a 0a20 2020 2020 2020 2072   None..        r
+00008de0: 6574 7572 6e20 4c55 585f 4d41 5050 494e  eturn LUX_MAPPIN
+00008df0: 475f 5641 4c55 4553 5b31 3020 2d20 7365  G_VALUES[10 - se
+00008e00: 6c66 2e69 7370 5f73 6574 7469 6e67 732e  lf.isp_settings.
+00008e10: 6963 725f 6375 7374 6f6d 5f76 616c 7565  icr_custom_value
+00008e20: 5d0a 0a20 2020 2064 6566 2067 6574 5f6c  ]..    def get_l
+00008e30: 6173 745f 736d 6172 745f 6465 7465 6374  ast_smart_detect
+00008e40: 5f65 7665 6e74 280a 2020 2020 2020 2020  _event(.        
+00008e50: 7365 6c66 2c0a 2020 2020 2020 2020 736d  self,.        sm
+00008e60: 6172 745f 7479 7065 3a20 536d 6172 7444  art_type: SmartD
+00008e70: 6574 6563 744f 626a 6563 7454 7970 652c  etectObjectType,
+00008e80: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
+00008e90: 616c 5b45 7665 6e74 5d3a 0a20 2020 2020  al[Event]:.     
+00008ea0: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
+00008eb0: 7374 2073 6d61 7274 2064 6574 6563 7420  st smart detect 
+00008ec0: 6576 656e 7420 666f 7220 6769 7665 6e20  event for given 
+00008ed0: 7479 7065 2e22 2222 0a0a 2020 2020 2020  type."""..      
+00008ee0: 2020 6576 656e 745f 6964 203d 2073 656c    event_id = sel
+00008ef0: 662e 6c61 7374 5f73 6d61 7274 5f64 6574  f.last_smart_det
+00008f00: 6563 745f 6576 656e 745f 6964 732e 6765  ect_event_ids.ge
+00008f10: 7428 736d 6172 745f 7479 7065 290a 2020  t(smart_type).  
+00008f20: 2020 2020 2020 6966 2065 7665 6e74 5f69        if event_i
+00008f30: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
+00008f40: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00008f50: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
+00008f60: 726e 2073 656c 662e 6170 692e 626f 6f74  rn self.api.boot
+00008f70: 7374 7261 702e 6576 656e 7473 2e67 6574  strap.events.get
+00008f80: 2865 7665 6e74 5f69 6429 0a0a 2020 2020  (event_id)..    
+00008f90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00008fa0: 6620 6c61 7374 5f73 6d61 7274 5f61 7564  f last_smart_aud
+00008fb0: 696f 5f64 6574 6563 745f 6576 656e 7428  io_detect_event(
+00008fc0: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+00008fd0: 6c5b 4576 656e 745d 3a0a 2020 2020 2020  l[Event]:.      
+00008fe0: 2020 2222 2247 6574 2074 6865 206c 6173    """Get the las
+00008ff0: 7420 736d 6172 7420 6175 6469 6f20 6465  t smart audio de
+00009000: 7465 6374 2065 7665 6e74 2069 642e 2222  tect event id.""
+00009010: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00009020: 6c66 2e6c 6173 745f 736d 6172 745f 6175  lf.last_smart_au
+00009030: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
+00009040: 5f69 6420 6973 204e 6f6e 653a 0a20 2020  _id is None:.   
+00009050: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009060: 4e6f 6e65 0a0a 2020 2020 2020 2020 7265  None..        re
+00009070: 7475 726e 2073 656c 662e 6170 692e 626f  turn self.api.bo
+00009080: 6f74 7374 7261 702e 6576 656e 7473 2e67  otstrap.events.g
+00009090: 6574 2873 656c 662e 6c61 7374 5f73 6d61  et(self.last_sma
+000090a0: 7274 5f61 7564 696f 5f64 6574 6563 745f  rt_audio_detect_
+000090b0: 6576 656e 745f 6964 290a 0a20 2020 2064  event_id)..    d
+000090c0: 6566 2067 6574 5f6c 6173 745f 736d 6172  ef get_last_smar
+000090d0: 745f 6175 6469 6f5f 6465 7465 6374 5f65  t_audio_detect_e
+000090e0: 7665 6e74 280a 2020 2020 2020 2020 7365  vent(.        se
+000090f0: 6c66 2c0a 2020 2020 2020 2020 736d 6172  lf,.        smar
+00009100: 745f 7479 7065 3a20 536d 6172 7444 6574  t_type: SmartDet
+00009110: 6563 7441 7564 696f 5479 7065 2c0a 2020  ectAudioType,.  
+00009120: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00009130: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
+00009140: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+00009150: 736d 6172 7420 6175 6469 6f20 6465 7465  smart audio dete
+00009160: 6374 2065 7665 6e74 2066 6f72 2067 6976  ct event for giv
+00009170: 656e 2074 7970 652e 2222 220a 0a20 2020  en type."""..   
+00009180: 2020 2020 2065 7665 6e74 5f69 6420 3d20       event_id = 
+00009190: 7365 6c66 2e6c 6173 745f 736d 6172 745f  self.last_smart_
+000091a0: 6175 6469 6f5f 6465 7465 6374 5f65 7665  audio_detect_eve
+000091b0: 6e74 5f69 6473 2e67 6574 2873 6d61 7274  nt_ids.get(smart
+000091c0: 5f74 7970 6529 0a20 2020 2020 2020 2069  _type).        i
+000091d0: 6620 6576 656e 745f 6964 2069 7320 4e6f  f event_id is No
+000091e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000091f0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00009200: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009210: 2e61 7069 2e62 6f6f 7473 7472 6170 2e65  .api.bootstrap.e
+00009220: 7665 6e74 732e 6765 7428 6576 656e 745f  vents.get(event_
+00009230: 6964 290a 0a20 2020 2040 7072 6f70 6572  id)..    @proper
+00009240: 7479 0a20 2020 2064 6566 2074 696d 656c  ty.    def timel
+00009250: 6170 7365 5f75 726c 2873 656c 6629 202d  apse_url(self) -
+00009260: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
+00009270: 6574 7572 6e20 6622 7b73 656c 662e 6170  eturn f"{self.ap
+00009280: 692e 6261 7365 5f75 726c 7d2f 7072 6f74  i.base_url}/prot
+00009290: 6563 742f 7469 6d65 6c61 7073 652f 7b73  ect/timelapse/{s
+000092a0: 656c 662e 6964 7d22 0a0a 2020 2020 4070  elf.id}"..    @p
+000092b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000092c0: 6973 5f70 7269 7661 6379 5f6f 6e28 7365  is_privacy_on(se
+000092d0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+000092e0: 2020 2020 2069 6e64 6578 2c20 5f20 3d20       index, _ = 
+000092f0: 7365 6c66 2e67 6574 5f70 7269 7661 6379  self.get_privacy
+00009300: 5f7a 6f6e 6528 290a 2020 2020 2020 2020  _zone().        
+00009310: 7265 7475 726e 2069 6e64 6578 2069 7320  return index is 
+00009320: 6e6f 7420 4e6f 6e65 0a0a 2020 2020 4070  not None..    @p
+00009330: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00009340: 6973 5f72 6563 6f72 6469 6e67 5f65 6e61  is_recording_ena
+00009350: 626c 6564 2873 656c 6629 202d 3e20 626f  bled(self) -> bo
+00009360: 6f6c 3a0a 2020 2020 2020 2020 2222 2249  ol:.        """I
+00009370: 7320 7265 636f 7264 696e 6720 666f 6f74  s recording foot
+00009380: 6167 652f 6576 656e 7473 2066 726f 6d20  age/events from 
+00009390: 7468 6520 6361 6d65 7261 2065 6e61 626c  the camera enabl
+000093a0: 6564 3f0a 0a20 2020 2020 2020 2049 6620  ed?..        If 
+000093b0: 7265 636f 7264 696e 6720 6973 206e 6f74  recording is not
+000093c0: 2065 6e61 626c 6564 2c20 6361 6d65 7261   enabled, camera
+000093d0: 7320 7769 6c6c 206e 6f74 2070 726f 6475  s will not produ
+000093e0: 6365 2061 6e79 2066 6f6f 7461 6765 2c20  ce any footage, 
+000093f0: 7468 756d 626e 6169 6c73 2c0a 2020 2020  thumbnails,.    
+00009400: 2020 2020 6d6f 7469 6f6e 2f73 6d61 7274      motion/smart
+00009410: 2064 6574 6563 7469 6f6e 2065 7665 6e74   detection event
+00009420: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
+00009430: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009440: 7573 655f 676c 6f62 616c 3a0a 2020 2020  use_global:.    
+00009450: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009460: 656c 662e 6170 692e 626f 6f74 7374 7261  elf.api.bootstra
+00009470: 702e 6e76 722e 6973 5f67 6c6f 6261 6c5f  p.nvr.is_global_
+00009480: 7265 636f 7264 696e 675f 656e 6162 6c65  recording_enable
+00009490: 640a 0a20 2020 2020 2020 2072 6574 7572  d..        retur
+000094a0: 6e20 7365 6c66 2e72 6563 6f72 6469 6e67  n self.recording
+000094b0: 5f73 6574 7469 6e67 732e 6d6f 6465 2069  _settings.mode i
+000094c0: 7320 6e6f 7420 5265 636f 7264 696e 674d  s not RecordingM
+000094d0: 6f64 652e 4e45 5645 520a 0a20 2020 2040  ode.NEVER..    @
 000094e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000094f0: 2063 616e 5f64 6574 6563 745f 7065 7273   can_detect_pers
-00009500: 6f6e 2873 656c 6629 202d 3e20 626f 6f6c  on(self) -> bool
-00009510: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00009520: 2053 6d61 7274 4465 7465 6374 4f62 6a65   SmartDetectObje
-00009530: 6374 5479 7065 2e50 4552 534f 4e20 696e  ctType.PERSON in
-00009540: 2073 656c 662e 6665 6174 7572 655f 666c   self.feature_fl
-00009550: 6167 732e 736d 6172 745f 6465 7465 6374  ags.smart_detect
-00009560: 5f74 7970 6573 0a0a 2020 2020 4070 726f  _types..    @pro
-00009570: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
-00009580: 5f70 6572 736f 6e5f 6465 7465 6374 696f  _person_detectio
-00009590: 6e5f 6f6e 2873 656c 6629 202d 3e20 626f  n_on(self) -> bo
-000095a0: 6f6c 3a0a 2020 2020 2020 2020 2222 2249  ol:.        """I
-000095b0: 7320 5065 7273 6f6e 2044 6574 6563 7469  s Person Detecti
-000095c0: 6f6e 2061 7661 696c 6162 6c65 2061 6e64  on available and
-000095d0: 2065 6e61 626c 6564 2028 6361 6d65 7261   enabled (camera
-000095e0: 2077 696c 6c20 7072 6f64 7563 6520 7065   will produce pe
-000095f0: 7273 6f6e 2073 6d61 7274 0a20 2020 2020  rson smart.     
-00009600: 2020 2064 6574 6563 7469 6f6e 2065 7665     detection eve
-00009610: 6e74 7329 3f0a 2020 2020 2020 2020 2222  nts)?.        ""
-00009620: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00009630: 6e20 7365 6c66 2e5f 6973 5f73 6d61 7274  n self._is_smart
-00009640: 5f65 6e61 626c 6564 2853 6d61 7274 4465  _enabled(SmartDe
-00009650: 7465 6374 4f62 6a65 6374 5479 7065 2e50  tectObjectType.P
-00009660: 4552 534f 4e29 0a0a 2020 2020 4070 726f  ERSON)..    @pro
-00009670: 7065 7274 790a 2020 2020 6465 6620 6c61  perty.    def la
-00009680: 7374 5f70 6572 736f 6e5f 6465 7465 6374  st_person_detect
-00009690: 5f65 7665 6e74 2873 656c 6629 202d 3e20  _event(self) -> 
-000096a0: 4f70 7469 6f6e 616c 5b45 7665 6e74 5d3a  Optional[Event]:
-000096b0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-000096c0: 7468 6520 6c61 7374 2070 6572 736f 6e20  the last person 
-000096d0: 736d 6172 7420 6465 7465 6374 696f 6e20  smart detection 
-000096e0: 6576 656e 742e 2222 220a 0a20 2020 2020  event."""..     
-000096f0: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-00009700: 6574 5f6c 6173 745f 736d 6172 745f 6465  et_last_smart_de
-00009710: 7465 6374 5f65 7665 6e74 2853 6d61 7274  tect_event(Smart
-00009720: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
-00009730: 2e50 4552 534f 4e29 0a0a 2020 2020 4070  .PERSON)..    @p
-00009740: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00009750: 6c61 7374 5f70 6572 736f 6e5f 6465 7465  last_person_dete
-00009760: 6374 2873 656c 6629 202d 3e20 4f70 7469  ct(self) -> Opti
-00009770: 6f6e 616c 5b64 6174 6574 696d 655d 3a0a  onal[datetime]:.
-00009780: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-00009790: 6865 206c 6173 7420 7065 7273 6f6e 2073  he last person s
-000097a0: 6d61 7274 2064 6574 6563 7469 6f6e 2065  mart detection e
-000097b0: 7665 6e74 2e22 2222 0a0a 2020 2020 2020  vent."""..      
-000097c0: 2020 7265 7475 726e 2073 656c 662e 6c61    return self.la
-000097d0: 7374 5f73 6d61 7274 5f64 6574 6563 7473  st_smart_detects
-000097e0: 2e67 6574 2853 6d61 7274 4465 7465 6374  .get(SmartDetect
-000097f0: 4f62 6a65 6374 5479 7065 2e50 4552 534f  ObjectType.PERSO
-00009800: 4e29 0a0a 2020 2020 4070 726f 7065 7274  N)..    @propert
-00009810: 790a 2020 2020 6465 6620 6973 5f70 6572  y.    def is_per
-00009820: 736f 6e5f 6375 7272 656e 746c 795f 6465  son_currently_de
-00009830: 7465 6374 6564 2873 656c 6629 202d 3e20  tected(self) -> 
-00009840: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00009850: 2249 7320 7065 7273 6f6e 2063 7572 7265  "Is person curre
-00009860: 6e74 6c79 2062 6569 6e67 2064 6574 6563  ntly being detec
-00009870: 7465 6422 2222 0a0a 2020 2020 2020 2020  ted"""..        
-00009880: 7265 7475 726e 2073 656c 662e 5f69 735f  return self._is_
-00009890: 736d 6172 745f 6465 7465 6374 6564 2853  smart_detected(S
-000098a0: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
-000098b0: 5479 7065 2e50 4552 534f 4e29 0a0a 2020  Type.PERSON)..  
-000098c0: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
-000098d0: 7065 7273 6f6e 5f64 6574 6563 7469 6f6e  person_detection
-000098e0: 2873 656c 662c 2065 6e61 626c 6564 3a20  (self, enabled: 
-000098f0: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00009900: 2020 2020 2020 2022 2222 546f 6767 6c65         """Toggle
-00009910: 7320 7065 7273 6f6e 2073 6d61 7274 2064  s person smart d
-00009920: 6574 6563 7469 6f6e 2e20 5265 7175 6972  etection. Requir
-00009930: 6573 2063 616d 6572 6120 746f 2068 6176  es camera to hav
-00009940: 6520 736d 6172 7420 6465 7465 6374 696f  e smart detectio
-00009950: 6e22 2222 0a0a 2020 2020 2020 2020 7265  n"""..        re
-00009960: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00009970: 5f73 6574 5f6f 626a 6563 745f 6465 7465  _set_object_dete
-00009980: 6374 2853 6d61 7274 4465 7465 6374 4f62  ct(SmartDetectOb
-00009990: 6a65 6374 5479 7065 2e50 4552 534f 4e2c  jectType.PERSON,
-000099a0: 2065 6e61 626c 6564 290a 0a20 2020 2040   enabled)..    @
-000099b0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000099c0: 2069 735f 7065 7273 6f6e 5f74 7261 636b   is_person_track
-000099d0: 696e 675f 656e 6162 6c65 6428 7365 6c66  ing_enabled(self
-000099e0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-000099f0: 2020 2022 2222 4973 2070 6572 736f 6e20     """Is person 
-00009a00: 7472 6163 6b69 6e67 2065 6e61 626c 6564  tracking enabled
-00009a10: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00009a20: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
-00009a30: 2073 656c 662e 736d 6172 745f 6465 7465   self.smart_dete
-00009a40: 6374 5f73 6574 7469 6e67 732e 6175 746f  ct_settings.auto
-00009a50: 5f74 7261 636b 696e 675f 6f62 6a65 6374  _tracking_object
-00009a60: 5f74 7970 6573 2069 7320 6e6f 7420 4e6f  _types is not No
-00009a70: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
-00009a80: 6e64 2053 6d61 7274 4465 7465 6374 4f62  nd SmartDetectOb
-00009a90: 6a65 6374 5479 7065 2e50 4552 534f 4e0a  jectType.PERSON.
-00009aa0: 2020 2020 2020 2020 2020 2020 696e 2073              in s
-00009ab0: 656c 662e 736d 6172 745f 6465 7465 6374  elf.smart_detect
-00009ac0: 5f73 6574 7469 6e67 732e 6175 746f 5f74  _settings.auto_t
-00009ad0: 7261 636b 696e 675f 6f62 6a65 6374 5f74  racking_object_t
-00009ae0: 7970 6573 0a20 2020 2020 2020 2029 0a0a  ypes.        )..
-00009af0: 2020 2020 2320 7665 6869 636c 650a 0a20      # vehicle.. 
-00009b00: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00009b10: 2064 6566 2063 616e 5f64 6574 6563 745f   def can_detect_
-00009b20: 7665 6869 636c 6528 7365 6c66 2920 2d3e  vehicle(self) ->
-00009b30: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
-00009b40: 6574 7572 6e20 536d 6172 7444 6574 6563  eturn SmartDetec
-00009b50: 744f 626a 6563 7454 7970 652e 5645 4849  tObjectType.VEHI
-00009b60: 434c 4520 696e 2073 656c 662e 6665 6174  CLE in self.feat
-00009b70: 7572 655f 666c 6167 732e 736d 6172 745f  ure_flags.smart_
-00009b80: 6465 7465 6374 5f74 7970 6573 0a0a 2020  detect_types..  
-00009b90: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00009ba0: 6465 6620 6973 5f76 6568 6963 6c65 5f64  def is_vehicle_d
-00009bb0: 6574 6563 7469 6f6e 5f6f 6e28 7365 6c66  etection_on(self
-00009bc0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00009bd0: 2020 2022 2222 4973 2056 6568 6963 6c65     """Is Vehicle
-00009be0: 2044 6574 6563 7469 6f6e 2061 7661 696c   Detection avail
-00009bf0: 6162 6c65 2061 6e64 2065 6e61 626c 6564  able and enabled
-00009c00: 2028 6361 6d65 7261 2077 696c 6c20 7072   (camera will pr
-00009c10: 6f64 7563 6520 7665 6869 636c 6520 736d  oduce vehicle sm
-00009c20: 6172 740a 2020 2020 2020 2020 6465 7465  art.        dete
-00009c30: 6374 696f 6e20 6576 656e 7473 293f 0a20  ction events)?. 
-00009c40: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00009c50: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00009c60: 5f69 735f 736d 6172 745f 656e 6162 6c65  _is_smart_enable
-00009c70: 6428 536d 6172 7444 6574 6563 744f 626a  d(SmartDetectObj
-00009c80: 6563 7454 7970 652e 5645 4849 434c 4529  ectType.VEHICLE)
-00009c90: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00009ca0: 2020 2020 6465 6620 6c61 7374 5f76 6568      def last_veh
-00009cb0: 6963 6c65 5f64 6574 6563 745f 6576 656e  icle_detect_even
-00009cc0: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
-00009cd0: 6e61 6c5b 4576 656e 745d 3a0a 2020 2020  nal[Event]:.    
-00009ce0: 2020 2020 2222 2247 6574 2074 6865 206c      """Get the l
-00009cf0: 6173 7420 7665 6869 636c 6520 736d 6172  ast vehicle smar
-00009d00: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
-00009d10: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
-00009d20: 6574 7572 6e20 7365 6c66 2e67 6574 5f6c  eturn self.get_l
-00009d30: 6173 745f 736d 6172 745f 6465 7465 6374  ast_smart_detect
-00009d40: 5f65 7665 6e74 2853 6d61 7274 4465 7465  _event(SmartDete
-00009d50: 6374 4f62 6a65 6374 5479 7065 2e56 4548  ctObjectType.VEH
-00009d60: 4943 4c45 290a 0a20 2020 2040 7072 6f70  ICLE)..    @prop
-00009d70: 6572 7479 0a20 2020 2064 6566 206c 6173  erty.    def las
-00009d80: 745f 7665 6869 636c 655f 6465 7465 6374  t_vehicle_detect
-00009d90: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00009da0: 616c 5b64 6174 6574 696d 655d 3a0a 2020  al[datetime]:.  
-00009db0: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-00009dc0: 206c 6173 7420 7665 6869 636c 6520 736d   last vehicle sm
-00009dd0: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
-00009de0: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-00009df0: 2072 6574 7572 6e20 7365 6c66 2e6c 6173   return self.las
-00009e00: 745f 736d 6172 745f 6465 7465 6374 732e  t_smart_detects.
-00009e10: 6765 7428 536d 6172 7444 6574 6563 744f  get(SmartDetectO
-00009e20: 626a 6563 7454 7970 652e 5645 4849 434c  bjectType.VEHICL
-00009e30: 4529 0a0a 2020 2020 4070 726f 7065 7274  E)..    @propert
-00009e40: 790a 2020 2020 6465 6620 6973 5f76 6568  y.    def is_veh
-00009e50: 6963 6c65 5f63 7572 7265 6e74 6c79 5f64  icle_currently_d
-00009e60: 6574 6563 7465 6428 7365 6c66 2920 2d3e  etected(self) ->
-00009e70: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00009e80: 2222 4973 2076 6568 6963 6c65 2063 7572  ""Is vehicle cur
-00009e90: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
-00009ea0: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
-00009eb0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
-00009ec0: 735f 736d 6172 745f 6465 7465 6374 6564  s_smart_detected
-00009ed0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
-00009ee0: 6374 5479 7065 2e56 4548 4943 4c45 290a  ctType.VEHICLE).
-00009ef0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00009f00: 6574 5f76 6568 6963 6c65 5f64 6574 6563  et_vehicle_detec
-00009f10: 7469 6f6e 2873 656c 662c 2065 6e61 626c  tion(self, enabl
-00009f20: 6564 3a20 626f 6f6c 2920 2d3e 204e 6f6e  ed: bool) -> Non
-00009f30: 653a 0a20 2020 2020 2020 2022 2222 546f  e:.        """To
-00009f40: 6767 6c65 7320 7665 6869 636c 6520 736d  ggles vehicle sm
-00009f50: 6172 7420 6465 7465 6374 696f 6e2e 2052  art detection. R
-00009f60: 6571 7569 7265 7320 6361 6d65 7261 2074  equires camera t
-00009f70: 6f20 6861 7665 2073 6d61 7274 2064 6574  o have smart det
-00009f80: 6563 7469 6f6e 2222 220a 0a20 2020 2020  ection"""..     
-00009f90: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00009fa0: 7365 6c66 2e5f 7365 745f 6f62 6a65 6374  self._set_object
-00009fb0: 5f64 6574 6563 7428 536d 6172 7444 6574  _detect(SmartDet
-00009fc0: 6563 744f 626a 6563 7454 7970 652e 5645  ectObjectType.VE
-00009fd0: 4849 434c 452c 2065 6e61 626c 6564 290a  HICLE, enabled).
-00009fe0: 0a20 2020 2023 206c 6963 656e 7365 2070  .    # license p
-00009ff0: 6c61 7465 0a0a 2020 2020 4070 726f 7065  late..    @prope
-0000a000: 7274 790a 2020 2020 6465 6620 6361 6e5f  rty.    def can_
-0000a010: 6465 7465 6374 5f6c 6963 656e 7365 5f70  detect_license_p
-0000a020: 6c61 7465 2873 656c 6629 202d 3e20 626f  late(self) -> bo
-0000a030: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-0000a040: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
-0000a050: 2053 6d61 7274 4465 7465 6374 4f62 6a65   SmartDetectObje
-0000a060: 6374 5479 7065 2e4c 4943 454e 5345 5f50  ctType.LICENSE_P
-0000a070: 4c41 5445 2069 6e20 7365 6c66 2e66 6561  LATE in self.fea
-0000a080: 7475 7265 5f66 6c61 6773 2e73 6d61 7274  ture_flags.smart
-0000a090: 5f64 6574 6563 745f 7479 7065 730a 2020  _detect_types.  
-0000a0a0: 2020 2020 2020 290a 0a20 2020 2040 7072        )..    @pr
-0000a0b0: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
-0000a0c0: 735f 6c69 6365 6e73 655f 706c 6174 655f  s_license_plate_
-0000a0d0: 6465 7465 6374 696f 6e5f 6f6e 2873 656c  detection_on(sel
-0000a0e0: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-0000a0f0: 2020 2020 2222 2249 7320 4c69 6365 6e73      """Is Licens
-0000a100: 6520 506c 6174 6520 4465 7465 6374 696f  e Plate Detectio
-0000a110: 6e20 6176 6169 6c61 626c 6520 616e 6420  n available and 
-0000a120: 656e 6162 6c65 6420 2863 616d 6572 6120  enabled (camera 
-0000a130: 7769 6c6c 2070 726f 6475 6365 2066 6163  will produce fac
-0000a140: 6520 6c69 6365 6e73 650a 2020 2020 2020  e license.      
-0000a150: 2020 706c 6174 6520 6465 7465 6374 696f    plate detectio
-0000a160: 6e20 6576 656e 7473 293f 0a20 2020 2020  n events)?.     
-0000a170: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-0000a180: 7265 7475 726e 2073 656c 662e 5f69 735f  return self._is_
-0000a190: 736d 6172 745f 656e 6162 6c65 6428 536d  smart_enabled(Sm
-0000a1a0: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
-0000a1b0: 7970 652e 4c49 4345 4e53 455f 504c 4154  ype.LICENSE_PLAT
-0000a1c0: 4529 0a0a 2020 2020 4070 726f 7065 7274  E)..    @propert
-0000a1d0: 790a 2020 2020 6465 6620 6c61 7374 5f6c  y.    def last_l
-0000a1e0: 6963 656e 7365 5f70 6c61 7465 5f64 6574  icense_plate_det
-0000a1f0: 6563 745f 6576 656e 7428 7365 6c66 2920  ect_event(self) 
-0000a200: 2d3e 204f 7074 696f 6e61 6c5b 4576 656e  -> Optional[Even
-0000a210: 745d 3a0a 2020 2020 2020 2020 2222 2247  t]:.        """G
-0000a220: 6574 2074 6865 206c 6173 7420 6c69 6365  et the last lice
-0000a230: 6e73 6520 706c 6174 6520 736d 6172 7420  nse plate smart 
-0000a240: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
-0000a250: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0000a260: 7572 6e20 7365 6c66 2e67 6574 5f6c 6173  urn self.get_las
-0000a270: 745f 736d 6172 745f 6465 7465 6374 5f65  t_smart_detect_e
-0000a280: 7665 6e74 2853 6d61 7274 4465 7465 6374  vent(SmartDetect
-0000a290: 4f62 6a65 6374 5479 7065 2e4c 4943 454e  ObjectType.LICEN
-0000a2a0: 5345 5f50 4c41 5445 290a 0a20 2020 2040  SE_PLATE)..    @
-0000a2b0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000a2c0: 206c 6173 745f 6c69 6365 6e73 655f 706c   last_license_pl
-0000a2d0: 6174 655f 6465 7465 6374 2873 656c 6629  ate_detect(self)
-0000a2e0: 202d 3e20 4f70 7469 6f6e 616c 5b64 6174   -> Optional[dat
-0000a2f0: 6574 696d 655d 3a0a 2020 2020 2020 2020  etime]:.        
-0000a300: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
-0000a310: 6c69 6365 6e73 6520 706c 6174 6520 736d  license plate sm
-0000a320: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
-0000a330: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-0000a340: 2072 6574 7572 6e20 7365 6c66 2e6c 6173   return self.las
-0000a350: 745f 736d 6172 745f 6465 7465 6374 732e  t_smart_detects.
-0000a360: 6765 7428 536d 6172 7444 6574 6563 744f  get(SmartDetectO
-0000a370: 626a 6563 7454 7970 652e 4c49 4345 4e53  bjectType.LICENS
-0000a380: 455f 504c 4154 4529 0a0a 2020 2020 4070  E_PLATE)..    @p
-0000a390: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000a3a0: 6973 5f6c 6963 656e 7365 5f70 6c61 7465  is_license_plate
-0000a3b0: 5f63 7572 7265 6e74 6c79 5f64 6574 6563  _currently_detec
-0000a3c0: 7465 6428 7365 6c66 2920 2d3e 2062 6f6f  ted(self) -> boo
-0000a3d0: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
-0000a3e0: 206c 6963 656e 7365 2070 6c61 7465 2063   license plate c
-0000a3f0: 7572 7265 6e74 6c79 2062 6569 6e67 2064  urrently being d
-0000a400: 6574 6563 7465 6422 2222 0a0a 2020 2020  etected"""..    
-0000a410: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000a420: 5f69 735f 736d 6172 745f 6465 7465 6374  _is_smart_detect
-0000a430: 6564 2853 6d61 7274 4465 7465 6374 4f62  ed(SmartDetectOb
-0000a440: 6a65 6374 5479 7065 2e4c 4943 454e 5345  jectType.LICENSE
-0000a450: 5f50 4c41 5445 290a 0a20 2020 2061 7379  _PLATE)..    asy
-0000a460: 6e63 2064 6566 2073 6574 5f6c 6963 656e  nc def set_licen
-0000a470: 7365 5f70 6c61 7465 5f64 6574 6563 7469  se_plate_detecti
-0000a480: 6f6e 2873 656c 662c 2065 6e61 626c 6564  on(self, enabled
-0000a490: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-0000a4a0: 0a20 2020 2020 2020 2022 2222 546f 6767  .        """Togg
-0000a4b0: 6c65 7320 6c69 6365 6e73 6520 706c 6174  les license plat
-0000a4c0: 6520 736d 6172 7420 6465 7465 6374 696f  e smart detectio
-0000a4d0: 6e2e 2052 6571 7569 7265 7320 6361 6d65  n. Requires came
-0000a4e0: 7261 2074 6f20 6861 7665 2073 6d61 7274  ra to have smart
-0000a4f0: 2064 6574 6563 7469 6f6e 2222 220a 0a20   detection""".. 
-0000a500: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-0000a510: 6169 7420 7365 6c66 2e5f 7365 745f 6f62  ait self._set_ob
-0000a520: 6a65 6374 5f64 6574 6563 7428 0a20 2020  ject_detect(.   
-0000a530: 2020 2020 2020 2020 2053 6d61 7274 4465           SmartDe
-0000a540: 7465 6374 4f62 6a65 6374 5479 7065 2e4c  tectObjectType.L
-0000a550: 4943 454e 5345 5f50 4c41 5445 2c0a 2020  ICENSE_PLATE,.  
-0000a560: 2020 2020 2020 2020 2020 656e 6162 6c65            enable
-0000a570: 642c 0a20 2020 2020 2020 2029 0a0a 2020  d,.        )..  
-0000a580: 2020 2320 7061 636b 6167 650a 0a20 2020    # package..   
-0000a590: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000a5a0: 6566 2063 616e 5f64 6574 6563 745f 7061  ef can_detect_pa
-0000a5b0: 636b 6167 6528 7365 6c66 2920 2d3e 2062  ckage(self) -> b
-0000a5c0: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
-0000a5d0: 7572 6e20 536d 6172 7444 6574 6563 744f  urn SmartDetectO
-0000a5e0: 626a 6563 7454 7970 652e 5041 434b 4147  bjectType.PACKAG
-0000a5f0: 4520 696e 2073 656c 662e 6665 6174 7572  E in self.featur
-0000a600: 655f 666c 6167 732e 736d 6172 745f 6465  e_flags.smart_de
-0000a610: 7465 6374 5f74 7970 6573 0a0a 2020 2020  tect_types..    
-0000a620: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a630: 6620 6973 5f70 6163 6b61 6765 5f64 6574  f is_package_det
-0000a640: 6563 7469 6f6e 5f6f 6e28 7365 6c66 2920  ection_on(self) 
-0000a650: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000a660: 2022 2222 4973 2050 6163 6b61 6765 2044   """Is Package D
-0000a670: 6574 6563 7469 6f6e 2061 7661 696c 6162  etection availab
-0000a680: 6c65 2061 6e64 2065 6e61 626c 6564 2028  le and enabled (
-0000a690: 6361 6d65 7261 2077 696c 6c20 7072 6f64  camera will prod
-0000a6a0: 7563 6520 7061 636b 6167 6520 736d 6172  uce package smar
-0000a6b0: 740a 2020 2020 2020 2020 6465 7465 6374  t.        detect
-0000a6c0: 696f 6e20 6576 656e 7473 293f 0a20 2020  ion events)?.   
-0000a6d0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000a6e0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
-0000a6f0: 735f 736d 6172 745f 656e 6162 6c65 6428  s_smart_enabled(
-0000a700: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
-0000a710: 7454 7970 652e 5041 434b 4147 4529 0a0a  tType.PACKAGE)..
-0000a720: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000a730: 2020 6465 6620 6c61 7374 5f70 6163 6b61    def last_packa
-0000a740: 6765 5f64 6574 6563 745f 6576 656e 7428  ge_detect_event(
-0000a750: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-0000a760: 6c5b 4576 656e 745d 3a0a 2020 2020 2020  l[Event]:.      
-0000a770: 2020 2222 2247 6574 2074 6865 206c 6173    """Get the las
-0000a780: 7420 7061 636b 6167 6520 736d 6172 7420  t package smart 
-0000a790: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
-0000a7a0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0000a7b0: 7572 6e20 7365 6c66 2e67 6574 5f6c 6173  urn self.get_las
-0000a7c0: 745f 736d 6172 745f 6465 7465 6374 5f65  t_smart_detect_e
-0000a7d0: 7665 6e74 2853 6d61 7274 4465 7465 6374  vent(SmartDetect
-0000a7e0: 4f62 6a65 6374 5479 7065 2e50 4143 4b41  ObjectType.PACKA
-0000a7f0: 4745 290a 0a20 2020 2040 7072 6f70 6572  GE)..    @proper
-0000a800: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
-0000a810: 7061 636b 6167 655f 6465 7465 6374 2873  package_detect(s
-0000a820: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-0000a830: 5b64 6174 6574 696d 655d 3a0a 2020 2020  [datetime]:.    
-0000a840: 2020 2020 2222 2247 6574 2074 6865 206c      """Get the l
-0000a850: 6173 7420 7061 636b 6167 6520 736d 6172  ast package smar
-0000a860: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
-0000a870: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
-0000a880: 6574 7572 6e20 7365 6c66 2e6c 6173 745f  eturn self.last_
-0000a890: 736d 6172 745f 6465 7465 6374 732e 6765  smart_detects.ge
-0000a8a0: 7428 536d 6172 7444 6574 6563 744f 626a  t(SmartDetectObj
-0000a8b0: 6563 7454 7970 652e 5041 434b 4147 4529  ectType.PACKAGE)
-0000a8c0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000a8d0: 2020 2020 6465 6620 6973 5f70 6163 6b61      def is_packa
-0000a8e0: 6765 5f63 7572 7265 6e74 6c79 5f64 6574  ge_currently_det
-0000a8f0: 6563 7465 6428 7365 6c66 2920 2d3e 2062  ected(self) -> b
-0000a900: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-0000a910: 4973 2070 6163 6b61 6765 2063 7572 7265  Is package curre
-0000a920: 6e74 6c79 2062 6569 6e67 2064 6574 6563  ntly being detec
-0000a930: 7465 6422 2222 0a0a 2020 2020 2020 2020  ted"""..        
-0000a940: 7265 7475 726e 2073 656c 662e 5f69 735f  return self._is_
-0000a950: 736d 6172 745f 6465 7465 6374 6564 2853  smart_detected(S
-0000a960: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
-0000a970: 5479 7065 2e50 4143 4b41 4745 290a 0a20  Type.PACKAGE).. 
-0000a980: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-0000a990: 5f70 6163 6b61 6765 5f64 6574 6563 7469  _package_detecti
-0000a9a0: 6f6e 2873 656c 662c 2065 6e61 626c 6564  on(self, enabled
-0000a9b0: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-0000a9c0: 0a20 2020 2020 2020 2022 2222 546f 6767  .        """Togg
-0000a9d0: 6c65 7320 7061 636b 6167 6520 736d 6172  les package smar
-0000a9e0: 7420 6465 7465 6374 696f 6e2e 2052 6571  t detection. Req
-0000a9f0: 7569 7265 7320 6361 6d65 7261 2074 6f20  uires camera to 
-0000aa00: 6861 7665 2073 6d61 7274 2064 6574 6563  have smart detec
-0000aa10: 7469 6f6e 2222 220a 0a20 2020 2020 2020  tion"""..       
-0000aa20: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0000aa30: 6c66 2e5f 7365 745f 6f62 6a65 6374 5f64  lf._set_object_d
-0000aa40: 6574 6563 7428 536d 6172 7444 6574 6563  etect(SmartDetec
-0000aa50: 744f 626a 6563 7454 7970 652e 5041 434b  tObjectType.PACK
-0000aa60: 4147 452c 2065 6e61 626c 6564 290a 0a20  AGE, enabled).. 
-0000aa70: 2020 2023 2061 6e69 6d61 6c0a 0a20 2020     # animal..   
-0000aa80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000aa90: 6566 2063 616e 5f64 6574 6563 745f 616e  ef can_detect_an
-0000aaa0: 696d 616c 2873 656c 6629 202d 3e20 626f  imal(self) -> bo
-0000aab0: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-0000aac0: 726e 2053 6d61 7274 4465 7465 6374 4f62  rn SmartDetectOb
-0000aad0: 6a65 6374 5479 7065 2e41 4e49 4d41 4c20  jectType.ANIMAL 
-0000aae0: 696e 2073 656c 662e 6665 6174 7572 655f  in self.feature_
-0000aaf0: 666c 6167 732e 736d 6172 745f 6465 7465  flags.smart_dete
-0000ab00: 6374 5f74 7970 6573 0a0a 2020 2020 4070  ct_types..    @p
-0000ab10: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000ab20: 6973 5f61 6e69 6d61 6c5f 6465 7465 6374  is_animal_detect
-0000ab30: 696f 6e5f 6f6e 2873 656c 6629 202d 3e20  ion_on(self) -> 
-0000ab40: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0000ab50: 2249 7320 416e 696d 616c 2044 6574 6563  "Is Animal Detec
-0000ab60: 7469 6f6e 2061 7661 696c 6162 6c65 2061  tion available a
-0000ab70: 6e64 2065 6e61 626c 6564 2028 6361 6d65  nd enabled (came
-0000ab80: 7261 2077 696c 6c20 7072 6f64 7563 6520  ra will produce 
-0000ab90: 7061 636b 6167 6520 736d 6172 740a 2020  package smart.  
-0000aba0: 2020 2020 2020 6465 7465 6374 696f 6e20        detection 
-0000abb0: 6576 656e 7473 293f 0a20 2020 2020 2020  events)?.       
-0000abc0: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
-0000abd0: 7475 726e 2073 656c 662e 5f69 735f 736d  turn self._is_sm
-0000abe0: 6172 745f 656e 6162 6c65 6428 536d 6172  art_enabled(Smar
-0000abf0: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-0000ac00: 652e 414e 494d 414c 290a 0a20 2020 2040  e.ANIMAL)..    @
-0000ac10: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000ac20: 206c 6173 745f 616e 696d 616c 5f64 6574   last_animal_det
-0000ac30: 6563 745f 6576 656e 7428 7365 6c66 2920  ect_event(self) 
-0000ac40: 2d3e 204f 7074 696f 6e61 6c5b 4576 656e  -> Optional[Even
-0000ac50: 745d 3a0a 2020 2020 2020 2020 2222 2247  t]:.        """G
-0000ac60: 6574 2074 6865 206c 6173 7420 616e 696d  et the last anim
-0000ac70: 616c 2073 6d61 7274 2064 6574 6563 7469  al smart detecti
-0000ac80: 6f6e 2065 7665 6e74 2e22 2222 0a0a 2020  on event."""..  
-0000ac90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000aca0: 662e 6765 745f 6c61 7374 5f73 6d61 7274  f.get_last_smart
-0000acb0: 5f64 6574 6563 745f 6576 656e 7428 536d  _detect_event(Sm
-0000acc0: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
-0000acd0: 7970 652e 414e 494d 414c 290a 0a20 2020  ype.ANIMAL)..   
-0000ace0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000acf0: 6566 206c 6173 745f 616e 696d 616c 5f64  ef last_animal_d
-0000ad00: 6574 6563 7428 7365 6c66 2920 2d3e 204f  etect(self) -> O
-0000ad10: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
-0000ad20: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-0000ad30: 7420 7468 6520 6c61 7374 2061 6e69 6d61  t the last anima
-0000ad40: 6c20 736d 6172 7420 6465 7465 6374 696f  l smart detectio
-0000ad50: 6e20 6576 656e 742e 2222 220a 0a20 2020  n event."""..   
-0000ad60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000ad70: 2e6c 6173 745f 736d 6172 745f 6465 7465  .last_smart_dete
-0000ad80: 6374 732e 6765 7428 536d 6172 7444 6574  cts.get(SmartDet
-0000ad90: 6563 744f 626a 6563 7454 7970 652e 414e  ectObjectType.AN
-0000ada0: 494d 414c 290a 0a20 2020 2040 7072 6f70  IMAL)..    @prop
-0000adb0: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
-0000adc0: 616e 696d 616c 5f63 7572 7265 6e74 6c79  animal_currently
-0000add0: 5f64 6574 6563 7465 6428 7365 6c66 2920  _detected(self) 
-0000ade0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000adf0: 2022 2222 4973 2061 6e69 6d61 6c20 6375   """Is animal cu
-0000ae00: 7272 656e 746c 7920 6265 696e 6720 6465  rrently being de
-0000ae10: 7465 6374 6564 2222 220a 0a20 2020 2020  tected"""..     
-0000ae20: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000ae30: 6973 5f73 6d61 7274 5f64 6574 6563 7465  is_smart_detecte
-0000ae40: 6428 536d 6172 7444 6574 6563 744f 626a  d(SmartDetectObj
-0000ae50: 6563 7454 7970 652e 414e 494d 414c 290a  ectType.ANIMAL).
-0000ae60: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-0000ae70: 6574 5f61 6e69 6d61 6c5f 6465 7465 6374  et_animal_detect
-0000ae80: 696f 6e28 7365 6c66 2c20 656e 6162 6c65  ion(self, enable
-0000ae90: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-0000aea0: 3a0a 2020 2020 2020 2020 2222 2254 6f67  :.        """Tog
-0000aeb0: 676c 6573 2061 6e69 6d61 6c20 736d 6172  gles animal smar
-0000aec0: 7420 6465 7465 6374 696f 6e2e 2052 6571  t detection. Req
-0000aed0: 7569 7265 7320 6361 6d65 7261 2074 6f20  uires camera to 
-0000aee0: 6861 7665 2073 6d61 7274 2064 6574 6563  have smart detec
-0000aef0: 7469 6f6e 2222 220a 0a20 2020 2020 2020  tion"""..       
-0000af00: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0000af10: 6c66 2e5f 7365 745f 6f62 6a65 6374 5f64  lf._set_object_d
-0000af20: 6574 6563 7428 536d 6172 7444 6574 6563  etect(SmartDetec
-0000af30: 744f 626a 6563 7454 7970 652e 414e 494d  tObjectType.ANIM
-0000af40: 414c 2c20 656e 6162 6c65 6429 0a0a 2020  AL, enabled)..  
-0000af50: 2020 2320 6175 6469 6f20 736d 6172 7420    # audio smart 
-0000af60: 6465 7465 6374 696f 6e73 0a0a 2020 2020  detections..    
-0000af70: 6465 6620 5f63 616e 5f64 6574 6563 745f  def _can_detect_
-0000af80: 6175 6469 6f28 7365 6c66 2c20 736d 6172  audio(self, smar
-0000af90: 745f 7479 7065 3a20 536d 6172 7444 6574  t_type: SmartDet
-0000afa0: 6563 744f 626a 6563 7454 7970 6529 202d  ectObjectType) -
-0000afb0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000afc0: 6175 6469 6f5f 7479 7065 203d 2073 6d61  audio_type = sma
-0000afd0: 7274 5f74 7970 652e 6175 6469 6f5f 7479  rt_type.audio_ty
-0000afe0: 7065 0a20 2020 2020 2020 2072 6574 7572  pe.        retur
-0000aff0: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-0000b000: 6175 6469 6f5f 7479 7065 2069 7320 6e6f  audio_type is no
-0000b010: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-0000b020: 2020 2061 6e64 2073 656c 662e 6665 6174     and self.feat
-0000b030: 7572 655f 666c 6167 732e 736d 6172 745f  ure_flags.smart_
-0000b040: 6465 7465 6374 5f61 7564 696f 5f74 7970  detect_audio_typ
-0000b050: 6573 2069 7320 6e6f 7420 4e6f 6e65 0a20  es is not None. 
-0000b060: 2020 2020 2020 2020 2020 2061 6e64 2061             and a
-0000b070: 7564 696f 5f74 7970 6520 696e 2073 656c  udio_type in sel
-0000b080: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
-0000b090: 736d 6172 745f 6465 7465 6374 5f61 7564  smart_detect_aud
-0000b0a0: 696f 5f74 7970 6573 0a20 2020 2020 2020  io_types.       
-0000b0b0: 2029 0a0a 2020 2020 6465 6620 5f69 735f   )..    def _is_
-0000b0c0: 6175 6469 6f5f 656e 6162 6c65 6428 7365  audio_enabled(se
-0000b0d0: 6c66 2c20 736d 6172 745f 7479 7065 3a20  lf, smart_type: 
-0000b0e0: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
-0000b0f0: 7454 7970 6529 202d 3e20 626f 6f6c 3a0a  tType) -> bool:.
-0000b100: 2020 2020 2020 2020 6175 6469 6f5f 7479          audio_ty
-0000b110: 7065 203d 2073 6d61 7274 5f74 7970 652e  pe = smart_type.
-0000b120: 6175 6469 6f5f 7479 7065 0a20 2020 2020  audio_type.     
-0000b130: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-0000b140: 2020 2020 2020 2020 6175 6469 6f5f 7479          audio_ty
-0000b150: 7065 2069 7320 6e6f 7420 4e6f 6e65 0a20  pe is not None. 
-0000b160: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
-0000b170: 656c 662e 6973 5f72 6563 6f72 6469 6e67  elf.is_recording
-0000b180: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
-0000b190: 2020 2020 2061 6e64 2073 656c 662e 6665       and self.fe
-0000b1a0: 6174 7572 655f 666c 6167 732e 736d 6172  ature_flags.smar
-0000b1b0: 745f 6465 7465 6374 5f61 7564 696f 5f74  t_detect_audio_t
-0000b1c0: 7970 6573 2069 7320 6e6f 7420 4e6f 6e65  ypes is not None
-0000b1d0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0000b1e0: 2073 656c 662e 736d 6172 745f 6465 7465   self.smart_dete
-0000b1f0: 6374 5f73 6574 7469 6e67 732e 6175 6469  ct_settings.audi
-0000b200: 6f5f 7479 7065 7320 6973 206e 6f74 204e  o_types is not N
-0000b210: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000b220: 616e 6420 6175 6469 6f5f 7479 7065 2069  and audio_type i
-0000b230: 6e20 7365 6c66 2e73 6d61 7274 5f64 6574  n self.smart_det
-0000b240: 6563 745f 7365 7474 696e 6773 2e61 7564  ect_settings.aud
-0000b250: 696f 5f74 7970 6573 0a20 2020 2020 2020  io_types.       
-0000b260: 2029 0a0a 2020 2020 6465 6620 5f69 735f   )..    def _is_
-0000b270: 6175 6469 6f5f 6465 7465 6374 6564 2873  audio_detected(s
-0000b280: 656c 662c 2073 6d61 7274 5f74 7970 653a  elf, smart_type:
-0000b290: 2053 6d61 7274 4465 7465 6374 4f62 6a65   SmartDetectObje
-0000b2a0: 6374 5479 7065 2920 2d3e 2062 6f6f 6c3a  ctType) -> bool:
-0000b2b0: 0a20 2020 2020 2020 2061 7564 696f 5f74  .        audio_t
-0000b2c0: 7970 6520 3d20 736d 6172 745f 7479 7065  ype = smart_type
-0000b2d0: 2e61 7564 696f 5f74 7970 650a 2020 2020  .audio_type.    
-0000b2e0: 2020 2020 6966 2061 7564 696f 5f74 7970      if audio_typ
-0000b2f0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-0000b300: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0000b310: 6c73 650a 0a20 2020 2020 2020 2065 7665  lse..        eve
-0000b320: 6e74 203d 2073 656c 662e 6765 745f 6c61  nt = self.get_la
-0000b330: 7374 5f73 6d61 7274 5f61 7564 696f 5f64  st_smart_audio_d
-0000b340: 6574 6563 745f 6576 656e 7428 6175 6469  etect_event(audi
-0000b350: 6f5f 7479 7065 290a 2020 2020 2020 2020  o_type).        
-0000b360: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
-0000b370: 2020 2020 2073 656c 662e 5f69 735f 6175       self._is_au
-0000b380: 6469 6f5f 656e 6162 6c65 6428 736d 6172  dio_enabled(smar
-0000b390: 745f 7479 7065 290a 2020 2020 2020 2020  t_type).        
-0000b3a0: 2020 2020 616e 6420 6576 656e 7420 6973      and event is
-0000b3b0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-0000b3c0: 2020 2020 2020 616e 6420 6576 656e 742e        and event.
-0000b3d0: 656e 6420 6973 204e 6f6e 650a 2020 2020  end is None.    
-0000b3e0: 2020 2020 2020 2020 616e 6420 736d 6172          and smar
-0000b3f0: 745f 7479 7065 2069 6e20 6576 656e 742e  t_type in event.
-0000b400: 736d 6172 745f 6465 7465 6374 5f74 7970  smart_detect_typ
-0000b410: 6573 0a20 2020 2020 2020 2029 0a0a 2020  es.        )..  
-0000b420: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000b430: 6465 6620 6973 5f61 7564 696f 5f63 7572  def is_audio_cur
-0000b440: 7265 6e74 6c79 5f64 6574 6563 7465 6428  rently_detected(
-0000b450: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000b460: 2020 2020 2020 2022 2222 4973 2061 7564         """Is aud
-0000b470: 696f 2064 6574 6563 7469 6f6e 2063 7572  io detection cur
-0000b480: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
-0000b490: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
-0000b4a0: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-0000b4b0: 2020 2020 2020 2073 656c 662e 6973 5f72         self.is_r
-0000b4c0: 6563 6f72 6469 6e67 5f65 6e61 626c 6564  ecording_enabled
-0000b4d0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0000b4e0: 2062 6f6f 6c28 7365 6c66 2e73 6d61 7274   bool(self.smart
-0000b4f0: 5f64 6574 6563 745f 7365 7474 696e 6773  _detect_settings
-0000b500: 2e61 7564 696f 5f74 7970 6573 290a 2020  .audio_types).  
-0000b510: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-0000b520: 6c66 2e6c 6173 745f 736d 6172 745f 6175  lf.last_smart_au
-0000b530: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
-0000b540: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000b550: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-0000b560: 662e 6c61 7374 5f73 6d61 7274 5f61 7564  f.last_smart_aud
-0000b570: 696f 5f64 6574 6563 745f 6576 656e 742e  io_detect_event.
-0000b580: 656e 6420 6973 204e 6f6e 650a 2020 2020  end is None.    
-0000b590: 2020 2020 290a 0a20 2020 2023 2073 6d6f      )..    # smo
-0000b5a0: 6b65 2061 6c61 726d 0a0a 2020 2020 4070  ke alarm..    @p
-0000b5b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000b5c0: 6361 6e5f 6465 7465 6374 5f73 6d6f 6b65  can_detect_smoke
-0000b5d0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-0000b5e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000b5f0: 656c 662e 5f63 616e 5f64 6574 6563 745f  elf._can_detect_
-0000b600: 6175 6469 6f28 536d 6172 7444 6574 6563  audio(SmartDetec
-0000b610: 744f 626a 6563 7454 7970 652e 534d 4f4b  tObjectType.SMOK
-0000b620: 4529 0a0a 2020 2020 4070 726f 7065 7274  E)..    @propert
-0000b630: 790a 2020 2020 6465 6620 6973 5f73 6d6f  y.    def is_smo
-0000b640: 6b65 5f64 6574 6563 7469 6f6e 5f6f 6e28  ke_detection_on(
-0000b650: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000b660: 2020 2020 2020 2022 2222 4973 2053 6d6f         """Is Smo
-0000b670: 6b65 2041 6c61 726d 2044 6574 6563 7469  ke Alarm Detecti
-0000b680: 6f6e 2061 7661 696c 6162 6c65 2061 6e64  on available and
-0000b690: 2065 6e61 626c 6564 2028 6361 6d65 7261   enabled (camera
-0000b6a0: 2077 696c 6c20 7072 6f64 7563 6520 736d   will produce sm
-0000b6b0: 6f6b 650a 2020 2020 2020 2020 736d 6172  oke.        smar
-0000b6c0: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
-0000b6d0: 7473 293f 0a20 2020 2020 2020 2022 2222  ts)?.        """
-0000b6e0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000b6f0: 2073 656c 662e 5f69 735f 6175 6469 6f5f   self._is_audio_
-0000b700: 656e 6162 6c65 6428 536d 6172 7444 6574  enabled(SmartDet
-0000b710: 6563 744f 626a 6563 7454 7970 652e 534d  ectObjectType.SM
-0000b720: 4f4b 4529 0a0a 2020 2020 4070 726f 7065  OKE)..    @prope
-0000b730: 7274 790a 2020 2020 6465 6620 6c61 7374  rty.    def last
-0000b740: 5f73 6d6f 6b65 5f64 6574 6563 745f 6576  _smoke_detect_ev
-0000b750: 656e 7428 7365 6c66 2920 2d3e 204f 7074  ent(self) -> Opt
-0000b760: 696f 6e61 6c5b 4576 656e 745d 3a0a 2020  ional[Event]:.  
-0000b770: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-0000b780: 206c 6173 7420 7065 7273 6f6e 2073 6d61   last person sma
-0000b790: 7274 2064 6574 6563 7469 6f6e 2065 7665  rt detection eve
-0000b7a0: 6e74 2e22 2222 0a0a 2020 2020 2020 2020  nt."""..        
-0000b7b0: 7265 7475 726e 2073 656c 662e 6765 745f  return self.get_
-0000b7c0: 6c61 7374 5f73 6d61 7274 5f61 7564 696f  last_smart_audio
-0000b7d0: 5f64 6574 6563 745f 6576 656e 7428 536d  _detect_event(Sm
-0000b7e0: 6172 7444 6574 6563 7441 7564 696f 5479  artDetectAudioTy
-0000b7f0: 7065 2e53 4d4f 4b45 290a 0a20 2020 2040  pe.SMOKE)..    @
-0000b800: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000b810: 206c 6173 745f 736d 6f6b 655f 6465 7465   last_smoke_dete
-0000b820: 6374 2873 656c 6629 202d 3e20 4f70 7469  ct(self) -> Opti
-0000b830: 6f6e 616c 5b64 6174 6574 696d 655d 3a0a  onal[datetime]:.
-0000b840: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-0000b850: 6865 206c 6173 7420 736d 6f6b 6520 736d  he last smoke sm
-0000b860: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
-0000b870: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-0000b880: 2072 6574 7572 6e20 7365 6c66 2e6c 6173   return self.las
-0000b890: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
-0000b8a0: 7465 6374 732e 6765 7428 536d 6172 7444  tects.get(SmartD
-0000b8b0: 6574 6563 7441 7564 696f 5479 7065 2e53  etectAudioType.S
-0000b8c0: 4d4f 4b45 290a 0a20 2020 2040 7072 6f70  MOKE)..    @prop
-0000b8d0: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
-0000b8e0: 736d 6f6b 655f 6375 7272 656e 746c 795f  smoke_currently_
-0000b8f0: 6465 7465 6374 6564 2873 656c 6629 202d  detected(self) -
-0000b900: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000b910: 2222 2249 7320 736d 6f6b 6520 616c 6172  """Is smoke alar
-0000b920: 6d20 6375 7272 656e 746c 7920 6265 696e  m currently bein
-0000b930: 6720 6465 7465 6374 6564 2222 220a 0a20  g detected""".. 
-0000b940: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000b950: 6c66 2e5f 6973 5f61 7564 696f 5f64 6574  lf._is_audio_det
-0000b960: 6563 7465 6428 536d 6172 7444 6574 6563  ected(SmartDetec
-0000b970: 744f 626a 6563 7454 7970 652e 534d 4f4b  tObjectType.SMOK
-0000b980: 4529 0a0a 2020 2020 6173 796e 6320 6465  E)..    async de
-0000b990: 6620 7365 745f 736d 6f6b 655f 6465 7465  f set_smoke_dete
-0000b9a0: 6374 696f 6e28 7365 6c66 2c20 656e 6162  ction(self, enab
-0000b9b0: 6c65 643a 2062 6f6f 6c29 202d 3e20 4e6f  led: bool) -> No
-0000b9c0: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
-0000b9d0: 6f67 676c 6573 2073 6d6f 6b65 2073 6d61  oggles smoke sma
-0000b9e0: 7274 2064 6574 6563 7469 6f6e 2e20 5265  rt detection. Re
-0000b9f0: 7175 6972 6573 2063 616d 6572 6120 746f  quires camera to
-0000ba00: 2068 6176 6520 736d 6172 7420 6465 7465   have smart dete
-0000ba10: 6374 696f 6e22 2222 0a0a 2020 2020 2020  ction"""..      
-0000ba20: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-0000ba30: 656c 662e 5f73 6574 5f61 7564 696f 5f64  elf._set_audio_d
-0000ba40: 6574 6563 7428 536d 6172 7444 6574 6563  etect(SmartDetec
-0000ba50: 7441 7564 696f 5479 7065 2e53 4d4f 4b45  tAudioType.SMOKE
-0000ba60: 2c20 656e 6162 6c65 6429 0a0a 2020 2020  , enabled)..    
-0000ba70: 2320 636f 2061 6c61 726d 0a0a 2020 2020  # co alarm..    
-0000ba80: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000ba90: 6620 6361 6e5f 6465 7465 6374 5f63 6f28  f can_detect_co(
-0000baa0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000bab0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000bac0: 6c66 2e5f 6361 6e5f 6465 7465 6374 5f61  lf._can_detect_a
-0000bad0: 7564 696f 2853 6d61 7274 4465 7465 6374  udio(SmartDetect
-0000bae0: 4f62 6a65 6374 5479 7065 2e43 4d4f 4e58  ObjectType.CMONX
-0000baf0: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-0000bb00: 0a20 2020 2064 6566 2069 735f 636f 5f64  .    def is_co_d
-0000bb10: 6574 6563 7469 6f6e 5f6f 6e28 7365 6c66  etection_on(self
-0000bb20: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-0000bb30: 2020 2022 2222 4973 2043 4f20 416c 6172     """Is CO Alar
-0000bb40: 6d20 4465 7465 6374 696f 6e20 6176 6169  m Detection avai
-0000bb50: 6c61 626c 6520 616e 6420 656e 6162 6c65  lable and enable
-0000bb60: 6420 2863 616d 6572 6120 7769 6c6c 2070  d (camera will p
-0000bb70: 726f 6475 6365 2073 6d6f 6b65 2073 6d61  roduce smoke sma
-0000bb80: 7274 0a20 2020 2020 2020 2064 6574 6563  rt.        detec
-0000bb90: 7469 6f6e 2065 7665 6e74 7329 3f0a 2020  tion events)?.  
-0000bba0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000bbb0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000bbc0: 6973 5f61 7564 696f 5f65 6e61 626c 6564  is_audio_enabled
-0000bbd0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
-0000bbe0: 6374 5479 7065 2e43 4d4f 4e58 290a 0a20  ctType.CMONX).. 
-0000bbf0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000bc00: 2064 6566 206c 6173 745f 636d 6f6e 785f   def last_cmonx_
-0000bc10: 6465 7465 6374 5f65 7665 6e74 2873 656c  detect_event(sel
-0000bc20: 6629 202d 3e20 4f70 7469 6f6e 616c 5b45  f) -> Optional[E
-0000bc30: 7665 6e74 5d3a 0a20 2020 2020 2020 2022  vent]:.        "
-0000bc40: 2222 4765 7420 7468 6520 6c61 7374 2043  ""Get the last C
-0000bc50: 4f20 616c 6172 6d20 736d 6172 7420 6465  O alarm smart de
-0000bc60: 7465 6374 696f 6e20 6576 656e 742e 2222  tection event.""
-0000bc70: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000bc80: 6e20 7365 6c66 2e67 6574 5f6c 6173 745f  n self.get_last_
-0000bc90: 736d 6172 745f 6175 6469 6f5f 6465 7465  smart_audio_dete
-0000bca0: 6374 5f65 7665 6e74 2853 6d61 7274 4465  ct_event(SmartDe
-0000bcb0: 7465 6374 4175 6469 6f54 7970 652e 434d  tectAudioType.CM
-0000bcc0: 4f4e 5829 0a0a 2020 2020 4070 726f 7065  ONX)..    @prope
-0000bcd0: 7274 790a 2020 2020 6465 6620 6c61 7374  rty.    def last
-0000bce0: 5f63 6d6f 6e78 5f64 6574 6563 7428 7365  _cmonx_detect(se
-0000bcf0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-0000bd00: 6461 7465 7469 6d65 5d3a 0a20 2020 2020  datetime]:.     
-0000bd10: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
-0000bd20: 7374 2043 4f20 616c 6172 6d20 736d 6172  st CO alarm smar
-0000bd30: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
-0000bd40: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
-0000bd50: 6574 7572 6e20 7365 6c66 2e6c 6173 745f  eturn self.last_
-0000bd60: 736d 6172 745f 6175 6469 6f5f 6465 7465  smart_audio_dete
-0000bd70: 6374 732e 6765 7428 536d 6172 7444 6574  cts.get(SmartDet
-0000bd80: 6563 7441 7564 696f 5479 7065 2e43 4d4f  ectAudioType.CMO
-0000bd90: 4e58 290a 0a20 2020 2040 7072 6f70 6572  NX)..    @proper
-0000bda0: 7479 0a20 2020 2064 6566 2069 735f 636d  ty.    def is_cm
-0000bdb0: 6f6e 785f 6375 7272 656e 746c 795f 6465  onx_currently_de
-0000bdc0: 7465 6374 6564 2873 656c 6629 202d 3e20  tected(self) -> 
-0000bdd0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0000bde0: 2249 7320 434f 2061 6c61 726d 2063 7572  "Is CO alarm cur
-0000bdf0: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
-0000be00: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
-0000be10: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
-0000be20: 735f 6175 6469 6f5f 6465 7465 6374 6564  s_audio_detected
-0000be30: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
-0000be40: 6374 5479 7065 2e43 4d4f 4e58 290a 0a20  ctType.CMONX).. 
-0000be50: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-0000be60: 5f63 6d6f 6e78 5f64 6574 6563 7469 6f6e  _cmonx_detection
-0000be70: 2873 656c 662c 2065 6e61 626c 6564 3a20  (self, enabled: 
-0000be80: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-0000be90: 2020 2020 2020 2022 2222 546f 6767 6c65         """Toggle
-0000bea0: 7320 736d 6f6b 6520 736d 6172 7420 6465  s smoke smart de
-0000beb0: 7465 6374 696f 6e2e 2052 6571 7569 7265  tection. Require
-0000bec0: 7320 6361 6d65 7261 2074 6f20 6861 7665  s camera to have
-0000bed0: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
-0000bee0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0000bef0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-0000bf00: 7365 745f 6175 6469 6f5f 6465 7465 6374  set_audio_detect
-0000bf10: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
-0000bf20: 6f54 7970 652e 434d 4f4e 582c 2065 6e61  oType.CMONX, ena
-0000bf30: 626c 6564 290a 0a20 2020 2023 2073 6972  bled)..    # sir
-0000bf40: 656e 0a0a 2020 2020 4070 726f 7065 7274  en..    @propert
-0000bf50: 790a 2020 2020 6465 6620 6361 6e5f 6465  y.    def can_de
-0000bf60: 7465 6374 5f73 6972 656e 2873 656c 6629  tect_siren(self)
-0000bf70: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000bf80: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-0000bf90: 616e 5f64 6574 6563 745f 6175 6469 6f28  an_detect_audio(
-0000bfa0: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
-0000bfb0: 7454 7970 652e 5349 5245 4e29 0a0a 2020  tType.SIREN)..  
-0000bfc0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000bfd0: 6465 6620 6973 5f73 6972 656e 5f64 6574  def is_siren_det
-0000bfe0: 6563 7469 6f6e 5f6f 6e28 7365 6c66 2920  ection_on(self) 
-0000bff0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000c000: 2022 2222 4973 2053 6972 656e 2044 6574   """Is Siren Det
-0000c010: 6563 7469 6f6e 2061 7661 696c 6162 6c65  ection available
-0000c020: 2061 6e64 2065 6e61 626c 6564 2028 6361   and enabled (ca
-0000c030: 6d65 7261 2077 696c 6c20 7072 6f64 7563  mera will produc
-0000c040: 6520 7369 7265 6e20 736d 6172 740a 2020  e siren smart.  
-0000c050: 2020 2020 2020 6465 7465 6374 696f 6e20        detection 
-0000c060: 6576 656e 7473 293f 0a20 2020 2020 2020  events)?.       
-0000c070: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
-0000c080: 7475 726e 2073 656c 662e 5f69 735f 6175  turn self._is_au
-0000c090: 6469 6f5f 656e 6162 6c65 6428 536d 6172  dio_enabled(Smar
-0000c0a0: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-0000c0b0: 652e 5349 5245 4e29 0a0a 2020 2020 4070  e.SIREN)..    @p
-0000c0c0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000c0d0: 6c61 7374 5f73 6972 656e 5f64 6574 6563  last_siren_detec
-0000c0e0: 745f 6576 656e 7428 7365 6c66 2920 2d3e  t_event(self) ->
-0000c0f0: 204f 7074 696f 6e61 6c5b 4576 656e 745d   Optional[Event]
-0000c100: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0000c110: 2074 6865 206c 6173 7420 5369 7265 6e20   the last Siren 
-0000c120: 736d 6172 7420 6465 7465 6374 696f 6e20  smart detection 
-0000c130: 6576 656e 742e 2222 220a 0a20 2020 2020  event."""..     
-0000c140: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0000c150: 6574 5f6c 6173 745f 736d 6172 745f 6175  et_last_smart_au
-0000c160: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
-0000c170: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
-0000c180: 6f54 7970 652e 5349 5245 4e29 0a0a 2020  oType.SIREN)..  
-0000c190: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000c1a0: 6465 6620 6c61 7374 5f73 6972 656e 5f64  def last_siren_d
-0000c1b0: 6574 6563 7428 7365 6c66 2920 2d3e 204f  etect(self) -> O
-0000c1c0: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
-0000c1d0: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-0000c1e0: 7420 7468 6520 6c61 7374 2053 6972 656e  t the last Siren
-0000c1f0: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
-0000c200: 2065 7665 6e74 2e22 2222 0a0a 2020 2020   event."""..    
-0000c210: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000c220: 6c61 7374 5f73 6d61 7274 5f61 7564 696f  last_smart_audio
-0000c230: 5f64 6574 6563 7473 2e67 6574 2853 6d61  _detects.get(Sma
-0000c240: 7274 4465 7465 6374 4175 6469 6f54 7970  rtDetectAudioTyp
-0000c250: 652e 5349 5245 4e29 0a0a 2020 2020 4070  e.SIREN)..    @p
-0000c260: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000c270: 6973 5f73 6972 656e 5f63 7572 7265 6e74  is_siren_current
-0000c280: 6c79 5f64 6574 6563 7465 6428 7365 6c66  ly_detected(self
-0000c290: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-0000c2a0: 2020 2022 2222 4973 2053 6972 656e 2063     """Is Siren c
-0000c2b0: 7572 7265 6e74 6c79 2062 6569 6e67 2064  urrently being d
-0000c2c0: 6574 6563 7465 6422 2222 0a0a 2020 2020  etected"""..    
-0000c2d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000c2e0: 5f69 735f 6175 6469 6f5f 6465 7465 6374  _is_audio_detect
-0000c2f0: 6564 2853 6d61 7274 4465 7465 6374 4f62  ed(SmartDetectOb
-0000c300: 6a65 6374 5479 7065 2e53 4952 454e 290a  jectType.SIREN).
-0000c310: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-0000c320: 6574 5f73 6972 656e 5f64 6574 6563 7469  et_siren_detecti
-0000c330: 6f6e 2873 656c 662c 2065 6e61 626c 6564  on(self, enabled
-0000c340: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-0000c350: 0a20 2020 2020 2020 2022 2222 546f 6767  .        """Togg
-0000c360: 6c65 7320 7369 7265 6e20 736d 6172 7420  les siren smart 
-0000c370: 6465 7465 6374 696f 6e2e 2052 6571 7569  detection. Requi
-0000c380: 7265 7320 6361 6d65 7261 2074 6f20 6861  res camera to ha
-0000c390: 7665 2073 6d61 7274 2064 6574 6563 7469  ve smart detecti
-0000c3a0: 6f6e 2222 220a 0a20 2020 2020 2020 2072  on"""..        r
-0000c3b0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0000c3c0: 2e5f 7365 745f 6175 6469 6f5f 6465 7465  ._set_audio_dete
-0000c3d0: 6374 2853 6d61 7274 4465 7465 6374 4175  ct(SmartDetectAu
-0000c3e0: 6469 6f54 7970 652e 5349 5245 4e2c 2065  dioType.SIREN, e
-0000c3f0: 6e61 626c 6564 290a 0a20 2020 2023 2062  nabled)..    # b
-0000c400: 6162 7920 6372 790a 0a20 2020 2040 7072  aby cry..    @pr
-0000c410: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-0000c420: 616e 5f64 6574 6563 745f 6261 6279 5f63  an_detect_baby_c
-0000c430: 7279 2873 656c 6629 202d 3e20 626f 6f6c  ry(self) -> bool
-0000c440: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000c450: 2073 656c 662e 5f63 616e 5f64 6574 6563   self._can_detec
-0000c460: 745f 6175 6469 6f28 536d 6172 7444 6574  t_audio(SmartDet
-0000c470: 6563 744f 626a 6563 7454 7970 652e 4241  ectObjectType.BA
-0000c480: 4259 5f43 5259 290a 0a20 2020 2040 7072  BY_CRY)..    @pr
-0000c490: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
-0000c4a0: 735f 6261 6279 5f63 7279 5f64 6574 6563  s_baby_cry_detec
-0000c4b0: 7469 6f6e 5f6f 6e28 7365 6c66 2920 2d3e  tion_on(self) ->
-0000c4c0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-0000c4d0: 2222 4973 2042 6162 7920 4372 7920 4465  ""Is Baby Cry De
-0000c4e0: 7465 6374 696f 6e20 6176 6169 6c61 626c  tection availabl
-0000c4f0: 6520 616e 6420 656e 6162 6c65 6420 2863  e and enabled (c
-0000c500: 616d 6572 6120 7769 6c6c 2070 726f 6475  amera will produ
-0000c510: 6365 2062 6162 7920 6372 7920 736d 6172  ce baby cry smar
-0000c520: 740a 2020 2020 2020 2020 6465 7465 6374  t.        detect
-0000c530: 696f 6e20 6576 656e 7473 293f 0a20 2020  ion events)?.   
-0000c540: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000c550: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
-0000c560: 735f 6175 6469 6f5f 656e 6162 6c65 6428  s_audio_enabled(
-0000c570: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
-0000c580: 7454 7970 652e 4241 4259 5f43 5259 290a  tType.BABY_CRY).
-0000c590: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000c5a0: 2020 2064 6566 206c 6173 745f 6261 6279     def last_baby
-0000c5b0: 5f63 7279 5f64 6574 6563 745f 6576 656e  _cry_detect_even
-0000c5c0: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
-0000c5d0: 6e61 6c5b 4576 656e 745d 3a0a 2020 2020  nal[Event]:.    
-0000c5e0: 2020 2020 2222 2247 6574 2074 6865 206c      """Get the l
-0000c5f0: 6173 7420 4261 6279 2043 7279 2073 6d61  ast Baby Cry sma
-0000c600: 7274 2064 6574 6563 7469 6f6e 2065 7665  rt detection eve
-0000c610: 6e74 2e22 2222 0a0a 2020 2020 2020 2020  nt."""..        
-0000c620: 7265 7475 726e 2073 656c 662e 6765 745f  return self.get_
-0000c630: 6c61 7374 5f73 6d61 7274 5f61 7564 696f  last_smart_audio
-0000c640: 5f64 6574 6563 745f 6576 656e 7428 536d  _detect_event(Sm
-0000c650: 6172 7444 6574 6563 7441 7564 696f 5479  artDetectAudioTy
-0000c660: 7065 2e42 4142 595f 4352 5929 0a0a 2020  pe.BABY_CRY)..  
-0000c670: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000c680: 6465 6620 6c61 7374 5f62 6162 795f 6372  def last_baby_cr
-0000c690: 795f 6465 7465 6374 2873 656c 6629 202d  y_detect(self) -
-0000c6a0: 3e20 4f70 7469 6f6e 616c 5b64 6174 6574  > Optional[datet
-0000c6b0: 696d 655d 3a0a 2020 2020 2020 2020 2222  ime]:.        ""
-0000c6c0: 2247 6574 2074 6865 206c 6173 7420 4261  "Get the last Ba
-0000c6d0: 6279 2043 7279 2073 6d61 7274 2064 6574  by Cry smart det
-0000c6e0: 6563 7469 6f6e 2065 7665 6e74 2e22 2222  ection event."""
-0000c6f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000c700: 2073 656c 662e 6c61 7374 5f73 6d61 7274   self.last_smart
-0000c710: 5f61 7564 696f 5f64 6574 6563 7473 2e67  _audio_detects.g
-0000c720: 6574 2853 6d61 7274 4465 7465 6374 4175  et(SmartDetectAu
-0000c730: 6469 6f54 7970 652e 4241 4259 5f43 5259  dioType.BABY_CRY
-0000c740: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-0000c750: 0a20 2020 2064 6566 2069 735f 6261 6279  .    def is_baby
-0000c760: 5f63 7279 5f63 7572 7265 6e74 6c79 5f64  _cry_currently_d
-0000c770: 6574 6563 7465 6428 7365 6c66 2920 2d3e  etected(self) ->
-0000c780: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-0000c790: 2222 4973 2042 6162 7920 4372 7920 6375  ""Is Baby Cry cu
-0000c7a0: 7272 656e 746c 7920 6265 696e 6720 6465  rrently being de
-0000c7b0: 7465 6374 6564 2222 220a 0a20 2020 2020  tected"""..     
-0000c7c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000c7d0: 6973 5f61 7564 696f 5f64 6574 6563 7465  is_audio_detecte
-0000c7e0: 6428 536d 6172 7444 6574 6563 744f 626a  d(SmartDetectObj
-0000c7f0: 6563 7454 7970 652e 4241 4259 5f43 5259  ectType.BABY_CRY
-0000c800: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-0000c810: 2073 6574 5f62 6162 795f 6372 795f 6465   set_baby_cry_de
-0000c820: 7465 6374 696f 6e28 7365 6c66 2c20 656e  tection(self, en
-0000c830: 6162 6c65 643a 2062 6f6f 6c29 202d 3e20  abled: bool) -> 
-0000c840: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000c850: 2254 6f67 676c 6573 2062 6162 795f 6372  "Toggles baby_cr
-0000c860: 7920 736d 6172 7420 6465 7465 6374 696f  y smart detectio
-0000c870: 6e2e 2052 6571 7569 7265 7320 6361 6d65  n. Requires came
-0000c880: 7261 2074 6f20 6861 7665 2073 6d61 7274  ra to have smart
-0000c890: 2064 6574 6563 7469 6f6e 2222 220a 0a20   detection""".. 
-0000c8a0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-0000c8b0: 6169 7420 7365 6c66 2e5f 7365 745f 6175  ait self._set_au
-0000c8c0: 6469 6f5f 6465 7465 6374 2853 6d61 7274  dio_detect(Smart
-0000c8d0: 4465 7465 6374 4175 6469 6f54 7970 652e  DetectAudioType.
-0000c8e0: 4241 4259 5f43 5259 2c20 656e 6162 6c65  BABY_CRY, enable
-0000c8f0: 6429 0a0a 2020 2020 2320 7370 6561 6b69  d)..    # speaki
-0000c900: 6e67 0a0a 2020 2020 4070 726f 7065 7274  ng..    @propert
-0000c910: 790a 2020 2020 6465 6620 6361 6e5f 6465  y.    def can_de
-0000c920: 7465 6374 5f73 7065 616b 696e 6728 7365  tect_speaking(se
-0000c930: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-0000c940: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c950: 2e5f 6361 6e5f 6465 7465 6374 5f61 7564  ._can_detect_aud
-0000c960: 696f 2853 6d61 7274 4465 7465 6374 4f62  io(SmartDetectOb
-0000c970: 6a65 6374 5479 7065 2e53 5045 414b 290a  jectType.SPEAK).
-0000c980: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000c990: 2020 2064 6566 2069 735f 7370 6561 6b69     def is_speaki
-0000c9a0: 6e67 5f64 6574 6563 7469 6f6e 5f6f 6e28  ng_detection_on(
-0000c9b0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000c9c0: 2020 2020 2020 2022 2222 4973 2053 7065         """Is Spe
-0000c9d0: 616b 696e 6720 4465 7465 6374 696f 6e20  aking Detection 
-0000c9e0: 6176 6169 6c61 626c 6520 616e 6420 656e  available and en
-0000c9f0: 6162 6c65 6420 2863 616d 6572 6120 7769  abled (camera wi
-0000ca00: 6c6c 2070 726f 6475 6365 2073 7065 616b  ll produce speak
-0000ca10: 696e 6720 736d 6172 740a 2020 2020 2020  ing smart.      
-0000ca20: 2020 6465 7465 6374 696f 6e20 6576 656e    detection even
-0000ca30: 7473 293f 0a20 2020 2020 2020 2022 2222  ts)?.        """
+000094f0: 2063 616e 5f6d 616e 6167 655f 7265 636f   can_manage_reco
+00009500: 7264 696e 675f 7365 7474 696e 6728 7365  rding_setting(se
+00009510: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00009520: 2020 2020 2022 2222 4361 6e20 7468 6973       """Can this
+00009530: 2063 616d 6572 6120 6d61 6e61 6765 2069   camera manage i
+00009540: 7473 206f 776e 2072 6563 6f72 6469 6e67  ts own recording
+00009550: 2073 6574 7469 6e67 733f 2222 220a 0a20   settings?""".. 
+00009560: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+00009570: 7420 7365 6c66 2e75 7365 5f67 6c6f 6261  t self.use_globa
+00009580: 6c0a 0a20 2020 2040 7072 6f70 6572 7479  l..    @property
+00009590: 0a20 2020 2064 6566 2069 735f 736d 6172  .    def is_smar
+000095a0: 745f 6465 7465 6374 696f 6e73 5f61 6c6c  t_detections_all
+000095b0: 6f77 6564 2873 656c 6629 202d 3e20 626f  owed(self) -> bo
+000095c0: 6f6c 3a0a 2020 2020 2020 2020 2222 2249  ol:.        """I
+000095d0: 7320 736d 6172 7420 6465 7465 6374 696f  s smart detectio
+000095e0: 6e73 2061 6c6c 6f77 6564 2066 6f72 2074  ns allowed for t
+000095f0: 6869 7320 6361 6d65 7261 3f22 2222 0a0a  his camera?"""..
+00009600: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00009610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009620: 662e 6973 5f72 6563 6f72 6469 6e67 5f65  f.is_recording_e
+00009630: 6e61 626c 6564 0a20 2020 2020 2020 2020  nabled.         
+00009640: 2020 2061 6e64 2073 656c 662e 6170 692e     and self.api.
+00009650: 626f 6f74 7374 7261 702e 6e76 722e 6973  bootstrap.nvr.is
+00009660: 5f73 6d61 7274 5f64 6574 6563 7469 6f6e  _smart_detection
+00009670: 735f 656e 6162 6c65 640a 2020 2020 2020  s_enabled.      
+00009680: 2020 290a 0a20 2020 2040 7072 6f70 6572    )..    @proper
+00009690: 7479 0a20 2020 2064 6566 2063 616e 5f6d  ty.    def can_m
+000096a0: 616e 6167 655f 736d 6172 745f 6465 7465  anage_smart_dete
+000096b0: 6374 696f 6e73 2873 656c 6629 202d 3e20  ctions(self) -> 
+000096c0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+000096d0: 2243 616e 2074 6869 7320 6361 6d65 7261  "Can this camera
+000096e0: 206d 616e 6167 6520 6974 7320 6f77 6e20   manage its own 
+000096f0: 7265 636f 7264 696e 6720 7365 7474 696e  recording settin
+00009700: 6773 3f22 2222 0a0a 2020 2020 2020 2020  gs?"""..        
+00009710: 7265 7475 726e 2028 6e6f 7420 7365 6c66  return (not self
+00009720: 2e75 7365 5f67 6c6f 6261 6c29 2061 6e64  .use_global) and
+00009730: 2073 656c 662e 6973 5f73 6d61 7274 5f64   self.is_smart_d
+00009740: 6574 6563 7469 6f6e 735f 616c 6c6f 7765  etections_allowe
+00009750: 640a 0a20 2020 2040 7072 6f70 6572 7479  d..    @property
+00009760: 0a20 2020 2064 6566 2069 735f 6c69 6365  .    def is_lice
+00009770: 6e73 655f 706c 6174 655f 6465 7465 6374  nse_plate_detect
+00009780: 696f 6e73 5f61 6c6c 6f77 6564 2873 656c  ions_allowed(sel
+00009790: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+000097a0: 2020 2020 2222 2249 7320 6c69 6365 6e73      """Is licens
+000097b0: 6520 706c 6174 6520 6465 7465 6374 696f  e plate detectio
+000097c0: 6e73 2061 6c6c 6f77 6564 2066 6f72 2074  ns allowed for t
+000097d0: 6869 7320 6361 6d65 7261 3f22 2222 0a0a  his camera?"""..
+000097e0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+000097f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009800: 662e 6973 5f72 6563 6f72 6469 6e67 5f65  f.is_recording_e
+00009810: 6e61 626c 6564 0a20 2020 2020 2020 2020  nabled.         
+00009820: 2020 2061 6e64 2073 656c 662e 6170 692e     and self.api.
+00009830: 626f 6f74 7374 7261 702e 6e76 722e 6973  bootstrap.nvr.is
+00009840: 5f6c 6963 656e 7365 5f70 6c61 7465 5f64  _license_plate_d
+00009850: 6574 6563 7469 6f6e 735f 656e 6162 6c65  etections_enable
+00009860: 640a 2020 2020 2020 2020 290a 0a20 2020  d.        )..   
+00009870: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00009880: 6566 2063 616e 5f6d 616e 6167 655f 6c69  ef can_manage_li
+00009890: 6365 6e73 655f 706c 6174 655f 6465 7465  cense_plate_dete
+000098a0: 6374 696f 6e73 2873 656c 6629 202d 3e20  ctions(self) -> 
+000098b0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+000098c0: 2243 616e 2074 6869 7320 6361 6d65 7261  "Can this camera
+000098d0: 206d 616e 6167 6520 6974 7320 6f77 6e20   manage its own 
+000098e0: 6c69 6365 6e73 6520 706c 6174 6520 7365  license plate se
+000098f0: 7474 696e 6773 3f22 2222 0a0a 2020 2020  ttings?"""..    
+00009900: 2020 2020 7265 7475 726e 2028 6e6f 7420      return (not 
+00009910: 7365 6c66 2e75 7365 5f67 6c6f 6261 6c29  self.use_global)
+00009920: 2061 6e64 2073 656c 662e 6973 5f6c 6963   and self.is_lic
+00009930: 656e 7365 5f70 6c61 7465 5f64 6574 6563  ense_plate_detec
+00009940: 7469 6f6e 735f 616c 6c6f 7765 640a 0a20  tions_allowed.. 
+00009950: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00009960: 2064 6566 2069 735f 6661 6365 5f64 6574   def is_face_det
+00009970: 6563 7469 6f6e 735f 616c 6c6f 7765 6428  ections_allowed(
+00009980: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00009990: 2020 2020 2020 2022 2222 4973 2066 6163         """Is fac
+000099a0: 6520 6465 7465 6374 696f 6e73 2061 6c6c  e detections all
+000099b0: 6f77 6564 2066 6f72 2074 6869 7320 6361  owed for this ca
+000099c0: 6d65 7261 3f22 2222 0a0a 2020 2020 2020  mera?"""..      
+000099d0: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
+000099e0: 2020 2020 2020 2073 656c 662e 6973 5f72         self.is_r
+000099f0: 6563 6f72 6469 6e67 5f65 6e61 626c 6564  ecording_enabled
+00009a00: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00009a10: 2073 656c 662e 6170 692e 626f 6f74 7374   self.api.bootst
+00009a20: 7261 702e 6e76 722e 6973 5f66 6163 655f  rap.nvr.is_face_
+00009a30: 6465 7465 6374 696f 6e73 5f65 6e61 626c  detections_enabl
+00009a40: 6564 0a20 2020 2020 2020 2029 0a0a 2020  ed.        )..  
+00009a50: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00009a60: 6465 6620 6361 6e5f 6d61 6e61 6765 5f66  def can_manage_f
+00009a70: 6163 655f 6465 7465 6374 696f 6e73 2873  ace_detections(s
+00009a80: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+00009a90: 2020 2020 2020 2222 2243 616e 2074 6869        """Can thi
+00009aa0: 7320 6361 6d65 7261 206d 616e 6167 6520  s camera manage 
+00009ab0: 6974 7320 6f77 6e20 6661 6365 2064 6574  its own face det
+00009ac0: 6563 7469 6f6e 2073 6574 7469 6e67 733f  ection settings?
+00009ad0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+00009ae0: 7572 6e20 286e 6f74 2073 656c 662e 7573  urn (not self.us
+00009af0: 655f 676c 6f62 616c 2920 616e 6420 7365  e_global) and se
+00009b00: 6c66 2e69 735f 6661 6365 5f64 6574 6563  lf.is_face_detec
+00009b10: 7469 6f6e 735f 616c 6c6f 7765 640a 0a20  tions_allowed.. 
+00009b20: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00009b30: 2064 6566 2061 6374 6976 655f 7265 636f   def active_reco
+00009b40: 7264 696e 675f 7365 7474 696e 6773 2873  rding_settings(s
+00009b50: 656c 6629 202d 3e20 5265 636f 7264 696e  elf) -> Recordin
+00009b60: 6753 6574 7469 6e67 733a 0a20 2020 2020  gSettings:.     
+00009b70: 2020 2022 2222 4765 7420 6163 7469 7665     """Get active
+00009b80: 2072 6563 6f72 6469 6e67 2073 6574 7469   recording setti
+00009b90: 6e67 732e 2222 220a 0a20 2020 2020 2020  ngs."""..       
+00009ba0: 2069 6620 7365 6c66 2e75 7365 5f67 6c6f   if self.use_glo
+00009bb0: 6261 6c20 616e 6420 7365 6c66 2e61 7069  bal and self.api
+00009bc0: 2e62 6f6f 7473 7472 6170 2e6e 7672 2e67  .bootstrap.nvr.g
+00009bd0: 6c6f 6261 6c5f 6361 6d65 7261 5f73 6574  lobal_camera_set
+00009be0: 7469 6e67 733a 0a20 2020 2020 2020 2020  tings:.         
+00009bf0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+00009c00: 7069 2e62 6f6f 7473 7472 6170 2e6e 7672  pi.bootstrap.nvr
+00009c10: 2e67 6c6f 6261 6c5f 6361 6d65 7261 5f73  .global_camera_s
+00009c20: 6574 7469 6e67 732e 7265 636f 7264 696e  ettings.recordin
+00009c30: 675f 7365 7474 696e 6773 0a0a 2020 2020  g_settings..    
+00009c40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00009c50: 7265 636f 7264 696e 675f 7365 7474 696e  recording_settin
+00009c60: 6773 0a0a 2020 2020 4070 726f 7065 7274  gs..    @propert
+00009c70: 790a 2020 2020 6465 6620 6163 7469 7665  y.    def active
+00009c80: 5f73 6d61 7274 5f64 6574 6563 745f 7365  _smart_detect_se
+00009c90: 7474 696e 6773 2873 656c 6629 202d 3e20  ttings(self) -> 
+00009ca0: 536d 6172 7444 6574 6563 7453 6574 7469  SmartDetectSetti
+00009cb0: 6e67 733a 0a20 2020 2020 2020 2022 2222  ngs:.        """
+00009cc0: 4765 7420 6163 7469 7665 2073 6d61 7274  Get active smart
+00009cd0: 2064 6574 6563 7469 6f6e 2073 6574 7469   detection setti
+00009ce0: 6e67 732e 2222 220a 0a20 2020 2020 2020  ngs."""..       
+00009cf0: 2069 6620 7365 6c66 2e75 7365 5f67 6c6f   if self.use_glo
+00009d00: 6261 6c20 616e 6420 7365 6c66 2e61 7069  bal and self.api
+00009d10: 2e62 6f6f 7473 7472 6170 2e6e 7672 2e67  .bootstrap.nvr.g
+00009d20: 6c6f 6261 6c5f 6361 6d65 7261 5f73 6574  lobal_camera_set
+00009d30: 7469 6e67 733a 0a20 2020 2020 2020 2020  tings:.         
+00009d40: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+00009d50: 7069 2e62 6f6f 7473 7472 6170 2e6e 7672  pi.bootstrap.nvr
+00009d60: 2e67 6c6f 6261 6c5f 6361 6d65 7261 5f73  .global_camera_s
+00009d70: 6574 7469 6e67 732e 736d 6172 745f 6465  ettings.smart_de
+00009d80: 7465 6374 5f73 6574 7469 6e67 730a 0a20  tect_settings.. 
+00009d90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009da0: 6c66 2e73 6d61 7274 5f64 6574 6563 745f  lf.smart_detect_
+00009db0: 7365 7474 696e 6773 0a0a 2020 2020 4070  settings..    @p
+00009dc0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00009dd0: 6163 7469 7665 5f73 6d61 7274 5f64 6574  active_smart_det
+00009de0: 6563 745f 7479 7065 7328 7365 6c66 2920  ect_types(self) 
+00009df0: 2d3e 2073 6574 5b53 6d61 7274 4465 7465  -> set[SmartDete
+00009e00: 6374 4f62 6a65 6374 5479 7065 5d3a 0a20  ctObjectType]:. 
+00009e10: 2020 2020 2020 2022 2222 4765 7420 6163         """Get ac
+00009e20: 7469 7665 2073 6d61 7274 2064 6574 6563  tive smart detec
+00009e30: 7469 6f6e 2074 7970 6573 2e22 2222 0a0a  tion types."""..
+00009e40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009e50: 7573 655f 676c 6f62 616c 3a0a 2020 2020  use_global:.    
+00009e60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009e70: 6574 2873 656c 662e 736d 6172 745f 6465  et(self.smart_de
+00009e80: 7465 6374 5f73 6574 7469 6e67 732e 6f62  tect_settings.ob
+00009e90: 6a65 6374 5f74 7970 6573 292e 696e 7465  ject_types).inte
+00009ea0: 7273 6563 7469 6f6e 280a 2020 2020 2020  rsection(.      
+00009eb0: 2020 2020 2020 2020 2020 7365 7428 7365            set(se
+00009ec0: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
+00009ed0: 2e73 6d61 7274 5f64 6574 6563 745f 7479  .smart_detect_ty
+00009ee0: 7065 7329 2c0a 2020 2020 2020 2020 2020  pes),.          
+00009ef0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00009f00: 7572 6e20 7365 7428 7365 6c66 2e73 6d61  urn set(self.sma
+00009f10: 7274 5f64 6574 6563 745f 7365 7474 696e  rt_detect_settin
+00009f20: 6773 2e6f 626a 6563 745f 7479 7065 7329  gs.object_types)
+00009f30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00009f40: 2020 2020 6465 6620 6163 7469 7665 5f61      def active_a
+00009f50: 7564 696f 5f64 6574 6563 745f 7479 7065  udio_detect_type
+00009f60: 7328 7365 6c66 2920 2d3e 2073 6574 5b53  s(self) -> set[S
+00009f70: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
+00009f80: 7970 655d 3a0a 2020 2020 2020 2020 2222  ype]:.        ""
+00009f90: 2247 6574 2061 6374 6976 6520 6175 6469  "Get active audi
+00009fa0: 6f20 6465 7465 6374 696f 6e20 7479 7065  o detection type
+00009fb0: 732e 2222 220a 0a20 2020 2020 2020 2069  s."""..        i
+00009fc0: 6620 7365 6c66 2e75 7365 5f67 6c6f 6261  f self.use_globa
+00009fd0: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+00009fe0: 6574 7572 6e20 7365 7428 7365 6c66 2e73  eturn set(self.s
+00009ff0: 6d61 7274 5f64 6574 6563 745f 7365 7474  mart_detect_sett
+0000a000: 696e 6773 2e61 7564 696f 5f74 7970 6573  ings.audio_types
+0000a010: 206f 7220 5b5d 292e 696e 7465 7273 6563   or []).intersec
+0000a020: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0000a030: 2020 2020 2020 7365 7428 7365 6c66 2e66        set(self.f
+0000a040: 6561 7475 7265 5f66 6c61 6773 2e73 6d61  eature_flags.sma
+0000a050: 7274 5f64 6574 6563 745f 6175 6469 6f5f  rt_detect_audio_
+0000a060: 7479 7065 7320 6f72 205b 5d29 2c0a 2020  types or []),.  
+0000a070: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000a080: 2020 2020 2072 6574 7572 6e20 7365 7428       return set(
+0000a090: 7365 6c66 2e73 6d61 7274 5f64 6574 6563  self.smart_detec
+0000a0a0: 745f 7365 7474 696e 6773 2e61 7564 696f  t_settings.audio
+0000a0b0: 5f74 7970 6573 206f 7220 5b5d 290a 0a20  _types or []).. 
+0000a0c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000a0d0: 2064 6566 2069 735f 6d6f 7469 6f6e 5f64   def is_motion_d
+0000a0e0: 6574 6563 7469 6f6e 5f6f 6e28 7365 6c66  etection_on(self
+0000a0f0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000a100: 2020 2022 2222 4973 204d 6f74 696f 6e20     """Is Motion 
+0000a110: 4465 7465 6374 696f 6e20 6176 6169 6c61  Detection availa
+0000a120: 626c 6520 616e 6420 656e 6162 6c65 6420  ble and enabled 
+0000a130: 2863 616d 6572 6120 7769 6c6c 2070 726f  (camera will pro
+0000a140: 6475 6365 206d 6f74 696f 6e20 6576 656e  duce motion even
+0000a150: 7473 293f 2222 220a 0a20 2020 2020 2020  ts)?"""..       
+0000a160: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
+0000a170: 2020 2020 2020 7365 6c66 2e69 735f 7265        self.is_re
+0000a180: 636f 7264 696e 675f 656e 6162 6c65 640a  cording_enabled.
+0000a190: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0000a1a0: 7365 6c66 2e61 6374 6976 655f 7265 636f  self.active_reco
+0000a1b0: 7264 696e 675f 7365 7474 696e 6773 2e65  rding_settings.e
+0000a1c0: 6e61 626c 655f 6d6f 7469 6f6e 5f64 6574  nable_motion_det
+0000a1d0: 6563 7469 6f6e 2069 7320 6e6f 7420 4661  ection is not Fa
+0000a1e0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+0000a1f0: 616e 6420 7365 6c66 2e63 616e 5f6d 616e  and self.can_man
+0000a200: 6167 655f 7265 636f 7264 696e 675f 7365  age_recording_se
+0000a210: 7474 696e 670a 2020 2020 2020 2020 290a  tting.        ).
+0000a220: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000a230: 2020 2064 6566 2069 735f 6d6f 7469 6f6e     def is_motion
+0000a240: 5f63 7572 7265 6e74 6c79 5f64 6574 6563  _currently_detec
+0000a250: 7465 6428 7365 6c66 2920 2d3e 2062 6f6f  ted(self) -> boo
+0000a260: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
+0000a270: 206d 6f74 696f 6e20 6375 7272 656e 746c   motion currentl
+0000a280: 7920 6265 696e 6720 6465 7465 6374 6564  y being detected
+0000a290: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000a2a0: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+0000a2b0: 2020 7365 6c66 2e69 735f 6d6f 7469 6f6e    self.is_motion
+0000a2c0: 5f64 6574 6563 7469 6f6e 5f6f 6e0a 2020  _detection_on.  
+0000a2d0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+0000a2e0: 6c66 2e69 735f 6d6f 7469 6f6e 5f64 6574  lf.is_motion_det
+0000a2f0: 6563 7465 640a 2020 2020 2020 2020 2020  ected.          
+0000a300: 2020 616e 6420 7365 6c66 2e6c 6173 745f    and self.last_
+0000a310: 6d6f 7469 6f6e 5f65 7665 6e74 2069 7320  motion_event is 
+0000a320: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000a330: 2020 2020 2061 6e64 2073 656c 662e 6c61       and self.la
+0000a340: 7374 5f6d 6f74 696f 6e5f 6576 656e 742e  st_motion_event.
+0000a350: 656e 6420 6973 204e 6f6e 650a 2020 2020  end is None.    
+0000a360: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
+0000a370: 2064 6566 2073 6574 5f6d 6f74 696f 6e5f   def set_motion_
+0000a380: 6465 7465 6374 696f 6e28 7365 6c66 2c20  detection(self, 
+0000a390: 656e 6162 6c65 643a 2062 6f6f 6c29 202d  enabled: bool) -
+0000a3a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000a3b0: 2222 2253 6574 7320 6d6f 7469 6f6e 2064  """Sets motion d
+0000a3c0: 6574 6563 7469 6f6e 206f 6e20 6361 6d65  etection on came
+0000a3d0: 7261 2222 220a 0a20 2020 2020 2020 2069  ra"""..        i
+0000a3e0: 6620 7365 6c66 2e75 7365 5f67 6c6f 6261  f self.use_globa
+0000a3f0: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+0000a400: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+0000a410: 2243 616d 6572 6120 6973 2075 7369 6e67  "Camera is using
+0000a420: 2067 6c6f 6261 6c20 7265 636f 7264 696e   global recordin
+0000a430: 6720 7365 7474 696e 6773 2e22 290a 0a20  g settings.").. 
+0000a440: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
+0000a450: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
+0000a460: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a470: 7265 636f 7264 696e 675f 7365 7474 696e  recording_settin
+0000a480: 6773 2e65 6e61 626c 655f 6d6f 7469 6f6e  gs.enable_motion
+0000a490: 5f64 6574 6563 7469 6f6e 203d 2065 6e61  _detection = ena
+0000a4a0: 626c 6564 0a0a 2020 2020 2020 2020 6177  bled..        aw
+0000a4b0: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
+0000a4c0: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
+0000a4d0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
+0000a4e0: 6574 5f75 7365 5f67 6c6f 6261 6c28 7365  et_use_global(se
+0000a4f0: 6c66 2c20 656e 6162 6c65 643a 2062 6f6f  lf, enabled: boo
+0000a500: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+0000a510: 2020 2020 2222 2253 6574 7320 6966 2063      """Sets if c
+0000a520: 616d 6572 6120 7368 6f75 6c64 2075 7365  amera should use
+0000a530: 2067 6c6f 6261 6c20 7265 636f 7264 696e   global recordin
+0000a540: 6720 7365 7474 696e 6773 206f 7220 6e6f  g settings or no
+0000a550: 742e 2222 220a 0a20 2020 2020 2020 2064  t."""..        d
+0000a560: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
+0000a570: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a580: 2020 2073 656c 662e 7573 655f 676c 6f62     self.use_glob
+0000a590: 616c 203d 2065 6e61 626c 6564 0a0a 2020  al = enabled..  
+0000a5a0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+0000a5b0: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
+0000a5c0: 6c6c 6261 636b 290a 0a20 2020 2023 2072  llback)..    # r
+0000a5d0: 6567 696f 6e20 4f62 6a65 6374 2053 6d61  egion Object Sma
+0000a5e0: 7274 2044 6574 6563 7469 6f6e 730a 0a20  rt Detections.. 
+0000a5f0: 2020 2064 6566 205f 6973 5f73 6d61 7274     def _is_smart
+0000a600: 5f65 6e61 626c 6564 2873 656c 662c 2073  _enabled(self, s
+0000a610: 6d61 7274 5f74 7970 653a 2053 6d61 7274  mart_type: Smart
+0000a620: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000a630: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000a640: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
+0000a650: 2020 2020 2020 2020 7365 6c66 2e69 735f          self.is_
+0000a660: 7265 636f 7264 696e 675f 656e 6162 6c65  recording_enable
+0000a670: 640a 2020 2020 2020 2020 2020 2020 616e  d.            an
+0000a680: 6420 736d 6172 745f 7479 7065 2069 6e20  d smart_type in 
+0000a690: 7365 6c66 2e61 6374 6976 655f 736d 6172  self.active_smar
+0000a6a0: 745f 6465 7465 6374 5f74 7970 6573 0a20  t_detect_types. 
+0000a6b0: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
+0000a6c0: 656c 662e 6361 6e5f 6d61 6e61 6765 5f73  elf.can_manage_s
+0000a6d0: 6d61 7274 5f64 6574 6563 7469 6f6e 730a  mart_detections.
+0000a6e0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000a6f0: 6566 205f 6973 5f73 6d61 7274 5f64 6574  ef _is_smart_det
+0000a700: 6563 7465 6428 7365 6c66 2c20 736d 6172  ected(self, smar
+0000a710: 745f 7479 7065 3a20 536d 6172 7444 6574  t_type: SmartDet
+0000a720: 6563 744f 626a 6563 7454 7970 6529 202d  ectObjectType) -
+0000a730: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000a740: 6576 656e 7420 3d20 7365 6c66 2e67 6574  event = self.get
+0000a750: 5f6c 6173 745f 736d 6172 745f 6465 7465  _last_smart_dete
+0000a760: 6374 5f65 7665 6e74 2873 6d61 7274 5f74  ct_event(smart_t
+0000a770: 7970 6529 0a20 2020 2020 2020 2072 6574  ype).        ret
+0000a780: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+0000a790: 2020 7365 6c66 2e5f 6973 5f73 6d61 7274    self._is_smart
+0000a7a0: 5f65 6e61 626c 6564 2873 6d61 7274 5f74  _enabled(smart_t
+0000a7b0: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
+0000a7c0: 2061 6e64 2073 656c 662e 6973 5f73 6d61   and self.is_sma
+0000a7d0: 7274 5f64 6574 6563 7465 640a 2020 2020  rt_detected.    
+0000a7e0: 2020 2020 2020 2020 616e 6420 6576 656e          and even
+0000a7f0: 7420 6973 206e 6f74 204e 6f6e 650a 2020  t is not None.  
+0000a800: 2020 2020 2020 2020 2020 616e 6420 6576            and ev
+0000a810: 656e 742e 656e 6420 6973 204e 6f6e 650a  ent.end is None.
+0000a820: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0000a830: 736d 6172 745f 7479 7065 2069 6e20 6576  smart_type in ev
+0000a840: 656e 742e 736d 6172 745f 6465 7465 6374  ent.smart_detect
+0000a850: 5f74 7970 6573 0a20 2020 2020 2020 2029  _types.        )
+0000a860: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a870: 2020 2020 6465 6620 6973 5f73 6d61 7274      def is_smart
+0000a880: 5f63 7572 7265 6e74 6c79 5f64 6574 6563  _currently_detec
+0000a890: 7465 6428 7365 6c66 2920 2d3e 2062 6f6f  ted(self) -> boo
+0000a8a0: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
+0000a8b0: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000a8c0: 2063 7572 7265 6e74 6c79 2062 6569 6e67   currently being
+0000a8d0: 2064 6574 6563 7465 6422 2222 0a0a 2020   detected"""..  
+0000a8e0: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+0000a8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a900: 6973 5f72 6563 6f72 6469 6e67 5f65 6e61  is_recording_ena
+0000a910: 626c 6564 0a20 2020 2020 2020 2020 2020  bled.           
+0000a920: 2061 6e64 2062 6f6f 6c28 7365 6c66 2e61   and bool(self.a
+0000a930: 6374 6976 655f 736d 6172 745f 6465 7465  ctive_smart_dete
+0000a940: 6374 5f74 7970 6573 290a 2020 2020 2020  ct_types).      
+0000a950: 2020 2020 2020 616e 6420 7365 6c66 2e69        and self.i
+0000a960: 735f 736d 6172 745f 6465 7465 6374 6564  s_smart_detected
+0000a970: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0000a980: 2073 656c 662e 6c61 7374 5f73 6d61 7274   self.last_smart
+0000a990: 5f64 6574 6563 745f 6576 656e 7420 6973  _detect_event is
+0000a9a0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000a9b0: 2020 2020 2020 616e 6420 7365 6c66 2e6c        and self.l
+0000a9c0: 6173 745f 736d 6172 745f 6465 7465 6374  ast_smart_detect
+0000a9d0: 5f65 7665 6e74 2e65 6e64 2069 7320 4e6f  _event.end is No
+0000a9e0: 6e65 0a20 2020 2020 2020 2029 0a0a 2020  ne.        )..  
+0000a9f0: 2020 2320 7265 6769 6f6e 2050 6572 736f    # region Perso
+0000aa00: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
+0000aa10: 0a20 2020 2064 6566 2063 616e 5f64 6574  .    def can_det
+0000aa20: 6563 745f 7065 7273 6f6e 2873 656c 6629  ect_person(self)
+0000aa30: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000aa40: 2020 7265 7475 726e 2053 6d61 7274 4465    return SmartDe
+0000aa50: 7465 6374 4f62 6a65 6374 5479 7065 2e50  tectObjectType.P
+0000aa60: 4552 534f 4e20 696e 2073 656c 662e 6665  ERSON in self.fe
+0000aa70: 6174 7572 655f 666c 6167 732e 736d 6172  ature_flags.smar
+0000aa80: 745f 6465 7465 6374 5f74 7970 6573 0a0a  t_detect_types..
+0000aa90: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000aaa0: 2020 6465 6620 6973 5f70 6572 736f 6e5f    def is_person_
+0000aab0: 6465 7465 6374 696f 6e5f 6f6e 2873 656c  detection_on(sel
+0000aac0: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+0000aad0: 2020 2020 2222 2249 7320 5065 7273 6f6e      """Is Person
+0000aae0: 2044 6574 6563 7469 6f6e 2061 7661 696c   Detection avail
+0000aaf0: 6162 6c65 2061 6e64 2065 6e61 626c 6564  able and enabled
+0000ab00: 2028 6361 6d65 7261 2077 696c 6c20 7072   (camera will pr
+0000ab10: 6f64 7563 6520 7065 7273 6f6e 2073 6d61  oduce person sma
+0000ab20: 7274 0a20 2020 2020 2020 2064 6574 6563  rt.        detec
+0000ab30: 7469 6f6e 2065 7665 6e74 7329 3f0a 2020  tion events)?.  
+0000ab40: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000ab50: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000ab60: 6973 5f73 6d61 7274 5f65 6e61 626c 6564  is_smart_enabled
+0000ab70: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000ab80: 6374 5479 7065 2e50 4552 534f 4e29 0a0a  ctType.PERSON)..
+0000ab90: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000aba0: 2020 6465 6620 6c61 7374 5f70 6572 736f    def last_perso
+0000abb0: 6e5f 6465 7465 6374 5f65 7665 6e74 2873  n_detect_event(s
+0000abc0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000abd0: 5b45 7665 6e74 5d3a 0a20 2020 2020 2020  [Event]:.       
+0000abe0: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
+0000abf0: 2070 6572 736f 6e20 736d 6172 7420 6465   person smart de
+0000ac00: 7465 6374 696f 6e20 6576 656e 742e 2222  tection event.""
+0000ac10: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000ac20: 6e20 7365 6c66 2e67 6574 5f6c 6173 745f  n self.get_last_
+0000ac30: 736d 6172 745f 6465 7465 6374 5f65 7665  smart_detect_eve
+0000ac40: 6e74 2853 6d61 7274 4465 7465 6374 4f62  nt(SmartDetectOb
+0000ac50: 6a65 6374 5479 7065 2e50 4552 534f 4e29  jectType.PERSON)
+0000ac60: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000ac70: 2020 2020 6465 6620 6c61 7374 5f70 6572      def last_per
+0000ac80: 736f 6e5f 6465 7465 6374 2873 656c 6629  son_detect(self)
+0000ac90: 202d 3e20 4f70 7469 6f6e 616c 5b64 6174   -> Optional[dat
+0000aca0: 6574 696d 655d 3a0a 2020 2020 2020 2020  etime]:.        
+0000acb0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+0000acc0: 7065 7273 6f6e 2073 6d61 7274 2064 6574  person smart det
+0000acd0: 6563 7469 6f6e 2065 7665 6e74 2e22 2222  ection event."""
+0000ace0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000acf0: 2073 656c 662e 6c61 7374 5f73 6d61 7274   self.last_smart
+0000ad00: 5f64 6574 6563 7473 2e67 6574 2853 6d61  _detects.get(Sma
+0000ad10: 7274 4465 7465 6374 4f62 6a65 6374 5479  rtDetectObjectTy
+0000ad20: 7065 2e50 4552 534f 4e29 0a0a 2020 2020  pe.PERSON)..    
+0000ad30: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000ad40: 6620 6973 5f70 6572 736f 6e5f 6375 7272  f is_person_curr
+0000ad50: 656e 746c 795f 6465 7465 6374 6564 2873  ently_detected(s
+0000ad60: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000ad70: 2020 2020 2020 2222 2249 7320 7065 7273        """Is pers
+0000ad80: 6f6e 2063 7572 7265 6e74 6c79 2062 6569  on currently bei
+0000ad90: 6e67 2064 6574 6563 7465 6422 2222 0a0a  ng detected"""..
+0000ada0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000adb0: 656c 662e 5f69 735f 736d 6172 745f 6465  elf._is_smart_de
+0000adc0: 7465 6374 6564 2853 6d61 7274 4465 7465  tected(SmartDete
+0000add0: 6374 4f62 6a65 6374 5479 7065 2e50 4552  ctObjectType.PER
+0000ade0: 534f 4e29 0a0a 2020 2020 6173 796e 6320  SON)..    async 
+0000adf0: 6465 6620 7365 745f 7065 7273 6f6e 5f64  def set_person_d
+0000ae00: 6574 6563 7469 6f6e 2873 656c 662c 2065  etection(self, e
+0000ae10: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
+0000ae20: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000ae30: 2222 546f 6767 6c65 7320 7065 7273 6f6e  ""Toggles person
+0000ae40: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000ae50: 2e20 5265 7175 6972 6573 2063 616d 6572  . Requires camer
+0000ae60: 6120 746f 2068 6176 6520 736d 6172 7420  a to have smart 
+0000ae70: 6465 7465 6374 696f 6e22 2222 0a0a 2020  detection"""..  
+0000ae80: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0000ae90: 6974 2073 656c 662e 5f73 6574 5f6f 626a  it self._set_obj
+0000aea0: 6563 745f 6465 7465 6374 2853 6d61 7274  ect_detect(Smart
+0000aeb0: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000aec0: 2e50 4552 534f 4e2c 2065 6e61 626c 6564  .PERSON, enabled
+0000aed0: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000aee0: 0a20 2020 2064 6566 2069 735f 7065 7273  .    def is_pers
+0000aef0: 6f6e 5f74 7261 636b 696e 675f 656e 6162  on_tracking_enab
+0000af00: 6c65 6428 7365 6c66 2920 2d3e 2062 6f6f  led(self) -> boo
+0000af10: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
+0000af20: 2070 6572 736f 6e20 7472 6163 6b69 6e67   person tracking
+0000af30: 2065 6e61 626c 6564 2222 220a 2020 2020   enabled""".    
+0000af40: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+0000af50: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+0000af60: 7469 7665 5f73 6d61 7274 5f64 6574 6563  tive_smart_detec
+0000af70: 745f 7365 7474 696e 6773 2e61 7574 6f5f  t_settings.auto_
+0000af80: 7472 6163 6b69 6e67 5f6f 626a 6563 745f  tracking_object_
+0000af90: 7479 7065 7320 6973 206e 6f74 204e 6f6e  types is not Non
+0000afa0: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+0000afb0: 6420 536d 6172 7444 6574 6563 744f 626a  d SmartDetectObj
+0000afc0: 6563 7454 7970 652e 5045 5253 4f4e 0a20  ectType.PERSON. 
+0000afd0: 2020 2020 2020 2020 2020 2069 6e20 7365             in se
+0000afe0: 6c66 2e61 6374 6976 655f 736d 6172 745f  lf.active_smart_
+0000aff0: 6465 7465 6374 5f73 6574 7469 6e67 732e  detect_settings.
+0000b000: 6175 746f 5f74 7261 636b 696e 675f 6f62  auto_tracking_ob
+0000b010: 6a65 6374 5f74 7970 6573 0a20 2020 2020  ject_types.     
+0000b020: 2020 2029 0a0a 2020 2020 2320 656e 6472     )..    # endr
+0000b030: 6567 696f 6e0a 2020 2020 2320 7265 6769  egion.    # regi
+0000b040: 6f6e 2056 6568 6963 6c65 0a0a 2020 2020  on Vehicle..    
+0000b050: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000b060: 6620 6361 6e5f 6465 7465 6374 5f76 6568  f can_detect_veh
+0000b070: 6963 6c65 2873 656c 6629 202d 3e20 626f  icle(self) -> bo
+0000b080: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
+0000b090: 726e 2053 6d61 7274 4465 7465 6374 4f62  rn SmartDetectOb
+0000b0a0: 6a65 6374 5479 7065 2e56 4548 4943 4c45  jectType.VEHICLE
+0000b0b0: 2069 6e20 7365 6c66 2e66 6561 7475 7265   in self.feature
+0000b0c0: 5f66 6c61 6773 2e73 6d61 7274 5f64 6574  _flags.smart_det
+0000b0d0: 6563 745f 7479 7065 730a 0a20 2020 2040  ect_types..    @
+0000b0e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000b0f0: 2069 735f 7665 6869 636c 655f 6465 7465   is_vehicle_dete
+0000b100: 6374 696f 6e5f 6f6e 2873 656c 6629 202d  ction_on(self) -
+0000b110: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000b120: 2222 2249 7320 5665 6869 636c 6520 4465  """Is Vehicle De
+0000b130: 7465 6374 696f 6e20 6176 6169 6c61 626c  tection availabl
+0000b140: 6520 616e 6420 656e 6162 6c65 6420 2863  e and enabled (c
+0000b150: 616d 6572 6120 7769 6c6c 2070 726f 6475  amera will produ
+0000b160: 6365 2076 6568 6963 6c65 2073 6d61 7274  ce vehicle smart
+0000b170: 0a20 2020 2020 2020 2064 6574 6563 7469  .        detecti
+0000b180: 6f6e 2065 7665 6e74 7329 3f0a 2020 2020  on events)?.    
+0000b190: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000b1a0: 2072 6574 7572 6e20 7365 6c66 2e5f 6973   return self._is
+0000b1b0: 5f73 6d61 7274 5f65 6e61 626c 6564 2853  _smart_enabled(S
+0000b1c0: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
+0000b1d0: 5479 7065 2e56 4548 4943 4c45 290a 0a20  Type.VEHICLE).. 
+0000b1e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000b1f0: 2064 6566 206c 6173 745f 7665 6869 636c   def last_vehicl
+0000b200: 655f 6465 7465 6374 5f65 7665 6e74 2873  e_detect_event(s
+0000b210: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000b220: 5b45 7665 6e74 5d3a 0a20 2020 2020 2020  [Event]:.       
+0000b230: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
+0000b240: 2076 6568 6963 6c65 2073 6d61 7274 2064   vehicle smart d
+0000b250: 6574 6563 7469 6f6e 2065 7665 6e74 2e22  etection event."
+0000b260: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000b270: 726e 2073 656c 662e 6765 745f 6c61 7374  rn self.get_last
+0000b280: 5f73 6d61 7274 5f64 6574 6563 745f 6576  _smart_detect_ev
+0000b290: 656e 7428 536d 6172 7444 6574 6563 744f  ent(SmartDetectO
+0000b2a0: 626a 6563 7454 7970 652e 5645 4849 434c  bjectType.VEHICL
+0000b2b0: 4529 0a0a 2020 2020 4070 726f 7065 7274  E)..    @propert
+0000b2c0: 790a 2020 2020 6465 6620 6c61 7374 5f76  y.    def last_v
+0000b2d0: 6568 6963 6c65 5f64 6574 6563 7428 7365  ehicle_detect(se
+0000b2e0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000b2f0: 6461 7465 7469 6d65 5d3a 0a20 2020 2020  datetime]:.     
+0000b300: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
+0000b310: 7374 2076 6568 6963 6c65 2073 6d61 7274  st vehicle smart
+0000b320: 2064 6574 6563 7469 6f6e 2065 7665 6e74   detection event
+0000b330: 2e22 2222 0a0a 2020 2020 2020 2020 7265  ."""..        re
+0000b340: 7475 726e 2073 656c 662e 6c61 7374 5f73  turn self.last_s
+0000b350: 6d61 7274 5f64 6574 6563 7473 2e67 6574  mart_detects.get
+0000b360: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000b370: 6374 5479 7065 2e56 4548 4943 4c45 290a  ctType.VEHICLE).
+0000b380: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000b390: 2020 2064 6566 2069 735f 7665 6869 636c     def is_vehicl
+0000b3a0: 655f 6375 7272 656e 746c 795f 6465 7465  e_currently_dete
+0000b3b0: 6374 6564 2873 656c 6629 202d 3e20 626f  cted(self) -> bo
+0000b3c0: 6f6c 3a0a 2020 2020 2020 2020 2222 2249  ol:.        """I
+0000b3d0: 7320 7665 6869 636c 6520 6375 7272 656e  s vehicle curren
+0000b3e0: 746c 7920 6265 696e 6720 6465 7465 6374  tly being detect
+0000b3f0: 6564 2222 220a 0a20 2020 2020 2020 2072  ed"""..        r
+0000b400: 6574 7572 6e20 7365 6c66 2e5f 6973 5f73  eturn self._is_s
+0000b410: 6d61 7274 5f64 6574 6563 7465 6428 536d  mart_detected(Sm
+0000b420: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
+0000b430: 7970 652e 5645 4849 434c 4529 0a0a 2020  ype.VEHICLE)..  
+0000b440: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+0000b450: 7665 6869 636c 655f 6465 7465 6374 696f  vehicle_detectio
+0000b460: 6e28 7365 6c66 2c20 656e 6162 6c65 643a  n(self, enabled:
+0000b470: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+0000b480: 2020 2020 2020 2020 2222 2254 6f67 676c          """Toggl
+0000b490: 6573 2076 6568 6963 6c65 2073 6d61 7274  es vehicle smart
+0000b4a0: 2064 6574 6563 7469 6f6e 2e20 5265 7175   detection. Requ
+0000b4b0: 6972 6573 2063 616d 6572 6120 746f 2068  ires camera to h
+0000b4c0: 6176 6520 736d 6172 7420 6465 7465 6374  ave smart detect
+0000b4d0: 696f 6e22 2222 0a0a 2020 2020 2020 2020  ion"""..        
+0000b4e0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+0000b4f0: 662e 5f73 6574 5f6f 626a 6563 745f 6465  f._set_object_de
+0000b500: 7465 6374 2853 6d61 7274 4465 7465 6374  tect(SmartDetect
+0000b510: 4f62 6a65 6374 5479 7065 2e56 4548 4943  ObjectType.VEHIC
+0000b520: 4c45 2c20 656e 6162 6c65 6429 0a0a 2020  LE, enabled)..  
+0000b530: 2020 2320 656e 6472 6567 696f 6e0a 2020    # endregion.  
+0000b540: 2020 2320 7265 6769 6f6e 204c 6963 656e    # region Licen
+0000b550: 7365 2050 6c61 7465 0a0a 2020 2020 4070  se Plate..    @p
+0000b560: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000b570: 6361 6e5f 6465 7465 6374 5f6c 6963 656e  can_detect_licen
+0000b580: 7365 5f70 6c61 7465 2873 656c 6629 202d  se_plate(self) -
+0000b590: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000b5a0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
+0000b5b0: 2020 2020 2053 6d61 7274 4465 7465 6374       SmartDetect
+0000b5c0: 4f62 6a65 6374 5479 7065 2e4c 4943 454e  ObjectType.LICEN
+0000b5d0: 5345 5f50 4c41 5445 2069 6e20 7365 6c66  SE_PLATE in self
+0000b5e0: 2e66 6561 7475 7265 5f66 6c61 6773 2e73  .feature_flags.s
+0000b5f0: 6d61 7274 5f64 6574 6563 745f 7479 7065  mart_detect_type
+0000b600: 730a 2020 2020 2020 2020 290a 0a20 2020  s.        )..   
+0000b610: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000b620: 6566 2069 735f 6c69 6365 6e73 655f 706c  ef is_license_pl
+0000b630: 6174 655f 6465 7465 6374 696f 6e5f 6f6e  ate_detection_on
+0000b640: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000b650: 2020 2020 2020 2020 2222 2249 7320 4c69          """Is Li
+0000b660: 6365 6e73 6520 506c 6174 6520 4465 7465  cense Plate Dete
+0000b670: 6374 696f 6e20 6176 6169 6c61 626c 6520  ction available 
+0000b680: 616e 6420 656e 6162 6c65 6420 2863 616d  and enabled (cam
+0000b690: 6572 6120 7769 6c6c 2070 726f 6475 6365  era will produce
+0000b6a0: 2066 6163 6520 6c69 6365 6e73 650a 2020   face license.  
+0000b6b0: 2020 2020 2020 706c 6174 6520 6465 7465        plate dete
+0000b6c0: 6374 696f 6e20 6576 656e 7473 293f 0a20  ction events)?. 
+0000b6d0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0000b6e0: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+0000b6f0: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
+0000b700: 735f 736d 6172 745f 656e 6162 6c65 6428  s_smart_enabled(
+0000b710: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
+0000b720: 7454 7970 652e 4c49 4345 4e53 455f 504c  tType.LICENSE_PL
+0000b730: 4154 4529 0a20 2020 2020 2020 2020 2020  ATE).           
+0000b740: 2061 6e64 2073 656c 662e 6973 5f6c 6963   and self.is_lic
+0000b750: 656e 7365 5f70 6c61 7465 5f64 6574 6563  ense_plate_detec
+0000b760: 7469 6f6e 735f 616c 6c6f 7765 640a 2020  tions_allowed.  
+0000b770: 2020 2020 2020 290a 0a20 2020 2040 7072        )..    @pr
+0000b780: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+0000b790: 6173 745f 6c69 6365 6e73 655f 706c 6174  ast_license_plat
+0000b7a0: 655f 6465 7465 6374 5f65 7665 6e74 2873  e_detect_event(s
+0000b7b0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000b7c0: 5b45 7665 6e74 5d3a 0a20 2020 2020 2020  [Event]:.       
+0000b7d0: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
+0000b7e0: 206c 6963 656e 7365 2070 6c61 7465 2073   license plate s
+0000b7f0: 6d61 7274 2064 6574 6563 7469 6f6e 2065  mart detection e
+0000b800: 7665 6e74 2e22 2222 0a0a 2020 2020 2020  vent."""..      
+0000b810: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
+0000b820: 745f 6c61 7374 5f73 6d61 7274 5f64 6574  t_last_smart_det
+0000b830: 6563 745f 6576 656e 7428 536d 6172 7444  ect_event(SmartD
+0000b840: 6574 6563 744f 626a 6563 7454 7970 652e  etectObjectType.
+0000b850: 4c49 4345 4e53 455f 504c 4154 4529 0a0a  LICENSE_PLATE)..
+0000b860: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000b870: 2020 6465 6620 6c61 7374 5f6c 6963 656e    def last_licen
+0000b880: 7365 5f70 6c61 7465 5f64 6574 6563 7428  se_plate_detect(
+0000b890: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+0000b8a0: 6c5b 6461 7465 7469 6d65 5d3a 0a20 2020  l[datetime]:.   
+0000b8b0: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+0000b8c0: 6c61 7374 206c 6963 656e 7365 2070 6c61  last license pla
+0000b8d0: 7465 2073 6d61 7274 2064 6574 6563 7469  te smart detecti
+0000b8e0: 6f6e 2065 7665 6e74 2e22 2222 0a0a 2020  on event."""..  
+0000b8f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b900: 662e 6c61 7374 5f73 6d61 7274 5f64 6574  f.last_smart_det
+0000b910: 6563 7473 2e67 6574 2853 6d61 7274 4465  ects.get(SmartDe
+0000b920: 7465 6374 4f62 6a65 6374 5479 7065 2e4c  tectObjectType.L
+0000b930: 4943 454e 5345 5f50 4c41 5445 290a 0a20  ICENSE_PLATE).. 
+0000b940: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000b950: 2064 6566 2069 735f 6c69 6365 6e73 655f   def is_license_
+0000b960: 706c 6174 655f 6375 7272 656e 746c 795f  plate_currently_
+0000b970: 6465 7465 6374 6564 2873 656c 6629 202d  detected(self) -
+0000b980: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000b990: 2222 2249 7320 6c69 6365 6e73 6520 706c  """Is license pl
+0000b9a0: 6174 6520 6375 7272 656e 746c 7920 6265  ate currently be
+0000b9b0: 696e 6720 6465 7465 6374 6564 2222 220a  ing detected""".
+0000b9c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b9d0: 7365 6c66 2e5f 6973 5f73 6d61 7274 5f64  self._is_smart_d
+0000b9e0: 6574 6563 7465 6428 536d 6172 7444 6574  etected(SmartDet
+0000b9f0: 6563 744f 626a 6563 7454 7970 652e 4c49  ectObjectType.LI
+0000ba00: 4345 4e53 455f 504c 4154 4529 0a0a 2020  CENSE_PLATE)..  
+0000ba10: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+0000ba20: 6c69 6365 6e73 655f 706c 6174 655f 6465  license_plate_de
+0000ba30: 7465 6374 696f 6e28 7365 6c66 2c20 656e  tection(self, en
+0000ba40: 6162 6c65 643a 2062 6f6f 6c29 202d 3e20  abled: bool) -> 
+0000ba50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000ba60: 2254 6f67 676c 6573 206c 6963 656e 7365  "Toggles license
+0000ba70: 2070 6c61 7465 2073 6d61 7274 2064 6574   plate smart det
+0000ba80: 6563 7469 6f6e 2e20 5265 7175 6972 6573  ection. Requires
+0000ba90: 2063 616d 6572 6120 746f 2068 6176 6520   camera to have 
+0000baa0: 736d 6172 7420 6465 7465 6374 696f 6e22  smart detection"
+0000bab0: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000bac0: 726e 2061 7761 6974 2073 656c 662e 5f73  rn await self._s
+0000bad0: 6574 5f6f 626a 6563 745f 6465 7465 6374  et_object_detect
+0000bae0: 280a 2020 2020 2020 2020 2020 2020 536d  (.            Sm
+0000baf0: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
+0000bb00: 7970 652e 4c49 4345 4e53 455f 504c 4154  ype.LICENSE_PLAT
+0000bb10: 452c 0a20 2020 2020 2020 2020 2020 2065  E,.            e
+0000bb20: 6e61 626c 6564 2c0a 2020 2020 2020 2020  nabled,.        
+0000bb30: 290a 0a20 2020 2023 2065 6e64 7265 6769  )..    # endregi
+0000bb40: 6f6e 0a20 2020 2023 2072 6567 696f 6e20  on.    # region 
+0000bb50: 5061 636b 6167 650a 0a20 2020 2040 7072  Package..    @pr
+0000bb60: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+0000bb70: 616e 5f64 6574 6563 745f 7061 636b 6167  an_detect_packag
+0000bb80: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
+0000bb90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bba0: 536d 6172 7444 6574 6563 744f 626a 6563  SmartDetectObjec
+0000bbb0: 7454 7970 652e 5041 434b 4147 4520 696e  tType.PACKAGE in
+0000bbc0: 2073 656c 662e 6665 6174 7572 655f 666c   self.feature_fl
+0000bbd0: 6167 732e 736d 6172 745f 6465 7465 6374  ags.smart_detect
+0000bbe0: 5f74 7970 6573 0a0a 2020 2020 4070 726f  _types..    @pro
+0000bbf0: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
+0000bc00: 5f70 6163 6b61 6765 5f64 6574 6563 7469  _package_detecti
+0000bc10: 6f6e 5f6f 6e28 7365 6c66 2920 2d3e 2062  on_on(self) -> b
+0000bc20: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0000bc30: 4973 2050 6163 6b61 6765 2044 6574 6563  Is Package Detec
+0000bc40: 7469 6f6e 2061 7661 696c 6162 6c65 2061  tion available a
+0000bc50: 6e64 2065 6e61 626c 6564 2028 6361 6d65  nd enabled (came
+0000bc60: 7261 2077 696c 6c20 7072 6f64 7563 6520  ra will produce 
+0000bc70: 7061 636b 6167 6520 736d 6172 740a 2020  package smart.  
+0000bc80: 2020 2020 2020 6465 7465 6374 696f 6e20        detection 
+0000bc90: 6576 656e 7473 293f 0a20 2020 2020 2020  events)?.       
+0000bca0: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+0000bcb0: 7475 726e 2073 656c 662e 5f69 735f 736d  turn self._is_sm
+0000bcc0: 6172 745f 656e 6162 6c65 6428 536d 6172  art_enabled(Smar
+0000bcd0: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
+0000bce0: 652e 5041 434b 4147 4529 0a0a 2020 2020  e.PACKAGE)..    
+0000bcf0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000bd00: 6620 6c61 7374 5f70 6163 6b61 6765 5f64  f last_package_d
+0000bd10: 6574 6563 745f 6576 656e 7428 7365 6c66  etect_event(self
+0000bd20: 2920 2d3e 204f 7074 696f 6e61 6c5b 4576  ) -> Optional[Ev
+0000bd30: 656e 745d 3a0a 2020 2020 2020 2020 2222  ent]:.        ""
+0000bd40: 2247 6574 2074 6865 206c 6173 7420 7061  "Get the last pa
+0000bd50: 636b 6167 6520 736d 6172 7420 6465 7465  ckage smart dete
+0000bd60: 6374 696f 6e20 6576 656e 742e 2222 220a  ction event.""".
+0000bd70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bd80: 7365 6c66 2e67 6574 5f6c 6173 745f 736d  self.get_last_sm
+0000bd90: 6172 745f 6465 7465 6374 5f65 7665 6e74  art_detect_event
+0000bda0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000bdb0: 6374 5479 7065 2e50 4143 4b41 4745 290a  ctType.PACKAGE).
+0000bdc0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000bdd0: 2020 2064 6566 206c 6173 745f 7061 636b     def last_pack
+0000bde0: 6167 655f 6465 7465 6374 2873 656c 6629  age_detect(self)
+0000bdf0: 202d 3e20 4f70 7469 6f6e 616c 5b64 6174   -> Optional[dat
+0000be00: 6574 696d 655d 3a0a 2020 2020 2020 2020  etime]:.        
+0000be10: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+0000be20: 7061 636b 6167 6520 736d 6172 7420 6465  package smart de
+0000be30: 7465 6374 696f 6e20 6576 656e 742e 2222  tection event.""
+0000be40: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000be50: 6e20 7365 6c66 2e6c 6173 745f 736d 6172  n self.last_smar
+0000be60: 745f 6465 7465 6374 732e 6765 7428 536d  t_detects.get(Sm
+0000be70: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
+0000be80: 7970 652e 5041 434b 4147 4529 0a0a 2020  ype.PACKAGE)..  
+0000be90: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000bea0: 6465 6620 6973 5f70 6163 6b61 6765 5f63  def is_package_c
+0000beb0: 7572 7265 6e74 6c79 5f64 6574 6563 7465  urrently_detecte
+0000bec0: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
+0000bed0: 0a20 2020 2020 2020 2022 2222 4973 2070  .        """Is p
+0000bee0: 6163 6b61 6765 2063 7572 7265 6e74 6c79  ackage currently
+0000bef0: 2062 6569 6e67 2064 6574 6563 7465 6422   being detected"
+0000bf00: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000bf10: 726e 2073 656c 662e 5f69 735f 736d 6172  rn self._is_smar
+0000bf20: 745f 6465 7465 6374 6564 2853 6d61 7274  t_detected(Smart
+0000bf30: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000bf40: 2e50 4143 4b41 4745 290a 0a20 2020 2061  .PACKAGE)..    a
+0000bf50: 7379 6e63 2064 6566 2073 6574 5f70 6163  sync def set_pac
+0000bf60: 6b61 6765 5f64 6574 6563 7469 6f6e 2873  kage_detection(s
+0000bf70: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
+0000bf80: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
+0000bf90: 2020 2020 2022 2222 546f 6767 6c65 7320       """Toggles 
+0000bfa0: 7061 636b 6167 6520 736d 6172 7420 6465  package smart de
+0000bfb0: 7465 6374 696f 6e2e 2052 6571 7569 7265  tection. Require
+0000bfc0: 7320 6361 6d65 7261 2074 6f20 6861 7665  s camera to have
+0000bfd0: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000bfe0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000bff0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
+0000c000: 7365 745f 6f62 6a65 6374 5f64 6574 6563  set_object_detec
+0000c010: 7428 536d 6172 7444 6574 6563 744f 626a  t(SmartDetectObj
+0000c020: 6563 7454 7970 652e 5041 434b 4147 452c  ectType.PACKAGE,
+0000c030: 2065 6e61 626c 6564 290a 0a20 2020 2023   enabled)..    #
+0000c040: 2065 6e64 7265 6769 6f6e 0a20 2020 2023   endregion.    #
+0000c050: 2072 6567 696f 6e20 416e 696d 616c 0a0a   region Animal..
+0000c060: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000c070: 2020 6465 6620 6361 6e5f 6465 7465 6374    def can_detect
+0000c080: 5f61 6e69 6d61 6c28 7365 6c66 2920 2d3e  _animal(self) ->
+0000c090: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
+0000c0a0: 6574 7572 6e20 536d 6172 7444 6574 6563  eturn SmartDetec
+0000c0b0: 744f 626a 6563 7454 7970 652e 414e 494d  tObjectType.ANIM
+0000c0c0: 414c 2069 6e20 7365 6c66 2e66 6561 7475  AL in self.featu
+0000c0d0: 7265 5f66 6c61 6773 2e73 6d61 7274 5f64  re_flags.smart_d
+0000c0e0: 6574 6563 745f 7479 7065 730a 0a20 2020  etect_types..   
+0000c0f0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000c100: 6566 2069 735f 616e 696d 616c 5f64 6574  ef is_animal_det
+0000c110: 6563 7469 6f6e 5f6f 6e28 7365 6c66 2920  ection_on(self) 
+0000c120: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000c130: 2022 2222 4973 2041 6e69 6d61 6c20 4465   """Is Animal De
+0000c140: 7465 6374 696f 6e20 6176 6169 6c61 626c  tection availabl
+0000c150: 6520 616e 6420 656e 6162 6c65 6420 2863  e and enabled (c
+0000c160: 616d 6572 6120 7769 6c6c 2070 726f 6475  amera will produ
+0000c170: 6365 2070 6163 6b61 6765 2073 6d61 7274  ce package smart
+0000c180: 0a20 2020 2020 2020 2064 6574 6563 7469  .        detecti
+0000c190: 6f6e 2065 7665 6e74 7329 3f0a 2020 2020  on events)?.    
+0000c1a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000c1b0: 2072 6574 7572 6e20 7365 6c66 2e5f 6973   return self._is
+0000c1c0: 5f73 6d61 7274 5f65 6e61 626c 6564 2853  _smart_enabled(S
+0000c1d0: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
+0000c1e0: 5479 7065 2e41 4e49 4d41 4c29 0a0a 2020  Type.ANIMAL)..  
+0000c1f0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000c200: 6465 6620 6c61 7374 5f61 6e69 6d61 6c5f  def last_animal_
+0000c210: 6465 7465 6374 5f65 7665 6e74 2873 656c  detect_event(sel
+0000c220: 6629 202d 3e20 4f70 7469 6f6e 616c 5b45  f) -> Optional[E
+0000c230: 7665 6e74 5d3a 0a20 2020 2020 2020 2022  vent]:.        "
+0000c240: 2222 4765 7420 7468 6520 6c61 7374 2061  ""Get the last a
+0000c250: 6e69 6d61 6c20 736d 6172 7420 6465 7465  nimal smart dete
+0000c260: 6374 696f 6e20 6576 656e 742e 2222 220a  ction event.""".
+0000c270: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c280: 7365 6c66 2e67 6574 5f6c 6173 745f 736d  self.get_last_sm
+0000c290: 6172 745f 6465 7465 6374 5f65 7665 6e74  art_detect_event
+0000c2a0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000c2b0: 6374 5479 7065 2e41 4e49 4d41 4c29 0a0a  ctType.ANIMAL)..
+0000c2c0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000c2d0: 2020 6465 6620 6c61 7374 5f61 6e69 6d61    def last_anima
+0000c2e0: 6c5f 6465 7465 6374 2873 656c 6629 202d  l_detect(self) -
+0000c2f0: 3e20 4f70 7469 6f6e 616c 5b64 6174 6574  > Optional[datet
+0000c300: 696d 655d 3a0a 2020 2020 2020 2020 2222  ime]:.        ""
+0000c310: 2247 6574 2074 6865 206c 6173 7420 616e  "Get the last an
+0000c320: 696d 616c 2073 6d61 7274 2064 6574 6563  imal smart detec
+0000c330: 7469 6f6e 2065 7665 6e74 2e22 2222 0a0a  tion event."""..
+0000c340: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c350: 656c 662e 6c61 7374 5f73 6d61 7274 5f64  elf.last_smart_d
+0000c360: 6574 6563 7473 2e67 6574 2853 6d61 7274  etects.get(Smart
+0000c370: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000c380: 2e41 4e49 4d41 4c29 0a0a 2020 2020 4070  .ANIMAL)..    @p
+0000c390: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000c3a0: 6973 5f61 6e69 6d61 6c5f 6375 7272 656e  is_animal_curren
+0000c3b0: 746c 795f 6465 7465 6374 6564 2873 656c  tly_detected(sel
+0000c3c0: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+0000c3d0: 2020 2020 2222 2249 7320 616e 696d 616c      """Is animal
+0000c3e0: 2063 7572 7265 6e74 6c79 2062 6569 6e67   currently being
+0000c3f0: 2064 6574 6563 7465 6422 2222 0a0a 2020   detected"""..  
+0000c400: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000c410: 662e 5f69 735f 736d 6172 745f 6465 7465  f._is_smart_dete
+0000c420: 6374 6564 2853 6d61 7274 4465 7465 6374  cted(SmartDetect
+0000c430: 4f62 6a65 6374 5479 7065 2e41 4e49 4d41  ObjectType.ANIMA
+0000c440: 4c29 0a0a 2020 2020 6173 796e 6320 6465  L)..    async de
+0000c450: 6620 7365 745f 616e 696d 616c 5f64 6574  f set_animal_det
+0000c460: 6563 7469 6f6e 2873 656c 662c 2065 6e61  ection(self, ena
+0000c470: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+0000c480: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000c490: 546f 6767 6c65 7320 616e 696d 616c 2073  Toggles animal s
+0000c4a0: 6d61 7274 2064 6574 6563 7469 6f6e 2e20  mart detection. 
+0000c4b0: 5265 7175 6972 6573 2063 616d 6572 6120  Requires camera 
+0000c4c0: 746f 2068 6176 6520 736d 6172 7420 6465  to have smart de
+0000c4d0: 7465 6374 696f 6e22 2222 0a0a 2020 2020  tection"""..    
+0000c4e0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0000c4f0: 2073 656c 662e 5f73 6574 5f6f 626a 6563   self._set_objec
+0000c500: 745f 6465 7465 6374 2853 6d61 7274 4465  t_detect(SmartDe
+0000c510: 7465 6374 4f62 6a65 6374 5479 7065 2e41  tectObjectType.A
+0000c520: 4e49 4d41 4c2c 2065 6e61 626c 6564 290a  NIMAL, enabled).
+0000c530: 0a20 2020 2023 2065 6e64 7265 6769 6f6e  .    # endregion
+0000c540: 0a20 2020 2023 2065 6e64 7265 6769 6f6e  .    # endregion
+0000c550: 0a20 2020 2023 2072 6567 696f 6e20 4175  .    # region Au
+0000c560: 6469 6f20 536d 6172 7420 4465 7465 6374  dio Smart Detect
+0000c570: 696f 6e73 0a0a 2020 2020 6465 6620 5f63  ions..    def _c
+0000c580: 616e 5f64 6574 6563 745f 6175 6469 6f28  an_detect_audio(
+0000c590: 7365 6c66 2c20 736d 6172 745f 7479 7065  self, smart_type
+0000c5a0: 3a20 536d 6172 7444 6574 6563 744f 626a  : SmartDetectObj
+0000c5b0: 6563 7454 7970 6529 202d 3e20 626f 6f6c  ectType) -> bool
+0000c5c0: 3a0a 2020 2020 2020 2020 6175 6469 6f5f  :.        audio_
+0000c5d0: 7479 7065 203d 2073 6d61 7274 5f74 7970  type = smart_typ
+0000c5e0: 652e 6175 6469 6f5f 7479 7065 0a20 2020  e.audio_type.   
+0000c5f0: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
+0000c600: 2020 2020 2020 2020 2020 6175 6469 6f5f            audio_
+0000c610: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+0000c620: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0000c630: 2073 656c 662e 6665 6174 7572 655f 666c   self.feature_fl
+0000c640: 6167 732e 736d 6172 745f 6465 7465 6374  ags.smart_detect
+0000c650: 5f61 7564 696f 5f74 7970 6573 2069 7320  _audio_types is 
+0000c660: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000c670: 2020 2020 2061 6e64 2061 7564 696f 5f74       and audio_t
+0000c680: 7970 6520 696e 2073 656c 662e 6665 6174  ype in self.feat
+0000c690: 7572 655f 666c 6167 732e 736d 6172 745f  ure_flags.smart_
+0000c6a0: 6465 7465 6374 5f61 7564 696f 5f74 7970  detect_audio_typ
+0000c6b0: 6573 0a20 2020 2020 2020 2029 0a0a 2020  es.        )..  
+0000c6c0: 2020 6465 6620 5f69 735f 6175 6469 6f5f    def _is_audio_
+0000c6d0: 656e 6162 6c65 6428 7365 6c66 2c20 736d  enabled(self, sm
+0000c6e0: 6172 745f 7479 7065 3a20 536d 6172 7444  art_type: SmartD
+0000c6f0: 6574 6563 744f 626a 6563 7454 7970 6529  etectObjectType)
+0000c700: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000c710: 2020 6175 6469 6f5f 7479 7065 203d 2073    audio_type = s
+0000c720: 6d61 7274 5f74 7970 652e 6175 6469 6f5f  mart_type.audio_
+0000c730: 7479 7065 0a20 2020 2020 2020 2072 6574  type.        ret
+0000c740: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+0000c750: 2020 6175 6469 6f5f 7479 7065 2069 7320    audio_type is 
+0000c760: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000c770: 2020 2020 2061 6e64 2073 656c 662e 6973       and self.is
+0000c780: 5f72 6563 6f72 6469 6e67 5f65 6e61 626c  _recording_enabl
+0000c790: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
+0000c7a0: 6e64 2061 7564 696f 5f74 7970 6520 696e  nd audio_type in
+0000c7b0: 2073 656c 662e 6163 7469 7665 5f61 7564   self.active_aud
+0000c7c0: 696f 5f64 6574 6563 745f 7479 7065 730a  io_detect_types.
+0000c7d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0000c7e0: 7365 6c66 2e63 616e 5f6d 616e 6167 655f  self.can_manage_
+0000c7f0: 736d 6172 745f 6465 7465 6374 696f 6e73  smart_detections
+0000c800: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000c810: 6465 6620 5f69 735f 6175 6469 6f5f 6465  def _is_audio_de
+0000c820: 7465 6374 6564 2873 656c 662c 2073 6d61  tected(self, sma
+0000c830: 7274 5f74 7970 653a 2053 6d61 7274 4465  rt_type: SmartDe
+0000c840: 7465 6374 4f62 6a65 6374 5479 7065 2920  tectObjectType) 
+0000c850: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000c860: 2061 7564 696f 5f74 7970 6520 3d20 736d   audio_type = sm
+0000c870: 6172 745f 7479 7065 2e61 7564 696f 5f74  art_type.audio_t
+0000c880: 7970 650a 2020 2020 2020 2020 6966 2061  ype.        if a
+0000c890: 7564 696f 5f74 7970 6520 6973 204e 6f6e  udio_type is Non
+0000c8a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000c8b0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+0000c8c0: 2020 2020 2065 7665 6e74 203d 2073 656c       event = sel
+0000c8d0: 662e 6765 745f 6c61 7374 5f73 6d61 7274  f.get_last_smart
+0000c8e0: 5f61 7564 696f 5f64 6574 6563 745f 6576  _audio_detect_ev
+0000c8f0: 656e 7428 6175 6469 6f5f 7479 7065 290a  ent(audio_type).
+0000c900: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000c910: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c920: 662e 5f69 735f 6175 6469 6f5f 656e 6162  f._is_audio_enab
+0000c930: 6c65 6428 736d 6172 745f 7479 7065 290a  led(smart_type).
+0000c940: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0000c950: 6576 656e 7420 6973 206e 6f74 204e 6f6e  event is not Non
+0000c960: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+0000c970: 6420 6576 656e 742e 656e 6420 6973 204e  d event.end is N
+0000c980: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000c990: 616e 6420 736d 6172 745f 7479 7065 2069  and smart_type i
+0000c9a0: 6e20 6576 656e 742e 736d 6172 745f 6465  n event.smart_de
+0000c9b0: 7465 6374 5f74 7970 6573 0a20 2020 2020  tect_types.     
+0000c9c0: 2020 2029 0a0a 2020 2020 4070 726f 7065     )..    @prope
+0000c9d0: 7274 790a 2020 2020 6465 6620 6973 5f61  rty.    def is_a
+0000c9e0: 7564 696f 5f63 7572 7265 6e74 6c79 5f64  udio_currently_d
+0000c9f0: 6574 6563 7465 6428 7365 6c66 2920 2d3e  etected(self) ->
+0000ca00: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+0000ca10: 2222 4973 2061 7564 696f 2064 6574 6563  ""Is audio detec
+0000ca20: 7469 6f6e 2063 7572 7265 6e74 6c79 2062  tion currently b
+0000ca30: 6569 6e67 2064 6574 6563 7465 6422 2222  eing detected"""
 0000ca40: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ca50: 2073 656c 662e 5f69 735f 6175 6469 6f5f   self._is_audio_
-0000ca60: 656e 6162 6c65 6428 536d 6172 7444 6574  enabled(SmartDet
-0000ca70: 6563 744f 626a 6563 7454 7970 652e 5350  ectObjectType.SP
-0000ca80: 4541 4b29 0a0a 2020 2020 4070 726f 7065  EAK)..    @prope
-0000ca90: 7274 790a 2020 2020 6465 6620 6c61 7374  rty.    def last
-0000caa0: 5f73 7065 616b 696e 675f 6465 7465 6374  _speaking_detect
-0000cab0: 5f65 7665 6e74 2873 656c 6629 202d 3e20  _event(self) -> 
-0000cac0: 4f70 7469 6f6e 616c 5b45 7665 6e74 5d3a  Optional[Event]:
-0000cad0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000cae0: 7468 6520 6c61 7374 2053 7065 616b 696e  the last Speakin
-0000caf0: 6720 736d 6172 7420 6465 7465 6374 696f  g smart detectio
-0000cb00: 6e20 6576 656e 742e 2222 220a 0a20 2020  n event."""..   
-0000cb10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000cb20: 2e67 6574 5f6c 6173 745f 736d 6172 745f  .get_last_smart_
-0000cb30: 6175 6469 6f5f 6465 7465 6374 5f65 7665  audio_detect_eve
-0000cb40: 6e74 2853 6d61 7274 4465 7465 6374 4175  nt(SmartDetectAu
-0000cb50: 6469 6f54 7970 652e 5350 4541 4b29 0a0a  dioType.SPEAK)..
-0000cb60: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000cb70: 2020 6465 6620 6c61 7374 5f73 7065 616b    def last_speak
-0000cb80: 696e 675f 6465 7465 6374 2873 656c 6629  ing_detect(self)
-0000cb90: 202d 3e20 4f70 7469 6f6e 616c 5b64 6174   -> Optional[dat
-0000cba0: 6574 696d 655d 3a0a 2020 2020 2020 2020  etime]:.        
-0000cbb0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
-0000cbc0: 5370 6561 6b69 6e67 2073 6d61 7274 2064  Speaking smart d
-0000cbd0: 6574 6563 7469 6f6e 2065 7665 6e74 2e22  etection event."
-0000cbe0: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0000cbf0: 726e 2073 656c 662e 6c61 7374 5f73 6d61  rn self.last_sma
-0000cc00: 7274 5f61 7564 696f 5f64 6574 6563 7473  rt_audio_detects
-0000cc10: 2e67 6574 2853 6d61 7274 4465 7465 6374  .get(SmartDetect
-0000cc20: 4175 6469 6f54 7970 652e 5350 4541 4b29  AudioType.SPEAK)
-0000cc30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000cc40: 2020 2020 6465 6620 6973 5f73 7065 616b      def is_speak
-0000cc50: 696e 675f 6375 7272 656e 746c 795f 6465  ing_currently_de
-0000cc60: 7465 6374 6564 2873 656c 6629 202d 3e20  tected(self) -> 
-0000cc70: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0000cc80: 2249 7320 5370 6561 6b69 6e67 2063 7572  "Is Speaking cur
-0000cc90: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
-0000cca0: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
-0000ccb0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
-0000ccc0: 735f 6175 6469 6f5f 6465 7465 6374 6564  s_audio_detected
-0000ccd0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
-0000cce0: 6374 5479 7065 2e53 5045 414b 290a 0a20  ctType.SPEAK).. 
-0000ccf0: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-0000cd00: 5f73 7065 616b 696e 675f 6465 7465 6374  _speaking_detect
-0000cd10: 696f 6e28 7365 6c66 2c20 656e 6162 6c65  ion(self, enable
-0000cd20: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-0000cd30: 3a0a 2020 2020 2020 2020 2222 2254 6f67  :.        """Tog
-0000cd40: 676c 6573 2073 7065 616b 696e 6720 736d  gles speaking sm
-0000cd50: 6172 7420 6465 7465 6374 696f 6e2e 2052  art detection. R
-0000cd60: 6571 7569 7265 7320 6361 6d65 7261 2074  equires camera t
-0000cd70: 6f20 6861 7665 2073 6d61 7274 2064 6574  o have smart det
-0000cd80: 6563 7469 6f6e 2222 220a 0a20 2020 2020  ection"""..     
-0000cd90: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0000cda0: 7365 6c66 2e5f 7365 745f 6175 6469 6f5f  self._set_audio_
-0000cdb0: 6465 7465 6374 2853 6d61 7274 4465 7465  detect(SmartDete
-0000cdc0: 6374 4175 6469 6f54 7970 652e 5350 4541  ctAudioType.SPEA
-0000cdd0: 4b2c 2065 6e61 626c 6564 290a 0a20 2020  K, enabled)..   
-0000cde0: 2023 2062 6172 6b0a 0a20 2020 2040 7072   # bark..    @pr
-0000cdf0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-0000ce00: 616e 5f64 6574 6563 745f 6261 726b 2873  an_detect_bark(s
-0000ce10: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-0000ce20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000ce30: 662e 5f63 616e 5f64 6574 6563 745f 6175  f._can_detect_au
-0000ce40: 6469 6f28 536d 6172 7444 6574 6563 744f  dio(SmartDetectO
-0000ce50: 626a 6563 7454 7970 652e 4241 524b 290a  bjectType.BARK).
-0000ce60: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000ce70: 2020 2064 6566 2069 735f 6261 726b 5f64     def is_bark_d
-0000ce80: 6574 6563 7469 6f6e 5f6f 6e28 7365 6c66  etection_on(self
-0000ce90: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-0000cea0: 2020 2022 2222 4973 2042 6172 6b20 4465     """Is Bark De
-0000ceb0: 7465 6374 696f 6e20 6176 6169 6c61 626c  tection availabl
-0000cec0: 6520 616e 6420 656e 6162 6c65 6420 2863  e and enabled (c
-0000ced0: 616d 6572 6120 7769 6c6c 2070 726f 6475  amera will produ
-0000cee0: 6365 2062 6172 6b69 6e67 2073 6d61 7274  ce barking smart
-0000cef0: 0a20 2020 2020 2020 2064 6574 6563 7469  .        detecti
-0000cf00: 6f6e 2065 7665 6e74 7329 3f0a 2020 2020  on events)?.    
-0000cf10: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000cf20: 2072 6574 7572 6e20 7365 6c66 2e5f 6973   return self._is
-0000cf30: 5f61 7564 696f 5f65 6e61 626c 6564 2853  _audio_enabled(S
-0000cf40: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
-0000cf50: 5479 7065 2e42 4152 4b29 0a0a 2020 2020  Type.BARK)..    
-0000cf60: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000cf70: 6620 6c61 7374 5f62 6172 6b5f 6465 7465  f last_bark_dete
-0000cf80: 6374 5f65 7665 6e74 2873 656c 6629 202d  ct_event(self) -
-0000cf90: 3e20 4f70 7469 6f6e 616c 5b45 7665 6e74  > Optional[Event
-0000cfa0: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-0000cfb0: 7420 7468 6520 6c61 7374 2042 6172 6b20  t the last Bark 
-0000cfc0: 736d 6172 7420 6465 7465 6374 696f 6e20  smart detection 
-0000cfd0: 6576 656e 742e 2222 220a 0a20 2020 2020  event."""..     
-0000cfe0: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0000cff0: 6574 5f6c 6173 745f 736d 6172 745f 6175  et_last_smart_au
-0000d000: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
-0000d010: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
-0000d020: 6f54 7970 652e 4241 524b 290a 0a20 2020  oType.BARK)..   
-0000d030: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000d040: 6566 206c 6173 745f 6261 726b 5f64 6574  ef last_bark_det
-0000d050: 6563 7428 7365 6c66 2920 2d3e 204f 7074  ect(self) -> Opt
-0000d060: 696f 6e61 6c5b 6461 7465 7469 6d65 5d3a  ional[datetime]:
-0000d070: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000d080: 7468 6520 6c61 7374 2042 6172 6b20 736d  the last Bark sm
-0000d090: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
-0000d0a0: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-0000d0b0: 2072 6574 7572 6e20 7365 6c66 2e6c 6173   return self.las
-0000d0c0: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
-0000d0d0: 7465 6374 732e 6765 7428 536d 6172 7444  tects.get(SmartD
-0000d0e0: 6574 6563 7441 7564 696f 5479 7065 2e42  etectAudioType.B
-0000d0f0: 4152 4b29 0a0a 2020 2020 4070 726f 7065  ARK)..    @prope
-0000d100: 7274 790a 2020 2020 6465 6620 6973 5f62  rty.    def is_b
-0000d110: 6172 6b5f 6375 7272 656e 746c 795f 6465  ark_currently_de
-0000d120: 7465 6374 6564 2873 656c 6629 202d 3e20  tected(self) -> 
-0000d130: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0000d140: 2249 7320 4261 726b 2063 7572 7265 6e74  "Is Bark current
-0000d150: 6c79 2062 6569 6e67 2064 6574 6563 7465  ly being detecte
-0000d160: 6422 2222 0a0a 2020 2020 2020 2020 7265  d"""..        re
-0000d170: 7475 726e 2073 656c 662e 5f69 735f 6175  turn self._is_au
-0000d180: 6469 6f5f 6465 7465 6374 6564 2853 6d61  dio_detected(Sma
-0000d190: 7274 4465 7465 6374 4f62 6a65 6374 5479  rtDetectObjectTy
-0000d1a0: 7065 2e42 4152 4b29 0a0a 2020 2020 6173  pe.BARK)..    as
-0000d1b0: 796e 6320 6465 6620 7365 745f 6261 726b  ync def set_bark
-0000d1c0: 5f64 6574 6563 7469 6f6e 2873 656c 662c  _detection(self,
-0000d1d0: 2065 6e61 626c 6564 3a20 626f 6f6c 2920   enabled: bool) 
-0000d1e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000d1f0: 2022 2222 546f 6767 6c65 7320 6261 726b   """Toggles bark
-0000d200: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
-0000d210: 2e20 5265 7175 6972 6573 2063 616d 6572  . Requires camer
-0000d220: 6120 746f 2068 6176 6520 736d 6172 7420  a to have smart 
-0000d230: 6465 7465 6374 696f 6e22 2222 0a0a 2020  detection"""..  
-0000d240: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0000d250: 6974 2073 656c 662e 5f73 6574 5f61 7564  it self._set_aud
-0000d260: 696f 5f64 6574 6563 7428 536d 6172 7444  io_detect(SmartD
-0000d270: 6574 6563 7441 7564 696f 5479 7065 2e42  etectAudioType.B
-0000d280: 4152 4b2c 2065 6e61 626c 6564 290a 0a20  ARK, enabled).. 
-0000d290: 2020 2023 2063 6172 2061 6c61 726d 2028     # car alarm (
-0000d2a0: 6275 7267 6c61 7220 696e 2063 6f64 652c  burglar in code,
-0000d2b0: 2063 6172 2061 6c61 726d 2069 6e20 5072   car alarm in Pr
-0000d2c0: 6f74 6563 7420 5549 290a 0a20 2020 2040  otect UI)..    @
-0000d2d0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000d2e0: 2063 616e 5f64 6574 6563 745f 6361 725f   can_detect_car_
-0000d2f0: 616c 6172 6d28 7365 6c66 2920 2d3e 2062  alarm(self) -> b
-0000d300: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
-0000d310: 7572 6e20 7365 6c66 2e5f 6361 6e5f 6465  urn self._can_de
-0000d320: 7465 6374 5f61 7564 696f 2853 6d61 7274  tect_audio(Smart
-0000d330: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
-0000d340: 2e42 5552 474c 4152 290a 0a20 2020 2040  .BURGLAR)..    @
-0000d350: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000d360: 2069 735f 6361 725f 616c 6172 6d5f 6465   is_car_alarm_de
-0000d370: 7465 6374 696f 6e5f 6f6e 2873 656c 6629  tection_on(self)
-0000d380: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000d390: 2020 2222 2249 7320 4361 7220 416c 6172    """Is Car Alar
-0000d3a0: 6d20 4465 7465 6374 696f 6e20 6176 6169  m Detection avai
-0000d3b0: 6c61 626c 6520 616e 6420 656e 6162 6c65  lable and enable
-0000d3c0: 6420 2863 616d 6572 6120 7769 6c6c 2070  d (camera will p
-0000d3d0: 726f 6475 6365 2063 6172 2061 6c61 726d  roduce car alarm
-0000d3e0: 2073 6d61 7274 0a20 2020 2020 2020 2064   smart.        d
-0000d3f0: 6574 6563 7469 6f6e 2065 7665 6e74 7329  etection events)
-0000d400: 3f0a 2020 2020 2020 2020 2222 220a 0a20  ?.        """.. 
-0000d410: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000d420: 6c66 2e5f 6973 5f61 7564 696f 5f65 6e61  lf._is_audio_ena
-0000d430: 626c 6564 2853 6d61 7274 4465 7465 6374  bled(SmartDetect
-0000d440: 4f62 6a65 6374 5479 7065 2e42 5552 474c  ObjectType.BURGL
-0000d450: 4152 290a 0a20 2020 2040 7072 6f70 6572  AR)..    @proper
-0000d460: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
-0000d470: 6361 725f 616c 6172 6d5f 6465 7465 6374  car_alarm_detect
-0000d480: 5f65 7665 6e74 2873 656c 6629 202d 3e20  _event(self) -> 
-0000d490: 4f70 7469 6f6e 616c 5b45 7665 6e74 5d3a  Optional[Event]:
-0000d4a0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000d4b0: 7468 6520 6c61 7374 2043 6172 2041 6c61  the last Car Ala
-0000d4c0: 726d 2073 6d61 7274 2064 6574 6563 7469  rm smart detecti
-0000d4d0: 6f6e 2065 7665 6e74 2e22 2222 0a0a 2020  on event."""..  
-0000d4e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d4f0: 662e 6765 745f 6c61 7374 5f73 6d61 7274  f.get_last_smart
-0000d500: 5f61 7564 696f 5f64 6574 6563 745f 6576  _audio_detect_ev
-0000d510: 656e 7428 536d 6172 7444 6574 6563 7441  ent(SmartDetectA
-0000d520: 7564 696f 5479 7065 2e42 5552 474c 4152  udioType.BURGLAR
-0000d530: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-0000d540: 0a20 2020 2064 6566 206c 6173 745f 6361  .    def last_ca
-0000d550: 725f 616c 6172 6d5f 6465 7465 6374 2873  r_alarm_detect(s
-0000d560: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-0000d570: 5b64 6174 6574 696d 655d 3a0a 2020 2020  [datetime]:.    
-0000d580: 2020 2020 2222 2247 6574 2074 6865 206c      """Get the l
-0000d590: 6173 7420 4361 7220 416c 6172 6d20 736d  ast Car Alarm sm
-0000d5a0: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
-0000d5b0: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-0000d5c0: 2072 6574 7572 6e20 7365 6c66 2e6c 6173   return self.las
-0000d5d0: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
-0000d5e0: 7465 6374 732e 6765 7428 536d 6172 7444  tects.get(SmartD
-0000d5f0: 6574 6563 7441 7564 696f 5479 7065 2e42  etectAudioType.B
-0000d600: 5552 474c 4152 290a 0a20 2020 2040 7072  URGLAR)..    @pr
-0000d610: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
-0000d620: 735f 6361 725f 616c 6172 6d5f 6375 7272  s_car_alarm_curr
-0000d630: 656e 746c 795f 6465 7465 6374 6564 2873  ently_detected(s
-0000d640: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-0000d650: 2020 2020 2020 2222 2249 7320 4361 7220        """Is Car 
-0000d660: 416c 6172 6d20 6375 7272 656e 746c 7920  Alarm currently 
-0000d670: 6265 696e 6720 6465 7465 6374 6564 2222  being detected""
-0000d680: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0000d690: 6e20 7365 6c66 2e5f 6973 5f61 7564 696f  n self._is_audio
-0000d6a0: 5f64 6574 6563 7465 6428 536d 6172 7444  _detected(SmartD
-0000d6b0: 6574 6563 744f 626a 6563 7454 7970 652e  etectObjectType.
-0000d6c0: 4255 5247 4c41 5229 0a0a 2020 2020 6173  BURGLAR)..    as
-0000d6d0: 796e 6320 6465 6620 7365 745f 6361 725f  ync def set_car_
-0000d6e0: 616c 6172 6d5f 6465 7465 6374 696f 6e28  alarm_detection(
-0000d6f0: 7365 6c66 2c20 656e 6162 6c65 643a 2062  self, enabled: b
-0000d700: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
-0000d710: 2020 2020 2020 2222 2254 6f67 676c 6573        """Toggles
-0000d720: 2063 6172 5f61 6c61 726d 2073 6d61 7274   car_alarm smart
-0000d730: 2064 6574 6563 7469 6f6e 2e20 5265 7175   detection. Requ
-0000d740: 6972 6573 2063 616d 6572 6120 746f 2068  ires camera to h
-0000d750: 6176 6520 736d 6172 7420 6465 7465 6374  ave smart detect
-0000d760: 696f 6e22 2222 0a0a 2020 2020 2020 2020  ion"""..        
-0000d770: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-0000d780: 662e 5f73 6574 5f61 7564 696f 5f64 6574  f._set_audio_det
-0000d790: 6563 7428 536d 6172 7444 6574 6563 7441  ect(SmartDetectA
-0000d7a0: 7564 696f 5479 7065 2e42 5552 474c 4152  udioType.BURGLAR
-0000d7b0: 2c20 656e 6162 6c65 6429 0a0a 2020 2020  , enabled)..    
-0000d7c0: 2320 6361 7220 686f 726e 0a0a 2020 2020  # car horn..    
-0000d7d0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000d7e0: 6620 6361 6e5f 6465 7465 6374 5f63 6172  f can_detect_car
-0000d7f0: 5f68 6f72 6e28 7365 6c66 2920 2d3e 2062  _horn(self) -> b
-0000d800: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
-0000d810: 7572 6e20 7365 6c66 2e5f 6361 6e5f 6465  urn self._can_de
-0000d820: 7465 6374 5f61 7564 696f 2853 6d61 7274  tect_audio(Smart
-0000d830: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
-0000d840: 2e43 4152 5f48 4f52 4e29 0a0a 2020 2020  .CAR_HORN)..    
-0000d850: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000d860: 6620 6973 5f63 6172 5f68 6f72 6e5f 6465  f is_car_horn_de
-0000d870: 7465 6374 696f 6e5f 6f6e 2873 656c 6629  tection_on(self)
-0000d880: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000d890: 2020 2222 2249 7320 4361 7220 486f 726e    """Is Car Horn
-0000d8a0: 2044 6574 6563 7469 6f6e 2061 7661 696c   Detection avail
-0000d8b0: 6162 6c65 2061 6e64 2065 6e61 626c 6564  able and enabled
-0000d8c0: 2028 6361 6d65 7261 2077 696c 6c20 7072   (camera will pr
-0000d8d0: 6f64 7563 6520 6361 7220 686f 726e 2073  oduce car horn s
-0000d8e0: 6d61 7274 0a20 2020 2020 2020 2064 6574  mart.        det
-0000d8f0: 6563 7469 6f6e 2065 7665 6e74 7329 3f0a  ection events)?.
-0000d900: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000d910: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000d920: 2e5f 6973 5f61 7564 696f 5f65 6e61 626c  ._is_audio_enabl
-0000d930: 6564 2853 6d61 7274 4465 7465 6374 4f62  ed(SmartDetectOb
-0000d940: 6a65 6374 5479 7065 2e43 4152 5f48 4f52  jectType.CAR_HOR
-0000d950: 4e29 0a0a 2020 2020 4070 726f 7065 7274  N)..    @propert
-0000d960: 790a 2020 2020 6465 6620 6c61 7374 5f63  y.    def last_c
-0000d970: 6172 5f68 6f72 6e5f 6465 7465 6374 5f65  ar_horn_detect_e
-0000d980: 7665 6e74 2873 656c 6629 202d 3e20 4f70  vent(self) -> Op
-0000d990: 7469 6f6e 616c 5b45 7665 6e74 5d3a 0a20  tional[Event]:. 
-0000d9a0: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-0000d9b0: 6520 6c61 7374 2043 6172 2048 6f72 6e20  e last Car Horn 
-0000d9c0: 736d 6172 7420 6465 7465 6374 696f 6e20  smart detection 
-0000d9d0: 6576 656e 742e 2222 220a 0a20 2020 2020  event."""..     
-0000d9e0: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0000d9f0: 6574 5f6c 6173 745f 736d 6172 745f 6175  et_last_smart_au
-0000da00: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
-0000da10: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
-0000da20: 6f54 7970 652e 4341 525f 484f 524e 290a  oType.CAR_HORN).
-0000da30: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000da40: 2020 2064 6566 206c 6173 745f 6361 725f     def last_car_
-0000da50: 686f 726e 5f64 6574 6563 7428 7365 6c66  horn_detect(self
-0000da60: 2920 2d3e 204f 7074 696f 6e61 6c5b 6461  ) -> Optional[da
-0000da70: 7465 7469 6d65 5d3a 0a20 2020 2020 2020  tetime]:.       
-0000da80: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
-0000da90: 2043 6172 2048 6f72 6e20 736d 6172 7420   Car Horn smart 
-0000daa0: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
-0000dab0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-0000dac0: 7572 6e20 7365 6c66 2e6c 6173 745f 736d  urn self.last_sm
-0000dad0: 6172 745f 6175 6469 6f5f 6465 7465 6374  art_audio_detect
-0000dae0: 732e 6765 7428 536d 6172 7444 6574 6563  s.get(SmartDetec
-0000daf0: 7441 7564 696f 5479 7065 2e43 4152 5f48  tAudioType.CAR_H
-0000db00: 4f52 4e29 0a0a 2020 2020 4070 726f 7065  ORN)..    @prope
-0000db10: 7274 790a 2020 2020 6465 6620 6973 5f63  rty.    def is_c
-0000db20: 6172 5f68 6f72 6e5f 6375 7272 656e 746c  ar_horn_currentl
-0000db30: 795f 6465 7465 6374 6564 2873 656c 6629  y_detected(self)
-0000db40: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000db50: 2020 2222 2249 7320 4361 7220 486f 726e    """Is Car Horn
-0000db60: 2063 7572 7265 6e74 6c79 2062 6569 6e67   currently being
-0000db70: 2064 6574 6563 7465 6422 2222 0a0a 2020   detected"""..  
-0000db80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000db90: 662e 5f69 735f 6175 6469 6f5f 6465 7465  f._is_audio_dete
-0000dba0: 6374 6564 2853 6d61 7274 4465 7465 6374  cted(SmartDetect
-0000dbb0: 4f62 6a65 6374 5479 7065 2e43 4152 5f48  ObjectType.CAR_H
-0000dbc0: 4f52 4e29 0a0a 2020 2020 6173 796e 6320  ORN)..    async 
-0000dbd0: 6465 6620 7365 745f 6361 725f 686f 726e  def set_car_horn
-0000dbe0: 5f64 6574 6563 7469 6f6e 2873 656c 662c  _detection(self,
-0000dbf0: 2065 6e61 626c 6564 3a20 626f 6f6c 2920   enabled: bool) 
-0000dc00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000dc10: 2022 2222 546f 6767 6c65 7320 6361 725f   """Toggles car_
-0000dc20: 686f 726e 2073 6d61 7274 2064 6574 6563  horn smart detec
-0000dc30: 7469 6f6e 2e20 5265 7175 6972 6573 2063  tion. Requires c
-0000dc40: 616d 6572 6120 746f 2068 6176 6520 736d  amera to have sm
-0000dc50: 6172 7420 6465 7465 6374 696f 6e22 2222  art detection"""
-0000dc60: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000dc70: 2061 7761 6974 2073 656c 662e 5f73 6574   await self._set
-0000dc80: 5f61 7564 696f 5f64 6574 6563 7428 536d  _audio_detect(Sm
-0000dc90: 6172 7444 6574 6563 7441 7564 696f 5479  artDetectAudioTy
-0000dca0: 7065 2e43 4152 5f48 4f52 4e2c 2065 6e61  pe.CAR_HORN, ena
-0000dcb0: 626c 6564 290a 0a20 2020 2023 2067 6c61  bled)..    # gla
-0000dcc0: 7373 2062 7265 616b 0a0a 2020 2020 4070  ss break..    @p
-0000dcd0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000dce0: 6361 6e5f 6465 7465 6374 5f67 6c61 7373  can_detect_glass
-0000dcf0: 5f62 7265 616b 2873 656c 6629 202d 3e20  _break(self) -> 
-0000dd00: 626f 6f6c 3a0a 2020 2020 2020 2020 7265  bool:.        re
-0000dd10: 7475 726e 2073 656c 662e 5f63 616e 5f64  turn self._can_d
-0000dd20: 6574 6563 745f 6175 6469 6f28 536d 6172  etect_audio(Smar
-0000dd30: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
-0000dd40: 652e 474c 4153 535f 4252 4541 4b29 0a0a  e.GLASS_BREAK)..
-0000dd50: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000dd60: 2020 6465 6620 6973 5f67 6c61 7373 5f62    def is_glass_b
-0000dd70: 7265 616b 5f64 6574 6563 7469 6f6e 5f6f  reak_detection_o
-0000dd80: 6e28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  n(self) -> bool:
-0000dd90: 0a20 2020 2020 2020 2022 2222 4973 2047  .        """Is G
-0000dda0: 6c61 7373 2042 7265 616b 2061 7661 696c  lass Break avail
-0000ddb0: 6162 6c65 2061 6e64 2065 6e61 626c 6564  able and enabled
-0000ddc0: 2028 6361 6d65 7261 2077 696c 6c20 7072   (camera will pr
-0000ddd0: 6f64 7563 6520 676c 6173 7320 6272 6561  oduce glass brea
-0000dde0: 6b20 736d 6172 740a 2020 2020 2020 2020  k smart.        
-0000ddf0: 6465 7465 6374 696f 6e20 6576 656e 7473  detection events
-0000de00: 293f 0a20 2020 2020 2020 2022 2222 0a0a  )?.        """..
-0000de10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000de20: 656c 662e 5f69 735f 6175 6469 6f5f 656e  elf._is_audio_en
-0000de30: 6162 6c65 6428 536d 6172 7444 6574 6563  abled(SmartDetec
-0000de40: 744f 626a 6563 7454 7970 652e 474c 4153  tObjectType.GLAS
-0000de50: 535f 4252 4541 4b29 0a0a 2020 2020 4070  S_BREAK)..    @p
-0000de60: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000de70: 6c61 7374 5f67 6c61 7373 5f62 7265 616b  last_glass_break
-0000de80: 5f64 6574 6563 745f 6576 656e 7428 7365  _detect_event(se
-0000de90: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-0000dea0: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
-0000deb0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
-0000dec0: 476c 6173 7320 4272 6561 6b20 736d 6172  Glass Break smar
-0000ded0: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
-0000dee0: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
-0000def0: 6574 7572 6e20 7365 6c66 2e67 6574 5f6c  eturn self.get_l
-0000df00: 6173 745f 736d 6172 745f 6175 6469 6f5f  ast_smart_audio_
-0000df10: 6465 7465 6374 5f65 7665 6e74 2853 6d61  detect_event(Sma
-0000df20: 7274 4465 7465 6374 4175 6469 6f54 7970  rtDetectAudioTyp
-0000df30: 652e 474c 4153 535f 4252 4541 4b29 0a0a  e.GLASS_BREAK)..
-0000df40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000df50: 2020 6465 6620 6c61 7374 5f67 6c61 7373    def last_glass
-0000df60: 5f62 7265 616b 5f64 6574 6563 7428 7365  _break_detect(se
-0000df70: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-0000df80: 6461 7465 7469 6d65 5d3a 0a20 2020 2020  datetime]:.     
-0000df90: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
-0000dfa0: 7374 2047 6c61 7373 2042 7265 616b 2073  st Glass Break s
-0000dfb0: 6d61 7274 2064 6574 6563 7469 6f6e 2065  mart detection e
-0000dfc0: 7665 6e74 2e22 2222 0a0a 2020 2020 2020  vent."""..      
-0000dfd0: 2020 7265 7475 726e 2073 656c 662e 6c61    return self.la
-0000dfe0: 7374 5f73 6d61 7274 5f61 7564 696f 5f64  st_smart_audio_d
-0000dff0: 6574 6563 7473 2e67 6574 2853 6d61 7274  etects.get(Smart
-0000e000: 4465 7465 6374 4175 6469 6f54 7970 652e  DetectAudioType.
-0000e010: 474c 4153 535f 4252 4541 4b29 0a0a 2020  GLASS_BREAK)..  
-0000e020: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000e030: 6465 6620 6973 5f67 6c61 7373 5f62 7265  def is_glass_bre
-0000e040: 616b 5f63 7572 7265 6e74 6c79 5f64 6574  ak_currently_det
-0000e050: 6563 7465 6428 7365 6c66 2920 2d3e 2062  ected(self) -> b
-0000e060: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-0000e070: 4973 2047 6c61 7373 2042 7265 616b 2063  Is Glass Break c
-0000e080: 7572 7265 6e74 6c79 2062 6569 6e67 2064  urrently being d
-0000e090: 6574 6563 7465 6422 2222 0a0a 2020 2020  etected"""..    
-0000e0a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e0b0: 5f69 735f 6175 6469 6f5f 6465 7465 6374  _is_audio_detect
-0000e0c0: 6564 2853 6d61 7274 4465 7465 6374 4f62  ed(SmartDetectOb
-0000e0d0: 6a65 6374 5479 7065 2e47 4c41 5353 5f42  jectType.GLASS_B
-0000e0e0: 5245 414b 290a 0a20 2020 2061 7379 6e63  REAK)..    async
-0000e0f0: 2064 6566 2073 6574 5f67 6c61 7373 5f62   def set_glass_b
-0000e100: 7265 616b 5f64 6574 6563 7469 6f6e 2873  reak_detection(s
-0000e110: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
-0000e120: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-0000e130: 2020 2020 2022 2222 546f 6767 6c65 7320       """Toggles 
-0000e140: 676c 6173 735f 6272 6561 6b20 736d 6172  glass_break smar
-0000e150: 7420 6465 7465 6374 696f 6e2e 2052 6571  t detection. Req
-0000e160: 7569 7265 7320 6361 6d65 7261 2074 6f20  uires camera to 
-0000e170: 6861 7665 2073 6d61 7274 2064 6574 6563  have smart detec
-0000e180: 7469 6f6e 2222 220a 0a20 2020 2020 2020  tion"""..       
-0000e190: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0000e1a0: 6c66 2e5f 7365 745f 6175 6469 6f5f 6465  lf._set_audio_de
-0000e1b0: 7465 6374 2853 6d61 7274 4465 7465 6374  tect(SmartDetect
-0000e1c0: 4175 6469 6f54 7970 652e 474c 4153 535f  AudioType.GLASS_
-0000e1d0: 4252 4541 4b2c 2065 6e61 626c 6564 290a  BREAK, enabled).
-0000e1e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000e1f0: 2020 2064 6566 2069 735f 7269 6e67 696e     def is_ringin
-0000e200: 6728 7365 6c66 2920 2d3e 2062 6f6f 6c3a  g(self) -> bool:
-0000e210: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e220: 2e5f 6c61 7374 5f72 696e 675f 7469 6d65  ._last_ring_time
-0000e230: 6f75 7420 6973 204e 6f6e 653a 0a20 2020  out is None:.   
-0000e240: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000e250: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
-0000e260: 7475 726e 2075 7463 5f6e 6f77 2829 203c  turn utc_now() <
-0000e270: 2073 656c 662e 5f6c 6173 745f 7269 6e67   self._last_ring
-0000e280: 5f74 696d 656f 7574 0a0a 2020 2020 4070  _timeout..    @p
-0000e290: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e2a0: 6368 696d 655f 7479 7065 2873 656c 6629  chime_type(self)
-0000e2b0: 202d 3e20 4368 696d 6554 7970 653a 0a20   -> ChimeType:. 
-0000e2c0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000e2d0: 6869 6d65 5f64 7572 6174 696f 6e2e 746f  hime_duration.to
-0000e2e0: 7461 6c5f 7365 636f 6e64 7328 2920 3d3d  tal_seconds() ==
-0000e2f0: 2030 2e33 3a0a 2020 2020 2020 2020 2020   0.3:.          
-0000e300: 2020 7265 7475 726e 2043 6869 6d65 5479    return ChimeTy
-0000e310: 7065 2e4d 4543 4841 4e49 4341 4c0a 2020  pe.MECHANICAL.  
-0000e320: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000e330: 696d 655f 6475 7261 7469 6f6e 2e74 6f74  ime_duration.tot
-0000e340: 616c 5f73 6563 6f6e 6473 2829 203e 2030  al_seconds() > 0
-0000e350: 2e33 3a0a 2020 2020 2020 2020 2020 2020  .3:.            
-0000e360: 7265 7475 726e 2043 6869 6d65 5479 7065  return ChimeType
-0000e370: 2e44 4947 4954 414c 0a20 2020 2020 2020  .DIGITAL.       
-0000e380: 2072 6574 7572 6e20 4368 696d 6554 7970   return ChimeTyp
-0000e390: 652e 4e4f 4e45 0a0a 2020 2020 4070 726f  e.NONE..    @pro
-0000e3a0: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
-0000e3b0: 5f64 6967 6974 616c 5f63 6869 6d65 2873  _digital_chime(s
-0000e3c0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-0000e3d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e3e0: 662e 6368 696d 655f 7479 7065 2069 7320  f.chime_type is 
-0000e3f0: 4368 696d 6554 7970 652e 4449 4749 5441  ChimeType.DIGITA
-0000e400: 4c0a 0a20 2020 2040 7072 6f70 6572 7479  L..    @property
-0000e410: 0a20 2020 2064 6566 2068 6967 685f 6361  .    def high_ca
-0000e420: 6d65 7261 5f63 6861 6e6e 656c 2873 656c  mera_channel(sel
-0000e430: 6629 202d 3e20 4f70 7469 6f6e 616c 5b43  f) -> Optional[C
-0000e440: 616d 6572 6143 6861 6e6e 656c 5d3a 0a20  ameraChannel]:. 
-0000e450: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-0000e460: 6c66 2e63 6861 6e6e 656c 7329 203e 3d20  lf.channels) >= 
-0000e470: 333a 0a20 2020 2020 2020 2020 2020 2072  3:.            r
-0000e480: 6574 7572 6e20 7365 6c66 2e63 6861 6e6e  eturn self.chann
-0000e490: 656c 735b 305d 0a20 2020 2020 2020 2072  els[0].        r
-0000e4a0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000e4b0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000e4c0: 6620 6d65 6469 756d 5f63 616d 6572 615f  f medium_camera_
-0000e4d0: 6368 616e 6e65 6c28 7365 6c66 2920 2d3e  channel(self) ->
-0000e4e0: 204f 7074 696f 6e61 6c5b 4361 6d65 7261   Optional[Camera
-0000e4f0: 4368 616e 6e65 6c5d 3a0a 2020 2020 2020  Channel]:.      
-0000e500: 2020 6966 206c 656e 2873 656c 662e 6368    if len(self.ch
-0000e510: 616e 6e65 6c73 2920 3e3d 2033 3a0a 2020  annels) >= 3:.  
-0000e520: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e530: 2073 656c 662e 6368 616e 6e65 6c73 5b31   self.channels[1
-0000e540: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-0000e550: 204e 6f6e 650a 0a20 2020 2040 7072 6f70   None..    @prop
-0000e560: 6572 7479 0a20 2020 2064 6566 206c 6f77  erty.    def low
-0000e570: 5f63 616d 6572 615f 6368 616e 6e65 6c28  _camera_channel(
-0000e580: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-0000e590: 6c5b 4361 6d65 7261 4368 616e 6e65 6c5d  l[CameraChannel]
-0000e5a0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
-0000e5b0: 2873 656c 662e 6368 616e 6e65 6c73 2920  (self.channels) 
-0000e5c0: 3e3d 2033 3a0a 2020 2020 2020 2020 2020  >= 3:.          
-0000e5d0: 2020 7265 7475 726e 2073 656c 662e 6368    return self.ch
-0000e5e0: 616e 6e65 6c73 5b32 5d0a 2020 2020 2020  annels[2].      
-0000e5f0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-0000e600: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000e610: 2064 6566 2064 6566 6175 6c74 5f63 616d   def default_cam
-0000e620: 6572 615f 6368 616e 6e65 6c28 7365 6c66  era_channel(self
-0000e630: 2920 2d3e 204f 7074 696f 6e61 6c5b 4361  ) -> Optional[Ca
-0000e640: 6d65 7261 4368 616e 6e65 6c5d 3a0a 2020  meraChannel]:.  
-0000e650: 2020 2020 2020 666f 7220 6368 616e 6e65        for channe
-0000e660: 6c20 696e 205b 0a20 2020 2020 2020 2020  l in [.         
-0000e670: 2020 2073 656c 662e 6869 6768 5f63 616d     self.high_cam
-0000e680: 6572 615f 6368 616e 6e65 6c2c 0a20 2020  era_channel,.   
-0000e690: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-0000e6a0: 6469 756d 5f63 616d 6572 615f 6368 616e  dium_camera_chan
-0000e6b0: 6e65 6c2c 0a20 2020 2020 2020 2020 2020  nel,.           
-0000e6c0: 2073 656c 662e 6c6f 775f 6361 6d65 7261   self.low_camera
-0000e6d0: 5f63 6861 6e6e 656c 2c0a 2020 2020 2020  _channel,.      
-0000e6e0: 2020 5d3a 0a20 2020 2020 2020 2020 2020    ]:.           
-0000e6f0: 2069 6620 6368 616e 6e65 6c20 6973 206e   if channel is n
-0000e700: 6f74 204e 6f6e 6520 616e 6420 6368 616e  ot None and chan
-0000e710: 6e65 6c2e 6973 5f72 7473 705f 656e 6162  nel.is_rtsp_enab
-0000e720: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-0000e730: 2020 2020 2072 6574 7572 6e20 6368 616e       return chan
-0000e740: 6e65 6c0a 2020 2020 2020 2020 7265 7475  nel.        retu
-0000e750: 726e 2073 656c 662e 6869 6768 5f63 616d  rn self.high_cam
-0000e760: 6572 615f 6368 616e 6e65 6c0a 0a20 2020  era_channel..   
-0000e770: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000e780: 6566 2070 6163 6b61 6765 5f63 616d 6572  ef package_camer
-0000e790: 615f 6368 616e 6e65 6c28 7365 6c66 2920  a_channel(self) 
-0000e7a0: 2d3e 204f 7074 696f 6e61 6c5b 4361 6d65  -> Optional[Came
-0000e7b0: 7261 4368 616e 6e65 6c5d 3a0a 2020 2020  raChannel]:.    
-0000e7c0: 2020 2020 6966 2073 656c 662e 6665 6174      if self.feat
-0000e7d0: 7572 655f 666c 6167 732e 6861 735f 7061  ure_flags.has_pa
-0000e7e0: 636b 6167 655f 6361 6d65 7261 2061 6e64  ckage_camera and
-0000e7f0: 206c 656e 2873 656c 662e 6368 616e 6e65   len(self.channe
-0000e800: 6c73 2920 3d3d 2034 3a0a 2020 2020 2020  ls) == 4:.      
-0000e810: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e820: 662e 6368 616e 6e65 6c73 5b33 5d0a 2020  f.channels[3].  
-0000e830: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000e840: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-0000e850: 0a20 2020 2064 6566 2069 735f 6869 6768  .    def is_high
-0000e860: 5f66 7073 5f65 6e61 626c 6564 2873 656c  _fps_enabled(sel
-0000e870: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-0000e880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e890: 7669 6465 6f5f 6d6f 6465 203d 3d20 5669  video_mode == Vi
-0000e8a0: 6465 6f4d 6f64 652e 4849 4748 5f46 5053  deoMode.HIGH_FPS
-0000e8b0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000e8c0: 2020 2020 6465 6620 6973 5f76 6964 656f      def is_video
-0000e8d0: 5f72 6561 6479 2873 656c 6629 202d 3e20  _ready(self) -> 
-0000e8e0: 626f 6f6c 3a0a 2020 2020 2020 2020 7265  bool:.        re
-0000e8f0: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
-0000e900: 2020 2073 656c 662e 6665 6174 7572 655f     self.feature_
-0000e910: 666c 6167 732e 6c65 6e73 5f74 7970 6520  flags.lens_type 
-0000e920: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
-0000e930: 2020 2020 6f72 2073 656c 662e 6665 6174      or self.feat
-0000e940: 7572 655f 666c 6167 732e 6c65 6e73 5f74  ure_flags.lens_t
-0000e950: 7970 6520 213d 204c 656e 7354 7970 652e  ype != LensType.
-0000e960: 4e4f 4e45 0a20 2020 2020 2020 2029 0a0a  NONE.        )..
-0000e970: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000e980: 2020 6465 6620 6861 735f 7265 6d6f 7661    def has_remova
-0000e990: 626c 655f 6c65 6e73 2873 656c 6629 202d  ble_lens(self) -
-0000e9a0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000e9b0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
-0000e9c0: 2020 2020 2073 656c 662e 6665 6174 7572       self.featur
-0000e9d0: 655f 666c 6167 732e 686f 7470 6c75 6720  e_flags.hotplug 
-0000e9e0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-0000e9f0: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-0000ea00: 2e66 6561 7475 7265 5f66 6c61 6773 2e68  .feature_flags.h
-0000ea10: 6f74 706c 7567 2e76 6964 656f 2069 7320  otplug.video is 
-0000ea20: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000ea30: 2029 0a0a 2020 2020 4070 726f 7065 7274   )..    @propert
-0000ea40: 790a 2020 2020 6465 6620 6861 735f 7265  y.    def has_re
-0000ea50: 6d6f 7661 626c 655f 7370 6561 6b65 7228  movable_speaker(
-0000ea60: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000ea70: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
-0000ea80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ea90: 2e66 6561 7475 7265 5f66 6c61 6773 2e68  .feature_flags.h
-0000eaa0: 6f74 706c 7567 2069 7320 6e6f 7420 4e6f  otplug is not No
-0000eab0: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
-0000eac0: 6e64 2073 656c 662e 6665 6174 7572 655f  nd self.feature_
-0000ead0: 666c 6167 732e 686f 7470 6c75 672e 6175  flags.hotplug.au
-0000eae0: 6469 6f20 6973 206e 6f74 204e 6f6e 650a  dio is not None.
-0000eaf0: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-0000eb00: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000eb10: 2068 6173 5f6d 6963 2873 656c 6629 202d   has_mic(self) -
-0000eb20: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000eb30: 7265 7475 726e 2073 656c 662e 6665 6174  return self.feat
-0000eb40: 7572 655f 666c 6167 732e 6861 735f 6d69  ure_flags.has_mi
-0000eb50: 6320 6f72 2073 656c 662e 6861 735f 7265  c or self.has_re
-0000eb60: 6d6f 7661 626c 655f 7370 6561 6b65 720a  movable_speaker.
-0000eb70: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000eb80: 2020 2064 6566 2068 6173 5f63 6f6c 6f72     def has_color
-0000eb90: 5f6e 6967 6874 5f76 6973 696f 6e28 7365  _night_vision(se
-0000eba0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-0000ebb0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-0000ebc0: 2020 2020 2020 7365 6c66 2e66 6561 7475        self.featu
-0000ebd0: 7265 5f66 6c61 6773 2e68 6f74 706c 7567  re_flags.hotplug
-0000ebe0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000ebf0: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-0000ec00: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
-0000ec10: 686f 7470 6c75 672e 6578 7465 6e64 6572  hotplug.extender
-0000ec20: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000ec30: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-0000ec40: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
-0000ec50: 686f 7470 6c75 672e 6578 7465 6e64 6572  hotplug.extender
-0000ec60: 2e69 735f 6174 7461 6368 6564 2069 7320  .is_attached is 
-0000ec70: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000ec80: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000ec90: 7265 7475 726e 2073 656c 662e 6665 6174  return self.feat
-0000eca0: 7572 655f 666c 6167 732e 686f 7470 6c75  ure_flags.hotplu
-0000ecb0: 672e 6578 7465 6e64 6572 2e69 735f 6174  g.extender.is_at
-0000ecc0: 7461 6368 6564 0a0a 2020 2020 2020 2020  tached..        
-0000ecd0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-0000ece0: 2020 6465 6620 7365 745f 7269 6e67 5f74    def set_ring_t
-0000ecf0: 696d 656f 7574 2873 656c 6629 202d 3e20  imeout(self) -> 
-0000ed00: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
-0000ed10: 6c66 2e5f 6c61 7374 5f72 696e 675f 7469  lf._last_ring_ti
-0000ed20: 6d65 6f75 7420 3d20 7574 635f 6e6f 7728  meout = utc_now(
-0000ed30: 2920 2b20 4556 454e 545f 5049 4e47 5f49  ) + EVENT_PING_I
-0000ed40: 4e54 4552 5641 4c0a 2020 2020 2020 2020  NTERVAL.        
-0000ed50: 7365 6c66 2e5f 6576 656e 745f 6361 6c6c  self._event_call
-0000ed60: 6261 636b 5f70 696e 6728 290a 0a20 2020  back_ping()..   
-0000ed70: 2064 6566 2067 6574 5f70 7269 7661 6379   def get_privacy
-0000ed80: 5f7a 6f6e 6528 7365 6c66 2920 2d3e 2074  _zone(self) -> t
-0000ed90: 7570 6c65 5b4f 7074 696f 6e61 6c5b 696e  uple[Optional[in
-0000eda0: 745d 2c20 4f70 7469 6f6e 616c 5b43 616d  t], Optional[Cam
-0000edb0: 6572 615a 6f6e 655d 5d3a 0a20 2020 2020  eraZone]]:.     
-0000edc0: 2020 2066 6f72 2069 6e64 6578 2c20 7a6f     for index, zo
-0000edd0: 6e65 2069 6e20 656e 756d 6572 6174 6528  ne in enumerate(
-0000ede0: 7365 6c66 2e70 7269 7661 6379 5f7a 6f6e  self.privacy_zon
-0000edf0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-0000ee00: 2069 6620 7a6f 6e65 2e6e 616d 6520 3d3d   if zone.name ==
-0000ee10: 2050 5249 5641 4359 5f5a 4f4e 455f 4e41   PRIVACY_ZONE_NA
-0000ee20: 4d45 3a0a 2020 2020 2020 2020 2020 2020  ME:.            
-0000ee30: 2020 2020 7265 7475 726e 2069 6e64 6578      return index
-0000ee40: 2c20 7a6f 6e65 0a20 2020 2020 2020 2072  , zone.        r
-0000ee50: 6574 7572 6e20 4e6f 6e65 2c20 4e6f 6e65  eturn None, None
-0000ee60: 0a0a 2020 2020 6465 6620 6164 645f 7072  ..    def add_pr
-0000ee70: 6976 6163 795f 7a6f 6e65 2873 656c 6629  ivacy_zone(self)
-0000ee80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000ee90: 2020 696e 6465 782c 205f 203d 2073 656c    index, _ = sel
-0000eea0: 662e 6765 745f 7072 6976 6163 795f 7a6f  f.get_privacy_zo
-0000eeb0: 6e65 2829 0a20 2020 2020 2020 2069 6620  ne().        if 
-0000eec0: 696e 6465 7820 6973 204e 6f6e 653a 0a20  index is None:. 
-0000eed0: 2020 2020 2020 2020 2020 207a 6f6e 655f             zone_
-0000eee0: 6964 203d 2030 0a20 2020 2020 2020 2020  id = 0.         
-0000eef0: 2020 2069 6620 6c65 6e28 7365 6c66 2e70     if len(self.p
-0000ef00: 7269 7661 6379 5f7a 6f6e 6573 2920 3e20  rivacy_zones) > 
-0000ef10: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000ef20: 2020 207a 6f6e 655f 6964 203d 2073 656c     zone_id = sel
-0000ef30: 662e 7072 6976 6163 795f 7a6f 6e65 735b  f.privacy_zones[
-0000ef40: 2d31 5d2e 6964 202b 2031 0a0a 2020 2020  -1].id + 1..    
-0000ef50: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-0000ef60: 7661 6379 5f7a 6f6e 6573 2e61 7070 656e  vacy_zones.appen
-0000ef70: 6428 4361 6d65 7261 5a6f 6e65 2e63 7265  d(CameraZone.cre
-0000ef80: 6174 655f 7072 6976 6163 795f 7a6f 6e65  ate_privacy_zone
-0000ef90: 287a 6f6e 655f 6964 2929 0a0a 2020 2020  (zone_id))..    
-0000efa0: 6465 6620 7265 6d6f 7665 5f70 7269 7661  def remove_priva
-0000efb0: 6379 5f7a 6f6e 6528 7365 6c66 2920 2d3e  cy_zone(self) ->
-0000efc0: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-0000efd0: 6e64 6578 2c20 5f20 3d20 7365 6c66 2e67  ndex, _ = self.g
-0000efe0: 6574 5f70 7269 7661 6379 5f7a 6f6e 6528  et_privacy_zone(
-0000eff0: 290a 0a20 2020 2020 2020 2069 6620 696e  )..        if in
-0000f000: 6465 7820 6973 206e 6f74 204e 6f6e 653a  dex is not None:
-0000f010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f020: 662e 7072 6976 6163 795f 7a6f 6e65 732e  f.privacy_zones.
-0000f030: 706f 7028 696e 6465 7829 0a0a 2020 2020  pop(index)..    
-0000f040: 6173 796e 6320 6465 6620 6765 745f 736e  async def get_sn
-0000f050: 6170 7368 6f74 280a 2020 2020 2020 2020  apshot(.        
-0000f060: 7365 6c66 2c0a 2020 2020 2020 2020 7769  self,.        wi
-0000f070: 6474 683a 204f 7074 696f 6e61 6c5b 696e  dth: Optional[in
-0000f080: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-0000f090: 2020 2068 6569 6768 743a 204f 7074 696f     height: Optio
-0000f0a0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0000f0b0: 0a20 2020 2020 2020 2064 743a 204f 7074  .        dt: Opt
-0000f0c0: 696f 6e61 6c5b 6461 7465 7469 6d65 5d20  ional[datetime] 
-0000f0d0: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
-0000f0e0: 204f 7074 696f 6e61 6c5b 6279 7465 735d   Optional[bytes]
-0000f0f0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0000f100: 7320 736e 6170 7368 6f74 2066 6f72 2063  s snapshot for c
-0000f110: 616d 6572 612e 0a0a 2020 2020 2020 2020  amera...        
-0000f120: 4461 7465 7469 6d65 206f 6620 7363 7265  Datetime of scre
-0000f130: 656e 7368 6f74 2069 7320 6170 7072 6f78  enshot is approx
-0000f140: 696d 6174 652e 2049 7420 6d61 7920 6265  imate. It may be
-0000f150: 202b 2f2d 2061 2066 6577 2073 6563 6f6e   +/- a few secon
-0000f160: 6473 2e0a 2020 2020 2020 2020 2222 220a  ds..        """.
-0000f170: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f180: 7365 6c66 2e61 7069 2e62 6f6f 7473 7472  self.api.bootstr
-0000f190: 6170 2e61 7574 685f 7573 6572 2e63 616e  ap.auth_user.can
-0000f1a0: 280a 2020 2020 2020 2020 2020 2020 4d6f  (.            Mo
-0000f1b0: 6465 6c54 7970 652e 4341 4d45 5241 2c0a  delType.CAMERA,.
-0000f1c0: 2020 2020 2020 2020 2020 2020 5065 726d              Perm
-0000f1d0: 6973 7369 6f6e 4e6f 6465 2e52 4541 445f  issionNode.READ_
-0000f1e0: 4d45 4449 412c 0a20 2020 2020 2020 2020  MEDIA,.         
-0000f1f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000f200: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000f210: 7261 6973 6520 4e6f 7441 7574 686f 7269  raise NotAuthori
-0000f220: 7a65 6428 0a20 2020 2020 2020 2020 2020  zed(.           
-0000f230: 2020 2020 2066 2244 6f20 6e6f 7420 6861       f"Do not ha
-0000f240: 7665 2070 6572 6d69 7373 696f 6e20 746f  ve permission to
-0000f250: 2072 6561 6420 6d65 6469 6120 666f 7220   read media for 
-0000f260: 6361 6d65 7261 3a20 7b73 656c 662e 6964  camera: {self.id
-0000f270: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-0000f280: 290a 0a20 2020 2020 2020 2069 6620 6865  )..        if he
-0000f290: 6967 6874 2069 7320 4e6f 6e65 2061 6e64  ight is None and
-0000f2a0: 2077 6964 7468 2069 7320 4e6f 6e65 2061   width is None a
-0000f2b0: 6e64 2073 656c 662e 6869 6768 5f63 616d  nd self.high_cam
-0000f2c0: 6572 615f 6368 616e 6e65 6c20 6973 206e  era_channel is n
-0000f2d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000f2e0: 2020 2020 2068 6569 6768 7420 3d20 7365       height = se
-0000f2f0: 6c66 2e68 6967 685f 6361 6d65 7261 5f63  lf.high_camera_c
-0000f300: 6861 6e6e 656c 2e68 6569 6768 740a 0a20  hannel.height.. 
-0000f310: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-0000f320: 6169 7420 7365 6c66 2e61 7069 2e67 6574  ait self.api.get
-0000f330: 5f63 616d 6572 615f 736e 6170 7368 6f74  _camera_snapshot
-0000f340: 2873 656c 662e 6964 2c20 7769 6474 682c  (self.id, width,
-0000f350: 2068 6569 6768 742c 2064 743d 6474 290a   height, dt=dt).
-0000f360: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
-0000f370: 6574 5f70 6163 6b61 6765 5f73 6e61 7073  et_package_snaps
-0000f380: 686f 7428 0a20 2020 2020 2020 2073 656c  hot(.        sel
-0000f390: 662c 0a20 2020 2020 2020 2077 6964 7468  f,.        width
-0000f3a0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000f3b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000f3c0: 6865 6967 6874 3a20 4f70 7469 6f6e 616c  height: Optional
-0000f3d0: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-0000f3e0: 2020 2020 2020 6474 3a20 4f70 7469 6f6e        dt: Option
-0000f3f0: 616c 5b64 6174 6574 696d 655d 203d 204e  al[datetime] = N
-0000f400: 6f6e 652c 0a20 2020 2029 202d 3e20 4f70  one,.    ) -> Op
-0000f410: 7469 6f6e 616c 5b62 7974 6573 5d3a 0a20  tional[bytes]:. 
-0000f420: 2020 2020 2020 2022 2222 4765 7473 2073         """Gets s
-0000f430: 6e61 7073 686f 7420 6672 6f6d 2074 6865  napshot from the
-0000f440: 2070 6163 6b61 6765 2063 616d 6572 612e   package camera.
-0000f450: 0a0a 2020 2020 2020 2020 4461 7465 7469  ..        Dateti
-0000f460: 6d65 206f 6620 7363 7265 656e 7368 6f74  me of screenshot
-0000f470: 2069 7320 6170 7072 6f78 696d 6174 652e   is approximate.
-0000f480: 2049 7420 6d61 7920 6265 202b 2f2d 2061   It may be +/- a
-0000f490: 2066 6577 2073 6563 6f6e 6473 2e0a 2020   few seconds..  
-0000f4a0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000f4b0: 2020 2069 6620 6e6f 7420 7365 6c66 2e66     if not self.f
-0000f4c0: 6561 7475 7265 5f66 6c61 6773 2e68 6173  eature_flags.has
-0000f4d0: 5f70 6163 6b61 6765 5f63 616d 6572 613a  _package_camera:
-0000f4e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000f4f0: 7365 2042 6164 5265 7175 6573 7428 2244  se BadRequest("D
-0000f500: 6576 6963 6520 646f 6573 206e 6f74 2068  evice does not h
-0000f510: 6176 6520 7061 636b 6167 6520 6361 6d65  ave package came
-0000f520: 7261 2229 0a0a 2020 2020 2020 2020 6966  ra")..        if
-0000f530: 206e 6f74 2073 656c 662e 6170 692e 626f   not self.api.bo
-0000f540: 6f74 7374 7261 702e 6175 7468 5f75 7365  otstrap.auth_use
-0000f550: 722e 6361 6e28 0a20 2020 2020 2020 2020  r.can(.         
-0000f560: 2020 204d 6f64 656c 5479 7065 2e43 414d     ModelType.CAM
-0000f570: 4552 412c 0a20 2020 2020 2020 2020 2020  ERA,.           
-0000f580: 2050 6572 6d69 7373 696f 6e4e 6f64 652e   PermissionNode.
-0000f590: 5245 4144 5f4d 4544 4941 2c0a 2020 2020  READ_MEDIA,.    
-0000f5a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000f5b0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-0000f5c0: 2020 2020 2072 6169 7365 204e 6f74 4175       raise NotAu
-0000f5d0: 7468 6f72 697a 6564 280a 2020 2020 2020  thorized(.      
-0000f5e0: 2020 2020 2020 2020 2020 6622 446f 206e            f"Do n
-0000f5f0: 6f74 2068 6176 6520 7065 726d 6973 7369  ot have permissi
-0000f600: 6f6e 2074 6f20 7265 6164 206d 6564 6961  on to read media
-0000f610: 2066 6f72 2063 616d 6572 613a 207b 7365   for camera: {se
-0000f620: 6c66 2e69 647d 222c 0a20 2020 2020 2020  lf.id}",.       
-0000f630: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000f640: 6966 2068 6569 6768 7420 6973 204e 6f6e  if height is Non
-0000f650: 6520 616e 6420 7769 6474 6820 6973 204e  e and width is N
-0000f660: 6f6e 6520 616e 6420 7365 6c66 2e70 6163  one and self.pac
-0000f670: 6b61 6765 5f63 616d 6572 615f 6368 616e  kage_camera_chan
-0000f680: 6e65 6c20 6973 206e 6f74 204e 6f6e 653a  nel is not None:
-0000f690: 0a20 2020 2020 2020 2020 2020 2068 6569  .            hei
-0000f6a0: 6768 7420 3d20 7365 6c66 2e70 6163 6b61  ght = self.packa
-0000f6b0: 6765 5f63 616d 6572 615f 6368 616e 6e65  ge_camera_channe
-0000f6c0: 6c2e 6865 6967 6874 0a0a 2020 2020 2020  l.height..      
-0000f6d0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-0000f6e0: 656c 662e 6170 692e 6765 745f 7061 636b  elf.api.get_pack
-0000f6f0: 6167 655f 6361 6d65 7261 5f73 6e61 7073  age_camera_snaps
-0000f700: 686f 7428 7365 6c66 2e69 642c 2077 6964  hot(self.id, wid
-0000f710: 7468 2c20 6865 6967 6874 2c20 6474 3d64  th, height, dt=d
-0000f720: 7429 0a0a 2020 2020 6173 796e 6320 6465  t)..    async de
-0000f730: 6620 6765 745f 7669 6465 6f28 0a20 2020  f get_video(.   
-0000f740: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000f750: 2020 2073 7461 7274 3a20 6461 7465 7469     start: dateti
-0000f760: 6d65 2c0a 2020 2020 2020 2020 656e 643a  me,.        end:
-0000f770: 2064 6174 6574 696d 652c 0a20 2020 2020   datetime,.     
-0000f780: 2020 2063 6861 6e6e 656c 5f69 6e64 6578     channel_index
-0000f790: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
-0000f7a0: 2020 206f 7574 7075 745f 6669 6c65 3a20     output_file: 
-0000f7b0: 4f70 7469 6f6e 616c 5b50 6174 685d 203d  Optional[Path] =
-0000f7c0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-0000f7d0: 7465 7261 746f 725f 6361 6c6c 6261 636b  terator_callback
-0000f7e0: 3a20 4f70 7469 6f6e 616c 5b49 7465 7261  : Optional[Itera
-0000f7f0: 746f 7243 616c 6c62 6163 6b5d 203d 204e  torCallback] = N
-0000f800: 6f6e 652c 0a20 2020 2020 2020 2070 726f  one,.        pro
-0000f810: 6772 6573 735f 6361 6c6c 6261 636b 3a20  gress_callback: 
-0000f820: 4f70 7469 6f6e 616c 5b50 726f 6772 6573  Optional[Progres
-0000f830: 7343 616c 6c62 6163 6b5d 203d 204e 6f6e  sCallback] = Non
-0000f840: 652c 0a20 2020 2020 2020 2063 6875 6e6b  e,.        chunk
-0000f850: 5f73 697a 653a 2069 6e74 203d 2036 3535  _size: int = 655
-0000f860: 3336 2c0a 2020 2020 2020 2020 6670 733a  36,.        fps:
-0000f870: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000f880: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-0000f890: 4f70 7469 6f6e 616c 5b62 7974 6573 5d3a  Optional[bytes]:
-0000f8a0: 0a20 2020 2020 2020 2022 2222 4578 706f  .        """Expo
-0000f8b0: 7274 7320 4d50 3420 7669 6465 6f20 6672  rts MP4 video fr
-0000f8c0: 6f6d 2061 2067 6976 656e 2063 616d 6572  om a given camer
-0000f8d0: 6120 6174 2061 2073 7065 6369 6669 6320  a at a specific 
-0000f8e0: 7469 6d65 2e0a 0a20 2020 2020 2020 2053  time...        S
-0000f8f0: 7461 7274 2f45 6e64 206f 6620 7669 6465  tart/End of vide
-0000f900: 6f20 6578 706f 7274 2061 7265 2061 7070  o export are app
-0000f910: 726f 7869 6d61 7465 2e20 4974 206d 6179  roximate. It may
-0000f920: 2062 6520 2b2f 2d20 6120 6665 7720 7365   be +/- a few se
-0000f930: 636f 6e64 732e 0a0a 2020 2020 2020 2020  conds...        
-0000f940: 4974 2069 7320 7265 636f 6d6d 656e 6465  It is recommende
-0000f950: 6420 746f 2070 726f 7669 6465 2061 206f  d to provide a o
-0000f960: 7574 7075 7420 6669 6c65 206f 7220 7072  utput file or pr
-0000f970: 6f67 7265 7373 2063 616c 6c62 6163 6b20  ogress callback 
-0000f980: 666f 7220 6c61 7267 6572 0a20 2020 2020  for larger.     
-0000f990: 2020 2076 6964 656f 2063 6c69 7073 2c20     video clips, 
-0000f9a0: 6f74 6865 7277 6973 6520 7468 6520 6675  otherwise the fu
-0000f9b0: 6c6c 2076 6964 656f 206d 7573 7420 6265  ll video must be
-0000f9c0: 2064 6f77 6e6c 6f61 6465 6420 746f 206d   downloaded to m
-0000f9d0: 656d 6f72 7920 6265 666f 7265 0a20 2020  emory before.   
-0000f9e0: 2020 2020 2062 6569 6e67 2077 7269 7474       being writt
-0000f9f0: 656e 2e0a 0a20 2020 2020 2020 2050 726f  en...        Pro
-0000fa00: 7669 6469 6e67 2074 6865 2060 6670 7360  viding the `fps`
-0000fa10: 2070 6172 616d 6574 6572 2063 7265 6174   parameter creat
-0000fa20: 6573 2061 2022 7469 6d65 6c61 7073 6522  es a "timelapse"
-0000fa30: 2065 7870 6f72 7420 7774 6968 2074 6865   export wtih the
-0000fa40: 2067 6976 656e 2046 5053 0a20 2020 2020   given FPS.     
-0000fa50: 2020 2076 616c 7565 2e20 5072 6f74 6563     value. Protec
-0000fa60: 7420 6170 7020 6769 7665 7320 7468 6520  t app gives the 
-0000fa70: 6f70 7469 6f6e 7320 666f 7220 3630 7820  options for 60x 
-0000fa80: 2866 7073 3d34 292c 2031 3230 7820 2866  (fps=4), 120x (f
-0000fa90: 7073 3d38 292c 2033 3030 780a 2020 2020  ps=8), 300x.    
-0000faa0: 2020 2020 2866 7073 3d32 3029 2c20 616e      (fps=20), an
-0000fab0: 6420 3630 3078 2028 6670 733d 3430 292e  d 600x (fps=40).
-0000fac0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0000fad0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000fae0: 662e 6170 692e 626f 6f74 7374 7261 702e  f.api.bootstrap.
-0000faf0: 6175 7468 5f75 7365 722e 6361 6e28 0a20  auth_user.can(. 
-0000fb00: 2020 2020 2020 2020 2020 204d 6f64 656c             Model
-0000fb10: 5479 7065 2e43 414d 4552 412c 0a20 2020  Type.CAMERA,.   
-0000fb20: 2020 2020 2020 2020 2050 6572 6d69 7373           Permiss
-0000fb30: 696f 6e4e 6f64 652e 5245 4144 5f4d 4544  ionNode.READ_MED
-0000fb40: 4941 2c0a 2020 2020 2020 2020 2020 2020  IA,.            
-0000fb50: 7365 6c66 2c0a 2020 2020 2020 2020 293a  self,.        ):
-0000fb60: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000fb70: 7365 204e 6f74 4175 7468 6f72 697a 6564  se NotAuthorized
-0000fb80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000fb90: 2020 6622 446f 206e 6f74 2068 6176 6520    f"Do not have 
-0000fba0: 7065 726d 6973 7369 6f6e 2074 6f20 7265  permission to re
-0000fbb0: 6164 206d 6564 6961 2066 6f72 2063 616d  ad media for cam
-0000fbc0: 6572 613a 207b 7365 6c66 2e69 647d 222c  era: {self.id}",
-0000fbd0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000fbe0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0000fbf0: 7761 6974 2073 656c 662e 6170 692e 6765  wait self.api.ge
-0000fc00: 745f 6361 6d65 7261 5f76 6964 656f 280a  t_camera_video(.
-0000fc10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fc20: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
-0000fc30: 2073 7461 7274 2c0a 2020 2020 2020 2020   start,.        
-0000fc40: 2020 2020 656e 642c 0a20 2020 2020 2020      end,.       
-0000fc50: 2020 2020 2063 6861 6e6e 656c 5f69 6e64       channel_ind
-0000fc60: 6578 2c0a 2020 2020 2020 2020 2020 2020  ex,.            
-0000fc70: 6f75 7470 7574 5f66 696c 653d 6f75 7470  output_file=outp
-0000fc80: 7574 5f66 696c 652c 0a20 2020 2020 2020  ut_file,.       
-0000fc90: 2020 2020 2069 7465 7261 746f 725f 6361       iterator_ca
-0000fca0: 6c6c 6261 636b 3d69 7465 7261 746f 725f  llback=iterator_
-0000fcb0: 6361 6c6c 6261 636b 2c0a 2020 2020 2020  callback,.      
-0000fcc0: 2020 2020 2020 7072 6f67 7265 7373 5f63        progress_c
-0000fcd0: 616c 6c62 6163 6b3d 7072 6f67 7265 7373  allback=progress
-0000fce0: 5f63 616c 6c62 6163 6b2c 0a20 2020 2020  _callback,.     
-0000fcf0: 2020 2020 2020 2063 6875 6e6b 5f73 697a         chunk_siz
-0000fd00: 653d 6368 756e 6b5f 7369 7a65 2c0a 2020  e=chunk_size,.  
-0000fd10: 2020 2020 2020 2020 2020 6670 733d 6670            fps=fp
-0000fd20: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
-0000fd30: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
-0000fd40: 7265 636f 7264 696e 675f 6d6f 6465 2873  recording_mode(s
-0000fd50: 656c 662c 206d 6f64 653a 2052 6563 6f72  elf, mode: Recor
-0000fd60: 6469 6e67 4d6f 6465 2920 2d3e 204e 6f6e  dingMode) -> Non
-0000fd70: 653a 0a20 2020 2020 2020 2022 2222 5365  e:.        """Se
-0000fd80: 7473 2072 6563 6f72 6469 6e67 206d 6f64  ts recording mod
-0000fd90: 6520 6f6e 2063 616d 6572 6122 2222 0a0a  e on camera"""..
-0000fda0: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
-0000fdb0: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
-0000fdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fdd0: 2e72 6563 6f72 6469 6e67 5f73 6574 7469  .recording_setti
-0000fde0: 6e67 732e 6d6f 6465 203d 206d 6f64 650a  ngs.mode = mode.
-0000fdf0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-0000fe00: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
-0000fe10: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
-0000fe20: 6173 796e 6320 6465 6620 7365 745f 6972  async def set_ir
-0000fe30: 5f6c 6564 5f6d 6f64 656c 2873 656c 662c  _led_model(self,
-0000fe40: 206d 6f64 653a 2049 524c 4544 4d6f 6465   mode: IRLEDMode
-0000fe50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000fe60: 2020 2022 2222 5365 7473 2049 5220 4c45     """Sets IR LE
-0000fe70: 4420 6d6f 6465 206f 6e20 6361 6d65 7261  D mode on camera
-0000fe80: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-0000fe90: 6e6f 7420 7365 6c66 2e66 6561 7475 7265  not self.feature
-0000fea0: 5f66 6c61 6773 2e68 6173 5f6c 6564 5f69  _flags.has_led_i
-0000feb0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-0000fec0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
-0000fed0: 2243 616d 6572 6120 646f 6573 206e 6f74  "Camera does not
-0000fee0: 2068 6176 6520 616e 204c 4544 2049 5222   have an LED IR"
-0000fef0: 290a 0a20 2020 2020 2020 2064 6566 2063  )..        def c
-0000ff00: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
-0000ff10: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000ff20: 656c 662e 6973 705f 7365 7474 696e 6773  elf.isp_settings
-0000ff30: 2e69 725f 6c65 645f 6d6f 6465 203d 206d  .ir_led_mode = m
-0000ff40: 6f64 650a 0a20 2020 2020 2020 2061 7761  ode..        awa
-0000ff50: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-0000ff60: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-0000ff70: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-0000ff80: 745f 6963 725f 6375 7374 6f6d 5f6c 7578  t_icr_custom_lux
-0000ff90: 2873 656c 662c 2076 616c 7565 3a20 4943  (self, value: IC
-0000ffa0: 524c 7578 5661 6c75 6529 202d 3e20 4e6f  RLuxValue) -> No
-0000ffb0: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
-0000ffc0: 6574 2049 4352 4375 7374 6f6d 5661 6c75  et ICRCustomValu
-0000ffd0: 6520 6672 6f6d 206c 7578 2076 616c 7565  e from lux value
-0000ffe0: 2e22 2222 0a0a 2020 2020 2020 2020 6966  ."""..        if
-0000fff0: 206e 6f74 2073 656c 662e 6665 6174 7572   not self.featur
-00010000: 655f 666c 6167 732e 6861 735f 6c65 645f  e_flags.has_led_
-00010010: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-00010020: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
-00010030: 2822 4361 6d65 7261 2064 6f65 7320 6e6f  ("Camera does no
-00010040: 7420 6861 7665 2061 6e20 4c45 4420 4952  t have an LED IR
-00010050: 2229 0a0a 2020 2020 2020 2020 6963 725f  ")..        icr_
-00010060: 7661 6c75 6520 3d20 300a 2020 2020 2020  value = 0.      
-00010070: 2020 666f 7220 696e 6465 782c 2074 6872    for index, thr
-00010080: 6573 686f 6c64 2069 6e20 656e 756d 6572  eshold in enumer
-00010090: 6174 6528 4c55 585f 4d41 5050 494e 475f  ate(LUX_MAPPING_
-000100a0: 5641 4c55 4553 293a 0a20 2020 2020 2020  VALUES):.       
-000100b0: 2020 2020 2069 6620 7661 6c75 6520 3e3d       if value >=
-000100c0: 2074 6872 6573 686f 6c64 3a0a 2020 2020   threshold:.    
-000100d0: 2020 2020 2020 2020 2020 2020 6963 725f              icr_
-000100e0: 7661 6c75 6520 3d20 3130 202d 2069 6e64  value = 10 - ind
-000100f0: 6578 0a20 2020 2020 2020 2020 2020 2020  ex.             
-00010100: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00010110: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
-00010120: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00010130: 2020 2020 2020 7365 6c66 2e69 7370 5f73        self.isp_s
-00010140: 6574 7469 6e67 732e 6963 725f 6375 7374  ettings.icr_cust
-00010150: 6f6d 5f76 616c 7565 203d 2063 6173 7428  om_value = cast(
-00010160: 4943 5243 7573 746f 6d56 616c 7565 2c20  ICRCustomValue, 
-00010170: 6963 725f 7661 6c75 6529 0a0a 2020 2020  icr_value)..    
-00010180: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00010190: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-000101a0: 6261 636b 290a 0a20 2020 2040 7072 6f70  back)..    @prop
-000101b0: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
-000101c0: 6972 5f6c 6564 5f73 6c69 6465 725f 656e  ir_led_slider_en
-000101d0: 6162 6c65 6428 7365 6c66 2920 2d3e 2062  abled(self) -> b
-000101e0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-000101f0: 5265 7475 726e 2069 6620 4952 204c 4544  Return if IR LED
-00010200: 2063 7573 746f 6d20 736c 6964 6572 2069   custom slider i
-00010210: 7320 656e 6162 6c65 642e 2222 220a 0a20  s enabled.""".. 
-00010220: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
-00010230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010240: 2e66 6561 7475 7265 5f66 6c61 6773 2e68  .feature_flags.h
-00010250: 6173 5f6c 6564 5f69 720a 2020 2020 2020  as_led_ir.      
-00010260: 2020 2020 2020 616e 6420 7365 6c66 2e69        and self.i
-00010270: 7370 5f73 6574 7469 6e67 732e 6972 5f6c  sp_settings.ir_l
-00010280: 6564 5f6d 6f64 6520 3d3d 2049 524c 4544  ed_mode == IRLED
-00010290: 4d6f 6465 2e43 5553 544f 4d0a 2020 2020  Mode.CUSTOM.    
-000102a0: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-000102b0: 2064 6566 2073 6574 5f73 7461 7475 735f   def set_status_
-000102c0: 6c69 6768 7428 7365 6c66 2c20 656e 6162  light(self, enab
-000102d0: 6c65 643a 2062 6f6f 6c29 202d 3e20 4e6f  led: bool) -> No
-000102e0: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
-000102f0: 6574 7320 7374 6174 7573 2069 6e64 6963  ets status indic
-00010300: 6963 6174 6f72 206c 6967 6874 206f 6e20  icator light on 
-00010310: 6361 6d65 7261 2222 220a 0a20 2020 2020  camera"""..     
-00010320: 2020 2069 6620 6e6f 7420 7365 6c66 2e66     if not self.f
-00010330: 6561 7475 7265 5f66 6c61 6773 2e68 6173  eature_flags.has
-00010340: 5f6c 6564 5f73 7461 7475 733a 0a20 2020  _led_status:.   
-00010350: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
-00010360: 6164 5265 7175 6573 7428 2243 616d 6572  adRequest("Camer
-00010370: 6120 646f 6573 206e 6f74 2068 6176 6520  a does not have 
-00010380: 7374 6174 7573 206c 6967 6874 2229 0a0a  status light")..
-00010390: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
-000103a0: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
-000103b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000103c0: 2e6c 6564 5f73 6574 7469 6e67 732e 6973  .led_settings.is
-000103d0: 5f65 6e61 626c 6564 203d 2065 6e61 626c  _enabled = enabl
-000103e0: 6564 0a20 2020 2020 2020 2020 2020 2073  ed.            s
-000103f0: 656c 662e 6c65 645f 7365 7474 696e 6773  elf.led_settings
-00010400: 2e62 6c69 6e6b 5f72 6174 6520 3d20 300a  .blink_rate = 0.
-00010410: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-00010420: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
-00010430: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
-00010440: 6173 796e 6320 6465 6620 7365 745f 6864  async def set_hd
-00010450: 7228 7365 6c66 2c20 656e 6162 6c65 643a  r(self, enabled:
-00010460: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
-00010470: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
-00010480: 4844 5220 2848 6967 6820 4479 6e61 6d69  HDR (High Dynami
-00010490: 6320 5261 6e67 6529 206f 6e20 6361 6d65  c Range) on came
-000104a0: 7261 2222 220a 0a20 2020 2020 2020 2077  ra"""..        w
-000104b0: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
-000104c0: 2020 2020 2020 2020 2020 2273 6574 5f68            "set_h
-000104d0: 6472 2069 7320 6465 7072 6563 6174 6564  dr is deprecated
-000104e0: 2061 6e64 2072 6570 6c61 6365 6420 7769   and replaced wi
-000104f0: 7468 2073 6574 5f68 6472 5f6d 6f64 6520  th set_hdr_mode 
-00010500: 666f 7220 7665 7273 696f 6e73 206f 6620  for versions of 
-00010510: 556e 6946 6920 5072 6f74 6563 7420 7633  UniFi Protect v3
-00010520: 2e30 2b22 2c0a 2020 2020 2020 2020 2020  .0+",.          
-00010530: 2020 4465 7072 6563 6174 696f 6e57 6172    DeprecationWar
-00010540: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
-00010550: 2020 7374 6163 6b6c 6576 656c 3d32 2c0a    stacklevel=2,.
-00010560: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00010570: 2020 2069 6620 6e6f 7420 7365 6c66 2e66     if not self.f
-00010580: 6561 7475 7265 5f66 6c61 6773 2e68 6173  eature_flags.has
-00010590: 5f68 6472 3a0a 2020 2020 2020 2020 2020  _hdr:.          
-000105a0: 2020 7261 6973 6520 4261 6452 6571 7565    raise BadReque
-000105b0: 7374 2822 4361 6d65 7261 2064 6f65 7320  st("Camera does 
-000105c0: 6e6f 7420 6861 7665 2048 4452 2229 0a0a  not have HDR")..
-000105d0: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
-000105e0: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
-000105f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010600: 2e68 6472 5f6d 6f64 6520 3d20 656e 6162  .hdr_mode = enab
-00010610: 6c65 640a 0a20 2020 2020 2020 2061 7761  led..        awa
-00010620: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-00010630: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-00010640: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-00010650: 745f 6864 725f 6d6f 6465 2873 656c 662c  t_hdr_mode(self,
-00010660: 206d 6f64 653a 204c 6974 6572 616c 5b22   mode: Literal["
-00010670: 6175 746f 222c 2022 6f66 6622 2c20 2261  auto", "off", "a
-00010680: 6c77 6179 7322 5d29 202d 3e20 4e6f 6e65  lways"]) -> None
-00010690: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-000106a0: 7320 4844 5220 6d6f 6465 2073 696d 696c  s HDR mode simil
-000106b0: 6172 2074 6f20 686f 7720 5072 6f74 6563  ar to how Protec
-000106c0: 7420 696e 7465 7266 6163 6520 776f 726b  t interface work
-000106d0: 732e 2222 220a 0a20 2020 2020 2020 2069  s."""..        i
-000106e0: 6620 6e6f 7420 7365 6c66 2e66 6561 7475  f not self.featu
-000106f0: 7265 5f66 6c61 6773 2e68 6173 5f68 6472  re_flags.has_hdr
-00010700: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00010710: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00010720: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
-00010730: 6861 7665 2048 4452 2229 0a0a 2020 2020  have HDR")..    
-00010740: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
-00010750: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00010760: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-00010770: 3d3d 2022 6f66 6622 3a0a 2020 2020 2020  == "off":.      
-00010780: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00010790: 6472 5f6d 6f64 6520 3d20 4661 6c73 650a  dr_mode = False.
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 6966 2073 656c 662e 6973 705f 7365 7474  if self.isp_sett
-000107c0: 696e 6773 2e68 6472 5f6d 6f64 6520 6973  ings.hdr_mode is
-000107d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000107f0: 656c 662e 6973 705f 7365 7474 696e 6773  elf.isp_settings
-00010800: 2e68 6472 5f6d 6f64 6520 3d20 4844 524d  .hdr_mode = HDRM
-00010810: 6f64 652e 4e4f 524d 414c 0a20 2020 2020  ode.NORMAL.     
-00010820: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00010830: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010840: 662e 6864 725f 6d6f 6465 203d 2054 7275  f.hdr_mode = Tru
-00010850: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00010860: 2020 6966 2073 656c 662e 6973 705f 7365    if self.isp_se
-00010870: 7474 696e 6773 2e68 6472 5f6d 6f64 6520  ttings.hdr_mode 
-00010880: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2073 656c 662e 6973 705f 7365 7474 696e   self.isp_settin
-000108b0: 6773 2e68 6472 5f6d 6f64 6520 3d20 280a  gs.hdr_mode = (.
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 2020 4844 524d 6f64 652e          HDRMode.
-000108e0: 4e4f 524d 414c 2069 6620 6d6f 6465 203d  NORMAL if mode =
-000108f0: 3d20 2261 7574 6f22 2065 6c73 6520 4844  = "auto" else HD
-00010900: 524d 6f64 652e 414c 5741 5953 5f4f 4e0a  RMode.ALWAYS_ON.
-00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
-00010930: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
-00010940: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
-00010950: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00010960: 7365 745f 636f 6c6f 725f 6e69 6768 745f  set_color_night_
-00010970: 7669 7369 6f6e 2873 656c 662c 2065 6e61  vision(self, ena
-00010980: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
-00010990: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000109a0: 5365 7473 2043 6f6c 6f72 204e 6967 6874  Sets Color Night
-000109b0: 2056 6973 696f 6e20 6f6e 2063 616d 6572   Vision on camer
-000109c0: 6122 2222 0a0a 2020 2020 2020 2020 6966  a"""..        if
-000109d0: 206e 6f74 2073 656c 662e 6861 735f 636f   not self.has_co
-000109e0: 6c6f 725f 6e69 6768 745f 7669 7369 6f6e  lor_night_vision
-000109f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00010a00: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00010a10: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
-00010a20: 6861 7665 2043 6f6c 6f72 204e 6967 6874  have Color Night
-00010a30: 2056 6973 696f 6e22 290a 0a20 2020 2020   Vision")..     
-00010a40: 2020 2064 6566 2063 616c 6c62 6163 6b28     def callback(
-00010a50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00010a60: 2020 2020 2020 2073 656c 662e 6973 705f         self.isp_
-00010a70: 7365 7474 696e 6773 2e69 735f 636f 6c6f  settings.is_colo
-00010a80: 725f 6e69 6768 745f 7669 7369 6f6e 5f65  r_night_vision_e
-00010a90: 6e61 626c 6564 203d 2065 6e61 626c 6564  nabled = enabled
-00010aa0: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00010ab0: 7365 6c66 2e71 7565 7565 5f75 7064 6174  self.queue_updat
-00010ac0: 6528 6361 6c6c 6261 636b 290a 0a20 2020  e(callback)..   
-00010ad0: 2061 7379 6e63 2064 6566 2073 6574 5f76   async def set_v
-00010ae0: 6964 656f 5f6d 6f64 6528 7365 6c66 2c20  ideo_mode(self, 
-00010af0: 6d6f 6465 3a20 5669 6465 6f4d 6f64 6529  mode: VideoMode)
-00010b00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00010b10: 2020 2222 2253 6574 7320 7669 6465 6f20    """Sets video 
-00010b20: 6d6f 6465 206f 6e20 6361 6d65 7261 2222  mode on camera""
-00010b30: 220a 0a20 2020 2020 2020 2069 6620 6d6f  "..        if mo
-00010b40: 6465 206e 6f74 2069 6e20 7365 6c66 2e66  de not in self.f
-00010b50: 6561 7475 7265 5f66 6c61 6773 2e76 6964  eature_flags.vid
-00010b60: 656f 5f6d 6f64 6573 3a0a 2020 2020 2020  eo_modes:.      
-00010b70: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
-00010b80: 6571 7565 7374 2866 2243 616d 6572 6120  equest(f"Camera 
-00010b90: 646f 6573 206e 6f74 2068 6176 6520 7b6d  does not have {m
-00010ba0: 6f64 657d 2229 0a0a 2020 2020 2020 2020  ode}")..        
-00010bb0: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
-00010bc0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00010bd0: 2020 2020 7365 6c66 2e76 6964 656f 5f6d      self.video_m
-00010be0: 6f64 6520 3d20 6d6f 6465 0a0a 2020 2020  ode = mode..    
-00010bf0: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00010c00: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00010c10: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-00010c20: 2064 6566 2073 6574 5f63 616d 6572 615f   def set_camera_
-00010c30: 7a6f 6f6d 2873 656c 662c 206c 6576 656c  zoom(self, level
-00010c40: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00010c50: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
-00010c60: 7a6f 6f6d 206c 6576 656c 2066 6f72 2063  zoom level for c
-00010c70: 616d 6572 6122 2222 0a0a 2020 2020 2020  amera"""..      
-00010c80: 2020 6966 206e 6f74 2073 656c 662e 6665    if not self.fe
-00010c90: 6174 7572 655f 666c 6167 732e 6361 6e5f  ature_flags.can_
-00010ca0: 6f70 7469 6361 6c5f 7a6f 6f6d 3a0a 2020  optical_zoom:.  
-00010cb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00010cc0: 4261 6452 6571 7565 7374 2822 4361 6d65  BadRequest("Came
-00010cd0: 7261 2063 616e 6e6f 7420 6f70 7469 6361  ra cannot optica
-00010ce0: 6c20 7a6f 6f6d 2229 0a0a 2020 2020 2020  l zoom")..      
-00010cf0: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
-00010d00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00010d10: 2020 2020 2020 7365 6c66 2e69 7370 5f73        self.isp_s
-00010d20: 6574 7469 6e67 732e 7a6f 6f6d 5f70 6f73  ettings.zoom_pos
-00010d30: 6974 696f 6e20 3d20 5065 7263 656e 7449  ition = PercentI
-00010d40: 6e74 286c 6576 656c 290a 0a20 2020 2020  nt(level)..     
-00010d50: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
-00010d60: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
-00010d70: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
-00010d80: 6465 6620 7365 745f 7764 725f 6c65 7665  def set_wdr_leve
-00010d90: 6c28 7365 6c66 2c20 6c65 7665 6c3a 2069  l(self, level: i
-00010da0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00010db0: 2020 2020 2022 2222 5365 7473 2057 4452       """Sets WDR
-00010dc0: 2028 5769 6465 2044 796e 616d 6963 2052   (Wide Dynamic R
-00010dd0: 616e 6765 2920 6f6e 2063 616d 6572 6122  ange) on camera"
-00010de0: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-00010df0: 656c 662e 6665 6174 7572 655f 666c 6167  elf.feature_flag
-00010e00: 732e 6861 735f 6864 723a 0a20 2020 2020  s.has_hdr:.     
-00010e10: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
-00010e20: 5265 7175 6573 7428 2243 616e 6e6f 7420  Request("Cannot 
-00010e30: 7365 7420 5744 5220 6f6e 2063 616d 6572  set WDR on camer
-00010e40: 6173 2077 6974 6820 4844 5222 290a 0a20  as with HDR").. 
-00010e50: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
-00010e60: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
-00010e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010e80: 6973 705f 7365 7474 696e 6773 2e77 6472  isp_settings.wdr
-00010e90: 203d 2057 4452 4c65 7665 6c28 6c65 7665   = WDRLevel(leve
-00010ea0: 6c29 0a0a 2020 2020 2020 2020 6177 6169  l)..        awai
-00010eb0: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
-00010ec0: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
-00010ed0: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-00010ee0: 5f6d 6963 5f76 6f6c 756d 6528 7365 6c66  _mic_volume(self
-00010ef0: 2c20 6c65 7665 6c3a 2069 6e74 2920 2d3e  , level: int) ->
-00010f00: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00010f10: 2222 5365 7473 2074 6865 206d 6963 2073  ""Sets the mic s
-00010f20: 656e 7369 7469 7669 7479 206c 6576 656c  ensitivity level
-00010f30: 206f 6e20 6361 6d65 7261 2222 220a 0a20   on camera""".. 
-00010f40: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00010f50: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
-00010f60: 2e68 6173 5f6d 6963 3a0a 2020 2020 2020  .has_mic:.      
-00010f70: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
-00010f80: 6571 7565 7374 2822 4361 6d65 7261 2064  equest("Camera d
-00010f90: 6f65 7320 6e6f 7420 6861 7665 206d 6963  oes not have mic
-00010fa0: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
-00010fb0: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
-00010fc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00010fd0: 7365 6c66 2e6d 6963 5f76 6f6c 756d 6520  self.mic_volume 
-00010fe0: 3d20 5065 7263 656e 7449 6e74 286c 6576  = PercentInt(lev
-00010ff0: 656c 290a 0a20 2020 2020 2020 2061 7761  el)..        awa
-00011000: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-00011010: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-00011020: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-00011030: 745f 7370 6561 6b65 725f 766f 6c75 6d65  t_speaker_volume
-00011040: 2873 656c 662c 206c 6576 656c 3a20 696e  (self, level: in
-00011050: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00011060: 2020 2020 2222 2253 6574 7320 7468 6520      """Sets the 
-00011070: 7370 6561 6b65 7220 7365 6e73 6974 6976  speaker sensitiv
-00011080: 6974 7920 6c65 7665 6c20 6f6e 2063 616d  ity level on cam
-00011090: 6572 612e 2052 6571 7569 7265 7320 6361  era. Requires ca
-000110a0: 6d65 7261 2074 6f20 6861 7665 2073 7065  mera to have spe
-000110b0: 616b 6572 7322 2222 0a0a 2020 2020 2020  akers"""..      
-000110c0: 2020 6966 206e 6f74 2073 656c 662e 6665    if not self.fe
-000110d0: 6174 7572 655f 666c 6167 732e 6861 735f  ature_flags.has_
-000110e0: 7370 6561 6b65 723a 0a20 2020 2020 2020  speaker:.       
-000110f0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-00011100: 7175 6573 7428 2243 616d 6572 6120 646f  quest("Camera do
-00011110: 6573 206e 6f74 2068 6176 6520 7370 6561  es not have spea
-00011120: 6b65 7222 290a 0a20 2020 2020 2020 2064  ker")..        d
-00011130: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
-00011140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011150: 2020 2073 656c 662e 7370 6561 6b65 725f     self.speaker_
-00011160: 7365 7474 696e 6773 2e76 6f6c 756d 6520  settings.volume 
-00011170: 3d20 5065 7263 656e 7449 6e74 286c 6576  = PercentInt(lev
-00011180: 656c 290a 0a20 2020 2020 2020 2061 7761  el)..        awa
-00011190: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-000111a0: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-000111b0: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-000111c0: 745f 6368 696d 655f 7479 7065 2873 656c  t_chime_type(sel
-000111d0: 662c 2063 6869 6d65 5f74 7970 653a 2043  f, chime_type: C
-000111e0: 6869 6d65 5479 7065 2920 2d3e 204e 6f6e  himeType) -> Non
-000111f0: 653a 0a20 2020 2020 2020 2022 2222 5365  e:.        """Se
-00011200: 7473 2063 6869 6d65 2074 7970 6520 666f  ts chime type fo
-00011210: 7220 646f 6f72 6265 6c6c 2e20 5265 7175  r doorbell. Requ
-00011220: 6972 6573 2063 616d 6572 6120 746f 2062  ires camera to b
-00011230: 6520 6120 646f 6f72 6265 6c6c 2222 220a  e a doorbell""".
-00011240: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-00011250: 656c 662e 7365 745f 6368 696d 655f 6475  elf.set_chime_du
-00011260: 7261 7469 6f6e 2874 696d 6564 656c 7461  ration(timedelta
-00011270: 286d 696c 6c69 7365 636f 6e64 733d 6368  (milliseconds=ch
-00011280: 696d 655f 7479 7065 2e76 616c 7565 2929  ime_type.value))
-00011290: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000112a0: 7365 745f 6368 696d 655f 6475 7261 7469  set_chime_durati
-000112b0: 6f6e 2873 656c 662c 2064 7572 6174 696f  on(self, duratio
-000112c0: 6e3a 2074 696d 6564 656c 7461 207c 2066  n: timedelta | f
-000112d0: 6c6f 6174 2920 2d3e 204e 6f6e 653a 0a20  loat) -> None:. 
-000112e0: 2020 2020 2020 2022 2222 5365 7473 2063         """Sets c
-000112f0: 6869 6d65 2064 7572 6174 696f 6e20 666f  hime duration fo
-00011300: 7220 646f 6f72 6265 6c6c 2e20 5265 7175  r doorbell. Requ
-00011310: 6972 6573 2063 616d 6572 6120 746f 2062  ires camera to b
-00011320: 6520 6120 646f 6f72 6265 6c6c 2222 220a  e a doorbell""".
-00011330: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00011340: 7365 6c66 2e66 6561 7475 7265 5f66 6c61  self.feature_fla
-00011350: 6773 2e68 6173 5f63 6869 6d65 3a0a 2020  gs.has_chime:.  
-00011360: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00011370: 4261 6452 6571 7565 7374 2822 4361 6d65  BadRequest("Came
-00011380: 7261 2064 6f65 7320 6e6f 7420 6861 7665  ra does not have
-00011390: 2061 2063 6869 6d65 2229 0a0a 2020 2020   a chime")..    
-000113a0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000113b0: 6528 6475 7261 7469 6f6e 2c20 2866 6c6f  e(duration, (flo
-000113c0: 6174 2c20 696e 7429 293a 0a20 2020 2020  at, int)):.     
-000113d0: 2020 2020 2020 2069 6620 6475 7261 7469         if durati
-000113e0: 6f6e 203c 2030 3a0a 2020 2020 2020 2020  on < 0:.        
-000113f0: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
-00011400: 6452 6571 7565 7374 2822 4368 696d 6520  dRequest("Chime 
-00011410: 6475 7261 7469 6f6e 206d 7573 7420 6265  duration must be
-00011420: 2061 2070 6f73 6974 6976 6520 6e75 6d62   a positive numb
-00011430: 6572 206f 6620 7365 636f 6e64 7322 290a  er of seconds").
-00011440: 2020 2020 2020 2020 2020 2020 6475 7261              dura
-00011450: 7469 6f6e 5f74 6420 3d20 7469 6d65 6465  tion_td = timede
-00011460: 6c74 6128 7365 636f 6e64 733d 6475 7261  lta(seconds=dura
-00011470: 7469 6f6e 290a 2020 2020 2020 2020 656c  tion).        el
-00011480: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00011490: 6475 7261 7469 6f6e 5f74 6420 3d20 6475  duration_td = du
-000114a0: 7261 7469 6f6e 0a0a 2020 2020 2020 2020  ration..        
-000114b0: 6966 2064 7572 6174 696f 6e5f 7464 2e74  if duration_td.t
-000114c0: 6f74 616c 5f73 6563 6f6e 6473 2829 203e  otal_seconds() >
-000114d0: 2031 303a 0a20 2020 2020 2020 2020 2020   10:.           
-000114e0: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-000114f0: 7428 2243 6869 6d65 2064 7572 6174 696f  t("Chime duratio
-00011500: 6e20 6973 2074 6f6f 206c 6f6e 6722 290a  n is too long").
-00011510: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
-00011520: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
-00011530: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011540: 662e 6368 696d 655f 6475 7261 7469 6f6e  f.chime_duration
-00011550: 203d 2064 7572 6174 696f 6e5f 7464 0a0a   = duration_td..
-00011560: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00011570: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
-00011580: 6361 6c6c 6261 636b 290a 0a20 2020 2061  callback)..    a
-00011590: 7379 6e63 2064 6566 2073 6574 5f73 7973  sync def set_sys
-000115a0: 7465 6d5f 736f 756e 6473 2873 656c 662c  tem_sounds(self,
-000115b0: 2065 6e61 626c 6564 3a20 626f 6f6c 2920   enabled: bool) 
-000115c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000115d0: 2022 2222 5365 7473 2073 7973 7465 6d20   """Sets system 
-000115e0: 736f 756e 6420 706c 6179 6261 636b 2074  sound playback t
-000115f0: 6872 6f75 6768 2073 7065 616b 6572 732e  hrough speakers.
-00011600: 2052 6571 7569 7265 7320 6361 6d65 7261   Requires camera
-00011610: 2074 6f20 6861 7665 2073 7065 616b 6572   to have speaker
-00011620: 7322 2222 0a0a 2020 2020 2020 2020 6966  s"""..        if
-00011630: 206e 6f74 2073 656c 662e 6665 6174 7572   not self.featur
-00011640: 655f 666c 6167 732e 6861 735f 7370 6561  e_flags.has_spea
-00011650: 6b65 723a 0a20 2020 2020 2020 2020 2020  ker:.           
-00011660: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-00011670: 7428 2243 616d 6572 6120 646f 6573 206e  t("Camera does n
-00011680: 6f74 2068 6176 6520 7370 6561 6b65 7222  ot have speaker"
-00011690: 290a 0a20 2020 2020 2020 2064 6566 2063  )..        def c
-000116a0: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
-000116b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000116c0: 656c 662e 7370 6561 6b65 725f 7365 7474  elf.speaker_sett
-000116d0: 696e 6773 2e61 7265 5f73 7973 7465 6d5f  ings.are_system_
-000116e0: 736f 756e 6473 5f65 6e61 626c 6564 203d  sounds_enabled =
-000116f0: 2065 6e61 626c 6564 0a0a 2020 2020 2020   enabled..      
-00011700: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
-00011710: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
-00011720: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
-00011730: 6566 2073 6574 5f6f 7364 5f6e 616d 6528  ef set_osd_name(
-00011740: 7365 6c66 2c20 656e 6162 6c65 643a 2062  self, enabled: b
-00011750: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
-00011760: 2020 2020 2020 2222 2253 6574 7320 7768        """Sets wh
-00011770: 6574 6865 7220 6361 6d65 7261 206e 616d  ether camera nam
-00011780: 6520 6973 2069 6e20 7468 6520 4f6e 2053  e is in the On S
-00011790: 6372 6565 6e20 4469 7370 6c61 7922 2222  creen Display"""
-000117a0: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
-000117b0: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
-000117c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000117d0: 6c66 2e6f 7364 5f73 6574 7469 6e67 732e  lf.osd_settings.
-000117e0: 6973 5f6e 616d 655f 656e 6162 6c65 6420  is_name_enabled 
-000117f0: 3d20 656e 6162 6c65 640a 0a20 2020 2020  = enabled..     
-00011800: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
-00011810: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
-00011820: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
-00011830: 6465 6620 7365 745f 6f73 645f 6461 7465  def set_osd_date
-00011840: 2873 656c 662c 2065 6e61 626c 6564 3a20  (self, enabled: 
-00011850: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00011860: 2020 2020 2020 2022 2222 5365 7473 2077         """Sets w
-00011870: 6865 7468 6572 2063 7572 7265 6e74 2064  hether current d
-00011880: 6174 6520 6973 2069 6e20 7468 6520 4f6e  ate is in the On
-00011890: 2053 6372 6565 6e20 4469 7370 6c61 7922   Screen Display"
-000118a0: 2222 0a0a 2020 2020 2020 2020 6465 6620  ""..        def 
-000118b0: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
-000118c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000118d0: 7365 6c66 2e6f 7364 5f73 6574 7469 6e67  self.osd_setting
-000118e0: 732e 6973 5f64 6174 655f 656e 6162 6c65  s.is_date_enable
-000118f0: 6420 3d20 656e 6162 6c65 640a 0a20 2020  d = enabled..   
-00011900: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-00011910: 7175 6575 655f 7570 6461 7465 2863 616c  queue_update(cal
-00011920: 6c62 6163 6b29 0a0a 2020 2020 6173 796e  lback)..    asyn
-00011930: 6320 6465 6620 7365 745f 6f73 645f 6c6f  c def set_osd_lo
-00011940: 676f 2873 656c 662c 2065 6e61 626c 6564  go(self, enabled
-00011950: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-00011960: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
-00011970: 2077 6865 7468 6572 2074 6865 2055 6e69   whether the Uni
-00011980: 4669 206c 6f67 6f20 6973 2069 6e20 7468  Fi logo is in th
-00011990: 6520 4f6e 2053 6372 6565 6e20 4469 7370  e On Screen Disp
-000119a0: 6c61 7922 2222 0a0a 2020 2020 2020 2020  lay"""..        
-000119b0: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
-000119c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000119d0: 2020 2020 7365 6c66 2e6f 7364 5f73 6574      self.osd_set
-000119e0: 7469 6e67 732e 6973 5f6c 6f67 6f5f 656e  tings.is_logo_en
-000119f0: 6162 6c65 6420 3d20 656e 6162 6c65 640a  abled = enabled.
-00011a00: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-00011a10: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
-00011a20: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
-00011a30: 6173 796e 6320 6465 6620 7365 745f 6f73  async def set_os
-00011a40: 645f 6269 7472 6174 6528 7365 6c66 2c20  d_bitrate(self, 
-00011a50: 656e 6162 6c65 643a 2062 6f6f 6c29 202d  enabled: bool) -
-00011a60: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011a70: 2222 2253 6574 7320 7768 6574 6865 7220  """Sets whether 
-00011a80: 6361 6d65 7261 2062 6974 7261 7465 2069  camera bitrate i
-00011a90: 7320 696e 2074 6865 204f 6e20 5363 7265  s in the On Scre
-00011aa0: 656e 2044 6973 706c 6179 2222 220a 0a20  en Display""".. 
-00011ab0: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
-00011ac0: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
-00011ad0: 2020 2020 2020 2020 2020 2023 206d 6973             # mis
-00011ae0: 6d61 7463 6820 6265 7477 6565 6e20 5549  match between UI
-00011af0: 2069 6e74 6572 6e61 6c20 6461 7461 2073   internal data s
-00011b00: 7472 7563 7475 7265 2064 6562 7567 203d  tructure debug =
-00011b10: 2062 6974 7261 7465 2064 6174 610a 2020   bitrate data.  
-00011b20: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00011b30: 7364 5f73 6574 7469 6e67 732e 6973 5f64  sd_settings.is_d
-00011b40: 6562 7567 5f65 6e61 626c 6564 203d 2065  ebug_enabled = e
-00011b50: 6e61 626c 6564 0a0a 2020 2020 2020 2020  nabled..        
-00011b60: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
-00011b70: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
-00011b80: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00011b90: 2073 6574 5f73 6d61 7274 5f64 6574 6563   set_smart_detec
-00011ba0: 745f 7479 7065 7328 7365 6c66 2c20 7479  t_types(self, ty
-00011bb0: 7065 733a 206c 6973 745b 536d 6172 7444  pes: list[SmartD
-00011bc0: 6574 6563 744f 626a 6563 7454 7970 655d  etectObjectType]
-00011bd0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00011be0: 2020 2022 2222 5365 7473 2063 7572 7265     """Sets curre
-00011bf0: 6e74 2065 6e61 626c 6564 2073 6d61 7274  nt enabled smart
-00011c00: 2064 6574 6563 7469 6f6e 2074 7970 6573   detection types
-00011c10: 2e20 5265 7175 6972 6573 2063 616d 6572  . Requires camer
-00011c20: 6120 746f 2068 6176 6520 736d 6172 7420  a to have smart 
-00011c30: 6465 7465 6374 696f 6e22 2222 0a0a 2020  detection"""..  
-00011c40: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00011c50: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
-00011c60: 6861 735f 736d 6172 745f 6465 7465 6374  has_smart_detect
-00011c70: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00011c80: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00011c90: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
-00011ca0: 6861 7665 2061 2073 6d61 7274 2064 6574  have a smart det
-00011cb0: 6563 7469 6f6e 7322 290a 0a20 2020 2020  ections")..     
-00011cc0: 2020 2064 6566 2063 616c 6c62 6163 6b28     def callback(
-00011cd0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00011ce0: 2020 2020 2020 2073 656c 662e 736d 6172         self.smar
-00011cf0: 745f 6465 7465 6374 5f73 6574 7469 6e67  t_detect_setting
-00011d00: 732e 6f62 6a65 6374 5f74 7970 6573 203d  s.object_types =
-00011d10: 2074 7970 6573 0a0a 2020 2020 2020 2020   types..        
-00011d20: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
-00011d30: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
-00011d40: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00011d50: 2073 6574 5f73 6d61 7274 5f61 7564 696f   set_smart_audio
-00011d60: 5f64 6574 6563 745f 7479 7065 7328 0a20  _detect_types(. 
-00011d70: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00011d80: 2020 2020 2074 7970 6573 3a20 6c69 7374       types: list
-00011d90: 5b53 6d61 7274 4465 7465 6374 4175 6469  [SmartDetectAudi
-00011da0: 6f54 7970 655d 2c0a 2020 2020 2920 2d3e  oType],.    ) ->
-00011db0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00011dc0: 2222 5365 7473 2063 7572 7265 6e74 2065  ""Sets current e
-00011dd0: 6e61 626c 6564 2073 6d61 7274 2061 7564  nabled smart aud
-00011de0: 696f 2064 6574 6563 7469 6f6e 2074 7970  io detection typ
-00011df0: 6573 2e20 5265 7175 6972 6573 2063 616d  es. Requires cam
-00011e00: 6572 6120 746f 2068 6176 6520 736d 6172  era to have smar
-00011e10: 7420 6465 7465 6374 696f 6e22 2222 0a0a  t detection"""..
-00011e20: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00011e30: 656c 662e 6665 6174 7572 655f 666c 6167  elf.feature_flag
-00011e40: 732e 6861 735f 736d 6172 745f 6465 7465  s.has_smart_dete
-00011e50: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
-00011e60: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
-00011e70: 2822 4361 6d65 7261 2064 6f65 7320 6e6f  ("Camera does no
-00011e80: 7420 6861 7665 2061 2073 6d61 7274 2064  t have a smart d
-00011e90: 6574 6563 7469 6f6e 7322 290a 0a20 2020  etections")..   
-00011ea0: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
-00011eb0: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
-00011ec0: 2020 2020 2020 2020 2073 656c 662e 736d           self.sm
-00011ed0: 6172 745f 6465 7465 6374 5f73 6574 7469  art_detect_setti
-00011ee0: 6e67 732e 6175 6469 6f5f 7479 7065 7320  ngs.audio_types 
-00011ef0: 3d20 7479 7065 730a 0a20 2020 2020 2020  = types..       
-00011f00: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
-00011f10: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
-00011f20: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
-00011f30: 6620 5f73 6574 5f6f 626a 6563 745f 6465  f _set_object_de
-00011f40: 7465 6374 280a 2020 2020 2020 2020 7365  tect(.        se
-00011f50: 6c66 2c0a 2020 2020 2020 2020 6f62 6a5f  lf,.        obj_
-00011f60: 746f 5f6d 6f64 3a20 536d 6172 7444 6574  to_mod: SmartDet
-00011f70: 6563 744f 626a 6563 7454 7970 652c 0a20  ectObjectType,. 
-00011f80: 2020 2020 2020 2065 6e61 626c 6564 3a20         enabled: 
-00011f90: 626f 6f6c 2c0a 2020 2020 2920 2d3e 204e  bool,.    ) -> N
-00011fa0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00011fb0: 6f62 6a5f 746f 5f6d 6f64 206e 6f74 2069  obj_to_mod not i
-00011fc0: 6e20 7365 6c66 2e66 6561 7475 7265 5f66  n self.feature_f
-00011fd0: 6c61 6773 2e73 6d61 7274 5f64 6574 6563  lags.smart_detec
-00011fe0: 745f 7479 7065 733a 0a20 2020 2020 2020  t_types:.       
-00011ff0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-00012000: 7175 6573 7428 6622 4361 6d65 7261 2064  quest(f"Camera d
-00012010: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-00012020: 7468 6520 7b6f 626a 5f74 6f5f 6d6f 647d  the {obj_to_mod}
-00012030: 2064 6574 6563 7469 6f6e 2074 7970 6522   detection type"
-00012040: 290a 0a20 2020 2020 2020 2064 6566 2063  )..        def c
-00012050: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
-00012060: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
-00012070: 626a 6563 7473 203d 2073 656c 662e 736d  bjects = self.sm
-00012080: 6172 745f 6465 7465 6374 5f73 6574 7469  art_detect_setti
-00012090: 6e67 732e 6f62 6a65 6374 5f74 7970 6573  ngs.object_types
-000120a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000120b0: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
-000120c0: 2020 2020 2020 2020 2069 6620 6f62 6a5f           if obj_
-000120d0: 746f 5f6d 6f64 206e 6f74 2069 6e20 6f62  to_mod not in ob
-000120e0: 6a65 6374 733a 0a20 2020 2020 2020 2020  jects:.         
-000120f0: 2020 2020 2020 2020 2020 206f 626a 6563             objec
-00012100: 7473 203d 205b 2a6f 626a 6563 7473 2c20  ts = [*objects, 
-00012110: 6f62 6a5f 746f 5f6d 6f64 5d0a 2020 2020  obj_to_mod].    
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 6f62 6a65 6374 732e 736f 7274 2829 0a20  objects.sort(). 
-00012140: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00012150: 6f62 6a5f 746f 5f6d 6f64 2069 6e20 6f62  obj_to_mod in ob
-00012160: 6a65 6374 733a 0a20 2020 2020 2020 2020  jects:.         
-00012170: 2020 2020 2020 206f 626a 6563 7473 2e72         objects.r
-00012180: 656d 6f76 6528 6f62 6a5f 746f 5f6d 6f64  emove(obj_to_mod
-00012190: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000121a0: 6c66 2e73 6d61 7274 5f64 6574 6563 745f  lf.smart_detect_
-000121b0: 7365 7474 696e 6773 2e6f 626a 6563 745f  settings.object_
-000121c0: 7479 7065 7320 3d20 6f62 6a65 6374 730a  types = objects.
-000121d0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-000121e0: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
-000121f0: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
-00012200: 6173 796e 6320 6465 6620 5f73 6574 5f61  async def _set_a
-00012210: 7564 696f 5f64 6574 6563 7428 0a20 2020  udio_detect(.   
-00012220: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00012230: 2020 206f 626a 5f74 6f5f 6d6f 643a 2053     obj_to_mod: S
-00012240: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
-00012250: 7970 652c 0a20 2020 2020 2020 2065 6e61  ype,.        ena
-00012260: 626c 6564 3a20 626f 6f6c 2c0a 2020 2020  bled: bool,.    
-00012270: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012280: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00012290: 2020 2020 7365 6c66 2e66 6561 7475 7265      self.feature
-000122a0: 5f66 6c61 6773 2e73 6d61 7274 5f64 6574  _flags.smart_det
-000122b0: 6563 745f 6175 6469 6f5f 7479 7065 7320  ect_audio_types 
-000122c0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
-000122d0: 2020 2020 6f72 206f 626a 5f74 6f5f 6d6f      or obj_to_mo
-000122e0: 6420 6e6f 7420 696e 2073 656c 662e 6665  d not in self.fe
-000122f0: 6174 7572 655f 666c 6167 732e 736d 6172  ature_flags.smar
-00012300: 745f 6465 7465 6374 5f61 7564 696f 5f74  t_detect_audio_t
-00012310: 7970 6573 0a20 2020 2020 2020 2029 3a0a  ypes.        ):.
-00012320: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00012330: 6520 4261 6452 6571 7565 7374 2866 2243  e BadRequest(f"C
-00012340: 616d 6572 6120 646f 6573 206e 6f74 2073  amera does not s
-00012350: 7570 706f 7274 2074 6865 207b 6f62 6a5f  upport the {obj_
-00012360: 746f 5f6d 6f64 7d20 6465 7465 6374 696f  to_mod} detectio
-00012370: 6e20 7479 7065 2229 0a0a 2020 2020 2020  n type")..      
-00012380: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
-00012390: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000123a0: 2020 2020 2020 6f62 6a65 6374 7320 3d20        objects = 
-000123b0: 7365 6c66 2e73 6d61 7274 5f64 6574 6563  self.smart_detec
-000123c0: 745f 7365 7474 696e 6773 2e61 7564 696f  t_settings.audio
-000123d0: 5f74 7970 6573 206f 7220 5b5d 0a20 2020  _types or [].   
-000123e0: 2020 2020 2020 2020 2069 6620 656e 6162           if enab
-000123f0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00012400: 2020 2020 2069 6620 6f62 6a5f 746f 5f6d       if obj_to_m
-00012410: 6f64 206e 6f74 2069 6e20 6f62 6a65 6374  od not in object
-00012420: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00012430: 2020 2020 2020 206f 626a 6563 7473 203d         objects =
-00012440: 205b 2a6f 626a 6563 7473 2c20 6f62 6a5f   [*objects, obj_
-00012450: 746f 5f6d 6f64 5d0a 2020 2020 2020 2020  to_mod].        
-00012460: 2020 2020 2020 2020 2020 2020 6f62 6a65              obje
-00012470: 6374 732e 736f 7274 2829 0a20 2020 2020  cts.sort().     
-00012480: 2020 2020 2020 2065 6c69 6620 6f62 6a5f         elif obj_
-00012490: 746f 5f6d 6f64 2069 6e20 6f62 6a65 6374  to_mod in object
-000124a0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000124b0: 2020 206f 626a 6563 7473 2e72 656d 6f76     objects.remov
-000124c0: 6528 6f62 6a5f 746f 5f6d 6f64 290a 2020  e(obj_to_mod).  
-000124d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000124e0: 6d61 7274 5f64 6574 6563 745f 7365 7474  mart_detect_sett
-000124f0: 696e 6773 2e61 7564 696f 5f74 7970 6573  ings.audio_types
-00012500: 203d 206f 626a 6563 7473 0a0a 2020 2020   = objects..    
-00012510: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00012520: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00012530: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-00012540: 2064 6566 2073 6574 5f6c 6364 5f74 6578   def set_lcd_tex
-00012550: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-00012560: 0a20 2020 2020 2020 2074 6578 745f 7479  .        text_ty
-00012570: 7065 3a20 4f70 7469 6f6e 616c 5b44 6f6f  pe: Optional[Doo
-00012580: 7262 656c 6c4d 6573 7361 6765 5479 7065  rbellMessageType
-00012590: 5d2c 0a20 2020 2020 2020 2074 6578 743a  ],.        text:
-000125a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-000125b0: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-000125c0: 6573 6574 5f61 743a 2055 6e69 6f6e 5b4e  eset_at: Union[N
-000125d0: 6f6e 652c 2064 6174 6574 696d 652c 2044  one, datetime, D
-000125e0: 4546 4155 4c54 5f54 5950 455d 203d 204e  EFAULT_TYPE] = N
-000125f0: 6f6e 652c 0a20 2020 2029 202d 3e20 4e6f  one,.    ) -> No
-00012600: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
-00012610: 6574 7320 646f 6f72 6265 6c6c 204c 4344  ets doorbell LCD
-00012620: 2074 6578 742e 2052 6571 7569 7265 7320   text. Requires 
-00012630: 6361 6d65 7261 2074 6f20 6265 2064 6f6f  camera to be doo
-00012640: 7262 656c 6c22 2222 0a0a 2020 2020 2020  rbell"""..      
-00012650: 2020 6966 206e 6f74 2073 656c 662e 6665    if not self.fe
-00012660: 6174 7572 655f 666c 6167 732e 6861 735f  ature_flags.has_
-00012670: 6c63 645f 7363 7265 656e 3a0a 2020 2020  lcd_screen:.    
-00012680: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
-00012690: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
-000126a0: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
-000126b0: 6e20 4c43 4420 7363 7265 656e 2229 0a0a  n LCD screen")..
-000126c0: 2020 2020 2020 2020 6966 2074 6578 745f          if text_
-000126d0: 7479 7065 2069 7320 4e6f 6e65 3a0a 2020  type is None:.  
-000126e0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
-000126f0: 7769 7468 2073 656c 662e 5f75 7064 6174  with self._updat
-00012700: 655f 6c6f 636b 3a0a 2020 2020 2020 2020  e_lock:.        
-00012710: 2020 2020 2020 2020 6177 6169 7420 6173          await as
-00012720: 796e 6369 6f2e 736c 6565 7028 0a20 2020  yncio.sleep(.   
-00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
-00012750: 2020 2020 2920 2023 2079 6965 6c64 2074      )  # yield t
-00012760: 6f20 7468 6520 6576 656e 7420 6c6f 6f70  o the event loop
-00012770: 206f 6e63 6520 7765 2068 6176 6520 7468   once we have th
-00012780: 6520 6c6f 636b 2074 6f20 7072 6f63 6573  e lock to proces
-00012790: 7320 616e 7920 7065 6e64 696e 6720 7570  s any pending up
-000127a0: 6461 7465 730a 2020 2020 2020 2020 2020  dates.          
-000127b0: 2020 2020 2020 6461 7461 5f62 6566 6f72        data_befor
-000127c0: 655f 6368 616e 6765 7320 3d20 7365 6c66  e_changes = self
-000127d0: 2e64 6963 745f 7769 7468 5f65 7863 6c75  .dict_with_exclu
-000127e0: 6465 7328 290a 2020 2020 2020 2020 2020  des().          
-000127f0: 2020 2020 2020 7365 6c66 2e6c 6364 5f6d        self.lcd_m
-00012800: 6573 7361 6765 203d 204e 6f6e 650a 2020  essage = None.  
-00012810: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00012820: 556e 6946 6920 5072 6f74 6563 7420 6275  UniFi Protect bu
-00012830: 673a 2063 6c65 6172 696e 6720 4c43 4420  g: clearing LCD 
-00012840: 7465 7874 206d 6573 7361 6765 2064 6f65  text message doe
-00012850: 7320 5f6e 6f74 5f20 656d 6974 2061 2057  s _not_ emit a W
-00012860: 5320 6d65 7373 6167 650a 2020 2020 2020  S message.      
-00012870: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00012880: 7365 6c66 2e73 6176 655f 6465 7669 6365  self.save_device
-00012890: 2864 6174 615f 6265 666f 7265 5f63 6861  (data_before_cha
-000128a0: 6e67 6573 2c20 666f 7263 655f 656d 6974  nges, force_emit
-000128b0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-000128c0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-000128d0: 2020 2020 2020 2069 6620 7465 7874 5f74         if text_t
-000128e0: 7970 6520 213d 2044 6f6f 7262 656c 6c4d  ype != DoorbellM
-000128f0: 6573 7361 6765 5479 7065 2e43 5553 544f  essageType.CUSTO
-00012900: 4d5f 4d45 5353 4147 453a 0a20 2020 2020  M_MESSAGE:.     
-00012910: 2020 2020 2020 2069 6620 7465 7874 2069         if text i
-00012920: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00012930: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00012940: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
-00012950: 6e20 6f6e 6c79 2073 6574 2074 6578 7420  n only set text 
-00012960: 6966 2074 6578 745f 7479 7065 2069 7320  if text_type is 
-00012970: 4355 5354 4f4d 5f4d 4553 5341 4745 2229  CUSTOM_MESSAGE")
-00012980: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00012990: 7420 3d20 7465 7874 5f74 7970 652e 7661  t = text_type.va
-000129a0: 6c75 652e 7265 706c 6163 6528 225f 222c  lue.replace("_",
-000129b0: 2022 2022 290a 0a20 2020 2020 2020 2069   " ")..        i
-000129c0: 6620 7265 7365 745f 6174 203d 3d20 4445  f reset_at == DE
-000129d0: 4641 554c 543a 0a20 2020 2020 2020 2020  FAULT:.         
-000129e0: 2020 2072 6573 6574 5f61 7420 3d20 280a     reset_at = (.
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 7574 635f 6e6f 7728 290a 2020 2020 2020  utc_now().      
-00012a10: 2020 2020 2020 2020 2020 2b20 7365 6c66            + self
-00012a20: 2e61 7069 2e62 6f6f 7473 7472 6170 2e6e  .api.bootstrap.n
-00012a30: 7672 2e64 6f6f 7262 656c 6c5f 7365 7474  vr.doorbell_sett
-00012a40: 696e 6773 2e64 6566 6175 6c74 5f6d 6573  ings.default_mes
-00012a50: 7361 6765 5f72 6573 6574 5f74 696d 656f  sage_reset_timeo
-00012a60: 7574 0a20 2020 2020 2020 2020 2020 2029  ut.            )
-00012a70: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
-00012a80: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
-00012a90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012aa0: 6c66 2e6c 6364 5f6d 6573 7361 6765 203d  lf.lcd_message =
-00012ab0: 204c 4344 4d65 7373 6167 6528 2020 2320   LCDMessage(  # 
-00012ac0: 7479 7065 3a20 6967 6e6f 7265 5b63 616c  type: ignore[cal
-00012ad0: 6c2d 6172 675d 0a20 2020 2020 2020 2020  l-arg].         
-00012ae0: 2020 2020 2020 2061 7069 3d73 656c 662e         api=self.
-00012af0: 5f61 7069 2c0a 2020 2020 2020 2020 2020  _api,.          
-00012b00: 2020 2020 2020 7479 7065 3d74 6578 745f        type=text_
-00012b10: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-00012b20: 2020 2020 2020 7465 7874 3d74 6578 742c        text=text,
-00012b30: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-00012b40: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
-00012b50: 2020 2020 2020 2020 2020 2072 6573 6574             reset
-00012b60: 5f61 743d 7265 7365 745f 6174 2c20 2023  _at=reset_at,  #
-00012b70: 2074 7970 653a 2069 676e 6f72 655b 6172   type: ignore[ar
-00012b80: 672d 7479 7065 5d0a 2020 2020 2020 2020  g-type].        
-00012b90: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
-00012ba0: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
-00012bb0: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
-00012bc0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00012bd0: 7365 745f 7072 6976 6163 7928 0a20 2020  set_privacy(.   
-00012be0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00012bf0: 2020 2065 6e61 626c 6564 3a20 626f 6f6c     enabled: bool
-00012c00: 2c0a 2020 2020 2020 2020 6d69 635f 6c65  ,.        mic_le
-00012c10: 7665 6c3a 204f 7074 696f 6e61 6c5b 696e  vel: Optional[in
-00012c20: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-00012c30: 2020 2072 6563 6f72 6469 6e67 5f6d 6f64     recording_mod
-00012c40: 653a 204f 7074 696f 6e61 6c5b 5265 636f  e: Optional[Reco
-00012c50: 7264 696e 674d 6f64 655d 203d 204e 6f6e  rdingMode] = Non
-00012c60: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
-00012c70: 3a0a 2020 2020 2020 2020 2222 2241 6464  :.        """Add
-00012c80: 732f 7265 6d6f 7665 7320 6120 7072 6976  s/removes a priv
-00012c90: 6163 7920 7a6f 6e65 2074 6861 7420 626c  acy zone that bl
-00012ca0: 6163 6b73 206f 7574 2074 6865 2077 686f  acks out the who
-00012cb0: 6c65 2063 616d 6572 6122 2222 0a0a 2020  le camera"""..  
-00012cc0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00012cd0: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
-00012ce0: 6861 735f 7072 6976 6163 795f 6d61 736b  has_privacy_mask
-00012cf0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00012d00: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00012d10: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
-00012d20: 616c 6c6f 7720 7072 6976 6163 7920 7a6f  allow privacy zo
-00012d30: 6e65 7322 290a 0a20 2020 2020 2020 2064  nes")..        d
-00012d40: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
-00012d50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012d60: 2020 2069 6620 656e 6162 6c65 643a 0a20     if enabled:. 
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012d80: 656c 662e 6164 645f 7072 6976 6163 795f  elf.add_privacy_
-00012d90: 7a6f 6e65 2829 0a20 2020 2020 2020 2020  zone().         
-00012da0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012db0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00012dc0: 6d6f 7665 5f70 7269 7661 6379 5f7a 6f6e  move_privacy_zon
-00012dd0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
-00012de0: 2069 6620 6d69 635f 6c65 7665 6c20 6973   if mic_level is
-00012df0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00012e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012e10: 6d69 635f 766f 6c75 6d65 203d 2050 6572  mic_volume = Per
-00012e20: 6365 6e74 496e 7428 6d69 635f 6c65 7665  centInt(mic_leve
-00012e30: 6c29 0a0a 2020 2020 2020 2020 2020 2020  l)..            
-00012e40: 6966 2072 6563 6f72 6469 6e67 5f6d 6f64  if recording_mod
-00012e50: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012e70: 656c 662e 7265 636f 7264 696e 675f 7365  elf.recording_se
-00012e80: 7474 696e 6773 2e6d 6f64 6520 3d20 7265  ttings.mode = re
-00012e90: 636f 7264 696e 675f 6d6f 6465 0a0a 2020  cording_mode..  
-00012ea0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-00012eb0: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
-00012ec0: 6c6c 6261 636b 290a 0a20 2020 2061 7379  llback)..    asy
-00012ed0: 6e63 2064 6566 2073 6574 5f70 6572 736f  nc def set_perso
-00012ee0: 6e5f 7472 6163 6b28 7365 6c66 2c20 656e  n_track(self, en
-00012ef0: 6162 6c65 643a 2062 6f6f 6c29 202d 3e20  abled: bool) -> 
-00012f00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00012f10: 2253 6574 7320 7065 7273 6f6e 2074 7261  "Sets person tra
-00012f20: 636b 696e 6720 6f6e 2063 616d 6572 6122  cking on camera"
-00012f30: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
-00012f40: 6f74 2073 656c 662e 6665 6174 7572 655f  ot self.feature_
-00012f50: 666c 6167 732e 6973 5f70 747a 3a0a 2020  flags.is_ptz:.  
-00012f60: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00012f70: 4261 6452 6571 7565 7374 2822 4361 6d65  BadRequest("Came
-00012f80: 7261 2064 6f65 7320 6e6f 7420 7375 7070  ra does not supp
-00012f90: 6f72 7420 7065 7273 6f6e 2074 7261 636b  ort person track
-00012fa0: 696e 6722 290a 0a20 2020 2020 2020 2064  ing")..        d
-00012fb0: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
-00012fc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012fd0: 2020 2073 656c 662e 736d 6172 745f 6465     self.smart_de
-00012fe0: 7465 6374 5f73 6574 7469 6e67 732e 6175  tect_settings.au
-00012ff0: 746f 5f74 7261 636b 696e 675f 6f62 6a65  to_tracking_obje
-00013000: 6374 5f74 7970 6573 203d 2028 0a20 2020  ct_types = (.   
-00013010: 2020 2020 2020 2020 2020 2020 205b 536d               [Sm
-00013020: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
-00013030: 7970 652e 5045 5253 4f4e 5d20 6966 2065  ype.PERSON] if e
-00013040: 6e61 626c 6564 2065 6c73 6520 5b5d 0a20  nabled else []. 
-00013050: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00013060: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-00013070: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
-00013080: 6c6c 6261 636b 290a 0a20 2020 2064 6566  llback)..    def
-00013090: 2063 7265 6174 655f 7461 6c6b 6261 636b   create_talkback
-000130a0: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
-000130b0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-000130c0: 6f6e 7465 6e74 5f75 726c 3a20 7374 722c  ontent_url: str,
-000130d0: 0a20 2020 2020 2020 2066 666d 7065 675f  .        ffmpeg_
-000130e0: 7061 7468 3a20 4f70 7469 6f6e 616c 5b50  path: Optional[P
-000130f0: 6174 685d 203d 204e 6f6e 652c 0a20 2020  ath] = None,.   
-00013100: 2029 202d 3e20 5461 6c6b 6261 636b 5374   ) -> TalkbackSt
-00013110: 7265 616d 3a0a 2020 2020 2020 2020 2222  ream:.        ""
-00013120: 2243 7265 6174 6573 2061 2073 7562 7072  "Creates a subpr
-00013130: 6f63 6573 7320 746f 2070 6c61 7920 6175  ocess to play au
-00013140: 6469 6f20 746f 2061 2063 616d 6572 6120  dio to a camera 
-00013150: 7468 726f 7567 6820 6974 7320 7370 6561  through its spea
-00013160: 6b65 722e 0a0a 2020 2020 2020 2020 5265  ker...        Re
-00013170: 7175 6972 6573 2066 666d 7065 6720 746f  quires ffmpeg to
-00013180: 2075 7365 2e0a 0a20 2020 2020 2020 2041   use...        A
-00013190: 7267 733a 0a20 2020 2020 2020 202d 2d2d  rgs:.        ---
-000131a0: 2d0a 2020 2020 2020 2020 2020 2020 636f  -.            co
-000131b0: 6e74 656e 745f 7572 6c3a 2045 6974 6865  ntent_url: Eithe
-000131c0: 7220 6120 5552 4c20 6163 6365 7373 6962  r a URL accessib
-000131d0: 6c65 2062 7920 7079 7468 6f6e 206f 7220  le by python or 
-000131e0: 6120 7061 7468 2074 6f20 6120 6669 6c65  a path to a file
-000131f0: 2028 6666 6d65 7067 2773 2060 2d69 6020   (ffmepg's `-i` 
-00013200: 7061 7261 6d65 7465 7229 0a20 2020 2020  parameter).     
-00013210: 2020 2020 2020 2066 666d 7065 675f 7061         ffmpeg_pa
-00013220: 7468 3a20 4f70 7469 6f6e 616c 2070 6174  th: Optional pat
-00013230: 6820 746f 2066 666d 7065 6720 6269 6e61  h to ffmpeg bina
-00013240: 7279 0a0a 2020 2020 2020 2020 5573 6520  ry..        Use 
-00013250: 6569 7468 6572 2060 6177 6169 7420 7374  either `await st
-00013260: 7265 616d 2e72 756e 5f75 6e74 696c 5f63  ream.run_until_c
-00013270: 6f6d 706c 6574 6528 2960 206f 7220 6061  omplete()` or `a
-00013280: 7761 6974 2073 7472 6561 6d2e 7374 6172  wait stream.star
-00013290: 7428 2960 2074 6f20 7374 6172 7420 7375  t()` to start su
-000132a0: 6270 726f 6365 7373 2063 6f6d 6d61 6e64  bprocess command
-000132b0: 0a20 2020 2020 2020 2061 6674 6572 2067  .        after g
-000132c0: 6574 7469 6e67 2074 6865 2073 7472 6561  etting the strea
-000132d0: 6d2e 0a0a 2020 2020 2020 2020 602e 706c  m...        `.pl
-000132e0: 6179 5f61 7564 696f 2829 6020 6973 2061  ay_audio()` is a
-000132f0: 2068 656c 7065 7220 7468 6174 2077 7261   helper that wra
-00013300: 7073 2074 6869 7320 6d65 7468 6f64 2061  ps this method a
-00013310: 6e64 2061 7574 6f6d 6174 6963 616c 6c79  nd automatically
-00013320: 2072 756e 7320 7468 6520 7375 6270 726f   runs the subpro
-00013330: 6365 7373 2061 7320 7765 6c6c 0a20 2020  cess as well.   
-00013340: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00013350: 2020 6966 2073 656c 662e 7461 6c6b 6261    if self.talkba
-00013360: 636b 5f73 7472 6561 6d20 6973 206e 6f74  ck_stream is not
-00013370: 204e 6f6e 6520 616e 6420 7365 6c66 2e74   None and self.t
-00013380: 616c 6b62 6163 6b5f 7374 7265 616d 2e69  alkback_stream.i
-00013390: 735f 7275 6e6e 696e 673a 0a20 2020 2020  s_running:.     
-000133a0: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
-000133b0: 5265 7175 6573 7428 2243 616d 6572 6120  Request("Camera 
-000133c0: 6973 2061 6c72 6561 6479 2070 6c61 7969  is already playi
-000133d0: 6e67 2061 7564 696f 2229 0a0a 2020 2020  ng audio")..    
-000133e0: 2020 2020 7365 6c66 2e74 616c 6b62 6163      self.talkbac
-000133f0: 6b5f 7374 7265 616d 203d 2054 616c 6b62  k_stream = Talkb
-00013400: 6163 6b53 7472 6561 6d28 7365 6c66 2c20  ackStream(self, 
-00013410: 636f 6e74 656e 745f 7572 6c2c 2066 666d  content_url, ffm
-00013420: 7065 675f 7061 7468 290a 2020 2020 2020  peg_path).      
-00013430: 2020 7265 7475 726e 2073 656c 662e 7461    return self.ta
-00013440: 6c6b 6261 636b 5f73 7472 6561 6d0a 0a20  lkback_stream.. 
-00013450: 2020 2061 7379 6e63 2064 6566 2070 6c61     async def pla
-00013460: 795f 6175 6469 6f28 0a20 2020 2020 2020  y_audio(.       
-00013470: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-00013480: 6f6e 7465 6e74 5f75 726c 3a20 7374 722c  ontent_url: str,
-00013490: 0a20 2020 2020 2020 2066 666d 7065 675f  .        ffmpeg_
-000134a0: 7061 7468 3a20 4f70 7469 6f6e 616c 5b50  path: Optional[P
-000134b0: 6174 685d 203d 204e 6f6e 652c 0a20 2020  ath] = None,.   
-000134c0: 2020 2020 2062 6c6f 636b 696e 673a 2062       blocking: b
-000134d0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-000134e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000134f0: 2020 2022 2222 506c 6179 7320 6175 6469     """Plays audi
-00013500: 6f20 746f 2061 2063 616d 6572 6120 7468  o to a camera th
-00013510: 726f 7567 6820 6974 7320 7370 6561 6b65  rough its speake
-00013520: 722e 0a0a 2020 2020 2020 2020 5265 7175  r...        Requ
-00013530: 6972 6573 2066 666d 7065 6720 746f 2075  ires ffmpeg to u
-00013540: 7365 2e0a 0a20 2020 2020 2020 2041 7267  se...        Arg
-00013550: 733a 0a20 2020 2020 2020 202d 2d2d 2d0a  s:.        ----.
-00013560: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00013570: 656e 745f 7572 6c3a 2045 6974 6865 7220  ent_url: Either 
-00013580: 6120 5552 4c20 6163 6365 7373 6962 6c65  a URL accessible
-00013590: 2062 7920 7079 7468 6f6e 206f 7220 6120   by python or a 
-000135a0: 7061 7468 2074 6f20 6120 6669 6c65 2028  path to a file (
-000135b0: 6666 6d65 7067 2773 2060 2d69 6020 7061  ffmepg's `-i` pa
-000135c0: 7261 6d65 7465 7229 0a20 2020 2020 2020  rameter).       
-000135d0: 2020 2020 2066 666d 7065 675f 7061 7468       ffmpeg_path
-000135e0: 3a20 4f70 7469 6f6e 616c 2070 6174 6820  : Optional path 
-000135f0: 746f 2066 666d 7065 6720 6269 6e61 7279  to ffmpeg binary
-00013600: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-00013610: 636b 696e 673a 2041 7761 6974 7320 7374  cking: Awaits st
-00013620: 7265 616d 2063 6f6d 706c 6574 696f 6e20  ream completion 
-00013630: 616e 6420 6c6f 6773 2073 7464 6f75 742f  and logs stdout/
-00013640: 7374 6465 7272 0a20 2020 2020 2020 2022  stderr.        "
-00013650: 2222 0a0a 2020 2020 2020 2020 7374 7265  ""..        stre
-00013660: 616d 203d 2073 656c 662e 6372 6561 7465  am = self.create
-00013670: 5f74 616c 6b62 6163 6b5f 7374 7265 616d  _talkback_stream
-00013680: 2863 6f6e 7465 6e74 5f75 726c 2c20 6666  (content_url, ff
-00013690: 6d70 6567 5f70 6174 6829 0a20 2020 2020  mpeg_path).     
-000136a0: 2020 2061 7761 6974 2073 7472 6561 6d2e     await stream.
-000136b0: 7374 6172 7428 290a 0a20 2020 2020 2020  start()..       
-000136c0: 2069 6620 626c 6f63 6b69 6e67 3a0a 2020   if blocking:.  
-000136d0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-000136e0: 7365 6c66 2e77 6169 745f 756e 7469 6c5f  self.wait_until_
-000136f0: 6175 6469 6f5f 636f 6d70 6c65 7465 7328  audio_completes(
-00013700: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00013710: 2077 6169 745f 756e 7469 6c5f 6175 6469   wait_until_audi
-00013720: 6f5f 636f 6d70 6c65 7465 7328 7365 6c66  o_completes(self
-00013730: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00013740: 2020 2022 2222 4177 6169 7473 2073 7472     """Awaits str
-00013750: 6561 6d20 636f 6d70 6c65 7469 6f6e 206f  eam completion o
-00013760: 6620 6175 6469 6f20 616e 6420 6c6f 6773  f audio and logs
-00013770: 2073 7464 6f75 742f 7374 6465 7272 2e22   stdout/stderr."
-00013780: 2222 0a0a 2020 2020 2020 2020 7374 7265  ""..        stre
-00013790: 616d 203d 2073 656c 662e 7461 6c6b 6261  am = self.talkba
-000137a0: 636b 5f73 7472 6561 6d0a 2020 2020 2020  ck_stream.      
-000137b0: 2020 6966 2073 7472 6561 6d20 6973 204e    if stream is N
-000137c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000137d0: 2072 6169 7365 2053 7472 6561 6d45 7272   raise StreamErr
-000137e0: 6f72 2822 4e6f 2061 7564 696f 2070 6c61  or("No audio pla
-000137f0: 7969 6e67 2074 6f20 7761 6974 2066 6f72  ying to wait for
-00013800: 2229 0a0a 2020 2020 2020 2020 6177 6169  ")..        awai
-00013810: 7420 7374 7265 616d 2e72 756e 5f75 6e74  t stream.run_unt
-00013820: 696c 5f63 6f6d 706c 6574 6528 290a 0a20  il_complete().. 
-00013830: 2020 2020 2020 205f 4c4f 4747 4552 2e64         _LOGGER.d
-00013840: 6562 7567 2822 6666 6d70 6567 2073 7464  ebug("ffmpeg std
-00013850: 6f75 743a 5c6e 2573 222c 2022 5c6e 222e  out:\n%s", "\n".
-00013860: 6a6f 696e 2873 7472 6561 6d2e 7374 646f  join(stream.stdo
-00013870: 7574 2929 0a20 2020 2020 2020 205f 4c4f  ut)).        _LO
-00013880: 4747 4552 2e64 6562 7567 2822 6666 6d70  GGER.debug("ffmp
-00013890: 6567 2073 7464 6572 723a 5c6e 2573 222c  eg stderr:\n%s",
-000138a0: 2022 5c6e 222e 6a6f 696e 2873 7472 6561   "\n".join(strea
-000138b0: 6d2e 7374 6465 7272 2929 0a20 2020 2020  m.stderr)).     
-000138c0: 2020 2069 6620 7374 7265 616d 2e69 735f     if stream.is_
-000138d0: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
-000138e0: 2020 2065 7272 6f72 203d 2022 5c6e 222e     error = "\n".
-000138f0: 6a6f 696e 2873 7472 6561 6d2e 7374 6465  join(stream.stde
-00013900: 7272 290a 2020 2020 2020 2020 2020 2020  rr).            
-00013910: 7261 6973 6520 5374 7265 616d 4572 726f  raise StreamErro
-00013920: 7228 2245 7272 6f72 2077 6869 6c65 2070  r("Error while p
-00013930: 6c61 7969 6e67 2061 7564 696f 2028 6666  laying audio (ff
-00013940: 6d70 6567 293a 205c 6e22 202b 2065 7272  mpeg): \n" + err
-00013950: 6f72 290a 0a20 2020 2061 7379 6e63 2064  or)..    async d
-00013960: 6566 2073 746f 705f 6175 6469 6f28 7365  ef stop_audio(se
-00013970: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00013980: 2020 2020 2022 2222 5374 6f70 2063 7572       """Stop cur
-00013990: 7265 6e74 6c79 2070 6c61 7969 6e67 2061  rently playing a
-000139a0: 7564 696f 2e22 2222 0a20 2020 2020 2020  udio.""".       
-000139b0: 2073 7472 6561 6d20 3d20 7365 6c66 2e74   stream = self.t
-000139c0: 616c 6b62 6163 6b5f 7374 7265 616d 0a20  alkback_stream. 
-000139d0: 2020 2020 2020 2069 6620 7374 7265 616d         if stream
-000139e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000139f0: 2020 2020 2020 7261 6973 6520 5374 7265        raise Stre
-00013a00: 616d 4572 726f 7228 224e 6f20 6175 6469  amError("No audi
-00013a10: 6f20 706c 6179 696e 6720 746f 2073 746f  o playing to sto
-00013a20: 7022 290a 0a20 2020 2020 2020 2061 7761  p")..        awa
-00013a30: 6974 2073 7472 6561 6d2e 7374 6f70 2829  it stream.stop()
-00013a40: 0a0a 2020 2020 6465 6620 6361 6e5f 7265  ..    def can_re
-00013a50: 6164 5f6d 6564 6961 2873 656c 662c 2075  ad_media(self, u
-00013a60: 7365 723a 2055 7365 7229 202d 3e20 626f  ser: User) -> bo
-00013a70: 6f6c 3a0a 2020 2020 2020 2020 6966 2073  ol:.        if s
-00013a80: 656c 662e 6d6f 6465 6c20 6973 204e 6f6e  elf.model is Non
-00013a90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013aa0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00013ab0: 2020 2020 7265 7475 726e 2075 7365 722e      return user.
-00013ac0: 6361 6e28 7365 6c66 2e6d 6f64 656c 2c20  can(self.model, 
-00013ad0: 5065 726d 6973 7369 6f6e 4e6f 6465 2e52  PermissionNode.R
-00013ae0: 4541 445f 4d45 4449 412c 2073 656c 6629  EAD_MEDIA, self)
-00013af0: 0a0a 2020 2020 6465 6620 6361 6e5f 6465  ..    def can_de
-00013b00: 6c65 7465 5f6d 6564 6961 2873 656c 662c  lete_media(self,
-00013b10: 2075 7365 723a 2055 7365 7229 202d 3e20   user: User) -> 
-00013b20: 626f 6f6c 3a0a 2020 2020 2020 2020 6966  bool:.        if
-00013b30: 2073 656c 662e 6d6f 6465 6c20 6973 204e   self.model is N
-00013b40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00013b50: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-00013b60: 2020 2020 2020 7265 7475 726e 2075 7365        return use
-00013b70: 722e 6361 6e28 7365 6c66 2e6d 6f64 656c  r.can(self.model
-00013b80: 2c20 5065 726d 6973 7369 6f6e 4e6f 6465  , PermissionNode
-00013b90: 2e44 454c 4554 455f 4d45 4449 412c 2073  .DELETE_MEDIA, s
-00013ba0: 656c 6629 0a0a 0a63 6c61 7373 2056 6965  elf)...class Vie
-00013bb0: 7765 7228 5072 6f74 6563 7441 646f 7074  wer(ProtectAdopt
-00013bc0: 6162 6c65 4465 7669 6365 4d6f 6465 6c29  ableDeviceModel)
-00013bd0: 3a0a 2020 2020 7374 7265 616d 5f6c 696d  :.    stream_lim
-00013be0: 6974 3a20 696e 740a 2020 2020 736f 6674  it: int.    soft
-00013bf0: 7761 7265 5f76 6572 7369 6f6e 3a20 7374  ware_version: st
-00013c00: 720a 2020 2020 6c69 7665 7669 6577 5f69  r.    liveview_i
-00013c10: 643a 2073 7472 0a0a 2020 2020 4063 6c61  d: str..    @cla
-00013c20: 7373 6d65 7468 6f64 0a20 2020 2040 6361  ssmethod.    @ca
-00013c30: 6368 650a 2020 2020 6465 6620 5f67 6574  che.    def _get
-00013c40: 5f75 6e69 6669 5f72 656d 6170 7328 636c  _unifi_remaps(cl
-00013c50: 7329 202d 3e20 6469 6374 5b73 7472 2c20  s) -> dict[str, 
-00013c60: 7374 725d 3a0a 2020 2020 2020 2020 7265  str]:.        re
-00013c70: 7475 726e 207b 2a2a 7375 7065 7228 292e  turn {**super().
-00013c80: 5f67 6574 5f75 6e69 6669 5f72 656d 6170  _get_unifi_remap
-00013c90: 7328 292c 2022 6c69 7665 7669 6577 223a  s(), "liveview":
-00013ca0: 2022 6c69 7665 7669 6577 4964 227d 0a0a   "liveviewId"}..
-00013cb0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00013cc0: 0a20 2020 2040 6361 6368 650a 2020 2020  .    @cache.    
-00013cd0: 6465 6620 5f67 6574 5f72 6561 645f 6f6e  def _get_read_on
-00013ce0: 6c79 5f66 6965 6c64 7328 636c 7329 202d  ly_fields(cls) -
-00013cf0: 3e20 7365 745b 7374 725d 3a0a 2020 2020  > set[str]:.    
-00013d00: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00013d10: 2829 2e5f 6765 745f 7265 6164 5f6f 6e6c  ()._get_read_onl
-00013d20: 795f 6669 656c 6473 2829 207c 207b 2273  y_fields() | {"s
-00013d30: 6f66 7477 6172 6556 6572 7369 6f6e 227d  oftwareVersion"}
-00013d40: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00013d50: 2020 2020 6465 6620 6c69 7665 7669 6577      def liveview
-00013d60: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00013d70: 616c 5b4c 6976 6576 6965 775d 3a0a 2020  al[Liveview]:.  
-00013d80: 2020 2020 2020 2320 7573 6572 206d 6179        # user may
-00013d90: 206e 6f74 2068 6176 6520 7065 726d 6973   not have permis
-00013da0: 7369 6f6e 2074 6f20 7365 6520 7468 6520  sion to see the 
-00013db0: 6c69 7665 7669 6577 0a20 2020 2020 2020  liveview.       
-00013dc0: 2072 6574 7572 6e20 7365 6c66 2e61 7069   return self.api
-00013dd0: 2e62 6f6f 7473 7472 6170 2e6c 6976 6576  .bootstrap.livev
-00013de0: 6965 7773 2e67 6574 2873 656c 662e 6c69  iews.get(self.li
-00013df0: 7665 7669 6577 5f69 6429 0a0a 2020 2020  veview_id)..    
-00013e00: 6173 796e 6320 6465 6620 7365 745f 6c69  async def set_li
-00013e10: 7665 7669 6577 2873 656c 662c 206c 6976  veview(self, liv
-00013e20: 6576 6965 773a 204c 6976 6576 6965 7729  eview: Liveview)
-00013e30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00013e40: 2020 2222 2253 6574 7320 7468 6520 6c69    """Sets the li
-00013e50: 7665 7669 6577 2063 7572 7265 6e74 2073  veview current s
-00013e60: 6574 2066 6f72 2074 6865 2076 6965 7765  et for the viewe
-00013e70: 720a 0a20 2020 2020 2020 2041 7267 733a  r..        Args:
-00013e80: 0a20 2020 2020 2020 202d 2d2d 2d0a 2020  .        ----.  
-00013e90: 2020 2020 2020 2020 2020 6c69 7665 7669            livevi
-00013ea0: 6577 3a20 5468 6520 6c69 7665 7669 6577  ew: The liveview
-00013eb0: 2079 6f75 2077 616e 7420 746f 2073 6574   you want to set
-00013ec0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00013ed0: 2020 2020 2020 6966 2073 656c 662e 5f61        if self._a
-00013ee0: 7069 2069 7320 6e6f 7420 4e6f 6e65 2061  pi is not None a
-00013ef0: 6e64 206c 6976 6576 6965 772e 6964 206e  nd liveview.id n
-00013f00: 6f74 2069 6e20 7365 6c66 2e5f 6170 692e  ot in self._api.
-00013f10: 626f 6f74 7374 7261 702e 6c69 7665 7669  bootstrap.livevi
-00013f20: 6577 733a 0a20 2020 2020 2020 2020 2020  ews:.           
-00013f30: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-00013f40: 7428 2255 6e6b 6e6f 776e 206c 6976 6576  t("Unknown livev
-00013f50: 6965 7722 290a 0a20 2020 2020 2020 2061  iew")..        a
-00013f60: 7379 6e63 2077 6974 6820 7365 6c66 2e5f  sync with self._
-00013f70: 7570 6461 7465 5f6c 6f63 6b3a 0a20 2020  update_lock:.   
-00013f80: 2020 2020 2020 2020 2061 7761 6974 2061           await a
-00013f90: 7379 6e63 696f 2e73 6c65 6570 280a 2020  syncio.sleep(.  
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00013fb0: 0a20 2020 2020 2020 2020 2020 2029 2020  .            )  
-00013fc0: 2320 7969 656c 6420 746f 2074 6865 2065  # yield to the e
-00013fd0: 7665 6e74 206c 6f6f 7020 6f6e 6365 2077  vent loop once w
-00013fe0: 6520 6861 7665 2074 6865 206c 6f63 6b20  e have the lock 
-00013ff0: 746f 2070 726f 6365 7373 2061 6e79 2070  to process any p
-00014000: 656e 6469 6e67 2075 7064 6174 6573 0a20  ending updates. 
-00014010: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00014020: 6265 666f 7265 5f63 6861 6e67 6573 203d  before_changes =
-00014030: 2073 656c 662e 6469 6374 5f77 6974 685f   self.dict_with_
-00014040: 6578 636c 7564 6573 2829 0a20 2020 2020  excludes().     
-00014050: 2020 2020 2020 2073 656c 662e 6c69 7665         self.live
-00014060: 7669 6577 5f69 6420 3d20 6c69 7665 7669  view_id = livevi
-00014070: 6577 2e69 640a 2020 2020 2020 2020 2020  ew.id.          
-00014080: 2020 2320 556e 6946 6920 5072 6f74 6563    # UniFi Protec
-00014090: 7420 6275 673a 2063 6861 6e67 696e 6720  t bug: changing 
-000140a0: 7468 6520 6c69 7665 7669 6577 2064 6f65  the liveview doe
-000140b0: 7320 5f6e 6f74 5f20 656d 6974 2061 2057  s _not_ emit a W
-000140c0: 5320 6d65 7373 6167 650a 2020 2020 2020  S message.      
-000140d0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-000140e0: 2e73 6176 655f 6465 7669 6365 2864 6174  .save_device(dat
-000140f0: 615f 6265 666f 7265 5f63 6861 6e67 6573  a_before_changes
-00014100: 2c20 666f 7263 655f 656d 6974 3d54 7275  , force_emit=Tru
-00014110: 6529 0a0a 0a63 6c61 7373 2042 7269 6467  e)...class Bridg
-00014120: 6528 5072 6f74 6563 7441 646f 7074 6162  e(ProtectAdoptab
-00014130: 6c65 4465 7669 6365 4d6f 6465 6c29 3a0a  leDeviceModel):.
-00014140: 2020 2020 706c 6174 666f 726d 3a20 7374      platform: st
-00014150: 720a 0a0a 636c 6173 7320 5365 6e73 6f72  r...class Sensor
-00014160: 5365 7474 696e 6773 4261 7365 2850 726f  SettingsBase(Pro
-00014170: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
-00014180: 0a20 2020 2069 735f 656e 6162 6c65 643a  .    is_enabled:
-00014190: 2062 6f6f 6c0a 0a0a 636c 6173 7320 5365   bool...class Se
-000141a0: 6e73 6f72 5468 7265 7368 6f6c 6453 6574  nsorThresholdSet
-000141b0: 7469 6e67 7328 5365 6e73 6f72 5365 7474  tings(SensorSett
-000141c0: 696e 6773 4261 7365 293a 0a20 2020 206d  ingsBase):.    m
-000141d0: 6172 6769 6e3a 2066 6c6f 6174 2020 2320  argin: float  # 
-000141e0: 7265 6164 206f 6e6c 790a 2020 2020 2320  read only.    # 
-000141f0: 2273 6166 6522 2074 6872 6573 686f 6c64  "safe" threshold
-00014200: 7320 666f 7220 616c 6572 7469 6e67 0a20  s for alerting. 
-00014210: 2020 2023 2061 6e79 7468 696e 6720 6265     # anything be
-00014220: 6c6f 772f 6162 6f76 6520 7769 6c6c 2074  low/above will t
-00014230: 7269 6767 6572 2061 6c65 7274 0a20 2020  rigger alert.   
-00014240: 206c 6f77 5f74 6872 6573 686f 6c64 3a20   low_threshold: 
-00014250: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0a  Optional[float].
-00014260: 2020 2020 6869 6768 5f74 6872 6573 686f      high_thresho
-00014270: 6c64 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ld: Optional[flo
-00014280: 6174 5d0a 0a0a 636c 6173 7320 5365 6e73  at]...class Sens
-00014290: 6f72 5365 6e73 6974 6976 6974 7953 6574  orSensitivitySet
-000142a0: 7469 6e67 7328 5365 6e73 6f72 5365 7474  tings(SensorSett
-000142b0: 696e 6773 4261 7365 293a 0a20 2020 2073  ingsBase):.    s
-000142c0: 656e 7369 7469 7669 7479 3a20 5065 7263  ensitivity: Perc
-000142d0: 656e 7449 6e74 0a0a 0a63 6c61 7373 2053  entInt...class S
-000142e0: 656e 736f 7242 6174 7465 7279 5374 6174  ensorBatteryStat
-000142f0: 7573 2850 726f 7465 6374 4261 7365 4f62  us(ProtectBaseOb
-00014300: 6a65 6374 293a 0a20 2020 2070 6572 6365  ject):.    perce
-00014310: 6e74 6167 653a 204f 7074 696f 6e61 6c5b  ntage: Optional[
-00014320: 5065 7263 656e 7449 6e74 5d0a 2020 2020  PercentInt].    
-00014330: 6973 5f6c 6f77 3a20 626f 6f6c 0a0a 0a63  is_low: bool...c
-00014340: 6c61 7373 2053 656e 736f 7253 7461 7428  lass SensorStat(
-00014350: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
-00014360: 7429 3a0a 2020 2020 7661 6c75 653a 204f  t):.    value: O
-00014370: 7074 696f 6e61 6c5b 666c 6f61 745d 0a20  ptional[float]. 
-00014380: 2020 2073 7461 7475 733a 2053 656e 736f     status: Senso
-00014390: 7253 7461 7475 7354 7970 650a 0a0a 636c  rStatusType...cl
-000143a0: 6173 7320 5365 6e73 6f72 5374 6174 7328  ass SensorStats(
-000143b0: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
-000143c0: 7429 3a0a 2020 2020 6c69 6768 743a 2053  t):.    light: S
-000143d0: 656e 736f 7253 7461 740a 2020 2020 6875  ensorStat.    hu
-000143e0: 6d69 6469 7479 3a20 5365 6e73 6f72 5374  midity: SensorSt
-000143f0: 6174 0a20 2020 2074 656d 7065 7261 7475  at.    temperatu
-00014400: 7265 3a20 5365 6e73 6f72 5374 6174 0a0a  re: SensorStat..
-00014410: 0a63 6c61 7373 2053 656e 736f 7228 5072  .class Sensor(Pr
-00014420: 6f74 6563 7441 646f 7074 6162 6c65 4465  otectAdoptableDe
-00014430: 7669 6365 4d6f 6465 6c29 3a0a 2020 2020  viceModel):.    
-00014440: 616c 6172 6d5f 7365 7474 696e 6773 3a20  alarm_settings: 
-00014450: 5365 6e73 6f72 5365 7474 696e 6773 4261  SensorSettingsBa
-00014460: 7365 0a20 2020 2061 6c61 726d 5f74 7269  se.    alarm_tri
-00014470: 6767 6572 6564 5f61 743a 204f 7074 696f  ggered_at: Optio
-00014480: 6e61 6c5b 6461 7465 7469 6d65 5d0a 2020  nal[datetime].  
-00014490: 2020 6261 7474 6572 795f 7374 6174 7573    battery_status
-000144a0: 3a20 5365 6e73 6f72 4261 7474 6572 7953  : SensorBatteryS
-000144b0: 7461 7475 730a 2020 2020 6361 6d65 7261  tatus.    camera
-000144c0: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
-000144d0: 725d 0a20 2020 2068 756d 6964 6974 795f  r].    humidity_
-000144e0: 7365 7474 696e 6773 3a20 5365 6e73 6f72  settings: Sensor
-000144f0: 5468 7265 7368 6f6c 6453 6574 7469 6e67  ThresholdSetting
-00014500: 730a 2020 2020 6973 5f6d 6f74 696f 6e5f  s.    is_motion_
-00014510: 6465 7465 6374 6564 3a20 626f 6f6c 0a20  detected: bool. 
-00014520: 2020 2069 735f 6f70 656e 6564 3a20 626f     is_opened: bo
-00014530: 6f6c 0a20 2020 206c 6561 6b5f 6465 7465  ol.    leak_dete
-00014540: 6374 6564 5f61 743a 204f 7074 696f 6e61  cted_at: Optiona
-00014550: 6c5b 6461 7465 7469 6d65 5d0a 2020 2020  l[datetime].    
-00014560: 6c65 645f 7365 7474 696e 6773 3a20 5365  led_settings: Se
-00014570: 6e73 6f72 5365 7474 696e 6773 4261 7365  nsorSettingsBase
-00014580: 0a20 2020 206c 6967 6874 5f73 6574 7469  .    light_setti
-00014590: 6e67 733a 2053 656e 736f 7254 6872 6573  ngs: SensorThres
-000145a0: 686f 6c64 5365 7474 696e 6773 0a20 2020  holdSettings.   
-000145b0: 206d 6f74 696f 6e5f 6465 7465 6374 6564   motion_detected
-000145c0: 5f61 743a 204f 7074 696f 6e61 6c5b 6461  _at: Optional[da
-000145d0: 7465 7469 6d65 5d0a 2020 2020 6d6f 7469  tetime].    moti
-000145e0: 6f6e 5f73 6574 7469 6e67 733a 2053 656e  on_settings: Sen
-000145f0: 736f 7253 656e 7369 7469 7669 7479 5365  sorSensitivitySe
-00014600: 7474 696e 6773 0a20 2020 206f 7065 6e5f  ttings.    open_
-00014610: 7374 6174 7573 5f63 6861 6e67 6564 5f61  status_changed_a
-00014620: 743a 204f 7074 696f 6e61 6c5b 6461 7465  t: Optional[date
-00014630: 7469 6d65 5d0a 2020 2020 7374 6174 733a  time].    stats:
-00014640: 2053 656e 736f 7253 7461 7473 0a20 2020   SensorStats.   
-00014650: 2074 616d 7065 7269 6e67 5f64 6574 6563   tampering_detec
-00014660: 7465 645f 6174 3a20 4f70 7469 6f6e 616c  ted_at: Optional
-00014670: 5b64 6174 6574 696d 655d 0a20 2020 2074  [datetime].    t
-00014680: 656d 7065 7261 7475 7265 5f73 6574 7469  emperature_setti
-00014690: 6e67 733a 2053 656e 736f 7254 6872 6573  ngs: SensorThres
-000146a0: 686f 6c64 5365 7474 696e 6773 0a20 2020  holdSettings.   
-000146b0: 206d 6f75 6e74 5f74 7970 653a 204d 6f75   mount_type: Mou
-000146c0: 6e74 5479 7065 0a0a 2020 2020 2320 6e6f  ntType..    # no
-000146d0: 7420 6469 7265 6374 6c79 2066 726f 6d20  t directly from 
-000146e0: 556e 6946 690a 2020 2020 6c61 7374 5f6d  UniFi.    last_m
-000146f0: 6f74 696f 6e5f 6576 656e 745f 6964 3a20  otion_event_id: 
-00014700: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00014710: 4e6f 6e65 0a20 2020 206c 6173 745f 636f  None.    last_co
-00014720: 6e74 6163 745f 6576 656e 745f 6964 3a20  ntact_event_id: 
-00014730: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00014740: 4e6f 6e65 0a20 2020 206c 6173 745f 7661  None.    last_va
-00014750: 6c75 655f 6576 656e 745f 6964 3a20 4f70  lue_event_id: Op
-00014760: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00014770: 6e65 0a20 2020 206c 6173 745f 616c 6172  ne.    last_alar
-00014780: 6d5f 6576 656e 745f 6964 3a20 4f70 7469  m_event_id: Opti
-00014790: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000147a0: 0a20 2020 2065 7874 7265 6d65 5f76 616c  .    extreme_val
-000147b0: 7565 5f64 6574 6563 7465 645f 6174 3a20  ue_detected_at: 
-000147c0: 4f70 7469 6f6e 616c 5b64 6174 6574 696d  Optional[datetim
-000147d0: 655d 203d 204e 6f6e 650a 2020 2020 5f74  e] = None.    _t
-000147e0: 616d 7065 725f 7469 6d65 6f75 743a 204f  amper_timeout: O
-000147f0: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
-00014800: 5d20 3d20 5072 6976 6174 6541 7474 7228  ] = PrivateAttr(
-00014810: 4e6f 6e65 290a 2020 2020 5f61 6c61 726d  None).    _alarm
-00014820: 5f74 696d 656f 7574 3a20 4f70 7469 6f6e  _timeout: Option
-00014830: 616c 5b64 6174 6574 696d 655d 203d 2050  al[datetime] = P
-00014840: 7269 7661 7465 4174 7472 284e 6f6e 6529  rivateAttr(None)
-00014850: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00014860: 6f64 0a20 2020 2040 6361 6368 650a 2020  od.    @cache.  
-00014870: 2020 6465 6620 5f67 6574 5f75 6e69 6669    def _get_unifi
-00014880: 5f72 656d 6170 7328 636c 7329 202d 3e20  _remaps(cls) -> 
-00014890: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
-000148a0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-000148b0: 2a2a 7375 7065 7228 292e 5f67 6574 5f75  **super()._get_u
-000148c0: 6e69 6669 5f72 656d 6170 7328 292c 2022  nifi_remaps(), "
-000148d0: 6361 6d65 7261 223a 2022 6361 6d65 7261  camera": "camera
-000148e0: 4964 227d 0a0a 2020 2020 4063 6c61 7373  Id"}..    @class
-000148f0: 6d65 7468 6f64 0a20 2020 2040 6361 6368  method.    @cach
-00014900: 650a 2020 2020 6465 6620 5f67 6574 5f72  e.    def _get_r
-00014910: 6561 645f 6f6e 6c79 5f66 6965 6c64 7328  ead_only_fields(
-00014920: 636c 7329 202d 3e20 7365 745b 7374 725d  cls) -> set[str]
-00014930: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00014940: 2073 7570 6572 2829 2e5f 6765 745f 7265   super()._get_re
-00014950: 6164 5f6f 6e6c 795f 6669 656c 6473 2829  ad_only_fields()
-00014960: 207c 207b 0a20 2020 2020 2020 2020 2020   | {.           
-00014970: 2022 6261 7474 6572 7953 7461 7475 7322   "batteryStatus"
-00014980: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
-00014990: 734d 6f74 696f 6e44 6574 6563 7465 6422  sMotionDetected"
-000149a0: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-000149b0: 6561 6b44 6574 6563 7465 6441 7422 2c0a  eakDetectedAt",.
-000149c0: 2020 2020 2020 2020 2020 2020 2274 616d              "tam
-000149d0: 7065 7269 6e67 4465 7465 6374 6564 4174  peringDetectedAt
-000149e0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000149f0: 6973 4f70 656e 6564 222c 0a20 2020 2020  isOpened",.     
-00014a00: 2020 2020 2020 2022 6f70 656e 5374 6174         "openStat
-00014a10: 7573 4368 616e 6765 6441 7422 2c0a 2020  usChangedAt",.  
-00014a20: 2020 2020 2020 2020 2020 2261 6c61 726d            "alarm
-00014a30: 5472 6967 6765 7265 6441 7422 2c0a 2020  TriggeredAt",.  
-00014a40: 2020 2020 2020 2020 2020 226d 6f74 696f            "motio
-00014a50: 6e44 6574 6563 7465 6441 7422 2c0a 2020  nDetectedAt",.  
-00014a60: 2020 2020 2020 2020 2020 2273 7461 7473            "stats
-00014a70: 222c 0a20 2020 2020 2020 207d 0a0a 2020  ",.        }..  
-00014a80: 2020 6465 6620 756e 6966 695f 6469 6374    def unifi_dict
-00014a90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00014aa0: 2020 2020 2020 2020 6461 7461 3a20 4f70          data: Op
-00014ab0: 7469 6f6e 616c 5b64 6963 745b 7374 722c  tional[dict[str,
-00014ac0: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
-00014ad0: 2020 2020 2020 2065 7863 6c75 6465 3a20         exclude: 
-00014ae0: 4f70 7469 6f6e 616c 5b73 6574 5b73 7472  Optional[set[str
-00014af0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
-00014b00: 202d 3e20 6469 6374 5b73 7472 2c20 416e   -> dict[str, An
-00014b10: 795d 3a0a 2020 2020 2020 2020 6461 7461  y]:.        data
-00014b20: 203d 2073 7570 6572 2829 2e75 6e69 6669   = super().unifi
-00014b30: 5f64 6963 7428 6461 7461 3d64 6174 612c  _dict(data=data,
-00014b40: 2065 7863 6c75 6465 3d65 7863 6c75 6465   exclude=exclude
-00014b50: 290a 0a20 2020 2020 2020 2069 6620 226c  )..        if "l
-00014b60: 6173 744d 6f74 696f 6e45 7665 6e74 4964  astMotionEventId
-00014b70: 2220 696e 2064 6174 613a 0a20 2020 2020  " in data:.     
-00014b80: 2020 2020 2020 2064 656c 2064 6174 615b         del data[
-00014b90: 226c 6173 744d 6f74 696f 6e45 7665 6e74  "lastMotionEvent
-00014ba0: 4964 225d 0a20 2020 2020 2020 2069 6620  Id"].        if 
-00014bb0: 226c 6173 7443 6f6e 7461 6374 4576 656e  "lastContactEven
-00014bc0: 7449 6422 2069 6e20 6461 7461 3a0a 2020  tId" in data:.  
-00014bd0: 2020 2020 2020 2020 2020 6465 6c20 6461            del da
-00014be0: 7461 5b22 6c61 7374 436f 6e74 6163 7445  ta["lastContactE
-00014bf0: 7665 6e74 4964 225d 0a20 2020 2020 2020  ventId"].       
-00014c00: 2069 6620 226c 6173 7456 616c 7565 4576   if "lastValueEv
-00014c10: 656e 7449 6422 2069 6e20 6461 7461 3a0a  entId" in data:.
-00014c20: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00014c30: 6461 7461 5b22 6c61 7374 5661 6c75 6545  data["lastValueE
-00014c40: 7665 6e74 4964 225d 0a20 2020 2020 2020  ventId"].       
-00014c50: 2069 6620 226c 6173 7441 6c61 726d 4576   if "lastAlarmEv
-00014c60: 656e 7449 6422 2069 6e20 6461 7461 3a0a  entId" in data:.
-00014c70: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00014c80: 6461 7461 5b22 6c61 7374 416c 6172 6d45  data["lastAlarmE
-00014c90: 7665 6e74 4964 225d 0a20 2020 2020 2020  ventId"].       
-00014ca0: 2069 6620 2265 7874 7265 6d65 5661 6c75   if "extremeValu
-00014cb0: 6544 6574 6563 7465 6441 7422 2069 6e20  eDetectedAt" in 
-00014cc0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00014cd0: 2020 6465 6c20 6461 7461 5b22 6578 7472    del data["extr
-00014ce0: 656d 6556 616c 7565 4465 7465 6374 6564  emeValueDetected
-00014cf0: 4174 225d 0a0a 2020 2020 2020 2020 7265  At"]..        re
-00014d00: 7475 726e 2064 6174 610a 0a20 2020 2040  turn data..    @
-00014d10: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00014d20: 2063 616d 6572 6128 7365 6c66 2920 2d3e   camera(self) ->
-00014d30: 204f 7074 696f 6e61 6c5b 4361 6d65 7261   Optional[Camera
-00014d40: 5d3a 0a20 2020 2020 2020 2022 2222 5061  ]:.        """Pa
-00014d50: 6972 6564 2043 616d 6572 6120 7769 6c6c  ired Camera will
-00014d60: 2061 6c77 6179 7320 6265 206e 6f6e 6520   always be none 
-00014d70: 6966 206e 6f20 6361 6d65 7261 2069 7320  if no camera is 
-00014d80: 7061 6972 6564 2222 220a 0a20 2020 2020  paired"""..     
-00014d90: 2020 2069 6620 7365 6c66 2e63 616d 6572     if self.camer
-00014da0: 615f 6964 2069 7320 4e6f 6e65 3a0a 2020  a_id is None:.  
-00014db0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014dc0: 204e 6f6e 650a 0a20 2020 2020 2020 2072   None..        r
-00014dd0: 6574 7572 6e20 7365 6c66 2e61 7069 2e62  eturn self.api.b
-00014de0: 6f6f 7473 7472 6170 2e63 616d 6572 6173  ootstrap.cameras
-00014df0: 5b73 656c 662e 6361 6d65 7261 5f69 645d  [self.camera_id]
-00014e00: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00014e10: 2020 2020 6465 6620 6973 5f74 616d 7065      def is_tampe
-00014e20: 7269 6e67 5f64 6574 6563 7465 6428 7365  ring_detected(se
-00014e30: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00014e40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014e50: 2e74 616d 7065 7269 6e67 5f64 6574 6563  .tampering_detec
-00014e60: 7465 645f 6174 2069 7320 6e6f 7420 4e6f  ted_at is not No
-00014e70: 6e65 0a0a 2020 2020 4070 726f 7065 7274  ne..    @propert
-00014e80: 790a 2020 2020 6465 6620 6973 5f61 6c61  y.    def is_ala
-00014e90: 726d 5f64 6574 6563 7465 6428 7365 6c66  rm_detected(self
-00014ea0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00014eb0: 2020 2069 6620 7365 6c66 2e5f 616c 6172     if self._alar
-00014ec0: 6d5f 7469 6d65 6f75 7420 6973 204e 6f6e  m_timeout is Non
-00014ed0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00014ee0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00014ef0: 2020 2020 7265 7475 726e 2075 7463 5f6e      return utc_n
-00014f00: 6f77 2829 203c 2073 656c 662e 5f61 6c61  ow() < self._ala
-00014f10: 726d 5f74 696d 656f 7574 0a0a 2020 2020  rm_timeout..    
-00014f20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00014f30: 6620 6973 5f63 6f6e 7461 6374 5f73 656e  f is_contact_sen
-00014f40: 736f 725f 656e 6162 6c65 6428 7365 6c66  sor_enabled(self
-00014f50: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00014f60: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
-00014f70: 6f75 6e74 5f74 7970 6520 696e 207b 4d6f  ount_type in {Mo
-00014f80: 756e 7454 7970 652e 444f 4f52 2c20 4d6f  untType.DOOR, Mo
-00014f90: 756e 7454 7970 652e 5749 4e44 4f57 2c20  untType.WINDOW, 
-00014fa0: 4d6f 756e 7454 7970 652e 4741 5241 4745  MountType.GARAGE
-00014fb0: 7d0a 0a20 2020 2040 7072 6f70 6572 7479  }..    @property
-00014fc0: 0a20 2020 2064 6566 2069 735f 6d6f 7469  .    def is_moti
-00014fd0: 6f6e 5f73 656e 736f 725f 656e 6162 6c65  on_sensor_enable
-00014fe0: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
-00014ff0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015000: 7365 6c66 2e6d 6f75 6e74 5f74 7970 6520  self.mount_type 
-00015010: 213d 204d 6f75 6e74 5479 7065 2e4c 4541  != MountType.LEA
-00015020: 4b20 616e 6420 7365 6c66 2e6d 6f74 696f  K and self.motio
-00015030: 6e5f 7365 7474 696e 6773 2e69 735f 656e  n_settings.is_en
-00015040: 6162 6c65 640a 0a20 2020 2040 7072 6f70  abled..    @prop
-00015050: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
-00015060: 616c 6172 6d5f 7365 6e73 6f72 5f65 6e61  alarm_sensor_ena
-00015070: 626c 6564 2873 656c 6629 202d 3e20 626f  bled(self) -> bo
-00015080: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-00015090: 726e 2073 656c 662e 6d6f 756e 745f 7479  rn self.mount_ty
-000150a0: 7065 2021 3d20 4d6f 756e 7454 7970 652e  pe != MountType.
-000150b0: 4c45 414b 2061 6e64 2073 656c 662e 616c  LEAK and self.al
-000150c0: 6172 6d5f 7365 7474 696e 6773 2e69 735f  arm_settings.is_
-000150d0: 656e 6162 6c65 640a 0a20 2020 2040 7072  enabled..    @pr
-000150e0: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
-000150f0: 735f 6c69 6768 745f 7365 6e73 6f72 5f65  s_light_sensor_e
-00015100: 6e61 626c 6564 2873 656c 6629 202d 3e20  nabled(self) -> 
-00015110: 626f 6f6c 3a0a 2020 2020 2020 2020 7265  bool:.        re
-00015120: 7475 726e 2073 656c 662e 6d6f 756e 745f  turn self.mount_
-00015130: 7479 7065 2021 3d20 4d6f 756e 7454 7970  type != MountTyp
-00015140: 652e 4c45 414b 2061 6e64 2073 656c 662e  e.LEAK and self.
-00015150: 6c69 6768 745f 7365 7474 696e 6773 2e69  light_settings.i
-00015160: 735f 656e 6162 6c65 640a 0a20 2020 2040  s_enabled..    @
-00015170: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00015180: 2069 735f 7465 6d70 6572 6174 7572 655f   is_temperature_
-00015190: 7365 6e73 6f72 5f65 6e61 626c 6564 2873  sensor_enabled(s
-000151a0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-000151b0: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
-000151c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000151d0: 6d6f 756e 745f 7479 7065 2021 3d20 4d6f  mount_type != Mo
-000151e0: 756e 7454 7970 652e 4c45 414b 2061 6e64  untType.LEAK and
-000151f0: 2073 656c 662e 7465 6d70 6572 6174 7572   self.temperatur
-00015200: 655f 7365 7474 696e 6773 2e69 735f 656e  e_settings.is_en
-00015210: 6162 6c65 640a 2020 2020 2020 2020 290a  abled.        ).
-00015220: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00015230: 2020 2064 6566 2069 735f 6875 6d69 6469     def is_humidi
-00015240: 7479 5f73 656e 736f 725f 656e 6162 6c65  ty_sensor_enable
-00015250: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
-00015260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015270: 7365 6c66 2e6d 6f75 6e74 5f74 7970 6520  self.mount_type 
-00015280: 213d 204d 6f75 6e74 5479 7065 2e4c 4541  != MountType.LEA
-00015290: 4b20 616e 6420 7365 6c66 2e68 756d 6964  K and self.humid
-000152a0: 6974 795f 7365 7474 696e 6773 2e69 735f  ity_settings.is_
-000152b0: 656e 6162 6c65 640a 0a20 2020 2040 7072  enabled..    @pr
-000152c0: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
-000152d0: 735f 6c65 616b 5f73 656e 736f 725f 656e  s_leak_sensor_en
-000152e0: 6162 6c65 6428 7365 6c66 2920 2d3e 2062  abled(self) -> b
-000152f0: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
-00015300: 7572 6e20 7365 6c66 2e6d 6f75 6e74 5f74  urn self.mount_t
-00015310: 7970 6520 6973 204d 6f75 6e74 5479 7065  ype is MountType
-00015320: 2e4c 4541 4b0a 0a20 2020 2064 6566 2073  .LEAK..    def s
-00015330: 6574 5f61 6c61 726d 5f74 696d 656f 7574  et_alarm_timeout
-00015340: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00015350: 2020 2020 2020 2020 7365 6c66 2e5f 616c          self._al
-00015360: 6172 6d5f 7469 6d65 6f75 7420 3d20 7574  arm_timeout = ut
-00015370: 635f 6e6f 7728 2920 2b20 4556 454e 545f  c_now() + EVENT_
-00015380: 5049 4e47 5f49 4e54 4552 5641 4c0a 2020  PING_INTERVAL.  
-00015390: 2020 2020 2020 7365 6c66 2e5f 6576 656e        self._even
-000153a0: 745f 6361 6c6c 6261 636b 5f70 696e 6728  t_callback_ping(
-000153b0: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-000153c0: 0a20 2020 2064 6566 206c 6173 745f 6d6f  .    def last_mo
-000153d0: 7469 6f6e 5f65 7665 6e74 2873 656c 6629  tion_event(self)
-000153e0: 202d 3e20 4f70 7469 6f6e 616c 5b45 7665   -> Optional[Eve
-000153f0: 6e74 5d3a 0a20 2020 2020 2020 2069 6620  nt]:.        if 
-00015400: 7365 6c66 2e6c 6173 745f 6d6f 7469 6f6e  self.last_motion
-00015410: 5f65 7665 6e74 5f69 6420 6973 204e 6f6e  _event_id is Non
-00015420: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00015430: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00015440: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00015450: 6170 692e 626f 6f74 7374 7261 702e 6576  api.bootstrap.ev
-00015460: 656e 7473 2e67 6574 2873 656c 662e 6c61  ents.get(self.la
-00015470: 7374 5f6d 6f74 696f 6e5f 6576 656e 745f  st_motion_event_
-00015480: 6964 290a 0a20 2020 2040 7072 6f70 6572  id)..    @proper
-00015490: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
-000154a0: 636f 6e74 6163 745f 6576 656e 7428 7365  contact_event(se
-000154b0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-000154c0: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
-000154d0: 6966 2073 656c 662e 6c61 7374 5f63 6f6e  if self.last_con
-000154e0: 7461 6374 5f65 7665 6e74 5f69 6420 6973  tact_event_id is
-000154f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00015500: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00015510: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00015520: 656c 662e 6170 692e 626f 6f74 7374 7261  elf.api.bootstra
-00015530: 702e 6576 656e 7473 2e67 6574 2873 656c  p.events.get(sel
-00015540: 662e 6c61 7374 5f63 6f6e 7461 6374 5f65  f.last_contact_e
-00015550: 7665 6e74 5f69 6429 0a0a 2020 2020 4070  vent_id)..    @p
-00015560: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00015570: 6c61 7374 5f76 616c 7565 5f65 7665 6e74  last_value_event
-00015580: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00015590: 616c 5b45 7665 6e74 5d3a 0a20 2020 2020  al[Event]:.     
-000155a0: 2020 2069 6620 7365 6c66 2e6c 6173 745f     if self.last_
-000155b0: 7661 6c75 655f 6576 656e 745f 6964 2069  value_event_id i
-000155c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000155d0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000155e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000155f0: 7365 6c66 2e61 7069 2e62 6f6f 7473 7472  self.api.bootstr
-00015600: 6170 2e65 7665 6e74 732e 6765 7428 7365  ap.events.get(se
-00015610: 6c66 2e6c 6173 745f 7661 6c75 655f 6576  lf.last_value_ev
-00015620: 656e 745f 6964 290a 0a20 2020 2040 7072  ent_id)..    @pr
-00015630: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
-00015640: 6173 745f 616c 6172 6d5f 6576 656e 7428  ast_alarm_event(
-00015650: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-00015660: 6c5b 4576 656e 745d 3a0a 2020 2020 2020  l[Event]:.      
-00015670: 2020 6966 2073 656c 662e 6c61 7374 5f61    if self.last_a
-00015680: 6c61 726d 5f65 7665 6e74 5f69 6420 6973  larm_event_id is
-00015690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000156a0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-000156b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000156c0: 656c 662e 6170 692e 626f 6f74 7374 7261  elf.api.bootstra
-000156d0: 702e 6576 656e 7473 2e67 6574 2873 656c  p.events.get(sel
-000156e0: 662e 6c61 7374 5f61 6c61 726d 5f65 7665  f.last_alarm_eve
-000156f0: 6e74 5f69 6429 0a0a 2020 2020 4070 726f  nt_id)..    @pro
-00015700: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
-00015710: 5f6c 6561 6b5f 6465 7465 6374 6564 2873  _leak_detected(s
-00015720: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-00015730: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00015740: 662e 6c65 616b 5f64 6574 6563 7465 645f  f.leak_detected_
-00015750: 6174 2069 7320 6e6f 7420 4e6f 6e65 0a0a  at is not None..
-00015760: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-00015770: 745f 7374 6174 7573 5f6c 6967 6874 2873  t_status_light(s
-00015780: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
-00015790: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-000157a0: 2020 2020 2022 2222 5365 7473 2074 6865       """Sets the
-000157b0: 2073 7461 7475 7320 696e 6469 6361 746f   status indicato
-000157c0: 7220 6c69 6768 7420 666f 7220 7468 6520  r light for the 
-000157d0: 7365 6e73 6f72 2222 220a 0a20 2020 2020  sensor"""..     
-000157e0: 2020 2064 6566 2063 616c 6c62 6163 6b28     def callback(
-000157f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00015800: 2020 2020 2020 2073 656c 662e 6c65 645f         self.led_
-00015810: 7365 7474 696e 6773 2e69 735f 656e 6162  settings.is_enab
-00015820: 6c65 6420 3d20 656e 6162 6c65 640a 0a20  led = enabled.. 
-00015830: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
-00015840: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
-00015850: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
-00015860: 796e 6320 6465 6620 7365 745f 6d6f 756e  ync def set_moun
-00015870: 745f 7479 7065 2873 656c 662c 206d 6f75  t_type(self, mou
-00015880: 6e74 5f74 7970 653a 204d 6f75 6e74 5479  nt_type: MountTy
-00015890: 7065 2920 2d3e 204e 6f6e 653a 0a20 2020  pe) -> None:.   
-000158a0: 2020 2020 2022 2222 5365 7473 2063 7572       """Sets cur
-000158b0: 7265 6e74 206d 6f75 6e74 2074 7970 6520  rent mount type 
-000158c0: 666f 7220 7365 6e73 6f72 2222 220a 0a20  for sensor""".. 
-000158d0: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
-000158e0: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
-000158f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015900: 6d6f 756e 745f 7479 7065 203d 206d 6f75  mount_type = mou
-00015910: 6e74 5f74 7970 650a 0a20 2020 2020 2020  nt_type..       
-00015920: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
-00015930: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
-00015940: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
-00015950: 6620 7365 745f 6d6f 7469 6f6e 5f73 7461  f set_motion_sta
-00015960: 7475 7328 7365 6c66 2c20 656e 6162 6c65  tus(self, enable
-00015970: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-00015980: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-00015990: 7320 7468 6520 6d6f 7469 6f6e 2064 6574  s the motion det
-000159a0: 6563 7469 6f6e 2074 7970 6520 666f 7220  ection type for 
-000159b0: 7468 6520 7365 6e73 6f72 2222 220a 0a20  the sensor""".. 
-000159c0: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
-000159d0: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
-000159e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000159f0: 6d6f 7469 6f6e 5f73 6574 7469 6e67 732e  motion_settings.
-00015a00: 6973 5f65 6e61 626c 6564 203d 2065 6e61  is_enabled = ena
-00015a10: 626c 6564 0a0a 2020 2020 2020 2020 6177  bled..        aw
-00015a20: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
-00015a30: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
-00015a40: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00015a50: 6574 5f6d 6f74 696f 6e5f 7365 6e73 6974  et_motion_sensit
-00015a60: 6976 6974 7928 7365 6c66 2c20 7365 6e73  ivity(self, sens
-00015a70: 6974 6976 6974 793a 2069 6e74 2920 2d3e  itivity: int) ->
-00015a80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00015a90: 2222 5365 7473 2074 6865 206d 6f74 696f  ""Sets the motio
-00015aa0: 6e20 7365 6e73 6974 6976 6974 7920 666f  n sensitivity fo
-00015ab0: 7220 7468 6520 7365 6e73 6f72 2222 220a  r the sensor""".
-00015ac0: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
-00015ad0: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
-00015ae0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015af0: 662e 6d6f 7469 6f6e 5f73 6574 7469 6e67  f.motion_setting
-00015b00: 732e 7365 6e73 6974 6976 6974 7920 3d20  s.sensitivity = 
-00015b10: 5065 7263 656e 7449 6e74 2873 656e 7369  PercentInt(sensi
-00015b20: 7469 7669 7479 290a 0a20 2020 2020 2020  tivity)..       
-00015b30: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
-00015b40: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
-00015b50: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
-00015b60: 6620 7365 745f 7465 6d70 6572 6174 7572  f set_temperatur
-00015b70: 655f 7374 6174 7573 2873 656c 662c 2065  e_status(self, e
-00015b80: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
-00015b90: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00015ba0: 2222 5365 7473 2074 6865 2074 656d 7065  ""Sets the tempe
-00015bb0: 7261 7475 7265 2064 6574 6563 7469 6f6e  rature detection
-00015bc0: 2074 7970 6520 666f 7220 7468 6520 7365   type for the se
-00015bd0: 6e73 6f72 2222 220a 0a20 2020 2020 2020  nsor"""..       
-00015be0: 2064 6566 2063 616c 6c62 6163 6b28 2920   def callback() 
-00015bf0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015c00: 2020 2020 2073 656c 662e 7465 6d70 6572       self.temper
-00015c10: 6174 7572 655f 7365 7474 696e 6773 2e69  ature_settings.i
-00015c20: 735f 656e 6162 6c65 6420 3d20 656e 6162  s_enabled = enab
-00015c30: 6c65 640a 0a20 2020 2020 2020 2061 7761  led..        awa
-00015c40: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-00015c50: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-00015c60: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
-00015c70: 745f 7465 6d70 6572 6174 7572 655f 7361  t_temperature_sa
-00015c80: 6665 5f72 616e 6765 2873 656c 662c 206c  fe_range(self, l
-00015c90: 6f77 3a20 666c 6f61 742c 2068 6967 683a  ow: float, high:
-00015ca0: 2066 6c6f 6174 2920 2d3e 204e 6f6e 653a   float) -> None:
-00015cb0: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
-00015cc0: 2074 6865 2074 656d 7065 7261 7475 7265   the temperature
-00015cd0: 2073 6166 6520 7261 6e67 6520 666f 7220   safe range for 
-00015ce0: 7468 6520 7365 6e73 6f72 2222 220a 0a20  the sensor""".. 
-00015cf0: 2020 2020 2020 2069 6620 6c6f 7720 3c20         if low < 
-00015d00: 302e 303a 0a20 2020 2020 2020 2020 2020  0.0:.           
-00015d10: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-00015d20: 7428 224d 696e 696d 756d 2076 616c 7565  t("Minimum value
-00015d30: 2069 7320 30c2 b043 2229 0a20 2020 2020   is 0..C").     
-00015d40: 2020 2069 6620 6869 6768 203e 2034 352e     if high > 45.
-00015d50: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00015d60: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
-00015d70: 224d 6178 696d 756d 2076 616c 7565 2069  "Maximum value i
-00015d80: 7320 3435 c2b0 4322 290a 2020 2020 2020  s 45..C").      
-00015d90: 2020 6966 2068 6967 6820 3c3d 206c 6f77    if high <= low
-00015da0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00015db0: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00015dc0: 4869 6768 2076 616c 7565 206d 7573 7420  High value must 
-00015dd0: 6265 2061 626f 7665 206c 6f77 2076 616c  be above low val
-00015de0: 7565 2229 0a0a 2020 2020 2020 2020 6465  ue")..        de
-00015df0: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
-00015e00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00015e10: 2020 7365 6c66 2e74 656d 7065 7261 7475    self.temperatu
-00015e20: 7265 5f73 6574 7469 6e67 732e 6c6f 775f  re_settings.low_
-00015e30: 7468 7265 7368 6f6c 6420 3d20 6c6f 770a  threshold = low.
-00015e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015e50: 2e74 656d 7065 7261 7475 7265 5f73 6574  .temperature_set
-00015e60: 7469 6e67 732e 6869 6768 5f74 6872 6573  tings.high_thres
-00015e70: 686f 6c64 203d 2068 6967 680a 0a20 2020  hold = high..   
-00015e80: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-00015e90: 7175 6575 655f 7570 6461 7465 2863 616c  queue_update(cal
-00015ea0: 6c62 6163 6b29 0a0a 2020 2020 6173 796e  lback)..    asyn
-00015eb0: 6320 6465 6620 7265 6d6f 7665 5f74 656d  c def remove_tem
-00015ec0: 7065 7261 7475 7265 5f73 6166 655f 7261  perature_safe_ra
-00015ed0: 6e67 6528 7365 6c66 2920 2d3e 204e 6f6e  nge(self) -> Non
-00015ee0: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
-00015ef0: 6d6f 7665 7320 7468 6520 7465 6d70 6572  moves the temper
-00015f00: 6174 7572 6520 7361 6665 2072 616e 6765  ature safe range
-00015f10: 2066 6f72 2074 6865 2073 656e 736f 7222   for the sensor"
-00015f20: 2222 0a0a 2020 2020 2020 2020 6465 6620  ""..        def 
-00015f30: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
-00015f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00015f50: 7365 6c66 2e74 656d 7065 7261 7475 7265  self.temperature
-00015f60: 5f73 6574 7469 6e67 732e 6c6f 775f 7468  _settings.low_th
-00015f70: 7265 7368 6f6c 6420 3d20 4e6f 6e65 0a20  reshold = None. 
-00015f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015f90: 7465 6d70 6572 6174 7572 655f 7365 7474  temperature_sett
-00015fa0: 696e 6773 2e68 6967 685f 7468 7265 7368  ings.high_thresh
-00015fb0: 6f6c 6420 3d20 4e6f 6e65 0a0a 2020 2020  old = None..    
-00015fc0: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00015fd0: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00015fe0: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-00015ff0: 2064 6566 2073 6574 5f68 756d 6964 6974   def set_humidit
-00016000: 795f 7374 6174 7573 2873 656c 662c 2065  y_status(self, e
-00016010: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
-00016020: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00016030: 2222 5365 7473 2074 6865 2068 756d 6964  ""Sets the humid
-00016040: 6974 7920 6465 7465 6374 696f 6e20 7479  ity detection ty
-00016050: 7065 2066 6f72 2074 6865 2073 656e 736f  pe for the senso
-00016060: 7222 2222 0a0a 2020 2020 2020 2020 6465  r"""..        de
-00016070: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
-00016080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016090: 2020 7365 6c66 2e68 756d 6964 6974 795f    self.humidity_
-000160a0: 7365 7474 696e 6773 2e69 735f 656e 6162  settings.is_enab
-000160b0: 6c65 6420 3d20 656e 6162 6c65 640a 0a20  led = enabled.. 
-000160c0: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
-000160d0: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
-000160e0: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
-000160f0: 796e 6320 6465 6620 7365 745f 6875 6d69  ync def set_humi
-00016100: 6469 7479 5f73 6166 655f 7261 6e67 6528  dity_safe_range(
-00016110: 7365 6c66 2c20 6c6f 773a 2066 6c6f 6174  self, low: float
-00016120: 2c20 6869 6768 3a20 666c 6f61 7429 202d  , high: float) -
-00016130: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00016140: 2222 2253 6574 7320 7468 6520 6875 6d69  """Sets the humi
-00016150: 6469 7479 2073 6166 6520 7261 6e67 6520  dity safe range 
-00016160: 666f 7220 7468 6520 7365 6e73 6f72 2222  for the sensor""
-00016170: 220a 0a20 2020 2020 2020 2069 6620 6c6f  "..        if lo
-00016180: 7720 3c20 312e 303a 0a20 2020 2020 2020  w < 1.0:.       
-00016190: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-000161a0: 7175 6573 7428 224d 696e 696d 756d 2076  quest("Minimum v
-000161b0: 616c 7565 2069 7320 3125 2229 0a20 2020  alue is 1%").   
-000161c0: 2020 2020 2069 6620 6869 6768 203e 2039       if high > 9
-000161d0: 392e 303a 0a20 2020 2020 2020 2020 2020  9.0:.           
-000161e0: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
-000161f0: 7428 224d 6178 696d 756d 2076 616c 7565  t("Maximum value
-00016200: 2069 7320 3939 2522 290a 2020 2020 2020   is 99%").      
-00016210: 2020 6966 2068 6967 6820 3c3d 206c 6f77    if high <= low
-00016220: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00016230: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
-00016240: 4869 6768 2076 616c 7565 206d 7573 7420  High value must 
-00016250: 6265 2061 626f 7665 206c 6f77 2076 616c  be above low val
-00016260: 7565 2229 0a0a 2020 2020 2020 2020 6465  ue")..        de
-00016270: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
-00016280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016290: 2020 7365 6c66 2e68 756d 6964 6974 795f    self.humidity_
-000162a0: 7365 7474 696e 6773 2e6c 6f77 5f74 6872  settings.low_thr
-000162b0: 6573 686f 6c64 203d 206c 6f77 0a20 2020  eshold = low.   
-000162c0: 2020 2020 2020 2020 2073 656c 662e 6875           self.hu
-000162d0: 6d69 6469 7479 5f73 6574 7469 6e67 732e  midity_settings.
-000162e0: 6869 6768 5f74 6872 6573 686f 6c64 203d  high_threshold =
-000162f0: 2068 6967 680a 0a20 2020 2020 2020 2061   high..        a
-00016300: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
-00016310: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
-00016320: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00016330: 7265 6d6f 7665 5f68 756d 6964 6974 795f  remove_humidity_
-00016340: 7361 6665 5f72 616e 6765 2873 656c 6629  safe_range(self)
-00016350: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00016360: 2020 2222 2252 656d 6f76 6573 2074 6865    """Removes the
-00016370: 2068 756d 6964 6974 7920 7361 6665 2072   humidity safe r
-00016380: 616e 6765 2066 6f72 2074 6865 2073 656e  ange for the sen
-00016390: 736f 7222 2222 0a0a 2020 2020 2020 2020  sor"""..        
-000163a0: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
-000163b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000163c0: 2020 2020 7365 6c66 2e68 756d 6964 6974      self.humidit
-000163d0: 795f 7365 7474 696e 6773 2e6c 6f77 5f74  y_settings.low_t
-000163e0: 6872 6573 686f 6c64 203d 204e 6f6e 650a  hreshold = None.
-000163f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016400: 2e68 756d 6964 6974 795f 7365 7474 696e  .humidity_settin
-00016410: 6773 2e68 6967 685f 7468 7265 7368 6f6c  gs.high_threshol
-00016420: 6420 3d20 4e6f 6e65 0a0a 2020 2020 2020  d = None..      
-00016430: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
-00016440: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
-00016450: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
-00016460: 6566 2073 6574 5f6c 6967 6874 5f73 7461  ef set_light_sta
-00016470: 7475 7328 7365 6c66 2c20 656e 6162 6c65  tus(self, enable
-00016480: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-00016490: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-000164a0: 7320 7468 6520 6c69 6768 7420 6465 7465  s the light dete
-000164b0: 6374 696f 6e20 7479 7065 2066 6f72 2074  ction type for t
-000164c0: 6865 2073 656e 736f 7222 2222 0a0a 2020  he sensor"""..  
-000164d0: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
-000164e0: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
-000164f0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00016500: 6967 6874 5f73 6574 7469 6e67 732e 6973  ight_settings.is
-00016510: 5f65 6e61 626c 6564 203d 2065 6e61 626c  _enabled = enabl
-00016520: 6564 0a0a 2020 2020 2020 2020 6177 6169  ed..        awai
-00016530: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
-00016540: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
-00016550: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
-00016560: 5f6c 6967 6874 5f73 6166 655f 7261 6e67  _light_safe_rang
-00016570: 6528 7365 6c66 2c20 6c6f 773a 2066 6c6f  e(self, low: flo
-00016580: 6174 2c20 6869 6768 3a20 666c 6f61 7429  at, high: float)
-00016590: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000165a0: 2020 2222 2253 6574 7320 7468 6520 6c69    """Sets the li
-000165b0: 6768 7420 7361 6665 2072 616e 6765 2066  ght safe range f
-000165c0: 6f72 2074 6865 2073 656e 736f 7222 2222  or the sensor"""
-000165d0: 0a0a 2020 2020 2020 2020 6966 206c 6f77  ..        if low
-000165e0: 203c 2031 2e30 3a0a 2020 2020 2020 2020   < 1.0:.        
-000165f0: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
-00016600: 7565 7374 2822 4d69 6e69 6d75 6d20 7661  uest("Minimum va
-00016610: 6c75 6520 6973 2031 206c 7578 2229 0a20  lue is 1 lux"). 
-00016620: 2020 2020 2020 2069 6620 6869 6768 203e         if high >
-00016630: 2031 3030 302e 303a 0a20 2020 2020 2020   1000.0:.       
-00016640: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
-00016650: 7175 6573 7428 224d 6178 696d 756d 2076  quest("Maximum v
-00016660: 616c 7565 2069 7320 3130 3030 206c 7578  alue is 1000 lux
-00016670: 2229 0a20 2020 2020 2020 2069 6620 6869  ").        if hi
-00016680: 6768 203c 3d20 6c6f 773a 0a20 2020 2020  gh <= low:.     
-00016690: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
-000166a0: 5265 7175 6573 7428 2248 6967 6820 7661  Request("High va
-000166b0: 6c75 6520 6d75 7374 2062 6520 6162 6f76  lue must be abov
-000166c0: 6520 6c6f 7720 7661 6c75 6522 290a 0a20  e low value").. 
-000166d0: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
-000166e0: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
-000166f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016700: 6c69 6768 745f 7365 7474 696e 6773 2e6c  light_settings.l
-00016710: 6f77 5f74 6872 6573 686f 6c64 203d 206c  ow_threshold = l
-00016720: 6f77 0a20 2020 2020 2020 2020 2020 2073  ow.            s
-00016730: 656c 662e 6c69 6768 745f 7365 7474 696e  elf.light_settin
-00016740: 6773 2e68 6967 685f 7468 7265 7368 6f6c  gs.high_threshol
-00016750: 6420 3d20 6869 6768 0a0a 2020 2020 2020  d = high..      
-00016760: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
-00016770: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
-00016780: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
-00016790: 6566 2072 656d 6f76 655f 6c69 6768 745f  ef remove_light_
-000167a0: 7361 6665 5f72 616e 6765 2873 656c 6629  safe_range(self)
-000167b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000167c0: 2020 2222 2252 656d 6f76 6573 2074 6865    """Removes the
-000167d0: 206c 6967 6874 2073 6166 6520 7261 6e67   light safe rang
-000167e0: 6520 666f 7220 7468 6520 7365 6e73 6f72  e for the sensor
-000167f0: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
-00016800: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
-00016810: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016820: 2073 656c 662e 6c69 6768 745f 7365 7474   self.light_sett
-00016830: 696e 6773 2e6c 6f77 5f74 6872 6573 686f  ings.low_thresho
-00016840: 6c64 203d 204e 6f6e 650a 2020 2020 2020  ld = None.      
-00016850: 2020 2020 2020 7365 6c66 2e6c 6967 6874        self.light
-00016860: 5f73 6574 7469 6e67 732e 6869 6768 5f74  _settings.high_t
-00016870: 6872 6573 686f 6c64 203d 204e 6f6e 650a  hreshold = None.
-00016880: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
-00016890: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
-000168a0: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
-000168b0: 6173 796e 6320 6465 6620 7365 745f 616c  async def set_al
-000168c0: 6172 6d5f 7374 6174 7573 2873 656c 662c  arm_status(self,
-000168d0: 2065 6e61 626c 6564 3a20 626f 6f6c 2920   enabled: bool) 
-000168e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000168f0: 2022 2222 5365 7473 2074 6865 2061 6c61   """Sets the ala
-00016900: 726d 2064 6574 6563 7469 6f6e 2074 7970  rm detection typ
-00016910: 6520 666f 7220 7468 6520 7365 6e73 6f72  e for the sensor
-00016920: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
-00016930: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
-00016940: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016950: 2073 656c 662e 616c 6172 6d5f 7365 7474   self.alarm_sett
-00016960: 696e 6773 2e69 735f 656e 6162 6c65 6420  ings.is_enabled 
-00016970: 3d20 656e 6162 6c65 640a 0a20 2020 2020  = enabled..     
-00016980: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
-00016990: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
-000169a0: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
-000169b0: 6465 6620 7365 745f 7061 6972 6564 5f63  def set_paired_c
-000169c0: 616d 6572 6128 7365 6c66 2c20 6361 6d65  amera(self, came
-000169d0: 7261 3a20 4f70 7469 6f6e 616c 5b43 616d  ra: Optional[Cam
-000169e0: 6572 615d 2920 2d3e 204e 6f6e 653a 0a20  era]) -> None:. 
-000169f0: 2020 2020 2020 2022 2222 5365 7473 2074         """Sets t
-00016a00: 6865 2063 616d 6572 6120 7061 6972 6564  he camera paired
-00016a10: 2077 6974 6820 7468 6520 7365 6e73 6f72   with the sensor
-00016a20: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
-00016a30: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
-00016a40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016a50: 2069 6620 6361 6d65 7261 2069 7320 4e6f   if camera is No
-00016a60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00016a70: 2020 2020 7365 6c66 2e63 616d 6572 615f      self.camera_
-00016a80: 6964 203d 204e 6f6e 650a 2020 2020 2020  id = None.      
-00016a90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00016aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016ab0: 2e63 616d 6572 615f 6964 203d 2063 616d  .camera_id = cam
-00016ac0: 6572 612e 6964 0a0a 2020 2020 2020 2020  era.id..        
-00016ad0: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
-00016ae0: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
-00016af0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00016b00: 2063 6c65 6172 5f74 616d 7065 7228 7365   clear_tamper(se
-00016b10: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00016b20: 2020 2020 2022 2222 436c 6561 7273 2074       """Clears t
-00016b30: 616d 7065 7220 7374 6174 7573 2066 6f72  amper status for
-00016b40: 2073 656e 736f 7222 2222 0a0a 2020 2020   sensor"""..    
-00016b50: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00016b60: 6170 692e 626f 6f74 7374 7261 702e 6175  api.bootstrap.au
-00016b70: 7468 5f75 7365 722e 6361 6e28 0a20 2020  th_user.can(.   
-00016b80: 2020 2020 2020 2020 204d 6f64 656c 5479           ModelTy
-00016b90: 7065 2e53 454e 534f 522c 0a20 2020 2020  pe.SENSOR,.     
-00016ba0: 2020 2020 2020 2050 6572 6d69 7373 696f         Permissio
-00016bb0: 6e4e 6f64 652e 5752 4954 452c 0a20 2020  nNode.WRITE,.   
-00016bc0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00016bd0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00016be0: 2020 2020 2020 7261 6973 6520 4e6f 7441        raise NotA
-00016bf0: 7574 686f 7269 7a65 6428 0a20 2020 2020  uthorized(.     
-00016c00: 2020 2020 2020 2020 2020 2066 2244 6f20             f"Do 
-00016c10: 6e6f 7420 6861 7665 2070 6572 6d69 7373  not have permiss
-00016c20: 696f 6e20 746f 2063 6c65 6172 2074 616d  ion to clear tam
-00016c30: 7065 7220 666f 7220 7365 6e73 6f72 3a20  per for sensor: 
-00016c40: 7b73 656c 662e 6964 7d22 2c0a 2020 2020  {self.id}",.    
-00016c50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016c60: 2020 6177 6169 7420 7365 6c66 2e61 7069    await self.api
-00016c70: 2e63 6c65 6172 5f74 616d 7065 725f 7365  .clear_tamper_se
-00016c80: 6e73 6f72 2873 656c 662e 6964 290a 0a0a  nsor(self.id)...
-00016c90: 636c 6173 7320 446f 6f72 6c6f 636b 2850  class Doorlock(P
-00016ca0: 726f 7465 6374 4164 6f70 7461 626c 6544  rotectAdoptableD
-00016cb0: 6576 6963 654d 6f64 656c 293a 0a20 2020  eviceModel):.   
-00016cc0: 2063 7265 6465 6e74 6961 6c73 3a20 4f70   credentials: Op
-00016cd0: 7469 6f6e 616c 5b73 7472 5d0a 2020 2020  tional[str].    
-00016ce0: 6c6f 636b 5f73 7461 7475 733a 204c 6f63  lock_status: Loc
-00016cf0: 6b53 7461 7475 7354 7970 650a 2020 2020  kStatusType.    
-00016d00: 656e 6162 6c65 5f68 6f6d 656b 6974 3a20  enable_homekit: 
-00016d10: 626f 6f6c 0a20 2020 2061 7574 6f5f 636c  bool.    auto_cl
-00016d20: 6f73 655f 7469 6d65 3a20 7469 6d65 6465  ose_time: timede
-00016d30: 6c74 610a 2020 2020 6c65 645f 7365 7474  lta.    led_sett
-00016d40: 696e 6773 3a20 5365 6e73 6f72 5365 7474  ings: SensorSett
-00016d50: 696e 6773 4261 7365 0a20 2020 2062 6174  ingsBase.    bat
-00016d60: 7465 7279 5f73 7461 7475 733a 2053 656e  tery_status: Sen
-00016d70: 736f 7242 6174 7465 7279 5374 6174 7573  sorBatteryStatus
-00016d80: 0a20 2020 2063 616d 6572 615f 6964 3a20  .    camera_id: 
-00016d90: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00016da0: 2020 6861 735f 686f 6d65 6b69 743a 2062    has_homekit: b
-00016db0: 6f6f 6c0a 2020 2020 7072 6976 6174 655f  ool.    private_
-00016dc0: 746f 6b65 6e3a 2073 7472 0a0a 2020 2020  token: str..    
-00016dd0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00016de0: 2040 6361 6368 650a 2020 2020 6465 6620   @cache.    def 
-00016df0: 5f67 6574 5f75 6e69 6669 5f72 656d 6170  _get_unifi_remap
-00016e00: 7328 636c 7329 202d 3e20 6469 6374 5b73  s(cls) -> dict[s
-00016e10: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
-00016e20: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-00016e30: 2020 2020 2020 202a 2a73 7570 6572 2829         **super()
-00016e40: 2e5f 6765 745f 756e 6966 695f 7265 6d61  ._get_unifi_rema
-00016e50: 7073 2829 2c0a 2020 2020 2020 2020 2020  ps(),.          
-00016e60: 2020 2263 616d 6572 6122 3a20 2263 616d    "camera": "cam
-00016e70: 6572 6149 6422 2c0a 2020 2020 2020 2020  eraId",.        
-00016e80: 2020 2020 2261 7574 6f43 6c6f 7365 5469      "autoCloseTi
-00016e90: 6d65 4d73 223a 2022 6175 746f 436c 6f73  meMs": "autoClos
-00016ea0: 6554 696d 6522 2c0a 2020 2020 2020 2020  eTime",.        
-00016eb0: 7d0a 0a20 2020 2040 636c 6173 736d 6574  }..    @classmet
-00016ec0: 686f 640a 2020 2020 4063 6163 6865 0a20  hod.    @cache. 
-00016ed0: 2020 2064 6566 205f 6765 745f 7265 6164     def _get_read
-00016ee0: 5f6f 6e6c 795f 6669 656c 6473 2863 6c73  _only_fields(cls
-00016ef0: 2920 2d3e 2073 6574 5b73 7472 5d3a 0a20  ) -> set[str]:. 
-00016f00: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00016f10: 7065 7228 292e 5f67 6574 5f72 6561 645f  per()._get_read_
-00016f20: 6f6e 6c79 5f66 6965 6c64 7328 2920 7c20  only_fields() | 
-00016f30: 7b0a 2020 2020 2020 2020 2020 2020 2263  {.            "c
-00016f40: 7265 6465 6e74 6961 6c73 222c 0a20 2020  redentials",.   
-00016f50: 2020 2020 2020 2020 2022 6c6f 636b 5374           "lockSt
-00016f60: 6174 7573 222c 0a20 2020 2020 2020 2020  atus",.         
-00016f70: 2020 2022 6261 7474 6572 7953 7461 7475     "batteryStatu
-00016f80: 7322 2c0a 2020 2020 2020 2020 7d0a 0a20  s",.        }.. 
-00016f90: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00016fa0: 2020 2020 6465 6620 756e 6966 695f 6469      def unifi_di
-00016fb0: 6374 5f74 6f5f 6469 6374 2863 6c73 2c20  ct_to_dict(cls, 
-00016fc0: 6461 7461 3a20 6469 6374 5b73 7472 2c20  data: dict[str, 
-00016fd0: 416e 795d 2920 2d3e 2064 6963 745b 7374  Any]) -> dict[st
-00016fe0: 722c 2041 6e79 5d3a 0a20 2020 2020 2020  r, Any]:.       
-00016ff0: 2069 6620 2261 7574 6f43 6c6f 7365 5469   if "autoCloseTi
-00017000: 6d65 4d73 2220 696e 2064 6174 6120 616e  meMs" in data an
-00017010: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
-00017020: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-00017030: 7461 5b22 6175 746f 436c 6f73 6554 696d  ta["autoCloseTim
-00017040: 654d 7322 5d2c 0a20 2020 2020 2020 2020  eMs"],.         
-00017050: 2020 2074 696d 6564 656c 7461 2c0a 2020     timedelta,.  
-00017060: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00017070: 2020 2020 2064 6174 615b 2261 7574 6f43       data["autoC
-00017080: 6c6f 7365 5469 6d65 4d73 225d 203d 2074  loseTimeMs"] = t
-00017090: 696d 6564 656c 7461 286d 696c 6c69 7365  imedelta(millise
-000170a0: 636f 6e64 733d 6461 7461 5b22 6175 746f  conds=data["auto
-000170b0: 436c 6f73 6554 696d 654d 7322 5d29 0a0a  CloseTimeMs"])..
-000170c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000170d0: 7570 6572 2829 2e75 6e69 6669 5f64 6963  uper().unifi_dic
-000170e0: 745f 746f 5f64 6963 7428 6461 7461 290a  t_to_dict(data).
-000170f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00017100: 2020 2064 6566 2063 616d 6572 6128 7365     def camera(se
-00017110: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-00017120: 4361 6d65 7261 5d3a 0a20 2020 2020 2020  Camera]:.       
-00017130: 2022 2222 5061 6972 6564 2043 616d 6572   """Paired Camer
-00017140: 6120 7769 6c6c 2061 6c77 6179 7320 6265  a will always be
-00017150: 206e 6f6e 6520 6966 206e 6f20 6361 6d65   none if no came
-00017160: 7261 2069 7320 7061 6972 6564 2222 220a  ra is paired""".
-00017170: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00017180: 2e63 616d 6572 615f 6964 2069 7320 4e6f  .camera_id is No
-00017190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000171a0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-000171b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000171c0: 2e61 7069 2e62 6f6f 7473 7472 6170 2e63  .api.bootstrap.c
-000171d0: 616d 6572 6173 5b73 656c 662e 6361 6d65  ameras[self.came
-000171e0: 7261 5f69 645d 0a0a 2020 2020 6173 796e  ra_id]..    asyn
-000171f0: 6320 6465 6620 7365 745f 7061 6972 6564  c def set_paired
-00017200: 5f63 616d 6572 6128 7365 6c66 2c20 6361  _camera(self, ca
-00017210: 6d65 7261 3a20 4f70 7469 6f6e 616c 5b43  mera: Optional[C
-00017220: 616d 6572 615d 2920 2d3e 204e 6f6e 653a  amera]) -> None:
-00017230: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
-00017240: 2074 6865 2063 616d 6572 6120 7061 6972   the camera pair
-00017250: 6564 2077 6974 6820 7468 6520 7365 6e73  ed with the sens
-00017260: 6f72 2222 220a 0a20 2020 2020 2020 2064  or"""..        d
-00017270: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
-00017280: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017290: 2020 2069 6620 6361 6d65 7261 2069 7320     if camera is 
-000172a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000172b0: 2020 2020 2020 7365 6c66 2e63 616d 6572        self.camer
-000172c0: 615f 6964 203d 204e 6f6e 650a 2020 2020  a_id = None.    
-000172d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000172e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000172f0: 6c66 2e63 616d 6572 615f 6964 203d 2063  lf.camera_id = c
-00017300: 616d 6572 612e 6964 0a0a 2020 2020 2020  amera.id..      
-00017310: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
-00017320: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
-00017330: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
-00017340: 6566 2073 6574 5f73 7461 7475 735f 6c69  ef set_status_li
-00017350: 6768 7428 7365 6c66 2c20 656e 6162 6c65  ght(self, enable
-00017360: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-00017370: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-00017380: 7320 7468 6520 7374 6174 7573 2069 6e64  s the status ind
-00017390: 6963 6174 6f72 206c 6967 6874 2066 6f72  icator light for
-000173a0: 2074 6865 2064 6f6f 726c 6f63 6b22 2222   the doorlock"""
-000173b0: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
-000173c0: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
-000173d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000173e0: 6c66 2e6c 6564 5f73 6574 7469 6e67 732e  lf.led_settings.
-000173f0: 6973 5f65 6e61 626c 6564 203d 2065 6e61  is_enabled = ena
-00017400: 626c 6564 0a0a 2020 2020 2020 2020 6177  bled..        aw
-00017410: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
-00017420: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
-00017430: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00017440: 6574 5f61 7574 6f5f 636c 6f73 655f 7469  et_auto_close_ti
-00017450: 6d65 2873 656c 662c 2064 7572 6174 696f  me(self, duratio
-00017460: 6e3a 2074 696d 6564 656c 7461 2920 2d3e  n: timedelta) ->
-00017470: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00017480: 2222 5365 7473 2074 6865 2061 7574 6f2d  ""Sets the auto-
-00017490: 636c 6f73 6520 7469 6d65 2066 6f72 2064  close time for d
-000174a0: 6f6f 726c 6f63 6b2e 2030 2073 6563 6f6e  oorlock. 0 secon
-000174b0: 6473 203d 2064 6973 6162 6c65 642e 2222  ds = disabled.""
-000174c0: 220a 0a20 2020 2020 2020 2069 6620 6475  "..        if du
-000174d0: 7261 7469 6f6e 203e 2074 696d 6564 656c  ration > timedel
-000174e0: 7461 2868 6f75 7273 3d31 293a 0a20 2020  ta(hours=1):.   
-000174f0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
-00017500: 6164 5265 7175 6573 7428 224d 6178 2064  adRequest("Max d
-00017510: 7572 6174 696f 6e20 6973 2031 2068 6f75  uration is 1 hou
-00017520: 7222 290a 0a20 2020 2020 2020 2064 6566  r")..        def
-00017530: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
-00017540: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00017550: 2073 656c 662e 6175 746f 5f63 6c6f 7365   self.auto_close
-00017560: 5f74 696d 6520 3d20 6475 7261 7469 6f6e  _time = duration
-00017570: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00017580: 7365 6c66 2e71 7565 7565 5f75 7064 6174  self.queue_updat
-00017590: 6528 6361 6c6c 6261 636b 290a 0a20 2020  e(callback)..   
-000175a0: 2061 7379 6e63 2064 6566 2063 6c6f 7365   async def close
-000175b0: 5f6c 6f63 6b28 7365 6c66 2920 2d3e 204e  _lock(self) -> N
-000175c0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000175d0: 436c 6f73 6520 646f 6f72 6c6f 636b 2028  Close doorlock (
-000175e0: 6c6f 636b 2922 2222 0a0a 2020 2020 2020  lock)"""..      
-000175f0: 2020 6966 2073 656c 662e 6c6f 636b 5f73    if self.lock_s
-00017600: 7461 7475 7320 213d 204c 6f63 6b53 7461  tatus != LockSta
-00017610: 7475 7354 7970 652e 4f50 454e 3a0a 2020  tusType.OPEN:.  
-00017620: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017630: 4261 6452 6571 7565 7374 2822 4c6f 636b  BadRequest("Lock
-00017640: 2069 7320 6e6f 7420 6f70 656e 2229 0a0a   is not open")..
-00017650: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00017660: 6c66 2e61 7069 2e63 6c6f 7365 5f6c 6f63  lf.api.close_loc
-00017670: 6b28 7365 6c66 2e69 6429 0a0a 2020 2020  k(self.id)..    
-00017680: 6173 796e 6320 6465 6620 6f70 656e 5f6c  async def open_l
-00017690: 6f63 6b28 7365 6c66 2920 2d3e 204e 6f6e  ock(self) -> Non
-000176a0: 653a 0a20 2020 2020 2020 2022 2222 4f70  e:.        """Op
-000176b0: 656e 2064 6f6f 726c 6f63 6b20 2875 6e6c  en doorlock (unl
-000176c0: 6f63 6b29 2222 220a 0a20 2020 2020 2020  ock)"""..       
-000176d0: 2069 6620 7365 6c66 2e6c 6f63 6b5f 7374   if self.lock_st
-000176e0: 6174 7573 2021 3d20 4c6f 636b 5374 6174  atus != LockStat
-000176f0: 7573 5479 7065 2e43 4c4f 5345 443a 0a20  usType.CLOSED:. 
-00017700: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00017710: 2042 6164 5265 7175 6573 7428 224c 6f63   BadRequest("Loc
-00017720: 6b20 6973 206e 6f74 2063 6c6f 7365 6422  k is not closed"
-00017730: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
-00017740: 2073 656c 662e 6170 692e 6f70 656e 5f6c   self.api.open_l
-00017750: 6f63 6b28 7365 6c66 2e69 6429 0a0a 2020  ock(self.id)..  
-00017760: 2020 6173 796e 6320 6465 6620 6361 6c69    async def cali
-00017770: 6272 6174 6528 7365 6c66 2920 2d3e 204e  brate(self) -> N
-00017780: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00017790: 4361 6c69 6272 6174 6520 7468 6520 646f  Calibrate the do
-000177a0: 6f72 6c6f 636b 2e0a 0a20 2020 2020 2020  orlock...       
-000177b0: 2044 6f6f 7220 6d75 7374 2062 6520 6f70   Door must be op
-000177c0: 656e 2061 6e64 206c 6f63 6b20 756e 6c6f  en and lock unlo
-000177d0: 636b 6564 2e0a 2020 2020 2020 2020 2222  cked..        ""
-000177e0: 220a 0a20 2020 2020 2020 2061 7761 6974  "..        await
-000177f0: 2073 656c 662e 6170 692e 6361 6c69 6272   self.api.calibr
-00017800: 6174 655f 6c6f 636b 2873 656c 662e 6964  ate_lock(self.id
-00017810: 290a 0a0a 636c 6173 7320 4368 696d 6546  )...class ChimeF
-00017820: 6561 7475 7265 466c 6167 7328 5072 6f74  eatureFlags(Prot
-00017830: 6563 7442 6173 654f 626a 6563 7429 3a0a  ectBaseObject):.
-00017840: 2020 2020 6861 735f 7769 6669 3a20 626f      has_wifi: bo
-00017850: 6f6c 0a20 2020 2023 2032 2e39 2e32 302b  ol.    # 2.9.20+
-00017860: 0a20 2020 2068 6173 5f68 7474 7073 5f63  .    has_https_c
-00017870: 6c69 656e 745f 6f74 613a 204f 7074 696f  lient_ota: Optio
-00017880: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00017890: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-000178a0: 6f64 0a20 2020 2040 6361 6368 650a 2020  od.    @cache.  
-000178b0: 2020 6465 6620 5f67 6574 5f75 6e69 6669    def _get_unifi
-000178c0: 5f72 656d 6170 7328 636c 7329 202d 3e20  _remaps(cls) -> 
-000178d0: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
-000178e0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-000178f0: 2a2a 7375 7065 7228 292e 5f67 6574 5f75  **super()._get_u
-00017900: 6e69 6669 5f72 656d 6170 7328 292c 2022  nifi_remaps(), "
-00017910: 6861 7348 7474 7073 436c 6965 6e74 4f54  hasHttpsClientOT
-00017920: 4122 3a20 2268 6173 4874 7470 7343 6c69  A": "hasHttpsCli
-00017930: 656e 744f 7461 227d 0a0a 0a63 6c61 7373  entOta"}...class
-00017940: 2052 696e 6753 6574 7469 6e67 2850 726f   RingSetting(Pro
-00017950: 7465 6374 4261 7365 4f62 6a65 6374 293a  tectBaseObject):
-00017960: 0a20 2020 2063 616d 6572 615f 6964 3a20  .    camera_id: 
-00017970: 7374 720a 2020 2020 7265 7065 6174 5f74  str.    repeat_t
-00017980: 696d 6573 3a20 5265 7065 6174 5469 6d65  imes: RepeatTime
-00017990: 730a 2020 2020 7472 6163 6b5f 6e6f 3a20  s.    track_no: 
-000179a0: 696e 740a 2020 2020 766f 6c75 6d65 3a20  int.    volume: 
-000179b0: 696e 740a 0a20 2020 2040 636c 6173 736d  int..    @classm
-000179c0: 6574 686f 640a 2020 2020 4063 6163 6865  ethod.    @cache
-000179d0: 0a20 2020 2064 6566 205f 6765 745f 756e  .    def _get_un
-000179e0: 6966 695f 7265 6d61 7073 2863 6c73 2920  ifi_remaps(cls) 
-000179f0: 2d3e 2064 6963 745b 7374 722c 2073 7472  -> dict[str, str
-00017a00: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-00017a10: 6e20 7b2a 2a73 7570 6572 2829 2e5f 6765  n {**super()._ge
-00017a20: 745f 756e 6966 695f 7265 6d61 7073 2829  t_unifi_remaps()
-00017a30: 2c20 2263 616d 6572 6122 3a20 2263 616d  , "camera": "cam
-00017a40: 6572 6149 6422 7d0a 0a20 2020 2040 7072  eraId"}..    @pr
-00017a50: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-00017a60: 616d 6572 6128 7365 6c66 2920 2d3e 204f  amera(self) -> O
-00017a70: 7074 696f 6e61 6c5b 4361 6d65 7261 5d3a  ptional[Camera]:
-00017a80: 0a20 2020 2020 2020 2022 2222 5061 6972  .        """Pair
-00017a90: 6564 2043 616d 6572 6120 7769 6c6c 2061  ed Camera will a
-00017aa0: 6c77 6179 7320 6265 206e 6f6e 6520 6966  lways be none if
-00017ab0: 206e 6f20 6361 6d65 7261 2069 7320 7061   no camera is pa
-00017ac0: 6972 6564 2222 220a 0a20 2020 2020 2020  ired"""..       
-00017ad0: 2069 6620 7365 6c66 2e63 616d 6572 615f   if self.camera_
-00017ae0: 6964 2069 7320 4e6f 6e65 3a0a 2020 2020  id is None:.    
-00017af0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00017b00: 6f6e 650a 0a20 2020 2020 2020 2072 6574  one..        ret
-00017b10: 7572 6e20 7365 6c66 2e61 7069 2e62 6f6f  urn self.api.boo
-00017b20: 7473 7472 6170 2e63 616d 6572 6173 5b73  tstrap.cameras[s
-00017b30: 656c 662e 6361 6d65 7261 5f69 645d 0a0a  elf.camera_id]..
-00017b40: 0a63 6c61 7373 2043 6869 6d65 5472 6163  .class ChimeTrac
-00017b50: 6b28 5072 6f74 6563 7442 6173 654f 626a  k(ProtectBaseObj
-00017b60: 6563 7429 3a0a 2020 2020 6d64 353a 2073  ect):.    md5: s
-00017b70: 7472 0a20 2020 206e 616d 653a 2073 7472  tr.    name: str
-00017b80: 0a20 2020 2073 7461 7465 3a20 7374 720a  .    state: str.
-00017b90: 2020 2020 7472 6163 6b5f 6e6f 3a20 696e      track_no: in
-00017ba0: 740a 2020 2020 766f 6c75 6d65 3a20 696e  t.    volume: in
-00017bb0: 740a 2020 2020 7369 7a65 3a20 696e 740a  t.    size: int.
-00017bc0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00017bd0: 640a 2020 2020 4063 6163 6865 0a20 2020  d.    @cache.   
-00017be0: 2064 6566 205f 6765 745f 756e 6966 695f   def _get_unifi_
-00017bf0: 7265 6d61 7073 2863 6c73 2920 2d3e 2064  remaps(cls) -> d
-00017c00: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
-00017c10: 2020 2020 2020 2072 6574 7572 6e20 7b2a         return {*
-00017c20: 2a73 7570 6572 2829 2e5f 6765 745f 756e  *super()._get_un
-00017c30: 6966 695f 7265 6d61 7073 2829 2c20 2274  ifi_remaps(), "t
-00017c40: 7261 636b 5f6e 6f22 3a20 2274 7261 636b  rack_no": "track
-00017c50: 4e6f 227d 0a0a 0a63 6c61 7373 2043 6869  No"}...class Chi
-00017c60: 6d65 2850 726f 7465 6374 4164 6f70 7461  me(ProtectAdopta
-00017c70: 626c 6544 6576 6963 654d 6f64 656c 293a  bleDeviceModel):
-00017c80: 0a20 2020 2076 6f6c 756d 653a 2050 6572  .    volume: Per
-00017c90: 6365 6e74 496e 740a 2020 2020 6973 5f70  centInt.    is_p
-00017ca0: 726f 6269 6e67 5f66 6f72 5f77 6966 693a  robing_for_wifi:
-00017cb0: 2062 6f6f 6c0a 2020 2020 6c61 7374 5f72   bool.    last_r
-00017cc0: 696e 673a 204f 7074 696f 6e61 6c5b 6461  ing: Optional[da
-00017cd0: 7465 7469 6d65 5d0a 2020 2020 6973 5f77  tetime].    is_w
-00017ce0: 6972 656c 6573 735f 7570 6c69 6e6b 5f65  ireless_uplink_e
-00017cf0: 6e61 626c 6564 3a20 626f 6f6c 0a20 2020  nabled: bool.   
-00017d00: 2063 616d 6572 615f 6964 733a 206c 6973   camera_ids: lis
-00017d10: 745b 7374 725d 0a20 2020 2023 2072 6571  t[str].    # req
-00017d20: 7569 7265 7320 322e 362e 3137 2b0a 2020  uires 2.6.17+.  
-00017d30: 2020 6170 5f6d 676d 745f 6970 3a20 4f70    ap_mgmt_ip: Op
-00017d40: 7469 6f6e 616c 5b49 5076 3441 6464 7265  tional[IPv4Addre
-00017d50: 7373 5d20 3d20 4e6f 6e65 0a20 2020 2023  ss] = None.    #
-00017d60: 2072 6571 7569 7265 7320 322e 372e 3135   requires 2.7.15
-00017d70: 2b0a 2020 2020 6665 6174 7572 655f 666c  +.    feature_fl
-00017d80: 6167 733a 204f 7074 696f 6e61 6c5b 4368  ags: Optional[Ch
-00017d90: 696d 6546 6561 7475 7265 466c 6167 735d  imeFeatureFlags]
-00017da0: 203d 204e 6f6e 650a 2020 2020 2320 7265   = None.    # re
-00017db0: 7175 6972 6573 2032 2e38 2e32 322b 0a20  quires 2.8.22+. 
-00017dc0: 2020 2075 7365 725f 636f 6e66 6967 7572     user_configur
-00017dd0: 6564 5f61 703a 204f 7074 696f 6e61 6c5b  ed_ap: Optional[
-00017de0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a20 2020  bool] = None.   
-00017df0: 2023 2072 6571 7569 7265 7320 332e 302e   # requires 3.0.
-00017e00: 3232 2b0a 2020 2020 6861 735f 6874 7470  22+.    has_http
-00017e10: 735f 636c 6965 6e74 5f6f 7461 3a20 4f70  s_client_ota: Op
-00017e20: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00017e30: 6f6e 650a 2020 2020 706c 6174 666f 726d  one.    platform
-00017e40: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00017e50: 3d20 4e6f 6e65 0a20 2020 2072 6570 6561  = None.    repea
-00017e60: 745f 7469 6d65 733a 204f 7074 696f 6e61  t_times: Optiona
-00017e70: 6c5b 5265 7065 6174 5469 6d65 735d 203d  l[RepeatTimes] =
-00017e80: 204e 6f6e 650a 2020 2020 7472 6163 6b5f   None.    track_
-00017e90: 6e6f 3a20 4f70 7469 6f6e 616c 5b69 6e74  no: Optional[int
-00017ea0: 5d20 3d20 4e6f 6e65 0a20 2020 2072 696e  ] = None.    rin
-00017eb0: 675f 7365 7474 696e 6773 3a20 6c69 7374  g_settings: list
-00017ec0: 5b52 696e 6753 6574 7469 6e67 5d20 3d20  [RingSetting] = 
-00017ed0: 5b5d 0a20 2020 2073 7065 616b 6572 5f74  [].    speaker_t
-00017ee0: 7261 636b 5f6c 6973 743a 206c 6973 745b  rack_list: list[
-00017ef0: 4368 696d 6554 7261 636b 5d20 3d20 5b5d  ChimeTrack] = []
-00017f00: 0a0a 2020 2020 2320 544f 444f 3a20 7573  ..    # TODO: us
-00017f10: 6564 2066 6f72 2061 646f 7074 696f 6e0a  ed for adoption.
-00017f20: 2020 2020 2320 6170 4d61 6320 2072 6561      # apMac  rea
-00017f30: 6420 6f6e 6c79 0a20 2020 2023 2061 7052  d only.    # apR
-00017f40: 7373 6920 2072 6561 6420 6f6e 6c79 0a20  ssi  read only. 
-00017f50: 2020 2023 2065 6c65 6d65 6e74 496e 666f     # elementInfo
-00017f60: 2020 7265 6164 206f 6e6c 790a 0a20 2020    read only..   
-00017f70: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00017f80: 2020 4063 6163 6865 0a20 2020 2064 6566    @cache.    def
-00017f90: 205f 6765 745f 756e 6966 695f 7265 6d61   _get_unifi_rema
-00017fa0: 7073 2863 6c73 2920 2d3e 2064 6963 745b  ps(cls) -> dict[
-00017fb0: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-00017fc0: 2020 2072 6574 7572 6e20 7b2a 2a73 7570     return {**sup
-00017fd0: 6572 2829 2e5f 6765 745f 756e 6966 695f  er()._get_unifi_
-00017fe0: 7265 6d61 7073 2829 2c20 2268 6173 4874  remaps(), "hasHt
-00017ff0: 7470 7343 6c69 656e 744f 5441 223a 2022  tpsClientOTA": "
-00018000: 6861 7348 7474 7073 436c 6965 6e74 4f74  hasHttpsClientOt
-00018010: 6122 7d0a 0a20 2020 2040 636c 6173 736d  a"}..    @classm
-00018020: 6574 686f 640a 2020 2020 4063 6163 6865  ethod.    @cache
-00018030: 0a20 2020 2064 6566 205f 6765 745f 7265  .    def _get_re
-00018040: 6164 5f6f 6e6c 795f 6669 656c 6473 2863  ad_only_fields(c
-00018050: 6c73 2920 2d3e 2073 6574 5b73 7472 5d3a  ls) -> set[str]:
-00018060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018070: 7375 7065 7228 292e 5f67 6574 5f72 6561  super()._get_rea
-00018080: 645f 6f6e 6c79 5f66 6965 6c64 7328 2920  d_only_fields() 
-00018090: 7c20 7b22 6973 5072 6f62 696e 6746 6f72  | {"isProbingFor
-000180a0: 5769 6669 222c 2022 6c61 7374 5269 6e67  Wifi", "lastRing
-000180b0: 227d 0a0a 2020 2020 4070 726f 7065 7274  "}..    @propert
-000180c0: 790a 2020 2020 6465 6620 6361 6d65 7261  y.    def camera
-000180d0: 7328 7365 6c66 2920 2d3e 206c 6973 745b  s(self) -> list[
-000180e0: 4361 6d65 7261 5d3a 0a20 2020 2020 2020  Camera]:.       
-000180f0: 2022 2222 5061 6972 6564 2043 616d 6572   """Paired Camer
-00018100: 6173 2066 6f72 2063 6869 6d65 2222 220a  as for chime""".
-00018110: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00018120: 7365 6c66 2e63 616d 6572 615f 6964 7329  self.camera_ids)
-00018130: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00018140: 2020 2072 6574 7572 6e20 5b5d 0a20 2020     return [].   
-00018150: 2020 2020 2072 6574 7572 6e20 5b73 656c       return [sel
-00018160: 662e 6170 692e 626f 6f74 7374 7261 702e  f.api.bootstrap.
-00018170: 6361 6d65 7261 735b 635d 2066 6f72 2063  cameras[c] for c
-00018180: 2069 6e20 7365 6c66 2e63 616d 6572 615f   in self.camera_
-00018190: 6964 735d 0a0a 2020 2020 6173 796e 6320  ids]..    async 
-000181a0: 6465 6620 7365 745f 766f 6c75 6d65 2873  def set_volume(s
-000181b0: 656c 662c 206c 6576 656c 3a20 696e 7429  elf, level: int)
-000181c0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000181d0: 2020 2222 2253 6574 2074 6865 2076 6f6c    """Set the vol
-000181e0: 756d 6520 6f6e 2063 6869 6d65 2e22 2222  ume on chime."""
-000181f0: 0a0a 2020 2020 2020 2020 6f6c 645f 7661  ..        old_va
-00018200: 6c75 6520 3d20 7365 6c66 2e76 6f6c 756d  lue = self.volum
-00018210: 650a 2020 2020 2020 2020 6e65 775f 7661  e.        new_va
-00018220: 6c75 6520 3d20 5065 7263 656e 7449 6e74  lue = PercentInt
-00018230: 286c 6576 656c 290a 0a20 2020 2020 2020  (level)..       
-00018240: 2064 6566 2063 616c 6c62 6163 6b28 2920   def callback() 
-00018250: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00018260: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
-00018270: 203d 206e 6577 5f76 616c 7565 0a20 2020   = new_value.   
-00018280: 2020 2020 2020 2020 2066 6f72 2073 6574           for set
-00018290: 7469 6e67 2069 6e20 7365 6c66 2e72 696e  ting in self.rin
-000182a0: 675f 7365 7474 696e 6773 3a0a 2020 2020  g_settings:.    
-000182b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000182c0: 6574 7469 6e67 2e76 6f6c 756d 6520 3d3d  etting.volume ==
-000182d0: 206f 6c64 5f76 616c 7565 3a0a 2020 2020   old_value:.    
-000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182f0: 7365 7474 696e 672e 766f 6c75 6d65 203d  setting.volume =
-00018300: 206e 6577 5f76 616c 7565 0a0a 2020 2020   new_value..    
-00018310: 2020 2020 6177 6169 7420 7365 6c66 2e71      await self.q
-00018320: 7565 7565 5f75 7064 6174 6528 6361 6c6c  ueue_update(call
-00018330: 6261 636b 290a 0a20 2020 2061 7379 6e63  back)..    async
-00018340: 2064 6566 2073 6574 5f76 6f6c 756d 655f   def set_volume_
-00018350: 666f 725f 6361 6d65 7261 2873 656c 662c  for_camera(self,
-00018360: 2063 616d 6572 613a 2043 616d 6572 612c   camera: Camera,
-00018370: 206c 6576 656c 3a20 696e 7429 202d 3e20   level: int) -> 
-00018380: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00018390: 2253 6574 2074 6865 2076 6f6c 756d 6520  "Set the volume 
-000183a0: 6f6e 2063 6869 6d65 2066 6f72 2073 7065  on chime for spe
-000183b0: 6369 6669 6320 6361 6d65 7261 2e22 2222  cific camera."""
-000183c0: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
-000183d0: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
-000183e0: 3a0a 2020 2020 2020 2020 2020 2020 6861  :.            ha
-000183f0: 6e64 6c65 6420 3d20 4661 6c73 650a 2020  ndled = False.  
-00018400: 2020 2020 2020 2020 2020 666f 7220 7365            for se
-00018410: 7474 696e 6720 696e 2073 656c 662e 7269  tting in self.ri
-00018420: 6e67 5f73 6574 7469 6e67 733a 0a20 2020  ng_settings:.   
-00018430: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018440: 7365 7474 696e 672e 6361 6d65 7261 5f69  setting.camera_i
-00018450: 6420 3d3d 2063 616d 6572 612e 6964 3a0a  d == camera.id:.
-00018460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018470: 2020 2020 7365 7474 696e 672e 766f 6c75      setting.volu
-00018480: 6d65 203d 2063 6173 7428 5065 7263 656e  me = cast(Percen
-00018490: 7449 6e74 2c20 6c65 7665 6c29 0a20 2020  tInt, level).   
-000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184b0: 2068 616e 646c 6564 203d 2054 7275 650a   handled = True.
-000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
-000184e0: 2020 2020 2020 2069 6620 6e6f 7420 6861         if not ha
-000184f0: 6e64 6c65 643a 0a20 2020 2020 2020 2020  ndled:.         
-00018500: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
-00018510: 5265 7175 6573 7428 2243 616d 6572 6120  Request("Camera 
-00018520: 2573 2069 7320 6e6f 7420 7061 6972 6564  %s is not paired
-00018530: 2077 6974 6820 6368 696d 6522 2c20 6361   with chime", ca
-00018540: 6d65 7261 2e69 6429 0a0a 2020 2020 2020  mera.id)..      
-00018550: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
-00018560: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
-00018570: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
-00018580: 6566 2061 6464 5f63 616d 6572 6128 7365  ef add_camera(se
-00018590: 6c66 2c20 6361 6d65 7261 3a20 4361 6d65  lf, camera: Came
-000185a0: 7261 2920 2d3e 204e 6f6e 653a 0a20 2020  ra) -> None:.   
-000185b0: 2020 2020 2022 2222 4164 6473 206e 6577       """Adds new
-000185c0: 2070 6169 7265 6420 6361 6d65 7261 2074   paired camera t
-000185d0: 6f20 6368 696d 6522 2222 0a0a 2020 2020  o chime"""..    
-000185e0: 2020 2020 6966 206e 6f74 2063 616d 6572      if not camer
-000185f0: 612e 6665 6174 7572 655f 666c 6167 732e  a.feature_flags.
-00018600: 6973 5f64 6f6f 7262 656c 6c3a 0a20 2020  is_doorbell:.   
-00018610: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
-00018620: 6164 5265 7175 6573 7428 2243 616d 6572  adRequest("Camer
-00018630: 6120 646f 6573 206e 6f74 2068 6176 6520  a does not have 
-00018640: 6120 6368 696d 6522 290a 0a20 2020 2020  a chime")..     
-00018650: 2020 2069 6620 6361 6d65 7261 2e69 6420     if camera.id 
-00018660: 696e 2073 656c 662e 6361 6d65 7261 5f69  in self.camera_i
-00018670: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-00018680: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
-00018690: 2822 4361 6d65 7261 2069 7320 616c 7265  ("Camera is alre
-000186a0: 6164 7920 7061 6972 6564 2229 0a0a 2020  ady paired")..  
-000186b0: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
-000186c0: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
-000186d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000186e0: 616d 6572 615f 6964 732e 6170 7065 6e64  amera_ids.append
-000186f0: 2863 616d 6572 612e 6964 290a 0a20 2020  (camera.id)..   
-00018700: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
-00018710: 7175 6575 655f 7570 6461 7465 2863 616c  queue_update(cal
-00018720: 6c62 6163 6b29 0a0a 2020 2020 6173 796e  lback)..    asyn
-00018730: 6320 6465 6620 7265 6d6f 7665 5f63 616d  c def remove_cam
-00018740: 6572 6128 7365 6c66 2c20 6361 6d65 7261  era(self, camera
-00018750: 3a20 4361 6d65 7261 2920 2d3e 204e 6f6e  : Camera) -> Non
-00018760: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
-00018770: 6d6f 7665 7320 7061 6972 6564 2063 616d  moves paired cam
-00018780: 6572 6120 6672 6f6d 2063 6869 6d65 2222  era from chime""
-00018790: 220a 0a20 2020 2020 2020 2069 6620 6361  "..        if ca
-000187a0: 6d65 7261 2e69 6420 6e6f 7420 696e 2073  mera.id not in s
-000187b0: 656c 662e 6361 6d65 7261 5f69 6473 3a0a  elf.camera_ids:.
-000187c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000187d0: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
-000187e0: 6d65 7261 2069 7320 6e6f 7420 7061 6972  mera is not pair
-000187f0: 6564 2229 0a0a 2020 2020 2020 2020 6465  ed")..        de
-00018800: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
-00018810: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00018820: 2020 7365 6c66 2e63 616d 6572 615f 6964    self.camera_id
-00018830: 732e 7265 6d6f 7665 2863 616d 6572 612e  s.remove(camera.
-00018840: 6964 290a 0a20 2020 2020 2020 2061 7761  id)..        awa
-00018850: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
-00018860: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
-00018870: 2020 2020 6173 796e 6320 6465 6620 706c      async def pl
-00018880: 6179 280a 2020 2020 2020 2020 7365 6c66  ay(.        self
-00018890: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-000188a0: 2020 2020 2076 6f6c 756d 653a 2069 6e74       volume: int
-000188b0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-000188c0: 2020 2020 2020 2020 7265 7065 6174 5f74          repeat_t
-000188d0: 696d 6573 3a20 696e 7420 7c20 4e6f 6e65  imes: int | None
-000188e0: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
-000188f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00018900: 2222 2250 6c61 7973 2063 6869 6d65 2074  """Plays chime t
-00018910: 6f6e 6522 2222 0a0a 2020 2020 2020 2020  one"""..        
-00018920: 6177 6169 7420 7365 6c66 2e61 7069 2e70  await self.api.p
-00018930: 6c61 795f 7370 6561 6b65 7228 7365 6c66  lay_speaker(self
-00018940: 2e69 642c 2076 6f6c 756d 653d 766f 6c75  .id, volume=volu
-00018950: 6d65 2c20 7265 7065 6174 5f74 696d 6573  me, repeat_times
-00018960: 3d72 6570 6561 745f 7469 6d65 7329 0a0a  =repeat_times)..
-00018970: 2020 2020 6173 796e 6320 6465 6620 706c      async def pl
-00018980: 6179 5f62 757a 7a65 7228 7365 6c66 2920  ay_buzzer(self) 
-00018990: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000189a0: 2022 2222 506c 6179 7320 6368 696d 6520   """Plays chime 
-000189b0: 6275 7a7a 6572 2222 220a 0a20 2020 2020  buzzer"""..     
-000189c0: 2020 2061 7761 6974 2073 656c 662e 6170     await self.ap
-000189d0: 692e 706c 6179 5f62 757a 7a65 7228 7365  i.play_buzzer(se
-000189e0: 6c66 2e69 6429 0a0a 2020 2020 6173 796e  lf.id)..    asyn
-000189f0: 6320 6465 6620 7365 745f 7265 7065 6174  c def set_repeat
-00018a00: 5f74 696d 6573 2873 656c 662c 2076 616c  _times(self, val
-00018a10: 7565 3a20 696e 7429 202d 3e20 4e6f 6e65  ue: int) -> None
-00018a20: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-00018a30: 2072 6570 6561 7420 7469 6d65 7320 6f6e   repeat times on
-00018a40: 2063 6869 6d65 2e22 2222 0a0a 2020 2020   chime."""..    
-00018a50: 2020 2020 6f6c 645f 7661 6c75 6520 3d20      old_value = 
-00018a60: 7365 6c66 2e72 6570 6561 745f 7469 6d65  self.repeat_time
-00018a70: 730a 0a20 2020 2020 2020 2064 6566 2063  s..        def c
-00018a80: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
-00018a90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00018aa0: 656c 662e 7265 7065 6174 5f74 696d 6573  elf.repeat_times
-00018ab0: 203d 2063 6173 7428 5265 7065 6174 5469   = cast(RepeatTi
-00018ac0: 6d65 732c 2076 616c 7565 290a 2020 2020  mes, value).    
-00018ad0: 2020 2020 2020 2020 666f 7220 7365 7474          for sett
-00018ae0: 696e 6720 696e 2073 656c 662e 7269 6e67  ing in self.ring
-00018af0: 5f73 6574 7469 6e67 733a 0a20 2020 2020  _settings:.     
-00018b00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00018b10: 7474 696e 672e 7265 7065 6174 5f74 696d  tting.repeat_tim
-00018b20: 6573 203d 3d20 6f6c 645f 7661 6c75 653a  es == old_value:
-00018b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018b40: 2020 2020 2073 6574 7469 6e67 2e72 6570       setting.rep
-00018b50: 6561 745f 7469 6d65 7320 3d20 6361 7374  eat_times = cast
-00018b60: 2852 6570 6561 7454 696d 6573 2c20 7661  (RepeatTimes, va
-00018b70: 6c75 6529 0a0a 2020 2020 2020 2020 6177  lue)..        aw
-00018b80: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
-00018b90: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
-00018ba0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00018bb0: 6574 5f72 6570 6561 745f 7469 6d65 735f  et_repeat_times_
-00018bc0: 666f 725f 6361 6d65 7261 280a 2020 2020  for_camera(.    
-00018bd0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00018be0: 2020 6361 6d65 7261 3a20 4361 6d65 7261    camera: Camera
-00018bf0: 2c0a 2020 2020 2020 2020 7661 6c75 653a  ,.        value:
-00018c00: 2069 6e74 2c0a 2020 2020 2920 2d3e 204e   int,.    ) -> N
-00018c10: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00018c20: 5365 7420 7265 7065 6174 2074 696d 6573  Set repeat times
-00018c30: 206f 6e20 6368 696d 6520 666f 7220 7370   on chime for sp
-00018c40: 6563 6966 6963 2063 616d 6572 612e 2222  ecific camera.""
-00018c50: 220a 0a20 2020 2020 2020 2064 6566 2063  "..        def c
-00018c60: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
-00018c70: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
-00018c80: 616e 646c 6564 203d 2046 616c 7365 0a20  andled = False. 
-00018c90: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00018ca0: 6574 7469 6e67 2069 6e20 7365 6c66 2e72  etting in self.r
-00018cb0: 696e 675f 7365 7474 696e 6773 3a0a 2020  ing_settings:.  
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018cd0: 2073 6574 7469 6e67 2e63 616d 6572 615f   setting.camera_
-00018ce0: 6964 203d 3d20 6361 6d65 7261 2e69 643a  id == camera.id:
-00018cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d00: 2020 2020 2073 6574 7469 6e67 2e72 6570       setting.rep
-00018d10: 6561 745f 7469 6d65 7320 3d20 6361 7374  eat_times = cast
-00018d20: 2852 6570 6561 7454 696d 6573 2c20 7661  (RepeatTimes, va
-00018d30: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
-00018d40: 2020 2020 2020 2020 2068 616e 646c 6564           handled
-00018d50: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00018d60: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00018d70: 6b0a 0a20 2020 2020 2020 2020 2020 2069  k..            i
-00018d80: 6620 6e6f 7420 6861 6e64 6c65 643a 0a20  f not handled:. 
-00018d90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018da0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
-00018db0: 2243 616d 6572 6120 2573 2069 7320 6e6f  "Camera %s is no
-00018dc0: 7420 7061 6972 6564 2077 6974 6820 6368  t paired with ch
-00018dd0: 696d 6522 2c20 6361 6d65 7261 2e69 6429  ime", camera.id)
-00018de0: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00018df0: 7365 6c66 2e71 7565 7565 5f75 7064 6174  self.queue_updat
-00018e00: 6528 6361 6c6c 6261 636b 290a            e(callback).
+0000ca50: 2028 0a20 2020 2020 2020 2020 2020 2073   (.            s
+0000ca60: 656c 662e 6973 5f72 6563 6f72 6469 6e67  elf.is_recording
+0000ca70: 5f65 6e61 626c 6564 0a20 2020 2020 2020  _enabled.       
+0000ca80: 2020 2020 2061 6e64 2062 6f6f 6c28 7365       and bool(se
+0000ca90: 6c66 2e61 6374 6976 655f 6175 6469 6f5f  lf.active_audio_
+0000caa0: 6465 7465 6374 5f74 7970 6573 290a 2020  detect_types).  
+0000cab0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+0000cac0: 6c66 2e6c 6173 745f 736d 6172 745f 6175  lf.last_smart_au
+0000cad0: 6469 6f5f 6465 7465 6374 5f65 7665 6e74  dio_detect_event
+0000cae0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000caf0: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
+0000cb00: 662e 6c61 7374 5f73 6d61 7274 5f61 7564  f.last_smart_aud
+0000cb10: 696f 5f64 6574 6563 745f 6576 656e 742e  io_detect_event.
+0000cb20: 656e 6420 6973 204e 6f6e 650a 2020 2020  end is None.    
+0000cb30: 2020 2020 290a 0a20 2020 2023 2072 6567      )..    # reg
+0000cb40: 696f 6e20 536d 6f6b 6520 416c 6172 6d0a  ion Smoke Alarm.
+0000cb50: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000cb60: 2020 2064 6566 2063 616e 5f64 6574 6563     def can_detec
+0000cb70: 745f 736d 6f6b 6528 7365 6c66 2920 2d3e  t_smoke(self) ->
+0000cb80: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
+0000cb90: 6574 7572 6e20 7365 6c66 2e5f 6361 6e5f  eturn self._can_
+0000cba0: 6465 7465 6374 5f61 7564 696f 2853 6d61  detect_audio(Sma
+0000cbb0: 7274 4465 7465 6374 4f62 6a65 6374 5479  rtDetectObjectTy
+0000cbc0: 7065 2e53 4d4f 4b45 290a 0a20 2020 2040  pe.SMOKE)..    @
+0000cbd0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000cbe0: 2069 735f 736d 6f6b 655f 6465 7465 6374   is_smoke_detect
+0000cbf0: 696f 6e5f 6f6e 2873 656c 6629 202d 3e20  ion_on(self) -> 
+0000cc00: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+0000cc10: 2249 7320 536d 6f6b 6520 416c 6172 6d20  "Is Smoke Alarm 
+0000cc20: 4465 7465 6374 696f 6e20 6176 6169 6c61  Detection availa
+0000cc30: 626c 6520 616e 6420 656e 6162 6c65 6420  ble and enabled 
+0000cc40: 2863 616d 6572 6120 7769 6c6c 2070 726f  (camera will pro
+0000cc50: 6475 6365 2073 6d6f 6b65 0a20 2020 2020  duce smoke.     
+0000cc60: 2020 2073 6d61 7274 2064 6574 6563 7469     smart detecti
+0000cc70: 6f6e 2065 7665 6e74 7329 3f0a 2020 2020  on events)?.    
+0000cc80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000cc90: 2072 6574 7572 6e20 7365 6c66 2e5f 6973   return self._is
+0000cca0: 5f61 7564 696f 5f65 6e61 626c 6564 2853  _audio_enabled(S
+0000ccb0: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
+0000ccc0: 5479 7065 2e53 4d4f 4b45 290a 0a20 2020  Type.SMOKE)..   
+0000ccd0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000cce0: 6566 206c 6173 745f 736d 6f6b 655f 6465  ef last_smoke_de
+0000ccf0: 7465 6374 5f65 7665 6e74 2873 656c 6629  tect_event(self)
+0000cd00: 202d 3e20 4f70 7469 6f6e 616c 5b45 7665   -> Optional[Eve
+0000cd10: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
+0000cd20: 4765 7420 7468 6520 6c61 7374 2070 6572  Get the last per
+0000cd30: 736f 6e20 736d 6172 7420 6465 7465 6374  son smart detect
+0000cd40: 696f 6e20 6576 656e 742e 2222 220a 0a20  ion event.""".. 
+0000cd50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000cd60: 6c66 2e67 6574 5f6c 6173 745f 736d 6172  lf.get_last_smar
+0000cd70: 745f 6175 6469 6f5f 6465 7465 6374 5f65  t_audio_detect_e
+0000cd80: 7665 6e74 2853 6d61 7274 4465 7465 6374  vent(SmartDetect
+0000cd90: 4175 6469 6f54 7970 652e 534d 4f4b 4529  AudioType.SMOKE)
+0000cda0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000cdb0: 2020 2020 6465 6620 6c61 7374 5f73 6d6f      def last_smo
+0000cdc0: 6b65 5f64 6574 6563 7428 7365 6c66 2920  ke_detect(self) 
+0000cdd0: 2d3e 204f 7074 696f 6e61 6c5b 6461 7465  -> Optional[date
+0000cde0: 7469 6d65 5d3a 0a20 2020 2020 2020 2022  time]:.        "
+0000cdf0: 2222 4765 7420 7468 6520 6c61 7374 2073  ""Get the last s
+0000ce00: 6d6f 6b65 2073 6d61 7274 2064 6574 6563  moke smart detec
+0000ce10: 7469 6f6e 2065 7665 6e74 2e22 2222 0a0a  tion event."""..
+0000ce20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000ce30: 656c 662e 6c61 7374 5f73 6d61 7274 5f61  elf.last_smart_a
+0000ce40: 7564 696f 5f64 6574 6563 7473 2e67 6574  udio_detects.get
+0000ce50: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
+0000ce60: 6f54 7970 652e 534d 4f4b 4529 0a0a 2020  oType.SMOKE)..  
+0000ce70: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000ce80: 6465 6620 6973 5f73 6d6f 6b65 5f63 7572  def is_smoke_cur
+0000ce90: 7265 6e74 6c79 5f64 6574 6563 7465 6428  rently_detected(
+0000cea0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+0000ceb0: 2020 2020 2020 2022 2222 4973 2073 6d6f         """Is smo
+0000cec0: 6b65 2061 6c61 726d 2063 7572 7265 6e74  ke alarm current
+0000ced0: 6c79 2062 6569 6e67 2064 6574 6563 7465  ly being detecte
+0000cee0: 6422 2222 0a0a 2020 2020 2020 2020 7265  d"""..        re
+0000cef0: 7475 726e 2073 656c 662e 5f69 735f 6175  turn self._is_au
+0000cf00: 6469 6f5f 6465 7465 6374 6564 2853 6d61  dio_detected(Sma
+0000cf10: 7274 4465 7465 6374 4f62 6a65 6374 5479  rtDetectObjectTy
+0000cf20: 7065 2e53 4d4f 4b45 290a 0a20 2020 2061  pe.SMOKE)..    a
+0000cf30: 7379 6e63 2064 6566 2073 6574 5f73 6d6f  sync def set_smo
+0000cf40: 6b65 5f64 6574 6563 7469 6f6e 2873 656c  ke_detection(sel
+0000cf50: 662c 2065 6e61 626c 6564 3a20 626f 6f6c  f, enabled: bool
+0000cf60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000cf70: 2020 2022 2222 546f 6767 6c65 7320 736d     """Toggles sm
+0000cf80: 6f6b 6520 736d 6172 7420 6465 7465 6374  oke smart detect
+0000cf90: 696f 6e2e 2052 6571 7569 7265 7320 6361  ion. Requires ca
+0000cfa0: 6d65 7261 2074 6f20 6861 7665 2073 6d61  mera to have sma
+0000cfb0: 7274 2064 6574 6563 7469 6f6e 2222 220a  rt detection""".
+0000cfc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cfd0: 6177 6169 7420 7365 6c66 2e5f 7365 745f  await self._set_
+0000cfe0: 6175 6469 6f5f 6465 7465 6374 2853 6d61  audio_detect(Sma
+0000cff0: 7274 4465 7465 6374 4175 6469 6f54 7970  rtDetectAudioTyp
+0000d000: 652e 534d 4f4b 452c 2065 6e61 626c 6564  e.SMOKE, enabled
+0000d010: 290a 0a20 2020 2023 2065 6e64 7265 6769  )..    # endregi
+0000d020: 6f6e 0a20 2020 2023 2072 6567 696f 6e20  on.    # region 
+0000d030: 434f 2041 6c61 726d 0a0a 2020 2020 4070  CO Alarm..    @p
+0000d040: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000d050: 6361 6e5f 6465 7465 6374 5f63 6f28 7365  can_detect_co(se
+0000d060: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+0000d070: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000d080: 2e5f 6361 6e5f 6465 7465 6374 5f61 7564  ._can_detect_aud
+0000d090: 696f 2853 6d61 7274 4465 7465 6374 4f62  io(SmartDetectOb
+0000d0a0: 6a65 6374 5479 7065 2e43 4d4f 4e58 290a  jectType.CMONX).
+0000d0b0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000d0c0: 2020 2064 6566 2069 735f 636f 5f64 6574     def is_co_det
+0000d0d0: 6563 7469 6f6e 5f6f 6e28 7365 6c66 2920  ection_on(self) 
+0000d0e0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000d0f0: 2022 2222 4973 2043 4f20 416c 6172 6d20   """Is CO Alarm 
+0000d100: 4465 7465 6374 696f 6e20 6176 6169 6c61  Detection availa
+0000d110: 626c 6520 616e 6420 656e 6162 6c65 6420  ble and enabled 
+0000d120: 2863 616d 6572 6120 7769 6c6c 2070 726f  (camera will pro
+0000d130: 6475 6365 2073 6d6f 6b65 2073 6d61 7274  duce smoke smart
+0000d140: 0a20 2020 2020 2020 2064 6574 6563 7469  .        detecti
+0000d150: 6f6e 2065 7665 6e74 7329 3f0a 2020 2020  on events)?.    
+0000d160: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000d170: 2072 6574 7572 6e20 7365 6c66 2e5f 6973   return self._is
+0000d180: 5f61 7564 696f 5f65 6e61 626c 6564 2853  _audio_enabled(S
+0000d190: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
+0000d1a0: 5479 7065 2e43 4d4f 4e58 290a 0a20 2020  Type.CMONX)..   
+0000d1b0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000d1c0: 6566 206c 6173 745f 636d 6f6e 785f 6465  ef last_cmonx_de
+0000d1d0: 7465 6374 5f65 7665 6e74 2873 656c 6629  tect_event(self)
+0000d1e0: 202d 3e20 4f70 7469 6f6e 616c 5b45 7665   -> Optional[Eve
+0000d1f0: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
+0000d200: 4765 7420 7468 6520 6c61 7374 2043 4f20  Get the last CO 
+0000d210: 616c 6172 6d20 736d 6172 7420 6465 7465  alarm smart dete
+0000d220: 6374 696f 6e20 6576 656e 742e 2222 220a  ction event.""".
+0000d230: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d240: 7365 6c66 2e67 6574 5f6c 6173 745f 736d  self.get_last_sm
+0000d250: 6172 745f 6175 6469 6f5f 6465 7465 6374  art_audio_detect
+0000d260: 5f65 7665 6e74 2853 6d61 7274 4465 7465  _event(SmartDete
+0000d270: 6374 4175 6469 6f54 7970 652e 434d 4f4e  ctAudioType.CMON
+0000d280: 5829 0a0a 2020 2020 4070 726f 7065 7274  X)..    @propert
+0000d290: 790a 2020 2020 6465 6620 6c61 7374 5f63  y.    def last_c
+0000d2a0: 6d6f 6e78 5f64 6574 6563 7428 7365 6c66  monx_detect(self
+0000d2b0: 2920 2d3e 204f 7074 696f 6e61 6c5b 6461  ) -> Optional[da
+0000d2c0: 7465 7469 6d65 5d3a 0a20 2020 2020 2020  tetime]:.       
+0000d2d0: 2022 2222 4765 7420 7468 6520 6c61 7374   """Get the last
+0000d2e0: 2043 4f20 616c 6172 6d20 736d 6172 7420   CO alarm smart 
+0000d2f0: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
+0000d300: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000d310: 7572 6e20 7365 6c66 2e6c 6173 745f 736d  urn self.last_sm
+0000d320: 6172 745f 6175 6469 6f5f 6465 7465 6374  art_audio_detect
+0000d330: 732e 6765 7428 536d 6172 7444 6574 6563  s.get(SmartDetec
+0000d340: 7441 7564 696f 5479 7065 2e43 4d4f 4e58  tAudioType.CMONX
+0000d350: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000d360: 0a20 2020 2064 6566 2069 735f 636d 6f6e  .    def is_cmon
+0000d370: 785f 6375 7272 656e 746c 795f 6465 7465  x_currently_dete
+0000d380: 6374 6564 2873 656c 6629 202d 3e20 626f  cted(self) -> bo
+0000d390: 6f6c 3a0a 2020 2020 2020 2020 2222 2249  ol:.        """I
+0000d3a0: 7320 434f 2061 6c61 726d 2063 7572 7265  s CO alarm curre
+0000d3b0: 6e74 6c79 2062 6569 6e67 2064 6574 6563  ntly being detec
+0000d3c0: 7465 6422 2222 0a0a 2020 2020 2020 2020  ted"""..        
+0000d3d0: 7265 7475 726e 2073 656c 662e 5f69 735f  return self._is_
+0000d3e0: 6175 6469 6f5f 6465 7465 6374 6564 2853  audio_detected(S
+0000d3f0: 6d61 7274 4465 7465 6374 4f62 6a65 6374  martDetectObject
+0000d400: 5479 7065 2e43 4d4f 4e58 290a 0a20 2020  Type.CMONX)..   
+0000d410: 2061 7379 6e63 2064 6566 2073 6574 5f63   async def set_c
+0000d420: 6d6f 6e78 5f64 6574 6563 7469 6f6e 2873  monx_detection(s
+0000d430: 656c 662c 2065 6e61 626c 6564 3a20 626f  elf, enabled: bo
+0000d440: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
+0000d450: 2020 2020 2022 2222 546f 6767 6c65 7320       """Toggles 
+0000d460: 736d 6f6b 6520 736d 6172 7420 6465 7465  smoke smart dete
+0000d470: 6374 696f 6e2e 2052 6571 7569 7265 7320  ction. Requires 
+0000d480: 6361 6d65 7261 2074 6f20 6861 7665 2073  camera to have s
+0000d490: 6d61 7274 2064 6574 6563 7469 6f6e 2222  mart detection""
+0000d4a0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000d4b0: 6e20 6177 6169 7420 7365 6c66 2e5f 7365  n await self._se
+0000d4c0: 745f 6175 6469 6f5f 6465 7465 6374 2853  t_audio_detect(S
+0000d4d0: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
+0000d4e0: 7970 652e 434d 4f4e 582c 2065 6e61 626c  ype.CMONX, enabl
+0000d4f0: 6564 290a 0a20 2020 2023 2065 6e64 7265  ed)..    # endre
+0000d500: 6769 6f6e 0a20 2020 2023 2072 6567 696f  gion.    # regio
+0000d510: 6e20 5369 7265 6e0a 0a20 2020 2040 7072  n Siren..    @pr
+0000d520: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+0000d530: 616e 5f64 6574 6563 745f 7369 7265 6e28  an_detect_siren(
+0000d540: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+0000d550: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000d560: 6c66 2e5f 6361 6e5f 6465 7465 6374 5f61  lf._can_detect_a
+0000d570: 7564 696f 2853 6d61 7274 4465 7465 6374  udio(SmartDetect
+0000d580: 4f62 6a65 6374 5479 7065 2e53 4952 454e  ObjectType.SIREN
+0000d590: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000d5a0: 0a20 2020 2064 6566 2069 735f 7369 7265  .    def is_sire
+0000d5b0: 6e5f 6465 7465 6374 696f 6e5f 6f6e 2873  n_detection_on(s
+0000d5c0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000d5d0: 2020 2020 2020 2222 2249 7320 5369 7265        """Is Sire
+0000d5e0: 6e20 4465 7465 6374 696f 6e20 6176 6169  n Detection avai
+0000d5f0: 6c61 626c 6520 616e 6420 656e 6162 6c65  lable and enable
+0000d600: 6420 2863 616d 6572 6120 7769 6c6c 2070  d (camera will p
+0000d610: 726f 6475 6365 2073 6972 656e 2073 6d61  roduce siren sma
+0000d620: 7274 0a20 2020 2020 2020 2064 6574 6563  rt.        detec
+0000d630: 7469 6f6e 2065 7665 6e74 7329 3f0a 2020  tion events)?.  
+0000d640: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000d650: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000d660: 6973 5f61 7564 696f 5f65 6e61 626c 6564  is_audio_enabled
+0000d670: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000d680: 6374 5479 7065 2e53 4952 454e 290a 0a20  ctType.SIREN).. 
+0000d690: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000d6a0: 2064 6566 206c 6173 745f 7369 7265 6e5f   def last_siren_
+0000d6b0: 6465 7465 6374 5f65 7665 6e74 2873 656c  detect_event(sel
+0000d6c0: 6629 202d 3e20 4f70 7469 6f6e 616c 5b45  f) -> Optional[E
+0000d6d0: 7665 6e74 5d3a 0a20 2020 2020 2020 2022  vent]:.        "
+0000d6e0: 2222 4765 7420 7468 6520 6c61 7374 2053  ""Get the last S
+0000d6f0: 6972 656e 2073 6d61 7274 2064 6574 6563  iren smart detec
+0000d700: 7469 6f6e 2065 7665 6e74 2e22 2222 0a0a  tion event."""..
+0000d710: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d720: 656c 662e 6765 745f 6c61 7374 5f73 6d61  elf.get_last_sma
+0000d730: 7274 5f61 7564 696f 5f64 6574 6563 745f  rt_audio_detect_
+0000d740: 6576 656e 7428 536d 6172 7444 6574 6563  event(SmartDetec
+0000d750: 7441 7564 696f 5479 7065 2e53 4952 454e  tAudioType.SIREN
+0000d760: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000d770: 0a20 2020 2064 6566 206c 6173 745f 7369  .    def last_si
+0000d780: 7265 6e5f 6465 7465 6374 2873 656c 6629  ren_detect(self)
+0000d790: 202d 3e20 4f70 7469 6f6e 616c 5b64 6174   -> Optional[dat
+0000d7a0: 6574 696d 655d 3a0a 2020 2020 2020 2020  etime]:.        
+0000d7b0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+0000d7c0: 5369 7265 6e20 736d 6172 7420 6465 7465  Siren smart dete
+0000d7d0: 6374 696f 6e20 6576 656e 742e 2222 220a  ction event.""".
+0000d7e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d7f0: 7365 6c66 2e6c 6173 745f 736d 6172 745f  self.last_smart_
+0000d800: 6175 6469 6f5f 6465 7465 6374 732e 6765  audio_detects.ge
+0000d810: 7428 536d 6172 7444 6574 6563 7441 7564  t(SmartDetectAud
+0000d820: 696f 5479 7065 2e53 4952 454e 290a 0a20  ioType.SIREN).. 
+0000d830: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000d840: 2064 6566 2069 735f 7369 7265 6e5f 6375   def is_siren_cu
+0000d850: 7272 656e 746c 795f 6465 7465 6374 6564  rrently_detected
+0000d860: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000d870: 2020 2020 2020 2020 2222 2249 7320 5369          """Is Si
+0000d880: 7265 6e20 6375 7272 656e 746c 7920 6265  ren currently be
+0000d890: 696e 6720 6465 7465 6374 6564 2222 220a  ing detected""".
+0000d8a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d8b0: 7365 6c66 2e5f 6973 5f61 7564 696f 5f64  self._is_audio_d
+0000d8c0: 6574 6563 7465 6428 536d 6172 7444 6574  etected(SmartDet
+0000d8d0: 6563 744f 626a 6563 7454 7970 652e 5349  ectObjectType.SI
+0000d8e0: 5245 4e29 0a0a 2020 2020 6173 796e 6320  REN)..    async 
+0000d8f0: 6465 6620 7365 745f 7369 7265 6e5f 6465  def set_siren_de
+0000d900: 7465 6374 696f 6e28 7365 6c66 2c20 656e  tection(self, en
+0000d910: 6162 6c65 643a 2062 6f6f 6c29 202d 3e20  abled: bool) -> 
+0000d920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000d930: 2254 6f67 676c 6573 2073 6972 656e 2073  "Toggles siren s
+0000d940: 6d61 7274 2064 6574 6563 7469 6f6e 2e20  mart detection. 
+0000d950: 5265 7175 6972 6573 2063 616d 6572 6120  Requires camera 
+0000d960: 746f 2068 6176 6520 736d 6172 7420 6465  to have smart de
+0000d970: 7465 6374 696f 6e22 2222 0a0a 2020 2020  tection"""..    
+0000d980: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0000d990: 2073 656c 662e 5f73 6574 5f61 7564 696f   self._set_audio
+0000d9a0: 5f64 6574 6563 7428 536d 6172 7444 6574  _detect(SmartDet
+0000d9b0: 6563 7441 7564 696f 5479 7065 2e53 4952  ectAudioType.SIR
+0000d9c0: 454e 2c20 656e 6162 6c65 6429 0a0a 2020  EN, enabled)..  
+0000d9d0: 2020 2320 656e 6472 6567 696f 6e0a 2020    # endregion.  
+0000d9e0: 2020 2320 7265 6769 6f6e 2042 6162 7920    # region Baby 
+0000d9f0: 4372 790a 0a20 2020 2040 7072 6f70 6572  Cry..    @proper
+0000da00: 7479 0a20 2020 2064 6566 2063 616e 5f64  ty.    def can_d
+0000da10: 6574 6563 745f 6261 6279 5f63 7279 2873  etect_baby_cry(s
+0000da20: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000da30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000da40: 662e 5f63 616e 5f64 6574 6563 745f 6175  f._can_detect_au
+0000da50: 6469 6f28 536d 6172 7444 6574 6563 744f  dio(SmartDetectO
+0000da60: 626a 6563 7454 7970 652e 4241 4259 5f43  bjectType.BABY_C
+0000da70: 5259 290a 0a20 2020 2040 7072 6f70 6572  RY)..    @proper
+0000da80: 7479 0a20 2020 2064 6566 2069 735f 6261  ty.    def is_ba
+0000da90: 6279 5f63 7279 5f64 6574 6563 7469 6f6e  by_cry_detection
+0000daa0: 5f6f 6e28 7365 6c66 2920 2d3e 2062 6f6f  _on(self) -> boo
+0000dab0: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
+0000dac0: 2042 6162 7920 4372 7920 4465 7465 6374   Baby Cry Detect
+0000dad0: 696f 6e20 6176 6169 6c61 626c 6520 616e  ion available an
+0000dae0: 6420 656e 6162 6c65 6420 2863 616d 6572  d enabled (camer
+0000daf0: 6120 7769 6c6c 2070 726f 6475 6365 2062  a will produce b
+0000db00: 6162 7920 6372 7920 736d 6172 740a 2020  aby cry smart.  
+0000db10: 2020 2020 2020 6465 7465 6374 696f 6e20        detection 
+0000db20: 6576 656e 7473 293f 0a20 2020 2020 2020  events)?.       
+0000db30: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+0000db40: 7475 726e 2073 656c 662e 5f69 735f 6175  turn self._is_au
+0000db50: 6469 6f5f 656e 6162 6c65 6428 536d 6172  dio_enabled(Smar
+0000db60: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
+0000db70: 652e 4241 4259 5f43 5259 290a 0a20 2020  e.BABY_CRY)..   
+0000db80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000db90: 6566 206c 6173 745f 6261 6279 5f63 7279  ef last_baby_cry
+0000dba0: 5f64 6574 6563 745f 6576 656e 7428 7365  _detect_event(se
+0000dbb0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000dbc0: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
+0000dbd0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+0000dbe0: 4261 6279 2043 7279 2073 6d61 7274 2064  Baby Cry smart d
+0000dbf0: 6574 6563 7469 6f6e 2065 7665 6e74 2e22  etection event."
+0000dc00: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000dc10: 726e 2073 656c 662e 6765 745f 6c61 7374  rn self.get_last
+0000dc20: 5f73 6d61 7274 5f61 7564 696f 5f64 6574  _smart_audio_det
+0000dc30: 6563 745f 6576 656e 7428 536d 6172 7444  ect_event(SmartD
+0000dc40: 6574 6563 7441 7564 696f 5479 7065 2e42  etectAudioType.B
+0000dc50: 4142 595f 4352 5929 0a0a 2020 2020 4070  ABY_CRY)..    @p
+0000dc60: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000dc70: 6c61 7374 5f62 6162 795f 6372 795f 6465  last_baby_cry_de
+0000dc80: 7465 6374 2873 656c 6629 202d 3e20 4f70  tect(self) -> Op
+0000dc90: 7469 6f6e 616c 5b64 6174 6574 696d 655d  tional[datetime]
+0000dca0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000dcb0: 2074 6865 206c 6173 7420 4261 6279 2043   the last Baby C
+0000dcc0: 7279 2073 6d61 7274 2064 6574 6563 7469  ry smart detecti
+0000dcd0: 6f6e 2065 7665 6e74 2e22 2222 0a0a 2020  on event."""..  
+0000dce0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000dcf0: 662e 6c61 7374 5f73 6d61 7274 5f61 7564  f.last_smart_aud
+0000dd00: 696f 5f64 6574 6563 7473 2e67 6574 2853  io_detects.get(S
+0000dd10: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
+0000dd20: 7970 652e 4241 4259 5f43 5259 290a 0a20  ype.BABY_CRY).. 
+0000dd30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000dd40: 2064 6566 2069 735f 6261 6279 5f63 7279   def is_baby_cry
+0000dd50: 5f63 7572 7265 6e74 6c79 5f64 6574 6563  _currently_detec
+0000dd60: 7465 6428 7365 6c66 2920 2d3e 2062 6f6f  ted(self) -> boo
+0000dd70: 6c3a 0a20 2020 2020 2020 2022 2222 4973  l:.        """Is
+0000dd80: 2042 6162 7920 4372 7920 6375 7272 656e   Baby Cry curren
+0000dd90: 746c 7920 6265 696e 6720 6465 7465 6374  tly being detect
+0000dda0: 6564 2222 220a 0a20 2020 2020 2020 2072  ed"""..        r
+0000ddb0: 6574 7572 6e20 7365 6c66 2e5f 6973 5f61  eturn self._is_a
+0000ddc0: 7564 696f 5f64 6574 6563 7465 6428 536d  udio_detected(Sm
+0000ddd0: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
+0000dde0: 7970 652e 4241 4259 5f43 5259 290a 0a20  ype.BABY_CRY).. 
+0000ddf0: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+0000de00: 5f62 6162 795f 6372 795f 6465 7465 6374  _baby_cry_detect
+0000de10: 696f 6e28 7365 6c66 2c20 656e 6162 6c65  ion(self, enable
+0000de20: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
+0000de30: 3a0a 2020 2020 2020 2020 2222 2254 6f67  :.        """Tog
+0000de40: 676c 6573 2062 6162 795f 6372 7920 736d  gles baby_cry sm
+0000de50: 6172 7420 6465 7465 6374 696f 6e2e 2052  art detection. R
+0000de60: 6571 7569 7265 7320 6361 6d65 7261 2074  equires camera t
+0000de70: 6f20 6861 7665 2073 6d61 7274 2064 6574  o have smart det
+0000de80: 6563 7469 6f6e 2222 220a 0a20 2020 2020  ection"""..     
+0000de90: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+0000dea0: 7365 6c66 2e5f 7365 745f 6175 6469 6f5f  self._set_audio_
+0000deb0: 6465 7465 6374 2853 6d61 7274 4465 7465  detect(SmartDete
+0000dec0: 6374 4175 6469 6f54 7970 652e 4241 4259  ctAudioType.BABY
+0000ded0: 5f43 5259 2c20 656e 6162 6c65 6429 0a0a  _CRY, enabled)..
+0000dee0: 2020 2020 2320 656e 6472 6567 696f 6e0a      # endregion.
+0000def0: 2020 2020 2320 7265 6769 6f6e 2053 7065      # region Spe
+0000df00: 616b 696e 670a 0a20 2020 2040 7072 6f70  aking..    @prop
+0000df10: 6572 7479 0a20 2020 2064 6566 2063 616e  erty.    def can
+0000df20: 5f64 6574 6563 745f 7370 6561 6b69 6e67  _detect_speaking
+0000df30: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000df40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000df50: 656c 662e 5f63 616e 5f64 6574 6563 745f  elf._can_detect_
+0000df60: 6175 6469 6f28 536d 6172 7444 6574 6563  audio(SmartDetec
+0000df70: 744f 626a 6563 7454 7970 652e 5350 4541  tObjectType.SPEA
+0000df80: 4b29 0a0a 2020 2020 4070 726f 7065 7274  K)..    @propert
+0000df90: 790a 2020 2020 6465 6620 6973 5f73 7065  y.    def is_spe
+0000dfa0: 616b 696e 675f 6465 7465 6374 696f 6e5f  aking_detection_
+0000dfb0: 6f6e 2873 656c 6629 202d 3e20 626f 6f6c  on(self) -> bool
+0000dfc0: 3a0a 2020 2020 2020 2020 2222 2249 7320  :.        """Is 
+0000dfd0: 5370 6561 6b69 6e67 2044 6574 6563 7469  Speaking Detecti
+0000dfe0: 6f6e 2061 7661 696c 6162 6c65 2061 6e64  on available and
+0000dff0: 2065 6e61 626c 6564 2028 6361 6d65 7261   enabled (camera
+0000e000: 2077 696c 6c20 7072 6f64 7563 6520 7370   will produce sp
+0000e010: 6561 6b69 6e67 2073 6d61 7274 0a20 2020  eaking smart.   
+0000e020: 2020 2020 2064 6574 6563 7469 6f6e 2065       detection e
+0000e030: 7665 6e74 7329 3f0a 2020 2020 2020 2020  vents)?.        
+0000e040: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000e050: 7572 6e20 7365 6c66 2e5f 6973 5f61 7564  urn self._is_aud
+0000e060: 696f 5f65 6e61 626c 6564 2853 6d61 7274  io_enabled(Smart
+0000e070: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000e080: 2e53 5045 414b 290a 0a20 2020 2040 7072  .SPEAK)..    @pr
+0000e090: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+0000e0a0: 6173 745f 7370 6561 6b69 6e67 5f64 6574  ast_speaking_det
+0000e0b0: 6563 745f 6576 656e 7428 7365 6c66 2920  ect_event(self) 
+0000e0c0: 2d3e 204f 7074 696f 6e61 6c5b 4576 656e  -> Optional[Even
+0000e0d0: 745d 3a0a 2020 2020 2020 2020 2222 2247  t]:.        """G
+0000e0e0: 6574 2074 6865 206c 6173 7420 5370 6561  et the last Spea
+0000e0f0: 6b69 6e67 2073 6d61 7274 2064 6574 6563  king smart detec
+0000e100: 7469 6f6e 2065 7665 6e74 2e22 2222 0a0a  tion event."""..
+0000e110: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000e120: 656c 662e 6765 745f 6c61 7374 5f73 6d61  elf.get_last_sma
+0000e130: 7274 5f61 7564 696f 5f64 6574 6563 745f  rt_audio_detect_
+0000e140: 6576 656e 7428 536d 6172 7444 6574 6563  event(SmartDetec
+0000e150: 7441 7564 696f 5479 7065 2e53 5045 414b  tAudioType.SPEAK
+0000e160: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000e170: 0a20 2020 2064 6566 206c 6173 745f 7370  .    def last_sp
+0000e180: 6561 6b69 6e67 5f64 6574 6563 7428 7365  eaking_detect(se
+0000e190: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000e1a0: 6461 7465 7469 6d65 5d3a 0a20 2020 2020  datetime]:.     
+0000e1b0: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
+0000e1c0: 7374 2053 7065 616b 696e 6720 736d 6172  st Speaking smar
+0000e1d0: 7420 6465 7465 6374 696f 6e20 6576 656e  t detection even
+0000e1e0: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
+0000e1f0: 6574 7572 6e20 7365 6c66 2e6c 6173 745f  eturn self.last_
+0000e200: 736d 6172 745f 6175 6469 6f5f 6465 7465  smart_audio_dete
+0000e210: 6374 732e 6765 7428 536d 6172 7444 6574  cts.get(SmartDet
+0000e220: 6563 7441 7564 696f 5479 7065 2e53 5045  ectAudioType.SPE
+0000e230: 414b 290a 0a20 2020 2040 7072 6f70 6572  AK)..    @proper
+0000e240: 7479 0a20 2020 2064 6566 2069 735f 7370  ty.    def is_sp
+0000e250: 6561 6b69 6e67 5f63 7572 7265 6e74 6c79  eaking_currently
+0000e260: 5f64 6574 6563 7465 6428 7365 6c66 2920  _detected(self) 
+0000e270: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000e280: 2022 2222 4973 2053 7065 616b 696e 6720   """Is Speaking 
+0000e290: 6375 7272 656e 746c 7920 6265 696e 6720  currently being 
+0000e2a0: 6465 7465 6374 6564 2222 220a 0a20 2020  detected"""..   
+0000e2b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000e2c0: 2e5f 6973 5f61 7564 696f 5f64 6574 6563  ._is_audio_detec
+0000e2d0: 7465 6428 536d 6172 7444 6574 6563 744f  ted(SmartDetectO
+0000e2e0: 626a 6563 7454 7970 652e 5350 4541 4b29  bjectType.SPEAK)
+0000e2f0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0000e300: 7365 745f 7370 6561 6b69 6e67 5f64 6574  set_speaking_det
+0000e310: 6563 7469 6f6e 2873 656c 662c 2065 6e61  ection(self, ena
+0000e320: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+0000e330: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000e340: 546f 6767 6c65 7320 7370 6561 6b69 6e67  Toggles speaking
+0000e350: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000e360: 2e20 5265 7175 6972 6573 2063 616d 6572  . Requires camer
+0000e370: 6120 746f 2068 6176 6520 736d 6172 7420  a to have smart 
+0000e380: 6465 7465 6374 696f 6e22 2222 0a0a 2020  detection"""..  
+0000e390: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0000e3a0: 6974 2073 656c 662e 5f73 6574 5f61 7564  it self._set_aud
+0000e3b0: 696f 5f64 6574 6563 7428 536d 6172 7444  io_detect(SmartD
+0000e3c0: 6574 6563 7441 7564 696f 5479 7065 2e53  etectAudioType.S
+0000e3d0: 5045 414b 2c20 656e 6162 6c65 6429 0a0a  PEAK, enabled)..
+0000e3e0: 2020 2020 2320 656e 6472 6567 696f 6e0a      # endregion.
+0000e3f0: 2020 2020 2320 7265 6769 6f6e 2042 6172      # region Bar
+0000e400: 6b0a 0a20 2020 2040 7072 6f70 6572 7479  k..    @property
+0000e410: 0a20 2020 2064 6566 2063 616e 5f64 6574  .    def can_det
+0000e420: 6563 745f 6261 726b 2873 656c 6629 202d  ect_bark(self) -
+0000e430: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000e440: 7265 7475 726e 2073 656c 662e 5f63 616e  return self._can
+0000e450: 5f64 6574 6563 745f 6175 6469 6f28 536d  _detect_audio(Sm
+0000e460: 6172 7444 6574 6563 744f 626a 6563 7454  artDetectObjectT
+0000e470: 7970 652e 4241 524b 290a 0a20 2020 2040  ype.BARK)..    @
+0000e480: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000e490: 2069 735f 6261 726b 5f64 6574 6563 7469   is_bark_detecti
+0000e4a0: 6f6e 5f6f 6e28 7365 6c66 2920 2d3e 2062  on_on(self) -> b
+0000e4b0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0000e4c0: 4973 2042 6172 6b20 4465 7465 6374 696f  Is Bark Detectio
+0000e4d0: 6e20 6176 6169 6c61 626c 6520 616e 6420  n available and 
+0000e4e0: 656e 6162 6c65 6420 2863 616d 6572 6120  enabled (camera 
+0000e4f0: 7769 6c6c 2070 726f 6475 6365 2062 6172  will produce bar
+0000e500: 6b69 6e67 2073 6d61 7274 0a20 2020 2020  king smart.     
+0000e510: 2020 2064 6574 6563 7469 6f6e 2065 7665     detection eve
+0000e520: 6e74 7329 3f0a 2020 2020 2020 2020 2222  nts)?.        ""
+0000e530: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000e540: 6e20 7365 6c66 2e5f 6973 5f61 7564 696f  n self._is_audio
+0000e550: 5f65 6e61 626c 6564 2853 6d61 7274 4465  _enabled(SmartDe
+0000e560: 7465 6374 4f62 6a65 6374 5479 7065 2e42  tectObjectType.B
+0000e570: 4152 4b29 0a0a 2020 2020 4070 726f 7065  ARK)..    @prope
+0000e580: 7274 790a 2020 2020 6465 6620 6c61 7374  rty.    def last
+0000e590: 5f62 6172 6b5f 6465 7465 6374 5f65 7665  _bark_detect_eve
+0000e5a0: 6e74 2873 656c 6629 202d 3e20 4f70 7469  nt(self) -> Opti
+0000e5b0: 6f6e 616c 5b45 7665 6e74 5d3a 0a20 2020  onal[Event]:.   
+0000e5c0: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+0000e5d0: 6c61 7374 2042 6172 6b20 736d 6172 7420  last Bark smart 
+0000e5e0: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
+0000e5f0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000e600: 7572 6e20 7365 6c66 2e67 6574 5f6c 6173  urn self.get_las
+0000e610: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
+0000e620: 7465 6374 5f65 7665 6e74 2853 6d61 7274  tect_event(Smart
+0000e630: 4465 7465 6374 4175 6469 6f54 7970 652e  DetectAudioType.
+0000e640: 4241 524b 290a 0a20 2020 2040 7072 6f70  BARK)..    @prop
+0000e650: 6572 7479 0a20 2020 2064 6566 206c 6173  erty.    def las
+0000e660: 745f 6261 726b 5f64 6574 6563 7428 7365  t_bark_detect(se
+0000e670: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000e680: 6461 7465 7469 6d65 5d3a 0a20 2020 2020  datetime]:.     
+0000e690: 2020 2022 2222 4765 7420 7468 6520 6c61     """Get the la
+0000e6a0: 7374 2042 6172 6b20 736d 6172 7420 6465  st Bark smart de
+0000e6b0: 7465 6374 696f 6e20 6576 656e 742e 2222  tection event.""
+0000e6c0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000e6d0: 6e20 7365 6c66 2e6c 6173 745f 736d 6172  n self.last_smar
+0000e6e0: 745f 6175 6469 6f5f 6465 7465 6374 732e  t_audio_detects.
+0000e6f0: 6765 7428 536d 6172 7444 6574 6563 7441  get(SmartDetectA
+0000e700: 7564 696f 5479 7065 2e42 4152 4b29 0a0a  udioType.BARK)..
+0000e710: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000e720: 2020 6465 6620 6973 5f62 6172 6b5f 6375    def is_bark_cu
+0000e730: 7272 656e 746c 795f 6465 7465 6374 6564  rrently_detected
+0000e740: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000e750: 2020 2020 2020 2020 2222 2249 7320 4261          """Is Ba
+0000e760: 726b 2063 7572 7265 6e74 6c79 2062 6569  rk currently bei
+0000e770: 6e67 2064 6574 6563 7465 6422 2222 0a0a  ng detected"""..
+0000e780: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000e790: 656c 662e 5f69 735f 6175 6469 6f5f 6465  elf._is_audio_de
+0000e7a0: 7465 6374 6564 2853 6d61 7274 4465 7465  tected(SmartDete
+0000e7b0: 6374 4f62 6a65 6374 5479 7065 2e42 4152  ctObjectType.BAR
+0000e7c0: 4b29 0a0a 2020 2020 6173 796e 6320 6465  K)..    async de
+0000e7d0: 6620 7365 745f 6261 726b 5f64 6574 6563  f set_bark_detec
+0000e7e0: 7469 6f6e 2873 656c 662c 2065 6e61 626c  tion(self, enabl
+0000e7f0: 6564 3a20 626f 6f6c 2920 2d3e 204e 6f6e  ed: bool) -> Non
+0000e800: 653a 0a20 2020 2020 2020 2022 2222 546f  e:.        """To
+0000e810: 6767 6c65 7320 6261 726b 2073 6d61 7274  ggles bark smart
+0000e820: 2064 6574 6563 7469 6f6e 2e20 5265 7175   detection. Requ
+0000e830: 6972 6573 2063 616d 6572 6120 746f 2068  ires camera to h
+0000e840: 6176 6520 736d 6172 7420 6465 7465 6374  ave smart detect
+0000e850: 696f 6e22 2222 0a0a 2020 2020 2020 2020  ion"""..        
+0000e860: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+0000e870: 662e 5f73 6574 5f61 7564 696f 5f64 6574  f._set_audio_det
+0000e880: 6563 7428 536d 6172 7444 6574 6563 7441  ect(SmartDetectA
+0000e890: 7564 696f 5479 7065 2e42 4152 4b2c 2065  udioType.BARK, e
+0000e8a0: 6e61 626c 6564 290a 0a20 2020 2023 2065  nabled)..    # e
+0000e8b0: 6e64 7265 6769 6f6e 0a20 2020 2023 2072  ndregion.    # r
+0000e8c0: 6567 696f 6e20 4361 7220 416c 6172 6d0a  egion Car Alarm.
+0000e8d0: 2020 2020 2320 2862 7572 676c 6172 2069      # (burglar i
+0000e8e0: 6e20 636f 6465 2c20 6361 7220 616c 6172  n code, car alar
+0000e8f0: 6d20 696e 2050 726f 7465 6374 2055 4929  m in Protect UI)
+0000e900: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000e910: 2020 2020 6465 6620 6361 6e5f 6465 7465      def can_dete
+0000e920: 6374 5f63 6172 5f61 6c61 726d 2873 656c  ct_car_alarm(sel
+0000e930: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+0000e940: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000e950: 5f63 616e 5f64 6574 6563 745f 6175 6469  _can_detect_audi
+0000e960: 6f28 536d 6172 7444 6574 6563 744f 626a  o(SmartDetectObj
+0000e970: 6563 7454 7970 652e 4255 5247 4c41 5229  ectType.BURGLAR)
+0000e980: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000e990: 2020 2020 6465 6620 6973 5f63 6172 5f61      def is_car_a
+0000e9a0: 6c61 726d 5f64 6574 6563 7469 6f6e 5f6f  larm_detection_o
+0000e9b0: 6e28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  n(self) -> bool:
+0000e9c0: 0a20 2020 2020 2020 2022 2222 4973 2043  .        """Is C
+0000e9d0: 6172 2041 6c61 726d 2044 6574 6563 7469  ar Alarm Detecti
+0000e9e0: 6f6e 2061 7661 696c 6162 6c65 2061 6e64  on available and
+0000e9f0: 2065 6e61 626c 6564 2028 6361 6d65 7261   enabled (camera
+0000ea00: 2077 696c 6c20 7072 6f64 7563 6520 6361   will produce ca
+0000ea10: 7220 616c 6172 6d20 736d 6172 740a 2020  r alarm smart.  
+0000ea20: 2020 2020 2020 6465 7465 6374 696f 6e20        detection 
+0000ea30: 6576 656e 7473 293f 0a20 2020 2020 2020  events)?.       
+0000ea40: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+0000ea50: 7475 726e 2073 656c 662e 5f69 735f 6175  turn self._is_au
+0000ea60: 6469 6f5f 656e 6162 6c65 6428 536d 6172  dio_enabled(Smar
+0000ea70: 7444 6574 6563 744f 626a 6563 7454 7970  tDetectObjectTyp
+0000ea80: 652e 4255 5247 4c41 5229 0a0a 2020 2020  e.BURGLAR)..    
+0000ea90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000eaa0: 6620 6c61 7374 5f63 6172 5f61 6c61 726d  f last_car_alarm
+0000eab0: 5f64 6574 6563 745f 6576 656e 7428 7365  _detect_event(se
+0000eac0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000ead0: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
+0000eae0: 2222 2247 6574 2074 6865 206c 6173 7420  """Get the last 
+0000eaf0: 4361 7220 416c 6172 6d20 736d 6172 7420  Car Alarm smart 
+0000eb00: 6465 7465 6374 696f 6e20 6576 656e 742e  detection event.
+0000eb10: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000eb20: 7572 6e20 7365 6c66 2e67 6574 5f6c 6173  urn self.get_las
+0000eb30: 745f 736d 6172 745f 6175 6469 6f5f 6465  t_smart_audio_de
+0000eb40: 7465 6374 5f65 7665 6e74 2853 6d61 7274  tect_event(Smart
+0000eb50: 4465 7465 6374 4175 6469 6f54 7970 652e  DetectAudioType.
+0000eb60: 4255 5247 4c41 5229 0a0a 2020 2020 4070  BURGLAR)..    @p
+0000eb70: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000eb80: 6c61 7374 5f63 6172 5f61 6c61 726d 5f64  last_car_alarm_d
+0000eb90: 6574 6563 7428 7365 6c66 2920 2d3e 204f  etect(self) -> O
+0000eba0: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
+0000ebb0: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
+0000ebc0: 7420 7468 6520 6c61 7374 2043 6172 2041  t the last Car A
+0000ebd0: 6c61 726d 2073 6d61 7274 2064 6574 6563  larm smart detec
+0000ebe0: 7469 6f6e 2065 7665 6e74 2e22 2222 0a0a  tion event."""..
+0000ebf0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000ec00: 656c 662e 6c61 7374 5f73 6d61 7274 5f61  elf.last_smart_a
+0000ec10: 7564 696f 5f64 6574 6563 7473 2e67 6574  udio_detects.get
+0000ec20: 2853 6d61 7274 4465 7465 6374 4175 6469  (SmartDetectAudi
+0000ec30: 6f54 7970 652e 4255 5247 4c41 5229 0a0a  oType.BURGLAR)..
+0000ec40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000ec50: 2020 6465 6620 6973 5f63 6172 5f61 6c61    def is_car_ala
+0000ec60: 726d 5f63 7572 7265 6e74 6c79 5f64 6574  rm_currently_det
+0000ec70: 6563 7465 6428 7365 6c66 2920 2d3e 2062  ected(self) -> b
+0000ec80: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0000ec90: 4973 2043 6172 2041 6c61 726d 2063 7572  Is Car Alarm cur
+0000eca0: 7265 6e74 6c79 2062 6569 6e67 2064 6574  rently being det
+0000ecb0: 6563 7465 6422 2222 0a0a 2020 2020 2020  ected"""..      
+0000ecc0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
+0000ecd0: 735f 6175 6469 6f5f 6465 7465 6374 6564  s_audio_detected
+0000ece0: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000ecf0: 6374 5479 7065 2e42 5552 474c 4152 290a  ctType.BURGLAR).
+0000ed00: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
+0000ed10: 6574 5f63 6172 5f61 6c61 726d 5f64 6574  et_car_alarm_det
+0000ed20: 6563 7469 6f6e 2873 656c 662c 2065 6e61  ection(self, ena
+0000ed30: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+0000ed40: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000ed50: 546f 6767 6c65 7320 6361 725f 616c 6172  Toggles car_alar
+0000ed60: 6d20 736d 6172 7420 6465 7465 6374 696f  m smart detectio
+0000ed70: 6e2e 2052 6571 7569 7265 7320 6361 6d65  n. Requires came
+0000ed80: 7261 2074 6f20 6861 7665 2073 6d61 7274  ra to have smart
+0000ed90: 2064 6574 6563 7469 6f6e 2222 220a 0a20   detection""".. 
+0000eda0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+0000edb0: 6169 7420 7365 6c66 2e5f 7365 745f 6175  ait self._set_au
+0000edc0: 6469 6f5f 6465 7465 6374 2853 6d61 7274  dio_detect(Smart
+0000edd0: 4465 7465 6374 4175 6469 6f54 7970 652e  DetectAudioType.
+0000ede0: 4255 5247 4c41 522c 2065 6e61 626c 6564  BURGLAR, enabled
+0000edf0: 290a 0a20 2020 2023 2065 6e64 7265 6769  )..    # endregi
+0000ee00: 6f6e 0a20 2020 2023 2072 6567 696f 6e20  on.    # region 
+0000ee10: 4361 7220 486f 726e 0a0a 2020 2020 4070  Car Horn..    @p
+0000ee20: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000ee30: 6361 6e5f 6465 7465 6374 5f63 6172 5f68  can_detect_car_h
+0000ee40: 6f72 6e28 7365 6c66 2920 2d3e 2062 6f6f  orn(self) -> boo
+0000ee50: 6c3a 0a20 2020 2020 2020 2072 6574 7572  l:.        retur
+0000ee60: 6e20 7365 6c66 2e5f 6361 6e5f 6465 7465  n self._can_dete
+0000ee70: 6374 5f61 7564 696f 2853 6d61 7274 4465  ct_audio(SmartDe
+0000ee80: 7465 6374 4f62 6a65 6374 5479 7065 2e43  tectObjectType.C
+0000ee90: 4152 5f48 4f52 4e29 0a0a 2020 2020 4070  AR_HORN)..    @p
+0000eea0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000eeb0: 6973 5f63 6172 5f68 6f72 6e5f 6465 7465  is_car_horn_dete
+0000eec0: 6374 696f 6e5f 6f6e 2873 656c 6629 202d  ction_on(self) -
+0000eed0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000eee0: 2222 2249 7320 4361 7220 486f 726e 2044  """Is Car Horn D
+0000eef0: 6574 6563 7469 6f6e 2061 7661 696c 6162  etection availab
+0000ef00: 6c65 2061 6e64 2065 6e61 626c 6564 2028  le and enabled (
+0000ef10: 6361 6d65 7261 2077 696c 6c20 7072 6f64  camera will prod
+0000ef20: 7563 6520 6361 7220 686f 726e 2073 6d61  uce car horn sma
+0000ef30: 7274 0a20 2020 2020 2020 2064 6574 6563  rt.        detec
+0000ef40: 7469 6f6e 2065 7665 6e74 7329 3f0a 2020  tion events)?.  
+0000ef50: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000ef60: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000ef70: 6973 5f61 7564 696f 5f65 6e61 626c 6564  is_audio_enabled
+0000ef80: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000ef90: 6374 5479 7065 2e43 4152 5f48 4f52 4e29  ctType.CAR_HORN)
+0000efa0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000efb0: 2020 2020 6465 6620 6c61 7374 5f63 6172      def last_car
+0000efc0: 5f68 6f72 6e5f 6465 7465 6374 5f65 7665  _horn_detect_eve
+0000efd0: 6e74 2873 656c 6629 202d 3e20 4f70 7469  nt(self) -> Opti
+0000efe0: 6f6e 616c 5b45 7665 6e74 5d3a 0a20 2020  onal[Event]:.   
+0000eff0: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+0000f000: 6c61 7374 2043 6172 2048 6f72 6e20 736d  last Car Horn sm
+0000f010: 6172 7420 6465 7465 6374 696f 6e20 6576  art detection ev
+0000f020: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
+0000f030: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+0000f040: 5f6c 6173 745f 736d 6172 745f 6175 6469  _last_smart_audi
+0000f050: 6f5f 6465 7465 6374 5f65 7665 6e74 2853  o_detect_event(S
+0000f060: 6d61 7274 4465 7465 6374 4175 6469 6f54  martDetectAudioT
+0000f070: 7970 652e 4341 525f 484f 524e 290a 0a20  ype.CAR_HORN).. 
+0000f080: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000f090: 2064 6566 206c 6173 745f 6361 725f 686f   def last_car_ho
+0000f0a0: 726e 5f64 6574 6563 7428 7365 6c66 2920  rn_detect(self) 
+0000f0b0: 2d3e 204f 7074 696f 6e61 6c5b 6461 7465  -> Optional[date
+0000f0c0: 7469 6d65 5d3a 0a20 2020 2020 2020 2022  time]:.        "
+0000f0d0: 2222 4765 7420 7468 6520 6c61 7374 2043  ""Get the last C
+0000f0e0: 6172 2048 6f72 6e20 736d 6172 7420 6465  ar Horn smart de
+0000f0f0: 7465 6374 696f 6e20 6576 656e 742e 2222  tection event.""
+0000f100: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000f110: 6e20 7365 6c66 2e6c 6173 745f 736d 6172  n self.last_smar
+0000f120: 745f 6175 6469 6f5f 6465 7465 6374 732e  t_audio_detects.
+0000f130: 6765 7428 536d 6172 7444 6574 6563 7441  get(SmartDetectA
+0000f140: 7564 696f 5479 7065 2e43 4152 5f48 4f52  udioType.CAR_HOR
+0000f150: 4e29 0a0a 2020 2020 4070 726f 7065 7274  N)..    @propert
+0000f160: 790a 2020 2020 6465 6620 6973 5f63 6172  y.    def is_car
+0000f170: 5f68 6f72 6e5f 6375 7272 656e 746c 795f  _horn_currently_
+0000f180: 6465 7465 6374 6564 2873 656c 6629 202d  detected(self) -
+0000f190: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000f1a0: 2222 2249 7320 4361 7220 486f 726e 2063  """Is Car Horn c
+0000f1b0: 7572 7265 6e74 6c79 2062 6569 6e67 2064  urrently being d
+0000f1c0: 6574 6563 7465 6422 2222 0a0a 2020 2020  etected"""..    
+0000f1d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000f1e0: 5f69 735f 6175 6469 6f5f 6465 7465 6374  _is_audio_detect
+0000f1f0: 6564 2853 6d61 7274 4465 7465 6374 4f62  ed(SmartDetectOb
+0000f200: 6a65 6374 5479 7065 2e43 4152 5f48 4f52  jectType.CAR_HOR
+0000f210: 4e29 0a0a 2020 2020 6173 796e 6320 6465  N)..    async de
+0000f220: 6620 7365 745f 6361 725f 686f 726e 5f64  f set_car_horn_d
+0000f230: 6574 6563 7469 6f6e 2873 656c 662c 2065  etection(self, e
+0000f240: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
+0000f250: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000f260: 2222 546f 6767 6c65 7320 6361 725f 686f  ""Toggles car_ho
+0000f270: 726e 2073 6d61 7274 2064 6574 6563 7469  rn smart detecti
+0000f280: 6f6e 2e20 5265 7175 6972 6573 2063 616d  on. Requires cam
+0000f290: 6572 6120 746f 2068 6176 6520 736d 6172  era to have smar
+0000f2a0: 7420 6465 7465 6374 696f 6e22 2222 0a0a  t detection"""..
+0000f2b0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0000f2c0: 7761 6974 2073 656c 662e 5f73 6574 5f61  wait self._set_a
+0000f2d0: 7564 696f 5f64 6574 6563 7428 536d 6172  udio_detect(Smar
+0000f2e0: 7444 6574 6563 7441 7564 696f 5479 7065  tDetectAudioType
+0000f2f0: 2e43 4152 5f48 4f52 4e2c 2065 6e61 626c  .CAR_HORN, enabl
+0000f300: 6564 290a 0a20 2020 2023 2065 6e64 7265  ed)..    # endre
+0000f310: 6769 6f6e 0a20 2020 2023 2072 6567 696f  gion.    # regio
+0000f320: 6e20 476c 6173 7320 4272 6561 6b0a 0a20  n Glass Break.. 
+0000f330: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000f340: 2064 6566 2063 616e 5f64 6574 6563 745f   def can_detect_
+0000f350: 676c 6173 735f 6272 6561 6b28 7365 6c66  glass_break(self
+0000f360: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000f370: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000f380: 6361 6e5f 6465 7465 6374 5f61 7564 696f  can_detect_audio
+0000f390: 2853 6d61 7274 4465 7465 6374 4f62 6a65  (SmartDetectObje
+0000f3a0: 6374 5479 7065 2e47 4c41 5353 5f42 5245  ctType.GLASS_BRE
+0000f3b0: 414b 290a 0a20 2020 2040 7072 6f70 6572  AK)..    @proper
+0000f3c0: 7479 0a20 2020 2064 6566 2069 735f 676c  ty.    def is_gl
+0000f3d0: 6173 735f 6272 6561 6b5f 6465 7465 6374  ass_break_detect
+0000f3e0: 696f 6e5f 6f6e 2873 656c 6629 202d 3e20  ion_on(self) -> 
+0000f3f0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+0000f400: 2249 7320 476c 6173 7320 4272 6561 6b20  "Is Glass Break 
+0000f410: 6176 6169 6c61 626c 6520 616e 6420 656e  available and en
+0000f420: 6162 6c65 6420 2863 616d 6572 6120 7769  abled (camera wi
+0000f430: 6c6c 2070 726f 6475 6365 2067 6c61 7373  ll produce glass
+0000f440: 2062 7265 616b 2073 6d61 7274 0a20 2020   break smart.   
+0000f450: 2020 2020 2064 6574 6563 7469 6f6e 2065       detection e
+0000f460: 7665 6e74 7329 3f0a 2020 2020 2020 2020  vents)?.        
+0000f470: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+0000f480: 7572 6e20 7365 6c66 2e5f 6973 5f61 7564  urn self._is_aud
+0000f490: 696f 5f65 6e61 626c 6564 2853 6d61 7274  io_enabled(Smart
+0000f4a0: 4465 7465 6374 4f62 6a65 6374 5479 7065  DetectObjectType
+0000f4b0: 2e47 4c41 5353 5f42 5245 414b 290a 0a20  .GLASS_BREAK).. 
+0000f4c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000f4d0: 2064 6566 206c 6173 745f 676c 6173 735f   def last_glass_
+0000f4e0: 6272 6561 6b5f 6465 7465 6374 5f65 7665  break_detect_eve
+0000f4f0: 6e74 2873 656c 6629 202d 3e20 4f70 7469  nt(self) -> Opti
+0000f500: 6f6e 616c 5b45 7665 6e74 5d3a 0a20 2020  onal[Event]:.   
+0000f510: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+0000f520: 6c61 7374 2047 6c61 7373 2042 7265 616b  last Glass Break
+0000f530: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000f540: 2065 7665 6e74 2e22 2222 0a0a 2020 2020   event."""..    
+0000f550: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000f560: 6765 745f 6c61 7374 5f73 6d61 7274 5f61  get_last_smart_a
+0000f570: 7564 696f 5f64 6574 6563 745f 6576 656e  udio_detect_even
+0000f580: 7428 536d 6172 7444 6574 6563 7441 7564  t(SmartDetectAud
+0000f590: 696f 5479 7065 2e47 4c41 5353 5f42 5245  ioType.GLASS_BRE
+0000f5a0: 414b 290a 0a20 2020 2040 7072 6f70 6572  AK)..    @proper
+0000f5b0: 7479 0a20 2020 2064 6566 206c 6173 745f  ty.    def last_
+0000f5c0: 676c 6173 735f 6272 6561 6b5f 6465 7465  glass_break_dete
+0000f5d0: 6374 2873 656c 6629 202d 3e20 4f70 7469  ct(self) -> Opti
+0000f5e0: 6f6e 616c 5b64 6174 6574 696d 655d 3a0a  onal[datetime]:.
+0000f5f0: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+0000f600: 6865 206c 6173 7420 476c 6173 7320 4272  he last Glass Br
+0000f610: 6561 6b20 736d 6172 7420 6465 7465 6374  eak smart detect
+0000f620: 696f 6e20 6576 656e 742e 2222 220a 0a20  ion event.""".. 
+0000f630: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000f640: 6c66 2e6c 6173 745f 736d 6172 745f 6175  lf.last_smart_au
+0000f650: 6469 6f5f 6465 7465 6374 732e 6765 7428  dio_detects.get(
+0000f660: 536d 6172 7444 6574 6563 7441 7564 696f  SmartDetectAudio
+0000f670: 5479 7065 2e47 4c41 5353 5f42 5245 414b  Type.GLASS_BREAK
+0000f680: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000f690: 0a20 2020 2064 6566 2069 735f 676c 6173  .    def is_glas
+0000f6a0: 735f 6272 6561 6b5f 6375 7272 656e 746c  s_break_currentl
+0000f6b0: 795f 6465 7465 6374 6564 2873 656c 6629  y_detected(self)
+0000f6c0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+0000f6d0: 2020 2222 2249 7320 476c 6173 7320 4272    """Is Glass Br
+0000f6e0: 6561 6b20 6375 7272 656e 746c 7920 6265  eak currently be
+0000f6f0: 696e 6720 6465 7465 6374 6564 2222 220a  ing detected""".
+0000f700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f710: 7365 6c66 2e5f 6973 5f61 7564 696f 5f64  self._is_audio_d
+0000f720: 6574 6563 7465 6428 536d 6172 7444 6574  etected(SmartDet
+0000f730: 6563 744f 626a 6563 7454 7970 652e 474c  ectObjectType.GL
+0000f740: 4153 535f 4252 4541 4b29 0a0a 2020 2020  ASS_BREAK)..    
+0000f750: 6173 796e 6320 6465 6620 7365 745f 676c  async def set_gl
+0000f760: 6173 735f 6272 6561 6b5f 6465 7465 6374  ass_break_detect
+0000f770: 696f 6e28 7365 6c66 2c20 656e 6162 6c65  ion(self, enable
+0000f780: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
+0000f790: 3a0a 2020 2020 2020 2020 2222 2254 6f67  :.        """Tog
+0000f7a0: 676c 6573 2067 6c61 7373 5f62 7265 616b  gles glass_break
+0000f7b0: 2073 6d61 7274 2064 6574 6563 7469 6f6e   smart detection
+0000f7c0: 2e20 5265 7175 6972 6573 2063 616d 6572  . Requires camer
+0000f7d0: 6120 746f 2068 6176 6520 736d 6172 7420  a to have smart 
+0000f7e0: 6465 7465 6374 696f 6e22 2222 0a0a 2020  detection"""..  
+0000f7f0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0000f800: 6974 2073 656c 662e 5f73 6574 5f61 7564  it self._set_aud
+0000f810: 696f 5f64 6574 6563 7428 536d 6172 7444  io_detect(SmartD
+0000f820: 6574 6563 7441 7564 696f 5479 7065 2e47  etectAudioType.G
+0000f830: 4c41 5353 5f42 5245 414b 2c20 656e 6162  LASS_BREAK, enab
+0000f840: 6c65 6429 0a0a 2020 2020 2320 656e 6472  led)..    # endr
+0000f850: 6567 696f 6e0a 2020 2020 2320 656e 6472  egion.    # endr
+0000f860: 6567 696f 6e0a 0a20 2020 2040 7072 6f70  egion..    @prop
+0000f870: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
+0000f880: 7269 6e67 696e 6728 7365 6c66 2920 2d3e  ringing(self) ->
+0000f890: 2062 6f6f 6c3a 0a20 2020 2020 2020 2069   bool:.        i
+0000f8a0: 6620 7365 6c66 2e5f 6c61 7374 5f72 696e  f self._last_rin
+0000f8b0: 675f 7469 6d65 6f75 7420 6973 204e 6f6e  g_timeout is Non
+0000f8c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000f8d0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000f8e0: 2020 2020 7265 7475 726e 2075 7463 5f6e      return utc_n
+0000f8f0: 6f77 2829 203c 2073 656c 662e 5f6c 6173  ow() < self._las
+0000f900: 745f 7269 6e67 5f74 696d 656f 7574 0a0a  t_ring_timeout..
+0000f910: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000f920: 2020 6465 6620 6368 696d 655f 7479 7065    def chime_type
+0000f930: 2873 656c 6629 202d 3e20 4368 696d 6554  (self) -> ChimeT
+0000f940: 7970 653a 0a20 2020 2020 2020 2069 6620  ype:.        if 
+0000f950: 7365 6c66 2e63 6869 6d65 5f64 7572 6174  self.chime_durat
+0000f960: 696f 6e2e 746f 7461 6c5f 7365 636f 6e64  ion.total_second
+0000f970: 7328 2920 3d3d 2030 2e33 3a0a 2020 2020  s() == 0.3:.    
+0000f980: 2020 2020 2020 2020 7265 7475 726e 2043          return C
+0000f990: 6869 6d65 5479 7065 2e4d 4543 4841 4e49  himeType.MECHANI
+0000f9a0: 4341 4c0a 2020 2020 2020 2020 6966 2073  CAL.        if s
+0000f9b0: 656c 662e 6368 696d 655f 6475 7261 7469  elf.chime_durati
+0000f9c0: 6f6e 2e74 6f74 616c 5f73 6563 6f6e 6473  on.total_seconds
+0000f9d0: 2829 203e 2030 2e33 3a0a 2020 2020 2020  () > 0.3:.      
+0000f9e0: 2020 2020 2020 7265 7475 726e 2043 6869        return Chi
+0000f9f0: 6d65 5479 7065 2e44 4947 4954 414c 0a20  meType.DIGITAL. 
+0000fa00: 2020 2020 2020 2072 6574 7572 6e20 4368         return Ch
+0000fa10: 696d 6554 7970 652e 4e4f 4e45 0a0a 2020  imeType.NONE..  
+0000fa20: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000fa30: 6465 6620 6973 5f64 6967 6974 616c 5f63  def is_digital_c
+0000fa40: 6869 6d65 2873 656c 6629 202d 3e20 626f  hime(self) -> bo
+0000fa50: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
+0000fa60: 726e 2073 656c 662e 6368 696d 655f 7479  rn self.chime_ty
+0000fa70: 7065 2069 7320 4368 696d 6554 7970 652e  pe is ChimeType.
+0000fa80: 4449 4749 5441 4c0a 0a20 2020 2040 7072  DIGITAL..    @pr
+0000fa90: 6f70 6572 7479 0a20 2020 2064 6566 2068  operty.    def h
+0000faa0: 6967 685f 6361 6d65 7261 5f63 6861 6e6e  igh_camera_chann
+0000fab0: 656c 2873 656c 6629 202d 3e20 4f70 7469  el(self) -> Opti
+0000fac0: 6f6e 616c 5b43 616d 6572 6143 6861 6e6e  onal[CameraChann
+0000fad0: 656c 5d3a 0a20 2020 2020 2020 2069 6620  el]:.        if 
+0000fae0: 6c65 6e28 7365 6c66 2e63 6861 6e6e 656c  len(self.channel
+0000faf0: 7329 203e 3d20 333a 0a20 2020 2020 2020  s) >= 3:.       
+0000fb00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000fb10: 2e63 6861 6e6e 656c 735b 305d 0a20 2020  .channels[0].   
+0000fb20: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000fb30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000fb40: 2020 2020 6465 6620 6d65 6469 756d 5f63      def medium_c
+0000fb50: 616d 6572 615f 6368 616e 6e65 6c28 7365  amera_channel(se
+0000fb60: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000fb70: 4361 6d65 7261 4368 616e 6e65 6c5d 3a0a  CameraChannel]:.
+0000fb80: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+0000fb90: 656c 662e 6368 616e 6e65 6c73 2920 3e3d  elf.channels) >=
+0000fba0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+0000fbb0: 7265 7475 726e 2073 656c 662e 6368 616e  return self.chan
+0000fbc0: 6e65 6c73 5b31 5d0a 2020 2020 2020 2020  nels[1].        
+0000fbd0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000fbe0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000fbf0: 6566 206c 6f77 5f63 616d 6572 615f 6368  ef low_camera_ch
+0000fc00: 616e 6e65 6c28 7365 6c66 2920 2d3e 204f  annel(self) -> O
+0000fc10: 7074 696f 6e61 6c5b 4361 6d65 7261 4368  ptional[CameraCh
+0000fc20: 616e 6e65 6c5d 3a0a 2020 2020 2020 2020  annel]:.        
+0000fc30: 6966 206c 656e 2873 656c 662e 6368 616e  if len(self.chan
+0000fc40: 6e65 6c73 2920 3e3d 2033 3a0a 2020 2020  nels) >= 3:.    
+0000fc50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000fc60: 656c 662e 6368 616e 6e65 6c73 5b32 5d0a  elf.channels[2].
+0000fc70: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+0000fc80: 6f6e 650a 0a20 2020 2040 7072 6f70 6572  one..    @proper
+0000fc90: 7479 0a20 2020 2064 6566 2064 6566 6175  ty.    def defau
+0000fca0: 6c74 5f63 616d 6572 615f 6368 616e 6e65  lt_camera_channe
+0000fcb0: 6c28 7365 6c66 2920 2d3e 204f 7074 696f  l(self) -> Optio
+0000fcc0: 6e61 6c5b 4361 6d65 7261 4368 616e 6e65  nal[CameraChanne
+0000fcd0: 6c5d 3a0a 2020 2020 2020 2020 666f 7220  l]:.        for 
+0000fce0: 6368 616e 6e65 6c20 696e 205b 0a20 2020  channel in [.   
+0000fcf0: 2020 2020 2020 2020 2073 656c 662e 6869           self.hi
+0000fd00: 6768 5f63 616d 6572 615f 6368 616e 6e65  gh_camera_channe
+0000fd10: 6c2c 0a20 2020 2020 2020 2020 2020 2073  l,.            s
+0000fd20: 656c 662e 6d65 6469 756d 5f63 616d 6572  elf.medium_camer
+0000fd30: 615f 6368 616e 6e65 6c2c 0a20 2020 2020  a_channel,.     
+0000fd40: 2020 2020 2020 2073 656c 662e 6c6f 775f         self.low_
+0000fd50: 6361 6d65 7261 5f63 6861 6e6e 656c 2c0a  camera_channel,.
+0000fd60: 2020 2020 2020 2020 5d3a 0a20 2020 2020          ]:.     
+0000fd70: 2020 2020 2020 2069 6620 6368 616e 6e65         if channe
+0000fd80: 6c20 6973 206e 6f74 204e 6f6e 6520 616e  l is not None an
+0000fd90: 6420 6368 616e 6e65 6c2e 6973 5f72 7473  d channel.is_rts
+0000fda0: 705f 656e 6162 6c65 643a 0a20 2020 2020  p_enabled:.     
+0000fdb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fdc0: 6e20 6368 616e 6e65 6c0a 2020 2020 2020  n channel.      
+0000fdd0: 2020 7265 7475 726e 2073 656c 662e 6869    return self.hi
+0000fde0: 6768 5f63 616d 6572 615f 6368 616e 6e65  gh_camera_channe
+0000fdf0: 6c0a 0a20 2020 2040 7072 6f70 6572 7479  l..    @property
+0000fe00: 0a20 2020 2064 6566 2070 6163 6b61 6765  .    def package
+0000fe10: 5f63 616d 6572 615f 6368 616e 6e65 6c28  _camera_channel(
+0000fe20: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+0000fe30: 6c5b 4361 6d65 7261 4368 616e 6e65 6c5d  l[CameraChannel]
+0000fe40: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+0000fe50: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
+0000fe60: 6861 735f 7061 636b 6167 655f 6361 6d65  has_package_came
+0000fe70: 7261 2061 6e64 206c 656e 2873 656c 662e  ra and len(self.
+0000fe80: 6368 616e 6e65 6c73 2920 3d3d 2034 3a0a  channels) == 4:.
+0000fe90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fea0: 726e 2073 656c 662e 6368 616e 6e65 6c73  rn self.channels
+0000feb0: 5b33 5d0a 2020 2020 2020 2020 7265 7475  [3].        retu
+0000fec0: 726e 204e 6f6e 650a 0a20 2020 2040 7072  rn None..    @pr
+0000fed0: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
+0000fee0: 735f 6869 6768 5f66 7073 5f65 6e61 626c  s_high_fps_enabl
+0000fef0: 6564 2873 656c 6629 202d 3e20 626f 6f6c  ed(self) -> bool
+0000ff00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000ff10: 2073 656c 662e 7669 6465 6f5f 6d6f 6465   self.video_mode
+0000ff20: 203d 3d20 5669 6465 6f4d 6f64 652e 4849   == VideoMode.HI
+0000ff30: 4748 5f46 5053 0a0a 2020 2020 4070 726f  GH_FPS..    @pro
+0000ff40: 7065 7274 790a 2020 2020 6465 6620 6973  perty.    def is
+0000ff50: 5f76 6964 656f 5f72 6561 6479 2873 656c  _video_ready(sel
+0000ff60: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+0000ff70: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+0000ff80: 2020 2020 2020 2020 2073 656c 662e 6665           self.fe
+0000ff90: 6174 7572 655f 666c 6167 732e 6c65 6e73  ature_flags.lens
+0000ffa0: 5f74 7970 6520 6973 204e 6f6e 650a 2020  _type is None.  
+0000ffb0: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
+0000ffc0: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
+0000ffd0: 6c65 6e73 5f74 7970 6520 213d 204c 656e  lens_type != Len
+0000ffe0: 7354 7970 652e 4e4f 4e45 0a20 2020 2020  sType.NONE.     
+0000fff0: 2020 2029 0a0a 2020 2020 4070 726f 7065     )..    @prope
+00010000: 7274 790a 2020 2020 6465 6620 6861 735f  rty.    def has_
+00010010: 7265 6d6f 7661 626c 655f 6c65 6e73 2873  removable_lens(s
+00010020: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+00010030: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+00010040: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010050: 6665 6174 7572 655f 666c 6167 732e 686f  feature_flags.ho
+00010060: 7470 6c75 6720 6973 206e 6f74 204e 6f6e  tplug is not Non
+00010070: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+00010080: 6420 7365 6c66 2e66 6561 7475 7265 5f66  d self.feature_f
+00010090: 6c61 6773 2e68 6f74 706c 7567 2e76 6964  lags.hotplug.vid
+000100a0: 656f 2069 7320 6e6f 7420 4e6f 6e65 0a20  eo is not None. 
+000100b0: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
+000100c0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000100d0: 6861 735f 7265 6d6f 7661 626c 655f 7370  has_removable_sp
+000100e0: 6561 6b65 7228 7365 6c66 2920 2d3e 2062  eaker(self) -> b
+000100f0: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
+00010100: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+00010110: 2020 7365 6c66 2e66 6561 7475 7265 5f66    self.feature_f
+00010120: 6c61 6773 2e68 6f74 706c 7567 2069 7320  lags.hotplug is 
+00010130: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00010140: 2020 2020 2061 6e64 2073 656c 662e 6665       and self.fe
+00010150: 6174 7572 655f 666c 6167 732e 686f 7470  ature_flags.hotp
+00010160: 6c75 672e 6175 6469 6f20 6973 206e 6f74  lug.audio is not
+00010170: 204e 6f6e 650a 2020 2020 2020 2020 290a   None.        ).
+00010180: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00010190: 2020 2064 6566 2068 6173 5f6d 6963 2873     def has_mic(s
+000101a0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+000101b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000101c0: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
+000101d0: 6861 735f 6d69 6320 6f72 2073 656c 662e  has_mic or self.
+000101e0: 6861 735f 7265 6d6f 7661 626c 655f 7370  has_removable_sp
+000101f0: 6561 6b65 720a 0a20 2020 2040 7072 6f70  eaker..    @prop
+00010200: 6572 7479 0a20 2020 2064 6566 2068 6173  erty.    def has
+00010210: 5f63 6f6c 6f72 5f6e 6967 6874 5f76 6973  _color_night_vis
+00010220: 696f 6e28 7365 6c66 2920 2d3e 2062 6f6f  ion(self) -> boo
+00010230: 6c3a 0a20 2020 2020 2020 2069 6620 280a  l:.        if (.
+00010240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010250: 2e66 6561 7475 7265 5f66 6c61 6773 2e68  .feature_flags.h
+00010260: 6f74 706c 7567 2069 7320 6e6f 7420 4e6f  otplug is not No
+00010270: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
+00010280: 6e64 2073 656c 662e 6665 6174 7572 655f  nd self.feature_
+00010290: 666c 6167 732e 686f 7470 6c75 672e 6578  flags.hotplug.ex
+000102a0: 7465 6e64 6572 2069 7320 6e6f 7420 4e6f  tender is not No
+000102b0: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
+000102c0: 6e64 2073 656c 662e 6665 6174 7572 655f  nd self.feature_
+000102d0: 666c 6167 732e 686f 7470 6c75 672e 6578  flags.hotplug.ex
+000102e0: 7465 6e64 6572 2e69 735f 6174 7461 6368  tender.is_attach
+000102f0: 6564 2069 7320 6e6f 7420 4e6f 6e65 0a20  ed is not None. 
+00010300: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00010310: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00010320: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
+00010330: 686f 7470 6c75 672e 6578 7465 6e64 6572  hotplug.extender
+00010340: 2e69 735f 6174 7461 6368 6564 0a0a 2020  .is_attached..  
+00010350: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00010360: 7365 0a0a 2020 2020 6465 6620 7365 745f  se..    def set_
+00010370: 7269 6e67 5f74 696d 656f 7574 2873 656c  ring_timeout(sel
+00010380: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00010390: 2020 2020 7365 6c66 2e5f 6c61 7374 5f72      self._last_r
+000103a0: 696e 675f 7469 6d65 6f75 7420 3d20 7574  ing_timeout = ut
+000103b0: 635f 6e6f 7728 2920 2b20 4556 454e 545f  c_now() + EVENT_
+000103c0: 5049 4e47 5f49 4e54 4552 5641 4c0a 2020  PING_INTERVAL.  
+000103d0: 2020 2020 2020 7365 6c66 2e5f 6576 656e        self._even
+000103e0: 745f 6361 6c6c 6261 636b 5f70 696e 6728  t_callback_ping(
+000103f0: 290a 0a20 2020 2064 6566 2067 6574 5f70  )..    def get_p
+00010400: 7269 7661 6379 5f7a 6f6e 6528 7365 6c66  rivacy_zone(self
+00010410: 2920 2d3e 2074 7570 6c65 5b4f 7074 696f  ) -> tuple[Optio
+00010420: 6e61 6c5b 696e 745d 2c20 4f70 7469 6f6e  nal[int], Option
+00010430: 616c 5b43 616d 6572 615a 6f6e 655d 5d3a  al[CameraZone]]:
+00010440: 0a20 2020 2020 2020 2066 6f72 2069 6e64  .        for ind
+00010450: 6578 2c20 7a6f 6e65 2069 6e20 656e 756d  ex, zone in enum
+00010460: 6572 6174 6528 7365 6c66 2e70 7269 7661  erate(self.priva
+00010470: 6379 5f7a 6f6e 6573 293a 0a20 2020 2020  cy_zones):.     
+00010480: 2020 2020 2020 2069 6620 7a6f 6e65 2e6e         if zone.n
+00010490: 616d 6520 3d3d 2050 5249 5641 4359 5f5a  ame == PRIVACY_Z
+000104a0: 4f4e 455f 4e41 4d45 3a0a 2020 2020 2020  ONE_NAME:.      
+000104b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000104c0: 2069 6e64 6578 2c20 7a6f 6e65 0a20 2020   index, zone.   
+000104d0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000104e0: 2c20 4e6f 6e65 0a0a 2020 2020 6465 6620  , None..    def 
+000104f0: 6164 645f 7072 6976 6163 795f 7a6f 6e65  add_privacy_zone
+00010500: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00010510: 2020 2020 2020 2020 696e 6465 782c 205f          index, _
+00010520: 203d 2073 656c 662e 6765 745f 7072 6976   = self.get_priv
+00010530: 6163 795f 7a6f 6e65 2829 0a20 2020 2020  acy_zone().     
+00010540: 2020 2069 6620 696e 6465 7820 6973 204e     if index is N
+00010550: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010560: 207a 6f6e 655f 6964 203d 2030 0a20 2020   zone_id = 0.   
+00010570: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00010580: 7365 6c66 2e70 7269 7661 6379 5f7a 6f6e  self.privacy_zon
+00010590: 6573 2920 3e20 303a 0a20 2020 2020 2020  es) > 0:.       
+000105a0: 2020 2020 2020 2020 207a 6f6e 655f 6964           zone_id
+000105b0: 203d 2073 656c 662e 7072 6976 6163 795f   = self.privacy_
+000105c0: 7a6f 6e65 735b 2d31 5d2e 6964 202b 2031  zones[-1].id + 1
+000105d0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000105e0: 6c66 2e70 7269 7661 6379 5f7a 6f6e 6573  lf.privacy_zones
+000105f0: 2e61 7070 656e 6428 4361 6d65 7261 5a6f  .append(CameraZo
+00010600: 6e65 2e63 7265 6174 655f 7072 6976 6163  ne.create_privac
+00010610: 795f 7a6f 6e65 287a 6f6e 655f 6964 2929  y_zone(zone_id))
+00010620: 0a0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+00010630: 5f70 7269 7661 6379 5f7a 6f6e 6528 7365  _privacy_zone(se
+00010640: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00010650: 2020 2020 2069 6e64 6578 2c20 5f20 3d20       index, _ = 
+00010660: 7365 6c66 2e67 6574 5f70 7269 7661 6379  self.get_privacy
+00010670: 5f7a 6f6e 6528 290a 0a20 2020 2020 2020  _zone()..       
+00010680: 2069 6620 696e 6465 7820 6973 206e 6f74   if index is not
+00010690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000106a0: 2020 2073 656c 662e 7072 6976 6163 795f     self.privacy_
+000106b0: 7a6f 6e65 732e 706f 7028 696e 6465 7829  zones.pop(index)
+000106c0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+000106d0: 6765 745f 736e 6170 7368 6f74 280a 2020  get_snapshot(.  
+000106e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000106f0: 2020 2020 7769 6474 683a 204f 7074 696f      width: Optio
+00010700: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+00010710: 0a20 2020 2020 2020 2068 6569 6768 743a  .        height:
+00010720: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00010730: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+00010740: 743a 204f 7074 696f 6e61 6c5b 6461 7465  t: Optional[date
+00010750: 7469 6d65 5d20 3d20 4e6f 6e65 2c0a 2020  time] = None,.  
+00010760: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00010770: 6279 7465 735d 3a0a 2020 2020 2020 2020  bytes]:.        
+00010780: 2222 2247 6574 7320 736e 6170 7368 6f74  """Gets snapshot
+00010790: 2066 6f72 2063 616d 6572 612e 0a0a 2020   for camera...  
+000107a0: 2020 2020 2020 4461 7465 7469 6d65 206f        Datetime o
+000107b0: 6620 7363 7265 656e 7368 6f74 2069 7320  f screenshot is 
+000107c0: 6170 7072 6f78 696d 6174 652e 2049 7420  approximate. It 
+000107d0: 6d61 7920 6265 202b 2f2d 2061 2066 6577  may be +/- a few
+000107e0: 2073 6563 6f6e 6473 2e0a 2020 2020 2020   seconds..      
+000107f0: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+00010800: 6620 6e6f 7420 7365 6c66 2e61 7069 2e62  f not self.api.b
+00010810: 6f6f 7473 7472 6170 2e61 7574 685f 7573  ootstrap.auth_us
+00010820: 6572 2e63 616e 280a 2020 2020 2020 2020  er.can(.        
+00010830: 2020 2020 4d6f 6465 6c54 7970 652e 4341      ModelType.CA
+00010840: 4d45 5241 2c0a 2020 2020 2020 2020 2020  MERA,.          
+00010850: 2020 5065 726d 6973 7369 6f6e 4e6f 6465    PermissionNode
+00010860: 2e52 4541 445f 4d45 4449 412c 0a20 2020  .READ_MEDIA,.   
+00010870: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00010880: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00010890: 2020 2020 2020 7261 6973 6520 4e6f 7441        raise NotA
+000108a0: 7574 686f 7269 7a65 6428 0a20 2020 2020  uthorized(.     
+000108b0: 2020 2020 2020 2020 2020 2066 2244 6f20             f"Do 
+000108c0: 6e6f 7420 6861 7665 2070 6572 6d69 7373  not have permiss
+000108d0: 696f 6e20 746f 2072 6561 6420 6d65 6469  ion to read medi
+000108e0: 6120 666f 7220 6361 6d65 7261 3a20 7b73  a for camera: {s
+000108f0: 656c 662e 6964 7d22 2c0a 2020 2020 2020  elf.id}",.      
+00010900: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010910: 2069 6620 6865 6967 6874 2069 7320 4e6f   if height is No
+00010920: 6e65 2061 6e64 2077 6964 7468 2069 7320  ne and width is 
+00010930: 4e6f 6e65 2061 6e64 2073 656c 662e 6869  None and self.hi
+00010940: 6768 5f63 616d 6572 615f 6368 616e 6e65  gh_camera_channe
+00010950: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
+00010960: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+00010970: 7420 3d20 7365 6c66 2e68 6967 685f 6361  t = self.high_ca
+00010980: 6d65 7261 5f63 6861 6e6e 656c 2e68 6569  mera_channel.hei
+00010990: 6768 740a 0a20 2020 2020 2020 2072 6574  ght..        ret
+000109a0: 7572 6e20 6177 6169 7420 7365 6c66 2e61  urn await self.a
+000109b0: 7069 2e67 6574 5f63 616d 6572 615f 736e  pi.get_camera_sn
+000109c0: 6170 7368 6f74 2873 656c 662e 6964 2c20  apshot(self.id, 
+000109d0: 7769 6474 682c 2068 6569 6768 742c 2064  width, height, d
+000109e0: 743d 6474 290a 0a20 2020 2061 7379 6e63  t=dt)..    async
+000109f0: 2064 6566 2067 6574 5f70 6163 6b61 6765   def get_package
+00010a00: 5f73 6e61 7073 686f 7428 0a20 2020 2020  _snapshot(.     
+00010a10: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00010a20: 2077 6964 7468 3a20 4f70 7469 6f6e 616c   width: Optional
+00010a30: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+00010a40: 2020 2020 2020 6865 6967 6874 3a20 4f70        height: Op
+00010a50: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00010a60: 6e65 2c0a 2020 2020 2020 2020 6474 3a20  ne,.        dt: 
+00010a70: 4f70 7469 6f6e 616c 5b64 6174 6574 696d  Optional[datetim
+00010a80: 655d 203d 204e 6f6e 652c 0a20 2020 2029  e] = None,.    )
+00010a90: 202d 3e20 4f70 7469 6f6e 616c 5b62 7974   -> Optional[byt
+00010aa0: 6573 5d3a 0a20 2020 2020 2020 2022 2222  es]:.        """
+00010ab0: 4765 7473 2073 6e61 7073 686f 7420 6672  Gets snapshot fr
+00010ac0: 6f6d 2074 6865 2070 6163 6b61 6765 2063  om the package c
+00010ad0: 616d 6572 612e 0a0a 2020 2020 2020 2020  amera...        
+00010ae0: 4461 7465 7469 6d65 206f 6620 7363 7265  Datetime of scre
+00010af0: 656e 7368 6f74 2069 7320 6170 7072 6f78  enshot is approx
+00010b00: 696d 6174 652e 2049 7420 6d61 7920 6265  imate. It may be
+00010b10: 202b 2f2d 2061 2066 6577 2073 6563 6f6e   +/- a few secon
+00010b20: 6473 2e0a 2020 2020 2020 2020 2222 220a  ds..        """.
+00010b30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00010b40: 7365 6c66 2e66 6561 7475 7265 5f66 6c61  self.feature_fla
+00010b50: 6773 2e68 6173 5f70 6163 6b61 6765 5f63  gs.has_package_c
+00010b60: 616d 6572 613a 0a20 2020 2020 2020 2020  amera:.         
+00010b70: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+00010b80: 6573 7428 2244 6576 6963 6520 646f 6573  est("Device does
+00010b90: 206e 6f74 2068 6176 6520 7061 636b 6167   not have packag
+00010ba0: 6520 6361 6d65 7261 2229 0a0a 2020 2020  e camera")..    
+00010bb0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00010bc0: 6170 692e 626f 6f74 7374 7261 702e 6175  api.bootstrap.au
+00010bd0: 7468 5f75 7365 722e 6361 6e28 0a20 2020  th_user.can(.   
+00010be0: 2020 2020 2020 2020 204d 6f64 656c 5479           ModelTy
+00010bf0: 7065 2e43 414d 4552 412c 0a20 2020 2020  pe.CAMERA,.     
+00010c00: 2020 2020 2020 2050 6572 6d69 7373 696f         Permissio
+00010c10: 6e4e 6f64 652e 5245 4144 5f4d 4544 4941  nNode.READ_MEDIA
+00010c20: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00010c30: 6c66 2c0a 2020 2020 2020 2020 293a 0a20  lf,.        ):. 
+00010c40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010c50: 204e 6f74 4175 7468 6f72 697a 6564 280a   NotAuthorized(.
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c70: 6622 446f 206e 6f74 2068 6176 6520 7065  f"Do not have pe
+00010c80: 726d 6973 7369 6f6e 2074 6f20 7265 6164  rmission to read
+00010c90: 206d 6564 6961 2066 6f72 2063 616d 6572   media for camer
+00010ca0: 613a 207b 7365 6c66 2e69 647d 222c 0a20  a: {self.id}",. 
+00010cb0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00010cc0: 2020 2020 2020 6966 2068 6569 6768 7420        if height 
+00010cd0: 6973 204e 6f6e 6520 616e 6420 7769 6474  is None and widt
+00010ce0: 6820 6973 204e 6f6e 6520 616e 6420 7365  h is None and se
+00010cf0: 6c66 2e70 6163 6b61 6765 5f63 616d 6572  lf.package_camer
+00010d00: 615f 6368 616e 6e65 6c20 6973 206e 6f74  a_channel is not
+00010d10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00010d20: 2020 2068 6569 6768 7420 3d20 7365 6c66     height = self
+00010d30: 2e70 6163 6b61 6765 5f63 616d 6572 615f  .package_camera_
+00010d40: 6368 616e 6e65 6c2e 6865 6967 6874 0a0a  channel.height..
+00010d50: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00010d60: 7761 6974 2073 656c 662e 6170 692e 6765  wait self.api.ge
+00010d70: 745f 7061 636b 6167 655f 6361 6d65 7261  t_package_camera
+00010d80: 5f73 6e61 7073 686f 7428 7365 6c66 2e69  _snapshot(self.i
+00010d90: 642c 2077 6964 7468 2c20 6865 6967 6874  d, width, height
+00010da0: 2c20 6474 3d64 7429 0a0a 2020 2020 6173  , dt=dt)..    as
+00010db0: 796e 6320 6465 6620 6765 745f 7669 6465  ync def get_vide
+00010dc0: 6f28 0a20 2020 2020 2020 2073 656c 662c  o(.        self,
+00010dd0: 0a20 2020 2020 2020 2073 7461 7274 3a20  .        start: 
+00010de0: 6461 7465 7469 6d65 2c0a 2020 2020 2020  datetime,.      
+00010df0: 2020 656e 643a 2064 6174 6574 696d 652c    end: datetime,
+00010e00: 0a20 2020 2020 2020 2063 6861 6e6e 656c  .        channel
+00010e10: 5f69 6e64 6578 3a20 696e 7420 3d20 302c  _index: int = 0,
+00010e20: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00010e30: 6669 6c65 3a20 4f70 7469 6f6e 616c 5b50  file: Optional[P
+00010e40: 6174 685d 203d 204e 6f6e 652c 0a20 2020  ath] = None,.   
+00010e50: 2020 2020 2069 7465 7261 746f 725f 6361       iterator_ca
+00010e60: 6c6c 6261 636b 3a20 4f70 7469 6f6e 616c  llback: Optional
+00010e70: 5b49 7465 7261 746f 7243 616c 6c62 6163  [IteratorCallbac
+00010e80: 6b5d 203d 204e 6f6e 652c 0a20 2020 2020  k] = None,.     
+00010e90: 2020 2070 726f 6772 6573 735f 6361 6c6c     progress_call
+00010ea0: 6261 636b 3a20 4f70 7469 6f6e 616c 5b50  back: Optional[P
+00010eb0: 726f 6772 6573 7343 616c 6c62 6163 6b5d  rogressCallback]
+00010ec0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00010ed0: 2063 6875 6e6b 5f73 697a 653a 2069 6e74   chunk_size: int
+00010ee0: 203d 2036 3535 3336 2c0a 2020 2020 2020   = 65536,.      
+00010ef0: 2020 6670 733a 204f 7074 696f 6e61 6c5b    fps: Optional[
+00010f00: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+00010f10: 2029 202d 3e20 4f70 7469 6f6e 616c 5b62   ) -> Optional[b
+00010f20: 7974 6573 5d3a 0a20 2020 2020 2020 2022  ytes]:.        "
+00010f30: 2222 4578 706f 7274 7320 4d50 3420 7669  ""Exports MP4 vi
+00010f40: 6465 6f20 6672 6f6d 2061 2067 6976 656e  deo from a given
+00010f50: 2063 616d 6572 6120 6174 2061 2073 7065   camera at a spe
+00010f60: 6369 6669 6320 7469 6d65 2e0a 0a20 2020  cific time...   
+00010f70: 2020 2020 2053 7461 7274 2f45 6e64 206f       Start/End o
+00010f80: 6620 7669 6465 6f20 6578 706f 7274 2061  f video export a
+00010f90: 7265 2061 7070 726f 7869 6d61 7465 2e20  re approximate. 
+00010fa0: 4974 206d 6179 2062 6520 2b2f 2d20 6120  It may be +/- a 
+00010fb0: 6665 7720 7365 636f 6e64 732e 0a0a 2020  few seconds...  
+00010fc0: 2020 2020 2020 4974 2069 7320 7265 636f        It is reco
+00010fd0: 6d6d 656e 6465 6420 746f 2070 726f 7669  mmended to provi
+00010fe0: 6465 2061 206f 7574 7075 7420 6669 6c65  de a output file
+00010ff0: 206f 7220 7072 6f67 7265 7373 2063 616c   or progress cal
+00011000: 6c62 6163 6b20 666f 7220 6c61 7267 6572  lback for larger
+00011010: 0a20 2020 2020 2020 2076 6964 656f 2063  .        video c
+00011020: 6c69 7073 2c20 6f74 6865 7277 6973 6520  lips, otherwise 
+00011030: 7468 6520 6675 6c6c 2076 6964 656f 206d  the full video m
+00011040: 7573 7420 6265 2064 6f77 6e6c 6f61 6465  ust be downloade
+00011050: 6420 746f 206d 656d 6f72 7920 6265 666f  d to memory befo
+00011060: 7265 0a20 2020 2020 2020 2062 6569 6e67  re.        being
+00011070: 2077 7269 7474 656e 2e0a 0a20 2020 2020   written...     
+00011080: 2020 2050 726f 7669 6469 6e67 2074 6865     Providing the
+00011090: 2060 6670 7360 2070 6172 616d 6574 6572   `fps` parameter
+000110a0: 2063 7265 6174 6573 2061 2022 7469 6d65   creates a "time
+000110b0: 6c61 7073 6522 2065 7870 6f72 7420 7774  lapse" export wt
+000110c0: 6968 2074 6865 2067 6976 656e 2046 5053  ih the given FPS
+000110d0: 0a20 2020 2020 2020 2076 616c 7565 2e20  .        value. 
+000110e0: 5072 6f74 6563 7420 6170 7020 6769 7665  Protect app give
+000110f0: 7320 7468 6520 6f70 7469 6f6e 7320 666f  s the options fo
+00011100: 7220 3630 7820 2866 7073 3d34 292c 2031  r 60x (fps=4), 1
+00011110: 3230 7820 2866 7073 3d38 292c 2033 3030  20x (fps=8), 300
+00011120: 780a 2020 2020 2020 2020 2866 7073 3d32  x.        (fps=2
+00011130: 3029 2c20 616e 6420 3630 3078 2028 6670  0), and 600x (fp
+00011140: 733d 3430 292e 0a20 2020 2020 2020 2022  s=40)..        "
+00011150: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+00011160: 6f74 2073 656c 662e 6170 692e 626f 6f74  ot self.api.boot
+00011170: 7374 7261 702e 6175 7468 5f75 7365 722e  strap.auth_user.
+00011180: 6361 6e28 0a20 2020 2020 2020 2020 2020  can(.           
+00011190: 204d 6f64 656c 5479 7065 2e43 414d 4552   ModelType.CAMER
+000111a0: 412c 0a20 2020 2020 2020 2020 2020 2050  A,.            P
+000111b0: 6572 6d69 7373 696f 6e4e 6f64 652e 5245  ermissionNode.RE
+000111c0: 4144 5f4d 4544 4941 2c0a 2020 2020 2020  AD_MEDIA,.      
+000111d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000111e0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000111f0: 2020 2072 6169 7365 204e 6f74 4175 7468     raise NotAuth
+00011200: 6f72 697a 6564 280a 2020 2020 2020 2020  orized(.        
+00011210: 2020 2020 2020 2020 6622 446f 206e 6f74          f"Do not
+00011220: 2068 6176 6520 7065 726d 6973 7369 6f6e   have permission
+00011230: 2074 6f20 7265 6164 206d 6564 6961 2066   to read media f
+00011240: 6f72 2063 616d 6572 613a 207b 7365 6c66  or camera: {self
+00011250: 2e69 647d 222c 0a20 2020 2020 2020 2020  .id}",.         
+00011260: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+00011270: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00011280: 6170 692e 6765 745f 6361 6d65 7261 5f76  api.get_camera_v
+00011290: 6964 656f 280a 2020 2020 2020 2020 2020  ideo(.          
+000112a0: 2020 7365 6c66 2e69 642c 0a20 2020 2020    self.id,.     
+000112b0: 2020 2020 2020 2073 7461 7274 2c0a 2020         start,.  
+000112c0: 2020 2020 2020 2020 2020 656e 642c 0a20            end,. 
+000112d0: 2020 2020 2020 2020 2020 2063 6861 6e6e             chann
+000112e0: 656c 5f69 6e64 6578 2c0a 2020 2020 2020  el_index,.      
+000112f0: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00011300: 653d 6f75 7470 7574 5f66 696c 652c 0a20  e=output_file,. 
+00011310: 2020 2020 2020 2020 2020 2069 7465 7261             itera
+00011320: 746f 725f 6361 6c6c 6261 636b 3d69 7465  tor_callback=ite
+00011330: 7261 746f 725f 6361 6c6c 6261 636b 2c0a  rator_callback,.
+00011340: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
+00011350: 7265 7373 5f63 616c 6c62 6163 6b3d 7072  ress_callback=pr
+00011360: 6f67 7265 7373 5f63 616c 6c62 6163 6b2c  ogress_callback,
+00011370: 0a20 2020 2020 2020 2020 2020 2063 6875  .            chu
+00011380: 6e6b 5f73 697a 653d 6368 756e 6b5f 7369  nk_size=chunk_si
+00011390: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+000113a0: 6670 733d 6670 732c 0a20 2020 2020 2020  fps=fps,.       
+000113b0: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
+000113c0: 6620 7365 745f 7265 636f 7264 696e 675f  f set_recording_
+000113d0: 6d6f 6465 2873 656c 662c 206d 6f64 653a  mode(self, mode:
+000113e0: 2052 6563 6f72 6469 6e67 4d6f 6465 2920   RecordingMode) 
+000113f0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011400: 2022 2222 5365 7473 2072 6563 6f72 6469   """Sets recordi
+00011410: 6e67 206d 6f64 6520 6f6e 2063 616d 6572  ng mode on camer
+00011420: 6122 2222 0a0a 2020 2020 2020 2020 6966  a"""..        if
+00011430: 2073 656c 662e 7573 655f 676c 6f62 616c   self.use_global
+00011440: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00011450: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
+00011460: 4361 6d65 7261 2069 7320 7573 696e 6720  Camera is using 
+00011470: 676c 6f62 616c 2072 6563 6f72 6469 6e67  global recording
+00011480: 2073 6574 7469 6e67 732e 2229 0a0a 2020   settings.")..  
+00011490: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
+000114a0: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
+000114b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000114c0: 6563 6f72 6469 6e67 5f73 6574 7469 6e67  ecording_setting
+000114d0: 732e 6d6f 6465 203d 206d 6f64 650a 0a20  s.mode = mode.. 
+000114e0: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+000114f0: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
+00011500: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
+00011510: 796e 6320 6465 6620 7365 745f 6972 5f6c  ync def set_ir_l
+00011520: 6564 5f6d 6f64 656c 2873 656c 662c 206d  ed_model(self, m
+00011530: 6f64 653a 2049 524c 4544 4d6f 6465 2920  ode: IRLEDMode) 
+00011540: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011550: 2022 2222 5365 7473 2049 5220 4c45 4420   """Sets IR LED 
+00011560: 6d6f 6465 206f 6e20 6361 6d65 7261 2222  mode on camera""
+00011570: 220a 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
+00011580: 7420 7365 6c66 2e66 6561 7475 7265 5f66  t self.feature_f
+00011590: 6c61 6773 2e68 6173 5f6c 6564 5f69 723a  lags.has_led_ir:
+000115a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000115b0: 7365 2042 6164 5265 7175 6573 7428 2243  se BadRequest("C
+000115c0: 616d 6572 6120 646f 6573 206e 6f74 2068  amera does not h
+000115d0: 6176 6520 616e 204c 4544 2049 5222 290a  ave an LED IR").
+000115e0: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
+000115f0: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
+00011600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011610: 662e 6973 705f 7365 7474 696e 6773 2e69  f.isp_settings.i
+00011620: 725f 6c65 645f 6d6f 6465 203d 206d 6f64  r_led_mode = mod
+00011630: 650a 0a20 2020 2020 2020 2061 7761 6974  e..        await
+00011640: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+00011650: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+00011660: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+00011670: 6963 725f 6375 7374 6f6d 5f6c 7578 2873  icr_custom_lux(s
+00011680: 656c 662c 2076 616c 7565 3a20 4943 524c  elf, value: ICRL
+00011690: 7578 5661 6c75 6529 202d 3e20 4e6f 6e65  uxValue) -> None
+000116a0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+000116b0: 2049 4352 4375 7374 6f6d 5661 6c75 6520   ICRCustomValue 
+000116c0: 6672 6f6d 206c 7578 2076 616c 7565 2e22  from lux value."
+000116d0: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+000116e0: 6f74 2073 656c 662e 6665 6174 7572 655f  ot self.feature_
+000116f0: 666c 6167 732e 6861 735f 6c65 645f 6972  flags.has_led_ir
+00011700: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00011710: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
+00011720: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
+00011730: 6861 7665 2061 6e20 4c45 4420 4952 2229  have an LED IR")
+00011740: 0a0a 2020 2020 2020 2020 6963 725f 7661  ..        icr_va
+00011750: 6c75 6520 3d20 300a 2020 2020 2020 2020  lue = 0.        
+00011760: 666f 7220 696e 6465 782c 2074 6872 6573  for index, thres
+00011770: 686f 6c64 2069 6e20 656e 756d 6572 6174  hold in enumerat
+00011780: 6528 4c55 585f 4d41 5050 494e 475f 5641  e(LUX_MAPPING_VA
+00011790: 4c55 4553 293a 0a20 2020 2020 2020 2020  LUES):.         
+000117a0: 2020 2069 6620 7661 6c75 6520 3e3d 2074     if value >= t
+000117b0: 6872 6573 686f 6c64 3a0a 2020 2020 2020  hreshold:.      
+000117c0: 2020 2020 2020 2020 2020 6963 725f 7661            icr_va
+000117d0: 6c75 6520 3d20 3130 202d 2069 6e64 6578  lue = 10 - index
+000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117f0: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
+00011800: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
+00011810: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00011820: 2020 2020 7365 6c66 2e69 7370 5f73 6574      self.isp_set
+00011830: 7469 6e67 732e 6963 725f 6375 7374 6f6d  tings.icr_custom
+00011840: 5f76 616c 7565 203d 2063 6173 7428 4943  _value = cast(IC
+00011850: 5243 7573 746f 6d56 616c 7565 2c20 6963  RCustomValue, ic
+00011860: 725f 7661 6c75 6529 0a0a 2020 2020 2020  r_value)..      
+00011870: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
+00011880: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
+00011890: 636b 290a 0a20 2020 2040 7072 6f70 6572  ck)..    @proper
+000118a0: 7479 0a20 2020 2064 6566 2069 735f 6972  ty.    def is_ir
+000118b0: 5f6c 6564 5f73 6c69 6465 725f 656e 6162  _led_slider_enab
+000118c0: 6c65 6428 7365 6c66 2920 2d3e 2062 6f6f  led(self) -> boo
+000118d0: 6c3a 0a20 2020 2020 2020 2022 2222 5265  l:.        """Re
+000118e0: 7475 726e 2069 6620 4952 204c 4544 2063  turn if IR LED c
+000118f0: 7573 746f 6d20 736c 6964 6572 2069 7320  ustom slider is 
+00011900: 656e 6162 6c65 642e 2222 220a 0a20 2020  enabled."""..   
+00011910: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
+00011920: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00011930: 6561 7475 7265 5f66 6c61 6773 2e68 6173  eature_flags.has
+00011940: 5f6c 6564 5f69 720a 2020 2020 2020 2020  _led_ir.        
+00011950: 2020 2020 616e 6420 7365 6c66 2e69 7370      and self.isp
+00011960: 5f73 6574 7469 6e67 732e 6972 5f6c 6564  _settings.ir_led
+00011970: 5f6d 6f64 6520 3d3d 2049 524c 4544 4d6f  _mode == IRLEDMo
+00011980: 6465 2e43 5553 544f 4d0a 2020 2020 2020  de.CUSTOM.      
+00011990: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
+000119a0: 6566 2073 6574 5f73 7461 7475 735f 6c69  ef set_status_li
+000119b0: 6768 7428 7365 6c66 2c20 656e 6162 6c65  ght(self, enable
+000119c0: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
+000119d0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+000119e0: 7320 7374 6174 7573 2069 6e64 6963 6963  s status indicic
+000119f0: 6174 6f72 206c 6967 6874 206f 6e20 6361  ator light on ca
+00011a00: 6d65 7261 2222 220a 0a20 2020 2020 2020  mera"""..       
+00011a10: 2069 6620 6e6f 7420 7365 6c66 2e66 6561   if not self.fea
+00011a20: 7475 7265 5f66 6c61 6773 2e68 6173 5f6c  ture_flags.has_l
+00011a30: 6564 5f73 7461 7475 733a 0a20 2020 2020  ed_status:.     
+00011a40: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
+00011a50: 5265 7175 6573 7428 2243 616d 6572 6120  Request("Camera 
+00011a60: 646f 6573 206e 6f74 2068 6176 6520 7374  does not have st
+00011a70: 6174 7573 206c 6967 6874 2229 0a0a 2020  atus light")..  
+00011a80: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
+00011a90: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
+00011aa0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00011ab0: 6564 5f73 6574 7469 6e67 732e 6973 5f65  ed_settings.is_e
+00011ac0: 6e61 626c 6564 203d 2065 6e61 626c 6564  nabled = enabled
+00011ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011ae0: 662e 6c65 645f 7365 7474 696e 6773 2e62  f.led_settings.b
+00011af0: 6c69 6e6b 5f72 6174 6520 3d20 300a 0a20  link_rate = 0.. 
+00011b00: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00011b10: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
+00011b20: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
+00011b30: 796e 6320 6465 6620 7365 745f 6864 7228  ync def set_hdr(
+00011b40: 7365 6c66 2c20 656e 6162 6c65 643a 2062  self, enabled: b
+00011b50: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+00011b60: 2020 2020 2020 2222 2253 6574 7320 4844        """Sets HD
+00011b70: 5220 2848 6967 6820 4479 6e61 6d69 6320  R (High Dynamic 
+00011b80: 5261 6e67 6529 206f 6e20 6361 6d65 7261  Range) on camera
+00011b90: 2222 220a 0a20 2020 2020 2020 2077 6172  """..        war
+00011ba0: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
+00011bb0: 2020 2020 2020 2020 2273 6574 5f68 6472          "set_hdr
+00011bc0: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
+00011bd0: 6e64 2072 6570 6c61 6365 6420 7769 7468  nd replaced with
+00011be0: 2073 6574 5f68 6472 5f6d 6f64 6520 666f   set_hdr_mode fo
+00011bf0: 7220 7665 7273 696f 6e73 206f 6620 556e  r versions of Un
+00011c00: 6946 6920 5072 6f74 6563 7420 7633 2e30  iFi Protect v3.0
+00011c10: 2b22 2c0a 2020 2020 2020 2020 2020 2020  +",.            
+00011c20: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+00011c30: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+00011c40: 7374 6163 6b6c 6576 656c 3d32 2c0a 2020  stacklevel=2,.  
+00011c50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00011c60: 2069 6620 6e6f 7420 7365 6c66 2e66 6561   if not self.fea
+00011c70: 7475 7265 5f66 6c61 6773 2e68 6173 5f68  ture_flags.has_h
+00011c80: 6472 3a0a 2020 2020 2020 2020 2020 2020  dr:.            
+00011c90: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
+00011ca0: 2822 4361 6d65 7261 2064 6f65 7320 6e6f  ("Camera does no
+00011cb0: 7420 6861 7665 2048 4452 2229 0a0a 2020  t have HDR")..  
+00011cc0: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
+00011cd0: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
+00011ce0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00011cf0: 6472 5f6d 6f64 6520 3d20 656e 6162 6c65  dr_mode = enable
+00011d00: 640a 0a20 2020 2020 2020 2061 7761 6974  d..        await
+00011d10: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+00011d20: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+00011d30: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+00011d40: 6864 725f 6d6f 6465 2873 656c 662c 206d  hdr_mode(self, m
+00011d50: 6f64 653a 204c 6974 6572 616c 5b22 6175  ode: Literal["au
+00011d60: 746f 222c 2022 6f66 6622 2c20 2261 6c77  to", "off", "alw
+00011d70: 6179 7322 5d29 202d 3e20 4e6f 6e65 3a0a  ays"]) -> None:.
+00011d80: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00011d90: 4844 5220 6d6f 6465 2073 696d 696c 6172  HDR mode similar
+00011da0: 2074 6f20 686f 7720 5072 6f74 6563 7420   to how Protect 
+00011db0: 696e 7465 7266 6163 6520 776f 726b 732e  interface works.
+00011dc0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00011dd0: 6e6f 7420 7365 6c66 2e66 6561 7475 7265  not self.feature
+00011de0: 5f66 6c61 6773 2e68 6173 5f68 6472 3a0a  _flags.has_hdr:.
+00011df0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00011e00: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
+00011e10: 6d65 7261 2064 6f65 7320 6e6f 7420 6861  mera does not ha
+00011e20: 7665 2048 4452 2229 0a0a 2020 2020 2020  ve HDR")..      
+00011e30: 2020 6465 6620 6361 6c6c 6261 636b 2829    def callback()
+00011e40: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00011e50: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
+00011e60: 2022 6f66 6622 3a0a 2020 2020 2020 2020   "off":.        
+00011e70: 2020 2020 2020 2020 7365 6c66 2e68 6472          self.hdr
+00011e80: 5f6d 6f64 6520 3d20 4661 6c73 650a 2020  _mode = False.  
+00011e90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011ea0: 2073 656c 662e 6973 705f 7365 7474 696e   self.isp_settin
+00011eb0: 6773 2e68 6472 5f6d 6f64 6520 6973 206e  gs.hdr_mode is n
+00011ec0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00011ed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011ee0: 662e 6973 705f 7365 7474 696e 6773 2e68  f.isp_settings.h
+00011ef0: 6472 5f6d 6f64 6520 3d20 4844 524d 6f64  dr_mode = HDRMod
+00011f00: 652e 4e4f 524d 414c 0a20 2020 2020 2020  e.NORMAL.       
+00011f10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00011f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011f30: 6864 725f 6d6f 6465 203d 2054 7275 650a  hdr_mode = True.
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 6966 2073 656c 662e 6973 705f 7365 7474  if self.isp_sett
+00011f60: 696e 6773 2e68 6472 5f6d 6f64 6520 6973  ings.hdr_mode is
+00011f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011f90: 656c 662e 6973 705f 7365 7474 696e 6773  elf.isp_settings
+00011fa0: 2e68 6472 5f6d 6f64 6520 3d20 280a 2020  .hdr_mode = (.  
+00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2020 4844 524d 6f64 652e 4e4f        HDRMode.NO
+00011fd0: 524d 414c 2069 6620 6d6f 6465 203d 3d20  RMAL if mode == 
+00011fe0: 2261 7574 6f22 2065 6c73 6520 4844 524d  "auto" else HDRM
+00011ff0: 6f64 652e 414c 5741 5953 5f4f 4e0a 2020  ode.ALWAYS_ON.  
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012010: 2020 290a 0a20 2020 2020 2020 2061 7761    )..        awa
+00012020: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
+00012030: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
+00012040: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
+00012050: 745f 636f 6c6f 725f 6e69 6768 745f 7669  t_color_night_vi
+00012060: 7369 6f6e 2873 656c 662c 2065 6e61 626c  sion(self, enabl
+00012070: 6564 3a20 626f 6f6c 2920 2d3e 204e 6f6e  ed: bool) -> Non
+00012080: 653a 0a20 2020 2020 2020 2022 2222 5365  e:.        """Se
+00012090: 7473 2043 6f6c 6f72 204e 6967 6874 2056  ts Color Night V
+000120a0: 6973 696f 6e20 6f6e 2063 616d 6572 6122  ision on camera"
+000120b0: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+000120c0: 6f74 2073 656c 662e 6861 735f 636f 6c6f  ot self.has_colo
+000120d0: 725f 6e69 6768 745f 7669 7369 6f6e 3a0a  r_night_vision:.
+000120e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000120f0: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
+00012100: 6d65 7261 2064 6f65 7320 6e6f 7420 6861  mera does not ha
+00012110: 7665 2043 6f6c 6f72 204e 6967 6874 2056  ve Color Night V
+00012120: 6973 696f 6e22 290a 0a20 2020 2020 2020  ision")..       
+00012130: 2064 6566 2063 616c 6c62 6163 6b28 2920   def callback() 
+00012140: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00012150: 2020 2020 2073 656c 662e 6973 705f 7365       self.isp_se
+00012160: 7474 696e 6773 2e69 735f 636f 6c6f 725f  ttings.is_color_
+00012170: 6e69 6768 745f 7669 7369 6f6e 5f65 6e61  night_vision_ena
+00012180: 626c 6564 203d 2065 6e61 626c 6564 0a0a  bled = enabled..
+00012190: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+000121a0: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
+000121b0: 6361 6c6c 6261 636b 290a 0a20 2020 2061  callback)..    a
+000121c0: 7379 6e63 2064 6566 2073 6574 5f76 6964  sync def set_vid
+000121d0: 656f 5f6d 6f64 6528 7365 6c66 2c20 6d6f  eo_mode(self, mo
+000121e0: 6465 3a20 5669 6465 6f4d 6f64 6529 202d  de: VideoMode) -
+000121f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012200: 2222 2253 6574 7320 7669 6465 6f20 6d6f  """Sets video mo
+00012210: 6465 206f 6e20 6361 6d65 7261 2222 220a  de on camera""".
+00012220: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+00012230: 206e 6f74 2069 6e20 7365 6c66 2e66 6561   not in self.fea
+00012240: 7475 7265 5f66 6c61 6773 2e76 6964 656f  ture_flags.video
+00012250: 5f6d 6f64 6573 3a0a 2020 2020 2020 2020  _modes:.        
+00012260: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+00012270: 7565 7374 2866 2243 616d 6572 6120 646f  uest(f"Camera do
+00012280: 6573 206e 6f74 2068 6176 6520 7b6d 6f64  es not have {mod
+00012290: 657d 2229 0a0a 2020 2020 2020 2020 6465  e}")..        de
+000122a0: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
+000122b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000122c0: 2020 7365 6c66 2e76 6964 656f 5f6d 6f64    self.video_mod
+000122d0: 6520 3d20 6d6f 6465 0a0a 2020 2020 2020  e = mode..      
+000122e0: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
+000122f0: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
+00012300: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
+00012310: 6566 2073 6574 5f63 616d 6572 615f 7a6f  ef set_camera_zo
+00012320: 6f6d 2873 656c 662c 206c 6576 656c 3a20  om(self, level: 
+00012330: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00012340: 2020 2020 2020 2222 2253 6574 7320 7a6f        """Sets zo
+00012350: 6f6d 206c 6576 656c 2066 6f72 2063 616d  om level for cam
+00012360: 6572 6122 2222 0a0a 2020 2020 2020 2020  era"""..        
+00012370: 6966 206e 6f74 2073 656c 662e 6665 6174  if not self.feat
+00012380: 7572 655f 666c 6167 732e 6361 6e5f 6f70  ure_flags.can_op
+00012390: 7469 6361 6c5f 7a6f 6f6d 3a0a 2020 2020  tical_zoom:.    
+000123a0: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+000123b0: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
+000123c0: 2063 616e 6e6f 7420 6f70 7469 6361 6c20   cannot optical 
+000123d0: 7a6f 6f6d 2229 0a0a 2020 2020 2020 2020  zoom")..        
+000123e0: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
+000123f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012400: 2020 2020 7365 6c66 2e69 7370 5f73 6574      self.isp_set
+00012410: 7469 6e67 732e 7a6f 6f6d 5f70 6f73 6974  tings.zoom_posit
+00012420: 696f 6e20 3d20 5065 7263 656e 7449 6e74  ion = PercentInt
+00012430: 286c 6576 656c 290a 0a20 2020 2020 2020  (level)..       
+00012440: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
+00012450: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
+00012460: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
+00012470: 6620 7365 745f 7764 725f 6c65 7665 6c28  f set_wdr_level(
+00012480: 7365 6c66 2c20 6c65 7665 6c3a 2069 6e74  self, level: int
+00012490: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000124a0: 2020 2022 2222 5365 7473 2057 4452 2028     """Sets WDR (
+000124b0: 5769 6465 2044 796e 616d 6963 2052 616e  Wide Dynamic Ran
+000124c0: 6765 2920 6f6e 2063 616d 6572 6122 2222  ge) on camera"""
+000124d0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+000124e0: 662e 6665 6174 7572 655f 666c 6167 732e  f.feature_flags.
+000124f0: 6861 735f 6864 723a 0a20 2020 2020 2020  has_hdr:.       
+00012500: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+00012510: 7175 6573 7428 2243 616e 6e6f 7420 7365  quest("Cannot se
+00012520: 7420 5744 5220 6f6e 2063 616d 6572 6173  t WDR on cameras
+00012530: 2077 6974 6820 4844 5222 290a 0a20 2020   with HDR")..   
+00012540: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+00012550: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+00012560: 2020 2020 2020 2020 2073 656c 662e 6973           self.is
+00012570: 705f 7365 7474 696e 6773 2e77 6472 203d  p_settings.wdr =
+00012580: 2057 4452 4c65 7665 6c28 6c65 7665 6c29   WDRLevel(level)
+00012590: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+000125a0: 7365 6c66 2e71 7565 7565 5f75 7064 6174  self.queue_updat
+000125b0: 6528 6361 6c6c 6261 636b 290a 0a20 2020  e(callback)..   
+000125c0: 2061 7379 6e63 2064 6566 2073 6574 5f6d   async def set_m
+000125d0: 6963 5f76 6f6c 756d 6528 7365 6c66 2c20  ic_volume(self, 
+000125e0: 6c65 7665 6c3a 2069 6e74 2920 2d3e 204e  level: int) -> N
+000125f0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00012600: 5365 7473 2074 6865 206d 6963 2073 656e  Sets the mic sen
+00012610: 7369 7469 7669 7479 206c 6576 656c 206f  sitivity level o
+00012620: 6e20 6361 6d65 7261 2222 220a 0a20 2020  n camera"""..   
+00012630: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00012640: 2e66 6561 7475 7265 5f66 6c61 6773 2e68  .feature_flags.h
+00012650: 6173 5f6d 6963 3a0a 2020 2020 2020 2020  as_mic:.        
+00012660: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+00012670: 7565 7374 2822 4361 6d65 7261 2064 6f65  uest("Camera doe
+00012680: 7320 6e6f 7420 6861 7665 206d 6963 2229  s not have mic")
+00012690: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
+000126a0: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
+000126b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000126c0: 6c66 2e6d 6963 5f76 6f6c 756d 6520 3d20  lf.mic_volume = 
+000126d0: 5065 7263 656e 7449 6e74 286c 6576 656c  PercentInt(level
+000126e0: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
+000126f0: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+00012700: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+00012710: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+00012720: 7370 6561 6b65 725f 766f 6c75 6d65 2873  speaker_volume(s
+00012730: 656c 662c 206c 6576 656c 3a20 696e 7429  elf, level: int)
+00012740: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00012750: 2020 2222 2253 6574 7320 7468 6520 7370    """Sets the sp
+00012760: 6561 6b65 7220 7365 6e73 6974 6976 6974  eaker sensitivit
+00012770: 7920 6c65 7665 6c20 6f6e 2063 616d 6572  y level on camer
+00012780: 612e 2052 6571 7569 7265 7320 6361 6d65  a. Requires came
+00012790: 7261 2074 6f20 6861 7665 2073 7065 616b  ra to have speak
+000127a0: 6572 7322 2222 0a0a 2020 2020 2020 2020  ers"""..        
+000127b0: 6966 206e 6f74 2073 656c 662e 6665 6174  if not self.feat
+000127c0: 7572 655f 666c 6167 732e 6861 735f 7370  ure_flags.has_sp
+000127d0: 6561 6b65 723a 0a20 2020 2020 2020 2020  eaker:.         
+000127e0: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+000127f0: 6573 7428 2243 616d 6572 6120 646f 6573  est("Camera does
+00012800: 206e 6f74 2068 6176 6520 7370 6561 6b65   not have speake
+00012810: 7222 290a 0a20 2020 2020 2020 2064 6566  r")..        def
+00012820: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
+00012830: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00012840: 2073 656c 662e 7370 6561 6b65 725f 7365   self.speaker_se
+00012850: 7474 696e 6773 2e76 6f6c 756d 6520 3d20  ttings.volume = 
+00012860: 5065 7263 656e 7449 6e74 286c 6576 656c  PercentInt(level
+00012870: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
+00012880: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+00012890: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+000128a0: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+000128b0: 6368 696d 655f 7479 7065 2873 656c 662c  chime_type(self,
+000128c0: 2063 6869 6d65 5f74 7970 653a 2043 6869   chime_type: Chi
+000128d0: 6d65 5479 7065 2920 2d3e 204e 6f6e 653a  meType) -> None:
+000128e0: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
+000128f0: 2063 6869 6d65 2074 7970 6520 666f 7220   chime type for 
+00012900: 646f 6f72 6265 6c6c 2e20 5265 7175 6972  doorbell. Requir
+00012910: 6573 2063 616d 6572 6120 746f 2062 6520  es camera to be 
+00012920: 6120 646f 6f72 6265 6c6c 2222 220a 0a20  a doorbell""".. 
+00012930: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00012940: 662e 7365 745f 6368 696d 655f 6475 7261  f.set_chime_dura
+00012950: 7469 6f6e 2874 696d 6564 656c 7461 286d  tion(timedelta(m
+00012960: 696c 6c69 7365 636f 6e64 733d 6368 696d  illiseconds=chim
+00012970: 655f 7479 7065 2e76 616c 7565 2929 0a0a  e_type.value))..
+00012980: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
+00012990: 745f 6368 696d 655f 6475 7261 7469 6f6e  t_chime_duration
+000129a0: 2873 656c 662c 2064 7572 6174 696f 6e3a  (self, duration:
+000129b0: 2074 696d 6564 656c 7461 207c 2066 6c6f   timedelta | flo
+000129c0: 6174 2920 2d3e 204e 6f6e 653a 0a20 2020  at) -> None:.   
+000129d0: 2020 2020 2022 2222 5365 7473 2063 6869       """Sets chi
+000129e0: 6d65 2064 7572 6174 696f 6e20 666f 7220  me duration for 
+000129f0: 646f 6f72 6265 6c6c 2e20 5265 7175 6972  doorbell. Requir
+00012a00: 6573 2063 616d 6572 6120 746f 2062 6520  es camera to be 
+00012a10: 6120 646f 6f72 6265 6c6c 2222 220a 0a20  a doorbell""".. 
+00012a20: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00012a30: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
+00012a40: 2e68 6173 5f63 6869 6d65 3a0a 2020 2020  .has_chime:.    
+00012a50: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+00012a60: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
+00012a70: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
+00012a80: 2063 6869 6d65 2229 0a0a 2020 2020 2020   chime")..      
+00012a90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00012aa0: 6475 7261 7469 6f6e 2c20 2866 6c6f 6174  duration, (float
+00012ab0: 2c20 696e 7429 293a 0a20 2020 2020 2020  , int)):.       
+00012ac0: 2020 2020 2069 6620 6475 7261 7469 6f6e       if duration
+00012ad0: 203c 2030 3a0a 2020 2020 2020 2020 2020   < 0:.          
+00012ae0: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
+00012af0: 6571 7565 7374 2822 4368 696d 6520 6475  equest("Chime du
+00012b00: 7261 7469 6f6e 206d 7573 7420 6265 2061  ration must be a
+00012b10: 2070 6f73 6974 6976 6520 6e75 6d62 6572   positive number
+00012b20: 206f 6620 7365 636f 6e64 7322 290a 2020   of seconds").  
+00012b30: 2020 2020 2020 2020 2020 6475 7261 7469            durati
+00012b40: 6f6e 5f74 6420 3d20 7469 6d65 6465 6c74  on_td = timedelt
+00012b50: 6128 7365 636f 6e64 733d 6475 7261 7469  a(seconds=durati
+00012b60: 6f6e 290a 2020 2020 2020 2020 656c 7365  on).        else
+00012b70: 3a0a 2020 2020 2020 2020 2020 2020 6475  :.            du
+00012b80: 7261 7469 6f6e 5f74 6420 3d20 6475 7261  ration_td = dura
+00012b90: 7469 6f6e 0a0a 2020 2020 2020 2020 6966  tion..        if
+00012ba0: 2064 7572 6174 696f 6e5f 7464 2e74 6f74   duration_td.tot
+00012bb0: 616c 5f73 6563 6f6e 6473 2829 203e 2031  al_seconds() > 1
+00012bc0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00012bd0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+00012be0: 2243 6869 6d65 2064 7572 6174 696f 6e20  "Chime duration 
+00012bf0: 6973 2074 6f6f 206c 6f6e 6722 290a 0a20  is too long").. 
+00012c00: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
+00012c10: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
+00012c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012c30: 6368 696d 655f 6475 7261 7469 6f6e 203d  chime_duration =
+00012c40: 2064 7572 6174 696f 6e5f 7464 0a0a 2020   duration_td..  
+00012c50: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00012c60: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
+00012c70: 6c6c 6261 636b 290a 0a20 2020 2061 7379  llback)..    asy
+00012c80: 6e63 2064 6566 2073 6574 5f73 7973 7465  nc def set_syste
+00012c90: 6d5f 736f 756e 6473 2873 656c 662c 2065  m_sounds(self, e
+00012ca0: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
+00012cb0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00012cc0: 2222 5365 7473 2073 7973 7465 6d20 736f  ""Sets system so
+00012cd0: 756e 6420 706c 6179 6261 636b 2074 6872  und playback thr
+00012ce0: 6f75 6768 2073 7065 616b 6572 732e 2052  ough speakers. R
+00012cf0: 6571 7569 7265 7320 6361 6d65 7261 2074  equires camera t
+00012d00: 6f20 6861 7665 2073 7065 616b 6572 7322  o have speakers"
+00012d10: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+00012d20: 6f74 2073 656c 662e 6665 6174 7572 655f  ot self.feature_
+00012d30: 666c 6167 732e 6861 735f 7370 6561 6b65  flags.has_speake
+00012d40: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00012d50: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+00012d60: 2243 616d 6572 6120 646f 6573 206e 6f74  "Camera does not
+00012d70: 2068 6176 6520 7370 6561 6b65 7222 290a   have speaker").
+00012d80: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
+00012d90: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
+00012da0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012db0: 662e 7370 6561 6b65 725f 7365 7474 696e  f.speaker_settin
+00012dc0: 6773 2e61 7265 5f73 7973 7465 6d5f 736f  gs.are_system_so
+00012dd0: 756e 6473 5f65 6e61 626c 6564 203d 2065  unds_enabled = e
+00012de0: 6e61 626c 6564 0a0a 2020 2020 2020 2020  nabled..        
+00012df0: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+00012e00: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+00012e10: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00012e20: 2073 6574 5f6f 7364 5f6e 616d 6528 7365   set_osd_name(se
+00012e30: 6c66 2c20 656e 6162 6c65 643a 2062 6f6f  lf, enabled: boo
+00012e40: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+00012e50: 2020 2020 2222 2253 6574 7320 7768 6574      """Sets whet
+00012e60: 6865 7220 6361 6d65 7261 206e 616d 6520  her camera name 
+00012e70: 6973 2069 6e20 7468 6520 4f6e 2053 6372  is in the On Scr
+00012e80: 6565 6e20 4469 7370 6c61 7922 2222 0a0a  een Display"""..
+00012e90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012ea0: 7573 655f 676c 6f62 616c 3a0a 2020 2020  use_global:.    
+00012eb0: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+00012ec0: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
+00012ed0: 2069 7320 7573 696e 6720 676c 6f62 616c   is using global
+00012ee0: 2072 6563 6f72 6469 6e67 2073 6574 7469   recording setti
+00012ef0: 6e67 732e 2229 0a0a 2020 2020 2020 2020  ngs.")..        
+00012f00: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
+00012f10: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012f20: 2020 2020 7365 6c66 2e6f 7364 5f73 6574      self.osd_set
+00012f30: 7469 6e67 732e 6973 5f6e 616d 655f 656e  tings.is_name_en
+00012f40: 6162 6c65 6420 3d20 656e 6162 6c65 640a  abled = enabled.
+00012f50: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+00012f60: 656c 662e 7175 6575 655f 7570 6461 7465  elf.queue_update
+00012f70: 2863 616c 6c62 6163 6b29 0a0a 2020 2020  (callback)..    
+00012f80: 6173 796e 6320 6465 6620 7365 745f 6f73  async def set_os
+00012f90: 645f 6461 7465 2873 656c 662c 2065 6e61  d_date(self, ena
+00012fa0: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+00012fb0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00012fc0: 5365 7473 2077 6865 7468 6572 2063 7572  Sets whether cur
+00012fd0: 7265 6e74 2064 6174 6520 6973 2069 6e20  rent date is in 
+00012fe0: 7468 6520 4f6e 2053 6372 6565 6e20 4469  the On Screen Di
+00012ff0: 7370 6c61 7922 2222 0a0a 2020 2020 2020  splay"""..      
+00013000: 2020 6966 2073 656c 662e 7573 655f 676c    if self.use_gl
+00013010: 6f62 616c 3a0a 2020 2020 2020 2020 2020  obal:.          
+00013020: 2020 7261 6973 6520 4261 6452 6571 7565    raise BadReque
+00013030: 7374 2822 4361 6d65 7261 2069 7320 7573  st("Camera is us
+00013040: 696e 6720 676c 6f62 616c 2072 6563 6f72  ing global recor
+00013050: 6469 6e67 2073 6574 7469 6e67 732e 2229  ding settings.")
+00013060: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
+00013070: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
+00013080: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013090: 6c66 2e6f 7364 5f73 6574 7469 6e67 732e  lf.osd_settings.
+000130a0: 6973 5f64 6174 655f 656e 6162 6c65 6420  is_date_enabled 
+000130b0: 3d20 656e 6162 6c65 640a 0a20 2020 2020  = enabled..     
+000130c0: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
+000130d0: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
+000130e0: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
+000130f0: 6465 6620 7365 745f 6f73 645f 6c6f 676f  def set_osd_logo
+00013100: 2873 656c 662c 2065 6e61 626c 6564 3a20  (self, enabled: 
+00013110: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
+00013120: 2020 2020 2020 2022 2222 5365 7473 2077         """Sets w
+00013130: 6865 7468 6572 2074 6865 2055 6e69 4669  hether the UniFi
+00013140: 206c 6f67 6f20 6973 2069 6e20 7468 6520   logo is in the 
+00013150: 4f6e 2053 6372 6565 6e20 4469 7370 6c61  On Screen Displa
+00013160: 7922 2222 0a0a 2020 2020 2020 2020 6966  y"""..        if
+00013170: 2073 656c 662e 7573 655f 676c 6f62 616c   self.use_global
+00013180: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00013190: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
+000131a0: 4361 6d65 7261 2069 7320 7573 696e 6720  Camera is using 
+000131b0: 676c 6f62 616c 2072 6563 6f72 6469 6e67  global recording
+000131c0: 2073 6574 7469 6e67 732e 2229 0a0a 2020   settings.")..  
+000131d0: 2020 2020 2020 6465 6620 6361 6c6c 6261        def callba
+000131e0: 636b 2829 202d 3e20 4e6f 6e65 3a0a 2020  ck() -> None:.  
+000131f0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+00013200: 7364 5f73 6574 7469 6e67 732e 6973 5f6c  sd_settings.is_l
+00013210: 6f67 6f5f 656e 6162 6c65 6420 3d20 656e  ogo_enabled = en
+00013220: 6162 6c65 640a 0a20 2020 2020 2020 2061  abled..        a
+00013230: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00013240: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00013250: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00013260: 7365 745f 6f73 645f 6269 7472 6174 6528  set_osd_bitrate(
+00013270: 7365 6c66 2c20 656e 6162 6c65 643a 2062  self, enabled: b
+00013280: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+00013290: 2020 2020 2020 2222 2253 6574 7320 7768        """Sets wh
+000132a0: 6574 6865 7220 6361 6d65 7261 2062 6974  ether camera bit
+000132b0: 7261 7465 2069 7320 696e 2074 6865 204f  rate is in the O
+000132c0: 6e20 5363 7265 656e 2044 6973 706c 6179  n Screen Display
+000132d0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+000132e0: 7365 6c66 2e75 7365 5f67 6c6f 6261 6c3a  self.use_global:
+000132f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00013300: 7365 2042 6164 5265 7175 6573 7428 2243  se BadRequest("C
+00013310: 616d 6572 6120 6973 2075 7369 6e67 2067  amera is using g
+00013320: 6c6f 6261 6c20 7265 636f 7264 696e 6720  lobal recording 
+00013330: 7365 7474 696e 6773 2e22 290a 0a20 2020  settings.")..   
+00013340: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+00013350: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+00013360: 2020 2020 2020 2020 2023 206d 6973 6d61           # misma
+00013370: 7463 6820 6265 7477 6565 6e20 5549 2069  tch between UI i
+00013380: 6e74 6572 6e61 6c20 6461 7461 2073 7472  nternal data str
+00013390: 7563 7475 7265 2064 6562 7567 203d 2062  ucture debug = b
+000133a0: 6974 7261 7465 2064 6174 610a 2020 2020  itrate data.    
+000133b0: 2020 2020 2020 2020 7365 6c66 2e6f 7364          self.osd
+000133c0: 5f73 6574 7469 6e67 732e 6973 5f64 6562  _settings.is_deb
+000133d0: 7567 5f65 6e61 626c 6564 203d 2065 6e61  ug_enabled = ena
+000133e0: 626c 6564 0a0a 2020 2020 2020 2020 6177  bled..        aw
+000133f0: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
+00013400: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
+00013410: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
+00013420: 6574 5f73 6d61 7274 5f64 6574 6563 745f  et_smart_detect_
+00013430: 7479 7065 7328 7365 6c66 2c20 7479 7065  types(self, type
+00013440: 733a 206c 6973 745b 536d 6172 7444 6574  s: list[SmartDet
+00013450: 6563 744f 626a 6563 7454 7970 655d 2920  ectObjectType]) 
+00013460: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00013470: 2022 2222 5365 7473 2063 7572 7265 6e74   """Sets current
+00013480: 2065 6e61 626c 6564 2073 6d61 7274 2064   enabled smart d
+00013490: 6574 6563 7469 6f6e 2074 7970 6573 2e20  etection types. 
+000134a0: 5265 7175 6972 6573 2063 616d 6572 6120  Requires camera 
+000134b0: 746f 2068 6176 6520 736d 6172 7420 6465  to have smart de
+000134c0: 7465 6374 696f 6e22 2222 0a0a 2020 2020  tection"""..    
+000134d0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+000134e0: 6665 6174 7572 655f 666c 6167 732e 6861  feature_flags.ha
+000134f0: 735f 736d 6172 745f 6465 7465 6374 3a0a  s_smart_detect:.
+00013500: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00013510: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
+00013520: 6d65 7261 2064 6f65 7320 6e6f 7420 6861  mera does not ha
+00013530: 7665 2061 2073 6d61 7274 2064 6574 6563  ve a smart detec
+00013540: 7469 6f6e 7322 290a 0a20 2020 2020 2020  tions")..       
+00013550: 2069 6620 7365 6c66 2e75 7365 5f67 6c6f   if self.use_glo
+00013560: 6261 6c3a 0a20 2020 2020 2020 2020 2020  bal:.           
+00013570: 2072 6169 7365 2042 6164 5265 7175 6573   raise BadReques
+00013580: 7428 2243 616d 6572 6120 6973 2075 7369  t("Camera is usi
+00013590: 6e67 2067 6c6f 6261 6c20 7265 636f 7264  ng global record
+000135a0: 696e 6720 7365 7474 696e 6773 2e22 290a  ing settings.").
+000135b0: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
+000135c0: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
+000135d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000135e0: 662e 736d 6172 745f 6465 7465 6374 5f73  f.smart_detect_s
+000135f0: 6574 7469 6e67 732e 6f62 6a65 6374 5f74  ettings.object_t
+00013600: 7970 6573 203d 2074 7970 6573 0a0a 2020  ypes = types..  
+00013610: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00013620: 2e71 7565 7565 5f75 7064 6174 6528 6361  .queue_update(ca
+00013630: 6c6c 6261 636b 290a 0a20 2020 2061 7379  llback)..    asy
+00013640: 6e63 2064 6566 2073 6574 5f73 6d61 7274  nc def set_smart
+00013650: 5f61 7564 696f 5f64 6574 6563 745f 7479  _audio_detect_ty
+00013660: 7065 7328 0a20 2020 2020 2020 2073 656c  pes(.        sel
+00013670: 662c 0a20 2020 2020 2020 2074 7970 6573  f,.        types
+00013680: 3a20 6c69 7374 5b53 6d61 7274 4465 7465  : list[SmartDete
+00013690: 6374 4175 6469 6f54 7970 655d 2c0a 2020  ctAudioType],.  
+000136a0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+000136b0: 2020 2020 2022 2222 5365 7473 2063 7572       """Sets cur
+000136c0: 7265 6e74 2065 6e61 626c 6564 2073 6d61  rent enabled sma
+000136d0: 7274 2061 7564 696f 2064 6574 6563 7469  rt audio detecti
+000136e0: 6f6e 2074 7970 6573 2e20 5265 7175 6972  on types. Requir
+000136f0: 6573 2063 616d 6572 6120 746f 2068 6176  es camera to hav
+00013700: 6520 736d 6172 7420 6465 7465 6374 696f  e smart detectio
+00013710: 6e22 2222 0a0a 2020 2020 2020 2020 6966  n"""..        if
+00013720: 206e 6f74 2073 656c 662e 6665 6174 7572   not self.featur
+00013730: 655f 666c 6167 732e 6861 735f 736d 6172  e_flags.has_smar
+00013740: 745f 6465 7465 6374 3a0a 2020 2020 2020  t_detect:.      
+00013750: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
+00013760: 6571 7565 7374 2822 4361 6d65 7261 2064  equest("Camera d
+00013770: 6f65 7320 6e6f 7420 6861 7665 2061 2073  oes not have a s
+00013780: 6d61 7274 2064 6574 6563 7469 6f6e 7322  mart detections"
+00013790: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+000137a0: 6c66 2e75 7365 5f67 6c6f 6261 6c3a 0a20  lf.use_global:. 
+000137b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000137c0: 2042 6164 5265 7175 6573 7428 2243 616d   BadRequest("Cam
+000137d0: 6572 6120 6973 2075 7369 6e67 2067 6c6f  era is using glo
+000137e0: 6261 6c20 7265 636f 7264 696e 6720 7365  bal recording se
+000137f0: 7474 696e 6773 2e22 290a 0a20 2020 2020  ttings.")..     
+00013800: 2020 2064 6566 2063 616c 6c62 6163 6b28     def callback(
+00013810: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00013820: 2020 2020 2020 2073 656c 662e 736d 6172         self.smar
+00013830: 745f 6465 7465 6374 5f73 6574 7469 6e67  t_detect_setting
+00013840: 732e 6175 6469 6f5f 7479 7065 7320 3d20  s.audio_types = 
+00013850: 7479 7065 730a 0a20 2020 2020 2020 2061  types..        a
+00013860: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00013870: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00013880: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00013890: 5f73 6574 5f6f 626a 6563 745f 6465 7465  _set_object_dete
+000138a0: 6374 280a 2020 2020 2020 2020 7365 6c66  ct(.        self
+000138b0: 2c0a 2020 2020 2020 2020 6f62 6a5f 746f  ,.        obj_to
+000138c0: 5f6d 6f64 3a20 536d 6172 7444 6574 6563  _mod: SmartDetec
+000138d0: 744f 626a 6563 7454 7970 652c 0a20 2020  tObjectType,.   
+000138e0: 2020 2020 2065 6e61 626c 6564 3a20 626f       enabled: bo
+000138f0: 6f6c 2c0a 2020 2020 2920 2d3e 204e 6f6e  ol,.    ) -> Non
+00013900: 653a 0a20 2020 2020 2020 2069 6620 6f62  e:.        if ob
+00013910: 6a5f 746f 5f6d 6f64 206e 6f74 2069 6e20  j_to_mod not in 
+00013920: 7365 6c66 2e66 6561 7475 7265 5f66 6c61  self.feature_fla
+00013930: 6773 2e73 6d61 7274 5f64 6574 6563 745f  gs.smart_detect_
+00013940: 7479 7065 733a 0a20 2020 2020 2020 2020  types:.         
+00013950: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+00013960: 6573 7428 6622 4361 6d65 7261 2064 6f65  est(f"Camera doe
+00013970: 7320 6e6f 7420 7375 7070 6f72 7420 7468  s not support th
+00013980: 6520 7b6f 626a 5f74 6f5f 6d6f 647d 2064  e {obj_to_mod} d
+00013990: 6574 6563 7469 6f6e 2074 7970 6522 290a  etection type").
+000139a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000139b0: 2e75 7365 5f67 6c6f 6261 6c3a 0a20 2020  .use_global:.   
+000139c0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+000139d0: 6164 5265 7175 6573 7428 2243 616d 6572  adRequest("Camer
+000139e0: 6120 6973 2075 7369 6e67 2067 6c6f 6261  a is using globa
+000139f0: 6c20 7265 636f 7264 696e 6720 7365 7474  l recording sett
+00013a00: 696e 6773 2e22 290a 0a20 2020 2020 2020  ings.")..       
+00013a10: 2064 6566 2063 616c 6c62 6163 6b28 2920   def callback() 
+00013a20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00013a30: 2020 2020 206f 626a 6563 7473 203d 2073       objects = s
+00013a40: 656c 662e 736d 6172 745f 6465 7465 6374  elf.smart_detect
+00013a50: 5f73 6574 7469 6e67 732e 6f62 6a65 6374  _settings.object
+00013a60: 5f74 7970 6573 0a20 2020 2020 2020 2020  _types.         
+00013a70: 2020 2069 6620 656e 6162 6c65 643a 0a20     if enabled:. 
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013a90: 6620 6f62 6a5f 746f 5f6d 6f64 206e 6f74  f obj_to_mod not
+00013aa0: 2069 6e20 6f62 6a65 6374 733a 0a20 2020   in objects:.   
+00013ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ac0: 206f 626a 6563 7473 203d 205b 2a6f 626a   objects = [*obj
+00013ad0: 6563 7473 2c20 6f62 6a5f 746f 5f6d 6f64  ects, obj_to_mod
+00013ae0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00013af0: 2020 2020 2020 6f62 6a65 6374 732e 736f        objects.so
+00013b00: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
+00013b10: 2065 6c69 6620 6f62 6a5f 746f 5f6d 6f64   elif obj_to_mod
+00013b20: 2069 6e20 6f62 6a65 6374 733a 0a20 2020   in objects:.   
+00013b30: 2020 2020 2020 2020 2020 2020 206f 626a               obj
+00013b40: 6563 7473 2e72 656d 6f76 6528 6f62 6a5f  ects.remove(obj_
+00013b50: 746f 5f6d 6f64 290a 2020 2020 2020 2020  to_mod).        
+00013b60: 2020 2020 7365 6c66 2e73 6d61 7274 5f64      self.smart_d
+00013b70: 6574 6563 745f 7365 7474 696e 6773 2e6f  etect_settings.o
+00013b80: 626a 6563 745f 7479 7065 7320 3d20 6f62  bject_types = ob
+00013b90: 6a65 6374 730a 0a20 2020 2020 2020 2061  jects..        a
+00013ba0: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00013bb0: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00013bc0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00013bd0: 5f73 6574 5f61 7564 696f 5f64 6574 6563  _set_audio_detec
+00013be0: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+00013bf0: 0a20 2020 2020 2020 206f 626a 5f74 6f5f  .        obj_to_
+00013c00: 6d6f 643a 2053 6d61 7274 4465 7465 6374  mod: SmartDetect
+00013c10: 4175 6469 6f54 7970 652c 0a20 2020 2020  AudioType,.     
+00013c20: 2020 2065 6e61 626c 6564 3a20 626f 6f6c     enabled: bool
+00013c30: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00013c40: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+00013c50: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00013c60: 6561 7475 7265 5f66 6c61 6773 2e73 6d61  eature_flags.sma
+00013c70: 7274 5f64 6574 6563 745f 6175 6469 6f5f  rt_detect_audio_
+00013c80: 7479 7065 7320 6973 204e 6f6e 650a 2020  types is None.  
+00013c90: 2020 2020 2020 2020 2020 6f72 206f 626a            or obj
+00013ca0: 5f74 6f5f 6d6f 6420 6e6f 7420 696e 2073  _to_mod not in s
+00013cb0: 656c 662e 6665 6174 7572 655f 666c 6167  elf.feature_flag
+00013cc0: 732e 736d 6172 745f 6465 7465 6374 5f61  s.smart_detect_a
+00013cd0: 7564 696f 5f74 7970 6573 0a20 2020 2020  udio_types.     
+00013ce0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00013cf0: 2020 7261 6973 6520 4261 6452 6571 7565    raise BadReque
+00013d00: 7374 2866 2243 616d 6572 6120 646f 6573  st(f"Camera does
+00013d10: 206e 6f74 2073 7570 706f 7274 2074 6865   not support the
+00013d20: 207b 6f62 6a5f 746f 5f6d 6f64 7d20 6465   {obj_to_mod} de
+00013d30: 7465 6374 696f 6e20 7479 7065 2229 0a0a  tection type")..
+00013d40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013d50: 7573 655f 676c 6f62 616c 3a0a 2020 2020  use_global:.    
+00013d60: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+00013d70: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
+00013d80: 2069 7320 7573 696e 6720 676c 6f62 616c   is using global
+00013d90: 2072 6563 6f72 6469 6e67 2073 6574 7469   recording setti
+00013da0: 6e67 732e 2229 0a0a 2020 2020 2020 2020  ngs.")..        
+00013db0: 6465 6620 6361 6c6c 6261 636b 2829 202d  def callback() -
+00013dc0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00013dd0: 2020 2020 6f62 6a65 6374 7320 3d20 7365      objects = se
+00013de0: 6c66 2e73 6d61 7274 5f64 6574 6563 745f  lf.smart_detect_
+00013df0: 7365 7474 696e 6773 2e61 7564 696f 5f74  settings.audio_t
+00013e00: 7970 6573 206f 7220 5b5d 0a20 2020 2020  ypes or [].     
+00013e10: 2020 2020 2020 2069 6620 656e 6162 6c65         if enable
+00013e20: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+00013e30: 2020 2069 6620 6f62 6a5f 746f 5f6d 6f64     if obj_to_mod
+00013e40: 206e 6f74 2069 6e20 6f62 6a65 6374 733a   not in objects:
+00013e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e60: 2020 2020 206f 626a 6563 7473 203d 205b       objects = [
+00013e70: 2a6f 626a 6563 7473 2c20 6f62 6a5f 746f  *objects, obj_to
+00013e80: 5f6d 6f64 5d0a 2020 2020 2020 2020 2020  _mod].          
+00013e90: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+00013ea0: 732e 736f 7274 2829 0a20 2020 2020 2020  s.sort().       
+00013eb0: 2020 2020 2065 6c69 6620 6f62 6a5f 746f       elif obj_to
+00013ec0: 5f6d 6f64 2069 6e20 6f62 6a65 6374 733a  _mod in objects:
+00013ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ee0: 206f 626a 6563 7473 2e72 656d 6f76 6528   objects.remove(
+00013ef0: 6f62 6a5f 746f 5f6d 6f64 290a 2020 2020  obj_to_mod).    
+00013f00: 2020 2020 2020 2020 7365 6c66 2e73 6d61          self.sma
+00013f10: 7274 5f64 6574 6563 745f 7365 7474 696e  rt_detect_settin
+00013f20: 6773 2e61 7564 696f 5f74 7970 6573 203d  gs.audio_types =
+00013f30: 206f 626a 6563 7473 0a0a 2020 2020 2020   objects..      
+00013f40: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
+00013f50: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
+00013f60: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
+00013f70: 6566 2073 6574 5f6c 6364 5f74 6578 7428  ef set_lcd_text(
+00013f80: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00013f90: 2020 2020 2020 2074 6578 745f 7479 7065         text_type
+00013fa0: 3a20 4f70 7469 6f6e 616c 5b44 6f6f 7262  : Optional[Doorb
+00013fb0: 656c 6c4d 6573 7361 6765 5479 7065 5d2c  ellMessageType],
+00013fc0: 0a20 2020 2020 2020 2074 6578 743a 204f  .        text: O
+00013fd0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00013fe0: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
+00013ff0: 6574 5f61 743a 2055 6e69 6f6e 5b4e 6f6e  et_at: Union[Non
+00014000: 652c 2064 6174 6574 696d 652c 2044 4546  e, datetime, DEF
+00014010: 4155 4c54 5f54 5950 455d 203d 204e 6f6e  AULT_TYPE] = Non
+00014020: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
+00014030: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+00014040: 7320 646f 6f72 6265 6c6c 204c 4344 2074  s doorbell LCD t
+00014050: 6578 742e 2052 6571 7569 7265 7320 6361  ext. Requires ca
+00014060: 6d65 7261 2074 6f20 6265 2064 6f6f 7262  mera to be doorb
+00014070: 656c 6c22 2222 0a0a 2020 2020 2020 2020  ell"""..        
+00014080: 6966 206e 6f74 2073 656c 662e 6665 6174  if not self.feat
+00014090: 7572 655f 666c 6167 732e 6861 735f 6c63  ure_flags.has_lc
+000140a0: 645f 7363 7265 656e 3a0a 2020 2020 2020  d_screen:.      
+000140b0: 2020 2020 2020 7261 6973 6520 4261 6452        raise BadR
+000140c0: 6571 7565 7374 2822 4361 6d65 7261 2064  equest("Camera d
+000140d0: 6f65 7320 6e6f 7420 6861 7665 2061 6e20  oes not have an 
+000140e0: 4c43 4420 7363 7265 656e 2229 0a0a 2020  LCD screen")..  
+000140f0: 2020 2020 2020 6966 2074 6578 745f 7479        if text_ty
+00014100: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00014110: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+00014120: 7468 2073 656c 662e 5f75 7064 6174 655f  th self._update_
+00014130: 6c6f 636b 3a0a 2020 2020 2020 2020 2020  lock:.          
+00014140: 2020 2020 2020 6177 6169 7420 6173 796e        await asyn
+00014150: 6369 6f2e 736c 6565 7028 0a20 2020 2020  cio.sleep(.     
+00014160: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00014170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014180: 2020 2920 2023 2079 6965 6c64 2074 6f20    )  # yield to 
+00014190: 7468 6520 6576 656e 7420 6c6f 6f70 206f  the event loop o
+000141a0: 6e63 6520 7765 2068 6176 6520 7468 6520  nce we have the 
+000141b0: 6c6f 636b 2074 6f20 7072 6f63 6573 7320  lock to process 
+000141c0: 616e 7920 7065 6e64 696e 6720 7570 6461  any pending upda
+000141d0: 7465 730a 2020 2020 2020 2020 2020 2020  tes.            
+000141e0: 2020 2020 6461 7461 5f62 6566 6f72 655f      data_before_
+000141f0: 6368 616e 6765 7320 3d20 7365 6c66 2e64  changes = self.d
+00014200: 6963 745f 7769 7468 5f65 7863 6c75 6465  ict_with_exclude
+00014210: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00014220: 2020 2020 7365 6c66 2e6c 6364 5f6d 6573      self.lcd_mes
+00014230: 7361 6765 203d 204e 6f6e 650a 2020 2020  sage = None.    
+00014240: 2020 2020 2020 2020 2020 2020 2320 556e              # Un
+00014250: 6946 6920 5072 6f74 6563 7420 6275 673a  iFi Protect bug:
+00014260: 2063 6c65 6172 696e 6720 4c43 4420 7465   clearing LCD te
+00014270: 7874 206d 6573 7361 6765 2064 6f65 7320  xt message does 
+00014280: 5f6e 6f74 5f20 656d 6974 2061 2057 5320  _not_ emit a WS 
+00014290: 6d65 7373 6167 650a 2020 2020 2020 2020  message.        
+000142a0: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+000142b0: 6c66 2e73 6176 655f 6465 7669 6365 2864  lf.save_device(d
+000142c0: 6174 615f 6265 666f 7265 5f63 6861 6e67  ata_before_chang
+000142d0: 6573 2c20 666f 7263 655f 656d 6974 3d54  es, force_emit=T
+000142e0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+000142f0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+00014300: 2020 2020 2069 6620 7465 7874 5f74 7970       if text_typ
+00014310: 6520 213d 2044 6f6f 7262 656c 6c4d 6573  e != DoorbellMes
+00014320: 7361 6765 5479 7065 2e43 5553 544f 4d5f  sageType.CUSTOM_
+00014330: 4d45 5353 4147 453a 0a20 2020 2020 2020  MESSAGE:.       
+00014340: 2020 2020 2069 6620 7465 7874 2069 7320       if text is 
+00014350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014360: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00014370: 4261 6452 6571 7565 7374 2822 4361 6e20  BadRequest("Can 
+00014380: 6f6e 6c79 2073 6574 2074 6578 7420 6966  only set text if
+00014390: 2074 6578 745f 7479 7065 2069 7320 4355   text_type is CU
+000143a0: 5354 4f4d 5f4d 4553 5341 4745 2229 0a20  STOM_MESSAGE"). 
+000143b0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+000143c0: 3d20 7465 7874 5f74 7970 652e 7661 6c75  = text_type.valu
+000143d0: 652e 7265 706c 6163 6528 225f 222c 2022  e.replace("_", "
+000143e0: 2022 290a 0a20 2020 2020 2020 2069 6620   ")..        if 
+000143f0: 7265 7365 745f 6174 203d 3d20 4445 4641  reset_at == DEFA
+00014400: 554c 543a 0a20 2020 2020 2020 2020 2020  ULT:.           
+00014410: 2072 6573 6574 5f61 7420 3d20 280a 2020   reset_at = (.  
+00014420: 2020 2020 2020 2020 2020 2020 2020 7574                ut
+00014430: 635f 6e6f 7728 290a 2020 2020 2020 2020  c_now().        
+00014440: 2020 2020 2020 2020 2b20 7365 6c66 2e61          + self.a
+00014450: 7069 2e62 6f6f 7473 7472 6170 2e6e 7672  pi.bootstrap.nvr
+00014460: 2e64 6f6f 7262 656c 6c5f 7365 7474 696e  .doorbell_settin
+00014470: 6773 2e64 6566 6175 6c74 5f6d 6573 7361  gs.default_messa
+00014480: 6765 5f72 6573 6574 5f74 696d 656f 7574  ge_reset_timeout
+00014490: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+000144a0: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
+000144b0: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
+000144c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000144d0: 2e6c 6364 5f6d 6573 7361 6765 203d 204c  .lcd_message = L
+000144e0: 4344 4d65 7373 6167 6528 2020 2320 7479  CDMessage(  # ty
+000144f0: 7065 3a20 6967 6e6f 7265 5b63 616c 6c2d  pe: ignore[call-
+00014500: 6172 675d 0a20 2020 2020 2020 2020 2020  arg].           
+00014510: 2020 2020 2061 7069 3d73 656c 662e 5f61       api=self._a
+00014520: 7069 2c0a 2020 2020 2020 2020 2020 2020  pi,.            
+00014530: 2020 2020 7479 7065 3d74 6578 745f 7479      type=text_ty
+00014540: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+00014550: 2020 2020 7465 7874 3d74 6578 742c 2020      text=text,  
+00014560: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
+00014570: 7267 2d74 7970 655d 0a20 2020 2020 2020  rg-type].       
+00014580: 2020 2020 2020 2020 2072 6573 6574 5f61           reset_a
+00014590: 743d 7265 7365 745f 6174 2c20 2023 2074  t=reset_at,  # t
+000145a0: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
+000145b0: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
+000145c0: 2020 290a 0a20 2020 2020 2020 2061 7761    )..        awa
+000145d0: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
+000145e0: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
+000145f0: 2020 2020 6173 796e 6320 6465 6620 7365      async def se
+00014600: 745f 7072 6976 6163 7928 0a20 2020 2020  t_privacy(.     
+00014610: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00014620: 2065 6e61 626c 6564 3a20 626f 6f6c 2c0a   enabled: bool,.
+00014630: 2020 2020 2020 2020 6d69 635f 6c65 7665          mic_leve
+00014640: 6c3a 204f 7074 696f 6e61 6c5b 696e 745d  l: Optional[int]
+00014650: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00014660: 2072 6563 6f72 6469 6e67 5f6d 6f64 653a   recording_mode:
+00014670: 204f 7074 696f 6e61 6c5b 5265 636f 7264   Optional[Record
+00014680: 696e 674d 6f64 655d 203d 204e 6f6e 652c  ingMode] = None,
+00014690: 0a20 2020 2020 2020 2072 6565 6e61 626c  .        reenabl
+000146a0: 655f 676c 6f62 616c 3a20 626f 6f6c 203d  e_global: bool =
+000146b0: 2046 616c 7365 2c0a 2020 2020 2920 2d3e   False,.    ) ->
+000146c0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000146d0: 2222 4164 6473 2f72 656d 6f76 6573 2061  ""Adds/removes a
+000146e0: 2070 7269 7661 6379 207a 6f6e 6520 7468   privacy zone th
+000146f0: 6174 2062 6c61 636b 7320 6f75 7420 7468  at blacks out th
+00014700: 6520 7768 6f6c 6520 6361 6d65 7261 2e22  e whole camera."
+00014710: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+00014720: 6f74 2073 656c 662e 6665 6174 7572 655f  ot self.feature_
+00014730: 666c 6167 732e 6861 735f 7072 6976 6163  flags.has_privac
+00014740: 795f 6d61 736b 3a0a 2020 2020 2020 2020  y_mask:.        
+00014750: 2020 2020 7261 6973 6520 4261 6452 6571      raise BadReq
+00014760: 7565 7374 2822 4361 6d65 7261 2064 6f65  uest("Camera doe
+00014770: 7320 6e6f 7420 616c 6c6f 7720 7072 6976  s not allow priv
+00014780: 6163 7920 7a6f 6e65 7322 290a 0a20 2020  acy zones")..   
+00014790: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+000147a0: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+000147b0: 2020 2020 2020 2020 2069 6620 656e 6162           if enab
+000147c0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+000147d0: 2020 2020 2073 656c 662e 7573 655f 676c       self.use_gl
+000147e0: 6f62 616c 203d 2046 616c 7365 0a20 2020  obal = False.   
+000147f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014800: 662e 6164 645f 7072 6976 6163 795f 7a6f  f.add_privacy_zo
+00014810: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
+00014820: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00014830: 2020 2020 2020 2069 6620 7265 656e 6162         if reenab
+00014840: 6c65 5f67 6c6f 6261 6c3a 0a20 2020 2020  le_global:.     
+00014850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014860: 656c 662e 7573 655f 676c 6f62 616c 203d  elf.use_global =
+00014870: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00014880: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
+00014890: 655f 7072 6976 6163 795f 7a6f 6e65 2829  e_privacy_zone()
+000148a0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000148b0: 206e 6f74 2072 6565 6e61 626c 655f 676c   not reenable_gl
+000148c0: 6f62 616c 3a0a 2020 2020 2020 2020 2020  obal:.          
+000148d0: 2020 2020 2020 6966 206d 6963 5f6c 6576        if mic_lev
+000148e0: 656c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  el is not None:.
+000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014900: 2020 2020 7365 6c66 2e6d 6963 5f76 6f6c      self.mic_vol
+00014910: 756d 6520 3d20 5065 7263 656e 7449 6e74  ume = PercentInt
+00014920: 286d 6963 5f6c 6576 656c 290a 0a20 2020  (mic_level)..   
+00014930: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014940: 7265 636f 7264 696e 675f 6d6f 6465 2069  recording_mode i
+00014950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00014960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014970: 7365 6c66 2e72 6563 6f72 6469 6e67 5f73  self.recording_s
+00014980: 6574 7469 6e67 732e 6d6f 6465 203d 2072  ettings.mode = r
+00014990: 6563 6f72 6469 6e67 5f6d 6f64 650a 0a20  ecording_mode.. 
+000149a0: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+000149b0: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
+000149c0: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
+000149d0: 796e 6320 6465 6620 7365 745f 7065 7273  ync def set_pers
+000149e0: 6f6e 5f74 7261 636b 2873 656c 662c 2065  on_track(self, e
+000149f0: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
+00014a00: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00014a10: 2222 5365 7473 2070 6572 736f 6e20 7472  ""Sets person tr
+00014a20: 6163 6b69 6e67 206f 6e20 6361 6d65 7261  acking on camera
+00014a30: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00014a40: 6e6f 7420 7365 6c66 2e66 6561 7475 7265  not self.feature
+00014a50: 5f66 6c61 6773 2e69 735f 7074 7a3a 0a20  _flags.is_ptz:. 
+00014a60: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00014a70: 2042 6164 5265 7175 6573 7428 2243 616d   BadRequest("Cam
+00014a80: 6572 6120 646f 6573 206e 6f74 2073 7570  era does not sup
+00014a90: 706f 7274 2070 6572 736f 6e20 7472 6163  port person trac
+00014aa0: 6b69 6e67 2229 0a0a 2020 2020 2020 2020  king")..        
+00014ab0: 6966 2073 656c 662e 7573 655f 676c 6f62  if self.use_glob
+00014ac0: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
+00014ad0: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
+00014ae0: 2822 4361 6d65 7261 2069 7320 7573 696e  ("Camera is usin
+00014af0: 6720 676c 6f62 616c 2072 6563 6f72 6469  g global recordi
+00014b00: 6e67 2073 6574 7469 6e67 732e 2229 0a0a  ng settings.")..
+00014b10: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
+00014b20: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
+00014b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014b40: 2e73 6d61 7274 5f64 6574 6563 745f 7365  .smart_detect_se
+00014b50: 7474 696e 6773 2e61 7574 6f5f 7472 6163  ttings.auto_trac
+00014b60: 6b69 6e67 5f6f 626a 6563 745f 7479 7065  king_object_type
+00014b70: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
+00014b80: 2020 2020 2020 5b53 6d61 7274 4465 7465        [SmartDete
+00014b90: 6374 4f62 6a65 6374 5479 7065 2e50 4552  ctObjectType.PER
+00014ba0: 534f 4e5d 2069 6620 656e 6162 6c65 6420  SON] if enabled 
+00014bb0: 656c 7365 205b 5d0a 2020 2020 2020 2020  else [].        
+00014bc0: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
+00014bd0: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00014be0: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00014bf0: 0a0a 2020 2020 6465 6620 6372 6561 7465  ..    def create
+00014c00: 5f74 616c 6b62 6163 6b5f 7374 7265 616d  _talkback_stream
+00014c10: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00014c20: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+00014c30: 7572 6c3a 2073 7472 2c0a 2020 2020 2020  url: str,.      
+00014c40: 2020 6666 6d70 6567 5f70 6174 683a 204f    ffmpeg_path: O
+00014c50: 7074 696f 6e61 6c5b 5061 7468 5d20 3d20  ptional[Path] = 
+00014c60: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2054  None,.    ) -> T
+00014c70: 616c 6b62 6163 6b53 7472 6561 6d3a 0a20  alkbackStream:. 
+00014c80: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
+00014c90: 7320 6120 7375 6270 726f 6365 7373 2074  s a subprocess t
+00014ca0: 6f20 706c 6179 2061 7564 696f 2074 6f20  o play audio to 
+00014cb0: 6120 6361 6d65 7261 2074 6872 6f75 6768  a camera through
+00014cc0: 2069 7473 2073 7065 616b 6572 2e0a 0a20   its speaker... 
+00014cd0: 2020 2020 2020 2052 6571 7569 7265 7320         Requires 
+00014ce0: 6666 6d70 6567 2074 6f20 7573 652e 0a0a  ffmpeg to use...
+00014cf0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00014d00: 2020 2020 2020 2d2d 2d2d 0a20 2020 2020        ----.     
+00014d10: 2020 2020 2020 2063 6f6e 7465 6e74 5f75         content_u
+00014d20: 726c 3a20 4569 7468 6572 2061 2055 524c  rl: Either a URL
+00014d30: 2061 6363 6573 7369 626c 6520 6279 2070   accessible by p
+00014d40: 7974 686f 6e20 6f72 2061 2070 6174 6820  ython or a path 
+00014d50: 746f 2061 2066 696c 6520 2866 666d 6570  to a file (ffmep
+00014d60: 6727 7320 602d 6960 2070 6172 616d 6574  g's `-i` paramet
+00014d70: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
+00014d80: 6666 6d70 6567 5f70 6174 683a 204f 7074  ffmpeg_path: Opt
+00014d90: 696f 6e61 6c20 7061 7468 2074 6f20 6666  ional path to ff
+00014da0: 6d70 6567 2062 696e 6172 790a 0a20 2020  mpeg binary..   
+00014db0: 2020 2020 2055 7365 2065 6974 6865 7220       Use either 
+00014dc0: 6061 7761 6974 2073 7472 6561 6d2e 7275  `await stream.ru
+00014dd0: 6e5f 756e 7469 6c5f 636f 6d70 6c65 7465  n_until_complete
+00014de0: 2829 6020 6f72 2060 6177 6169 7420 7374  ()` or `await st
+00014df0: 7265 616d 2e73 7461 7274 2829 6020 746f  ream.start()` to
+00014e00: 2073 7461 7274 2073 7562 7072 6f63 6573   start subproces
+00014e10: 7320 636f 6d6d 616e 640a 2020 2020 2020  s command.      
+00014e20: 2020 6166 7465 7220 6765 7474 696e 6720    after getting 
+00014e30: 7468 6520 7374 7265 616d 2e0a 0a20 2020  the stream...   
+00014e40: 2020 2020 2060 2e70 6c61 795f 6175 6469       `.play_audi
+00014e50: 6f28 2960 2069 7320 6120 6865 6c70 6572  o()` is a helper
+00014e60: 2074 6861 7420 7772 6170 7320 7468 6973   that wraps this
+00014e70: 206d 6574 686f 6420 616e 6420 6175 746f   method and auto
+00014e80: 6d61 7469 6361 6c6c 7920 7275 6e73 2074  matically runs t
+00014e90: 6865 2073 7562 7072 6f63 6573 7320 6173  he subprocess as
+00014ea0: 2077 656c 6c0a 2020 2020 2020 2020 2222   well.        ""
+00014eb0: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00014ec0: 6c66 2e74 616c 6b62 6163 6b5f 7374 7265  lf.talkback_stre
+00014ed0: 616d 2069 7320 6e6f 7420 4e6f 6e65 2061  am is not None a
+00014ee0: 6e64 2073 656c 662e 7461 6c6b 6261 636b  nd self.talkback
+00014ef0: 5f73 7472 6561 6d2e 6973 5f72 756e 6e69  _stream.is_runni
+00014f00: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00014f10: 7261 6973 6520 4261 6452 6571 7565 7374  raise BadRequest
+00014f20: 2822 4361 6d65 7261 2069 7320 616c 7265  ("Camera is alre
+00014f30: 6164 7920 706c 6179 696e 6720 6175 6469  ady playing audi
+00014f40: 6f22 290a 0a20 2020 2020 2020 2073 656c  o")..        sel
+00014f50: 662e 7461 6c6b 6261 636b 5f73 7472 6561  f.talkback_strea
+00014f60: 6d20 3d20 5461 6c6b 6261 636b 5374 7265  m = TalkbackStre
+00014f70: 616d 2873 656c 662c 2063 6f6e 7465 6e74  am(self, content
+00014f80: 5f75 726c 2c20 6666 6d70 6567 5f70 6174  _url, ffmpeg_pat
+00014f90: 6829 0a20 2020 2020 2020 2072 6574 7572  h).        retur
+00014fa0: 6e20 7365 6c66 2e74 616c 6b62 6163 6b5f  n self.talkback_
+00014fb0: 7374 7265 616d 0a0a 2020 2020 6173 796e  stream..    asyn
+00014fc0: 6320 6465 6620 706c 6179 5f61 7564 696f  c def play_audio
+00014fd0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00014fe0: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+00014ff0: 7572 6c3a 2073 7472 2c0a 2020 2020 2020  url: str,.      
+00015000: 2020 6666 6d70 6567 5f70 6174 683a 204f    ffmpeg_path: O
+00015010: 7074 696f 6e61 6c5b 5061 7468 5d20 3d20  ptional[Path] = 
+00015020: 4e6f 6e65 2c0a 2020 2020 2020 2020 626c  None,.        bl
+00015030: 6f63 6b69 6e67 3a20 626f 6f6c 203d 2054  ocking: bool = T
+00015040: 7275 652c 0a20 2020 2029 202d 3e20 4e6f  rue,.    ) -> No
+00015050: 6e65 3a0a 2020 2020 2020 2020 2222 2250  ne:.        """P
+00015060: 6c61 7973 2061 7564 696f 2074 6f20 6120  lays audio to a 
+00015070: 6361 6d65 7261 2074 6872 6f75 6768 2069  camera through i
+00015080: 7473 2073 7065 616b 6572 2e0a 0a20 2020  ts speaker...   
+00015090: 2020 2020 2052 6571 7569 7265 7320 6666       Requires ff
+000150a0: 6d70 6567 2074 6f20 7573 652e 0a0a 2020  mpeg to use...  
+000150b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000150c0: 2020 2020 2d2d 2d2d 0a20 2020 2020 2020      ----.       
+000150d0: 2020 2020 2063 6f6e 7465 6e74 5f75 726c       content_url
+000150e0: 3a20 4569 7468 6572 2061 2055 524c 2061  : Either a URL a
+000150f0: 6363 6573 7369 626c 6520 6279 2070 7974  ccessible by pyt
+00015100: 686f 6e20 6f72 2061 2070 6174 6820 746f  hon or a path to
+00015110: 2061 2066 696c 6520 2866 666d 6570 6727   a file (ffmepg'
+00015120: 7320 602d 6960 2070 6172 616d 6574 6572  s `-i` parameter
+00015130: 290a 2020 2020 2020 2020 2020 2020 6666  ).            ff
+00015140: 6d70 6567 5f70 6174 683a 204f 7074 696f  mpeg_path: Optio
+00015150: 6e61 6c20 7061 7468 2074 6f20 6666 6d70  nal path to ffmp
+00015160: 6567 2062 696e 6172 790a 2020 2020 2020  eg binary.      
+00015170: 2020 2020 2020 626c 6f63 6b69 6e67 3a20        blocking: 
+00015180: 4177 6169 7473 2073 7472 6561 6d20 636f  Awaits stream co
+00015190: 6d70 6c65 7469 6f6e 2061 6e64 206c 6f67  mpletion and log
+000151a0: 7320 7374 646f 7574 2f73 7464 6572 720a  s stdout/stderr.
+000151b0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+000151c0: 2020 2020 2073 7472 6561 6d20 3d20 7365       stream = se
+000151d0: 6c66 2e63 7265 6174 655f 7461 6c6b 6261  lf.create_talkba
+000151e0: 636b 5f73 7472 6561 6d28 636f 6e74 656e  ck_stream(conten
+000151f0: 745f 7572 6c2c 2066 666d 7065 675f 7061  t_url, ffmpeg_pa
+00015200: 7468 290a 2020 2020 2020 2020 6177 6169  th).        awai
+00015210: 7420 7374 7265 616d 2e73 7461 7274 2829  t stream.start()
+00015220: 0a0a 2020 2020 2020 2020 6966 2062 6c6f  ..        if blo
+00015230: 636b 696e 673a 0a20 2020 2020 2020 2020  cking:.         
+00015240: 2020 2061 7761 6974 2073 656c 662e 7761     await self.wa
+00015250: 6974 5f75 6e74 696c 5f61 7564 696f 5f63  it_until_audio_c
+00015260: 6f6d 706c 6574 6573 2829 0a0a 2020 2020  ompletes()..    
+00015270: 6173 796e 6320 6465 6620 7761 6974 5f75  async def wait_u
+00015280: 6e74 696c 5f61 7564 696f 5f63 6f6d 706c  ntil_audio_compl
+00015290: 6574 6573 2873 656c 6629 202d 3e20 4e6f  etes(self) -> No
+000152a0: 6e65 3a0a 2020 2020 2020 2020 2222 2241  ne:.        """A
+000152b0: 7761 6974 7320 7374 7265 616d 2063 6f6d  waits stream com
+000152c0: 706c 6574 696f 6e20 6f66 2061 7564 696f  pletion of audio
+000152d0: 2061 6e64 206c 6f67 7320 7374 646f 7574   and logs stdout
+000152e0: 2f73 7464 6572 722e 2222 220a 0a20 2020  /stderr."""..   
+000152f0: 2020 2020 2073 7472 6561 6d20 3d20 7365       stream = se
+00015300: 6c66 2e74 616c 6b62 6163 6b5f 7374 7265  lf.talkback_stre
+00015310: 616d 0a20 2020 2020 2020 2069 6620 7374  am.        if st
+00015320: 7265 616d 2069 7320 4e6f 6e65 3a0a 2020  ream is None:.  
+00015330: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00015340: 5374 7265 616d 4572 726f 7228 224e 6f20  StreamError("No 
+00015350: 6175 6469 6f20 706c 6179 696e 6720 746f  audio playing to
+00015360: 2077 6169 7420 666f 7222 290a 0a20 2020   wait for")..   
+00015370: 2020 2020 2061 7761 6974 2073 7472 6561       await strea
+00015380: 6d2e 7275 6e5f 756e 7469 6c5f 636f 6d70  m.run_until_comp
+00015390: 6c65 7465 2829 0a0a 2020 2020 2020 2020  lete()..        
+000153a0: 5f4c 4f47 4745 522e 6465 6275 6728 2266  _LOGGER.debug("f
+000153b0: 666d 7065 6720 7374 646f 7574 3a5c 6e25  fmpeg stdout:\n%
+000153c0: 7322 2c20 225c 6e22 2e6a 6f69 6e28 7374  s", "\n".join(st
+000153d0: 7265 616d 2e73 7464 6f75 7429 290a 2020  ream.stdout)).  
+000153e0: 2020 2020 2020 5f4c 4f47 4745 522e 6465        _LOGGER.de
+000153f0: 6275 6728 2266 666d 7065 6720 7374 6465  bug("ffmpeg stde
+00015400: 7272 3a5c 6e25 7322 2c20 225c 6e22 2e6a  rr:\n%s", "\n".j
+00015410: 6f69 6e28 7374 7265 616d 2e73 7464 6572  oin(stream.stder
+00015420: 7229 290a 2020 2020 2020 2020 6966 2073  r)).        if s
+00015430: 7472 6561 6d2e 6973 5f65 7272 6f72 3a0a  tream.is_error:.
+00015440: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00015450: 7220 3d20 225c 6e22 2e6a 6f69 6e28 7374  r = "\n".join(st
+00015460: 7265 616d 2e73 7464 6572 7229 0a20 2020  ream.stderr).   
+00015470: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+00015480: 7472 6561 6d45 7272 6f72 2822 4572 726f  treamError("Erro
+00015490: 7220 7768 696c 6520 706c 6179 696e 6720  r while playing 
+000154a0: 6175 6469 6f20 2866 666d 7065 6729 3a20  audio (ffmpeg): 
+000154b0: 5c6e 2220 2b20 6572 726f 7229 0a0a 2020  \n" + error)..  
+000154c0: 2020 6173 796e 6320 6465 6620 7374 6f70    async def stop
+000154d0: 5f61 7564 696f 2873 656c 6629 202d 3e20  _audio(self) -> 
+000154e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000154f0: 2253 746f 7020 6375 7272 656e 746c 7920  "Stop currently 
+00015500: 706c 6179 696e 6720 6175 6469 6f2e 2222  playing audio.""
+00015510: 220a 2020 2020 2020 2020 7374 7265 616d  ".        stream
+00015520: 203d 2073 656c 662e 7461 6c6b 6261 636b   = self.talkback
+00015530: 5f73 7472 6561 6d0a 2020 2020 2020 2020  _stream.        
+00015540: 6966 2073 7472 6561 6d20 6973 204e 6f6e  if stream is Non
+00015550: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00015560: 6169 7365 2053 7472 6561 6d45 7272 6f72  aise StreamError
+00015570: 2822 4e6f 2061 7564 696f 2070 6c61 7969  ("No audio playi
+00015580: 6e67 2074 6f20 7374 6f70 2229 0a0a 2020  ng to stop")..  
+00015590: 2020 2020 2020 6177 6169 7420 7374 7265        await stre
+000155a0: 616d 2e73 746f 7028 290a 0a20 2020 2064  am.stop()..    d
+000155b0: 6566 2063 616e 5f72 6561 645f 6d65 6469  ef can_read_medi
+000155c0: 6128 7365 6c66 2c20 7573 6572 3a20 5573  a(self, user: Us
+000155d0: 6572 2920 2d3e 2062 6f6f 6c3a 0a20 2020  er) -> bool:.   
+000155e0: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+000155f0: 656c 2069 7320 4e6f 6e65 3a0a 2020 2020  el is None:.    
+00015600: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00015610: 7275 650a 0a20 2020 2020 2020 2072 6574  rue..        ret
+00015620: 7572 6e20 7573 6572 2e63 616e 2873 656c  urn user.can(sel
+00015630: 662e 6d6f 6465 6c2c 2050 6572 6d69 7373  f.model, Permiss
+00015640: 696f 6e4e 6f64 652e 5245 4144 5f4d 4544  ionNode.READ_MED
+00015650: 4941 2c20 7365 6c66 290a 0a20 2020 2064  IA, self)..    d
+00015660: 6566 2063 616e 5f64 656c 6574 655f 6d65  ef can_delete_me
+00015670: 6469 6128 7365 6c66 2c20 7573 6572 3a20  dia(self, user: 
+00015680: 5573 6572 2920 2d3e 2062 6f6f 6c3a 0a20  User) -> bool:. 
+00015690: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+000156a0: 6f64 656c 2069 7320 4e6f 6e65 3a0a 2020  odel is None:.  
+000156b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000156c0: 2054 7275 650a 0a20 2020 2020 2020 2072   True..        r
+000156d0: 6574 7572 6e20 7573 6572 2e63 616e 2873  eturn user.can(s
+000156e0: 656c 662e 6d6f 6465 6c2c 2050 6572 6d69  elf.model, Permi
+000156f0: 7373 696f 6e4e 6f64 652e 4445 4c45 5445  ssionNode.DELETE
+00015700: 5f4d 4544 4941 2c20 7365 6c66 290a 0a20  _MEDIA, self).. 
+00015710: 2020 2023 2072 6567 696f 6e20 5054 5a0a     # region PTZ.
+00015720: 0a20 2020 2061 7379 6e63 2064 6566 2070  .    async def p
+00015730: 747a 5f72 656c 6174 6976 655f 6d6f 7665  tz_relative_move
+00015740: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00015750: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+00015760: 2020 2070 616e 3a20 666c 6f61 742c 0a20     pan: float,. 
+00015770: 2020 2020 2020 2074 696c 743a 2066 6c6f         tilt: flo
+00015780: 6174 2c0a 2020 2020 2020 2020 7061 6e5f  at,.        pan_
+00015790: 7370 6565 643a 2069 6e74 203d 2031 302c  speed: int = 10,
+000157a0: 0a20 2020 2020 2020 2074 696c 745f 7370  .        tilt_sp
+000157b0: 6565 643a 2069 6e74 203d 2031 302c 0a20  eed: int = 10,. 
+000157c0: 2020 2020 2020 2073 6361 6c65 3a20 696e         scale: in
+000157d0: 7420 3d20 302c 0a20 2020 2020 2020 2075  t = 0,.        u
+000157e0: 7365 5f6e 6174 6976 653a 2062 6f6f 6c20  se_native: bool 
+000157f0: 3d20 4661 6c73 652c 0a20 2020 2029 202d  = False,.    ) -
+00015800: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00015810: 2222 224d 6f76 6520 5054 5a20 7265 6c61  """Move PTZ rela
+00015820: 7469 7665 2074 6f20 6375 7272 656e 7420  tive to current 
+00015830: 706f 7369 7469 6f6e 2e0a 0a20 2020 2020  position...     
+00015840: 2020 2050 616e 2f74 696c 7420 7661 6c75     Pan/tilt valu
+00015850: 6573 2076 6172 7920 6672 6f6d 2063 616d  es vary from cam
+00015860: 6572 6120 746f 2063 616d 6572 612c 2062  era to camera, b
+00015870: 7574 2066 6f72 2047 3420 5054 5a3a 0a20  ut for G4 PTZ:. 
+00015880: 2020 2020 2020 2020 2020 202a 2050 616e             * Pan
+00015890: 2076 616c 7565 7320 7261 6e67 6520 6672   values range fr
+000158a0: 6f6d 2030 c2b0 2061 6e64 2067 6f20 746f  om 0.. and go to
+000158b0: 2033 3630 c2b0 2f30 c2b0 0a20 2020 2020   360../0...     
+000158c0: 2020 2020 2020 202a 2054 696c 7420 7661         * Tilt va
+000158d0: 6c75 6573 2072 616e 6765 2066 726f 6d20  lues range from 
+000158e0: 2d32 30c2 b020 616e 6420 676f 2074 6f20  -20.. and go to 
+000158f0: 3930 c2b0 0a0a 2020 2020 2020 2020 5265  90....        Re
+00015900: 6c61 7469 7665 2070 6f73 6974 696f 6e73  lative positions
+00015910: 2063 616e 6e6f 7420 6d6f 7665 206d 6f72   cannot move mor
+00015920: 6520 7468 656e 2034 3039 3520 7374 6570  e then 4095 step
+00015930: 7320 6174 2061 2074 696d 6520 696e 2061  s at a time in a
+00015940: 6e79 2064 6972 6563 7469 6f6e 2e0a 0a20  ny direction... 
+00015950: 2020 2020 2020 2046 6f72 2074 6865 2047         For the G
+00015960: 3420 5054 5a2c 2034 3039 3520 7374 6570  4 PTZ, 4095 step
+00015970: 7320 6973 207e 3431 c2b0 2066 6f72 2070  s is ~41.. for p
+00015980: 616e 2061 6e64 207e 3435 c2b0 2066 6f72  an and ~45.. for
+00015990: 2074 696c 742e 0a0a 2020 2020 2020 2020   tilt...        
+000159a0: 6075 7365 5f6e 6174 6976 6560 206c 6574  `use_native` let
+000159b0: 7320 796f 7520 7573 6520 7468 6520 6e61  s you use the na
+000159c0: 7469 7665 2073 7465 7020 7661 6c75 6573  tive step values
+000159d0: 2069 6e73 7465 6164 206f 6620 6465 6772   instead of degr
+000159e0: 6565 732e 0a20 2020 2020 2020 2022 2222  ees..        """
+000159f0: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00015a00: 2073 656c 662e 6665 6174 7572 655f 666c   self.feature_fl
+00015a10: 6167 732e 6973 5f70 747a 3a0a 2020 2020  ags.is_ptz:.    
+00015a20: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+00015a30: 6452 6571 7565 7374 2822 4361 6d65 7261  dRequest("Camera
+00015a40: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+00015a50: 7420 5054 5a20 6665 6174 7572 6573 2e22  t PTZ features."
+00015a60: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+00015a70: 7420 7573 655f 6e61 7469 7665 3a0a 2020  t use_native:.  
+00015a80: 2020 2020 2020 2020 2020 7061 6e20 3d20            pan = 
+00015a90: 7365 6c66 2e66 6561 7475 7265 5f66 6c61  self.feature_fla
+00015aa0: 6773 2e70 616e 2e74 6f5f 6e61 7469 7665  gs.pan.to_native
+00015ab0: 5f76 616c 7565 2870 616e 2c20 6973 5f72  _value(pan, is_r
+00015ac0: 656c 6174 6976 653d 5472 7565 290a 2020  elative=True).  
+00015ad0: 2020 2020 2020 2020 2020 7469 6c74 203d            tilt =
+00015ae0: 2073 656c 662e 6665 6174 7572 655f 666c   self.feature_fl
+00015af0: 6167 732e 7469 6c74 2e74 6f5f 6e61 7469  ags.tilt.to_nati
+00015b00: 7665 5f76 616c 7565 2874 696c 742c 2069  ve_value(tilt, i
+00015b10: 735f 7265 6c61 7469 7665 3d54 7275 6529  s_relative=True)
+00015b20: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00015b30: 7365 6c66 2e61 7069 2e72 656c 6174 6976  self.api.relativ
+00015b40: 655f 6d6f 7665 5f70 747a 5f63 616d 6572  e_move_ptz_camer
+00015b50: 6128 0a20 2020 2020 2020 2020 2020 2073  a(.            s
+00015b60: 656c 662e 6964 2c0a 2020 2020 2020 2020  elf.id,.        
+00015b70: 2020 2020 7061 6e3d 7061 6e2c 0a20 2020      pan=pan,.   
+00015b80: 2020 2020 2020 2020 2074 696c 743d 7469           tilt=ti
+00015b90: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
+00015ba0: 7061 6e5f 7370 6565 643d 7061 6e5f 7370  pan_speed=pan_sp
+00015bb0: 6565 642c 0a20 2020 2020 2020 2020 2020  eed,.           
+00015bc0: 2074 696c 745f 7370 6565 643d 7469 6c74   tilt_speed=tilt
+00015bd0: 5f73 7065 6564 2c0a 2020 2020 2020 2020  _speed,.        
+00015be0: 2020 2020 7363 616c 653d 7363 616c 652c      scale=scale,
+00015bf0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00015c00: 6173 796e 6320 6465 6620 7074 7a5f 6365  async def ptz_ce
+00015c10: 6e74 6572 2873 656c 662c 202a 2c20 783a  nter(self, *, x:
+00015c20: 2069 6e74 2c20 793a 2069 6e74 2c20 7a3a   int, y: int, z:
+00015c30: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00015c40: 2020 2020 2020 2022 2222 4365 6e74 6572         """Center
+00015c50: 2050 545a 2043 616d 6572 6120 6f6e 2070   PTZ Camera on p
+00015c60: 6f69 6e74 2069 6e20 7669 6577 706f 7274  oint in viewport
+00015c70: 2e0a 0a20 2020 2020 2020 2078 2c20 792c  ...        x, y,
+00015c80: 207a 2076 616c 7565 7320 7261 6e67 6520   z values range 
+00015c90: 6672 6f6d 2030 2074 6f20 3130 3030 2e0a  from 0 to 1000..
+00015ca0: 0a20 2020 2020 2020 2078 2c20 7920 6172  .        x, y ar
+00015cb0: 6520 7265 6c61 7469 7665 2063 6f6f 7264  e relative coord
+00015cc0: 7320 666f 7220 7468 6520 6375 7272 656e  s for the curren
+00015cd0: 7420 7669 6577 706f 7274 3a0a 2020 2020  t viewport:.    
+00015ce0: 2020 2020 2020 2020 2a20 2830 2c20 3029          * (0, 0)
+00015cf0: 2069 7320 746f 7020 6c65 6674 0a20 2020   is top left.   
+00015d00: 2020 2020 2020 2020 202a 2028 3530 302c           * (500,
+00015d10: 2035 3030 2920 6973 2074 6865 2063 656e   500) is the cen
+00015d20: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00015d30: 2a20 2831 3030 302c 2031 3030 3029 2069  * (1000, 1000) i
+00015d40: 7320 7468 6520 626f 7474 6f6d 2072 6967  s the bottom rig
+00015d50: 6874 0a0a 2020 2020 2020 2020 7a20 7661  ht..        z va
+00015d60: 6c75 6520 6973 207a 6f6f 6d2c 2062 7574  lue is zoom, but
+00015d70: 2073 696e 6365 2069 7420 6973 2063 6170   since it is cap
+00015d80: 7065 6420 6174 2031 3030 302c 2070 726f  ped at 1000, pro
+00015d90: 6261 626c 7920 6265 7474 6572 2074 6f20  bably better to 
+00015da0: 7573 6520 6070 747a 5f7a 6f6f 6d60 2e0a  use `ptz_zoom`..
+00015db0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00015dc0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00015dd0: 6170 692e 6365 6e74 6572 5f70 747a 5f63  api.center_ptz_c
+00015de0: 616d 6572 6128 7365 6c66 2e69 642c 2078  amera(self.id, x
+00015df0: 3d78 2c20 793d 792c 207a 3d7a 290a 0a20  =x, y=y, z=z).. 
+00015e00: 2020 2061 7379 6e63 2064 6566 2070 747a     async def ptz
+00015e10: 5f7a 6f6f 6d28 0a20 2020 2020 2020 2073  _zoom(.        s
+00015e20: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+00015e30: 2020 2020 2020 2020 7a6f 6f6d 3a20 666c          zoom: fl
+00015e40: 6f61 742c 0a20 2020 2020 2020 2073 7065  oat,.        spe
+00015e50: 6564 3a20 696e 7420 3d20 3130 302c 0a20  ed: int = 100,. 
+00015e60: 2020 2020 2020 2075 7365 5f6e 6174 6976         use_nativ
+00015e70: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00015e80: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+00015e90: 2020 2020 2020 2020 2222 225a 6f6f 6d20          """Zoom 
+00015ea0: 5054 5a20 4361 6d65 7261 2e0a 0a20 2020  PTZ Camera...   
+00015eb0: 2020 2020 205a 6f6f 6d20 6c65 7665 6c73       Zoom levels
+00015ec0: 2076 6172 7920 6672 6f6d 2063 616d 6572   vary from camer
+00015ed0: 6120 746f 2063 616d 6572 612c 2062 7574  a to camera, but
+00015ee0: 2066 6f72 2047 3420 5054 5a20 6974 2067   for G4 PTZ it g
+00015ef0: 6f65 7320 6672 6f6d 2031 7820 746f 2032  oes from 1x to 2
+00015f00: 3278 2e0a 0a20 2020 2020 2020 205a 6f6f  2x...        Zoo
+00015f10: 6d20 7370 6565 6420 7365 656d 7320 746f  m speed seems to
+00015f20: 2072 616e 6765 2066 726f 6d20 3020 746f   range from 0 to
+00015f30: 2031 3030 2e20 416e 7920 7661 6c75 6520   100. Any value 
+00015f40: 6f76 6572 2031 3030 2072 6573 756c 7473  over 100 results
+00015f50: 2069 6e20 6120 7370 6565 6420 6f66 2030   in a speed of 0
+00015f60: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00015f70: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00015f80: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
+00015f90: 2e69 735f 7074 7a3a 0a20 2020 2020 2020  .is_ptz:.       
+00015fa0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+00015fb0: 7175 6573 7428 2243 616d 6572 6120 646f  quest("Camera do
+00015fc0: 6573 206e 6f74 2073 7570 706f 7274 2050  es not support P
+00015fd0: 545a 2066 6561 7475 7265 732e 2229 0a0a  TZ features.")..
+00015fe0: 2020 2020 2020 2020 6966 206e 6f74 2075          if not u
+00015ff0: 7365 5f6e 6174 6976 653a 0a20 2020 2020  se_native:.     
+00016000: 2020 2020 2020 207a 6f6f 6d20 3d20 7365         zoom = se
+00016010: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
+00016020: 2e7a 6f6f 6d2e 746f 5f6e 6174 6976 655f  .zoom.to_native_
+00016030: 7661 6c75 6528 7a6f 6f6d 290a 0a20 2020  value(zoom)..   
+00016040: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00016050: 6170 692e 7a6f 6f6d 5f70 747a 5f63 616d  api.zoom_ptz_cam
+00016060: 6572 6128 7365 6c66 2e69 642c 207a 6f6f  era(self.id, zoo
+00016070: 6d3d 7a6f 6f6d 2c20 7370 6565 643d 7370  m=zoom, speed=sp
+00016080: 6565 6429 0a0a 2020 2020 6173 796e 6320  eed)..    async 
+00016090: 6465 6620 6765 745f 7074 7a5f 706f 7369  def get_ptz_posi
+000160a0: 7469 6f6e 2873 656c 6629 202d 3e20 5054  tion(self) -> PT
+000160b0: 5a50 6f73 6974 696f 6e3a 0a20 2020 2020  ZPosition:.     
+000160c0: 2020 2022 2222 4765 7420 6375 7272 656e     """Get curren
+000160d0: 7420 5054 5a20 506f 7369 7469 6f6e 2e22  t PTZ Position."
+000160e0: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+000160f0: 6f74 2073 656c 662e 6665 6174 7572 655f  ot self.feature_
+00016100: 666c 6167 732e 6973 5f70 747a 3a0a 2020  flags.is_ptz:.  
+00016110: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00016120: 4261 6452 6571 7565 7374 2822 4361 6d65  BadRequest("Came
+00016130: 7261 2064 6f65 7320 6e6f 7420 7375 7070  ra does not supp
+00016140: 6f72 7420 5054 5a20 6665 6174 7572 6573  ort PTZ features
+00016150: 2e22 290a 0a20 2020 2020 2020 2072 6574  .")..        ret
+00016160: 7572 6e20 6177 6169 7420 7365 6c66 2e61  urn await self.a
+00016170: 7069 2e67 6574 5f70 6f73 6974 696f 6e5f  pi.get_position_
+00016180: 7074 7a5f 6361 6d65 7261 2873 656c 662e  ptz_camera(self.
+00016190: 6964 290a 0a20 2020 2061 7379 6e63 2064  id)..    async d
+000161a0: 6566 2067 6f74 6f5f 7074 7a5f 736c 6f74  ef goto_ptz_slot
+000161b0: 2873 656c 662c 202a 2c20 736c 6f74 3a20  (self, *, slot: 
+000161c0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+000161d0: 2020 2020 2020 2222 2247 6f74 6f20 5054        """Goto PT
+000161e0: 5a20 736c 6f74 2070 6f73 6974 696f 6e2e  Z slot position.
+000161f0: 0a0a 2020 2020 2020 2020 2d31 2069 7320  ..        -1 is 
+00016200: 486f 6d65 2073 6c6f 742e 0a20 2020 2020  Home slot..     
+00016210: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00016220: 6966 206e 6f74 2073 656c 662e 6665 6174  if not self.feat
+00016230: 7572 655f 666c 6167 732e 6973 5f70 747a  ure_flags.is_ptz
+00016240: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00016250: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
+00016260: 4361 6d65 7261 2064 6f65 7320 6e6f 7420  Camera does not 
+00016270: 7375 7070 6f72 7420 5054 5a20 6665 6174  support PTZ feat
+00016280: 7572 6573 2e22 290a 0a20 2020 2020 2020  ures.")..       
+00016290: 2061 7761 6974 2073 656c 662e 6170 692e   await self.api.
+000162a0: 676f 746f 5f70 747a 5f63 616d 6572 6128  goto_ptz_camera(
+000162b0: 7365 6c66 2e69 642c 2073 6c6f 743d 736c  self.id, slot=sl
+000162c0: 6f74 290a 0a20 2020 2061 7379 6e63 2064  ot)..    async d
+000162d0: 6566 2063 7265 6174 655f 7074 7a5f 7072  ef create_ptz_pr
+000162e0: 6573 6574 2873 656c 662c 202a 2c20 6e61  eset(self, *, na
+000162f0: 6d65 3a20 7374 7229 202d 3e20 5054 5a50  me: str) -> PTZP
+00016300: 7265 7365 743a 0a20 2020 2020 2020 2022  reset:.        "
+00016310: 2222 4372 6561 7465 2050 545a 2050 7265  ""Create PTZ Pre
+00016320: 7365 7420 666f 7220 6361 6d65 7261 2062  set for camera b
+00016330: 6173 6564 206f 6e20 6375 7272 656e 7420  ased on current 
+00016340: 6361 6d65 7261 2073 6574 7469 6e67 732e  camera settings.
+00016350: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00016360: 6e6f 7420 7365 6c66 2e66 6561 7475 7265  not self.feature
+00016370: 5f66 6c61 6773 2e69 735f 7074 7a3a 0a20  _flags.is_ptz:. 
+00016380: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00016390: 2042 6164 5265 7175 6573 7428 2243 616d   BadRequest("Cam
+000163a0: 6572 6120 646f 6573 206e 6f74 2073 7570  era does not sup
+000163b0: 706f 7274 2050 545a 2066 6561 7475 7265  port PTZ feature
+000163c0: 732e 2229 0a0a 2020 2020 2020 2020 7265  s.")..        re
+000163d0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+000163e0: 6170 692e 6372 6561 7465 5f70 7265 7365  api.create_prese
+000163f0: 745f 7074 7a5f 6361 6d65 7261 2873 656c  t_ptz_camera(sel
+00016400: 662e 6964 2c20 6e61 6d65 3d6e 616d 6529  f.id, name=name)
+00016410: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00016420: 6765 745f 7074 7a5f 7072 6573 6574 7328  get_ptz_presets(
+00016430: 7365 6c66 2920 2d3e 206c 6973 745b 5054  self) -> list[PT
+00016440: 5a50 7265 7365 745d 3a0a 2020 2020 2020  ZPreset]:.      
+00016450: 2020 2222 2247 6574 2050 545a 2050 7265    """Get PTZ Pre
+00016460: 7365 7473 2066 6f72 2063 616d 6572 612e  sets for camera.
+00016470: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00016480: 6e6f 7420 7365 6c66 2e66 6561 7475 7265  not self.feature
+00016490: 5f66 6c61 6773 2e69 735f 7074 7a3a 0a20  _flags.is_ptz:. 
+000164a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000164b0: 2042 6164 5265 7175 6573 7428 2243 616d   BadRequest("Cam
+000164c0: 6572 6120 646f 6573 206e 6f74 2073 7570  era does not sup
+000164d0: 706f 7274 2050 545a 2066 6561 7475 7265  port PTZ feature
+000164e0: 732e 2229 0a0a 2020 2020 2020 2020 7265  s.")..        re
+000164f0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00016500: 6170 692e 6765 745f 7072 6573 6574 735f  api.get_presets_
+00016510: 7074 7a5f 6361 6d65 7261 2873 656c 662e  ptz_camera(self.
+00016520: 6964 290a 0a20 2020 2061 7379 6e63 2064  id)..    async d
+00016530: 6566 2064 656c 6574 655f 7074 7a5f 7072  ef delete_ptz_pr
+00016540: 6573 6574 2873 656c 662c 202a 2c20 736c  eset(self, *, sl
+00016550: 6f74 3a20 696e 7429 202d 3e20 4e6f 6e65  ot: int) -> None
+00016560: 3a0a 2020 2020 2020 2020 2222 2244 656c  :.        """Del
+00016570: 6574 6520 5054 5a20 7072 6573 6574 2066  ete PTZ preset f
+00016580: 6f72 2063 616d 6572 612e 2222 220a 0a20  or camera.""".. 
+00016590: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+000165a0: 6c66 2e66 6561 7475 7265 5f66 6c61 6773  lf.feature_flags
+000165b0: 2e69 735f 7074 7a3a 0a20 2020 2020 2020  .is_ptz:.       
+000165c0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+000165d0: 7175 6573 7428 2243 616d 6572 6120 646f  quest("Camera do
+000165e0: 6573 206e 6f74 2073 7570 706f 7274 2050  es not support P
+000165f0: 545a 2066 6561 7475 7265 732e 2229 0a0a  TZ features.")..
+00016600: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+00016610: 6c66 2e61 7069 2e64 656c 6574 655f 7072  lf.api.delete_pr
+00016620: 6573 6574 5f70 747a 5f63 616d 6572 6128  eset_ptz_camera(
+00016630: 7365 6c66 2e69 642c 2073 6c6f 743d 736c  self.id, slot=sl
+00016640: 6f74 290a 0a20 2020 2061 7379 6e63 2064  ot)..    async d
+00016650: 6566 2067 6574 5f70 747a 5f68 6f6d 6528  ef get_ptz_home(
+00016660: 7365 6c66 2920 2d3e 2050 545a 5072 6573  self) -> PTZPres
+00016670: 6574 3a0a 2020 2020 2020 2020 2222 2247  et:.        """G
+00016680: 6574 2050 545a 2068 6f6d 6520 7072 6573  et PTZ home pres
+00016690: 6574 2028 2d31 292e 2222 220a 0a20 2020  et (-1)."""..   
+000166a0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000166b0: 2e66 6561 7475 7265 5f66 6c61 6773 2e69  .feature_flags.i
+000166c0: 735f 7074 7a3a 0a20 2020 2020 2020 2020  s_ptz:.         
+000166d0: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+000166e0: 6573 7428 2243 616d 6572 6120 646f 6573  est("Camera does
+000166f0: 206e 6f74 2073 7570 706f 7274 2050 545a   not support PTZ
+00016700: 2066 6561 7475 7265 732e 2229 0a0a 2020   features.")..  
+00016710: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00016720: 6974 2073 656c 662e 6170 692e 6765 745f  it self.api.get_
+00016730: 686f 6d65 5f70 747a 5f63 616d 6572 6128  home_ptz_camera(
+00016740: 7365 6c66 2e69 6429 0a0a 2020 2020 6173  self.id)..    as
+00016750: 796e 6320 6465 6620 7365 745f 7074 7a5f  ync def set_ptz_
+00016760: 686f 6d65 2873 656c 6629 202d 3e20 5054  home(self) -> PT
+00016770: 5a50 7265 7365 743a 0a20 2020 2020 2020  ZPreset:.       
+00016780: 2022 2222 4765 7420 5054 5a20 686f 6d65   """Get PTZ home
+00016790: 2070 7265 7365 7420 282d 3129 2074 6f20   preset (-1) to 
+000167a0: 6375 7272 656e 7420 706f 7369 7469 6f6e  current position
+000167b0: 2e22 2222 0a0a 2020 2020 2020 2020 6966  ."""..        if
+000167c0: 206e 6f74 2073 656c 662e 6665 6174 7572   not self.featur
+000167d0: 655f 666c 6167 732e 6973 5f70 747a 3a0a  e_flags.is_ptz:.
+000167e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000167f0: 6520 4261 6452 6571 7565 7374 2822 4361  e BadRequest("Ca
+00016800: 6d65 7261 2064 6f65 7320 6e6f 7420 7375  mera does not su
+00016810: 7070 6f72 7420 5054 5a20 6665 6174 7572  pport PTZ featur
+00016820: 6573 2e22 290a 0a20 2020 2020 2020 2072  es.")..        r
+00016830: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00016840: 2e61 7069 2e73 6574 5f68 6f6d 655f 7074  .api.set_home_pt
+00016850: 7a5f 6361 6d65 7261 2873 656c 662e 6964  z_camera(self.id
+00016860: 290a 0a20 2020 2023 2065 6e64 7265 6769  )..    # endregi
+00016870: 6f6e 0a0a 0a63 6c61 7373 2056 6965 7765  on...class Viewe
+00016880: 7228 5072 6f74 6563 7441 646f 7074 6162  r(ProtectAdoptab
+00016890: 6c65 4465 7669 6365 4d6f 6465 6c29 3a0a  leDeviceModel):.
+000168a0: 2020 2020 7374 7265 616d 5f6c 696d 6974      stream_limit
+000168b0: 3a20 696e 740a 2020 2020 736f 6674 7761  : int.    softwa
+000168c0: 7265 5f76 6572 7369 6f6e 3a20 7374 720a  re_version: str.
+000168d0: 2020 2020 6c69 7665 7669 6577 5f69 643a      liveview_id:
+000168e0: 2073 7472 0a0a 2020 2020 4063 6c61 7373   str..    @class
+000168f0: 6d65 7468 6f64 0a20 2020 2040 6361 6368  method.    @cach
+00016900: 650a 2020 2020 6465 6620 5f67 6574 5f75  e.    def _get_u
+00016910: 6e69 6669 5f72 656d 6170 7328 636c 7329  nifi_remaps(cls)
+00016920: 202d 3e20 6469 6374 5b73 7472 2c20 7374   -> dict[str, st
+00016930: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
+00016940: 726e 207b 2a2a 7375 7065 7228 292e 5f67  rn {**super()._g
+00016950: 6574 5f75 6e69 6669 5f72 656d 6170 7328  et_unifi_remaps(
+00016960: 292c 2022 6c69 7665 7669 6577 223a 2022  ), "liveview": "
+00016970: 6c69 7665 7669 6577 4964 227d 0a0a 2020  liveviewId"}..  
+00016980: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00016990: 2020 2040 6361 6368 650a 2020 2020 6465     @cache.    de
+000169a0: 6620 5f67 6574 5f72 6561 645f 6f6e 6c79  f _get_read_only
+000169b0: 5f66 6965 6c64 7328 636c 7329 202d 3e20  _fields(cls) -> 
+000169c0: 7365 745b 7374 725d 3a0a 2020 2020 2020  set[str]:.      
+000169d0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+000169e0: 2e5f 6765 745f 7265 6164 5f6f 6e6c 795f  ._get_read_only_
+000169f0: 6669 656c 6473 2829 207c 207b 2273 6f66  fields() | {"sof
+00016a00: 7477 6172 6556 6572 7369 6f6e 227d 0a0a  twareVersion"}..
+00016a10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00016a20: 2020 6465 6620 6c69 7665 7669 6577 2873    def liveview(s
+00016a30: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+00016a40: 5b4c 6976 6576 6965 775d 3a0a 2020 2020  [Liveview]:.    
+00016a50: 2020 2020 2320 7573 6572 206d 6179 206e      # user may n
+00016a60: 6f74 2068 6176 6520 7065 726d 6973 7369  ot have permissi
+00016a70: 6f6e 2074 6f20 7365 6520 7468 6520 6c69  on to see the li
+00016a80: 7665 7669 6577 0a20 2020 2020 2020 2072  veview.        r
+00016a90: 6574 7572 6e20 7365 6c66 2e61 7069 2e62  eturn self.api.b
+00016aa0: 6f6f 7473 7472 6170 2e6c 6976 6576 6965  ootstrap.livevie
+00016ab0: 7773 2e67 6574 2873 656c 662e 6c69 7665  ws.get(self.live
+00016ac0: 7669 6577 5f69 6429 0a0a 2020 2020 6173  view_id)..    as
+00016ad0: 796e 6320 6465 6620 7365 745f 6c69 7665  ync def set_live
+00016ae0: 7669 6577 2873 656c 662c 206c 6976 6576  view(self, livev
+00016af0: 6965 773a 204c 6976 6576 6965 7729 202d  iew: Liveview) -
+00016b00: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00016b10: 2222 2253 6574 7320 7468 6520 6c69 7665  """Sets the live
+00016b20: 7669 6577 2063 7572 7265 6e74 2073 6574  view current set
+00016b30: 2066 6f72 2074 6865 2076 6965 7765 720a   for the viewer.
+00016b40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00016b50: 2020 2020 2020 202d 2d2d 2d0a 2020 2020         ----.    
+00016b60: 2020 2020 2020 2020 6c69 7665 7669 6577          liveview
+00016b70: 3a20 5468 6520 6c69 7665 7669 6577 2079  : The liveview y
+00016b80: 6f75 2077 616e 7420 746f 2073 6574 0a20  ou want to set. 
+00016b90: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00016ba0: 2020 2020 6966 2073 656c 662e 5f61 7069      if self._api
+00016bb0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00016bc0: 206c 6976 6576 6965 772e 6964 206e 6f74   liveview.id not
+00016bd0: 2069 6e20 7365 6c66 2e5f 6170 692e 626f   in self._api.bo
+00016be0: 6f74 7374 7261 702e 6c69 7665 7669 6577  otstrap.liveview
+00016bf0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00016c00: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+00016c10: 2255 6e6b 6e6f 776e 206c 6976 6576 6965  "Unknown livevie
+00016c20: 7722 290a 0a20 2020 2020 2020 2061 7379  w")..        asy
+00016c30: 6e63 2077 6974 6820 7365 6c66 2e5f 7570  nc with self._up
+00016c40: 6461 7465 5f6c 6f63 6b3a 0a20 2020 2020  date_lock:.     
+00016c50: 2020 2020 2020 2061 7761 6974 2061 7379         await asy
+00016c60: 6e63 696f 2e73 6c65 6570 280a 2020 2020  ncio.sleep(.    
+00016c70: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
+00016c80: 2020 2020 2020 2020 2020 2029 2020 2320             )  # 
+00016c90: 7969 656c 6420 746f 2074 6865 2065 7665  yield to the eve
+00016ca0: 6e74 206c 6f6f 7020 6f6e 6365 2077 6520  nt loop once we 
+00016cb0: 6861 7665 2074 6865 206c 6f63 6b20 746f  have the lock to
+00016cc0: 2070 726f 6365 7373 2061 6e79 2070 656e   process any pen
+00016cd0: 6469 6e67 2075 7064 6174 6573 0a20 2020  ding updates.   
+00016ce0: 2020 2020 2020 2020 2064 6174 615f 6265           data_be
+00016cf0: 666f 7265 5f63 6861 6e67 6573 203d 2073  fore_changes = s
+00016d00: 656c 662e 6469 6374 5f77 6974 685f 6578  elf.dict_with_ex
+00016d10: 636c 7564 6573 2829 0a20 2020 2020 2020  cludes().       
+00016d20: 2020 2020 2073 656c 662e 6c69 7665 7669       self.livevi
+00016d30: 6577 5f69 6420 3d20 6c69 7665 7669 6577  ew_id = liveview
+00016d40: 2e69 640a 2020 2020 2020 2020 2020 2020  .id.            
+00016d50: 2320 556e 6946 6920 5072 6f74 6563 7420  # UniFi Protect 
+00016d60: 6275 673a 2063 6861 6e67 696e 6720 7468  bug: changing th
+00016d70: 6520 6c69 7665 7669 6577 2064 6f65 7320  e liveview does 
+00016d80: 5f6e 6f74 5f20 656d 6974 2061 2057 5320  _not_ emit a WS 
+00016d90: 6d65 7373 6167 650a 2020 2020 2020 2020  message.        
+00016da0: 2020 2020 6177 6169 7420 7365 6c66 2e73      await self.s
+00016db0: 6176 655f 6465 7669 6365 2864 6174 615f  ave_device(data_
+00016dc0: 6265 666f 7265 5f63 6861 6e67 6573 2c20  before_changes, 
+00016dd0: 666f 7263 655f 656d 6974 3d54 7275 6529  force_emit=True)
+00016de0: 0a0a 0a63 6c61 7373 2042 7269 6467 6528  ...class Bridge(
+00016df0: 5072 6f74 6563 7441 646f 7074 6162 6c65  ProtectAdoptable
+00016e00: 4465 7669 6365 4d6f 6465 6c29 3a0a 2020  DeviceModel):.  
+00016e10: 2020 706c 6174 666f 726d 3a20 7374 720a    platform: str.
+00016e20: 0a0a 636c 6173 7320 5365 6e73 6f72 5365  ..class SensorSe
+00016e30: 7474 696e 6773 4261 7365 2850 726f 7465  ttingsBase(Prote
+00016e40: 6374 4261 7365 4f62 6a65 6374 293a 0a20  ctBaseObject):. 
+00016e50: 2020 2069 735f 656e 6162 6c65 643a 2062     is_enabled: b
+00016e60: 6f6f 6c0a 0a0a 636c 6173 7320 5365 6e73  ool...class Sens
+00016e70: 6f72 5468 7265 7368 6f6c 6453 6574 7469  orThresholdSetti
+00016e80: 6e67 7328 5365 6e73 6f72 5365 7474 696e  ngs(SensorSettin
+00016e90: 6773 4261 7365 293a 0a20 2020 206d 6172  gsBase):.    mar
+00016ea0: 6769 6e3a 2066 6c6f 6174 2020 2320 7265  gin: float  # re
+00016eb0: 6164 206f 6e6c 790a 2020 2020 2320 2273  ad only.    # "s
+00016ec0: 6166 6522 2074 6872 6573 686f 6c64 7320  afe" thresholds 
+00016ed0: 666f 7220 616c 6572 7469 6e67 0a20 2020  for alerting.   
+00016ee0: 2023 2061 6e79 7468 696e 6720 6265 6c6f   # anything belo
+00016ef0: 772f 6162 6f76 6520 7769 6c6c 2074 7269  w/above will tri
+00016f00: 6767 6572 2061 6c65 7274 0a20 2020 206c  gger alert.    l
+00016f10: 6f77 5f74 6872 6573 686f 6c64 3a20 4f70  ow_threshold: Op
+00016f20: 7469 6f6e 616c 5b66 6c6f 6174 5d0a 2020  tional[float].  
+00016f30: 2020 6869 6768 5f74 6872 6573 686f 6c64    high_threshold
+00016f40: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+00016f50: 5d0a 0a0a 636c 6173 7320 5365 6e73 6f72  ]...class Sensor
+00016f60: 5365 6e73 6974 6976 6974 7953 6574 7469  SensitivitySetti
+00016f70: 6e67 7328 5365 6e73 6f72 5365 7474 696e  ngs(SensorSettin
+00016f80: 6773 4261 7365 293a 0a20 2020 2073 656e  gsBase):.    sen
+00016f90: 7369 7469 7669 7479 3a20 5065 7263 656e  sitivity: Percen
+00016fa0: 7449 6e74 0a0a 0a63 6c61 7373 2053 656e  tInt...class Sen
+00016fb0: 736f 7242 6174 7465 7279 5374 6174 7573  sorBatteryStatus
+00016fc0: 2850 726f 7465 6374 4261 7365 4f62 6a65  (ProtectBaseObje
+00016fd0: 6374 293a 0a20 2020 2070 6572 6365 6e74  ct):.    percent
+00016fe0: 6167 653a 204f 7074 696f 6e61 6c5b 5065  age: Optional[Pe
+00016ff0: 7263 656e 7449 6e74 5d0a 2020 2020 6973  rcentInt].    is
+00017000: 5f6c 6f77 3a20 626f 6f6c 0a0a 0a63 6c61  _low: bool...cla
+00017010: 7373 2053 656e 736f 7253 7461 7428 5072  ss SensorStat(Pr
+00017020: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
+00017030: 3a0a 2020 2020 7661 6c75 653a 204f 7074  :.    value: Opt
+00017040: 696f 6e61 6c5b 666c 6f61 745d 0a20 2020  ional[float].   
+00017050: 2073 7461 7475 733a 2053 656e 736f 7253   status: SensorS
+00017060: 7461 7475 7354 7970 650a 0a0a 636c 6173  tatusType...clas
+00017070: 7320 5365 6e73 6f72 5374 6174 7328 5072  s SensorStats(Pr
+00017080: 6f74 6563 7442 6173 654f 626a 6563 7429  otectBaseObject)
+00017090: 3a0a 2020 2020 6c69 6768 743a 2053 656e  :.    light: Sen
+000170a0: 736f 7253 7461 740a 2020 2020 6875 6d69  sorStat.    humi
+000170b0: 6469 7479 3a20 5365 6e73 6f72 5374 6174  dity: SensorStat
+000170c0: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
+000170d0: 3a20 5365 6e73 6f72 5374 6174 0a0a 0a63  : SensorStat...c
+000170e0: 6c61 7373 2053 656e 736f 7228 5072 6f74  lass Sensor(Prot
+000170f0: 6563 7441 646f 7074 6162 6c65 4465 7669  ectAdoptableDevi
+00017100: 6365 4d6f 6465 6c29 3a0a 2020 2020 616c  ceModel):.    al
+00017110: 6172 6d5f 7365 7474 696e 6773 3a20 5365  arm_settings: Se
+00017120: 6e73 6f72 5365 7474 696e 6773 4261 7365  nsorSettingsBase
+00017130: 0a20 2020 2061 6c61 726d 5f74 7269 6767  .    alarm_trigg
+00017140: 6572 6564 5f61 743a 204f 7074 696f 6e61  ered_at: Optiona
+00017150: 6c5b 6461 7465 7469 6d65 5d0a 2020 2020  l[datetime].    
+00017160: 6261 7474 6572 795f 7374 6174 7573 3a20  battery_status: 
+00017170: 5365 6e73 6f72 4261 7474 6572 7953 7461  SensorBatterySta
+00017180: 7475 730a 2020 2020 6361 6d65 7261 5f69  tus.    camera_i
+00017190: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+000171a0: 0a20 2020 2068 756d 6964 6974 795f 7365  .    humidity_se
+000171b0: 7474 696e 6773 3a20 5365 6e73 6f72 5468  ttings: SensorTh
+000171c0: 7265 7368 6f6c 6453 6574 7469 6e67 730a  resholdSettings.
+000171d0: 2020 2020 6973 5f6d 6f74 696f 6e5f 6465      is_motion_de
+000171e0: 7465 6374 6564 3a20 626f 6f6c 0a20 2020  tected: bool.   
+000171f0: 2069 735f 6f70 656e 6564 3a20 626f 6f6c   is_opened: bool
+00017200: 0a20 2020 206c 6561 6b5f 6465 7465 6374  .    leak_detect
+00017210: 6564 5f61 743a 204f 7074 696f 6e61 6c5b  ed_at: Optional[
+00017220: 6461 7465 7469 6d65 5d0a 2020 2020 6c65  datetime].    le
+00017230: 645f 7365 7474 696e 6773 3a20 5365 6e73  d_settings: Sens
+00017240: 6f72 5365 7474 696e 6773 4261 7365 0a20  orSettingsBase. 
+00017250: 2020 206c 6967 6874 5f73 6574 7469 6e67     light_setting
+00017260: 733a 2053 656e 736f 7254 6872 6573 686f  s: SensorThresho
+00017270: 6c64 5365 7474 696e 6773 0a20 2020 206d  ldSettings.    m
+00017280: 6f74 696f 6e5f 6465 7465 6374 6564 5f61  otion_detected_a
+00017290: 743a 204f 7074 696f 6e61 6c5b 6461 7465  t: Optional[date
+000172a0: 7469 6d65 5d0a 2020 2020 6d6f 7469 6f6e  time].    motion
+000172b0: 5f73 6574 7469 6e67 733a 2053 656e 736f  _settings: Senso
+000172c0: 7253 656e 7369 7469 7669 7479 5365 7474  rSensitivitySett
+000172d0: 696e 6773 0a20 2020 206f 7065 6e5f 7374  ings.    open_st
+000172e0: 6174 7573 5f63 6861 6e67 6564 5f61 743a  atus_changed_at:
+000172f0: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
+00017300: 6d65 5d0a 2020 2020 7374 6174 733a 2053  me].    stats: S
+00017310: 656e 736f 7253 7461 7473 0a20 2020 2074  ensorStats.    t
+00017320: 616d 7065 7269 6e67 5f64 6574 6563 7465  ampering_detecte
+00017330: 645f 6174 3a20 4f70 7469 6f6e 616c 5b64  d_at: Optional[d
+00017340: 6174 6574 696d 655d 0a20 2020 2074 656d  atetime].    tem
+00017350: 7065 7261 7475 7265 5f73 6574 7469 6e67  perature_setting
+00017360: 733a 2053 656e 736f 7254 6872 6573 686f  s: SensorThresho
+00017370: 6c64 5365 7474 696e 6773 0a20 2020 206d  ldSettings.    m
+00017380: 6f75 6e74 5f74 7970 653a 204d 6f75 6e74  ount_type: Mount
+00017390: 5479 7065 0a0a 2020 2020 2320 6e6f 7420  Type..    # not 
+000173a0: 6469 7265 6374 6c79 2066 726f 6d20 556e  directly from Un
+000173b0: 6946 690a 2020 2020 6c61 7374 5f6d 6f74  iFi.    last_mot
+000173c0: 696f 6e5f 6576 656e 745f 6964 3a20 4f70  ion_event_id: Op
+000173d0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+000173e0: 6e65 0a20 2020 206c 6173 745f 636f 6e74  ne.    last_cont
+000173f0: 6163 745f 6576 656e 745f 6964 3a20 4f70  act_event_id: Op
+00017400: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00017410: 6e65 0a20 2020 206c 6173 745f 7661 6c75  ne.    last_valu
+00017420: 655f 6576 656e 745f 6964 3a20 4f70 7469  e_event_id: Opti
+00017430: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00017440: 0a20 2020 206c 6173 745f 616c 6172 6d5f  .    last_alarm_
+00017450: 6576 656e 745f 6964 3a20 4f70 7469 6f6e  event_id: Option
+00017460: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
+00017470: 2020 2065 7874 7265 6d65 5f76 616c 7565     extreme_value
+00017480: 5f64 6574 6563 7465 645f 6174 3a20 4f70  _detected_at: Op
+00017490: 7469 6f6e 616c 5b64 6174 6574 696d 655d  tional[datetime]
+000174a0: 203d 204e 6f6e 650a 2020 2020 5f74 616d   = None.    _tam
+000174b0: 7065 725f 7469 6d65 6f75 743a 204f 7074  per_timeout: Opt
+000174c0: 696f 6e61 6c5b 6461 7465 7469 6d65 5d20  ional[datetime] 
+000174d0: 3d20 5072 6976 6174 6541 7474 7228 4e6f  = PrivateAttr(No
+000174e0: 6e65 290a 2020 2020 5f61 6c61 726d 5f74  ne).    _alarm_t
+000174f0: 696d 656f 7574 3a20 4f70 7469 6f6e 616c  imeout: Optional
+00017500: 5b64 6174 6574 696d 655d 203d 2050 7269  [datetime] = Pri
+00017510: 7661 7465 4174 7472 284e 6f6e 6529 0a0a  vateAttr(None)..
+00017520: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00017530: 0a20 2020 2040 6361 6368 650a 2020 2020  .    @cache.    
+00017540: 6465 6620 5f67 6574 5f75 6e69 6669 5f72  def _get_unifi_r
+00017550: 656d 6170 7328 636c 7329 202d 3e20 6469  emaps(cls) -> di
+00017560: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
+00017570: 2020 2020 2020 7265 7475 726e 207b 2a2a        return {**
+00017580: 7375 7065 7228 292e 5f67 6574 5f75 6e69  super()._get_uni
+00017590: 6669 5f72 656d 6170 7328 292c 2022 6361  fi_remaps(), "ca
+000175a0: 6d65 7261 223a 2022 6361 6d65 7261 4964  mera": "cameraId
+000175b0: 227d 0a0a 2020 2020 4063 6c61 7373 6d65  "}..    @classme
+000175c0: 7468 6f64 0a20 2020 2040 6361 6368 650a  thod.    @cache.
+000175d0: 2020 2020 6465 6620 5f67 6574 5f72 6561      def _get_rea
+000175e0: 645f 6f6e 6c79 5f66 6965 6c64 7328 636c  d_only_fields(cl
+000175f0: 7329 202d 3e20 7365 745b 7374 725d 3a0a  s) -> set[str]:.
+00017600: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00017610: 7570 6572 2829 2e5f 6765 745f 7265 6164  uper()._get_read
+00017620: 5f6f 6e6c 795f 6669 656c 6473 2829 207c  _only_fields() |
+00017630: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00017640: 6261 7474 6572 7953 7461 7475 7322 2c0a  batteryStatus",.
+00017650: 2020 2020 2020 2020 2020 2020 2269 734d              "isM
+00017660: 6f74 696f 6e44 6574 6563 7465 6422 2c0a  otionDetected",.
+00017670: 2020 2020 2020 2020 2020 2020 226c 6561              "lea
+00017680: 6b44 6574 6563 7465 6441 7422 2c0a 2020  kDetectedAt",.  
+00017690: 2020 2020 2020 2020 2020 2274 616d 7065            "tampe
+000176a0: 7269 6e67 4465 7465 6374 6564 4174 222c  ringDetectedAt",
+000176b0: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+000176c0: 4f70 656e 6564 222c 0a20 2020 2020 2020  Opened",.       
+000176d0: 2020 2020 2022 6f70 656e 5374 6174 7573       "openStatus
+000176e0: 4368 616e 6765 6441 7422 2c0a 2020 2020  ChangedAt",.    
+000176f0: 2020 2020 2020 2020 2261 6c61 726d 5472          "alarmTr
+00017700: 6967 6765 7265 6441 7422 2c0a 2020 2020  iggeredAt",.    
+00017710: 2020 2020 2020 2020 226d 6f74 696f 6e44          "motionD
+00017720: 6574 6563 7465 6441 7422 2c0a 2020 2020  etectedAt",.    
+00017730: 2020 2020 2020 2020 2273 7461 7473 222c          "stats",
+00017740: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00017750: 6465 6620 756e 6966 695f 6469 6374 280a  def unifi_dict(.
+00017760: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00017770: 2020 2020 2020 6461 7461 3a20 4f70 7469        data: Opti
+00017780: 6f6e 616c 5b64 6963 745b 7374 722c 2041  onal[dict[str, A
+00017790: 6e79 5d5d 203d 204e 6f6e 652c 0a20 2020  ny]] = None,.   
+000177a0: 2020 2020 2065 7863 6c75 6465 3a20 4f70       exclude: Op
+000177b0: 7469 6f6e 616c 5b73 6574 5b73 7472 5d5d  tional[set[str]]
+000177c0: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
+000177d0: 3e20 6469 6374 5b73 7472 2c20 416e 795d  > dict[str, Any]
+000177e0: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
+000177f0: 2073 7570 6572 2829 2e75 6e69 6669 5f64   super().unifi_d
+00017800: 6963 7428 6461 7461 3d64 6174 612c 2065  ict(data=data, e
+00017810: 7863 6c75 6465 3d65 7863 6c75 6465 290a  xclude=exclude).
+00017820: 0a20 2020 2020 2020 2069 6620 226c 6173  .        if "las
+00017830: 744d 6f74 696f 6e45 7665 6e74 4964 2220  tMotionEventId" 
+00017840: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
+00017850: 2020 2020 2064 656c 2064 6174 615b 226c       del data["l
+00017860: 6173 744d 6f74 696f 6e45 7665 6e74 4964  astMotionEventId
+00017870: 225d 0a20 2020 2020 2020 2069 6620 226c  "].        if "l
+00017880: 6173 7443 6f6e 7461 6374 4576 656e 7449  astContactEventI
+00017890: 6422 2069 6e20 6461 7461 3a0a 2020 2020  d" in data:.    
+000178a0: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
+000178b0: 5b22 6c61 7374 436f 6e74 6163 7445 7665  ["lastContactEve
+000178c0: 6e74 4964 225d 0a20 2020 2020 2020 2069  ntId"].        i
+000178d0: 6620 226c 6173 7456 616c 7565 4576 656e  f "lastValueEven
+000178e0: 7449 6422 2069 6e20 6461 7461 3a0a 2020  tId" in data:.  
+000178f0: 2020 2020 2020 2020 2020 6465 6c20 6461            del da
+00017900: 7461 5b22 6c61 7374 5661 6c75 6545 7665  ta["lastValueEve
+00017910: 6e74 4964 225d 0a20 2020 2020 2020 2069  ntId"].        i
+00017920: 6620 226c 6173 7441 6c61 726d 4576 656e  f "lastAlarmEven
+00017930: 7449 6422 2069 6e20 6461 7461 3a0a 2020  tId" in data:.  
+00017940: 2020 2020 2020 2020 2020 6465 6c20 6461            del da
+00017950: 7461 5b22 6c61 7374 416c 6172 6d45 7665  ta["lastAlarmEve
+00017960: 6e74 4964 225d 0a20 2020 2020 2020 2069  ntId"].        i
+00017970: 6620 2265 7874 7265 6d65 5661 6c75 6544  f "extremeValueD
+00017980: 6574 6563 7465 6441 7422 2069 6e20 6461  etectedAt" in da
+00017990: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+000179a0: 6465 6c20 6461 7461 5b22 6578 7472 656d  del data["extrem
+000179b0: 6556 616c 7565 4465 7465 6374 6564 4174  eValueDetectedAt
+000179c0: 225d 0a0a 2020 2020 2020 2020 7265 7475  "]..        retu
+000179d0: 726e 2064 6174 610a 0a20 2020 2040 7072  rn data..    @pr
+000179e0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+000179f0: 616d 6572 6128 7365 6c66 2920 2d3e 204f  amera(self) -> O
+00017a00: 7074 696f 6e61 6c5b 4361 6d65 7261 5d3a  ptional[Camera]:
+00017a10: 0a20 2020 2020 2020 2022 2222 5061 6972  .        """Pair
+00017a20: 6564 2043 616d 6572 6120 7769 6c6c 2061  ed Camera will a
+00017a30: 6c77 6179 7320 6265 206e 6f6e 6520 6966  lways be none if
+00017a40: 206e 6f20 6361 6d65 7261 2069 7320 7061   no camera is pa
+00017a50: 6972 6564 2222 220a 0a20 2020 2020 2020  ired"""..       
+00017a60: 2069 6620 7365 6c66 2e63 616d 6572 615f   if self.camera_
+00017a70: 6964 2069 7320 4e6f 6e65 3a0a 2020 2020  id is None:.    
+00017a80: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00017a90: 6f6e 650a 0a20 2020 2020 2020 2072 6574  one..        ret
+00017aa0: 7572 6e20 7365 6c66 2e61 7069 2e62 6f6f  urn self.api.boo
+00017ab0: 7473 7472 6170 2e63 616d 6572 6173 5b73  tstrap.cameras[s
+00017ac0: 656c 662e 6361 6d65 7261 5f69 645d 0a0a  elf.camera_id]..
+00017ad0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00017ae0: 2020 6465 6620 6973 5f74 616d 7065 7269    def is_tamperi
+00017af0: 6e67 5f64 6574 6563 7465 6428 7365 6c66  ng_detected(self
+00017b00: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00017b10: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
+00017b20: 616d 7065 7269 6e67 5f64 6574 6563 7465  ampering_detecte
+00017b30: 645f 6174 2069 7320 6e6f 7420 4e6f 6e65  d_at is not None
+00017b40: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00017b50: 2020 2020 6465 6620 6973 5f61 6c61 726d      def is_alarm
+00017b60: 5f64 6574 6563 7465 6428 7365 6c66 2920  _detected(self) 
+00017b70: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00017b80: 2069 6620 7365 6c66 2e5f 616c 6172 6d5f   if self._alarm_
+00017b90: 7469 6d65 6f75 7420 6973 204e 6f6e 653a  timeout is None:
+00017ba0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00017bb0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00017bc0: 2020 7265 7475 726e 2075 7463 5f6e 6f77    return utc_now
+00017bd0: 2829 203c 2073 656c 662e 5f61 6c61 726d  () < self._alarm
+00017be0: 5f74 696d 656f 7574 0a0a 2020 2020 4070  _timeout..    @p
+00017bf0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00017c00: 6973 5f63 6f6e 7461 6374 5f73 656e 736f  is_contact_senso
+00017c10: 725f 656e 6162 6c65 6428 7365 6c66 2920  r_enabled(self) 
+00017c20: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00017c30: 2072 6574 7572 6e20 7365 6c66 2e6d 6f75   return self.mou
+00017c40: 6e74 5f74 7970 6520 696e 207b 4d6f 756e  nt_type in {Moun
+00017c50: 7454 7970 652e 444f 4f52 2c20 4d6f 756e  tType.DOOR, Moun
+00017c60: 7454 7970 652e 5749 4e44 4f57 2c20 4d6f  tType.WINDOW, Mo
+00017c70: 756e 7454 7970 652e 4741 5241 4745 7d0a  untType.GARAGE}.
+00017c80: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00017c90: 2020 2064 6566 2069 735f 6d6f 7469 6f6e     def is_motion
+00017ca0: 5f73 656e 736f 725f 656e 6162 6c65 6428  _sensor_enabled(
+00017cb0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00017cc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017cd0: 6c66 2e6d 6f75 6e74 5f74 7970 6520 213d  lf.mount_type !=
+00017ce0: 204d 6f75 6e74 5479 7065 2e4c 4541 4b20   MountType.LEAK 
+00017cf0: 616e 6420 7365 6c66 2e6d 6f74 696f 6e5f  and self.motion_
+00017d00: 7365 7474 696e 6773 2e69 735f 656e 6162  settings.is_enab
+00017d10: 6c65 640a 0a20 2020 2040 7072 6f70 6572  led..    @proper
+00017d20: 7479 0a20 2020 2064 6566 2069 735f 616c  ty.    def is_al
+00017d30: 6172 6d5f 7365 6e73 6f72 5f65 6e61 626c  arm_sensor_enabl
+00017d40: 6564 2873 656c 6629 202d 3e20 626f 6f6c  ed(self) -> bool
+00017d50: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00017d60: 2073 656c 662e 6d6f 756e 745f 7479 7065   self.mount_type
+00017d70: 2021 3d20 4d6f 756e 7454 7970 652e 4c45   != MountType.LE
+00017d80: 414b 2061 6e64 2073 656c 662e 616c 6172  AK and self.alar
+00017d90: 6d5f 7365 7474 696e 6773 2e69 735f 656e  m_settings.is_en
+00017da0: 6162 6c65 640a 0a20 2020 2040 7072 6f70  abled..    @prop
+00017db0: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
+00017dc0: 6c69 6768 745f 7365 6e73 6f72 5f65 6e61  light_sensor_ena
+00017dd0: 626c 6564 2873 656c 6629 202d 3e20 626f  bled(self) -> bo
+00017de0: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
+00017df0: 726e 2073 656c 662e 6d6f 756e 745f 7479  rn self.mount_ty
+00017e00: 7065 2021 3d20 4d6f 756e 7454 7970 652e  pe != MountType.
+00017e10: 4c45 414b 2061 6e64 2073 656c 662e 6c69  LEAK and self.li
+00017e20: 6768 745f 7365 7474 696e 6773 2e69 735f  ght_settings.is_
+00017e30: 656e 6162 6c65 640a 0a20 2020 2040 7072  enabled..    @pr
+00017e40: 6f70 6572 7479 0a20 2020 2064 6566 2069  operty.    def i
+00017e50: 735f 7465 6d70 6572 6174 7572 655f 7365  s_temperature_se
+00017e60: 6e73 6f72 5f65 6e61 626c 6564 2873 656c  nsor_enabled(sel
+00017e70: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+00017e80: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+00017e90: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
+00017ea0: 756e 745f 7479 7065 2021 3d20 4d6f 756e  unt_type != Moun
+00017eb0: 7454 7970 652e 4c45 414b 2061 6e64 2073  tType.LEAK and s
+00017ec0: 656c 662e 7465 6d70 6572 6174 7572 655f  elf.temperature_
+00017ed0: 7365 7474 696e 6773 2e69 735f 656e 6162  settings.is_enab
+00017ee0: 6c65 640a 2020 2020 2020 2020 290a 0a20  led.        ).. 
+00017ef0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00017f00: 2064 6566 2069 735f 6875 6d69 6469 7479   def is_humidity
+00017f10: 5f73 656e 736f 725f 656e 6162 6c65 6428  _sensor_enabled(
+00017f20: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00017f30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017f40: 6c66 2e6d 6f75 6e74 5f74 7970 6520 213d  lf.mount_type !=
+00017f50: 204d 6f75 6e74 5479 7065 2e4c 4541 4b20   MountType.LEAK 
+00017f60: 616e 6420 7365 6c66 2e68 756d 6964 6974  and self.humidit
+00017f70: 795f 7365 7474 696e 6773 2e69 735f 656e  y_settings.is_en
+00017f80: 6162 6c65 640a 0a20 2020 2040 7072 6f70  abled..    @prop
+00017f90: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
+00017fa0: 6c65 616b 5f73 656e 736f 725f 656e 6162  leak_sensor_enab
+00017fb0: 6c65 6428 7365 6c66 2920 2d3e 2062 6f6f  led(self) -> boo
+00017fc0: 6c3a 0a20 2020 2020 2020 2072 6574 7572  l:.        retur
+00017fd0: 6e20 7365 6c66 2e6d 6f75 6e74 5f74 7970  n self.mount_typ
+00017fe0: 6520 6973 204d 6f75 6e74 5479 7065 2e4c  e is MountType.L
+00017ff0: 4541 4b0a 0a20 2020 2064 6566 2073 6574  EAK..    def set
+00018000: 5f61 6c61 726d 5f74 696d 656f 7574 2873  _alarm_timeout(s
+00018010: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00018020: 2020 2020 2020 7365 6c66 2e5f 616c 6172        self._alar
+00018030: 6d5f 7469 6d65 6f75 7420 3d20 7574 635f  m_timeout = utc_
+00018040: 6e6f 7728 2920 2b20 4556 454e 545f 5049  now() + EVENT_PI
+00018050: 4e47 5f49 4e54 4552 5641 4c0a 2020 2020  NG_INTERVAL.    
+00018060: 2020 2020 7365 6c66 2e5f 6576 656e 745f      self._event_
+00018070: 6361 6c6c 6261 636b 5f70 696e 6728 290a  callback_ping().
+00018080: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00018090: 2020 2064 6566 206c 6173 745f 6d6f 7469     def last_moti
+000180a0: 6f6e 5f65 7665 6e74 2873 656c 6629 202d  on_event(self) -
+000180b0: 3e20 4f70 7469 6f6e 616c 5b45 7665 6e74  > Optional[Event
+000180c0: 5d3a 0a20 2020 2020 2020 2069 6620 7365  ]:.        if se
+000180d0: 6c66 2e6c 6173 745f 6d6f 7469 6f6e 5f65  lf.last_motion_e
+000180e0: 7665 6e74 5f69 6420 6973 204e 6f6e 653a  vent_id is None:
+000180f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00018100: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00018110: 2020 7265 7475 726e 2073 656c 662e 6170    return self.ap
+00018120: 692e 626f 6f74 7374 7261 702e 6576 656e  i.bootstrap.even
+00018130: 7473 2e67 6574 2873 656c 662e 6c61 7374  ts.get(self.last
+00018140: 5f6d 6f74 696f 6e5f 6576 656e 745f 6964  _motion_event_id
+00018150: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+00018160: 0a20 2020 2064 6566 206c 6173 745f 636f  .    def last_co
+00018170: 6e74 6163 745f 6576 656e 7428 7365 6c66  ntact_event(self
+00018180: 2920 2d3e 204f 7074 696f 6e61 6c5b 4576  ) -> Optional[Ev
+00018190: 656e 745d 3a0a 2020 2020 2020 2020 6966  ent]:.        if
+000181a0: 2073 656c 662e 6c61 7374 5f63 6f6e 7461   self.last_conta
+000181b0: 6374 5f65 7665 6e74 5f69 6420 6973 204e  ct_event_id is N
+000181c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000181d0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000181e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000181f0: 662e 6170 692e 626f 6f74 7374 7261 702e  f.api.bootstrap.
+00018200: 6576 656e 7473 2e67 6574 2873 656c 662e  events.get(self.
+00018210: 6c61 7374 5f63 6f6e 7461 6374 5f65 7665  last_contact_eve
+00018220: 6e74 5f69 6429 0a0a 2020 2020 4070 726f  nt_id)..    @pro
+00018230: 7065 7274 790a 2020 2020 6465 6620 6c61  perty.    def la
+00018240: 7374 5f76 616c 7565 5f65 7665 6e74 2873  st_value_event(s
+00018250: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+00018260: 5b45 7665 6e74 5d3a 0a20 2020 2020 2020  [Event]:.       
+00018270: 2069 6620 7365 6c66 2e6c 6173 745f 7661   if self.last_va
+00018280: 6c75 655f 6576 656e 745f 6964 2069 7320  lue_event_id is 
+00018290: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000182a0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+000182b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000182c0: 6c66 2e61 7069 2e62 6f6f 7473 7472 6170  lf.api.bootstrap
+000182d0: 2e65 7665 6e74 732e 6765 7428 7365 6c66  .events.get(self
+000182e0: 2e6c 6173 745f 7661 6c75 655f 6576 656e  .last_value_even
+000182f0: 745f 6964 290a 0a20 2020 2040 7072 6f70  t_id)..    @prop
+00018300: 6572 7479 0a20 2020 2064 6566 206c 6173  erty.    def las
+00018310: 745f 616c 6172 6d5f 6576 656e 7428 7365  t_alarm_event(se
+00018320: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+00018330: 4576 656e 745d 3a0a 2020 2020 2020 2020  Event]:.        
+00018340: 6966 2073 656c 662e 6c61 7374 5f61 6c61  if self.last_ala
+00018350: 726d 5f65 7665 6e74 5f69 6420 6973 204e  rm_event_id is N
+00018360: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00018370: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00018380: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00018390: 662e 6170 692e 626f 6f74 7374 7261 702e  f.api.bootstrap.
+000183a0: 6576 656e 7473 2e67 6574 2873 656c 662e  events.get(self.
+000183b0: 6c61 7374 5f61 6c61 726d 5f65 7665 6e74  last_alarm_event
+000183c0: 5f69 6429 0a0a 2020 2020 4070 726f 7065  _id)..    @prope
+000183d0: 7274 790a 2020 2020 6465 6620 6973 5f6c  rty.    def is_l
+000183e0: 6561 6b5f 6465 7465 6374 6564 2873 656c  eak_detected(sel
+000183f0: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+00018400: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00018410: 6c65 616b 5f64 6574 6563 7465 645f 6174  leak_detected_at
+00018420: 2069 7320 6e6f 7420 4e6f 6e65 0a0a 2020   is not None..  
+00018430: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+00018440: 7374 6174 7573 5f6c 6967 6874 2873 656c  status_light(sel
+00018450: 662c 2065 6e61 626c 6564 3a20 626f 6f6c  f, enabled: bool
+00018460: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00018470: 2020 2022 2222 5365 7473 2074 6865 2073     """Sets the s
+00018480: 7461 7475 7320 696e 6469 6361 746f 7220  tatus indicator 
+00018490: 6c69 6768 7420 666f 7220 7468 6520 7365  light for the se
+000184a0: 6e73 6f72 2222 220a 0a20 2020 2020 2020  nsor"""..       
+000184b0: 2064 6566 2063 616c 6c62 6163 6b28 2920   def callback() 
+000184c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000184d0: 2020 2020 2073 656c 662e 6c65 645f 7365       self.led_se
+000184e0: 7474 696e 6773 2e69 735f 656e 6162 6c65  ttings.is_enable
+000184f0: 6420 3d20 656e 6162 6c65 640a 0a20 2020  d = enabled..   
+00018500: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00018510: 7175 6575 655f 7570 6461 7465 2863 616c  queue_update(cal
+00018520: 6c62 6163 6b29 0a0a 2020 2020 6173 796e  lback)..    asyn
+00018530: 6320 6465 6620 7365 745f 6d6f 756e 745f  c def set_mount_
+00018540: 7479 7065 2873 656c 662c 206d 6f75 6e74  type(self, mount
+00018550: 5f74 7970 653a 204d 6f75 6e74 5479 7065  _type: MountType
+00018560: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00018570: 2020 2022 2222 5365 7473 2063 7572 7265     """Sets curre
+00018580: 6e74 206d 6f75 6e74 2074 7970 6520 666f  nt mount type fo
+00018590: 7220 7365 6e73 6f72 2222 220a 0a20 2020  r sensor"""..   
+000185a0: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+000185b0: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+000185c0: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
+000185d0: 756e 745f 7479 7065 203d 206d 6f75 6e74  unt_type = mount
+000185e0: 5f74 7970 650a 0a20 2020 2020 2020 2061  _type..        a
+000185f0: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00018600: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00018610: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00018620: 7365 745f 6d6f 7469 6f6e 5f73 7461 7475  set_motion_statu
+00018630: 7328 7365 6c66 2c20 656e 6162 6c65 643a  s(self, enabled:
+00018640: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+00018650: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00018660: 7468 6520 6d6f 7469 6f6e 2064 6574 6563  the motion detec
+00018670: 7469 6f6e 2074 7970 6520 666f 7220 7468  tion type for th
+00018680: 6520 7365 6e73 6f72 2222 220a 0a20 2020  e sensor"""..   
+00018690: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+000186a0: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+000186b0: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
+000186c0: 7469 6f6e 5f73 6574 7469 6e67 732e 6973  tion_settings.is
+000186d0: 5f65 6e61 626c 6564 203d 2065 6e61 626c  _enabled = enabl
+000186e0: 6564 0a0a 2020 2020 2020 2020 6177 6169  ed..        awai
+000186f0: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
+00018700: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
+00018710: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+00018720: 5f6d 6f74 696f 6e5f 7365 6e73 6974 6976  _motion_sensitiv
+00018730: 6974 7928 7365 6c66 2c20 7365 6e73 6974  ity(self, sensit
+00018740: 6976 6974 793a 2069 6e74 2920 2d3e 204e  ivity: int) -> N
+00018750: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00018760: 5365 7473 2074 6865 206d 6f74 696f 6e20  Sets the motion 
+00018770: 7365 6e73 6974 6976 6974 7920 666f 7220  sensitivity for 
+00018780: 7468 6520 7365 6e73 6f72 2222 220a 0a20  the sensor""".. 
+00018790: 2020 2020 2020 2064 6566 2063 616c 6c62         def callb
+000187a0: 6163 6b28 2920 2d3e 204e 6f6e 653a 0a20  ack() -> None:. 
+000187b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000187c0: 6d6f 7469 6f6e 5f73 6574 7469 6e67 732e  motion_settings.
+000187d0: 7365 6e73 6974 6976 6974 7920 3d20 5065  sensitivity = Pe
+000187e0: 7263 656e 7449 6e74 2873 656e 7369 7469  rcentInt(sensiti
+000187f0: 7669 7479 290a 0a20 2020 2020 2020 2061  vity)..        a
+00018800: 7761 6974 2073 656c 662e 7175 6575 655f  wait self.queue_
+00018810: 7570 6461 7465 2863 616c 6c62 6163 6b29  update(callback)
+00018820: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00018830: 7365 745f 7465 6d70 6572 6174 7572 655f  set_temperature_
+00018840: 7374 6174 7573 2873 656c 662c 2065 6e61  status(self, ena
+00018850: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+00018860: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00018870: 5365 7473 2074 6865 2074 656d 7065 7261  Sets the tempera
+00018880: 7475 7265 2064 6574 6563 7469 6f6e 2074  ture detection t
+00018890: 7970 6520 666f 7220 7468 6520 7365 6e73  ype for the sens
+000188a0: 6f72 2222 220a 0a20 2020 2020 2020 2064  or"""..        d
+000188b0: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
+000188c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000188d0: 2020 2073 656c 662e 7465 6d70 6572 6174     self.temperat
+000188e0: 7572 655f 7365 7474 696e 6773 2e69 735f  ure_settings.is_
+000188f0: 656e 6162 6c65 6420 3d20 656e 6162 6c65  enabled = enable
+00018900: 640a 0a20 2020 2020 2020 2061 7761 6974  d..        await
+00018910: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+00018920: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+00018930: 2020 6173 796e 6320 6465 6620 7365 745f    async def set_
+00018940: 7465 6d70 6572 6174 7572 655f 7361 6665  temperature_safe
+00018950: 5f72 616e 6765 2873 656c 662c 206c 6f77  _range(self, low
+00018960: 3a20 666c 6f61 742c 2068 6967 683a 2066  : float, high: f
+00018970: 6c6f 6174 2920 2d3e 204e 6f6e 653a 0a20  loat) -> None:. 
+00018980: 2020 2020 2020 2022 2222 5365 7473 2074         """Sets t
+00018990: 6865 2074 656d 7065 7261 7475 7265 2073  he temperature s
+000189a0: 6166 6520 7261 6e67 6520 666f 7220 7468  afe range for th
+000189b0: 6520 7365 6e73 6f72 2222 220a 0a20 2020  e sensor"""..   
+000189c0: 2020 2020 2069 6620 6c6f 7720 3c20 302e       if low < 0.
+000189d0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+000189e0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+000189f0: 224d 696e 696d 756d 2076 616c 7565 2069  "Minimum value i
+00018a00: 7320 30c2 b043 2229 0a20 2020 2020 2020  s 0..C").       
+00018a10: 2069 6620 6869 6768 203e 2034 352e 303a   if high > 45.0:
+00018a20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00018a30: 7365 2042 6164 5265 7175 6573 7428 224d  se BadRequest("M
+00018a40: 6178 696d 756d 2076 616c 7565 2069 7320  aximum value is 
+00018a50: 3435 c2b0 4322 290a 2020 2020 2020 2020  45..C").        
+00018a60: 6966 2068 6967 6820 3c3d 206c 6f77 3a0a  if high <= low:.
+00018a70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00018a80: 6520 4261 6452 6571 7565 7374 2822 4869  e BadRequest("Hi
+00018a90: 6768 2076 616c 7565 206d 7573 7420 6265  gh value must be
+00018aa0: 2061 626f 7665 206c 6f77 2076 616c 7565   above low value
+00018ab0: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
+00018ac0: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
+00018ad0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018ae0: 7365 6c66 2e74 656d 7065 7261 7475 7265  self.temperature
+00018af0: 5f73 6574 7469 6e67 732e 6c6f 775f 7468  _settings.low_th
+00018b00: 7265 7368 6f6c 6420 3d20 6c6f 770a 2020  reshold = low.  
+00018b10: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00018b20: 656d 7065 7261 7475 7265 5f73 6574 7469  emperature_setti
+00018b30: 6e67 732e 6869 6768 5f74 6872 6573 686f  ngs.high_thresho
+00018b40: 6c64 203d 2068 6967 680a 0a20 2020 2020  ld = high..     
+00018b50: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
+00018b60: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
+00018b70: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
+00018b80: 6465 6620 7265 6d6f 7665 5f74 656d 7065  def remove_tempe
+00018b90: 7261 7475 7265 5f73 6166 655f 7261 6e67  rature_safe_rang
+00018ba0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00018bb0: 0a20 2020 2020 2020 2022 2222 5265 6d6f  .        """Remo
+00018bc0: 7665 7320 7468 6520 7465 6d70 6572 6174  ves the temperat
+00018bd0: 7572 6520 7361 6665 2072 616e 6765 2066  ure safe range f
+00018be0: 6f72 2074 6865 2073 656e 736f 7222 2222  or the sensor"""
+00018bf0: 0a0a 2020 2020 2020 2020 6465 6620 6361  ..        def ca
+00018c00: 6c6c 6261 636b 2829 202d 3e20 4e6f 6e65  llback() -> None
+00018c10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018c20: 6c66 2e74 656d 7065 7261 7475 7265 5f73  lf.temperature_s
+00018c30: 6574 7469 6e67 732e 6c6f 775f 7468 7265  ettings.low_thre
+00018c40: 7368 6f6c 6420 3d20 4e6f 6e65 0a20 2020  shold = None.   
+00018c50: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00018c60: 6d70 6572 6174 7572 655f 7365 7474 696e  mperature_settin
+00018c70: 6773 2e68 6967 685f 7468 7265 7368 6f6c  gs.high_threshol
+00018c80: 6420 3d20 4e6f 6e65 0a0a 2020 2020 2020  d = None..      
+00018c90: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
+00018ca0: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
+00018cb0: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
+00018cc0: 6566 2073 6574 5f68 756d 6964 6974 795f  ef set_humidity_
+00018cd0: 7374 6174 7573 2873 656c 662c 2065 6e61  status(self, ena
+00018ce0: 626c 6564 3a20 626f 6f6c 2920 2d3e 204e  bled: bool) -> N
+00018cf0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00018d00: 5365 7473 2074 6865 2068 756d 6964 6974  Sets the humidit
+00018d10: 7920 6465 7465 6374 696f 6e20 7479 7065  y detection type
+00018d20: 2066 6f72 2074 6865 2073 656e 736f 7222   for the sensor"
+00018d30: 2222 0a0a 2020 2020 2020 2020 6465 6620  ""..        def 
+00018d40: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
+00018d50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018d60: 7365 6c66 2e68 756d 6964 6974 795f 7365  self.humidity_se
+00018d70: 7474 696e 6773 2e69 735f 656e 6162 6c65  ttings.is_enable
+00018d80: 6420 3d20 656e 6162 6c65 640a 0a20 2020  d = enabled..   
+00018d90: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00018da0: 7175 6575 655f 7570 6461 7465 2863 616c  queue_update(cal
+00018db0: 6c62 6163 6b29 0a0a 2020 2020 6173 796e  lback)..    asyn
+00018dc0: 6320 6465 6620 7365 745f 6875 6d69 6469  c def set_humidi
+00018dd0: 7479 5f73 6166 655f 7261 6e67 6528 7365  ty_safe_range(se
+00018de0: 6c66 2c20 6c6f 773a 2066 6c6f 6174 2c20  lf, low: float, 
+00018df0: 6869 6768 3a20 666c 6f61 7429 202d 3e20  high: float) -> 
+00018e00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00018e10: 2253 6574 7320 7468 6520 6875 6d69 6469  "Sets the humidi
+00018e20: 7479 2073 6166 6520 7261 6e67 6520 666f  ty safe range fo
+00018e30: 7220 7468 6520 7365 6e73 6f72 2222 220a  r the sensor""".
+00018e40: 0a20 2020 2020 2020 2069 6620 6c6f 7720  .        if low 
+00018e50: 3c20 312e 303a 0a20 2020 2020 2020 2020  < 1.0:.         
+00018e60: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+00018e70: 6573 7428 224d 696e 696d 756d 2076 616c  est("Minimum val
+00018e80: 7565 2069 7320 3125 2229 0a20 2020 2020  ue is 1%").     
+00018e90: 2020 2069 6620 6869 6768 203e 2039 392e     if high > 99.
+00018ea0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00018eb0: 6169 7365 2042 6164 5265 7175 6573 7428  aise BadRequest(
+00018ec0: 224d 6178 696d 756d 2076 616c 7565 2069  "Maximum value i
+00018ed0: 7320 3939 2522 290a 2020 2020 2020 2020  s 99%").        
+00018ee0: 6966 2068 6967 6820 3c3d 206c 6f77 3a0a  if high <= low:.
+00018ef0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00018f00: 6520 4261 6452 6571 7565 7374 2822 4869  e BadRequest("Hi
+00018f10: 6768 2076 616c 7565 206d 7573 7420 6265  gh value must be
+00018f20: 2061 626f 7665 206c 6f77 2076 616c 7565   above low value
+00018f30: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
+00018f40: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
+00018f50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018f60: 7365 6c66 2e68 756d 6964 6974 795f 7365  self.humidity_se
+00018f70: 7474 696e 6773 2e6c 6f77 5f74 6872 6573  ttings.low_thres
+00018f80: 686f 6c64 203d 206c 6f77 0a20 2020 2020  hold = low.     
+00018f90: 2020 2020 2020 2073 656c 662e 6875 6d69         self.humi
+00018fa0: 6469 7479 5f73 6574 7469 6e67 732e 6869  dity_settings.hi
+00018fb0: 6768 5f74 6872 6573 686f 6c64 203d 2068  gh_threshold = h
+00018fc0: 6967 680a 0a20 2020 2020 2020 2061 7761  igh..        awa
+00018fd0: 6974 2073 656c 662e 7175 6575 655f 7570  it self.queue_up
+00018fe0: 6461 7465 2863 616c 6c62 6163 6b29 0a0a  date(callback)..
+00018ff0: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
+00019000: 6d6f 7665 5f68 756d 6964 6974 795f 7361  move_humidity_sa
+00019010: 6665 5f72 616e 6765 2873 656c 6629 202d  fe_range(self) -
+00019020: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00019030: 2222 2252 656d 6f76 6573 2074 6865 2068  """Removes the h
+00019040: 756d 6964 6974 7920 7361 6665 2072 616e  umidity safe ran
+00019050: 6765 2066 6f72 2074 6865 2073 656e 736f  ge for the senso
+00019060: 7222 2222 0a0a 2020 2020 2020 2020 6465  r"""..        de
+00019070: 6620 6361 6c6c 6261 636b 2829 202d 3e20  f callback() -> 
+00019080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00019090: 2020 7365 6c66 2e68 756d 6964 6974 795f    self.humidity_
+000190a0: 7365 7474 696e 6773 2e6c 6f77 5f74 6872  settings.low_thr
+000190b0: 6573 686f 6c64 203d 204e 6f6e 650a 2020  eshold = None.  
+000190c0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000190d0: 756d 6964 6974 795f 7365 7474 696e 6773  umidity_settings
+000190e0: 2e68 6967 685f 7468 7265 7368 6f6c 6420  .high_threshold 
+000190f0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+00019100: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+00019110: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+00019120: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00019130: 2073 6574 5f6c 6967 6874 5f73 7461 7475   set_light_statu
+00019140: 7328 7365 6c66 2c20 656e 6162 6c65 643a  s(self, enabled:
+00019150: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+00019160: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00019170: 7468 6520 6c69 6768 7420 6465 7465 6374  the light detect
+00019180: 696f 6e20 7479 7065 2066 6f72 2074 6865  ion type for the
+00019190: 2073 656e 736f 7222 2222 0a0a 2020 2020   sensor"""..    
+000191a0: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
+000191b0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
+000191c0: 2020 2020 2020 2020 7365 6c66 2e6c 6967          self.lig
+000191d0: 6874 5f73 6574 7469 6e67 732e 6973 5f65  ht_settings.is_e
+000191e0: 6e61 626c 6564 203d 2065 6e61 626c 6564  nabled = enabled
+000191f0: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00019200: 7365 6c66 2e71 7565 7565 5f75 7064 6174  self.queue_updat
+00019210: 6528 6361 6c6c 6261 636b 290a 0a20 2020  e(callback)..   
+00019220: 2061 7379 6e63 2064 6566 2073 6574 5f6c   async def set_l
+00019230: 6967 6874 5f73 6166 655f 7261 6e67 6528  ight_safe_range(
+00019240: 7365 6c66 2c20 6c6f 773a 2066 6c6f 6174  self, low: float
+00019250: 2c20 6869 6768 3a20 666c 6f61 7429 202d  , high: float) -
+00019260: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00019270: 2222 2253 6574 7320 7468 6520 6c69 6768  """Sets the ligh
+00019280: 7420 7361 6665 2072 616e 6765 2066 6f72  t safe range for
+00019290: 2074 6865 2073 656e 736f 7222 2222 0a0a   the sensor"""..
+000192a0: 2020 2020 2020 2020 6966 206c 6f77 203c          if low <
+000192b0: 2031 2e30 3a0a 2020 2020 2020 2020 2020   1.0:.          
+000192c0: 2020 7261 6973 6520 4261 6452 6571 7565    raise BadReque
+000192d0: 7374 2822 4d69 6e69 6d75 6d20 7661 6c75  st("Minimum valu
+000192e0: 6520 6973 2031 206c 7578 2229 0a20 2020  e is 1 lux").   
+000192f0: 2020 2020 2069 6620 6869 6768 203e 2031       if high > 1
+00019300: 3030 302e 303a 0a20 2020 2020 2020 2020  000.0:.         
+00019310: 2020 2072 6169 7365 2042 6164 5265 7175     raise BadRequ
+00019320: 6573 7428 224d 6178 696d 756d 2076 616c  est("Maximum val
+00019330: 7565 2069 7320 3130 3030 206c 7578 2229  ue is 1000 lux")
+00019340: 0a20 2020 2020 2020 2069 6620 6869 6768  .        if high
+00019350: 203c 3d20 6c6f 773a 0a20 2020 2020 2020   <= low:.       
+00019360: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+00019370: 7175 6573 7428 2248 6967 6820 7661 6c75  quest("High valu
+00019380: 6520 6d75 7374 2062 6520 6162 6f76 6520  e must be above 
+00019390: 6c6f 7720 7661 6c75 6522 290a 0a20 2020  low value")..   
+000193a0: 2020 2020 2064 6566 2063 616c 6c62 6163       def callbac
+000193b0: 6b28 2920 2d3e 204e 6f6e 653a 0a20 2020  k() -> None:.   
+000193c0: 2020 2020 2020 2020 2073 656c 662e 6c69           self.li
+000193d0: 6768 745f 7365 7474 696e 6773 2e6c 6f77  ght_settings.low
+000193e0: 5f74 6872 6573 686f 6c64 203d 206c 6f77  _threshold = low
+000193f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019400: 662e 6c69 6768 745f 7365 7474 696e 6773  f.light_settings
+00019410: 2e68 6967 685f 7468 7265 7368 6f6c 6420  .high_threshold 
+00019420: 3d20 6869 6768 0a0a 2020 2020 2020 2020  = high..        
+00019430: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+00019440: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+00019450: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00019460: 2072 656d 6f76 655f 6c69 6768 745f 7361   remove_light_sa
+00019470: 6665 5f72 616e 6765 2873 656c 6629 202d  fe_range(self) -
+00019480: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00019490: 2222 2252 656d 6f76 6573 2074 6865 206c  """Removes the l
+000194a0: 6967 6874 2073 6166 6520 7261 6e67 6520  ight safe range 
+000194b0: 666f 7220 7468 6520 7365 6e73 6f72 2222  for the sensor""
+000194c0: 220a 0a20 2020 2020 2020 2064 6566 2063  "..        def c
+000194d0: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
+000194e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000194f0: 656c 662e 6c69 6768 745f 7365 7474 696e  elf.light_settin
+00019500: 6773 2e6c 6f77 5f74 6872 6573 686f 6c64  gs.low_threshold
+00019510: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00019520: 2020 2020 7365 6c66 2e6c 6967 6874 5f73      self.light_s
+00019530: 6574 7469 6e67 732e 6869 6768 5f74 6872  ettings.high_thr
+00019540: 6573 686f 6c64 203d 204e 6f6e 650a 0a20  eshold = None.. 
+00019550: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00019560: 662e 7175 6575 655f 7570 6461 7465 2863  f.queue_update(c
+00019570: 616c 6c62 6163 6b29 0a0a 2020 2020 6173  allback)..    as
+00019580: 796e 6320 6465 6620 7365 745f 616c 6172  ync def set_alar
+00019590: 6d5f 7374 6174 7573 2873 656c 662c 2065  m_status(self, e
+000195a0: 6e61 626c 6564 3a20 626f 6f6c 2920 2d3e  nabled: bool) ->
+000195b0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000195c0: 2222 5365 7473 2074 6865 2061 6c61 726d  ""Sets the alarm
+000195d0: 2064 6574 6563 7469 6f6e 2074 7970 6520   detection type 
+000195e0: 666f 7220 7468 6520 7365 6e73 6f72 2222  for the sensor""
+000195f0: 220a 0a20 2020 2020 2020 2064 6566 2063  "..        def c
+00019600: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
+00019610: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00019620: 656c 662e 616c 6172 6d5f 7365 7474 696e  elf.alarm_settin
+00019630: 6773 2e69 735f 656e 6162 6c65 6420 3d20  gs.is_enabled = 
+00019640: 656e 6162 6c65 640a 0a20 2020 2020 2020  enabled..       
+00019650: 2061 7761 6974 2073 656c 662e 7175 6575   await self.queu
+00019660: 655f 7570 6461 7465 2863 616c 6c62 6163  e_update(callbac
+00019670: 6b29 0a0a 2020 2020 6173 796e 6320 6465  k)..    async de
+00019680: 6620 7365 745f 7061 6972 6564 5f63 616d  f set_paired_cam
+00019690: 6572 6128 7365 6c66 2c20 6361 6d65 7261  era(self, camera
+000196a0: 3a20 4f70 7469 6f6e 616c 5b43 616d 6572  : Optional[Camer
+000196b0: 615d 2920 2d3e 204e 6f6e 653a 0a20 2020  a]) -> None:.   
+000196c0: 2020 2020 2022 2222 5365 7473 2074 6865       """Sets the
+000196d0: 2063 616d 6572 6120 7061 6972 6564 2077   camera paired w
+000196e0: 6974 6820 7468 6520 7365 6e73 6f72 2222  ith the sensor""
+000196f0: 220a 0a20 2020 2020 2020 2064 6566 2063  "..        def c
+00019700: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
+00019710: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00019720: 6620 6361 6d65 7261 2069 7320 4e6f 6e65  f camera is None
+00019730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019740: 2020 7365 6c66 2e63 616d 6572 615f 6964    self.camera_id
+00019750: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00019760: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00019770: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00019780: 616d 6572 615f 6964 203d 2063 616d 6572  amera_id = camer
+00019790: 612e 6964 0a0a 2020 2020 2020 2020 6177  a.id..        aw
+000197a0: 6169 7420 7365 6c66 2e71 7565 7565 5f75  ait self.queue_u
+000197b0: 7064 6174 6528 6361 6c6c 6261 636b 290a  pdate(callback).
+000197c0: 0a20 2020 2061 7379 6e63 2064 6566 2063  .    async def c
+000197d0: 6c65 6172 5f74 616d 7065 7228 7365 6c66  lear_tamper(self
+000197e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000197f0: 2020 2022 2222 436c 6561 7273 2074 616d     """Clears tam
+00019800: 7065 7220 7374 6174 7573 2066 6f72 2073  per status for s
+00019810: 656e 736f 7222 2222 0a0a 2020 2020 2020  ensor"""..      
+00019820: 2020 6966 206e 6f74 2073 656c 662e 6170    if not self.ap
+00019830: 692e 626f 6f74 7374 7261 702e 6175 7468  i.bootstrap.auth
+00019840: 5f75 7365 722e 6361 6e28 0a20 2020 2020  _user.can(.     
+00019850: 2020 2020 2020 204d 6f64 656c 5479 7065         ModelType
+00019860: 2e53 454e 534f 522c 0a20 2020 2020 2020  .SENSOR,.       
+00019870: 2020 2020 2050 6572 6d69 7373 696f 6e4e       PermissionN
+00019880: 6f64 652e 5752 4954 452c 0a20 2020 2020  ode.WRITE,.     
+00019890: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000198a0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+000198b0: 2020 2020 7261 6973 6520 4e6f 7441 7574      raise NotAut
+000198c0: 686f 7269 7a65 6428 0a20 2020 2020 2020  horized(.       
+000198d0: 2020 2020 2020 2020 2066 2244 6f20 6e6f           f"Do no
+000198e0: 7420 6861 7665 2070 6572 6d69 7373 696f  t have permissio
+000198f0: 6e20 746f 2063 6c65 6172 2074 616d 7065  n to clear tampe
+00019900: 7220 666f 7220 7365 6e73 6f72 3a20 7b73  r for sensor: {s
+00019910: 656c 662e 6964 7d22 2c0a 2020 2020 2020  elf.id}",.      
+00019920: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00019930: 6177 6169 7420 7365 6c66 2e61 7069 2e63  await self.api.c
+00019940: 6c65 6172 5f74 616d 7065 725f 7365 6e73  lear_tamper_sens
+00019950: 6f72 2873 656c 662e 6964 290a 0a0a 636c  or(self.id)...cl
+00019960: 6173 7320 446f 6f72 6c6f 636b 2850 726f  ass Doorlock(Pro
+00019970: 7465 6374 4164 6f70 7461 626c 6544 6576  tectAdoptableDev
+00019980: 6963 654d 6f64 656c 293a 0a20 2020 2063  iceModel):.    c
+00019990: 7265 6465 6e74 6961 6c73 3a20 4f70 7469  redentials: Opti
+000199a0: 6f6e 616c 5b73 7472 5d0a 2020 2020 6c6f  onal[str].    lo
+000199b0: 636b 5f73 7461 7475 733a 204c 6f63 6b53  ck_status: LockS
+000199c0: 7461 7475 7354 7970 650a 2020 2020 656e  tatusType.    en
+000199d0: 6162 6c65 5f68 6f6d 656b 6974 3a20 626f  able_homekit: bo
+000199e0: 6f6c 0a20 2020 2061 7574 6f5f 636c 6f73  ol.    auto_clos
+000199f0: 655f 7469 6d65 3a20 7469 6d65 6465 6c74  e_time: timedelt
+00019a00: 610a 2020 2020 6c65 645f 7365 7474 696e  a.    led_settin
+00019a10: 6773 3a20 5365 6e73 6f72 5365 7474 696e  gs: SensorSettin
+00019a20: 6773 4261 7365 0a20 2020 2062 6174 7465  gsBase.    batte
+00019a30: 7279 5f73 7461 7475 733a 2053 656e 736f  ry_status: Senso
+00019a40: 7242 6174 7465 7279 5374 6174 7573 0a20  rBatteryStatus. 
+00019a50: 2020 2063 616d 6572 615f 6964 3a20 4f70     camera_id: Op
+00019a60: 7469 6f6e 616c 5b73 7472 5d0a 2020 2020  tional[str].    
+00019a70: 6861 735f 686f 6d65 6b69 743a 2062 6f6f  has_homekit: boo
+00019a80: 6c0a 2020 2020 7072 6976 6174 655f 746f  l.    private_to
+00019a90: 6b65 6e3a 2073 7472 0a0a 2020 2020 4063  ken: str..    @c
+00019aa0: 6c61 7373 6d65 7468 6f64 0a20 2020 2040  lassmethod.    @
+00019ab0: 6361 6368 650a 2020 2020 6465 6620 5f67  cache.    def _g
+00019ac0: 6574 5f75 6e69 6669 5f72 656d 6170 7328  et_unifi_remaps(
+00019ad0: 636c 7329 202d 3e20 6469 6374 5b73 7472  cls) -> dict[str
+00019ae0: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
+00019af0: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
+00019b00: 2020 2020 202a 2a73 7570 6572 2829 2e5f       **super()._
+00019b10: 6765 745f 756e 6966 695f 7265 6d61 7073  get_unifi_remaps
+00019b20: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00019b30: 2263 616d 6572 6122 3a20 2263 616d 6572  "camera": "camer
+00019b40: 6149 6422 2c0a 2020 2020 2020 2020 2020  aId",.          
+00019b50: 2020 2261 7574 6f43 6c6f 7365 5469 6d65    "autoCloseTime
+00019b60: 4d73 223a 2022 6175 746f 436c 6f73 6554  Ms": "autoCloseT
+00019b70: 696d 6522 2c0a 2020 2020 2020 2020 7d0a  ime",.        }.
+00019b80: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00019b90: 640a 2020 2020 4063 6163 6865 0a20 2020  d.    @cache.   
+00019ba0: 2064 6566 205f 6765 745f 7265 6164 5f6f   def _get_read_o
+00019bb0: 6e6c 795f 6669 656c 6473 2863 6c73 2920  nly_fields(cls) 
+00019bc0: 2d3e 2073 6574 5b73 7472 5d3a 0a20 2020  -> set[str]:.   
+00019bd0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00019be0: 7228 292e 5f67 6574 5f72 6561 645f 6f6e  r()._get_read_on
+00019bf0: 6c79 5f66 6965 6c64 7328 2920 7c20 7b0a  ly_fields() | {.
+00019c00: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
+00019c10: 6465 6e74 6961 6c73 222c 0a20 2020 2020  dentials",.     
+00019c20: 2020 2020 2020 2022 6c6f 636b 5374 6174         "lockStat
+00019c30: 7573 222c 0a20 2020 2020 2020 2020 2020  us",.           
+00019c40: 2022 6261 7474 6572 7953 7461 7475 7322   "batteryStatus"
+00019c50: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+00019c60: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00019c70: 2020 6465 6620 756e 6966 695f 6469 6374    def unifi_dict
+00019c80: 5f74 6f5f 6469 6374 2863 6c73 2c20 6461  _to_dict(cls, da
+00019c90: 7461 3a20 6469 6374 5b73 7472 2c20 416e  ta: dict[str, An
+00019ca0: 795d 2920 2d3e 2064 6963 745b 7374 722c  y]) -> dict[str,
+00019cb0: 2041 6e79 5d3a 0a20 2020 2020 2020 2069   Any]:.        i
+00019cc0: 6620 2261 7574 6f43 6c6f 7365 5469 6d65  f "autoCloseTime
+00019cd0: 4d73 2220 696e 2064 6174 6120 616e 6420  Ms" in data and 
+00019ce0: 6e6f 7420 6973 696e 7374 616e 6365 280a  not isinstance(.
+00019cf0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00019d00: 5b22 6175 746f 436c 6f73 6554 696d 654d  ["autoCloseTimeM
+00019d10: 7322 5d2c 0a20 2020 2020 2020 2020 2020  s"],.           
+00019d20: 2074 696d 6564 656c 7461 2c0a 2020 2020   timedelta,.    
+00019d30: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00019d40: 2020 2064 6174 615b 2261 7574 6f43 6c6f     data["autoClo
+00019d50: 7365 5469 6d65 4d73 225d 203d 2074 696d  seTimeMs"] = tim
+00019d60: 6564 656c 7461 286d 696c 6c69 7365 636f  edelta(milliseco
+00019d70: 6e64 733d 6461 7461 5b22 6175 746f 436c  nds=data["autoCl
+00019d80: 6f73 6554 696d 654d 7322 5d29 0a0a 2020  oseTimeMs"])..  
+00019d90: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+00019da0: 6572 2829 2e75 6e69 6669 5f64 6963 745f  er().unifi_dict_
+00019db0: 746f 5f64 6963 7428 6461 7461 290a 0a20  to_dict(data).. 
+00019dc0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00019dd0: 2064 6566 2063 616d 6572 6128 7365 6c66   def camera(self
+00019de0: 2920 2d3e 204f 7074 696f 6e61 6c5b 4361  ) -> Optional[Ca
+00019df0: 6d65 7261 5d3a 0a20 2020 2020 2020 2022  mera]:.        "
+00019e00: 2222 5061 6972 6564 2043 616d 6572 6120  ""Paired Camera 
+00019e10: 7769 6c6c 2061 6c77 6179 7320 6265 206e  will always be n
+00019e20: 6f6e 6520 6966 206e 6f20 6361 6d65 7261  one if no camera
+00019e30: 2069 7320 7061 6972 6564 2222 220a 0a20   is paired""".. 
+00019e40: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00019e50: 616d 6572 615f 6964 2069 7320 4e6f 6e65  amera_id is None
+00019e60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00019e70: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
+00019e80: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+00019e90: 7069 2e62 6f6f 7473 7472 6170 2e63 616d  pi.bootstrap.cam
+00019ea0: 6572 6173 5b73 656c 662e 6361 6d65 7261  eras[self.camera
+00019eb0: 5f69 645d 0a0a 2020 2020 6173 796e 6320  _id]..    async 
+00019ec0: 6465 6620 7365 745f 7061 6972 6564 5f63  def set_paired_c
+00019ed0: 616d 6572 6128 7365 6c66 2c20 6361 6d65  amera(self, came
+00019ee0: 7261 3a20 4f70 7469 6f6e 616c 5b43 616d  ra: Optional[Cam
+00019ef0: 6572 615d 2920 2d3e 204e 6f6e 653a 0a20  era]) -> None:. 
+00019f00: 2020 2020 2020 2022 2222 5365 7473 2074         """Sets t
+00019f10: 6865 2063 616d 6572 6120 7061 6972 6564  he camera paired
+00019f20: 2077 6974 6820 7468 6520 7365 6e73 6f72   with the sensor
+00019f30: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
+00019f40: 2063 616c 6c62 6163 6b28 2920 2d3e 204e   callback() -> N
+00019f50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00019f60: 2069 6620 6361 6d65 7261 2069 7320 4e6f   if camera is No
+00019f70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019f80: 2020 2020 7365 6c66 2e63 616d 6572 615f      self.camera_
+00019f90: 6964 203d 204e 6f6e 650a 2020 2020 2020  id = None.      
+00019fa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00019fb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019fc0: 2e63 616d 6572 615f 6964 203d 2063 616d  .camera_id = cam
+00019fd0: 6572 612e 6964 0a0a 2020 2020 2020 2020  era.id..        
+00019fe0: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+00019ff0: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+0001a000: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+0001a010: 2073 6574 5f73 7461 7475 735f 6c69 6768   set_status_ligh
+0001a020: 7428 7365 6c66 2c20 656e 6162 6c65 643a  t(self, enabled:
+0001a030: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+0001a040: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+0001a050: 7468 6520 7374 6174 7573 2069 6e64 6963  the status indic
+0001a060: 6174 6f72 206c 6967 6874 2066 6f72 2074  ator light for t
+0001a070: 6865 2064 6f6f 726c 6f63 6b22 2222 0a0a  he doorlock"""..
+0001a080: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
+0001a090: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
+0001a0a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a0b0: 2e6c 6564 5f73 6574 7469 6e67 732e 6973  .led_settings.is
+0001a0c0: 5f65 6e61 626c 6564 203d 2065 6e61 626c  _enabled = enabl
+0001a0d0: 6564 0a0a 2020 2020 2020 2020 6177 6169  ed..        awai
+0001a0e0: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
+0001a0f0: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
+0001a100: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+0001a110: 5f61 7574 6f5f 636c 6f73 655f 7469 6d65  _auto_close_time
+0001a120: 2873 656c 662c 2064 7572 6174 696f 6e3a  (self, duration:
+0001a130: 2074 696d 6564 656c 7461 2920 2d3e 204e   timedelta) -> N
+0001a140: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0001a150: 5365 7473 2074 6865 2061 7574 6f2d 636c  Sets the auto-cl
+0001a160: 6f73 6520 7469 6d65 2066 6f72 2064 6f6f  ose time for doo
+0001a170: 726c 6f63 6b2e 2030 2073 6563 6f6e 6473  rlock. 0 seconds
+0001a180: 203d 2064 6973 6162 6c65 642e 2222 220a   = disabled.""".
+0001a190: 0a20 2020 2020 2020 2069 6620 6475 7261  .        if dura
+0001a1a0: 7469 6f6e 203e 2074 696d 6564 656c 7461  tion > timedelta
+0001a1b0: 2868 6f75 7273 3d31 293a 0a20 2020 2020  (hours=1):.     
+0001a1c0: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
+0001a1d0: 5265 7175 6573 7428 224d 6178 2064 7572  Request("Max dur
+0001a1e0: 6174 696f 6e20 6973 2031 2068 6f75 7222  ation is 1 hour"
+0001a1f0: 290a 0a20 2020 2020 2020 2064 6566 2063  )..        def c
+0001a200: 616c 6c62 6163 6b28 2920 2d3e 204e 6f6e  allback() -> Non
+0001a210: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001a220: 656c 662e 6175 746f 5f63 6c6f 7365 5f74  elf.auto_close_t
+0001a230: 696d 6520 3d20 6475 7261 7469 6f6e 0a0a  ime = duration..
+0001a240: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+0001a250: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
+0001a260: 6361 6c6c 6261 636b 290a 0a20 2020 2061  callback)..    a
+0001a270: 7379 6e63 2064 6566 2063 6c6f 7365 5f6c  sync def close_l
+0001a280: 6f63 6b28 7365 6c66 2920 2d3e 204e 6f6e  ock(self) -> Non
+0001a290: 653a 0a20 2020 2020 2020 2022 2222 436c  e:.        """Cl
+0001a2a0: 6f73 6520 646f 6f72 6c6f 636b 2028 6c6f  ose doorlock (lo
+0001a2b0: 636b 2922 2222 0a0a 2020 2020 2020 2020  ck)"""..        
+0001a2c0: 6966 2073 656c 662e 6c6f 636b 5f73 7461  if self.lock_sta
+0001a2d0: 7475 7320 213d 204c 6f63 6b53 7461 7475  tus != LockStatu
+0001a2e0: 7354 7970 652e 4f50 454e 3a0a 2020 2020  sType.OPEN:.    
+0001a2f0: 2020 2020 2020 2020 7261 6973 6520 4261          raise Ba
+0001a300: 6452 6571 7565 7374 2822 4c6f 636b 2069  dRequest("Lock i
+0001a310: 7320 6e6f 7420 6f70 656e 2229 0a0a 2020  s not open")..  
+0001a320: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+0001a330: 2e61 7069 2e63 6c6f 7365 5f6c 6f63 6b28  .api.close_lock(
+0001a340: 7365 6c66 2e69 6429 0a0a 2020 2020 6173  self.id)..    as
+0001a350: 796e 6320 6465 6620 6f70 656e 5f6c 6f63  ync def open_loc
+0001a360: 6b28 7365 6c66 2920 2d3e 204e 6f6e 653a  k(self) -> None:
+0001a370: 0a20 2020 2020 2020 2022 2222 4f70 656e  .        """Open
+0001a380: 2064 6f6f 726c 6f63 6b20 2875 6e6c 6f63   doorlock (unloc
+0001a390: 6b29 2222 220a 0a20 2020 2020 2020 2069  k)"""..        i
+0001a3a0: 6620 7365 6c66 2e6c 6f63 6b5f 7374 6174  f self.lock_stat
+0001a3b0: 7573 2021 3d20 4c6f 636b 5374 6174 7573  us != LockStatus
+0001a3c0: 5479 7065 2e43 4c4f 5345 443a 0a20 2020  Type.CLOSED:.   
+0001a3d0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+0001a3e0: 6164 5265 7175 6573 7428 224c 6f63 6b20  adRequest("Lock 
+0001a3f0: 6973 206e 6f74 2063 6c6f 7365 6422 290a  is not closed").
+0001a400: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+0001a410: 656c 662e 6170 692e 6f70 656e 5f6c 6f63  elf.api.open_loc
+0001a420: 6b28 7365 6c66 2e69 6429 0a0a 2020 2020  k(self.id)..    
+0001a430: 6173 796e 6320 6465 6620 6361 6c69 6272  async def calibr
+0001a440: 6174 6528 7365 6c66 2920 2d3e 204e 6f6e  ate(self) -> Non
+0001a450: 653a 0a20 2020 2020 2020 2022 2222 4361  e:.        """Ca
+0001a460: 6c69 6272 6174 6520 7468 6520 646f 6f72  librate the door
+0001a470: 6c6f 636b 2e0a 0a20 2020 2020 2020 2044  lock...        D
+0001a480: 6f6f 7220 6d75 7374 2062 6520 6f70 656e  oor must be open
+0001a490: 2061 6e64 206c 6f63 6b20 756e 6c6f 636b   and lock unlock
+0001a4a0: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
+0001a4b0: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+0001a4c0: 656c 662e 6170 692e 6361 6c69 6272 6174  elf.api.calibrat
+0001a4d0: 655f 6c6f 636b 2873 656c 662e 6964 290a  e_lock(self.id).
+0001a4e0: 0a0a 636c 6173 7320 4368 696d 6546 6561  ..class ChimeFea
+0001a4f0: 7475 7265 466c 6167 7328 5072 6f74 6563  tureFlags(Protec
+0001a500: 7442 6173 654f 626a 6563 7429 3a0a 2020  tBaseObject):.  
+0001a510: 2020 6861 735f 7769 6669 3a20 626f 6f6c    has_wifi: bool
+0001a520: 0a20 2020 2023 2032 2e39 2e32 302b 0a20  .    # 2.9.20+. 
+0001a530: 2020 2068 6173 5f68 7474 7073 5f63 6c69     has_https_cli
+0001a540: 656e 745f 6f74 613a 204f 7074 696f 6e61  ent_ota: Optiona
+0001a550: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a  l[bool] = None..
+0001a560: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+0001a570: 0a20 2020 2040 6361 6368 650a 2020 2020  .    @cache.    
+0001a580: 6465 6620 5f67 6574 5f75 6e69 6669 5f72  def _get_unifi_r
+0001a590: 656d 6170 7328 636c 7329 202d 3e20 6469  emaps(cls) -> di
+0001a5a0: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
+0001a5b0: 2020 2020 2020 7265 7475 726e 207b 2a2a        return {**
+0001a5c0: 7375 7065 7228 292e 5f67 6574 5f75 6e69  super()._get_uni
+0001a5d0: 6669 5f72 656d 6170 7328 292c 2022 6861  fi_remaps(), "ha
+0001a5e0: 7348 7474 7073 436c 6965 6e74 4f54 4122  sHttpsClientOTA"
+0001a5f0: 3a20 2268 6173 4874 7470 7343 6c69 656e  : "hasHttpsClien
+0001a600: 744f 7461 227d 0a0a 0a63 6c61 7373 2052  tOta"}...class R
+0001a610: 696e 6753 6574 7469 6e67 2850 726f 7465  ingSetting(Prote
+0001a620: 6374 4261 7365 4f62 6a65 6374 293a 0a20  ctBaseObject):. 
+0001a630: 2020 2063 616d 6572 615f 6964 3a20 7374     camera_id: st
+0001a640: 720a 2020 2020 7265 7065 6174 5f74 696d  r.    repeat_tim
+0001a650: 6573 3a20 5265 7065 6174 5469 6d65 730a  es: RepeatTimes.
+0001a660: 2020 2020 7472 6163 6b5f 6e6f 3a20 696e      track_no: in
+0001a670: 740a 2020 2020 766f 6c75 6d65 3a20 696e  t.    volume: in
+0001a680: 740a 0a20 2020 2040 636c 6173 736d 6574  t..    @classmet
+0001a690: 686f 640a 2020 2020 4063 6163 6865 0a20  hod.    @cache. 
+0001a6a0: 2020 2064 6566 205f 6765 745f 756e 6966     def _get_unif
+0001a6b0: 695f 7265 6d61 7073 2863 6c73 2920 2d3e  i_remaps(cls) ->
+0001a6c0: 2064 6963 745b 7374 722c 2073 7472 5d3a   dict[str, str]:
+0001a6d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a6e0: 7b2a 2a73 7570 6572 2829 2e5f 6765 745f  {**super()._get_
+0001a6f0: 756e 6966 695f 7265 6d61 7073 2829 2c20  unifi_remaps(), 
+0001a700: 2263 616d 6572 6122 3a20 2263 616d 6572  "camera": "camer
+0001a710: 6149 6422 7d0a 0a20 2020 2040 7072 6f70  aId"}..    @prop
+0001a720: 6572 7479 0a20 2020 2064 6566 2063 616d  erty.    def cam
+0001a730: 6572 6128 7365 6c66 2920 2d3e 204f 7074  era(self) -> Opt
+0001a740: 696f 6e61 6c5b 4361 6d65 7261 5d3a 0a20  ional[Camera]:. 
+0001a750: 2020 2020 2020 2022 2222 5061 6972 6564         """Paired
+0001a760: 2043 616d 6572 6120 7769 6c6c 2061 6c77   Camera will alw
+0001a770: 6179 7320 6265 206e 6f6e 6520 6966 206e  ays be none if n
+0001a780: 6f20 6361 6d65 7261 2069 7320 7061 6972  o camera is pair
+0001a790: 6564 2222 220a 0a20 2020 2020 2020 2069  ed"""..        i
+0001a7a0: 6620 7365 6c66 2e63 616d 6572 615f 6964  f self.camera_id
+0001a7b0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001a7c0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0001a7d0: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+0001a7e0: 6e20 7365 6c66 2e61 7069 2e62 6f6f 7473  n self.api.boots
+0001a7f0: 7472 6170 2e63 616d 6572 6173 5b73 656c  trap.cameras[sel
+0001a800: 662e 6361 6d65 7261 5f69 645d 0a0a 0a63  f.camera_id]...c
+0001a810: 6c61 7373 2043 6869 6d65 5472 6163 6b28  lass ChimeTrack(
+0001a820: 5072 6f74 6563 7442 6173 654f 626a 6563  ProtectBaseObjec
+0001a830: 7429 3a0a 2020 2020 6d64 353a 2073 7472  t):.    md5: str
+0001a840: 0a20 2020 206e 616d 653a 2073 7472 0a20  .    name: str. 
+0001a850: 2020 2073 7461 7465 3a20 7374 720a 2020     state: str.  
+0001a860: 2020 7472 6163 6b5f 6e6f 3a20 696e 740a    track_no: int.
+0001a870: 2020 2020 766f 6c75 6d65 3a20 696e 740a      volume: int.
+0001a880: 2020 2020 7369 7a65 3a20 696e 740a 0a20      size: int.. 
+0001a890: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0001a8a0: 2020 2020 4063 6163 6865 0a20 2020 2064      @cache.    d
+0001a8b0: 6566 205f 6765 745f 756e 6966 695f 7265  ef _get_unifi_re
+0001a8c0: 6d61 7073 2863 6c73 2920 2d3e 2064 6963  maps(cls) -> dic
+0001a8d0: 745b 7374 722c 2073 7472 5d3a 0a20 2020  t[str, str]:.   
+0001a8e0: 2020 2020 2072 6574 7572 6e20 7b2a 2a73       return {**s
+0001a8f0: 7570 6572 2829 2e5f 6765 745f 756e 6966  uper()._get_unif
+0001a900: 695f 7265 6d61 7073 2829 2c20 2274 7261  i_remaps(), "tra
+0001a910: 636b 5f6e 6f22 3a20 2274 7261 636b 4e6f  ck_no": "trackNo
+0001a920: 227d 0a0a 0a63 6c61 7373 2043 6869 6d65  "}...class Chime
+0001a930: 2850 726f 7465 6374 4164 6f70 7461 626c  (ProtectAdoptabl
+0001a940: 6544 6576 6963 654d 6f64 656c 293a 0a20  eDeviceModel):. 
+0001a950: 2020 2076 6f6c 756d 653a 2050 6572 6365     volume: Perce
+0001a960: 6e74 496e 740a 2020 2020 6973 5f70 726f  ntInt.    is_pro
+0001a970: 6269 6e67 5f66 6f72 5f77 6966 693a 2062  bing_for_wifi: b
+0001a980: 6f6f 6c0a 2020 2020 6c61 7374 5f72 696e  ool.    last_rin
+0001a990: 673a 204f 7074 696f 6e61 6c5b 6461 7465  g: Optional[date
+0001a9a0: 7469 6d65 5d0a 2020 2020 6973 5f77 6972  time].    is_wir
+0001a9b0: 656c 6573 735f 7570 6c69 6e6b 5f65 6e61  eless_uplink_ena
+0001a9c0: 626c 6564 3a20 626f 6f6c 0a20 2020 2063  bled: bool.    c
+0001a9d0: 616d 6572 615f 6964 733a 206c 6973 745b  amera_ids: list[
+0001a9e0: 7374 725d 0a20 2020 2023 2072 6571 7569  str].    # requi
+0001a9f0: 7265 7320 322e 362e 3137 2b0a 2020 2020  res 2.6.17+.    
+0001aa00: 6170 5f6d 676d 745f 6970 3a20 4f70 7469  ap_mgmt_ip: Opti
+0001aa10: 6f6e 616c 5b49 5076 3441 6464 7265 7373  onal[IPv4Address
+0001aa20: 5d20 3d20 4e6f 6e65 0a20 2020 2023 2072  ] = None.    # r
+0001aa30: 6571 7569 7265 7320 322e 372e 3135 2b0a  equires 2.7.15+.
+0001aa40: 2020 2020 6665 6174 7572 655f 666c 6167      feature_flag
+0001aa50: 733a 204f 7074 696f 6e61 6c5b 4368 696d  s: Optional[Chim
+0001aa60: 6546 6561 7475 7265 466c 6167 735d 203d  eFeatureFlags] =
+0001aa70: 204e 6f6e 650a 2020 2020 2320 7265 7175   None.    # requ
+0001aa80: 6972 6573 2032 2e38 2e32 322b 0a20 2020  ires 2.8.22+.   
+0001aa90: 2075 7365 725f 636f 6e66 6967 7572 6564   user_configured
+0001aaa0: 5f61 703a 204f 7074 696f 6e61 6c5b 626f  _ap: Optional[bo
+0001aab0: 6f6c 5d20 3d20 4e6f 6e65 0a20 2020 2023  ol] = None.    #
+0001aac0: 2072 6571 7569 7265 7320 332e 302e 3232   requires 3.0.22
+0001aad0: 2b0a 2020 2020 6861 735f 6874 7470 735f  +.    has_https_
+0001aae0: 636c 6965 6e74 5f6f 7461 3a20 4f70 7469  client_ota: Opti
+0001aaf0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+0001ab00: 650a 2020 2020 706c 6174 666f 726d 3a20  e.    platform: 
+0001ab10: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001ab20: 4e6f 6e65 0a20 2020 2072 6570 6561 745f  None.    repeat_
+0001ab30: 7469 6d65 733a 204f 7074 696f 6e61 6c5b  times: Optional[
+0001ab40: 5265 7065 6174 5469 6d65 735d 203d 204e  RepeatTimes] = N
+0001ab50: 6f6e 650a 2020 2020 7472 6163 6b5f 6e6f  one.    track_no
+0001ab60: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0001ab70: 3d20 4e6f 6e65 0a20 2020 2072 696e 675f  = None.    ring_
+0001ab80: 7365 7474 696e 6773 3a20 6c69 7374 5b52  settings: list[R
+0001ab90: 696e 6753 6574 7469 6e67 5d20 3d20 5b5d  ingSetting] = []
+0001aba0: 0a20 2020 2073 7065 616b 6572 5f74 7261  .    speaker_tra
+0001abb0: 636b 5f6c 6973 743a 206c 6973 745b 4368  ck_list: list[Ch
+0001abc0: 696d 6554 7261 636b 5d20 3d20 5b5d 0a0a  imeTrack] = []..
+0001abd0: 2020 2020 2320 544f 444f 3a20 7573 6564      # TODO: used
+0001abe0: 2066 6f72 2061 646f 7074 696f 6e0a 2020   for adoption.  
+0001abf0: 2020 2320 6170 4d61 6320 2072 6561 6420    # apMac  read 
+0001ac00: 6f6e 6c79 0a20 2020 2023 2061 7052 7373  only.    # apRss
+0001ac10: 6920 2072 6561 6420 6f6e 6c79 0a20 2020  i  read only.   
+0001ac20: 2023 2065 6c65 6d65 6e74 496e 666f 2020   # elementInfo  
+0001ac30: 7265 6164 206f 6e6c 790a 0a20 2020 2040  read only..    @
+0001ac40: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+0001ac50: 4063 6163 6865 0a20 2020 2064 6566 205f  @cache.    def _
+0001ac60: 6765 745f 756e 6966 695f 7265 6d61 7073  get_unifi_remaps
+0001ac70: 2863 6c73 2920 2d3e 2064 6963 745b 7374  (cls) -> dict[st
+0001ac80: 722c 2073 7472 5d3a 0a20 2020 2020 2020  r, str]:.       
+0001ac90: 2072 6574 7572 6e20 7b2a 2a73 7570 6572   return {**super
+0001aca0: 2829 2e5f 6765 745f 756e 6966 695f 7265  ()._get_unifi_re
+0001acb0: 6d61 7073 2829 2c20 2268 6173 4874 7470  maps(), "hasHttp
+0001acc0: 7343 6c69 656e 744f 5441 223a 2022 6861  sClientOTA": "ha
+0001acd0: 7348 7474 7073 436c 6965 6e74 4f74 6122  sHttpsClientOta"
+0001ace0: 7d0a 0a20 2020 2040 636c 6173 736d 6574  }..    @classmet
+0001acf0: 686f 640a 2020 2020 4063 6163 6865 0a20  hod.    @cache. 
+0001ad00: 2020 2064 6566 205f 6765 745f 7265 6164     def _get_read
+0001ad10: 5f6f 6e6c 795f 6669 656c 6473 2863 6c73  _only_fields(cls
+0001ad20: 2920 2d3e 2073 6574 5b73 7472 5d3a 0a20  ) -> set[str]:. 
+0001ad30: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+0001ad40: 7065 7228 292e 5f67 6574 5f72 6561 645f  per()._get_read_
+0001ad50: 6f6e 6c79 5f66 6965 6c64 7328 2920 7c20  only_fields() | 
+0001ad60: 7b22 6973 5072 6f62 696e 6746 6f72 5769  {"isProbingForWi
+0001ad70: 6669 222c 2022 6c61 7374 5269 6e67 227d  fi", "lastRing"}
+0001ad80: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0001ad90: 2020 2020 6465 6620 6361 6d65 7261 7328      def cameras(
+0001ada0: 7365 6c66 2920 2d3e 206c 6973 745b 4361  self) -> list[Ca
+0001adb0: 6d65 7261 5d3a 0a20 2020 2020 2020 2022  mera]:.        "
+0001adc0: 2222 5061 6972 6564 2043 616d 6572 6173  ""Paired Cameras
+0001add0: 2066 6f72 2063 6869 6d65 2222 220a 0a20   for chime""".. 
+0001ade0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+0001adf0: 6c66 2e63 616d 6572 615f 6964 7329 203d  lf.camera_ids) =
+0001ae00: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001ae10: 2072 6574 7572 6e20 5b5d 0a20 2020 2020   return [].     
+0001ae20: 2020 2072 6574 7572 6e20 5b73 656c 662e     return [self.
+0001ae30: 6170 692e 626f 6f74 7374 7261 702e 6361  api.bootstrap.ca
+0001ae40: 6d65 7261 735b 635d 2066 6f72 2063 2069  meras[c] for c i
+0001ae50: 6e20 7365 6c66 2e63 616d 6572 615f 6964  n self.camera_id
+0001ae60: 735d 0a0a 2020 2020 6173 796e 6320 6465  s]..    async de
+0001ae70: 6620 7365 745f 766f 6c75 6d65 2873 656c  f set_volume(sel
+0001ae80: 662c 206c 6576 656c 3a20 696e 7429 202d  f, level: int) -
+0001ae90: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0001aea0: 2222 2253 6574 2074 6865 2076 6f6c 756d  """Set the volum
+0001aeb0: 6520 6f6e 2063 6869 6d65 2e22 2222 0a0a  e on chime."""..
+0001aec0: 2020 2020 2020 2020 6f6c 645f 7661 6c75          old_valu
+0001aed0: 6520 3d20 7365 6c66 2e76 6f6c 756d 650a  e = self.volume.
+0001aee0: 2020 2020 2020 2020 6e65 775f 7661 6c75          new_valu
+0001aef0: 6520 3d20 5065 7263 656e 7449 6e74 286c  e = PercentInt(l
+0001af00: 6576 656c 290a 0a20 2020 2020 2020 2064  evel)..        d
+0001af10: 6566 2063 616c 6c62 6163 6b28 2920 2d3e  ef callback() ->
+0001af20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001af30: 2020 2073 656c 662e 766f 6c75 6d65 203d     self.volume =
+0001af40: 206e 6577 5f76 616c 7565 0a20 2020 2020   new_value.     
+0001af50: 2020 2020 2020 2066 6f72 2073 6574 7469         for setti
+0001af60: 6e67 2069 6e20 7365 6c66 2e72 696e 675f  ng in self.ring_
+0001af70: 7365 7474 696e 6773 3a0a 2020 2020 2020  settings:.      
+0001af80: 2020 2020 2020 2020 2020 6966 2073 6574            if set
+0001af90: 7469 6e67 2e76 6f6c 756d 6520 3d3d 206f  ting.volume == o
+0001afa0: 6c64 5f76 616c 7565 3a0a 2020 2020 2020  ld_value:.      
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001afc0: 7474 696e 672e 766f 6c75 6d65 203d 206e  tting.volume = n
+0001afd0: 6577 5f76 616c 7565 0a0a 2020 2020 2020  ew_value..      
+0001afe0: 2020 6177 6169 7420 7365 6c66 2e71 7565    await self.que
+0001aff0: 7565 5f75 7064 6174 6528 6361 6c6c 6261  ue_update(callba
+0001b000: 636b 290a 0a20 2020 2061 7379 6e63 2064  ck)..    async d
+0001b010: 6566 2073 6574 5f76 6f6c 756d 655f 666f  ef set_volume_fo
+0001b020: 725f 6361 6d65 7261 2873 656c 662c 2063  r_camera(self, c
+0001b030: 616d 6572 613a 2043 616d 6572 612c 206c  amera: Camera, l
+0001b040: 6576 656c 3a20 696e 7429 202d 3e20 4e6f  evel: int) -> No
+0001b050: 6e65 3a0a 2020 2020 2020 2020 2222 2253  ne:.        """S
+0001b060: 6574 2074 6865 2076 6f6c 756d 6520 6f6e  et the volume on
+0001b070: 2063 6869 6d65 2066 6f72 2073 7065 6369   chime for speci
+0001b080: 6669 6320 6361 6d65 7261 2e22 2222 0a0a  fic camera."""..
+0001b090: 2020 2020 2020 2020 6465 6620 6361 6c6c          def call
+0001b0a0: 6261 636b 2829 202d 3e20 4e6f 6e65 3a0a  back() -> None:.
+0001b0b0: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
+0001b0c0: 6c65 6420 3d20 4661 6c73 650a 2020 2020  led = False.    
+0001b0d0: 2020 2020 2020 2020 666f 7220 7365 7474          for sett
+0001b0e0: 696e 6720 696e 2073 656c 662e 7269 6e67  ing in self.ring
+0001b0f0: 5f73 6574 7469 6e67 733a 0a20 2020 2020  _settings:.     
+0001b100: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0001b110: 7474 696e 672e 6361 6d65 7261 5f69 6420  tting.camera_id 
+0001b120: 3d3d 2063 616d 6572 612e 6964 3a0a 2020  == camera.id:.  
+0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b140: 2020 7365 7474 696e 672e 766f 6c75 6d65    setting.volume
+0001b150: 203d 2063 6173 7428 5065 7263 656e 7449   = cast(PercentI
+0001b160: 6e74 2c20 6c65 7665 6c29 0a20 2020 2020  nt, level).     
+0001b170: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0001b180: 616e 646c 6564 203d 2054 7275 650a 2020  andled = True.  
+0001b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1a0: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
+0001b1b0: 2020 2020 2069 6620 6e6f 7420 6861 6e64       if not hand
+0001b1c0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+0001b1d0: 2020 2020 2072 6169 7365 2042 6164 5265       raise BadRe
+0001b1e0: 7175 6573 7428 2243 616d 6572 6120 2573  quest("Camera %s
+0001b1f0: 2069 7320 6e6f 7420 7061 6972 6564 2077   is not paired w
+0001b200: 6974 6820 6368 696d 6522 2c20 6361 6d65  ith chime", came
+0001b210: 7261 2e69 6429 0a0a 2020 2020 2020 2020  ra.id)..        
+0001b220: 6177 6169 7420 7365 6c66 2e71 7565 7565  await self.queue
+0001b230: 5f75 7064 6174 6528 6361 6c6c 6261 636b  _update(callback
+0001b240: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+0001b250: 2061 6464 5f63 616d 6572 6128 7365 6c66   add_camera(self
+0001b260: 2c20 6361 6d65 7261 3a20 4361 6d65 7261  , camera: Camera
+0001b270: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0001b280: 2020 2022 2222 4164 6473 206e 6577 2070     """Adds new p
+0001b290: 6169 7265 6420 6361 6d65 7261 2074 6f20  aired camera to 
+0001b2a0: 6368 696d 6522 2222 0a0a 2020 2020 2020  chime"""..      
+0001b2b0: 2020 6966 206e 6f74 2063 616d 6572 612e    if not camera.
+0001b2c0: 6665 6174 7572 655f 666c 6167 732e 6973  feature_flags.is
+0001b2d0: 5f64 6f6f 7262 656c 6c3a 0a20 2020 2020  _doorbell:.     
+0001b2e0: 2020 2020 2020 2072 6169 7365 2042 6164         raise Bad
+0001b2f0: 5265 7175 6573 7428 2243 616d 6572 6120  Request("Camera 
+0001b300: 646f 6573 206e 6f74 2068 6176 6520 6120  does not have a 
+0001b310: 6368 696d 6522 290a 0a20 2020 2020 2020  chime")..       
+0001b320: 2069 6620 6361 6d65 7261 2e69 6420 696e   if camera.id in
+0001b330: 2073 656c 662e 6361 6d65 7261 5f69 6473   self.camera_ids
+0001b340: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001b350: 6973 6520 4261 6452 6571 7565 7374 2822  ise BadRequest("
+0001b360: 4361 6d65 7261 2069 7320 616c 7265 6164  Camera is alread
+0001b370: 7920 7061 6972 6564 2229 0a0a 2020 2020  y paired")..    
+0001b380: 2020 2020 6465 6620 6361 6c6c 6261 636b      def callback
+0001b390: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
+0001b3a0: 2020 2020 2020 2020 7365 6c66 2e63 616d          self.cam
+0001b3b0: 6572 615f 6964 732e 6170 7065 6e64 2863  era_ids.append(c
+0001b3c0: 616d 6572 612e 6964 290a 0a20 2020 2020  amera.id)..     
+0001b3d0: 2020 2061 7761 6974 2073 656c 662e 7175     await self.qu
+0001b3e0: 6575 655f 7570 6461 7465 2863 616c 6c62  eue_update(callb
+0001b3f0: 6163 6b29 0a0a 2020 2020 6173 796e 6320  ack)..    async 
+0001b400: 6465 6620 7265 6d6f 7665 5f63 616d 6572  def remove_camer
+0001b410: 6128 7365 6c66 2c20 6361 6d65 7261 3a20  a(self, camera: 
+0001b420: 4361 6d65 7261 2920 2d3e 204e 6f6e 653a  Camera) -> None:
+0001b430: 0a20 2020 2020 2020 2022 2222 5265 6d6f  .        """Remo
+0001b440: 7665 7320 7061 6972 6564 2063 616d 6572  ves paired camer
+0001b450: 6120 6672 6f6d 2063 6869 6d65 2222 220a  a from chime""".
+0001b460: 0a20 2020 2020 2020 2069 6620 6361 6d65  .        if came
+0001b470: 7261 2e69 6420 6e6f 7420 696e 2073 656c  ra.id not in sel
+0001b480: 662e 6361 6d65 7261 5f69 6473 3a0a 2020  f.camera_ids:.  
+0001b490: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001b4a0: 4261 6452 6571 7565 7374 2822 4361 6d65  BadRequest("Came
+0001b4b0: 7261 2069 7320 6e6f 7420 7061 6972 6564  ra is not paired
+0001b4c0: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
+0001b4d0: 6361 6c6c 6261 636b 2829 202d 3e20 4e6f  callback() -> No
+0001b4e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001b4f0: 7365 6c66 2e63 616d 6572 615f 6964 732e  self.camera_ids.
+0001b500: 7265 6d6f 7665 2863 616d 6572 612e 6964  remove(camera.id
+0001b510: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
+0001b520: 2073 656c 662e 7175 6575 655f 7570 6461   self.queue_upda
+0001b530: 7465 2863 616c 6c62 6163 6b29 0a0a 2020  te(callback)..  
+0001b540: 2020 6173 796e 6320 6465 6620 706c 6179    async def play
+0001b550: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0001b560: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0001b570: 2020 2076 6f6c 756d 653a 2069 6e74 207c     volume: int |
+0001b580: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
+0001b590: 2020 2020 2020 7265 7065 6174 5f74 696d        repeat_tim
+0001b5a0: 6573 3a20 696e 7420 7c20 4e6f 6e65 203d  es: int | None =
+0001b5b0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+0001b5c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0001b5d0: 2250 6c61 7973 2063 6869 6d65 2074 6f6e  "Plays chime ton
+0001b5e0: 6522 2222 0a0a 2020 2020 2020 2020 6177  e"""..        aw
+0001b5f0: 6169 7420 7365 6c66 2e61 7069 2e70 6c61  ait self.api.pla
+0001b600: 795f 7370 6561 6b65 7228 7365 6c66 2e69  y_speaker(self.i
+0001b610: 642c 2076 6f6c 756d 653d 766f 6c75 6d65  d, volume=volume
+0001b620: 2c20 7265 7065 6174 5f74 696d 6573 3d72  , repeat_times=r
+0001b630: 6570 6561 745f 7469 6d65 7329 0a0a 2020  epeat_times)..  
+0001b640: 2020 6173 796e 6320 6465 6620 706c 6179    async def play
+0001b650: 5f62 757a 7a65 7228 7365 6c66 2920 2d3e  _buzzer(self) ->
+0001b660: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0001b670: 2222 506c 6179 7320 6368 696d 6520 6275  ""Plays chime bu
+0001b680: 7a7a 6572 2222 220a 0a20 2020 2020 2020  zzer"""..       
+0001b690: 2061 7761 6974 2073 656c 662e 6170 692e   await self.api.
+0001b6a0: 706c 6179 5f62 757a 7a65 7228 7365 6c66  play_buzzer(self
+0001b6b0: 2e69 6429 0a0a 2020 2020 6173 796e 6320  .id)..    async 
+0001b6c0: 6465 6620 7365 745f 7265 7065 6174 5f74  def set_repeat_t
+0001b6d0: 696d 6573 2873 656c 662c 2076 616c 7565  imes(self, value
+0001b6e0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+0001b6f0: 2020 2020 2020 2020 2222 2253 6574 2072          """Set r
+0001b700: 6570 6561 7420 7469 6d65 7320 6f6e 2063  epeat times on c
+0001b710: 6869 6d65 2e22 2222 0a0a 2020 2020 2020  hime."""..      
+0001b720: 2020 6f6c 645f 7661 6c75 6520 3d20 7365    old_value = se
+0001b730: 6c66 2e72 6570 6561 745f 7469 6d65 730a  lf.repeat_times.
+0001b740: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
+0001b750: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
+0001b760: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001b770: 662e 7265 7065 6174 5f74 696d 6573 203d  f.repeat_times =
+0001b780: 2063 6173 7428 5265 7065 6174 5469 6d65   cast(RepeatTime
+0001b790: 732c 2076 616c 7565 290a 2020 2020 2020  s, value).      
+0001b7a0: 2020 2020 2020 666f 7220 7365 7474 696e        for settin
+0001b7b0: 6720 696e 2073 656c 662e 7269 6e67 5f73  g in self.ring_s
+0001b7c0: 6574 7469 6e67 733a 0a20 2020 2020 2020  ettings:.       
+0001b7d0: 2020 2020 2020 2020 2069 6620 7365 7474           if sett
+0001b7e0: 696e 672e 7265 7065 6174 5f74 696d 6573  ing.repeat_times
+0001b7f0: 203d 3d20 6f6c 645f 7661 6c75 653a 0a20   == old_value:. 
+0001b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b810: 2020 2073 6574 7469 6e67 2e72 6570 6561     setting.repea
+0001b820: 745f 7469 6d65 7320 3d20 6361 7374 2852  t_times = cast(R
+0001b830: 6570 6561 7454 696d 6573 2c20 7661 6c75  epeatTimes, valu
+0001b840: 6529 0a0a 2020 2020 2020 2020 6177 6169  e)..        awai
+0001b850: 7420 7365 6c66 2e71 7565 7565 5f75 7064  t self.queue_upd
+0001b860: 6174 6528 6361 6c6c 6261 636b 290a 0a20  ate(callback).. 
+0001b870: 2020 2061 7379 6e63 2064 6566 2073 6574     async def set
+0001b880: 5f72 6570 6561 745f 7469 6d65 735f 666f  _repeat_times_fo
+0001b890: 725f 6361 6d65 7261 280a 2020 2020 2020  r_camera(.      
+0001b8a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0001b8b0: 6361 6d65 7261 3a20 4361 6d65 7261 2c0a  camera: Camera,.
+0001b8c0: 2020 2020 2020 2020 7661 6c75 653a 2069          value: i
+0001b8d0: 6e74 2c0a 2020 2020 2920 2d3e 204e 6f6e  nt,.    ) -> Non
+0001b8e0: 653a 0a20 2020 2020 2020 2022 2222 5365  e:.        """Se
+0001b8f0: 7420 7265 7065 6174 2074 696d 6573 206f  t repeat times o
+0001b900: 6e20 6368 696d 6520 666f 7220 7370 6563  n chime for spec
+0001b910: 6966 6963 2063 616d 6572 612e 2222 220a  ific camera.""".
+0001b920: 0a20 2020 2020 2020 2064 6566 2063 616c  .        def cal
+0001b930: 6c62 6163 6b28 2920 2d3e 204e 6f6e 653a  lback() -> None:
+0001b940: 0a20 2020 2020 2020 2020 2020 2068 616e  .            han
+0001b950: 646c 6564 203d 2046 616c 7365 0a20 2020  dled = False.   
+0001b960: 2020 2020 2020 2020 2066 6f72 2073 6574           for set
+0001b970: 7469 6e67 2069 6e20 7365 6c66 2e72 696e  ting in self.rin
+0001b980: 675f 7365 7474 696e 6773 3a0a 2020 2020  g_settings:.    
+0001b990: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001b9a0: 6574 7469 6e67 2e63 616d 6572 615f 6964  etting.camera_id
+0001b9b0: 203d 3d20 6361 6d65 7261 2e69 643a 0a20   == camera.id:. 
+0001b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9d0: 2020 2073 6574 7469 6e67 2e72 6570 6561     setting.repea
+0001b9e0: 745f 7469 6d65 7320 3d20 6361 7374 2852  t_times = cast(R
+0001b9f0: 6570 6561 7454 696d 6573 2c20 7661 6c75  epeatTimes, valu
+0001ba00: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0001ba10: 2020 2020 2020 2068 616e 646c 6564 203d         handled =
+0001ba20: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0001ba30: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0001ba40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001ba50: 6e6f 7420 6861 6e64 6c65 643a 0a20 2020  not handled:.   
+0001ba60: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0001ba70: 7365 2042 6164 5265 7175 6573 7428 2243  se BadRequest("C
+0001ba80: 616d 6572 6120 2573 2069 7320 6e6f 7420  amera %s is not 
+0001ba90: 7061 6972 6564 2077 6974 6820 6368 696d  paired with chim
+0001baa0: 6522 2c20 6361 6d65 7261 2e69 6429 0a0a  e", camera.id)..
+0001bab0: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+0001bac0: 6c66 2e71 7565 7565 5f75 7064 6174 6528  lf.queue_update(
+0001bad0: 6361 6c6c 6261 636b 290a                 callback).
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/nvr.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/nvr.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,57 +11,59 @@
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, Optional, Union
 from uuid import UUID
 import zoneinfo
 
 import aiofiles
 from aiofiles import os as aos
 import orjson
+from pydantic.v1.fields import PrivateAttr
 
 from pyunifiprotect.data.base import (
     ProtectBaseObject,
     ProtectDeviceModel,
     ProtectModelWithId,
 )
-from pyunifiprotect.data.devices import Camera, CameraZone, Light, Sensor
+from pyunifiprotect.data.devices import (
+    Camera,
+    CameraZone,
+    Light,
+    OSDSettings,
+    RecordingSettings,
+    Sensor,
+    SmartDetectSettings,
+)
 from pyunifiprotect.data.types import (
     AnalyticsOption,
     DoorbellMessageType,
     DoorbellText,
     EventCategories,
     EventType,
     FirmwareReleaseChannel,
     IteratorCallback,
     ModelType,
     MountType,
     PercentFloat,
     PercentInt,
     PermissionNode,
     ProgressCallback,
+    RecordingMode,
     RecordingType,
     ResolutionStorageType,
     SensorStatusType,
     SensorType,
     SmartDetectObjectType,
     StorageType,
     Version,
 )
 from pyunifiprotect.data.user import User, UserLocation
 from pyunifiprotect.exceptions import BadRequest, NotAuthorized
 from pyunifiprotect.utils import RELEASE_CACHE, process_datetime
 
-try:
-    from pydantic.v1.fields import PrivateAttr
-except ImportError:
-    from pydantic.fields import PrivateAttr
-
 if TYPE_CHECKING:
-    try:
-        from pydantic.v1.typing import SetStr
-    except ImportError:
-        from pydantic.typing import SetStr
+    from pydantic.v1.typing import SetStr
 
 
 _LOGGER = logging.getLogger(__name__)
 MAX_SUPPORTED_CAMERAS = 256
 MAX_EVENT_HISTORY_IN_STATE_MACHINE = MAX_SUPPORTED_CAMERAS * 2
 DELETE_KEYS_THUMB = {"color", "vehicleType"}
 DELETE_KEYS_EVENT = {"deletedAt", "category", "subCategory"}
@@ -481,15 +483,15 @@
             raise BadRequest("No camera on event")
 
         if self._smart_detect_zones is None:
             smart_track = await self.get_smart_detect_track()
 
             ids: set[int] = set()
             for item in smart_track.payload:
-                ids = ids | set(item.zone_ids)
+                ids |= set(item.zone_ids)
 
             self._smart_detect_zones = {
                 z.id: z for z in self.camera.smart_detect_zones if z.id in ids
             }
 
         return self._smart_detect_zones
 
@@ -629,15 +631,15 @@
         data: Optional[dict[str, Any]] = None,
         exclude: Optional[set[str]] = None,
     ) -> dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         # estimate is actually in seconds, not milliseconds
         if "estimate" in data and data["estimate"] is not None:
-            data["estimate"] = data["estimate"] / 1000
+            data["estimate"] /= 1000
 
         if "state" in data and data["state"] == "nodisk":
             delete_keys = [
                 "action",
                 "ata",
                 "bad_sector",
                 "estimate",
@@ -713,15 +715,15 @@
         data: Optional[dict[str, Any]] = None,
         exclude: Optional[set[str]] = None,
     ) -> dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         # estimate is actually in seconds, not milliseconds
         if "estimate" in data and data["estimate"] is not None:
-            data["estimate"] = data["estimate"] / 1000
+            data["estimate"] /= 1000
 
         return data
 
 
 class UOSStorage(ProtectBaseObject):
     disks: list[UOSDisk]
     space: list[UOSSpace]
@@ -888,14 +890,23 @@
 
 class NVRSmartDetection(ProtectBaseObject):
     enable: bool
     face_recognition: bool
     license_plate_recognition: bool
 
 
+class GlobalRecordingSettings(ProtectBaseObject):
+    osd_settings: OSDSettings
+    recording_settings: RecordingSettings
+    smart_detect_settings: SmartDetectSettings
+
+    # TODO:
+    # recordingSchedulesV2
+
+
 class NVR(ProtectDeviceModel):
     can_auto_update: bool
     is_stats_gathering_enabled: bool
     timezone: tzinfo
     version: Version
     ucore_version: str
     hardware_platform: str
@@ -959,21 +970,21 @@
     is_protect_updatable: Optional[bool] = None
     is_ucore_updatable: Optional[bool] = None
     # requires 2.11.13+
     last_device_fw_updates_checked_at: Optional[datetime] = None
     # requires 3.0.22+
     smart_detection: Optional[NVRSmartDetection] = None
     is_ucore_stacked: Optional[bool] = None
+    global_camera_settings: Optional[GlobalRecordingSettings] = None
 
     # TODO:
     # errorCode   read only
     # wifiSettings
     # smartDetectAgreement
     # dbRecoveryOptions
-    # globalCameraSettings
     # portStatus
     # cameraCapacity
     # deviceFirmwareSettings
 
     @classmethod
     @cache
     def _get_unifi_remaps(cls) -> dict[str, str]:
@@ -1047,14 +1058,54 @@
     def vault_cameras(self) -> list[Camera]:
         """Vault Cameras for NVR"""
 
         if len(self.vault_camera_ids) == 0:
             return []
         return [self.api.bootstrap.cameras[c] for c in self.vault_camera_ids]
 
+    @property
+    def is_global_recording_enabled(self) -> bool:
+        """Is recording footage/events from the camera enabled?
+
+        If recording is not enabled, cameras will not produce any footage, thumbnails,
+        motion/smart detection events.
+        """
+
+        return (
+            self.global_camera_settings is not None
+            and self.global_camera_settings.recording_settings.mode
+            is not RecordingMode.NEVER
+        )
+
+    @property
+    def is_smart_detections_enabled(self) -> bool:
+        """If smart detected enabled globally."""
+
+        return self.smart_detection is not None and self.smart_detection.enable
+
+    @property
+    def is_license_plate_detections_enabled(self) -> bool:
+        """If smart detected enabled globally."""
+
+        return (
+            self.smart_detection is not None
+            and self.smart_detection.enable
+            and self.smart_detection.license_plate_recognition
+        )
+
+    @property
+    def is_face_detections_enabled(self) -> bool:
+        """If smart detected enabled globally."""
+
+        return (
+            self.smart_detection is not None
+            and self.smart_detection.enable
+            and self.smart_detection.face_recognition
+        )
+
     def update_all_messages(self) -> None:
         """Updates doorbell_settings.all_messages after adding/removing custom message"""
 
         messages = self.doorbell_settings.custom_messages
         self.doorbell_settings.all_messages = [
             DoorbellMessage(
                 type=DoorbellMessageType.LEAVE_PACKAGE_AT_DOOR,
@@ -1188,14 +1239,249 @@
                     await cache_file.write(orjson.dumps([str(v) for v in versions]))
                 await aos.rename(tmp, cache_file_path)
             except Exception:
                 _LOGGER.warning("Failed write cache file.")
 
         return self.version not in versions
 
+    async def set_smart_detections(self, value: bool) -> None:
+        """Set if smart detections are enabled."""
+
+        def callback() -> None:
+            if self.smart_detection is not None:
+                self.smart_detection.enable = value
+
+        await self.queue_update(callback)
+
+    async def set_face_recognition(self, value: bool) -> None:
+        """Set if face detections are enabled. Requires smart detections to be enabled."""
+
+        if self.smart_detection is None or not self.smart_detection.enable:
+            raise BadRequest("Smart detections are not enabled.")
+
+        def callback() -> None:
+            if self.smart_detection is not None:
+                self.smart_detection.face_recognition = value
+
+        await self.queue_update(callback)
+
+    async def set_license_plate_recognition(self, value: bool) -> None:
+        """Set if license plate detections are enabled. Requires smart detections to be enabled."""
+
+        if self.smart_detection is None or not self.smart_detection.enable:
+            raise BadRequest("Smart detections are not enabled.")
+
+        def callback() -> None:
+            if self.smart_detection is not None:
+                self.smart_detection.license_plate_recognition = value
+
+        await self.queue_update(callback)
+
+    async def set_global_osd_name(self, enabled: bool) -> None:
+        """Sets whether camera name is in the On Screen Display"""
+
+        def callback() -> None:
+            if self.global_camera_settings:
+                self.global_camera_settings.osd_settings.is_name_enabled = enabled
+
+        await self.queue_update(callback)
+
+    async def set_global_osd_date(self, enabled: bool) -> None:
+        """Sets whether current date is in the On Screen Display"""
+
+        def callback() -> None:
+            if self.global_camera_settings:
+                self.global_camera_settings.osd_settings.is_date_enabled = enabled
+
+        await self.queue_update(callback)
+
+    async def set_global_osd_logo(self, enabled: bool) -> None:
+        """Sets whether the UniFi logo is in the On Screen Display"""
+
+        def callback() -> None:
+            if self.global_camera_settings:
+                self.global_camera_settings.osd_settings.is_logo_enabled = enabled
+
+        await self.queue_update(callback)
+
+    async def set_global_osd_bitrate(self, enabled: bool) -> None:
+        """Sets whether camera bitrate is in the On Screen Display"""
+
+        def callback() -> None:
+            # mismatch between UI internal data structure debug = bitrate data
+            if self.global_camera_settings:
+                self.global_camera_settings.osd_settings.is_debug_enabled = enabled
+
+        await self.queue_update(callback)
+
+    async def set_global_motion_detection(self, enabled: bool) -> None:
+        """Sets motion detection on camera"""
+
+        def callback() -> None:
+            if self.global_camera_settings:
+                self.global_camera_settings.recording_settings.enable_motion_detection = (
+                    enabled
+                )
+
+        await self.queue_update(callback)
+
+    async def set_global_recording_mode(self, mode: RecordingMode) -> None:
+        """Sets recording mode on camera"""
+
+        def callback() -> None:
+            if self.global_camera_settings:
+                self.global_camera_settings.recording_settings.mode = mode
+
+        await self.queue_update(callback)
+
+    # object smart detections
+
+    def _is_smart_enabled(self, smart_type: SmartDetectObjectType) -> bool:
+        return (
+            self.is_global_recording_enabled
+            and self.global_camera_settings is not None
+            and smart_type
+            in self.global_camera_settings.smart_detect_settings.object_types
+        )
+
+    @property
+    def is_global_person_detection_on(self) -> bool:
+        """Is Person Detection available and enabled (camera will produce person smart
+        detection events)?
+        """
+
+        return self._is_smart_enabled(SmartDetectObjectType.PERSON)
+
+    @property
+    def is_global_person_tracking_enabled(self) -> bool:
+        """Is person tracking enabled"""
+        return (
+            self.global_camera_settings is not None
+            and self.global_camera_settings.smart_detect_settings.auto_tracking_object_types
+            is not None
+            and SmartDetectObjectType.PERSON
+            in self.global_camera_settings.smart_detect_settings.auto_tracking_object_types
+        )
+
+    @property
+    def is_global_vehicle_detection_on(self) -> bool:
+        """Is Vehicle Detection available and enabled (camera will produce vehicle smart
+        detection events)?
+        """
+
+        return self._is_smart_enabled(SmartDetectObjectType.VEHICLE)
+
+    @property
+    def is_global_license_plate_detection_on(self) -> bool:
+        """Is License Plate Detection available and enabled (camera will produce face license
+        plate detection events)?
+        """
+
+        return self._is_smart_enabled(SmartDetectObjectType.LICENSE_PLATE)
+
+    @property
+    def is_global_package_detection_on(self) -> bool:
+        """Is Package Detection available and enabled (camera will produce package smart
+        detection events)?
+        """
+
+        return self._is_smart_enabled(SmartDetectObjectType.PACKAGE)
+
+    @property
+    def is_global_animal_detection_on(self) -> bool:
+        """Is Animal Detection available and enabled (camera will produce package smart
+        detection events)?
+        """
+
+        return self._is_smart_enabled(SmartDetectObjectType.ANIMAL)
+
+    def _is_audio_enabled(self, smart_type: SmartDetectObjectType) -> bool:
+        audio_type = smart_type.audio_type
+        return (
+            audio_type is not None
+            and self.is_global_recording_enabled
+            and self.global_camera_settings is not None
+            and self.global_camera_settings.smart_detect_settings.audio_types
+            is not None
+            and audio_type
+            in self.global_camera_settings.smart_detect_settings.audio_types
+        )
+
+    @property
+    def is_global_smoke_detection_on(self) -> bool:
+        """Is Smoke Alarm Detection available and enabled (camera will produce smoke
+        smart detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.SMOKE)
+
+    @property
+    def is_global_co_detection_on(self) -> bool:
+        """Is CO Alarm Detection available and enabled (camera will produce smoke smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.CMONX)
+
+    @property
+    def is_global_siren_detection_on(self) -> bool:
+        """Is Siren Detection available and enabled (camera will produce siren smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.SIREN)
+
+    @property
+    def is_global_baby_cry_detection_on(self) -> bool:
+        """Is Baby Cry Detection available and enabled (camera will produce baby cry smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.BABY_CRY)
+
+    @property
+    def is_global_speaking_detection_on(self) -> bool:
+        """Is Speaking Detection available and enabled (camera will produce speaking smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.SPEAK)
+
+    @property
+    def is_global_bark_detection_on(self) -> bool:
+        """Is Bark Detection available and enabled (camera will produce barking smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.BARK)
+
+    @property
+    def is_global_car_alarm_detection_on(self) -> bool:
+        """Is Car Alarm Detection available and enabled (camera will produce car alarm smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.BURGLAR)
+
+    @property
+    def is_global_car_horn_detection_on(self) -> bool:
+        """Is Car Horn Detection available and enabled (camera will produce car horn smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.CAR_HORN)
+
+    @property
+    def is_global_glass_break_detection_on(self) -> bool:
+        """Is Glass Break available and enabled (camera will produce glass break smart
+        detection events)?
+        """
+
+        return self._is_audio_enabled(SmartDetectObjectType.GLASS_BREAK)
+
 
 class LiveviewSlot(ProtectBaseObject):
     camera_ids: list[str]
     cycle_mode: str
     cycle_interval: int
 
     _cameras: Optional[list[Camera]] = PrivateAttr(None)
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/types.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Coroutine
 import enum
 from typing import Any, Literal, Optional, TypeVar, Union
 
 from packaging.version import Version as BaseVersion
-
-try:
-    from pydantic.v1 import ConstrainedInt
-    from pydantic.v1.color import Color as BaseColor
-    from pydantic.v1.types import ConstrainedFloat, ConstrainedStr
-except ImportError:
-    from pydantic import ConstrainedInt
-    from pydantic.color import Color as BaseColor  # type: ignore[assignment]
-    from pydantic.types import ConstrainedFloat, ConstrainedStr
+from pydantic.v1 import BaseModel, ConstrainedInt
+from pydantic.v1.color import Color as BaseColor
+from pydantic.v1.types import ConstrainedFloat, ConstrainedStr
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 
 DEFAULT = "DEFAULT_VALUE"
 DEFAULT_TYPE = Literal["DEFAULT_VALUE"]
@@ -581,14 +575,45 @@
 
 
 class RepeatTimes(ConstrainedInt):
     ge = 1
     le = 6
 
 
+class PTZPositionDegree(BaseModel):
+    pan: float
+    tilt: float
+    zoom: int
+
+
+class PTZPositionSteps(BaseModel):
+    focus: int
+    pan: int
+    tilt: int
+    zoom: int
+
+
+class PTZPosition(BaseModel):
+    degree: PTZPositionDegree
+    steps: PTZPositionSteps
+
+
+class PTZPresetPosition(BaseModel):
+    pan: int
+    tilt: int
+    zoom: int
+
+
+class PTZPreset(BaseModel):
+    id: str
+    name: str
+    slot: int
+    ptz: PTZPresetPosition
+
+
 CoordType = Union[Percent, int, float]
 
 
 # TODO: fix when upgrading to pydantic v2
 class Color(BaseColor):  # noqa: PLW1641
     def __eq__(self, o: object) -> bool:
         if isinstance(o, Color):
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/user.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import cache
 from typing import Any, Optional
 
-try:
-    from pydantic.v1.fields import PrivateAttr
-except ImportError:
-    from pydantic.fields import PrivateAttr
+from pydantic.v1.fields import PrivateAttr
 
 from pyunifiprotect.data.base import ProtectBaseObject, ProtectModel, ProtectModelWithId
 from pyunifiprotect.data.types import ModelType, PermissionNode
 
 
 class Permission(ProtectBaseObject):
     raw_permission: str
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/data/websocket.py` & `pyunifiprotect-5.2.0/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-5.2.0/pyunifiprotect/test_util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,16 +215,15 @@
     ) -> None:
         def write() -> None:
             if raw is None:
                 self.log(f"No image data, skipping {name}...")
                 return
 
             self.log(f"Writing {name}...")
-            with open(self.output_folder / f"{name}.{ext}", "wb") as f:
-                f.write(raw)
+            Path(self.output_folder / f"{name}.{ext}").write_bytes(raw)
 
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, write)
 
     async def write_image_file(self, name: str, raw: Optional[bytes]) -> None:
         await self.write_binary_file(name, "png", raw)
```

### Comparing `pyunifiprotect-5.1.3/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-5.2.0/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/.gitignore` & `pyunifiprotect-5.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/LICENSE` & `pyunifiprotect-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/README.md` & `pyunifiprotect-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-5.1.3/pyproject.toml` & `pyunifiprotect-5.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "aiohttp",
     "aioshutil",
     "dateparser",
     "orjson",
     "packaging",
     "pillow",
     "platformdirs",
-    "pydantic!=1.9.1",
+    "pydantic>=1.10.15",
     "pyjwt",
     "typer[all]>0.6",
     "yarl>=1.9",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/AngellusMortis/pyunifiprotect/"
@@ -163,16 +163,16 @@
     "PTH",
     "SLF001",
     "TCH",
     "TD",
     "TRY",
 ]
 "pyunifiprotect/api.py" = ["ERA001"]
-"**/test_*.py" = ["FBT", "D", "SLF001", "PLR2004"]
-"tests/**/*.py" = ["FBT", "D", "SLF001", "PLR2004"]
+"**/test_*.py" = ["FBT", "D", "SLF001", "PLR2004", "RUF029"]
+"tests/**/*.py" = ["FBT", "D", "SLF001", "PLR2004", "RUF029"]
 
 [tool.isort]
 profile = "black"
 line_length = 88
 atomic = true
 skip_glob = ["**/migrations/*"]
 add_imports = ["from __future__ import annotations"]
```

### Comparing `pyunifiprotect-5.1.3/PKG-INFO` & `pyunifiprotect-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyunifiprotect
-Version: 5.1.3
+Version: 5.2.0
 Summary: Unofficial UniFi Protect Python API and CLI
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
 Project-URL: Changelog, https://github.com/AngellusMortis/pyunifiprotect/releases/
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
@@ -25,15 +25,15 @@
 Requires-Dist: aioshutil
 Requires-Dist: async-timeout; python_version < '3.11'
 Requires-Dist: dateparser
 Requires-Dist: orjson
 Requires-Dist: packaging
 Requires-Dist: pillow
 Requires-Dist: platformdirs
-Requires-Dist: pydantic!=1.9.1
+Requires-Dist: pydantic>=1.10.15
 Requires-Dist: pyjwt
 Requires-Dist: typer[all]>0.6
 Requires-Dist: yarl>=1.9
 Provides-Extra: backup
 Requires-Dist: aiosqlite; extra == 'backup'
 Requires-Dist: asyncify; extra == 'backup'
 Requires-Dist: av; extra == 'backup'
```

