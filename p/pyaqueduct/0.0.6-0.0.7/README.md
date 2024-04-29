# Comparing `tmp/pyaqueduct-0.0.6.tar.gz` & `tmp/pyaqueduct-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaqueduct-0.0.6.tar", max compression
+gzip compressed data, was "pyaqueduct-0.0.7.tar", max compression
```

## Comparing `pyaqueduct-0.0.6.tar` & `pyaqueduct-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/LICENSE
--rw-r--r--   0        0        0     2331 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/README.md
--rw-r--r--   0        0        0      145 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/__init__.py
--rw-r--r--   0        0        0     2996 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/api.py
--rw-r--r--   0        0        0      292 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/__init__.py
--rw-r--r--   0        0        0    12834 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/client.py
--rw-r--r--   0        0        0     2175 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/client/types.py
--rw-r--r--   0        0        0      929 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/exceptions.py
--rw-r--r--   0        0        0     3283 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/experiment.py
--rw-r--r--   0        0        0        0 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/__init__.py
--rw-r--r--   0        0        0     2463 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/mutations.py
--rw-r--r--   0        0        0     1696 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyaqueduct/schemas/queries.py
--rw-r--r--   0        0        0     1129 2024-04-05 09:36:01.557528 pyaqueduct-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 pyaqueduct-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-29 12:31:10.214111 pyaqueduct-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2331 2024-04-29 12:31:10.214111 pyaqueduct-0.0.7/README.md
+-rw-r--r--   0        0        0      145 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/__init__.py
+-rw-r--r--   0        0        0     3312 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/api.py
+-rw-r--r--   0        0        0      292 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/__init__.py
+-rw-r--r--   0        0        0    16160 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/client.py
+-rw-r--r--   0        0        0     2176 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/types.py
+-rw-r--r--   0        0        0      591 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/exceptions.py
+-rw-r--r--   0        0        0     3493 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/experiment.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/__init__.py
+-rw-r--r--   0        0        0     2463 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/mutations.py
+-rw-r--r--   0        0        0     1696 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/queries.py
+-rw-r--r--   0        0        0      237 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/settings.py
+-rw-r--r--   0        0        0     1144 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3397 1970-01-01 00:00:00.000000 pyaqueduct-0.0.7/PKG-INFO
```

### Comparing `pyaqueduct-0.0.6/LICENSE` & `pyaqueduct-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.6/README.md` & `pyaqueduct-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.6/pyaqueduct/api.py` & `pyaqueduct-0.0.7/pyaqueduct/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 from typing import List
 
 from pydantic import BaseModel, Field, HttpUrl, PositiveFloat, PrivateAttr
 
 from pyaqueduct.client import AqueductClient
 from pyaqueduct.experiment import _MAX_DESCRIPTION_LENGTH, _MAX_TITLE_LENGTH, Experiment
+from pyaqueduct.settings import Settings
 
 
 class API(BaseModel):
     """Aqueduct API interface to interact with experiments.
 
     Args:
         url: URL of the Aqueduct server including the prefix.
-        timeout: timeout of operations in seconds.
+        timeout: Timeout of operations in seconds.
 
     """
 
     url: HttpUrl
     timeout: PositiveFloat
 
     _client: AqueductClient = PrivateAttr()
@@ -27,15 +28,15 @@
     def __init__(self, url: str, timeout: float = 0.5):
         super().__init__(url=url, timeout=timeout)
 
         if not url.endswith("/"):
             url = url + "/"
         api_url = f"{url}api"
 
