# Comparing `tmp/license_manager_agent-3.1.1.tar.gz` & `tmp/license_manager_agent-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-3.1.1.tar", max compression
+gzip compressed data, was "license_manager_agent-3.2.0.tar", max compression
```

## Comparing `license_manager_agent-3.1.1.tar` & `license_manager_agent-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0     1911 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/backend_utils/__init__.py
--rw-r--r--   0        0        0      288 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/backend_utils/constants.py
--rw-r--r--   0        0        0     1808 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/backend_utils/models.py
--rw-r--r--   0        0        0     9831 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/backend_utils/utils.py
--rw-r--r--   0        0        0     3473 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/config.py
--rw-r--r--   0        0        0     1150 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/exceptions.py
--rw-r--r--   0        0        0     4427 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/license_report.py
--rw-r--r--   0        0        0     2519 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     1732 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3537 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4428 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4758 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     3265 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1054 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/reconcile.py
--rw-r--r--   0        0        0     8996 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/reconciliation.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     2844 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1620 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2745 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2711 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2703 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     2638 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0     1251 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0     8894 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0     1036 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3732 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     1524 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3921 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     1825 2024-03-26 20:29:53.065479 license_manager_agent-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1911 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/constants.py
+-rw-r--r--   0        0        0     1808 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/models.py
+-rw-r--r--   0        0        0     9582 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/utils.py
+-rw-r--r--   0        0        0     3473 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/config.py
+-rw-r--r--   0        0        0     1150 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     2519 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     4942 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3953 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4521 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4860 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     3405 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1063 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/reconcile.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     3002 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1871 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2844 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2810 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2802 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     2737 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/__init__.py
+-rw-r--r--   0        0        0     9881 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/clean_jobs_and_bookings.py
+-rw-r--r--   0        0        0     4721 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/license_report.py
+-rw-r--r--   0        0        0      496 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/models.py
+-rw-r--r--   0        0        0     6323 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/reconciliation.py
+-rw-r--r--   0        0        0     1269 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     8894 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0     1036 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3732 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1610 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3939 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     1825 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.2.0/PKG-INFO
```

### Comparing `license_manager_agent-3.1.1/README.md` & `license_manager_agent-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/backend_utils/models.py` & `license_manager_agent-3.2.0/lm_agent/backend_utils/models.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/backend_utils/utils.py` & `license_manager_agent-3.2.0/lm_agent/backend_utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import getpass
 from typing import Dict, List, Optional, Union
 
 import httpx
 import jwt
 
 from lm_agent.backend_utils.models import (
-    BookingSchema,
     ConfigurationSchema,
     FeatureSchema,
     JobSchema,
     LicenseBookingRequest,
 )
 from lm_agent.config import settings
 from lm_agent.exceptions import (
@@ -173,29 +172,14 @@
         "Could not parse configuration data returned from the backend", do_except=log_error
     ):
         configurations = [ConfigurationSchema.parse_obj(configuration) for configuration in parsed_resp]
 
     return configurations
 
 
-async def get_cluster_grace_times() -> Dict[int, int]:
-    """
-    Get the grace time for each feature_id in the cluster.
-    """
-    cluster_configurations = await get_cluster_configs_from_backend()
-
-    grace_times = {
-        feature.id: configuration.grace_time
-        for configuration in cluster_configurations
-        for feature in configuration.features
-    }
-
-    return grace_times
-
-
 async def make_feature_update(features_to_update: List[Dict]):
     """
     Update the feature with its current counters.
     """
     async with AsyncBackendClient() as backend_client:
         features_response = await backend_client.put(
             "/lm/features/bulk",
@@ -215,15 +199,15 @@
             "/lm/jobs",
             json=lbr.dict(),
         )
         if job_response.status_code != 201:
             logger.error(f"Failed to create booking: {job_response.text}")
             return False
 
-    logger.debug("##### Booking completed successfully #####")
+    logger.debug(f"##### Job {lbr.slurm_job_id} created successfully #####")
     return True
 
 
 async def remove_job_by_slurm_job_id(slurm_job_id: str):
     """
     Remove the job with its bookings for the given slurm_job_id in the cluster.
 
@@ -232,26 +216,29 @@
     async with AsyncBackendClient() as backend_client:
         resp = await backend_client.delete(f"lm/jobs/slurm_job_id/{slurm_job_id}")
 
         LicenseManagerBackendConnectionError.require_condition(
             resp.status_code in [200, 404], f"Failed to remove job: {resp.text}"
         )
 
-    logger.debug("##### Job removed successfully #####")
+    logger.debug(f"##### Job {slurm_job_id} removed successfully #####")
 
 
-async def get_bookings_for_all_jobs() -> Dict[str, List[BookingSchema]]:
+async def remove_booking(booking_id: int):
     """
