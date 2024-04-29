# Comparing `tmp/djangoldp_esa-2.0.2.tar.gz` & `tmp/djangoldp_esa-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_esa-2.0.2.tar", last modified: Thu Apr 18 16:20:44 2024, max compression
+gzip compressed data, was "djangoldp_esa-2.0.3.tar", last modified: Mon Apr 29 12:57:30 2024, max compression
```

## Comparing `djangoldp_esa-2.0.2.tar` & `djangoldp_esa-2.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.499638 djangoldp_esa-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 16:20:44.499638 djangoldp_esa-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-18 16:20:41.000000 djangoldp_esa-2.0.2/djangoldp_esa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    10639 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/migrations/0002_auto_20220623_1611.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/migrations/0003_auto_20220627_1354.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6128 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/models.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/admin/login.html
--rw-rw-rw-   0 root         (0) root         (0)    10587 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     2617 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)    11036 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/password/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.499638 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      650 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)    10225 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     1605 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 16:20:44.495638 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 16:20:44.000000 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1000 2024-04-18 16:20:44.000000 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 16:20:44.000000 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-04-18 16:20:44.000000 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 16:20:44.000000 djangoldp_esa-2.0.2/djangoldp_esa.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-18 16:20:44.499638 djangoldp_esa-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-18 16:20:26.000000 djangoldp_esa-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-29 12:57:27.000000 djangoldp_esa-2.0.3/djangoldp_esa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    10639 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/migrations/0002_auto_20220623_1611.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/migrations/0003_auto_20220627_1354.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6182 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/admin/login.html
+-rw-rw-rw-   0 root         (0) root         (0)    10587 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/password/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)    10225 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-29 12:57:30.000000 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-04-29 12:57:30.000000 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:57:30.000000 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-29 12:57:30.000000 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-29 12:57:30.000000 djangoldp_esa-2.0.3/djangoldp_esa.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-29 12:57:30.144178 djangoldp_esa-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-29 12:57:11.000000 djangoldp_esa-2.0.3/setup.py
```

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/admin.py` & `djangoldp_esa-2.0.3/djangoldp_esa/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/migrations/0001_initial.py` & `djangoldp_esa-2.0.3/djangoldp_esa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/migrations/0002_auto_20220623_1611.py` & `djangoldp_esa-2.0.3/djangoldp_esa/migrations/0002_auto_20220623_1611.py`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/models.py` & `djangoldp_esa-2.0.3/djangoldp_esa/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         permission_classes = [InheritPermissions]
         inherit_permissions = ['community']
 
         ordering = ['community']
         container_path = "/esaprofiles/"
         serializer_fields = ['@id', 'main_contact_first_name', 'main_contact_last_name', 'tags',
                              'role', 'sectors', 'spaces', 'status', 'graduation_year', 'position_esa_bic', 'location_esa_bic']
+        nested_fields = ['tags', 'sectors', 'spaces']
         rdf_type = "sib:CommunityEsaProfile"
         depth = 1
 
 
 class EsaCommunityTag(Model):
     name = models.CharField(max_length=254, blank=True, null=True, default='')
     esacommunity = models.ManyToManyField(
```

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/admin/login.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/email.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/oidc_provider/authorize.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/password/email.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/login.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_confirm.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_done.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_email.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa/templates/registration/password_reset_form.html` & `djangoldp_esa-2.0.3/djangoldp_esa/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/djangoldp_esa.egg-info/SOURCES.txt` & `djangoldp_esa-2.0.3/djangoldp_esa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.2/setup.cfg` & `djangoldp_esa-2.0.3/setup.cfg`

 * *Files identical despite different names*

