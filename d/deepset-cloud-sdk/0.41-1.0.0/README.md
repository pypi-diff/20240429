# Comparing `tmp/deepset_cloud_sdk-0.41.tar.gz` & `tmp/deepset_cloud_sdk-1.0.0.tar.gz`

## Comparing `deepset_cloud_sdk-0.41.tar` & `deepset_cloud_sdk-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/CONTRIBUTING.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/mkdocs.yml
--rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/assets/cli.gif
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/assets/logo.png
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/config.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/deepset_cloud_api.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/files.py
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/upload_sessions.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_s3/__init__.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_s3/upload.py
--rw-r--r--   0        0        0    28822 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_utils/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_utils/datetime.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/utils.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/index.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/upload_files.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_images/favicon.svg
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_images/white-logo.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/renderers.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/requirements.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/async_client.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/cli.yml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/sync_client.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_stylesheets/extra.css
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/sdk/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/sdk/upload.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example.txt.meta.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example2.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example2.txt.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/.gitignore
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/LICENSE
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/README.md
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/pyproject.toml
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/PKG-INFO
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/assets/cli.gif
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/assets/logo.png
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/config.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/deepset_cloud_api.py
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/files.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/upload_sessions.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/__init__.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/upload.py
+-rw-r--r--   0        0        0    31216 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_utils/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_utils/datetime.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/utils.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/index.md
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/upload_files.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_images/favicon.svg
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_images/white-logo.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/renderers.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/requirements.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/async_client.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/cli.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_pydoc/config/sync_client.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/_stylesheets/extra.css
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/sdk/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/docs/examples/sdk/upload.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example.txt.meta.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example2.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/test-upload/example2.txt.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/.gitignore
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deepset_cloud_sdk-1.0.0/PKG-INFO
```

### Comparing `deepset_cloud_sdk-0.41/.pre-commit-config.yaml` & `deepset_cloud_sdk-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/CONTRIBUTING.md` & `deepset_cloud_sdk-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/mkdocs.yml` & `deepset_cloud_sdk-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/assets/cli.gif` & `deepset_cloud_sdk-1.0.0/assets/cli.gif`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/assets/logo.png` & `deepset_cloud_sdk-1.0.0/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - Client layer
 - Service layer
 - Workflow layer
 
 
 ### API layer
 This layer is the lowest level of abstraction and contains the API definition, including all HTTP methods. It takes care of the authentication.
-You can find this layer in the `deepset_cloud_sdk/api/deepset_cloud_api.py` file. We should implement reties on this lowest layer.
+You can find this layer in the `deepset_cloud_sdk/_api/deepset_cloud_api.py` file. We should implement reties on this lowest layer.
 
 ### Client layer
 This layer adds a thin wrapper around the API layer and provides a more convenient interface to the API. It includes explicit methods
 for endpoints by specifying the HTTP methods and endpoints for example for uploading files.
 
 ### Service layer
 This layer takes care of combining client methods to provide more complex functionality. Within this layer, we can add functionalities like
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/cli.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,79 @@
 """The CLI for the deepset Cloud SDK."""
+
 import json
 import os
+from pathlib import Path
 from typing import List, Optional
 from uuid import UUID
 
 import typer
 from tabulate import tabulate
 
 from deepset_cloud_sdk.__about__ import __version__
 from deepset_cloud_sdk._api.config import DEFAULT_WORKSPACE_NAME, ENV_FILE_PATH
+from deepset_cloud_sdk._api.upload_sessions import WriteMode
 from deepset_cloud_sdk.workflows.sync_client.files import download as sync_download
 from deepset_cloud_sdk.workflows.sync_client.files import (
     get_upload_session as sync_get_upload_session,
 )
 from deepset_cloud_sdk.workflows.sync_client.files import list_files as sync_list_files
 from deepset_cloud_sdk.workflows.sync_client.files import (
     list_upload_sessions as sync_list_upload_sessions,
 )
-from deepset_cloud_sdk.workflows.sync_client.files import upload
+from deepset_cloud_sdk.workflows.sync_client.files import upload as sync_upload
 
 cli_app = typer.Typer(pretty_exceptions_show_locals=False)
 
+
 # cli commands
-cli_app.command()(upload)
+@cli_app.command()
+def upload(  # pylint: disable=too-many-arguments
+    paths: List[Path],
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    write_mode: WriteMode = WriteMode.KEEP,
+    blocking: bool = True,
+    timeout_s: Optional[int] = None,
+    show_progress: bool = True,
+    recursive: bool = False,
+    use_type: Optional[List[str]] = None,
+) -> None:
+    """Upload a folder to deepset Cloud.
+
+    :param paths: Path to the folder to upload. If the folder contains unsupported file types, they're skipped.
+    deepset Cloud supports csv, docx, html, json, md, txt, pdf, pptx, xlsx, xml.
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+    Possible options are:
+    KEEP - uploads the file with the same name and keeps both files in the workspace.
+    OVERWRITE - overwrites the file that is in the workspace.
+    FAIL - fails to upload the file with the same name.
+    :param blocking: Whether to wait for the files to be uploaded and displayed in deepset Cloud.
+    :param timeout_s: Timeout in seconds for the `blocking` parameter.
+    :param show_progress: Shows the upload progress.
+    :param recursive: Uploads files from subfolders as well.
+    :param use_type: A comma-separated string of allowed file types to upload, defaults to ".txt, .pdf".
+    """
+    use_type = use_type or [".txt", ".pdf"]
+    sync_upload(
+        paths=paths,
+        api_key=api_key,
+        api_url=api_url,
+        workspace_name=workspace_name,
+        write_mode=write_mode,
+        blocking=blocking,
+        timeout_s=timeout_s,
+        show_progress=show_progress,
+        recursive=recursive,
+        desired_file_types=use_type,
+    )
 
 
 @cli_app.command()
 def download(  # pylint: disable=too-many-arguments
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     file_dir: Optional[str] = None,
     name: Optional[str] = None,
@@ -37,21 +84,20 @@
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     show_progress: bool = True,
 ) -> None:
     """Download files from deepset Cloud to your local machine.
 
     :param workspace_name: Name of the workspace to download the files from. Uses the workspace from the .ENV file by default.
-    :param file_dir: Path to the folder to download. If the folder contains unsupported files, they're skipped.
-    during the upload. Supported file formats are TXT and PDF.
+    :param file_dir: Path to the folder where you want to download the files.
     :param name: Name of the file to odata_filter for.
     :param content: Content of the file to odata_filter for.
     :param odata_filter: odata_filter to apply to the file list.
-    :param include_meta: Whether to include the file meta in the folder.
-    :param batch_size: Batch size for the listing.
+    :param include_meta: Downloads metadata of the files.
+    :param batch_size: Batch size for file listing.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param show_progress: Shows the upload progress.
     """
     sync_download(
         workspace_name=workspace_name,
         file_dir=file_dir,
@@ -86,15 +132,15 @@
     api_url = "https://api.cloud.deepset.ai/api/v1"
     env_content = f"API_KEY={passed_api_key}\nAPI_URL={api_url}\nDEFAULT_WORKSPACE_NAME={passed_default_workspace_name}"
 
     os.makedirs(os.path.dirname(ENV_FILE_PATH), exist_ok=True)
     with open(ENV_FILE_PATH, "w", encoding="utf-8") as env_file:
         env_file.write(env_content)
 
-    typer.echo(f"{ENV_FILE_PATH} created successfully!")
+    typer.echo(f"{ENV_FILE_PATH} created successfully.")
 
 
 @cli_app.command()
 def logout() -> None:
     """Log out of deepset Cloud. This command deletes the .ENV file created during login.
 
     Example:
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/config.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/config.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/deepset_cloud_api.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/deepset_cloud_api.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/files.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/files.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/upload_sessions.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_api/upload_sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         Create FileAPI object.
 
         :param deepset_cloud_api: Instance of the DeepsetCloudAPI.
         """
         self._deepset_cloud_api = deepset_cloud_api
 
     async def create(self, workspace_name: str, write_mode: WriteMode = WriteMode.KEEP) -> UploadSession:
-        """Create and upload session.
+        """Create an upload session.
 
         This method creates an upload session for a given workspace. Use this session to upload files to deepset Cloud.
 
         You must close the session to start the file upload. If you don't close a session, it remains open for 24 hours.
         After that it's automatically closed and you must open a new session to upload more files.
 
         :param workspace_name: Name of the workspace.
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_s3/upload.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_s3/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_service/files_service.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/_service/files_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Module for all file-related operations."""
 from __future__ import annotations
 
 import asyncio
 import json
 import os
 import time
+from collections import defaultdict
 from contextlib import asynccontextmanager
 from pathlib import Path
-from typing import Any, AsyncGenerator, Dict, List, Optional, Union
+from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple, Union
 from uuid import UUID
 
 import structlog
 from tqdm import tqdm
 from yaspin import yaspin
 
 from deepset_cloud_sdk._api.config import CommonConfig
@@ -29,15 +30,15 @@
     WriteMode,
 )
 from deepset_cloud_sdk._s3.upload import S3, S3UploadResult, S3UploadSummary
 from deepset_cloud_sdk.models import DeepsetCloudFile
 
 logger = structlog.get_logger(__name__)
 
-ALLOWED_TYPE_SUFFIXES = [".txt", ".pdf"]
+SUPPORTED_TYPE_SUFFIXES = [".csv", ".docx", ".html", ".json", ".md", ".txt", ".pdf", ".pptx", ".xlsx", ".xml"]
 DIRECT_UPLOAD_THRESHOLD = 20
 
 
 class FilesService:
     """Service for all file-related operations."""
 
     def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, s3: S3):
@@ -107,18 +108,14 @@
         if total_files > 0:
             logger.info(
                 "Uploaded all files.",
                 total_files=total_files,
                 failed_files=upload_session_status.ingestion_status.failed_files,
             )
 
-        logger.warning(
-            "It may take up to three minutes for the files to be visible in deepset Cloud after they were marked as finished."
-        )
-
     @asynccontextmanager
     async def _create_upload_session(
         self,
         workspace_name: str,
         write_mode: WriteMode = WriteMode.KEEP,
     ) -> AsyncGenerator[UploadSession, None]:
         """Create a new upload session.
@@ -193,15 +190,19 @@
         :param timeout_s: Timeout in seconds for the `blocking` parameter.
         :param show_progress If True, shows a progress bar for S3 uploads.
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         if len(file_paths) <= DIRECT_UPLOAD_THRESHOLD:
             logger.info("Uploading files to deepset Cloud.", file_paths=file_paths)
             _coroutines = []
-            _raw_files = [path for path in file_paths if path.suffix.lower() in ALLOWED_TYPE_SUFFIXES]
+            _raw_files = [
+                path
+                for path in file_paths
+                if path.suffix.lower() in SUPPORTED_TYPE_SUFFIXES and not path.name.endswith(".meta.json")
+            ]
             for file_path in _raw_files:
                 meta: Dict[str, Any] = {}
                 meta_path = Path(str(file_path) + ".meta.json")
                 if meta_path in file_paths:
                     with meta_path.open("r") as meta_file:
                         meta = json.loads(meta_file.read())
 
@@ -260,96 +261,148 @@
         :param recursive: If True, recursively walk through all subfolders and return all files.
         """
         file_paths = []
         for path in paths:
             if path.is_file():
                 file_paths.append(path)
             elif recursive:
-                file_paths.extend([file_path for file_path in path.rglob("*")])
+                file_paths.extend([file_path for file_path in path.rglob("*") if file_path.is_file()])
             else:
-                file_paths.extend([file_path for file_path in path.glob("*")])
+                file_paths.extend([file_path for file_path in path.glob("*") if file_path.is_file()])
         return file_paths
 
     @staticmethod
     def _validate_file_paths(file_paths: List[Path]) -> None:
         """Validate a list of file paths.
 
         This method validates the file paths and raises a ValueError if the file paths are invalid.
         It also validates if there are metadata files mapped to not existing raw files.
 
         :param file_paths: A list of paths to upload.
         :raises ValueError: If the file paths are invalid.
         """
         logger.info("Validating file paths and metadata.")
-        allowed_suffixes = {".txt", ".json", ".pdf"}
         for file_path in file_paths:
-            if file_path.suffix.lower() not in allowed_suffixes:
-                raise ValueError(
-                    f"Invalid file extension: {file_path.suffix}. You can upload TXT and PDF files. Metadata files should have the `.meta.json` extension."
-                )
-            if file_path.suffix.lower() == ".json" and not str(file_path).endswith(".meta.json"):
+            if file_path.suffix.lower() not in SUPPORTED_TYPE_SUFFIXES:
                 raise ValueError(
-                    f"JSON files are only supported for metadata files. Make sure you follow this naming format for your metadata files: '<file_name>.meta.json'. Got {file_path.name}."
+                    f"Invalid file extension: {file_path.suffix}. Refer to the list of supported file types in `SUPPORTED_TYPE_SUFFIXES`. "
+                    "Metadata files should have the `.meta.json` extension."
                 )
         meta_file_names = list(
             map(
                 lambda fp: os.path.basename(fp),
-                [file_path for file_path in file_paths if file_path.suffix.lower() == ".json"],
+                [file_path for file_path in file_paths if str(file_path).lower().endswith(".meta.json")],
             )
         )
         file_names = list(map(lambda fp: os.path.basename(fp), file_paths))
-        file_name_set = set(filter(lambda fn: not fn.endswith(".meta.json"), file_names))
+        file_name_set = set(filter(lambda fn: not fn.lower().endswith(".meta.json"), file_names))
 
         not_mapped_meta_files = [
             meta_file_name
             for meta_file_name in meta_file_names
-            if meta_file_name.split(".meta.json")[0] not in file_name_set
+            if meta_file_name.lower().split(".meta.json")[0] not in file_name_set
         ]
 
         if len(not_mapped_meta_files) > 0:
             raise ValueError(
-                f"Metadata files without corresponding text files were found: {not_mapped_meta_files}. "
-                "Make sure each metadata file has a corresponding text or PDF file."
+                f"Metadata files without corresponding files were found: {not_mapped_meta_files}. "
+                "Make sure each metadata file has a corresponding file. "
                 "Map the files using file names like this: '<file_name>' and '<file_name>.meta.json'. "
                 "For example: 'file1.txt' and 'file1.txt.meta.json'."
             )
 
     @staticmethod
-    def _preprocess_paths(paths: List[Path], spinner: yaspin.Spinner = None, recursive: bool = False) -> List[Path]:
+    def _remove_duplicates(file_paths: List[Path]) -> List[Path]:
+        # Group files by their names
+        files_by_name = defaultdict(list)
+        for file_path in file_paths:
+            files_by_name[file_path.name].append(file_path)
+
+        # For each group, sort by modification time and select the most recent
+        most_recent_files = []
+        for file_name, file_group in files_by_name.items():
+            if len(file_group) > 1:
+                logger.warning(
+                    "Multiple files with the same name found. Keeping the most recent one.", file_name=file_name
+                )
+            most_recent_file = sorted(file_group, key=lambda x: x.stat().st_mtime, reverse=True)[0]
+            most_recent_files.append(most_recent_file)
+
+        return most_recent_files
+
+    @staticmethod
+    def _get_allowed_file_types(desired_file_types: Optional[List[Any]]) -> List[str]:
+        """Filter `SUPPORTED_TYPE_SUFFIXES` by `desired_file_types`.
+
+        If desired_file_types is empty, all supported file types are returned.
+        :param desired_file_types: A list of desired file types.
+        :return: A list of desired file types that can be processed by deepset Cloud.
+        """
+        if not desired_file_types:
+            return SUPPORTED_TYPE_SUFFIXES
+
+        desired_types_processed: Set[str] = {
+            str(file_type).lower() if str(file_type).startswith(".") else f".{str(file_type).lower()}"
+            for file_type in desired_file_types
+        }
+        allowed_types: Set[str] = {
+            file_type for file_type in SUPPORTED_TYPE_SUFFIXES if file_type in desired_types_processed
+        }
+
+        return list(allowed_types)
+
+    @staticmethod
+    def _preprocess_paths(
+        paths: List[Path],
+        spinner: yaspin.Spinner = None,
+        recursive: bool = False,
+        desired_file_types: Optional[List[str]] = None,
+    ) -> List[Path]:
         all_files = FilesService._get_file_paths(paths, recursive=recursive)
+
+        allowed_file_types: List[str] = FilesService._get_allowed_file_types(desired_file_types)
+        allowed_meta_types: Tuple = tuple(f"{file_type}.meta.json" for file_type in allowed_file_types)
+
+        meta_file_path = [
+            path for path in all_files if path.is_file() and str(path).lower().endswith(allowed_meta_types)
+        ]
         file_paths = [
             path
             for path in all_files
-            if path.is_file() and ((path.suffix in ALLOWED_TYPE_SUFFIXES) or path.name.endswith("meta.json"))
+            if path.is_file()
+            and (path.suffix.lower() in allowed_file_types and not str(path).lower().endswith(".meta.json"))
         ]
+        combined_paths = meta_file_path + file_paths
 
-        if len(file_paths) < len(all_files):
+        combined_paths = FilesService._remove_duplicates(combined_paths)
+        if len(combined_paths) < len(all_files):
             logger.warning(
                 "Skipping files with unsupported file format.",
                 paths=paths,
-                skipped_files=len(all_files) - len(file_paths),
+                skipped_files=len(all_files) - len(combined_paths),
             )
-            for skipped_file in set(all_files) - set(file_paths):
+            for skipped_file in set(all_files) - set(combined_paths):
                 logger.warning("Skipping file", file_path=skipped_file)
 
         if spinner is not None:
             spinner.text = "Validating files and metadata."
-        FilesService._validate_file_paths(file_paths)
+        FilesService._validate_file_paths(combined_paths)
 
-        return file_paths
+        return combined_paths
 
     async def upload(
         self,
         workspace_name: str,
         paths: List[Path],
         write_mode: WriteMode = WriteMode.KEEP,
         blocking: bool = True,
         timeout_s: Optional[int] = None,
         show_progress: bool = True,
         recursive: bool = False,
+        desired_file_types: List[str] = [".txt", ".pdf"],
     ) -> S3UploadSummary:
         """Upload a list of file or folder paths to a workspace.
 
         Upload files to a selected workspace using upload sessions. It first uploads the files to S3 and then lists them in deepset Cloud.
         Listing the files in deepset Cloud may take a couple of minutes. Use the `blocking` parameter to control if you want to wait until the files are listed and displayed in deepset Cloud.
         If blocking is set to `True`, the function waits until all files are visible in deepset Cloud. If blocking is set to `False`, the function returns immediately after
         the upload of the files to S3 is completed and doesn't wait until the files are shown in deepset Cloud.
@@ -361,24 +414,27 @@
         KEEP - uploads the file with the same name and keeps both files in the workspace.
         OVERWRITE - overwrites the file that is in the workspace.
         FAIL - fails to upload the file with the same name.
         :param blocking: If True, waits until the ingestion to S3 is finished and the files are visible in deepset Cloud.
         :param timeout_s: Timeout in seconds for the `blocking` parameter.
         :param show_progress If True, shows a progress bar for S3 uploads.
         :param recursive: If True, recursively uploads all files in the folder.
+        :param desired_file_types: A list of allowed file types to upload, defaults to ['.txt', '.pdf']
         :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
         """
         logger.info("Getting valid files from file path. This may take a few minutes.", recursive=recursive)
 
         if show_progress:
             with yaspin().arc as sp:
                 sp.text = "Finding uploadable files in the given paths."
-                file_paths = self._preprocess_paths(paths, spinner=sp, recursive=recursive)
+                file_paths = self._preprocess_paths(
+                    paths, spinner=sp, recursive=recursive, desired_file_types=desired_file_types
+                )
         else:
-            file_paths = self._preprocess_paths(paths, recursive=recursive)
+            file_paths = self._preprocess_paths(paths, recursive=recursive, desired_file_types=desired_file_types)
 
         return await self.upload_file_paths(
             workspace_name=workspace_name,
             file_paths=file_paths,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/files.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,41 +124,45 @@
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: Optional[int] = None,
     show_progress: bool = True,
     recursive: bool = False,
+    desired_file_types: Optional[List[str]] = None,
 ) -> S3UploadSummary:
     """Upload a folder to deepset Cloud.
 
     :param paths: Path to the folder to upload. If the folder contains unsupported files, they're skipped.
-    during the upload. Supported file formats are TXT and PDF.
+    during the upload. Supported file formats are txt, pdf, docx, pptx, xlsx, xml, csv, html, md, json.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
     :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
     Possible options are:
     KEEP - uploads the file with the same name and keeps both files in the workspace.
     OVERWRITE - overwrites the file that is in the workspace.
     FAIL - fails to upload the file with the same name.
     :param blocking: Whether to wait for the upload to finish.
     :param timeout_s: Timeout in seconds for the upload.
     :param show_progress: Shows the upload progress.
     :param recursive: Uploads files from subdirectories as well.
+    :param desired_file_types: A list of allowed file types to upload, defaults to ['.txt', '.pdf'].
     """
+    desired_file_types = desired_file_types or [".txt", ".pdf"]
     async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
         return await file_service.upload(
             workspace_name=workspace_name,
             paths=paths,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
             show_progress=show_progress,
             recursive=recursive,
+            desired_file_types=desired_file_types,
         )
 
 
 async def download(
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     file_dir: Optional[Union[Path, str]] = None,
     name: Optional[str] = None,
@@ -172,16 +176,15 @@
     timeout_s: Optional[int] = None,
 ) -> None:
     """Download a folder to deepset Cloud.
 
     Downloads all files from a workspace to a local folder.
 
     :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
-    :param file_dir: Path to the folder to download. If the folder contains unsupported files, they're skipped.
-    during the upload. Supported file formats are TXT and PDF.
+    :param file_dir: Path to the folder to download.
     :param name: Name of the file to odata_filter by.
     :param content: Content of a file to odata_filter by.
     :param odata_filter: odata_filter by file meta data.
     :param include_meta: Whether to include the file meta in the folder.
     :param batch_size: Batch size for the listing.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/files.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sync client for files workflow."""
+
 import asyncio
 from pathlib import Path
 from typing import Generator, List, Optional, Union
 from uuid import UUID
 
 import structlog
 
@@ -30,53 +31,57 @@
     upload_texts as async_upload_texts,
 )
 from deepset_cloud_sdk.workflows.sync_client.utils import iter_over_async
 
 logger = structlog.get_logger(__name__)
 
 
-def upload(
+def upload(  # pylint: disable=too-many-arguments
     paths: List[Path],
     api_key: Optional[str] = None,
     api_url: Optional[str] = None,
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     write_mode: WriteMode = WriteMode.KEEP,
     blocking: bool = True,
     timeout_s: Optional[int] = None,
     show_progress: bool = True,
     recursive: bool = False,
+    desired_file_types: Optional[List[str]] = None,
 ) -> S3UploadSummary:
     """Upload a folder to deepset Cloud.
 
     :param paths: Path to the folder to upload. If the folder contains unsupported file types, they're skipped.
-    deepset Cloud supports TXT and PDF files.
+    deepset Cloud supports csv, docx, html, json, md, txt, pdf, pptx, xlsx, xml.
     :param api_key: deepset Cloud API key to use for authentication.
     :param api_url: API URL to use for authentication.
     :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
     :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
     Possible options are:
     KEEP - uploads the file with the same name and keeps both files in the workspace.
     OVERWRITE - overwrites the file that is in the workspace.
     FAIL - fails to upload the file with the same name.
     :param blocking: Whether to wait for the files to be uploaded and displayed in deepset Cloud.
     :param timeout_s: Timeout in seconds for the `blocking` parameter.
     :param show_progress: Shows the upload progress.
     :param recursive: Uploads files from subfolders as well.
+    :param desired_file_types: A list of allowed file types to upload, defaults to ".txt, .pdf".
     """
+    desired_file_types = desired_file_types or [".txt", ".pdf"]
     return asyncio.run(
         async_upload(
             paths=paths,
             api_key=api_key,
             api_url=api_url,
             workspace_name=workspace_name,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
             show_progress=show_progress,
             recursive=recursive,
+            desired_file_types=desired_file_types,
         )
     )
 
 
 def download(  # pylint: disable=too-many-arguments
     workspace_name: str = DEFAULT_WORKSPACE_NAME,
     file_dir: Optional[Union[Path, str]] = None,
@@ -91,16 +96,15 @@
     timeout_s: Optional[int] = None,
 ) -> None:
     """Download a folder to deepset Cloud.
 
     Downloads all files from a workspace to a local folder.
 
     :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
-    :param file_dir: Path to the folder to download. If the folder contains unsupported files, they're skipped.
-    during the upload. Supported file formats are TXT and PDF.
+    :param file_dir: Path to the folder to download.
     :param name: Name of the file to odata_filter by.
     :param content: Content of a file to odata_filter by.
     :param odata_filter: odata_filter by file meta data.
     :param include_meta: Whether to include the file meta in the folder.
     :param batch_size: Batch size for the listing.
     :param api_key: API key to use for authentication.
     :param api_url: API URL to use for authentication.
```