-    Return the bookings for all jobs in the cluster.
+    Remove the booking with the given id.
     """
-    jobs = await get_cluster_jobs_from_backend()
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.delete(f"lm/bookings/{booking_id}")
 
-    bookings_for_all_jobs = {job.slurm_job_id: job.bookings for job in jobs}
+    LicenseManagerBackendConnectionError.require_condition(
+        resp.status_code == 200, f"Failed to remove booking: {resp.text}"
+    )
 
-    return bookings_for_all_jobs
+    logger.debug(f"##### Booking {booking_id} removed successfully")
 
 
 async def get_all_features_from_backend() -> List[FeatureSchema]:
     """
     Return the job with its bookings for the given job_id in the cluster.
     """
     async with AsyncBackendClient() as backend_client:
```

### Comparing `license_manager_agent-3.1.1/lm_agent/config.py` & `license_manager_agent-3.2.0/lm_agent/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/exceptions.py` & `license_manager_agent-3.2.0/lm_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/license_report.py` & `license_manager_agent-3.2.0/lm_agent/services/license_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,39 +72,51 @@
         lmx=LMXLicenseServer,
         olicense=OLicenseLicenseServer,
     )
 
     for entry in filtered_entries:
         product_features_to_check = []
         for feature in entry.features:
-            product_feature = f"{feature.product.name}.{feature.name}"
-            product_features_to_check.append(product_feature)
+            feature_info = (feature.id, f"{feature.product.name}.{feature.name}")
+            product_features_to_check.append(feature_info)
 
         logger.debug("### Features to check: ")
         logger.debug(product_features_to_check)
 
         server_type = server_type_map.get(entry.type)
 
         if server_type is None:
             raise LicenseManagerNonSupportedServerTypeError("License server type not supported.")
 
         license_server_interface = server_type(entry.license_servers)
 
-        for product_feature in product_features_to_check:
-            get_report_awaitables.append(license_server_interface.get_report_item(product_feature))
-            product_features_awaited.append(product_feature)
+        for feature_info_to_check in product_features_to_check:
+            feature_id, product_feature = feature_info_to_check
+
+            get_report_awaitables.append(
+                license_server_interface.get_report_item(feature_id, product_feature)
+            )
+            product_features_awaited.append(feature_info)
 
     results = await asyncio.gather(*get_report_awaitables, return_exceptions=True)
 
-    for result, product_feature in zip(results, product_features_awaited):
+    for result, feature_info in zip(results, product_features_awaited):
+        feature_id, product_feature = feature_info
+
         if isinstance(result, Exception):
             # If the report for a feature failed, the total will set to 0, preventing jobs from running
             logger.error(f"#### Report for feature {product_feature} failed with: {str(result)} ####")
 
-            failed_report_item = LicenseReportItem(product_feature=product_feature, used=0, total=0)
+            failed_report_item = LicenseReportItem(
+                feature_id=feature_id,
+                product_feature=product_feature,
+                used=0,
+                total=0,
+                uses=[],
+            )
             report_items.append(failed_report_item)
             continue
         report_items.append(result)
 
     logger.debug("#### Reconciliation items:")
     logger.debug(report_items)
```

### Comparing `license_manager_agent-3.1.1/lm_agent/logs.py` & `license_manager_agent-3.2.0/lm_agent/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/parsing/lmx.py` & `license_manager_agent-3.2.0/lm_agent/parsing/lmx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 """
 Parser for LM-X
 """
 import re
 from typing import Optional
+from lm_agent.server_interfaces.license_server_interface import LicenseUsesItem
+
 
 HOSTWORD = r"[a-zA-Z0-9-]+"
 HOSTNAME = rf"{HOSTWORD}(\.{HOSTWORD})*"
 INT = r"\d+"
 VERSION = rf"{INT}\.{INT}"
 
 FEATURE_LINE = rf"^Feature: (?P<feature>\w+) Version: (?P<version>{VERSION}) Vendor: (?P<vendor>\S+)$"
 IN_USE_LINE = rf"^(?P<in_use>{INT}) of (?P<total>{INT}) license\(s\) used(:)?$"
-USAGE_LINE = (
+USAGE_LINE_1 = (
     rf"^(?P<in_use>{INT}) license\(s\) "
     rf"used by (?P<user>\S+)@(?P<lead_host>{HOSTNAME}) "
     rf"\[{INT}\.{INT}\.{INT}\.{INT}\]"
 )
+USAGE_LINE_2 = (
+    rf"^(?P<in_use>{INT}) license\(s\) "
+    rf"used by (?P<user>\S+)@(?P<lead_host>{HOSTNAME})_\S+ "
+    rf"\[{INT}\.{INT}\.{INT}\.{INT}\]"
+)
 RX_FEATURE = re.compile(FEATURE_LINE)
 RX_IN_USE = re.compile(IN_USE_LINE)
-RX_USAGE = re.compile(USAGE_LINE)
+RX_USAGE_1 = re.compile(USAGE_LINE_1)
+RX_USAGE_2 = re.compile(USAGE_LINE_2)
+USAGE_LINES = [RX_USAGE_1, RX_USAGE_2]
 
 
 def parse_feature_line(line: str) -> Optional[str]:
     """
     Parse the feature line in the LM-X output.
     Data we need:
     - ``feature``: license name
