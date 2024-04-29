# Comparing `tmp/license_manager_backend-3.1.1.tar.gz` & `tmp/license_manager_backend-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_backend-3.1.1.tar", max compression
+gzip compressed data, was "license_manager_backend-3.2.0.tar", max compression
```

## Comparing `license_manager_backend-3.1.1.tar` & `license_manager_backend-3.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1829 2024-03-26 20:29:51.168266 license_manager_backend-3.1.1/README.md
--rw-r--r--   0        0        0       60 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/__init__.py
--rw-r--r--   0        0        0      929 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/cruds/__init__.py
--rw-r--r--   0        0        0     3078 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/cruds/booking.py
--rw-r--r--   0        0        0     2157 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/cruds/configuration.py
--rw-r--r--   0        0        0     6451 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/cruds/feature.py
--rw-r--r--   0        0        0     6101 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/cruds/generic.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/__init__.py
--rw-r--r--   0        0        0     1362 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/booking.py
--rw-r--r--   0        0        0     1703 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/configuration.py
--rw-r--r--   0        0        0      575 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/crud_base.py
--rw-r--r--   0        0        0     1992 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/feature.py
--rw-r--r--   0        0        0     1216 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/job.py
--rw-r--r--   0        0        0     1080 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/license_server.py
--rw-r--r--   0        0        0      777 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/models/product.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/__init__.py
--rw-r--r--   0        0        0     2112 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/bookings.py
--rw-r--r--   0        0        0     9370 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/configurations.py
--rw-r--r--   0        0        0     3661 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/features.py
--rw-r--r--   0        0        0     6990 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/jobs.py
--rw-r--r--   0        0        0     3361 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/license_servers.py
--rw-r--r--   0        0        0     2689 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/routes/products.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/__init__.py
--rw-r--r--   0        0        0      313 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/base.py
--rw-r--r--   0        0        0     1797 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/booking.py
--rw-r--r--   0        0        0     6361 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/configuration.py
--rw-r--r--   0        0        0     5736 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/feature.py
--rw-r--r--   0        0        0     3600 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/job.py
--rw-r--r--   0        0        0     4420 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/license_server.py
--rw-r--r--   0        0        0      984 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/api/schemas/product.py
--rw-r--r--   0        0        0     1821 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/config.py
--rw-r--r--   0        0        0      489 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/constants.py
--rw-r--r--   0        0        0     7202 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/database.py
--rw-r--r--   0        0        0     2850 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/main.py
--rw-r--r--   0        0        0      865 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/permissions.py
--rw-r--r--   0        0        0     3348 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/security.py
--rw-r--r--   0        0        0     1099 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/lm_api/version.py
--rw-r--r--   0        0        0     2015 2024-03-26 20:29:51.172266 license_manager_backend-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 license_manager_backend-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1829 2024-04-29 19:53:20.531443 license_manager_backend-3.2.0/README.md
+-rw-r--r--   0        0        0       60 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/booking.py
+-rw-r--r--   0        0        0     2157 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/configuration.py
+-rw-r--r--   0        0        0     6451 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/feature.py
+-rw-r--r--   0        0        0     6101 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/cruds/generic.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/__init__.py
+-rw-r--r--   0        0        0     1362 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/booking.py
+-rw-r--r--   0        0        0     1703 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/configuration.py
+-rw-r--r--   0        0        0      575 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/crud_base.py
+-rw-r--r--   0        0        0     1992 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/feature.py
+-rw-r--r--   0        0        0     1216 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/job.py
+-rw-r--r--   0        0        0     1080 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/license_server.py
+-rw-r--r--   0        0        0      777 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/models/product.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/__init__.py
+-rw-r--r--   0        0        0     2220 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/bookings.py
+-rw-r--r--   0        0        0     9532 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/configurations.py
+-rw-r--r--   0        0        0     3811 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/features.py
+-rw-r--r--   0        0        0     7185 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/jobs.py
+-rw-r--r--   0        0        0     3565 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/license_servers.py
+-rw-r--r--   0        0        0     2818 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/routes/products.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/base.py
+-rw-r--r--   0        0        0     1797 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/booking.py
+-rw-r--r--   0        0        0     6361 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/configuration.py
+-rw-r--r--   0        0        0     5736 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/feature.py
+-rw-r--r--   0        0        0     3600 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/job.py
+-rw-r--r--   0        0        0     4420 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/license_server.py
+-rw-r--r--   0        0        0      984 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/api/schemas/product.py
+-rw-r--r--   0        0        0     1821 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/config.py
+-rw-r--r--   0        0        0      489 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/constants.py
+-rw-r--r--   0        0        0     7203 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/database.py
+-rw-r--r--   0        0        0     2850 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/main.py
+-rw-r--r--   0        0        0     1481 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/permissions.py
+-rw-r--r--   0        0        0     3349 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/security.py
+-rw-r--r--   0        0        0     1099 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/lm_api/version.py
+-rw-r--r--   0        0        0     2021 2024-04-29 19:53:20.535443 license_manager_backend-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 license_manager_backend-3.2.0/PKG-INFO
```

### Comparing `license_manager_backend-3.1.1/README.md` & `license_manager_backend-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/__init__.py` & `license_manager_backend-3.2.0/lm_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/cruds/booking.py` & `license_manager_backend-3.2.0/lm_api/api/cruds/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/cruds/configuration.py` & `license_manager_backend-3.2.0/lm_api/api/cruds/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/cruds/feature.py` & `license_manager_backend-3.2.0/lm_api/api/cruds/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/cruds/generic.py` & `license_manager_backend-3.2.0/lm_api/api/cruds/generic.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/booking.py` & `license_manager_backend-3.2.0/lm_api/api/models/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/configuration.py` & `license_manager_backend-3.2.0/lm_api/api/models/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/crud_base.py` & `license_manager_backend-3.2.0/lm_api/api/models/crud_base.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/feature.py` & `license_manager_backend-3.2.0/lm_api/api/models/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/job.py` & `license_manager_backend-3.2.0/lm_api/api/models/job.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/license_server.py` & `license_manager_backend-3.2.0/lm_api/api/models/license_server.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/models/product.py` & `license_manager_backend-3.2.0/lm_api/api/models/product.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/bookings.py` & `license_manager_backend-3.2.0/lm_api/api/routes/bookings.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 @router.post(
     "",
     response_model=BookingSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_booking(
     booking: BookingCreateSchema = Body(..., description="Booking to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.BOOKING_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.BOOKING_CREATE)),
 ):
     """Create a new booking."""
     return await crud_booking.create(db_session=secure_session.session, obj=booking)
 
 
 @router.get(
     "",
     response_model=List[BookingSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_bookings(
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.BOOKING_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.BOOKING_READ, commit=False)
+    ),
 ):
     """Return all bookings."""
     return await crud_booking.read_all(
         db_session=secure_session.session,
         sort_field=sort_field,
         sort_ascending=sort_ascending,
     )
@@ -48,23 +50,25 @@
 @router.get(
     "/{booking_id}",
     response_model=BookingSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_booking(
     booking_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.BOOKING_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.BOOKING_READ, commit=False)
+    ),
 ):
     """Return a booking with associated bookings with the given id."""
     return await crud_booking.read(db_session=secure_session.session, id=booking_id)
 
 
 @router.delete(
     "/{booking_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_booking(
     booking_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.BOOKING_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.BOOKING_DELETE)),
 ):
     """Delete a booking from the database."""
     return await crud_booking.delete(db_session=secure_session.session, id=booking_id)
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/configurations.py` & `license_manager_backend-3.2.0/lm_api/api/routes/configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @router.post(
     "",
     response_model=ConfigurationSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_configuration(
     configuration: ConfigurationCompleteCreateSchema = Body(..., description="Configuration to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.CONFIG_CREATE)),
 ):
     """
     Create a new configuration.
 
     The features for the configuration will be specified in the request body.
     If the feature's product doesn't exist, it will be created.
     """
@@ -91,15 +91,17 @@
     response_model=List[ConfigurationSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_configurations(
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.CONFIG_READ, commit=False)
+    ),
 ):
     """Return all configurations with the associated license servers and features."""
     return await crud_configuration.read_all(
         db_session=secure_session.session,
         search=search,
         sort_field=sort_field,
         sort_ascending=sort_ascending,
@@ -108,15 +110,17 @@
 
 @router.get(
     "/by_client_id",
     response_model=List[ConfigurationSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_configurations_by_client_id(
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.CONFIG_READ, commit=False)
+    ),
 ):
     """Return the configurations with the specified client_id."""
     client_id = secure_session.identity_payload.client_id
 
     if not client_id:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
@@ -131,15 +135,17 @@
 @router.get(
     "/{configuration_id}",
     response_model=ConfigurationSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_configuration(
     configuration_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.CONFIG_READ, commit=False)
+    ),
 ):
     """Return a configuration with the associated license severs and features with a given id."""
     return await crud_configuration.read(
         db_session=secure_session.session, id=configuration_id, force_refresh=True
     )
 
 
@@ -147,15 +153,15 @@
     "/{configuration_id}",
     response_model=ConfigurationSchema,
     status_code=status.HTTP_200_OK,
 )
 async def update_configuration(
     configuration_id: int,
     configuration_update: ConfigurationCompleteUpdateSchema,
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.CONFIG_UPDATE)),
 ):
     """
     Update a configuration in the database.
 
     If there are features in the payload, they'll be updated if they have an id,
     or they will be created if the id is None.
 
@@ -235,15 +241,15 @@
 
 @router.delete(
     "/{configuration_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_configuration(
     configuration_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.CONFIG_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.CONFIG_DELETE)),
 ):
     """
     Delete a configuration from the database.
 
     This will also delete the features and license servers associated.
     """
     return await crud_configuration.delete(db_session=secure_session.session, id=configuration_id)
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/features.py` & `license_manager_backend-3.2.0/lm_api/api/routes/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,32 @@
 @router.post(
     "",
     response_model=FeatureSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_feature(
     feature: FeatureCreateSchema = Body(..., description="Feature to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.FEATURE_CREATE)),
 ):
     """Create a new feature"""
     return await crud_feature.create(db_session=secure_session.session, obj=feature)
 
 
 @router.get(
     "",
     response_model=List[FeatureSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_features(
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.FEATURE_READ, commit=False)
+    ),
 ):
     """Return all features with associated bookings."""
     return await crud_feature.read_all(
         db_session=secure_session.session,
         search=search,
         sort_field=sort_field,
         sort_ascending=sort_ascending,
@@ -54,27 +56,29 @@
 @router.get(
     "/{feature_id}",
     response_model=FeatureSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_feature(
     feature_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.FEATURE_READ, commit=False)
+    ),
 ):
     """Return a feature with associated bookings with the given id."""
     return await crud_feature.read(db_session=secure_session.session, id=feature_id)
 
 
 @router.put(
     "/bulk",
     status_code=status.HTTP_200_OK,
 )
 async def bulk_update_feature(
     features: List[FeatureUpdateByNameSchema],
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.FEATURE_UPDATE)),
 ):
     """
     Update a list of features in the database using the name of each feature.
     Since the name is not unique across clusters, the client_id
     in the token is used to identify the cluster.
     """
     client_id = secure_session.identity_payload.client_id
@@ -98,15 +102,15 @@
     "/{feature_id}",
     response_model=FeatureSchema,
     status_code=status.HTTP_200_OK,
 )
 async def update_feature(
     feature_id: int,
     feature_update: FeatureUpdateSchema,
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.FEATURE_UPDATE)),
 ):
     """Update a feature in the database."""
     return await crud_feature.update(
         db_session=secure_session.session,
         id=feature_id,
         obj=feature_update,
     )
@@ -114,13 +118,13 @@
 
 @router.delete(
     "/{feature_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_feature(
     feature_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.FEATURE_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.FEATURE_DELETE)),
 ):
     """
     Delete a feature from the database.
     """
     return await crud_feature.delete(db_session=secure_session.session, id=feature_id)
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/jobs.py` & `license_manager_backend-3.2.0/lm_api/api/routes/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @router.post(
     "",
     response_model=JobSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_job(
     job: JobWithBookingCreateSchema = Body(..., description="Job to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.JOB_CREATE)),
 ):
     """Create a new job."""
     client_id = secure_session.identity_payload.client_id
 
     if not client_id:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
@@ -76,15 +76,17 @@
 
 @router.get(
     "/by_client_id",
     response_model=List[JobSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_jobs_by_client_id(
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.JOB_READ, commit=False)
+    ),
 ):
     """Return the jobs with the specified OIDC client_id retrieved from the request."""
     client_id = secure_session.identity_payload.client_id
 
     if not client_id:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
@@ -101,15 +103,17 @@
     response_model=List[JobSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_jobs(
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.JOB_READ, commit=False)
+    ),
 ):
     """Return all jobs."""
     return await crud_job.read_all(
         db_session=secure_session.session,
         search=search,
         sort_field=sort_field,
         sort_ascending=sort_ascending,
@@ -119,39 +123,41 @@
 @router.get(
     "/{job_id}",
     response_model=JobSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_job(
     job_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.JOB_READ, commit=False)
+    ),
 ):
     """Return a job with associated bookings with the given id."""
     return await crud_job.read(db_session=secure_session.session, id=job_id, force_refresh=True)
 
 
 @router.delete(
     "/{job_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_job(
     job_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.JOB_DELETE)),
 ):
     """Delete a job from the database and associated bookings."""
     return await crud_job.delete(db_session=secure_session.session, id=job_id)
 
 
 @router.delete(
     "/slurm_job_id/{slurm_job_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_job_by_slurm_id(
     slurm_job_id: str,
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.JOB_DELETE)),
 ):
     """
     Delete a job from the database and associated bookings.
 
     Uses the slurm_job_id and the cluster client_id to filter the job.
 
     Since the slurm_job_id can be the same across clusters, we need the cluster client_id to validate.
