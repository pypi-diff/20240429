# Comparing `tmp/jobbergate_api-5.1.0a0.tar.gz` & `tmp/jobbergate_api-5.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-5.1.0a0.tar", max compression
+gzip compressed data, was "jobbergate_api-5.2.0a0.tar", max compression
```

## Comparing `jobbergate_api-5.1.0a0.tar` & `jobbergate_api-5.2.0a0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1082 2024-04-19 17:22:07.000610 jobbergate_api-5.1.0a0/LICENSE
--rw-r--r--   0        0        0      683 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/README.md
--rw-r--r--   0        0        0      169 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       54 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/__init__.py
--rw-r--r--   0        0        0      944 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/models.py
--rw-r--r--   0        0        0     2126 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/routers.py
--rw-r--r--   0        0        0     1582 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/schemas.py
--rw-r--r--   0        0        0      177 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/constants.py
--rw-r--r--   0        0        0     5251 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/dependencies.py
--rw-r--r--   0        0        0     3620 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/file_validation.py
--rw-r--r--   0        0        0     1955 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/garbage_collector.py
--rw-r--r--   0        0        0       43 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/__init__.py
--rw-r--r--   0        0        0      100 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/constants.py
--rw-r--r--   0        0        0     4098 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/models.py
--rw-r--r--   0        0        0    15042 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/routers.py
--rw-r--r--   0        0        0     7060 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/schemas.py
--rw-r--r--   0        0        0     3749 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/services.py
--rw-r--r--   0        0        0       40 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     2984 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    13361 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4759 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0     6390 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/services.py
--rw-r--r--   0        0        0     1295 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/tools.py
--rw-r--r--   0        0        0       44 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6561 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     3575 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    14275 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0     8208 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1285 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/services.py
--rw-r--r--   0        0        0     5986 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/models.py
--rw-r--r--   0        0        0      558 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     2254 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/schemas.py
--rw-r--r--   0        0        0    23693 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/services.py
--rw-r--r--   0        0        0     4589 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/config.py
--rw-r--r--   0        0        0     2467 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     1627 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/logging.py
--rw-r--r--   0        0        0     3622 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/main.py
--rw-r--r--   0        0        0     3436 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0     2781 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/rabbitmq_notification.py
--rw-r--r--   0        0        0     1082 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/safe_types.py
--rw-r--r--   0        0        0     4598 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/security.py
--rw-r--r--   0        0        0    10874 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/storage.py
--rw-r--r--   0        0        0     1146 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/version.py
--rw-r--r--   0        0        0     3982 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/README.md
+-rw-r--r--   0        0        0      169 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/__init__.py
+-rw-r--r--   0        0        0      944 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/models.py
+-rw-r--r--   0        0        0     2114 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/routers.py
+-rw-r--r--   0        0        0     1582 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/schemas.py
+-rw-r--r--   0        0        0      177 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/constants.py
+-rw-r--r--   0        0        0     5251 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/dependencies.py
+-rw-r--r--   0        0        0     3620 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/file_validation.py
+-rw-r--r--   0        0        0     1955 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/garbage_collector.py
+-rw-r--r--   0        0        0       43 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/constants.py
+-rw-r--r--   0        0        0     4098 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/models.py
+-rw-r--r--   0        0        0    15897 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/routers.py
+-rw-r--r--   0        0        0     7060 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/schemas.py
+-rw-r--r--   0        0        0     3749 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/services.py
+-rw-r--r--   0        0        0       40 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     2984 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    13925 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4759 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0     6390 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/services.py
+-rw-r--r--   0        0        0     1295 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/tools.py
+-rw-r--r--   0        0        0       44 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6561 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     3575 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    14577 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0     8208 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1285 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/services.py
+-rw-r--r--   0        0        0     5986 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/models.py
+-rw-r--r--   0        0        0     1065 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     2254 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/schemas.py
+-rw-r--r--   0        0        0    23693 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/apps/services.py
+-rw-r--r--   0        0        0     4589 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2467 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     1627 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/logging.py
+-rw-r--r--   0        0        0     3622 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3436 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0     2781 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/rabbitmq_notification.py
+-rw-r--r--   0        0        0     1082 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/safe_types.py
+-rw-r--r--   0        0        0     4598 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/security.py
+-rw-r--r--   0        0        0    10874 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/storage.py
+-rw-r--r--   0        0        0     1146 2024-04-29 20:17:27.676660 jobbergate_api-5.2.0a0/jobbergate_api/version.py
+-rw-r--r--   0        0        0     3982 2024-04-29 20:17:27.680660 jobbergate_api-5.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.2.0a0/PKG-INFO
```

### Comparing `jobbergate_api-5.1.0a0/LICENSE` & `jobbergate_api-5.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/README.md` & `jobbergate_api-5.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/models.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/routers.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/routers.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "/status",
     status_code=status.HTTP_202_ACCEPTED,
     description="Endpoints to accept a status check from the agent on the clusters.",
 )
 async def report_cluster_status(
     interval: int = Query(description="The interval in seconds between pings.", gt=0),
     secure_session: SecureSession = Depends(
-        secure_session(Permissions.JOB_SUBMISSIONS_EDIT, ensure_client_id=True)
+        secure_session(Permissions.CLUSTERS_UPDATE, ensure_client_id=True)
     ),
 ):
     """
     Report the status of the cluster.
     """
     logger.debug(
         "Got status report from client_id={}, another ping is expected in {} seconds",
@@ -48,15 +48,15 @@
 
 @router.get(
     "/status",
     description="Endpoint to get the status of the cluster.",
     response_model=Page[ClusterStatusView],
 )
 async def get_cluster_status(
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_SUBMISSIONS_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.CLUSTERS_READ, commit=False)),
 ):
     """
     Get the status of the cluster.
     """
     logger.debug("Getting list of cluster statuses")
     query = select(ClusterStatus).order_by(ClusterStatus.client_id)
     return await paginate(secure_session.session, query)
