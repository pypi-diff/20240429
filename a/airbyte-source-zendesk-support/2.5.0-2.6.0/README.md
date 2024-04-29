# Comparing `tmp/airbyte_source_zendesk_support-2.5.0.tar.gz` & `tmp/airbyte_source_zendesk_support-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_support-2.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_support-2.6.0.tar", max compression
```

## Comparing `airbyte_source_zendesk_support-2.5.0.tar` & `airbyte_source_zendesk_support-2.6.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0     4663 2024-04-25 21:04:20.753516 airbyte_source_zendesk_support-2.5.0/README.md
--rw-r--r--   0        0        0      832 2024-04-25 21:07:43.057729 airbyte_source_zendesk_support-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/__init__.py
--rw-r--r--   0        0        0      255 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/run.py
--rw-r--r--   0        0        0      392 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/account_attributes.json
--rw-r--r--   0        0        0     1064 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/article_comments.json
--rw-r--r--   0        0        0     1714 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/articles.json
--rw-r--r--   0        0        0     1625 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/attribute_definitions.json
--rw-r--r--   0        0        0      877 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/audit_logs.json
--rw-r--r--   0        0        0     1068 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/brands.json
--rw-r--r--   0        0        0     5246 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/custom_roles.json
--rw-r--r--   0        0        0      682 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/deleted_tickets.json
--rw-r--r--   0        0        0      514 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/group_memberships.json
--rw-r--r--   0        0        0      630 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/groups.json
--rw-r--r--   0        0        0     1423 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/macros.json
--rw-r--r--   0        0        0     1284 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organization_fields.json
--rw-r--r--   0        0        0      651 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organization_memberships.json
--rw-r--r--   0        0        0     1210 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organizations.json
--rw-r--r--   0        0        0     1004 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/post_comments.json
--rw-r--r--   0        0        0     1595 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/posts.json
--rw-r--r--   0        0        0      801 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0      708 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/schedules.json
--rw-r--r--   0        0        0     1958 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/attachments.json
--rw-r--r--   0        0        0     1835 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/metadata.json
--rw-r--r--   0        0        0     4521 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/tickets.json
--rw-r--r--   0        0        0     1617 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/via.json
--rw-r--r--   0        0        0     2707 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/via_channel.json
--rw-r--r--   0        0        0     1929 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/sla_policies.json
--rw-r--r--   0        0        0      165 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/tags.json
--rw-r--r--   0        0        0    17835 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_audits.json
--rw-r--r--   0        0        0     1151 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_comments.json
--rw-r--r--   0        0        0     2335 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_fields.json
--rw-r--r--   0        0        0     1359 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_forms.json
--rw-r--r--   0        0        0      394 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_metric_events.json
--rw-r--r--   0        0        0     3616 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_metrics.json
--rw-r--r--   0        0        0      512 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_skips.json
--rw-r--r--   0        0        0       27 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/tickets.json
--rw-r--r--   0        0        0      902 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/topics.json
--rw-r--r--   0        0        0     1054 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/user_fields.json
--rw-r--r--   0        0        0     4496 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/users.json
--rw-r--r--   0        0        0      647 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/votes.json
--rw-r--r--   0        0        0     7572 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/source.py
--rw-r--r--   0        0        0     5975 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/spec.json
--rw-r--r--   0        0        0    39231 2024-04-25 21:04:20.757516 airbyte_source_zendesk_support-2.5.0/source_zendesk_support/streams.py
--rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4663 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/README.md
+-rw-r--r--   0        0        0      832 2024-04-29 14:58:10.032643 airbyte_source_zendesk_support-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/__init__.py
+-rw-r--r--   0        0        0     3380 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/components.py
+-rw-r--r--   0        0        0    19125 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/manifest.yaml
+-rw-r--r--   0        0        0      255 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/run.py
+-rw-r--r--   0        0        0      392 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/account_attributes.json
+-rw-r--r--   0        0        0     1064 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/article_comments.json
+-rw-r--r--   0        0        0     1714 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/articles.json
+-rw-r--r--   0        0        0     1625 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/attribute_definitions.json
+-rw-r--r--   0        0        0      877 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/audit_logs.json
+-rw-r--r--   0        0        0     1068 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/brands.json
+-rw-r--r--   0        0        0     5246 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/custom_roles.json
+-rw-r--r--   0        0        0      682 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/deleted_tickets.json
+-rw-r--r--   0        0        0      514 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/group_memberships.json
+-rw-r--r--   0        0        0      630 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/groups.json
+-rw-r--r--   0        0        0     1423 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/macros.json
+-rw-r--r--   0        0        0     1284 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organization_fields.json
+-rw-r--r--   0        0        0      651 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organization_memberships.json
+-rw-r--r--   0        0        0     1210 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organizations.json
+-rw-r--r--   0        0        0     1004 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/post_comments.json
+-rw-r--r--   0        0        0     1595 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/posts.json
+-rw-r--r--   0        0        0      801 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0      708 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/schedules.json
+-rw-r--r--   0        0        0     1958 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/attachments.json
+-rw-r--r--   0        0        0     1835 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/metadata.json
+-rw-r--r--   0        0        0     4521 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/tickets.json
+-rw-r--r--   0        0        0     1617 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/via.json
+-rw-r--r--   0        0        0     2707 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/via_channel.json
+-rw-r--r--   0        0        0     1929 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/sla_policies.json
+-rw-r--r--   0        0        0      165 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/tags.json
+-rw-r--r--   0        0        0     2114 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_activities.json
+-rw-r--r--   0        0        0    17835 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_audits.json
+-rw-r--r--   0        0        0     1151 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_comments.json
+-rw-r--r--   0        0        0     2335 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     1359 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_forms.json
+-rw-r--r--   0        0        0      394 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_metric_events.json
+-rw-r--r--   0        0        0     3616 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_metrics.json
+-rw-r--r--   0        0        0      512 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_skips.json
+-rw-r--r--   0        0        0       27 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/tickets.json
+-rw-r--r--   0        0        0      902 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/topics.json
+-rw-r--r--   0        0        0     1054 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/user_fields.json
+-rw-r--r--   0        0        0     4496 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/users.json
+-rw-r--r--   0        0        0      647 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/votes.json
+-rw-r--r--   0        0        0     7876 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/source.py
+-rw-r--r--   0        0        0     5975 2024-04-29 14:54:08.492602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/spec.json
+-rw-r--r--   0        0        0    39231 2024-04-29 14:54:08.496602 airbyte_source_zendesk_support-2.6.0/source_zendesk_support/streams.py
+-rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.0/PKG-INFO
```

### Comparing `airbyte_source_zendesk_support-2.5.0/README.md` & `airbyte_source_zendesk_support-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/pyproject.toml` & `airbyte_source_zendesk_support-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.0"
+version = "2.6.0"
 name = "airbyte-source-zendesk-support"
 description = "Source implementation for Zendesk Support."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/__init__.py` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/article_comments.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/article_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/articles.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/attribute_definitions.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/attribute_definitions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/audit_logs.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/audit_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/brands.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/brands.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/custom_roles.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/custom_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/deleted_tickets.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/deleted_tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/group_memberships.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/groups.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/macros.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organization_fields.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organization_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organization_memberships.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organization_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/organizations.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/post_comments.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/post_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/posts.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/posts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/satisfaction_ratings.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/schedules.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/schedules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/attachments.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/metadata.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/tickets.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/via.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/shared/via_channel.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/shared/via_channel.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/sla_policies.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_audits.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_comments.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_fields.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_forms.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_metrics.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/ticket_skips.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/ticket_skips.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/topics.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/topics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/user_fields.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/user_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/users.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/schemas/votes.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/schemas/votes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/spec.json` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/source_zendesk_support/streams.py` & `airbyte_source_zendesk_support-2.6.0/source_zendesk_support/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.5.0/PKG-INFO` & `airbyte_source_zendesk_support-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-support
-Version: 2.5.0
+Version: 2.6.0
 Summary: Source implementation for Zendesk Support.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