@@ -53,35 +62,39 @@
 
     return {
         "used": int(in_use_data["in_use"]),
         "total": int(in_use_data["total"]),
     }
 
 
-def parse_usage_line(line: str) -> Optional[dict]:
+def parse_usage_line(line: str) -> Optional[LicenseUsesItem]:
     """
     Parse the usage line in the LS-Dyna output.
     Data we need:
-    -``user_name``: user who booked the license
+    -``username``: user who booked the license
     -``lead_host``: host using the license
     -``booked``: quantity of licenses being used
 
     Obs: this line also doesn't incluse the license name.
     The license in use is the last one parsed before this line.
     """
-    parsed_usage = RX_USAGE.match(line)
+    for RX in USAGE_LINES:
+        parsed_usage = RX.match(line)
+        if parsed_usage:
+            break
+
     if parsed_usage is None:
         return None
     usage_data = parsed_usage.groupdict()
 
-    return {
-        "user_name": usage_data["user"],
-        "lead_host": usage_data["lead_host"],
-        "booked": int(usage_data["in_use"]),
-    }
+    return LicenseUsesItem(
+        username=usage_data["user"].lower(),
+        lead_host=usage_data["lead_host"],
+        booked=int(usage_data["in_use"]),
+    )
 
 
 def parse(server_output: str) -> dict:
     """
     Parse the LM-X output using regex to match the lines we need:
     -``feature line``: info about each license
     -``in use line``: info about licenses in use
```

### Comparing `license_manager_agent-3.1.1/lm_agent/parsing/lsdyna.py` & `license_manager_agent-3.2.0/lm_agent/parsing/lsdyna.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Parser for LS-Dyna
 """
 
 import re
+from lm_agent.server_interfaces.license_server_interface import LicenseUsesItem
+
 
 HOSTWORD = r"[a-zA-Z0-9-]+"
 HOSTNAME = rf"{HOSTWORD}(\.{HOSTWORD})*"
 NONWS = r"\S+"
 INT = r"\d+"
 PROGRAM = r"[A-Z0-9\-_]+"
 EXPIRATION_DATE = r"((0[1-9]|1[012])[\/](0[1-9]|[12][0-9]|3[01])[\/](19|20)\d\d)"
@@ -58,31 +60,31 @@
     }
 
 
 def parse_usage_line(line: str):
     """
     Parse the usage line in the LS-Dyna output.
     Data we need:
-    - ``user_name``: user who booked the license
+    - ``username``: user who booked the license
     - ``lead_host``: host using the license
     - ``booked``: quantity of licenses being used
 
     Obs: this line doesn't include the license name.
     The license in use is the last one parsed before this line.
     """
     parsed_usage = RX_USAGE.match(line)
     if parsed_usage is None:
         return None
     usage_data = parsed_usage.groupdict()
 