```

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/schemas.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/clusters/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/dependencies.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/dependencies.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/file_validation.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/garbage_collector.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/models.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/routers.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/routers.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     status_code=status.HTTP_201_CREATED,
     response_model=JobTemplateDetailedView,
     description="Endpoint for job script template creation",
 )
 async def job_script_template_create(
     create_request: JobTemplateCreateRequest,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_CREATE, ensure_email=True)
     ),
 ):
     """Create a new job script template."""
     logger.info(f"Creating a new job script template with {create_request=}")
 
     try:
         return await secure_services.crud.template.create(
@@ -59,15 +59,15 @@
 @router.get(
     "/{id_or_identifier}",
     description="Endpoint to return a job script template by its id or identifier",
     response_model=JobTemplateDetailedView,
 )
 async def job_script_template_get(
     id_or_identifier: int | str = Path(),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_READ, commit=False)),
 ):
     """Get a job script template by id or identifier."""
     logger.info(f"Getting job script template with {id_or_identifier=}")
     return await secure_services.crud.template.get(id_or_identifier, include_files=True)
 
 
 @router.post(
@@ -76,15 +76,15 @@
     response_model=JobTemplateDetailedView,
     description="Endpoint for cloning a job script template to a new entry owned by the user",
 )
 async def job_script_template_clone(
     id_or_identifier: int | str = Path(),
     clone_request: JobTemplateCloneRequest | None = None,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_CREATE, ensure_email=True)
     ),
 ):
     """Clone a job script template by id or identifier."""
     logger.info(f"Cloning a job script template from {id_or_identifier=} with {clone_request=}")
 
     if clone_request is None:
         clone_request = JobTemplateCloneRequest()
@@ -119,15 +119,15 @@
     "",
     description="Endpoint to return a list of job script templates",
     response_model=Page[JobTemplateListView],
 )
 async def job_script_template_get_list(
     list_params: ListParams = Depends(),
     include_null_identifier: bool = Query(False),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_READ, commit=False)),
 ):
     """Get a list of job script templates."""
     logger.debug("Preparing to list job script templates")
 
     list_kwargs = list_params.dict(exclude_unset=True, exclude={"user_only", "include_parent"})
 
     if list_params.user_only:
@@ -145,55 +145,59 @@
     description="Endpoint to update a job script template by id or identifier",
     response_model=JobTemplateDetailedView,
 )
 async def job_script_template_update(
     update_request: JobTemplateUpdateRequest,
     id_or_identifier: int | str = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_UPDATE, ensure_email=True)
     ),
 ):
     """Update a job script template by id or identifier."""
     logger.info(f"Updating job script template {id_or_identifier=} with {update_request=}")
-    await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    instance = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            instance, owner_email=secure_services.identity_payload.email
+        )
     return await secure_services.crud.template.update(
         id_or_identifier, **update_request.dict(exclude_unset=True)
     )
 
 
 @router.delete(
     "/{id_or_identifier}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete a job script template by id or identifier",
 )
 async def job_script_template_delete(
     id_or_identifier: int | str = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_DELETE, ensure_email=True)
     ),
 ):
     """Delete a job script template by id or identifier."""
     logger.info(f"Deleting job script template with {id_or_identifier=}")
-    await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    isinstance = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            isinstance, owner_email=secure_services.identity_payload.email
+        )
     await secure_services.crud.template.delete(id_or_identifier)
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
     "/{id_or_identifier}/upload/template/{file_name:path}",
     description="Endpoint to get a file from a job script template by id or identifier",
 )
 async def job_script_template_get_file(
     id_or_identifier: int | str = Path(),
     file_name: str = Path(),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_READ, commit=False)),
 ):
     """
     Get a job script template file by id or identifier.
 
     Note:
         See https://fastapi.tiangolo.com/advanced/custom-response/#streamingresponse
     """
@@ -214,28 +218,30 @@
     response_model=TemplateFileDetailedView,
 )
 async def job_script_template_upload_file(
     id_or_identifier: int | str = Path(),
     file_type: FileType = Path(),
     upload_file: UploadFile = File(..., description="File to upload"),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_CREATE, ensure_email=True)
     ),
 ):
     """Upload a file to a job script template by id or identifier."""
     if upload_file.filename is None:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail="The upload file has no filename",
         )
 
     logger.debug(f"Uploading file {upload_file.filename} to job script template {id_or_identifier=}")
-    job_script_template = await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    job_script_template = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            job_script_template, owner_email=secure_services.identity_payload.email
+        )
 
     return await secure_services.file.template.upsert(
         parent_id=job_script_template.id,
         filename=upload_file.filename,
         upload_content=upload_file,
         file_type=file_type,
     )
@@ -246,32 +252,34 @@
     status_code=status.HTTP_200_OK,
     description="Endpoint to delete a file to a job script template by id or identifier",
 )
 async def job_script_template_delete_file(
     id_or_identifier: int | str = Path(),
     file_name: str = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_DELETE, ensure_email=True)
     ),
 ):
     """Delete a file from a job script template by id or identifier."""
-    job_script_template = await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    job_script_template = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            job_script_template, owner_email=secure_services.identity_payload.email
+        )
     job_script_template_file = await secure_services.file.template.get(job_script_template.id, file_name)
     await secure_services.file.template.delete(job_script_template_file)
 
 
 @router.get(
     "/{id_or_identifier}/upload/workflow",
     description="Endpoint to get a workflow file from a job script template by id or identifier",
 )
 async def job_script_workflow_get_file(
     id_or_identifier: int | str = Path(),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_READ, commit=False)),
 ):
     """
     Get a workflow file by id or identifier.
 
     Note:
         See https://fastapi.tiangolo.com/advanced/custom-response/#streamingresponse
     """
@@ -294,23 +302,24 @@
 async def job_script_workflow_upload_file(
     id_or_identifier: int | str = Path(),
     runtime_config: RunTimeConfig | None = Body(
         None, description="Runtime configuration is optional when the workflow file already exists"
     ),
     upload_file: UploadFile = File(..., description="File to upload"),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_CREATE, ensure_email=True)
     ),
 ):
     """Upload a file to a job script workflow by id or identifier."""
     logger.debug(f"Uploading workflow file to job script template {id_or_identifier=}: {runtime_config}")
-    job_script_template = await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
-
+    job_script_template = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            job_script_template, owner_email=secure_services.identity_payload.email
+        )
     upsert_kwargs = dict(
         parent_id=job_script_template.id, filename=WORKFLOW_FILE_NAME, upload_content=upload_file
     )
 
     try:
         await secure_services.file.workflow.get(job_script_template.id, WORKFLOW_FILE_NAME)
         file_exist = True
@@ -332,35 +341,37 @@
     "/{id_or_identifier}/upload/workflow",
     status_code=status.HTTP_200_OK,
     description="Endpoint to delete a workflow file from a job script template by id or identifier",
 )
 async def job_script_workflow_delete_file(
     id_or_identifier: int | str = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_TEMPLATES_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_TEMPLATES_DELETE, ensure_email=True)
     ),
 ):
     """Delete a workflow file from a job script template by id or identifier."""
     logger.debug(f"Deleting workflow file from job script template {id_or_identifier=}")
-    job_script_template = await secure_services.crud.template.get(
-        id_or_identifier, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    job_script_template = await secure_services.crud.template.get(id_or_identifier)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.template.ensure_attribute(
+            job_script_template, owner_email=secure_services.identity_payload.email
+        )
     workflow_file = await secure_services.file.workflow.get(job_script_template.id, WORKFLOW_FILE_NAME)
     await secure_services.file.workflow.delete(workflow_file)
 
 
 @router.delete(
     "/upload/garbage-collector",
     status_code=status.HTTP_202_ACCEPTED,
     description="Endpoint to delete all unused files from the job script template file storage",
     tags=["Garbage collector"],
 )
 async def job_script_template_garbage_collector(
     background_tasks: BackgroundTasks,
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_EDIT)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_TEMPLATES_DELETE)),
 ):
     """Delete all unused files from jobbergate templates on the file storage."""
     logger.info("Starting garbage collection from jobbergate file storage")
     background_tasks.add_task(
         garbage_collect,
         secure_services.session,
         secure_services.bucket,
```

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/schemas.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/services.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_script_templates/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "/clean-unused-entries",
     status_code=status.HTTP_202_ACCEPTED,
     description="Endpoint to automatically clean unused job scripts depending on a threshold",
     tags=["Garbage collector"],
 )
 def job_script_auto_clean_unused_entries(
     background_tasks: BackgroundTasks,
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_EDIT)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_DELETE)),
 ):
     """Automatically clean unused job scripts depending on a threshold."""
     logger.info("Starting automatically cleanup for unused job scripts")
     background_tasks.add_task(secure_services.crud.job_script.auto_clean_unused_job_scripts)
     return {"description": "Automatically cleanup started"}
 
 
