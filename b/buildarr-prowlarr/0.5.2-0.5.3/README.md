# Comparing `tmp/buildarr_prowlarr-0.5.2.tar.gz` & `tmp/buildarr_prowlarr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_prowlarr-0.5.2.tar", max compression
+gzip compressed data, was "buildarr_prowlarr-0.5.3.tar", max compression
```

## Comparing `buildarr_prowlarr-0.5.2.tar` & `buildarr_prowlarr-0.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/LICENSE
--rw-r--r--   0        0        0    11891 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/README.md
--rw-r--r--   0        0        0      975 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/__init__.py
--rw-r--r--   0        0        0     7086 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/api.py
--rw-r--r--   0        0        0     2881 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/cli.py
--rw-r--r--   0        0        0     5660 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/__init__.py
--rw-r--r--   0        0        0    27143 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/applications.py
--rw-r--r--   0        0        0     8813 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/sync_profiles.py
--rw-r--r--   0        0        0    10899 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/__init__.py
--rw-r--r--   0        0        0     8509 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/base.py
--rw-r--r--   0        0        0    32324 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/torrent.py
--rw-r--r--   0        0        0    14395 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/usenet.py
--rw-r--r--   0        0        0    19716 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/general.py
--rw-r--r--   0        0        0     2318 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/__init__.py
--rw-r--r--   0        0        0    31264 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/indexers.py
--rw-r--r--   0        0        0    16453 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/proxies.py
--rw-r--r--   0        0        0    43595 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/notifications.py
--rw-r--r--   0        0        0     2931 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/tags.py
--rw-r--r--   0        0        0     7227 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/ui.py
--rw-r--r--   0        0        0     1034 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/types.py
--rw-r--r--   0        0        0     1396 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/exceptions.py
--rw-r--r--   0        0        0      950 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/manager.py
--rw-r--r--   0        0        0     1189 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/plugin.py
--rw-r--r--   0        0        0        0 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/py.typed
--rw-r--r--   0        0        0     5970 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/secrets.py
--rw-r--r--   0        0        0      997 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/types.py
--rw-r--r--   0        0        0     1465 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/util.py
--rw-r--r--   0        0        0     2595 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    13569 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/LICENSE
+-rw-r--r--   0        0        0    11891 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/README.md
+-rw-r--r--   0        0        0      975 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/__init__.py
+-rw-r--r--   0        0        0     7086 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/api.py
+-rw-r--r--   0        0        0     2881 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/cli.py
+-rw-r--r--   0        0        0     5660 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/__init__.py
+-rw-r--r--   0        0        0    29162 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/applications.py
+-rw-r--r--   0        0        0     8813 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/sync_profiles.py
+-rw-r--r--   0        0        0    10899 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/__init__.py
+-rw-r--r--   0        0        0     8527 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/base.py
+-rw-r--r--   0        0        0    32324 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/torrent.py
+-rw-r--r--   0        0        0    14395 2024-04-28 23:32:40.009316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/usenet.py
+-rw-r--r--   0        0        0    19716 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/general.py
+-rw-r--r--   0        0        0     2318 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/__init__.py
+-rw-r--r--   0        0        0    31264 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/indexers.py
+-rw-r--r--   0        0        0    16471 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/proxies.py
+-rw-r--r--   0        0        0    45820 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/notifications.py
+-rw-r--r--   0        0        0     2931 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/tags.py
+-rw-r--r--   0        0        0     7227 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/ui.py
+-rw-r--r--   0        0        0     1034 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/types.py
+-rw-r--r--   0        0        0     1396 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/exceptions.py
+-rw-r--r--   0        0        0      950 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/manager.py
+-rw-r--r--   0        0        0     1189 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/py.typed
+-rw-r--r--   0        0        0     5970 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/secrets.py
+-rw-r--r--   0        0        0      997 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/types.py
+-rw-r--r--   0        0        0     1465 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/buildarr_prowlarr/util.py
+-rw-r--r--   0        0        0     2611 2024-04-28 23:32:40.013316 buildarr_prowlarr-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    13594 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.5.3/PKG-INFO
```

### Comparing `buildarr_prowlarr-0.5.2/LICENSE` & `buildarr_prowlarr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/README.md` & `buildarr_prowlarr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/api.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/api.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/cli.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/applications.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/applications.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from typing import Any, Dict, Iterable, List, Literal, Mapping, Optional, Set, Union, cast
 
 import prowlarr
 
 from buildarr.config import RemoteMapEntry
 from buildarr.state import state
 from buildarr.types import BaseEnum, InstanceName, LowerCaseNonEmptyStr, NonEmptyStr, Password