### Comparing `deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/utils.py` & `deepset_cloud_sdk-1.0.0/deepset_cloud_sdk/workflows/sync_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/index.md` & `deepset_cloud_sdk-1.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/upload_files.md` & `deepset_cloud_sdk-1.0.0/docs/upload_files.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,41 +8,64 @@
 
 ## Folder Structure
 
 You don't need to follow any specific folder structure. If your folder contains files with the same name, all these files are uploaded, by default. You can set the `--write-mode` to overwrite the files, keep them all, or fail the upload. For more information, see [CLI examples](/examples/cli/README.md) and [SDK examples](/examples/sdk/README.md).
 
 # Upload Files
 
-To upload files:
+## Upload text files:
+
+By default it is allowed to upload .txt and .pdf files. See below to upload different file types.
 
 1. Log in to the sdk: `deepset-cloud login` (MacOS and Linux) or `python -m deepset_cloud_sdk.cli login` (Windows).
 2. When prompted, paste your deepset Cloud API key.
 3. Type the name of the deepset Cloud workspace you want to set as default for all operations.
 4. Choose if you want to use the CLI or a Python script to upload:
     - To upload files from a folder using CLI, run: `deepset-cloud upload <path to the upload folder>` (MacOS and Linux) or `python -m deepset_cloud_sdk.cli upload <path to the upload folder>` (On Windows)