@@ -51,15 +51,15 @@
     "",
     status_code=status.HTTP_201_CREATED,
     response_model=JobScriptDetailedView,
     description="Endpoint for creating a stand alone job script. Use file upload to add files.",
 )
 async def job_script_create(
     create_request: JobScriptCreateRequest,
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_EDIT)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_CREATE)),
 ):
     """Create a stand alone job script."""
     logger.info(f"Creating a new job script with {create_request=}")
 
     if secure_services.identity_payload.email is None:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
@@ -78,15 +78,15 @@
     response_model=JobScriptDetailedView,
     description="Endpoint for cloning a job script to a new entry owned by the user",
 )
 async def job_script_clone(
     id: int = Path(),
     clone_request: JobScriptCloneRequest | None = None,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_CREATE, ensure_email=True)
     ),
 ):
     """Clone a job script by its id."""
     logger.info(f"Cloning a job script from {id=} with {clone_request=}")
 
     if clone_request is None:
         clone_request = JobScriptCloneRequest()
@@ -112,15 +112,15 @@
     description="Endpoint for job script creation",
 )
 async def job_script_create_from_template(
     create_request: JobScriptCreateRequest,
     render_request: RenderFromTemplateRequest,
     id_or_identifier: int | str = Path(...),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_CREATE, ensure_email=True)
     ),
 ):
     """Create a new job script from a job script template."""
     logger.info(f"Creating a new job script from {id_or_identifier=} with {create_request=}")
 
     base_template = cast(
         JobScriptTemplate, await secure_services.crud.template.get(id_or_identifier, include_files=True)
@@ -185,15 +185,15 @@
 @router.get(
     "/{id}",
     description="Endpoint to return a job script by its id",
     response_model=JobScriptDetailedView,
 )
 async def job_script_get(
     id: int = Path(),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_READ, commit=False)),
 ):
     """Get a job script by id."""
     logger.info(f"Getting job script {id=}")
     return await secure_services.crud.job_script.get(id, include_files=True)
 
 
 @router.get(
@@ -203,15 +203,15 @@
 )
 async def job_script_get_list(
     list_params: ListParams = Depends(),
     from_job_script_template_id: int | None = Query(
         None,
         description="Filter job-scripts by the job-script-template-id they were created from.",
     ),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_READ, commit=False)),
 ):
     """Get a list of job scripts."""
     logger.debug("Preparing to list job scripts")
 
     list_kwargs = list_params.dict(exclude_unset=True, exclude={"user_only"})
 
     if from_job_script_template_id is not None:
@@ -228,53 +228,57 @@
     description="Endpoint to update a job script by id",
     response_model=JobScriptListView,
 )
 async def job_script_update(
     update_params: JobScriptUpdateRequest,
     id: int = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_UPDATE, ensure_email=True)
     ),
 ):
     """Update a job script template by id or identifier."""
     logger.info(f"Updating job script {id=} with {update_params=}")
-    await secure_services.crud.job_script.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    instance = await secure_services.crud.job_script.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_script.ensure_attribute(
+            instance, owner_email=secure_services.identity_payload.email
+        )
     return await secure_services.crud.job_script.update(id, **update_params.dict(exclude_unset=True))
 
 
 @router.delete(
     "/{id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete a job script by id",
 )
 async def job_script_delete(
     id: int = Path(...),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_DELETE, ensure_email=True)
     ),
 ):
     """Delete a job script template by id or identifier."""
     logger.info(f"Deleting job script {id=}")
-    await secure_services.crud.job_script.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    instance = await secure_services.crud.job_script.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_script.ensure_attribute(
+            instance, owner_email=secure_services.identity_payload.email
+        )
     await secure_services.crud.job_script.delete(id)
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
     "/{id}/upload/{file_name:path}",
     description="Endpoint to get a file from a job script",
 )
 async def job_script_get_file(
     id: int = Path(...),
     file_name: str = Path(...),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_READ, commit=False)),
 ):
     """
     Get a job script file.
 
     Note:
         See https://fastapi.tiangolo.com/advanced/custom-response/#streamingresponse
     """