-    return {
-        "user_name": usage_data["user"],
-        "lead_host": usage_data["lead_host"],
-        "booked": int(usage_data["used"]),
-    }
+    return LicenseUsesItem(
+        username=usage_data["user"].lower(),
+        lead_host=usage_data["lead_host"],
+        booked=int(usage_data["used"]),
+    )
 
 
 def parse_total_line(line: str):
     """
     Parse the total line in the LS-Dyna output.
     Data we need:
     - ``used``: quantity of licenses being used in the server
```

### Comparing `license_manager_agent-3.1.1/lm_agent/parsing/olicense.py` & `license_manager_agent-3.2.0/lm_agent/parsing/olicense.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Parser for OLicense
 """
 import re
 from typing import Optional
+from lm_agent.server_interfaces.license_server_interface import LicenseUsesItem
+
 
 HOSTWORD = r"[a-zA-Z0-9-]+"
 HOSTNAME = rf"{HOSTWORD}(\.{HOSTWORD})*"
 INT = r"\d+"
 EXPIRATION_DATE = (
     r"[0-9]{4}-(0[1-9]|1[0-2])-(0[1-9]|[1-2][0-9]|3[0-1]) (2[0-3]|[01][0-9]):[0-5][0-9]:[0-5][0-9]"
 )
@@ -14,15 +16,15 @@
 FEATURE_LINE = (
     r"^\s+(?P<feature>\w+);"
     r"\s+(?P<license_type>\w+);"
     rf"\s+(?P<total>{INT});"
     rf"\s+(?P<expiration_date>{EXPIRATION_DATE});"
 )
 
-IN_USE_LINE = rf"^\s+(?P<in_use>{INT})\s+FloatsLockedBy:$"
+IN_USE_LINE = rf"^\s+(?P<in_use>{INT})\s+FloatsLockedBy"
 
 USAGE_LINE = rf"^\s+(?P<user>\S+)@(?P<lead_host>{HOSTNAME})\s+#(?P<booked>{INT})$"
 
 RX_FEATURE = re.compile(FEATURE_LINE)
 RX_IN_USE = re.compile(IN_USE_LINE)
 RX_USAGE = re.compile(USAGE_LINE)
 
@@ -66,35 +68,35 @@
     if parsed_in_use is None:
         return None
     in_use_data = parsed_in_use.groupdict()
 
     return int(in_use_data["in_use"])
 
 
-def parse_usage_line(line: str) -> Optional[dict]:
+def parse_usage_line(line: str) -> Optional[LicenseUsesItem]:
     """
     Parse the usage line in the Olicense output.
     Data we need:
-    -``user_name``: user who booked the license
+    -``username``: user who booked the license
     -``lead_host``: host using the license
     -``booked``: quantity of licenses booked by the user
 
     Obs: this line also doesn't include the license name.
     The license in use is the last one parsed before this line.
     """
     parsed_usage = RX_USAGE.match(line)
     if parsed_usage is None:
         return None
     usage_data = parsed_usage.groupdict()
 
-    return {
-        "user_name": usage_data["user"],
-        "lead_host": usage_data["lead_host"],
-        "booked": int(usage_data["booked"]),
-    }
+    return LicenseUsesItem(
+        username=usage_data["user"].lower(),
+        lead_host=usage_data["lead_host"],
+        booked=int(usage_data["booked"]),
+    )
 
 
 def parse(server_output: str) -> dict:
     """
     Parse the OLicense output using regex to match the lines we need:
     -``feature line``: info about each license
     -``in use line``: info about licenses in use
```

### Comparing `license_manager_agent-3.1.1/lm_agent/parsing/rlm.py` & `license_manager_agent-3.2.0/lm_agent/parsing/rlm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Parser for RLM
 """
 import re
 from typing import Optional
+from lm_agent.server_interfaces.license_server_interface import LicenseUsesItem
+
 
 INT = r"\d+"
 VERSION = rf"v{INT}\.{INT}"
 HOSTWORD = r"[a-zA-Z0-9-]+"
 HOSTWORD2 = r"[a-zA-Z0-9-.]+"
 HOSTNAME = rf"{HOSTWORD}(\.{HOSTWORD2})*"
 FEATURE_NAME = r"[\w-]+"