-        self._client = AqueductClient(url=api_url, timeout=timeout)
+        self._client = AqueductClient(url=api_url, timeout=timeout, api_token=Settings().api_token)
 
     def create_experiment(
         self,
         title: str = Field(..., min_length=1, max_length=_MAX_TITLE_LENGTH),
         description: str = Field("", max_length=_MAX_DESCRIPTION_LENGTH),
     ) -> Experiment:
         """Create an experiment with specific title and description.
@@ -48,52 +49,54 @@
             Experiment object to interact with its data.
 
         """
 
         experiment_data = self._client.create_experiment(title=title, description=description)
         return Experiment(
             client=self._client,
-            id=experiment_data.id,
+            experiment_id=experiment_data.id,
             alias=experiment_data.alias,
             created_at=experiment_data.created_at,
         )
 
     def get_experiment(self, alias: str) -> Experiment:
         """Get the experiment by the specified identifier to operate on.
 
         Args:
-            experiment_id: ID of the specified experiment.
+            alias: Alias of the specified experiment.
 
         Returns:
             Experiment object to interact with the experiment data.
 
         """
         experiment_data = self._client.get_experiment_by_alias(alias=alias)
         return Experiment(
             client=self._client,
-            id=experiment_data.id,
+            experiment_id=experiment_data.id,
             alias=experiment_data.alias,
             created_at=experiment_data.created_at,
         )
 
     def find_experiments(self, search: str, limit: int, offset: int = 0) -> List[Experiment]:
         """Find the experiments that have the search criteria in their title or id.
 
         Args:
-            search: Search string to match.
+            search: The string to search for in the title field of experiments.
+            limit: The maximum number of experiments to fetch in a single request.
+            offset: The number of experiments to skip from the beginning of the search results.
 
         Returns:
             List of experiment objects to operate on their data.
 
         """
         experiments = self._client.get_experiments(
             title=search, limit=limit, offset=offset
         ).experiments
         return [
             Experiment(
                 client=self._client,
-                id=experiment.id,
+                experiment_id=experiment.id,
                 alias=experiment.alias,
                 created_at=experiment.created_at,
             )
             for experiment in experiments
         ]
```

### Comparing `pyaqueduct-0.0.6/pyaqueduct/client/client.py` & `pyaqueduct-0.0.7/pyaqueduct/client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 """Aqueduct client class to enable experiment based operations."""
 
 import logging
 import os
 from datetime import date
-from http import HTTPStatus
-from typing import List, Optional
+from typing import Dict, List, Optional
 from uuid import UUID
 
 from gql import Client
 from gql.client import SyncClientSession
+from gql.transport import exceptions as gql_exceptions
 from gql.transport.httpx import HTTPXTransport
-from httpx import WriteTimeout, post, stream
+from httpx import TransportError, codes, post, stream
 from pydantic import BaseModel, HttpUrl, PrivateAttr
 from tqdm import tqdm
 
 from pyaqueduct.client.types import ExperimentData, ExperimentsInfo, TagsData
 from pyaqueduct.exceptions import (
-    InterruptedDownloadException,
-    InterruptedUploadException,
+    FileDownloadError,
+    FileUploadError,
+    ForbiddenError,
+    RemoteOperationError,
+    UnAuthorizedError,
 )
 from pyaqueduct.schemas.mutations import (
     add_tag_to_experiment_mutation,
     create_experiment_mutation,
     remove_tag_from_experiment_mutation,
     update_experiment_mutation,
 )
 from pyaqueduct.schemas.queries import (
     get_all_tags_query,
     get_experiment_query,
     get_experiments_query,
 )
 
 
-class AqueductClientResponse(BaseModel):
-    """Response of methods of Aqueduct client"""
+def process_response_common(code: codes) -> None:
+    """Process common HTTP return codes."""
+    if code is codes.OK:
+        return
 
-    result: str
-    message: str
+    if code is codes.FORBIDDEN:
+        raise ForbiddenError("Operation is not allowed for the current user.") from None
+
+    if code is codes.UNAUTHORIZED:
+        raise UnAuthorizedError("API token couldn't be verified or is missing.") from None
+
+    raise RemoteOperationError("Remove operation failed.")
 
 
 class AqueductClient(BaseModel):
     """
     AqueductClient - A client class for managing experiments, tags and files.
 
     This class provides methods for creating experiments, updating experiments,
@@ -48,36 +58,31 @@
 
     """
 
     url: HttpUrl
     timeout: float
     _gql_client: Client = PrivateAttr()
     _session: SyncClientSession = PrivateAttr()
+    _headers: Dict[str, str] = PrivateAttr()
 
-    def __init__(self, url: str, timeout: float):
+    def __init__(self, url: str, timeout: float, api_token: Optional[str] = None):
         """
         Args:
             url: URL of the Aqueduct server endpoint.
             timeout: Response timeout in seconds.
 
         """
         super().__init__(url=url, timeout=timeout)
+        self._headers = {"Authorization": f"Bearer {api_token}"} if api_token else {}
 
         self._gql_client = Client(
-            transport=HTTPXTransport(url=f"{url}/graphql", timeout=self.timeout)
+            transport=HTTPXTransport(
+                url=f"{url}/graphql", timeout=self.timeout, headers=self._headers
+            )
         )