+from packaging.version import Version
 from pydantic import AnyHttpUrl, Field, SecretStr, validator
 from typing_extensions import Annotated, Self
 
 from ....api import prowlarr_api_client
 from ....secrets import ProwlarrSecrets
 from ...types import ProwlarrConfigBase
 
@@ -98,14 +99,15 @@
 
     _implementation: str
     _remote_map: List[RemoteMapEntry] = []
 
     @classmethod
     def _get_base_remote_map(
         cls,
+        secrets: ProwlarrSecrets,
         api_schema: prowlarr.ApplicationResource,
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
         return [
             ("prowlarr_url", "prowlarrUrl", {"is_field": True}),
             ("base_url", "baseUrl", {"is_field": True}),
             ("sync_level", "syncLevel", {}),
@@ -127,14 +129,23 @@
                     ),
                     "encoder": lambda v: sorted(tag_ids[tag] for tag in v),
                 },
             ),
         ]
 
     @classmethod
+    def _get_remote_map(
+        cls,
+        secrets: ProwlarrSecrets,
+        api_schema: prowlarr.ApplicationResource,
+        tag_ids: Mapping[str, int],
+    ) -> List[RemoteMapEntry]:
+        return cls._remote_map
+
+    @classmethod
     def _get_sync_category_options(
         cls,
         api_schema: prowlarr.ApplicationResource,
     ) -> Dict[int, str]:
         return {
             select_option.value: select_option.name.lower()
             for select_option in cast(
@@ -166,21 +177,25 @@
     ) -> List[int]:
         category_ids = {v: k for k, v in cls._get_sync_category_options(api_schema).items()}
         return sorted(category_ids[category_name] for category_name in sync_categories)
 
     @classmethod
     def _from_remote(
         cls,
+        secrets: ProwlarrSecrets,
         api_schema: prowlarr.ApplicationResource,
         tag_ids: Mapping[str, int],
         remote_attrs: Mapping[str, Any],
     ) -> Self:
         return cls(
             **cls.get_local_attrs(
-                remote_map=cls._get_base_remote_map(api_schema, tag_ids) + cls._remote_map,
+                remote_map=(
+                    cls._get_base_remote_map(secrets, api_schema, tag_ids)
+                    + cls._get_remote_map(secrets, api_schema, tag_ids)
+                ),
                 remote_attrs=remote_attrs,
             ),
         )
 
     def _resolve(self) -> Self:
         return self
 
@@ -191,15 +206,18 @@
         api_schema: prowlarr.ApplicationResource,
         tag_ids: Mapping[str, int],
         application_name: str,
     ) -> None:
         api_schema_dict = api_schema.to_dict()
         set_attrs = self.get_create_remote_attrs(
             tree=tree,
-            remote_map=self._get_base_remote_map(api_schema, tag_ids) + self._remote_map,
+            remote_map=(
+                self._get_base_remote_map(secrets, api_schema, tag_ids)
+                + self._get_remote_map(secrets, api_schema, tag_ids)
+            ),
         )
         field_values: Dict[str, Any] = {
             field["name"]: field["value"] for field in set_attrs["fields"]
         }
         set_attrs["fields"] = [
             ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
             for f in api_schema_dict["fields"]
@@ -218,24 +236,28 @@
         api_schema: prowlarr.ApplicationResource,
         tag_ids: Mapping[str, int],
         api_application: prowlarr.ApplicationResource,
     ) -> bool:
         changed, set_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