@@ -55,28 +57,30 @@
 
 
 def parse_usage_line(line: str) -> Optional[dict]:
     """
     Parse the usage line in the RLM output.
     Data we need:
     - ``feature``: license name
-    - ``user_name``: user name
+    - ``username``: user name
     - ``lead_host``: lead host
     - ``license_used_by_host``: quantity of licenses being use
     """
     parsed_usage = RX_USAGE.match(line)
     if parsed_usage is None:
         return None
     usage_data = parsed_usage.groupdict()
 
     return {
         "license_feature": usage_data["license_feature"].lower(),
-        "user_name": usage_data["user_name"],
-        "lead_host": usage_data["lead_host"],
-        "booked": int(usage_data["license_used_by_host"]),
+        "use": LicenseUsesItem(
+            username=usage_data["user_name"].lower(),
+            lead_host=usage_data["lead_host"],
+            booked=int(usage_data["license_used_by_host"]),
+        ),
     }
 
 
 def parse(server_output: str) -> dict:
     """
     Parse the output from the RLM server.
     Data we need:
@@ -104,14 +108,14 @@
             }
             continue
 
         usage = parse_usage_line(line)
         if usage:
             feature = usage["license_feature"]
             del usage["license_feature"]
-            parsed_data[feature]["uses"].append(usage)
+            parsed_data[feature]["uses"].append(usage["use"])
             continue
 
         else:
             continue
 
     return parsed_data
```

### Comparing `license_manager_agent-3.1.1/lm_agent/reconcile.py` & `license_manager_agent-3.2.0/lm_agent/reconcile.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import sentry_sdk
 
 from lm_agent.backend_utils.utils import check_backend_health
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
-from lm_agent.reconciliation import reconcile
+from lm_agent.services.reconciliation import reconcile
 
 if settings.SENTRY_DSN:
     sentry_sdk.init(
         dsn=settings.SENTRY_DSN,
         sample_rate=typing.cast(float, settings.SENTRY_SAMPLE_RATE),  # The cast silences mypy
         environment=settings.DEPLOY_ENV,
     )
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/flexlm.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
 from lm_agent.parsing import flexlm
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
+from buzz import check_expressions
 
 
 class FlexLMLicenseServer(LicenseServerInterface):
     """Extract license information from FlexLM license server."""
 
     def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         self.license_servers = license_servers
@@ -46,29 +47,31 @@
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
         raise RuntimeError("None of the checks for FlexLM succeeded!")
 
-    async def get_report_item(self, product_feature: str):
+    async def get_report_item(self, feature_id: int, product_feature: str):
         """Override abstract method to parse FlexLM license server output into License Report Item."""
 
         server_output = await self.get_output_from_server(product_feature)
         parsed_output = self.parser(server_output)
 
         # raise exception if parser didn't output license information
-        if parsed_output.get("total") is None or any(
-            [
-                parsed_output.get("total", {}).get("used") is None,
-                parsed_output.get("total", {}).get("total") is None,
-            ]
-        ):
-            raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
+        with check_expressions(
+            "Invalid data returned from parser.", raise_exc_class=LicenseManagerBadServerOutput
+        ) as check:
+            check(parsed_output is not None)
+            check(parsed_output.get("total") is not None)
+            check(parsed_output.get("used") is not None)
+            check(parsed_output.get("uses") is not None)
 
         report_item = LicenseReportItem(
+            feature_id=feature_id,
             product_feature=product_feature,
-            used=parsed_output["total"]["used"],
-            total=parsed_output["total"]["total"],
+            used=parsed_output["used"],
+            total=parsed_output["total"],
+            uses=parsed_output["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/license_server_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module for license server interface abstract base class."""
 import abc
+from typing import List
 
 from pydantic import BaseModel, Field
 
 from lm_agent.config import PRODUCT_FEATURE_RX
 
 
 class LicenseServerInterface(metaclass=abc.ABCMeta):
@@ -34,19 +35,31 @@
         )
 
     @abc.abstractclassmethod
     def get_output_from_server(self, product_feature: str):
         """Return output from license server for the indicated features."""
 
     @abc.abstractclassmethod
-    def get_report_item(self, product_feature: str):
+    def get_report_item(self, feature_id: int, product_feature: str):
         """Parse license server output into a report item for the indicated feature."""
 
 
+class LicenseUsesItem(BaseModel):
+    """
+    A list of usage information for a license.
+    """
+
+    username: str
+    lead_host: str
+    booked: int
+
+
 class LicenseReportItem(BaseModel):
     """
     An item in a LicenseReport, a count of tokens for one product/feature.
     """
 
+    feature_id: int
     product_feature: str = Field(..., regex=PRODUCT_FEATURE_RX)
     used: int
     total: int
+    uses: List[LicenseUsesItem] = []
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/olicense.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-"""LM-X license server interface."""
+"""OLicense license server interface."""
 import typing
 
 from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import lmx