-        self.connect()
-
-    def connect(self):
-        """Connect to GraphQL connect"""
-        self._session = self._gql_client.connect_sync()  # type: ignore
-
-    def close(self):
-        """Close connection with GraphQL client"""
-        self._gql_client.close_sync()
 
     def create_experiment(
         self, title: str, description: str, tags: Optional[List[str]] = None
     ) -> ExperimentData:
         """
         Create an experiment with title, description and list of tags
 
@@ -85,28 +90,36 @@
         - title (str): Title of experiment
         - description (str): Description of experiment
         - tags (List[str]): List of tags to be assigned to experiment
 
         Returns:
         Experiment: Experiment objects having all fields
         """
-
-        experiment = self._session.execute(
-            create_experiment_mutation,
-            variable_values={"title": title, "description": description, "tags": tags or []},
-        )
+        try:
+            experiment = self._gql_client.execute(
+                create_experiment_mutation,
+                variable_values={"title": title, "description": description, "tags": tags or []},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
         experiment_obj = ExperimentData.from_dict(
             experiment["createExperiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Created experiment - %s - %s", experiment_obj.id, experiment_obj.title)
         return experiment_obj
 
     def update_experiment(
-        self, experiment_uuid: str, title: Optional[str] = None, description: Optional[str] = None
+        self, experiment_uuid: UUID, title: Optional[str] = None, description: Optional[str] = None
     ) -> ExperimentData:
         """
         Update title or description or both for experiment
 
         Args:
         - experiment_uuid (UUID): UUID of experiment to be updated
         - title (str): New title of experiment
@@ -117,22 +130,32 @@
         """
         if title and title == "":
             raise ValueError("Title cannot be an empty string")
 
         if description and description == "":
             raise ValueError("Description cannot be an empty string")
 
-        experiment = self._session.execute(
-            update_experiment_mutation,
-            variable_values={
-                "experimentId": experiment_uuid,
-                "title": title,
-                "description": description,
-            },
-        )
+        try:
+            experiment = self._gql_client.execute(
+                update_experiment_mutation,
+                variable_values={
+                    "experimentId": str(experiment_uuid),
+                    "title": title,
+                    "description": description,
+                },
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
+
         experiment_obj = ExperimentData.from_dict(
             experiment["updateExperiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Updated experiment - %s", experiment_obj.id)
         return experiment_obj
 
     def get_experiments(
@@ -157,50 +180,69 @@
 
         Returns:
         List[Experiment]: A list of experiments with filters applied
         """
         if limit <= 0:
             raise ValueError("Limit should be a positive number")
 
-        experiments = self._session.execute(
-            get_experiments_query,
-            variable_values={
-                "limit": limit,
-                "offset": offset,
-                "title": title,
-                "start_date": start_date,
-                "end_date": end_date,
-                "tags": tags or [],
-            },
-        )
+        try:
+            experiments = self._gql_client.execute(
+                get_experiments_query,
+                variable_values={
+                    "limit": limit,
+                    "offset": offset,
+                    "title": title,
+                    "start_date": start_date,
+                    "end_date": end_date,
+                    "tags": tags or [],
+                },
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
         experiments_obj = ExperimentsInfo.from_dict(
             experiments["experiments"]  # pylint: disable=unsubscriptable-object
         )
         logging.info(
             "Fetched %s experiments, total %s experiments",
             len(experiments_obj.experiments),
             experiments_obj.total_count,
         )
         return experiments_obj
 
-    def get_experiment(self, experiment_uuid: str) -> ExperimentData:
+    def get_experiment(self, experiment_uuid: UUID) -> ExperimentData:
         """
         Get an Experiment by ID or Alias
 
         Args:
         - id_ (str): "UUID | ALIAS" Unique identifier to be used
         - value (str): Value of unique identifier to use for fetching experiment
 
         Returns:
         Experiment: Experiment object having all fields
         """
-        experiment = self._session.execute(
-            get_experiment_query, variable_values={"type": "UUID", "value": experiment_uuid}
-        )
+        try:
+            experiment = self._gql_client.execute(
+                get_experiment_query,
+                variable_values={"type": "UUID", "value": str(experiment_uuid)},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
         experiment_obj = ExperimentData.from_dict(
             experiment["experiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Fetched experiment - %s", experiment_obj.title)
         return experiment_obj
 
@@ -211,105 +253,157 @@
         Args:
         - id_ (str): "UUID | ALIAS" Unique identifier to be used
         - value (str): Value of unique identifier to use for fetching experiment
 
         Returns:
         Experiment: Experiment object having all fields
         """
-        experiment = self._session.execute(
-            get_experiment_query, variable_values={"type": "ALIAS", "value": alias}
-        )
+        try:
+            experiment = self._gql_client.execute(
+                get_experiment_query, variable_values={"type": "ALIAS", "value": alias}
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
         experiment_obj = ExperimentData.from_dict(
             experiment["experiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Fetched experiment - %s", experiment_obj.title)
         return experiment_obj
 
-    def add_tag_to_experiment(self, experiment_uuid: str, tag: str) -> ExperimentData:
+    def add_tag_to_experiment(self, experiment_uuid: UUID, tag: str) -> ExperimentData:
         """
         Add a tag to an experiment
 
         Args:
         - experiment_uuid (UUID): UUID of experiment to which tag is to be added
         - tag (str): Tag to be added to experiment
 
         Returns:
         Experiment: Experiment having tag added
         """
+        try:
+            experiment = self._gql_client.execute(
+                add_tag_to_experiment_mutation,
+                variable_values={"experimentId": str(experiment_uuid), "tag": tag},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
-        experiment = self._session.execute(
-            add_tag_to_experiment_mutation,
-            variable_values={"experimentId": experiment_uuid, "tag": tag},
-        )
         experiment_obj = ExperimentData.from_dict(
             experiment["addTagToExperiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Added tag %s to experiment <%s>", tag, experiment_obj.title)
         return experiment_obj
 
-    def remove_tag_from_experiment(self, experiment_uuid: str, tag: str) -> ExperimentData:
+    def remove_tag_from_experiment(self, experiment_uuid: UUID, tag: str) -> ExperimentData:
         """
         Remove a tag from an experiment
 
         Args:
         - experiment_uuid (UUID): UUID of experiment frin which tag has to be removed
         - tag (str): Tag to be removed from experiment
 
         Returns:
         Experiment: Experiment having tag removed
         """
-
-        experiment = self._session.execute(
-            remove_tag_from_experiment_mutation,
-            variable_values={"experimentId": experiment_uuid, "tag": tag},
-        )
+        try:
+            experiment = self._gql_client.execute(
+                remove_tag_from_experiment_mutation,
+                variable_values={"experimentId": str(experiment_uuid), "tag": tag},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
 
         experiment_obj = ExperimentData.from_dict(
             experiment["removeTagFromExperiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Removed tag %s from experiment <%s>", tag, experiment_obj.title)
         return experiment_obj
 
-    def upload_file(self, experiment_uuid: UUID, file: str) -> AqueductClientResponse:
+    def get_tags(self, limit: int, offset: int, dangling: bool = True) -> TagsData:
+        """
+        Get a list of existing tags
+
+        Args:
+        - limit (int): Number of tags to be fetched
+        - offset (offset): Number of tags to skip
+        - dangling (bool): If tags not linked to any experiment should be included or not
+
+        Returns:
+        List[str]: A list of all existing tags
+        """
+        if limit <= 0:
+            raise ValueError("Limit cannot be 0")
+
+        try:
+            tags = self._gql_client.execute(
+                get_all_tags_query,
+                variable_values={"limit": limit, "offset": offset, "dangling": dangling},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
+
+        tags_obj = TagsData.from_dict(tags["tags"])  # pylint: disable=unsubscriptable-object
+        logging.info("Fetched %s tags, total %s tags", len(tags_obj.tags), tags_obj.total_count)
+        return tags_obj
+
+    def upload_file(self, experiment_uuid: UUID, file: str) -> None:
         """
         Upload file to a specific experiment.
 
         Args:
             experiment_uuid : The ID of the experiment.
             file_path: The local path to the file to be uploaded.
 
         Returns:
             Operation results object.
 
         """
 
-        headers = {
-            "file_name": os.path.basename(file),
-        }
+        headers = {"file_name": os.path.basename(file), **self._headers}
 
         upload_url = f"{self.url}/files/{str(experiment_uuid)}"
         with open(file, "rb") as files:
             try:
-                resp = post(
+                response = post(
                     upload_url, headers=headers, timeout=self.timeout, files={"file": files}
                 )
-            except InterruptedUploadException as exception:
-                return AqueductClientResponse(result="failed", message=exception.message)
+            except TransportError as error:
+                raise FileUploadError(f"Couldn't upload {file} due to transport error.") from error
+
+        process_response_common(codes(response.status_code))
 
-        if resp.status_code != 200:
-            return AqueductClientResponse(
-                result="failed", message=f"Upload failed {HTTPStatus(resp.status_code).name}"
-            )
         logging.info("Successfully uploaded file {files}")
-        return AqueductClientResponse(result="success", message="File uploaded successfully")
 
-    def download_file(
-        self, experiment_uuid: UUID, file_name: str, destination_dir: str
-    ) -> AqueductClientResponse:
+    def download_file(self, experiment_uuid: UUID, file_name: str, destination_dir: str) -> None:
         """
         Download file from a specific experiment.
 
         Args:
             experiment_uuid: The ID of the experiment.
             file_id: The ID of the file to be downloaded.
             destination: The local path where the downloaded file will be saved.
@@ -319,51 +413,24 @@
 
         """
         download_url: str = f"{self.url}/files/{experiment_uuid}/{file_name}"
         destination = f"{destination_dir}/{file_name}"
 
         try:
             with open(destination, "wb") as download_file:
-                with stream("GET", download_url, timeout=self.timeout) as response:
+                with stream(
+                    "GET", download_url, timeout=self.timeout, headers=self._headers
+                ) as response:
                     total = int(response.headers["Content-Length"])
                     with tqdm(
                         total=total, unit_scale=True, unit_divisor=1024, unit="B"
                     ) as progress:
                         num_bytes_downloaded = response.num_bytes_downloaded
                         for chunk in response.iter_bytes():
                             download_file.write(chunk)
                             progress.update(response.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = response.num_bytes_downloaded
 
-        except InterruptedDownloadException as exception:
-            return AqueductClientResponse(result="failed", message=exception.message)
-
-        except WriteTimeout as exception:
-            return AqueductClientResponse(
-                result="failed", message=f"Timeout error for file download {exception}"
-            )
-
-        return AqueductClientResponse(result="success", message=f"File downloaded to {destination}")
-
-    def get_tags(self, limit: int, offset: int, dangling: bool = True) -> TagsData:
-        """
-        Get a list of existing tags
-
-        Args:
-        - limit (int): Number of tags to be fetched
-        - offset (offset): Number of tags to skip
-        - dangling (bool): If tags not linked to any experiment should be included or not
-
-        Returns:
-        List[str]: A list of all existing tags
-        """
-        if limit <= 0:
-            raise ValueError("Limit cannot be 0")
-
-        tags = self._session.execute(
-            get_all_tags_query,
-            variable_values={"limit": limit, "offset": offset, "dangling": dangling},
-        )
-
-        tags_obj = TagsData.from_dict(tags["tags"])  # pylint: disable=unsubscriptable-object
-        logging.info("Fetched %s tags, total %s tags", len(tags_obj.tags), tags_obj.total_count)
-        return tags_obj
+        except Exception as error:
+            raise FileDownloadError(
+                f"Couldn't download {file_name} due to transport error."
+            ) from error
```

### Comparing `pyaqueduct-0.0.6/pyaqueduct/client/types.py` & `pyaqueduct-0.0.7/pyaqueduct/client/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dataclasses for experiment and it's components"""
+
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import List
 from uuid import UUID
 
 
 @dataclass
```

### Comparing `pyaqueduct-0.0.6/pyaqueduct/experiment.py` & `pyaqueduct-0.0.7/pyaqueduct/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,83 +22,89 @@
 
     return bool(pattern.match(tag))
 
 
 class Experiment(BaseModel):
     """Experiment model."""
 
-    client: AqueductClient
+    _client: AqueductClient
     "Client object reference."
     id: UUID
     "Unique ID of the experiment."
     alias: str
     "Alias of the experiment."
     created_at: datetime
     "Creation datetime of the experiment."
 
+    def __init__(
+        self, experiment_id: UUID, alias: str, created_at: datetime, client: AqueductClient, **data
+    ):
+        super().__init__(id=experiment_id, alias=alias, created_at=created_at, **data)
+        self._client = client
+
     @property
     def title(self) -> str:
         """Get title of experiment."""
-        return self.client.get_experiment(experiment_uuid=str(self.id)).title
+        return self._client.get_experiment(experiment_uuid=self.id).title
 
     @title.setter
     def title(self, value: str = Field(..., max_length=_MAX_TITLE_LENGTH)) -> None:
         """Set title of experiment.
 
         Args:
             value: New title.
 
         """
-        self.client.update_experiment(experiment_uuid=str(self.id), title=value)
+        self._client.update_experiment(experiment_uuid=self.id, title=value)
 
     @property
     def description(self) -> str:
         """Get description of experiment."""
-        return self.client.get_experiment(str(self.id)).description
+        return self._client.get_experiment(self.id).description
 
     @description.setter
     def description(self, value: str = Field(..., max_length=_MAX_DESCRIPTION_LENGTH)) -> None:
         """Set description of experiment.
 
         Args:
             value: New description.
 
         """
-        self.client.update_experiment(experiment_uuid=str(self.id), description=value)
+        self._client.update_experiment(experiment_uuid=self.id, description=value)
 
     @property
     def tags(self) -> List[str]:
         """Gets tags of experiment."""
-        return self.client.get_experiment(str(self.id)).tags
+        return self._client.get_experiment(self.id).tags
 
     def add_tag(self, tag: str = Field(..., max_length=_MAX_TAG_LENGTH)) -> None:
         """Add new tag to experiment."""
         if not is_valid_tag(tag):
             raise ValueError(
                 f"Tag {tag} should only contain alphanumeric characters, underscores or hyphens"
             )
 
-        self.client.add_tag_to_experiment(experiment_uuid=str(self.id), tag=tag)
+        self._client.add_tag_to_experiment(experiment_uuid=self.id, tag=tag)
 
     def remove_tag(self, tag: str = Field(..., max_length=_MAX_TAG_LENGTH)) -> None:
         """Remove tag from experiment."""
-        self.client.remove_tag_from_experiment(experiment_uuid=str(self.id), tag=tag)
+        self._client.remove_tag_from_experiment(experiment_uuid=self.id, tag=tag)
 
     @property
     def files(self) -> List[Tuple[str, datetime]]:
         """Get file names of expriment."""
         return [
-            (item.name, item.modified_at) for item in self.client.get_experiment(str(self.id)).files
+            (item.name, item.modified_at) for item in self._client.get_experiment(self.id).files
         ]
 
     def download_file(self, file_name: str, destination_dir: str) -> None:
         """Download the specified file of experiment."""
-        self.client.download_file(self.id, file_name=file_name, destination_dir=destination_dir)
+        self._client.download_file(self.id, file_name=file_name, destination_dir=destination_dir)
 
     def upload_file(self, file: str) -> None:
         """Upload the specified file to experiment."""
-        self.client.upload_file(self.id, file=file)
+        self._client.upload_file(self.id, file=file)
 
     @property
     def updated_at(self) -> datetime:
         """Get last updated datetime of the experiment."""
-        return self.client.get_experiment(str(self.id)).updated_at
+        return self._client.get_experiment(self.id).updated_at
```

### Comparing `pyaqueduct-0.0.6/pyaqueduct/schemas/mutations.py` & `pyaqueduct-0.0.7/pyaqueduct/schemas/mutations.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.6/pyaqueduct/schemas/queries.py` & `pyaqueduct-0.0.7/pyaqueduct/schemas/queries.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.6/pyproject.toml` & `pyaqueduct-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "pyaqueduct"
-version = "0.0.6"
+version = "0.0.7"
 description = "Aqueduct Python Client Library"
 authors = ["Aqueduct Team <aqueduct@riverlane.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aqueducthub.github.io/pyaqueduct"
 documentation = "https://aqueducthub.github.io/pyaqueduct"
 repository = "https://github.com/AqueductHub/pyaqueduct"
 
 [tool.poetry.dependencies]
 python = ">= 3.8,< 3.12"
 requests = "^2.31"
 tqdm = "^4.66"
 httpx = ">=0.15,<0.25"
 types-tqdm = "^4.66"
-pydantic = ">=1.10.13,<3.0.0"
+pydantic = "^2.0"
 gql = {extras = ["httpx"], version = "^3.5"}
+pydantic-settings = "^2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 pylint = "^2.17"
 yapf = "^0.40"
 mypy = "^1.5"
```

### Comparing `pyaqueduct-0.0.6/PKG-INFO` & `pyaqueduct-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pyaqueduct
-Version: 0.0.6
+Version: 0.0.7
 Summary: Aqueduct Python Client Library
 Home-page: https://aqueducthub.github.io/pyaqueduct
 License: MIT
 Author: Aqueduct Team
 Author-email: aqueduct@riverlane.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gql[httpx] (>=3.5,<4.0)
 Requires-Dist: httpx (>=0.15,<0.25)
-Requires-Dist: pydantic (>=1.10.13,<3.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-settings (>=2.2,<3.0)
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Requires-Dist: types-tqdm (>=4.66,<5.0)
 Project-URL: Documentation, https://aqueducthub.github.io/pyaqueduct
 Project-URL: Issues, https://github.com/AqueductHub/pyaqueduct/issues
 Project-URL: Repository, https://github.com/AqueductHub/pyaqueduct
 Description-Content-Type: text/markdown
```