@@ -178,15 +184,17 @@
 @router.get(
     "/slurm_job_id/{slurm_job_id}",
     response_model=JobSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_job_by_slurm_id(
     slurm_job_id: str,
-    secure_session: SecureSession = Depends(secure_session(Permissions.JOB_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.JOB_READ, commit=False)
+    ),
 ):
     """
     Read a job from the database and associated bookings.
 
     Uses the slurm_job_id and the cluster client_id to filter the job.
 
     Since the slurm_job_id can be the same across clusters, we need the cluster client_id to validate.
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/license_servers.py` & `license_manager_backend-3.2.0/lm_api/api/routes/license_servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,72 +21,82 @@
 
 @router.get(
     "/types/",
     status_code=status.HTTP_200_OK,
     response_model=List[LicenseServerType],
 )
 async def get_license_server_types(
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_READ, commit=False)
+    ),
 ):
     """Return a list of the available license server types."""
     return list(LicenseServerType)
 
 
 @router.post(
     "",
     response_model=LicenseServerSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_license_server(
     license_server: LicenseServerCreateSchema = Body(..., description="License server to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_EDIT)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_CREATE)
+    ),
 ):
     """Create a new license server."""
     return await crud_license_server.create(db_session=secure_session.session, obj=license_server)
 
 
 @router.get(
     "",
     response_model=List[LicenseServerSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_license_servers(
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_READ, commit=False)
+    ),
 ):
     """Return all license servers."""
     return await crud_license_server.read_all(
         db_session=secure_session.session, search=search, sort_field=sort_field, sort_ascending=sort_ascending
     )
 
 
 @router.get(
     "/{license_server_id}",
     response_model=LicenseServerSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_license_server(
     license_server_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_READ, commit=False)
+    ),
 ):
     """Return a license server with the given id."""
     return await crud_license_server.read(db_session=secure_session.session, id=license_server_id)
 
 
 @router.put(
     "/{license_server_id}",
     response_model=LicenseServerSchema,
     status_code=status.HTTP_200_OK,
 )
 async def update_license_server(
     license_server_id: int,
     license_server_update: LicenseServerUpdateSchema,
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_EDIT)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_UPDATE)
+    ),
 ):
     """Update a license server in the database."""
     return await crud_license_server.update(
         db_session=secure_session.session,
         id=license_server_id,
         obj=license_server_update,
     )
@@ -94,11 +104,13 @@
 
 @router.delete(
     "/{license_server_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_license_server(
     license_server_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.LICENSE_SERVER_EDIT)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.LICENSE_SERVER_DELETE)
+    ),
 ):
     """Delete a license server from the database."""
     return await crud_license_server.delete(db_session=secure_session.session, id=license_server_id)
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/routes/products.py` & `license_manager_backend-3.2.0/lm_api/api/routes/products.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,59 +17,63 @@
 @router.post(
     "",
     response_model=ProductSchema,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_product(
     product: ProductCreateSchema = Body(..., description="Product to be created"),
-    secure_session: SecureSession = Depends(secure_session(Permissions.PRODUCT_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.PRODUCT_CREATE)),
 ):
     """Create a new product."""
     return await crud_product.create(db_session=secure_session.session, obj=product)
 
 
 @router.get(
     "",
     response_model=List[ProductSchema],
     status_code=status.HTTP_200_OK,
 )
 async def read_all_products(
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
     sort_ascending: bool = Query(True),
-    secure_session: SecureSession = Depends(secure_session(Permissions.PRODUCT_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.PRODUCT_READ, commit=False)
+    ),
 ):
     """Return all products with associated features."""
     return await crud_product.read_all(
         db_session=secure_session.session, search=search, sort_field=sort_field, sort_ascending=sort_ascending
     )
 
 
 @router.get(
     "/{product_id}",
     response_model=ProductSchema,
     status_code=status.HTTP_200_OK,
 )
 async def read_product(
     product_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.PRODUCT_VIEW, commit=False)),
+    secure_session: SecureSession = Depends(
+        secure_session(Permissions.ADMIN, Permissions.PRODUCT_READ, commit=False)
+    ),
 ):
     """Return a product with associated features with the given id."""
     return await crud_product.read(db_session=secure_session.session, id=product_id)
 
 
 @router.put(
     "/{product_id}",
     response_model=ProductSchema,
     status_code=status.HTTP_200_OK,
 )
 async def update_product(
     product_id: int,
     product_update: ProductUpdateSchema,
-    secure_session: SecureSession = Depends(secure_session(Permissions.PRODUCT_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.PRODUCT_UPDATE)),
 ):
     """Update a product in the database."""
     return await crud_product.update(
         db_session=secure_session.session,
         id=product_id,
         obj=product_update,
     )
@@ -77,11 +81,11 @@
 
 @router.delete(
     "/{product_id}",
     status_code=status.HTTP_200_OK,
 )
 async def delete_product(
     product_id: int,
-    secure_session: SecureSession = Depends(secure_session(Permissions.PRODUCT_EDIT)),
+    secure_session: SecureSession = Depends(secure_session(Permissions.ADMIN, Permissions.PRODUCT_DELETE)),
 ):
     """Delete a product from the database and associated features."""
     return await crud_product.delete(db_session=secure_session.session, id=product_id)
```

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/booking.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/configuration.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/configuration.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/feature.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/feature.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/job.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/license_server.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/license_server.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/api/schemas/product.py` & `license_manager_backend-3.2.0/lm_api/api/schemas/product.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/config.py` & `license_manager_backend-3.2.0/lm_api/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/database.py` & `license_manager_backend-3.2.0/lm_api/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     Provide a container class for an IdentityPayload and AsyncSesson for the current request.
     """
 
     identity_payload: IdentityPayload
     session: AsyncSession
 
 
-def secure_session(*scopes: str, permission_mode: PermissionMode = PermissionMode.ALL, commit: bool = True):
+def secure_session(*scopes: str, permission_mode: PermissionMode = PermissionMode.SOME, commit: bool = True):
     """
     Provide an injectable for FastAPI that checks permissions and returns a database session for this request.
 
     This should be used for all secured routes that need access to the database. It will commit the
     transaction upon completion of the request. If an exception occurs, it will rollback the transaction.
     If multi-tenancy is enabled, it will retrieve a database session for the database associated with the
     client_id found in the requesting user's auth token.
```

### Comparing `license_manager_backend-3.1.1/lm_api/main.py` & `license_manager_backend-3.2.0/lm_api/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/lm_api/security.py` & `license_manager_backend-3.2.0/lm_api/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             **values,
             "organization_id": next(iter(organization_payload))
             if isinstance(organization_payload, dict)
             else organization_payload,
         }
 
 
-def lockdown_with_identity(*scopes: str, permission_mode: PermissionMode = PermissionMode.ALL):
+def lockdown_with_identity(*scopes: str, permission_mode: PermissionMode = PermissionMode.SOME):
     """
     Provide a wrapper to be used with dependency injection to extract identity on a secured route.
     """
 
     def dependency(
         token_payload: TokenPayload = Depends(guard.lockdown(*scopes, permission_mode=permission_mode)),
     ) -> IdentityPayload:
```

### Comparing `license_manager_backend-3.1.1/lm_api/version.py` & `license_manager_backend-3.2.0/lm_api/version.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-3.1.1/pyproject.toml` & `license_manager_backend-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "license-manager-backend"
-version = "3.1.1"
+version = "3.2.0"
 description = "Provides an API for managing license data"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-fastapi = "^0.68.0"
+fastapi = ">=0.68,<0.110"
 sentry-sdk = "1.18.0"
 jwt = {version = "^1.2.0", optional = true}
 SQLAlchemy-Utils = "^0.37.8"
 loguru = "^0.5.3"
 asyncpg = "^0.28"
 uvicorn = "^0.15.0"
 python-dotenv = "^0.19.0"
```

### Comparing `license_manager_backend-3.1.1/PKG-INFO` & `license_manager_backend-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: license-manager-backend
-Version: 3.1.1
+Version: 3.2.0
 Summary: Provides an API for managing license data
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy-Utils (>=0.37.8,<0.38.0)
 Requires-Dist: SQLAlchemy[mypy] (>=2.0.22,<3.0.0)
 Requires-Dist: armasec (>=0.11,<0.12)
 Requires-Dist: asyncpg (>=0.28,<0.29)
-Requires-Dist: fastapi (>=0.68.0,<0.69.0)
+Requires-Dist: fastapi (>=0.68,<0.110)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: py-buzz (>=3.2.1,<4.0.0)
 Requires-Dist: pydantic[email] (>=1,<2)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
```