-            remote_map=self._get_base_remote_map(api_schema, tag_ids) + self._remote_map,
+            remote_map=(
+                self._get_base_remote_map(secrets, api_schema, tag_ids)
+                + self._get_remote_map(secrets, api_schema, tag_ids)
+            ),
             set_unchanged=True,
         )
         if changed:
             if "fields" in set_attrs:
                 field_values: Dict[str, Any] = {
                     field["name"]: field["value"] for field in set_attrs["fields"]
                 }
                 set_attrs["fields"] = [
-                    {**f, "value": field_values[f["name"]]} for f in api_schema.to_dict()["fields"]
+                    ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
+                    for f in api_application.to_dict()["fields"]
                 ]
             remote_attrs = {**api_application.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
                 prowlarr.ApplicationApi(api_client).update_applications(
                     id=str(api_application.id),
                     application_resource=prowlarr.ApplicationResource.from_dict(remote_attrs),
                 )
@@ -243,14 +265,53 @@
         return False
 
     def _delete_remote(self, secrets: ProwlarrSecrets, application_id: int) -> None:
         with prowlarr_api_client(secrets=secrets) as api_client:
             prowlarr.ApplicationApi(api_client).delete_applications(id=application_id)
 
 
+class ArrApplication(Application):
+    sync_reject_blocklisted_torrent_hashes: bool = False
+    """
+    Enable syncing the "Reject Blocklisted Torrent Hashes While Grabbing"
+    indexer option to the target application.
+
+    If a torrent is blocked by hash it may not properly be rejected during RSS/Search
+    for some indexers, enabling this will allow it to be rejected after the torrent is grabbed,
+    but before it is sent to the client.
+
+    Available in Prowlarr v1.15 and above.
+
+    *New in version 0.5.3.*
+    """
+
+    @classmethod
+    def _get_base_remote_map(
+        cls,
+        secrets: ProwlarrSecrets,
+        api_schema: prowlarr.ApplicationResource,
+        tag_ids: Mapping[str, int],
+    ) -> List[RemoteMapEntry]:
+        remote_map = super()._get_base_remote_map(
+            secrets=secrets,
+            api_schema=api_schema,
+            tag_ids=tag_ids,
+        )
+        # https://github.com/Prowlarr/Prowlarr/releases/tag/v1.15.0.4361
+        if Version(secrets.version) >= Version("1.15.0.4361"):
+            remote_map.append(
+                (
+                    "sync_reject_blocklisted_torrent_hashes",
+                    "syncRejectBlocklistedTorrentHashesWhileGrabbing",
+                    {"is_field": True},
+                ),
+            )
+        return remote_map
+
+
 class LazylibrarianApplication(Application):
     """
     Add a [LazyLibrarian](https://lazylibrarian.gitlab.io) instance to sync with Prowlarr.
     """
 
     type: Literal["lazylibrarian", "lazylibrary"] = "lazylibrarian"
     """
@@ -274,15 +335,15 @@
     Default sync category values for this application type.
     """
 
     _implementation: str = "LazyLibrarian"
     _remote_map: List[RemoteMapEntry] = [("api_key", "apiKey", {"is_field": True})]
 
 
-class LidarrApplication(Application):
+class LidarrApplication(ArrApplication):
     """
     Add a [Lidarr](https://lidarr.audio) instance to sync with Prowlarr.
     """
 
     type: Literal["lidarr"] = "lidarr"
     """
     Type value associated with this kind of application.
@@ -328,15 +389,15 @@
     Default sync category values for this application type.
     """
 
     _implementation: str = "Mylar"
     _remote_map: List[RemoteMapEntry] = [("api_key", "apiKey", {"is_field": True})]
 
 
-class RadarrApplication(Application):
+class RadarrApplication(ArrApplication):
     """
     Add a [Radarr](https://radarr.video) instance to sync with Prowlarr.
 
     !!! note
 
         There is a [Radarr plugin for Buildarr](https://buildarr.github.io/plugins/radarr)
         that can be used to link Radarr instances with Prowlarr using the `instance_name`
@@ -396,15 +457,15 @@
             resolved.api_key = state.instance_secrets["radarr"][  # type: ignore[attr-defined]
                 self.instance_name
             ].api_key.get_secret_value()
             return resolved
         return self
 
 
-class ReadarrApplication(Application):
+class ReadarrApplication(ArrApplication):
     """
     Add a [Readarr](https://readarr.com) instance to sync with Prowlarr.
     """
 
     type: Literal["readarr"] = "readarr"
     """
     Type value associated with this kind of application.
@@ -428,15 +489,15 @@
     Default sync category values for this application type.
     """
 
     _implementation: str = "Readarr"
     _remote_map: List[RemoteMapEntry] = [("api_key", "apiKey", {"is_field": True})]
 
 
-class SonarrApplication(Application):
+class SonarrApplication(ArrApplication):
     """
     Add a [Sonarr](https://sonarr.tv) instance to sync with Prowlarr.
 
     !!! note
 
         There is a [Sonarr plugin for Buildarr](https://buildarr.github.io/plugins/sonarr)
         that can be used to link Sonarr instances with Prowlarr using the `instance_name`
@@ -497,21 +558,21 @@
         values: Dict[str, Any],
     ) -> Optional[SecretStr]:
         if not values.get("instance_name", None) and not value:
             raise ValueError("required when 'instance_name' is not defined")
         return value
 
     @classmethod
-    def _get_base_remote_map(
+    def _get_remote_map(
         cls,
+        secrets: ProwlarrSecrets,
         api_schema: prowlarr.ApplicationResource,
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
         return [
-            *super()._get_base_remote_map(api_schema, tag_ids),
             ("api_key", "apiKey", {"is_field": True}),
             (
                 "anime_sync_categories",
                 "animeSyncCategories",
                 {
                     "is_field": True,
                     "decoder": lambda v: cls._sync_categories_decoder(api_schema, v),
@@ -531,15 +592,15 @@
             resolved.api_key = state.instance_secrets["sonarr"][  # type: ignore[attr-defined]
                 self.instance_name
             ].api_key.get_secret_value()
             return resolved
         return self
 
 
-class WhisparrApplication(Application):
+class WhisparrApplication(ArrApplication):
     """
     Add a [Whisparr](https://github.com/Whisparr/Whisparr) instance to sync with Prowlarr.
     """
 
     type: Literal["whisparr"] = "whisparr"
     """
     Type value associated with this kind of application.
@@ -691,14 +752,15 @@
                 else {}
             )
         return cls(
             definitions={
                 api_application.name: APPLICATION_TYPE_MAP[  # type: ignore[attr-defined]
                     api_application.implementation
                 ]._from_remote(
+                    secrets=secrets,
                     api_schema=api_application_schemas[api_application.implementation],
                     tag_ids=tag_ids,
                     remote_attrs=api_application.to_dict(),
                 )
                 for api_application in api_applications
             },
         )
```

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/sync_profiles.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/apps/sync_profiles.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/base.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,16 +216,16 @@
         )
         if changed:
             if "fields" in set_attrs:
                 field_values: Dict[str, Any] = {
                     field["name"]: field["value"] for field in set_attrs["fields"]
                 }
                 set_attrs["fields"] = [
-                    {**f, "value": field_values[f["name"]]}
-                    for f in self._get_api_schema(api_downloadclient_schemas)["fields"]
+                    ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
+                    for f in api_downloadclient.to_dict()["fields"]
                 ]
             remote_attrs = {**api_downloadclient.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
                 prowlarr.DownloadClientApi(api_client).update_download_client(
                     id=str(api_downloadclient.id),
                     download_client_resource=prowlarr.DownloadClientResource.from_dict(
                         remote_attrs,
```

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/torrent.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/torrent.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/usenet.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/download_clients/usenet.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/general.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/general.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/__init__.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/indexers.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/indexers.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/proxies.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/indexers/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,16 @@
         )
         if changed:
             if "fields" in set_attrs:
                 field_values: Dict[str, Any] = {
                     field["name"]: field["value"] for field in set_attrs["fields"]
                 }
                 set_attrs["fields"] = [
-                    {**f, "value": field_values[f["name"]]}
-                    for f in self._get_api_schema(api_proxy_schemas)["fields"]
+                    ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
+                    for f in api_proxy.to_dict()["fields"]
                 ]
             remote_attrs = {**api_proxy.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
                 prowlarr.IndexerProxyApi(api_client).update_indexer_proxy(
                     id=str(api_proxy.id),
                     indexer_proxy_resource=prowlarr.IndexerProxyResource.from_dict(remote_attrs),
                 )
```

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/notifications.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Union
 
 import prowlarr
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
-from pydantic import AnyHttpUrl, ConstrainedInt, Field, NameEmail, SecretStr
+from packaging.version import Version
+from pydantic import AnyHttpUrl, ConstrainedInt, Field, NameEmail, SecretStr, validator
 from typing_extensions import Annotated, Self
 
 from ...api import prowlarr_api_client
 from ...secrets import ProwlarrSecrets
 from ..types import ProwlarrConfigBase
 
 logger = getLogger(__name__)
@@ -69,14 +70,20 @@
     subtitles = 8
     links = 9
     release = 10
     poster = 11
     fanart = 12
 
 
+class EmailUseEncryption(BaseEnum):
+    always = 0
+    preferred = 1
+    never = 2
+
+
 class GotifyPriority(BaseEnum):
     """
     Gotify notification priority.
     """
 
     min = 0
     low = 2
@@ -233,14 +240,15 @@
 
     _implementation: str
     _remote_map: List[RemoteMapEntry]
 
     @classmethod
     def _get_base_remote_map(
         cls,
+        secrets: ProwlarrSecrets,
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
         return [
             (
                 "tags",
                 "tags",
                 {
@@ -249,24 +257,40 @@
                     ),
                     "encoder": lambda v: sorted(tag_ids[tag] for tag in v),
                 },
             ),
         ]
 
     @classmethod
-    def _from_remote(cls, tag_ids: Mapping[str, int], remote_attrs: Mapping[str, Any]) -> Self:
+    def _get_remote_map(
+        cls,
+        secrets: ProwlarrSecrets,
+        tag_ids: Mapping[str, int],
+    ) -> List[RemoteMapEntry]:
+        return cls._remote_map
+
+    @classmethod
+    def _from_remote(
+        cls,
+        secrets: ProwlarrSecrets,
+        tag_ids: Mapping[str, int],
+        remote_attrs: Mapping[str, Any],
+    ) -> Self:
         return cls(
             notification_triggers=NotificationTriggers(
                 **NotificationTriggers.get_local_attrs(
                     remote_map=NotificationTriggers._remote_map,
                     remote_attrs=remote_attrs,
                 ),
             ),
             **cls.get_local_attrs(
-                remote_map=cls._get_base_remote_map(tag_ids) + cls._remote_map,
+                remote_map=(
+                    cls._get_base_remote_map(secrets=secrets, tag_ids=tag_ids)
+                    + cls._get_remote_map(secrets=secrets, tag_ids=tag_ids)
+                ),
                 remote_attrs=remote_attrs,
             ),
         )
 
     def _get_api_schema(self, schemas: List[prowlarr.NotificationResource]) -> Dict[str, Any]:
         return {
             k: v
@@ -290,15 +314,18 @@
         set_attrs = {
             **self.notification_triggers.get_create_remote_attrs(
                 tree=f"{tree}.notification_triggers",
                 remote_map=self.notification_triggers._remote_map,
             ),
             **self.get_create_remote_attrs(
                 tree=tree,
-                remote_map=self._get_base_remote_map(tag_ids) + self._remote_map,
+                remote_map=(
+                    self._get_base_remote_map(secrets=secrets, tag_ids=tag_ids)
+                    + self._get_remote_map(secrets=secrets, tag_ids=tag_ids)
+                ),
             ),
         }
         field_values: Dict[str, Any] = {
             field["name"]: field["value"] for field in set_attrs["fields"]
         }
         set_attrs["fields"] = [
             ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
@@ -326,15 +353,18 @@
             tree=tree,
             remote=remote.notification_triggers,
             remote_map=self.notification_triggers._remote_map,
         )
         base_updated, updated_base_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
-            remote_map=self._get_base_remote_map(tag_ids) + self._remote_map,
+            remote_map=(
+                self._get_base_remote_map(secrets=secrets, tag_ids=tag_ids)
+                + self._get_remote_map(secrets=secrets, tag_ids=tag_ids)
+            ),
         )
         if triggers_updated or base_updated:
             api_schema = self._get_api_schema(api_notification_schemas)
             api_notification_dict = api_notification.to_dict()
             updated_attrs = {**updated_triggers_attrs, **updated_base_attrs}
             if "fields" in updated_attrs:
                 updated_field_values: Dict[str, Any] = {
@@ -674,22 +704,36 @@
     port: Port = 587  # type: ignore[assignment]
     """
     The port number on the SMTP server to use to submit mail.
 
     The default is to use STARTTLS on the standard SMTP submission port.
     """
 
-    use_encryption: bool = True
+    use_encryption: EmailUseEncryption = EmailUseEncryption.always
     """
     Whether or not to use encryption when sending mail to the SMTP server.
 
     If the port number is set to 465, SMTPS (implicit TLS) will be used.
     Any other port number will result in STARTTLS being used.
 
-    The default is to enable encryption.
+    The default is to enforce encryption.
+
+    !!! note
+
+        Disabling encryption is available in Prowlarr v1.13 and above.
+        If this option is set to `never` on an older version, it will have the same
+        effect as setting it to `preferred`.
+
+    Values:
+
+    * `always`/`true` - Enforce encryption
+    * `preferred` - Prefer encryption, but allow unencrypted
+    * `never`/`false` - Disable encryption
+
+    *Changed in version 0.5.3*: Added support for the `always`, `preferred` and `never` values.
     """
 
     username: NonEmptyStr
     """
     SMTP username of the account to send the mail from.
     """
 
@@ -720,25 +764,53 @@
 
     bcc_addresses: Annotated[List[NameEmail], Field(unique_items=True)] = []
     """
     Optional list of email addresses to blind copy (BCC) the mail to.
     """
 
     _implementation: str = "Email"
-    _remote_map: List[RemoteMapEntry] = [
-        ("server", "server", {"is_field": True}),
-        ("port", "port", {"is_field": True}),
-        ("use_encryption", "requireEncryption", {"is_field": True}),
-        ("username", "username", {"is_field": True}),
-        ("password", "password", {"is_field": True}),
-        ("from_address", "from", {"is_field": True}),
-        ("recipient_addresses", "to", {"is_field": True}),
-        ("cc_addresses", "cc", {"is_field": True}),
-        ("bcc_addresses", "bcc", {"is_field": True}),
-    ]
+
+    @validator("use_encryption", pre=True)
+    def validate_use_encryption(cls, value: Union[bool, str]) -> Union[str, EmailUseEncryption]:
+        if value is True:
+            return EmailUseEncryption.always
+        if value is False:
+            return EmailUseEncryption.never
+        return value
+
+    @classmethod
+    def _get_remote_map(
+        cls,
+        secrets: ProwlarrSecrets,
+        tag_ids: Mapping[str, int],
+    ) -> List[RemoteMapEntry]:
+        return [
+            ("server", "server", {"is_field": True}),
+            ("port", "port", {"is_field": True}),
+            (
+                # https://github.com/Prowlarr/Prowlarr/releases/tag/v1.13.1.4243
+                ("use_encryption", "useEncryption", {"is_field": True})
+                if Version(secrets.version) >= Version("1.13.1.4243")
+                else (
+                    "use_encryption",
+                    "requireEncryption",
+                    {
+                        "is_field": True,
+                        "decoder": lambda v: 0 if v else 1,
+                        "encoder": lambda v: v == EmailUseEncryption.always,
+                    },
+                )
+            ),
+            ("username", "username", {"is_field": True}),
+            ("password", "password", {"is_field": True}),
+            ("from_address", "from", {"is_field": True}),
+            ("recipient_addresses", "to", {"is_field": True}),
+            ("cc_addresses", "cc", {"is_field": True}),
+            ("bcc_addresses", "bcc", {"is_field": True}),
+        ]
 
 
 class GotifyNotification(Notification):
     """
     Send media update and health alert push notifications via a Gotify server.
     """
 
@@ -1082,20 +1154,20 @@
     """
 
     type: Literal["pushover"] = "pushover"
     """
     Type value associated with this kind of connection.
     """
 
-    user_key: Annotated[SecretStr, Field(min_length=30, max_length=30)]
+    user_key: Password
     """
     User key to use to authenticate with your Pushover account.
     """
 
-    api_key: Annotated[SecretStr, Field(min_length=30, max_length=30)]
+    api_key: Password
     """
     API key assigned to Prowlarr in Pushover.
     """
 
     devices: Set[NonEmptyStr] = set()
     """
     List of device names to send notifications to.
@@ -1455,14 +1527,15 @@
                 else {}
             )
         return cls(
             definitions={
                 api_notification.name: NOTIFICATION_TYPE_MAP[  # type: ignore[attr-defined]
                     api_notification.implementation.lower()
                 ]._from_remote(
+                    secrets=secrets,
                     tag_ids=tag_ids,
                     remote_attrs=api_notification.to_dict(),
                 )
                 for api_notification in api_notifications
             },
         )
```

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/tags.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/tags.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/ui.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/settings/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/types.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/exceptions.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/manager.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/plugin.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/secrets.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/types.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/buildarr_prowlarr/util.py` & `buildarr_prowlarr-0.5.3/buildarr_prowlarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.2/pyproject.toml` & `buildarr_prowlarr-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-prowlarr"
-version = "0.5.2"
+version = "0.5.3"
 description = "Prowlarr indexer manager plugin for Buildarr"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr-prowlarr"
 documentation = "https://buildarr.github.io/plugins/prowlarr"
 keywords = [
@@ -44,14 +44,15 @@
 [tool.poetry.plugins."buildarr.plugins"]
 "prowlarr" = "buildarr_prowlarr.plugin:ProwlarrPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 prowlarr-py = ">=0.4.1,<0.5.0"
 json5 = ">=0.9.7"
+packaging = "*"
 buildarr = ">=0.7.0,<0.8.0"
 buildarr-sonarr = {version = ">=0.6.0", optional = true}
 buildarr-radarr = {version = ">=0.2.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "23.11.0"
 mypy = "1.7.0"
```

### Comparing `buildarr_prowlarr-0.5.2/PKG-INFO` & `buildarr_prowlarr-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-prowlarr
-Version: 0.5.2
+Version: 0.5.3
 Summary: Prowlarr indexer manager plugin for Buildarr
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,prowlarr,lazylibrarian,lidarr,mylar,radarr,readarr,sonarr,whisparr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -24,14 +24,15 @@
 Classifier: Typing :: Typed
 Provides-Extra: radarr
 Provides-Extra: sonarr
 Requires-Dist: buildarr (>=0.7.0,<0.8.0)
 Requires-Dist: buildarr-radarr (>=0.2.0) ; extra == "radarr"
 Requires-Dist: buildarr-sonarr (>=0.6.0) ; extra == "sonarr"
 Requires-Dist: json5 (>=0.9.7)
+Requires-Dist: packaging
 Requires-Dist: prowlarr-py (>=0.4.1,<0.5.0)
 Project-URL: Changes, https://buildarr.github.io/plugins/prowlarr/release-notes
 Project-URL: Documentation, https://buildarr.github.io/plugins/prowlarr
 Project-URL: Issue Tracker, https://github.com/buildarr/buildarr-prowlarr/issues
 Project-URL: Repository, https://github.com/buildarr/buildarr-prowlarr
 Description-Content-Type: text/markdown
```