-    - To upload files from a folder using a Python script, create the script and run it. Here's an example you can use: 
+    - To upload files from a folder using a Python script, create the script and run it. Here's an example you can use:
 
     ```python
     from pathlib import Path
     from deepset_cloud_sdk.workflows.sync_client.files import upload
-    
-    ## Uploads all files from a given path
+
+    ## Uploads all txt and pdf files from a given path
     upload(
     paths=[Path("<your_path_to_the_upload_folder>")],
     blocking=True,  # waits until the files are displayed in deepset Cloud,
                     # this may take a couple of minutes
     timeout_s=300,  # the timeout for the `blocking` parameter in number of seconds
     show_progress=True,  # shows the progress bar
-    recursive=True,  # uploads files from all subfolders as well
+    recursive=True,  # uploads text files from all subfolders as well
     )
+    ```
+
+## Upload other file types
 
+Deepset Cloud currently supports uploading : .csv, .docx, .html, .json, .md, .txt, .pdf, .pptx, .xlsx and .xml.
+
+
+    ```python
+    from pathlib import Path
+    from deepset_cloud_sdk.workflows.sync_client.files import upload
+
+    ## Uploads supported files from a given path
+    upload(
+    paths=[Path("<your_path_to_the_upload_folder>")],
+    blocking=True,
+    timeout_s=300,
+    show_progress=True,
+    recursive=True,
+    desired_file_types=[ # list of desired file types to upload
+        ".csv", ".docx", ".html", ".json", ".md", ".txt", ".pdf", ".pptx", ".xlsx", ".xml"
+    ]
+    )
     ```
 
 For more examples, see [CLI examples](/examples/cli/README.md) and [SDK examples](/examples/sdk/README.md).
 
 # Metadata
 