+from lm_agent.parsing import olicense
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class LMXLicenseServer(LicenseServerInterface):
-    """Extract license information from LM-X license server."""
+class OLicenseLicenseServer(LicenseServerInterface):
+    """Extract license information from OLicense license server."""
 
     def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         """Initialize the license server instance with the license server host and parser."""
         self.license_servers = license_servers
-        self.parser = lmx.parse
+        self.parser = olicense.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
         commands_to_run = []
         for license_server in self.license_servers:
             command_line = [
-                f"{settings.LMXENDUTIL_PATH}",
-                "-licstat",
-                "-host",
-                f"{license_server.host}",
-                "-port",
-                f"{license_server.port}",
+                f"{settings.OLIXTOOL_PATH}",
+                "-sv",
+                f"{license_server.host}:{license_server.port}",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from LM-X license server."""
+        """Override abstract method to get output from OLicense license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for LM-X succeeded!")
+        raise RuntimeError("None of the checks for OLicense succeeded!")
 
-    async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse LM-X license server output into License Report Item."""
+    async def get_report_item(self, feature_id: int, product_feature: str):
+        """Override abstract method to parse OLicense license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
 
         # raise exception if parser didn't output license information
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
+            feature_id=feature_id,
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
+            uses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/lsdyna.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,30 @@
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
         raise RuntimeError("None of the checks for LS-Dyna succeeded!")
 
-    async def get_report_item(self, product_feature: str):
+    async def get_report_item(self, feature_id: int, product_feature: str):
         """Override abstract method to parse LS-Dyna license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
 
         # raise exception if parser didn't output license information
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
+            feature_id=feature_id,
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
+            uses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/lmx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-"""OLicense license server interface."""
+"""LM-X license server interface."""
 import typing
 
 from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import olicense
+from lm_agent.parsing import lmx
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class OLicenseLicenseServer(LicenseServerInterface):
-    """Extract license information from OLicense license server."""
+class LMXLicenseServer(LicenseServerInterface):
+    """Extract license information from LM-X license server."""
 
     def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         """Initialize the license server instance with the license server host and parser."""
         self.license_servers = license_servers
-        self.parser = olicense.parse
+        self.parser = lmx.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
         commands_to_run = []
         for license_server in self.license_servers:
             command_line = [
-                f"{settings.OLIXTOOL_PATH}",
-                "-sv",
-                f"{license_server.host}:{license_server.port}",
+                f"{settings.LMXENDUTIL_PATH}",
+                "-licstat",
+                "-host",
+                f"{license_server.host}",
+                "-port",
+                f"{license_server.port}",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from OLicense license server."""
+        """Override abstract method to get output from LM-X license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for OLicense succeeded!")
+        raise RuntimeError("None of the checks for LM-X succeeded!")
 
-    async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse OLicense license server output into License Report Item."""
+    async def get_report_item(self, feature_id: int, product_feature: str):
+        """Override abstract method to parse LM-X license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
 
         # raise exception if parser didn't output license information
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
+            feature_id=feature_id,
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
+            uses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-3.1.1/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-3.2.0/lm_agent/server_interfaces/rlm.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,28 +45,30 @@
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
         raise RuntimeError("None of the checks for RLM succeeded!")
 
-    async def get_report_item(self, product_feature: str):
+    async def get_report_item(self, feature_id: int, product_feature: str):
         """Override abstract method to parse RLM license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
 
         # raise exception if parser didn't output license information
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
+            feature_id=feature_id,
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
+            uses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-3.1.1/lm_agent/utils.py` & `license_manager_agent-3.2.0/lm_agent/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     command_line = shlex.join(command_line_parts)
     proc = await asyncio.create_subprocess_shell(
         command_line, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
     )
 
     # block until the command succeeds
     stdout, _ = await asyncio.wait_for(proc.communicate(), TOOL_TIMEOUT)
-    output = str(stdout, encoding=ENCODING)
+    output = str(stdout, encoding=ENCODING, errors="replace")
 
     if proc.returncode != 0:
         error_message = shlex.join(
             [
                 f"Command {command_line} failed!",
                 f"Error: {output}",
                 f"Return code: {proc.returncode}",
```

### Comparing `license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/common.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/reservations.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import asyncio
 import sys
 
 from lm_agent.backend_utils.utils import remove_job_by_slurm_job_id
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
-from lm_agent.reconciliation import update_features
+from lm_agent.services.reconciliation import update_features
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def epilog():
     # Initialize the logger
     init_logging("slurmctld-epilog")
@@ -32,20 +32,21 @@
     try:
         required_licenses = get_required_licenses_for_job(job_licenses)
     except Exception as e:
         logger.error(f"Failed to call get_required_licenses_for_job with {e}")
         sys.exit(1)
 
     if not required_licenses:
-        logger.debug("No licenses required, exiting!")
+        logger.debug(f"No licenses required for job {job_id}, exiting!")
         sys.exit(0)
 
     if len(required_licenses) > 0:
         # Attempt to remove the job with its bookings.
         await remove_job_by_slurm_job_id(job_id)
+        logger.debug(f"Job {job_id} removed successfully")
 
 
 def main():
     asyncio.run(epilog())
 
 
 if __name__ == "__main__":
```

### Comparing `license_manager_agent-3.1.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import asyncio
 import sys
 
 from lm_agent.backend_utils.models import LicenseBookingRequest
 from lm_agent.backend_utils.utils import get_cluster_configs_from_backend, make_booking_request
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
-from lm_agent.reconciliation import update_features
+from lm_agent.services.reconciliation import update_features
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def prolog():
     """The PrologSlurmctld for the license-manager-agent."""
     # Initialize the logger
@@ -38,18 +38,18 @@
     try:
         required_licenses = get_required_licenses_for_job(job_licenses)
     except Exception as e:
         logger.error(f"Failed to call get_required_licenses_for_job with {e}")
         sys.exit(1)
 
     if not required_licenses:
-        logger.debug("No licenses required, exiting!")
+        logger.debug(f"No licenses required for job {job_id}, exiting!")
         sys.exit(0)
 
-    logger.debug(f"Required licenses: {required_licenses}")
+    logger.debug(f"Required licenses for job {job_id}: {required_licenses}")
 
     tracked_licenses = list()
 
     # Create a list of tracked licenses in the form <product>.<feature>
     if len(required_licenses) > 0:
         # Create a list of tracked licenses in the form <product>.<feature>
         try:
@@ -57,46 +57,46 @@
         except Exception as e:
             logger.error(f"Failed to call get_config_from_backend with {e}")
             sys.exit(1)
 
         for entry in entries:
             for feature in entry.features:
                 tracked_licenses.append(f"{feature.product.name}.{feature.name}")
-    logger.debug(f"Tracked licenses: {tracked_licenses}")
 
     # Create a tracked LicenseBookingRequest for licenses that we actually
     # track. These tracked licenses are what we will check feature token
     # availability for.
     tracked_license_booking_request = LicenseBookingRequest(
         slurm_job_id=job_id,
         username=user_name,
         lead_host=lead_host,
         bookings=[],
     )
     for booking in required_licenses:
         if booking.product_feature in tracked_licenses:
             tracked_license_booking_request.bookings.append(booking)
-    logger.debug(f"Tracked license bookings: {tracked_license_booking_request}")
+    logger.debug(f"Tracked licenses bookings for job {job_id}: {tracked_license_booking_request}")
 
     if len(tracked_license_booking_request.bookings) > 0:
         # Check if reconciliation should be triggered.
         if settings.USE_RECONCILE_IN_PROLOG_EPILOG:
             # Force a reconciliation before we check the feature token availability.
             try:
                 await update_features()
             except Exception as e:
                 logger.error(f"Failed to call reconcile with {e}")
                 sys.exit(1)
 
         booking_request = await make_booking_request(tracked_license_booking_request)
         if not booking_request:
-            logger.debug("Booking request unsuccessful, not enough licenses.")
+            logger.debug(f"Booking request for job {job_id} unsuccessful, not enough licenses.")
             sys.exit(1)
-        logger.debug(f"License booking sucessful, job id: {job_id}.")
-        logger.debug(f"Licenses booked: {repr(tracked_license_booking_request.bookings)}")
+        logger.debug(
+            f"Booking request for job {job_id} sucessful, licenses booked: {repr(tracked_license_booking_request.bookings)}"
+        )
     sys.exit(0)
 
 
 def main():
     asyncio.run(prolog())
```

### Comparing `license_manager_agent-3.1.1/pyproject.toml` & `license_manager_agent-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "3.1.1"
+version = "3.2.0"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
```

### Comparing `license_manager_agent-3.1.1/PKG-INFO` & `license_manager_agent-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 3.1.1
+Version: 3.2.0
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