@@ -293,29 +297,31 @@
     description="Endpoint to upload a file to a job script file",
 )
 async def job_script_upload_file(
     id: int = Path(...),
     file_type: FileType = Path(...),
     upload_file: UploadFile = File(..., description="File to upload"),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_CREATE, ensure_email=True)
     ),
 ):
     """Upload a file to a job script."""
     if upload_file.filename is None:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail="The upload file has no filename",
         )
 
     logger.debug(f"Uploading file {upload_file.filename} to job script {id=}")
 
-    job_script = await secure_services.crud.job_script.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    job_script = await secure_services.crud.job_script.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_script.ensure_attribute(
+            job_script, owner_email=secure_services.identity_payload.email
+        )
 
     await secure_services.file.job_script.upsert(
         parent_id=job_script.id,
         filename=upload_file.filename,
         upload_content=upload_file,
         file_type=file_type,
     )
@@ -326,34 +332,36 @@
     status_code=status.HTTP_200_OK,
     description="Endpoint to delete a file from a job script",
 )
 async def job_script_delete_file(
     id: int = Path(...),
     file_name: str = Path(...),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SCRIPTS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SCRIPTS_DELETE, ensure_email=True)
     ),
 ):
     """Delete a file from a job script template by id or identifier."""
-    job_script = await secure_services.crud.job_script.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    job_script = await secure_services.crud.job_script.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_script.ensure_attribute(
+            job_script, owner_email=secure_services.identity_payload.email
+        )
     job_script_file = await secure_services.file.job_script.get(job_script.id, file_name)
     await secure_services.file.job_script.delete(job_script_file)
 
 
 @router.delete(
     "/upload/garbage-collector",
     status_code=status.HTTP_202_ACCEPTED,
     description="Endpoint to delete all unused files from the job script file storage",
     tags=["Garbage collector"],
 )
 def job_script_garbage_collector(
     background_tasks: BackgroundTasks,
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_EDIT)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SCRIPTS_DELETE)),
 ):
     """Delete all unused files from job scripts on the file storage."""
     logger.info("Starting garbage collection from jobbergate file storage")
     background_tasks.add_task(
         garbage_collect,
         secure_services.session,
         secure_services.bucket,
```

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/services.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/tools.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     status_code=status.HTTP_201_CREATED,
     description="Endpoint for job_submission creation",
     response_model=JobSubmissionDetailedView,
 )
 async def job_submission_create(
     create_request: JobSubmissionCreateRequest,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_CREATE, ensure_email=True)
     ),
 ):
     """
     Create a new job submission.
 
     Make a post request to this endpoint with the required values to create a new job submission.
     """
@@ -90,15 +90,15 @@
 @router.get(
     "/{id}",
     description="Endpoint to get a job_submission",
     response_model=JobSubmissionDetailedView,
 )
 async def job_submission_get(
     id: int = Path(...),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SUBMISSIONS_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SUBMISSIONS_READ, commit=False)),
 ):
     """Return the job_submission given it's id."""
     logger.debug(f"Getting job submission {id=}")
     return await secure_services.crud.job_submission.get(id)
 
 
 @router.get(
@@ -116,15 +116,15 @@
         None,
         description="Limit results to those with matching status",
     ),
     from_job_script_id: int | None = Query(
         None,
         description="Filter job-submissions by the job-script-id they were created from.",
     ),
-    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SUBMISSIONS_VIEW, commit=False)),
+    secure_services: SecureService = Depends(secure_services(Permissions.JOB_SUBMISSIONS_READ, commit=False)),
 ):
     """List job_submissions for the authenticated user."""
     logger.debug("Fetching job submissions")
 
     list_kwargs = list_params.dict(exclude_unset=True, exclude={"user_only", "include_archived"})
 
     if list_params.user_only:
@@ -151,59 +151,63 @@
     "/{id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job submission",
 )
 async def job_submission_delete(
     id: int = Path(..., description="id of the job submission to delete"),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_DELETE, ensure_email=True)
     ),
 ):
     """Delete job_submission given its id."""
     logger.info(f"Deleting job submission {id=}")
-    await secure_services.crud.job_submission.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    instance = await secure_services.crud.job_submission.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_submission.ensure_attribute(
+            instance, owner_email=secure_services.identity_payload.email
+        )
     await secure_services.crud.job_submission.delete(id)
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.put(
     "/{id}",
     status_code=status.HTTP_200_OK,
     description="Endpoint to update a job_submission given the id",
     response_model=JobSubmissionDetailedView,
 )
 async def job_submission_update(
     update_params: JobSubmissionUpdateRequest,
     id: int = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_email=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_UPDATE, ensure_email=True)
     ),
 ):
     """Update a job_submission given its id."""
     logger.debug(f"Updating {id=} with {update_params=}")
-    await secure_services.crud.job_submission.get(
-        id, ensure_attributes={"owner_email": secure_services.identity_payload.email}
-    )
+    instance = await secure_services.crud.job_submission.get(id)
+    if Permissions.ADMIN not in secure_services.identity_payload.permissions:
+        secure_services.crud.job_submission.ensure_attribute(
+            instance, owner_email=secure_services.identity_payload.email
+        )
     return await secure_services.crud.job_submission.update(id, **update_params.dict(exclude_unset=True))
 
 
 # The "agent" routes are used for agents to fetch pending job submissions and update their statuses
 @router.put(
     "/agent/{id}",
     status_code=status.HTTP_202_ACCEPTED,
     description="Endpoint for an agent to update the status of a job_submission",
     tags=["Agent"],
 )
 async def job_submission_agent_update(
     update_params: JobSubmissionAgentUpdateRequest,
     id: int = Path(),
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_client_id=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_UPDATE, ensure_client_id=True)
     ),
 ):
     """
     Update a job_submission with slurm_job_state and slurm_job_info.
 
     Note that if the new slurm_job_state is a termination state, the job submission status will be updated.
     """
@@ -263,15 +267,15 @@
     description="Endpoint to report that a pending job_submission was submitted",
     tags=["Agent"],
     status_code=status.HTTP_202_ACCEPTED,
 )
 async def job_submissions_agent_submitted(
     submitted_request: JobSubmissionAgentSubmittedRequest,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_client_id=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_UPDATE, ensure_client_id=True)
     ),
 ):
     """Update a job_submission to indicate that it was submitted to Slurm."""
     logger.debug("Agent is reporting that a pending job has been submitted")
 
     job_submission = await secure_services.crud.job_submission.get(
         submitted_request.id, ensure_attributes={"client_id": secure_services.identity_payload.client_id}
@@ -300,15 +304,15 @@
     description="Endpoint to report that a pending job_submission was rejected by Slurm",
     tags=["Agent"],
     status_code=status.HTTP_202_ACCEPTED,
 )
 async def job_submissions_agent_rejected(
     rejected_request: JobSubmissionAgentRejectedRequest,
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_EDIT, ensure_client_id=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_UPDATE, ensure_client_id=True)
     ),
 ):
     """Update a job_submission to indicate that it was rejected by Slurm."""
     logger.debug("Agent is reporting that a pending job has been rejected")
 
     job_submission = await secure_services.crud.job_submission.get(
         rejected_request.id, ensure_attributes={"client_id": secure_services.identity_payload.client_id}
@@ -345,15 +349,15 @@
     description="Endpoint to list pending job_submissions for the requesting client",
     response_model=Page[PendingJobSubmission],
     response_model_exclude_none=True,
     tags=["Agent"],
 )
 async def job_submissions_agent_pending(
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_VIEW, commit=False, ensure_client_id=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_READ, commit=False, ensure_client_id=True)
     ),
 ):
     """Get a list of pending job submissions for the cluster-agent."""
     logger.debug("Agent is requesting a list of pending job submissions")
 
     client_id = secure_services.identity_payload.client_id
 
@@ -371,15 +375,15 @@
     "/agent/active",
     description="Endpoint to list active job_submissions for the requesting client",
     response_model=Page[ActiveJobSubmission],
     tags=["Agent"],
 )
 async def job_submissions_agent_active(
     secure_services: SecureService = Depends(
-        secure_services(Permissions.JOB_SUBMISSIONS_VIEW, commit=False, ensure_client_id=True)
+        secure_services(Permissions.JOB_SUBMISSIONS_READ, commit=False, ensure_client_id=True)
     ),
 ):
     """Get a list of active job submissions for the cluster-agent."""
     logger.debug("Agent is requesting a list of active job submissions")
 
     client_id = secure_services.identity_payload.client_id
```

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/services.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/job_submissions/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/models.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/schemas.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/apps/services.py` & `jobbergate_api-5.2.0a0/jobbergate_api/apps/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/config.py` & `jobbergate_api-5.2.0a0/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/email_notification.py` & `jobbergate_api-5.2.0a0/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/logging.py` & `jobbergate_api-5.2.0a0/jobbergate_api/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/main.py` & `jobbergate_api-5.2.0a0/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/meta_mapper.py` & `jobbergate_api-5.2.0a0/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/rabbitmq_notification.py` & `jobbergate_api-5.2.0a0/jobbergate_api/rabbitmq_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/safe_types.py` & `jobbergate_api-5.2.0a0/jobbergate_api/safe_types.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/security.py` & `jobbergate_api-5.2.0a0/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/storage.py` & `jobbergate_api-5.2.0a0/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/jobbergate_api/version.py` & `jobbergate_api-5.2.0a0/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.1.0a0/pyproject.toml` & `jobbergate_api-5.2.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "5.1.0a0"
+version = "5.2.0a0"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-5.1.0a0/PKG-INFO` & `jobbergate_api-5.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 5.1.0a0
+Version: 5.2.0a0
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