-To add metadata to your files, create one metadata file for each TXT or PDF file you upload. The metadata file must be a JSON with the same name as the file whose metadata it contains and the extension `meta.json`.
+To add metadata to your files, create one metadata file for each file you upload. The metadata file must be a JSON with the same name as the file whose metadata it contains and the extension `meta.json`.
 
 For example, if you're uploading a file called `example.txt`, the metadata file should be called `example.txt.meta.json`. If you're uploading a file called `example.pdf`, the metadata file should be `example.pdf.meta.json`.
 
-The format your metadata in your metadata files should follow is: `{"meta_key1": "value1", "meta_key2": "value2"}`. See the [example metadata file](/examples/data/example.txt.meta.json).
+The format your metadata in your metadata files should follow is: `{"meta_key1": "value1", "meta_key2": "value2"}`. See the [example metadata file](/examples/data/example.txt.meta.json).
```

### Comparing `deepset_cloud_sdk-0.41/docs/_images/favicon.svg` & `deepset_cloud_sdk-1.0.0/docs/_images/favicon.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/_images/white-logo.svg` & `deepset_cloud_sdk-1.0.0/docs/_images/white-logo.svg`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/_pydoc/renderers.py` & `deepset_cloud_sdk-1.0.0/docs/_pydoc/renderers.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/_pydoc/config/async_client.yml` & `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/async_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/_pydoc/config/cli.yml` & `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/cli.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/_pydoc/config/sync_client.yml` & `deepset_cloud_sdk-1.0.0/docs/_pydoc/config/sync_client.yml`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/examples/cli/README.md` & `deepset_cloud_sdk-1.0.0/docs/examples/cli/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -44,28 +44,29 @@
 
 ## Example Commands
 
 ### Upload Files and Folders
 
 You don't have to follow any special folder structure. If there are multiple files with the same name in your folder, they're all uploaded by default. You can change this behavior with the `--write-mode` flag. See the examples below.
 
-This command uploads the file example.txt to your deepset Cloud workspace. 
+This command uploads the file example.txt to your deepset Cloud workspace.
 On MacOS and Linux:
 
 ```shell
 deepset-cloud upload ./examples/data/example.txt
 ```
 
 On Windows:
 
 ```shell
 python -m deepset_cloud_sdk.cli upload ./examples/data/example.txt
 ```
 
-This command uploads the entire data folder located in the _examples_ directory to your deepset Cloud workspace.
+This command uploads all `.txt` and `.pdf` files from the folder located in the _examples_ directory to your deepset Cloud workspace. By default only `.txt` and `.pdf` files are uploaded. To upload different file types see below.
+
 The paths in the examples are relative to the current working directory.
 
 On MacOS and Linux:
 
 ```shell
 deepset-cloud upload ./examples/data
 ```
@@ -81,14 +82,28 @@
 ```
 On Windows:
 ```shell
 python -m deepset_cloud_sdk.cli upload ./examples/data --write-mode OVERWRITE
 ```
 This syncs your local files with the files in your deepset Cloud workspace without having to manually delete the files in your workspace.
 
+## Upload different file types
+
+To upload other file types than text, specify the desired file types using the flag `--use-type`.
+The command below uploads all file types from the ./example/data directory that are supported by deepset Cloud.
+
+```shell
+deepset-cloud upload ./examples/data --use-type .csv --use-type .docx --use-type .html --use-type .json --use-type .md --use-type .txt --use-type .pdf --use-type .pptx --use-type .xlsx --use-type .xml
+
+```
+On Windows:
+```shell
+python -m deepset_cloud_sdk.cli upload ./examples/data --use-type .csv --use-type .docx --use-type .html --use-type .json --use-type .md --use-type .txt --use-type .pdf --use-type .pptx --use-type .xlsx --use-type .xml
+```
+
 
 ### Downloading Files from deepset Cloud
 This command downloads all files from a workspace to a local directory. For example:
 
 On MacOS and Linux:
 
 ```shell
```

### Comparing `deepset_cloud_sdk-0.41/docs/examples/data/example.pdf` & `deepset_cloud_sdk-1.0.0/docs/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/examples/sdk/README.md` & `deepset_cloud_sdk-1.0.0/docs/examples/sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/docs/examples/sdk/upload.py` & `deepset_cloud_sdk-1.0.0/docs/examples/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/.gitignore` & `deepset_cloud_sdk-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/LICENSE` & `deepset_cloud_sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/README.md` & `deepset_cloud_sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.41/pyproject.toml` & `deepset_cloud_sdk-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,49 +6,47 @@
 name = "deepset-cloud-sdk"
 dynamic = ["version"]
 description = 'deepset Cloud SDK'
 readme = "README.md"
 requires-python = ">= 3.8"
 license = "Apache-2.0"
 keywords = []
-authors = [
-  { name = "deepset", email = "rohan.janjua@deepset.ai" },
-]
+authors = [{ name = "deepset", email = "rohan.janjua@deepset.ai" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "structlog==24.1.0",
-  "httpx==0.26.0",
-  "python-dotenv==1.0.0",
-  "typer==0.9.0",
+  "httpx==0.27.0",
+  "python-dotenv==1.0.1",
+  "typer==0.12.3",
   "tenacity==8.2.3",
-  "aiohttp==3.9.1",
+  "aiohttp==3.9.5",
   "aiofiles==23.2.1",
   "tabulate==0.9.0",
-  "tqdm==4.66.1",
+  "tqdm==4.66.2",
   "yaspin==2.3.0",
-  "pyrate-limiter==3.4.1",
+  "pyrate-limiter==3.6.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/deepset-cloud-sdk#readme"
 Issues = "https://github.com/deepset-ai/deepset-cloud-sdk/issues"
 Source = "https://github.com/deepset-ai/deepset-cloud-sdk"
 
 
 [project.scripts]
-deepset-cloud  = "deepset_cloud_sdk.cli:run_packaged"
+deepset-cloud = "deepset_cloud_sdk.cli:run_packaged"
 
 [tool.hatch.version]
 path = "deepset_cloud_sdk/__about__.py"
 
 [tool.hatch.envs.default.scripts]
 tests-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
 tests-unit = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
@@ -56,50 +54,50 @@
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10"]
 
 [tool.hatch.envs.default]
 dependencies = [
   "structlog==24.1.0",
-  "httpx==0.26.0",
-  "python-dotenv==1.0.0",
+  "httpx==0.27.0",
+  "python-dotenv==1.0.1",
   "tenacity==8.2.3",
-  "aiohttp==3.9.1",
-  "pyrate-limiter==3.4.1",
+  "aiohttp==3.9.5",
+  "pyrate-limiter==3.6.0",
 ]
 
 [tool.hatch.envs.test.scripts]
 unit-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
 integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
 
 [tool.hatch.envs.test]
-template='default'
+template = 'default'
 dependencies = [
   "pytest-cov==4.0.0",
   "pytest==7.3.1",
   "pytest-asyncio==0.21.0",
   "Faker==19.13.0",
 ]
 
 
 [tool.hatch.envs.code-quality]
 python = "3.10"
-template='default'
+template = 'default'
 detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
 dependencies = [
   "pylint==2.17.4",
   "pydocstyle==6.3.0",
   "black==23.3.0",
   "isort==5.12.0",
   "mypy==1.1.1",
   "pre-commit==2.20.0",
   "types-aiofiles==23.1.0.2",
   "types-tabulate==0.9.0.2",
-  "autoflake==2.1.1"
+  "autoflake==2.1.1",
 ]
 
 [tool.hatch.envs.code-quality.scripts]
 types = "mypy deepset_cloud_sdk tests"
 format = "black deepset_cloud_sdk tests --check"
 format-fix = "black deepset_cloud_sdk tests"
 lint = "pylint deepset_cloud_sdk"
@@ -109,71 +107,54 @@
 docstrings = "pydocstyle deepset_cloud_sdk"
 flake = "autoflake --remove-all-unused-imports --remove-duplicate-keys --remove-unused-variables -v -r ./deepset_cloud_sdk"
 all = "hatch run types && hatch run format-fix && hatch run lint && hatch run sort && hatch run docstrings && hatch run flake"
 
 [tool.hatch.envs.tools]
 detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
-dependencies = [
-  "pip-tools==6.13.0",
-]
+dependencies = ["pip-tools==6.13.0"]
 
 [tool.hatch.envs.tools.scripts]
 requirements = "pip-compile -o requirements.txt pyproject.toml"
 
 [tool.coverage.run]
 branch = true
 relative_files = true
-omit = [
-  "deepset_cloud_sdk/__about__.py",
-]
+omit = ["deepset_cloud_sdk/__about__.py"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
 python_version = "3.10"
 warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 [tool.pylint.'MESSAGES CONTROL']
-max-line-length=150
+max-line-length = 150
 disable = [
   "fixme",
   "c-extension-no-member",
   "wrong-spelling-in-comment",
   "wrong-spelling-in-docstring",
-  "missing-module-docstring"
-  ]
+  "missing-module-docstring",
+]
 [tool.pylint.'DESIGN']
-max-args=9
+max-args = 9
 
 [tool.pylint.'SIMILARITIES']
-min-similarity-lines=10
+min-similarity-lines = 10
 
 [tool.pylint.'BASIC']
-good-names=[
-  "i",
-  "k",
-  "v",
-  "_",
-  "f1"
-  ]
+good-names = ["i", "k", "v", "_", "f1"]
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-  "/tests",
-]
+exclude = ["/.github", "/tests"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["deepset_cloud_sdk"]
```

### Comparing `deepset_cloud_sdk-0.41/PKG-INFO` & `deepset_cloud_sdk-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: deepset-cloud-sdk
-Version: 0.41
+Version: 1.0.0
 Summary: deepset Cloud SDK
 Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
 Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
 Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
 Author-email: deepset <rohan.janjua@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -14,23 +14,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: httpx==0.26.0
-Requires-Dist: pyrate-limiter==3.4.1
-Requires-Dist: python-dotenv==1.0.0
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: httpx==0.27.0
+Requires-Dist: pyrate-limiter==3.6.0
+Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tenacity==8.2.3
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: typer==0.9.0
+Requires-Dist: tqdm==4.66.2
+Requires-Dist: typer==0.12.3
 Requires-Dist: yaspin==2.3.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.41 Summary: deepset
+Metadata-Version: 2.3 Name: deepset-cloud-sdk Version: 1.0.0 Summary: deepset
 Cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
 cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
 cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
 cloud-sdk Author-email: deepset
 deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8 Requires-
-Dist: aiofiles==23.2.1 Requires-Dist: aiohttp==3.9.1 Requires-Dist:
-httpx==0.26.0 Requires-Dist: pyrate-limiter==3.4.1 Requires-Dist: python-
-dotenv==1.0.0 Requires-Dist: structlog==24.1.0 Requires-Dist: tabulate==0.9.0
-Requires-Dist: tenacity==8.2.3 Requires-Dist: tqdm==4.66.1 Requires-Dist:
-typer==0.9.0 Requires-Dist: yaspin==2.3.0 Description-Content-Type: text/
+Dist: aiofiles==23.2.1 Requires-Dist: aiohttp==3.9.5 Requires-Dist:
+httpx==0.27.0 Requires-Dist: pyrate-limiter==3.6.0 Requires-Dist: python-
+dotenv==1.0.1 Requires-Dist: structlog==24.1.0 Requires-Dist: tabulate==0.9.0
+Requires-Dist: tenacity==8.2.3 Requires-Dist: tqdm==4.66.2 Requires-Dist:
+typer==0.12.3 Requires-Dist: yaspin==2.3.0 Description-Content-Type: text/
 markdown
                               _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _S_D_K_]
 [![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-
 coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-
 cloud-sdk/tree/python-coverage-comment-action-data) [![Tests](https://
 github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-
 integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/
```

