# Comparing `tmp/grove-1.2.2.tar.gz` & `tmp/grove-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grove-1.2.2.tar", last modified: Mon Dec 11 16:09:26 2023, max compression
+gzip compressed data, was "grove-1.3.0.tar", last modified: Mon Apr 29 14:47:30 2024, max compression
```

## Comparing `grove-1.2.2.tar` & `grove-1.3.0.tar`

### file list

```diff
@@ -1,427 +1,437 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.113798 grove-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.057798 grove-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-11 16:09:11.000000 grove-1.2.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.057798 grove-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-11 16:09:11.000000 grove-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-12-11 16:09:11.000000 grove-1.2.2/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-11 16:09:11.000000 grove-1.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-12-11 16:09:11.000000 grove-1.2.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.057798 grove-1.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-11 16:09:11.000000 grove-1.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-11 16:09:11.000000 grove-1.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-12-11 16:09:11.000000 grove-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-11 16:09:11.000000 grove-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-12-11 16:09:26.113798 grove-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2023-12-11 16:09:11.000000 grove-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-11 16:09:11.000000 grove-1.2.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.061798 grove-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-11 16:09:11.000000 grove-1.2.2/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.061798 grove-1.2.2/docs/_generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:11.000000 grove-1.2.2/docs/_generated/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-11 16:09:11.000000 grove-1.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-11 16:09:11.000000 grove-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2023-12-11 16:09:11.000000 grove-1.2.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-11 16:09:11.000000 grove-1.2.2/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-11 16:09:11.000000 grove-1.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2023-12-11 16:09:11.000000 grove-1.2.2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-12-11 16:09:11.000000 grove-1.2.2/docs/grove.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-12-11 16:09:11.000000 grove-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2023-12-11 16:09:11.000000 grove-1.2.2/docs/internals.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-11 16:09:11.000000 grove-1.2.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2023-12-11 16:09:11.000000 grove-1.2.2/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.061798 grove-1.2.2/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    51212 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/flow.png
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-logo-small-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    19248 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    73194 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-support-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    78562 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove-support.png
--rw-r--r--   0 runner    (1001) docker     (127)    53548 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/grove.png
--rw-r--r--   0 runner    (1001) docker     (127)    41033 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/plugin_structure.png
--rw-r--r--   0 runner    (1001) docker     (127)    69230 2023-12-11 16:09:11.000000 grove-1.2.2/docs/static/pointers.png
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-11 16:09:11.000000 grove-1.2.2/docs/style.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-11 16:09:11.000000 grove-1.2.2/grove/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-11 16:09:11.000000 grove-1.2.2/grove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/caches/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-12-11 16:09:11.000000 grove-1.2.2/grove/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-12-11 16:09:11.000000 grove-1.2.2/grove/caches/aws_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2023-12-11 16:09:11.000000 grove-1.2.2/grove/caches/local_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-11 16:09:11.000000 grove-1.2.2/grove/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2023-12-11 16:09:11.000000 grove-1.2.2/grove/configs/aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-12-11 16:09:11.000000 grove-1.2.2/grove/configs/local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)    38204 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/connectors/atlassian/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/atlassian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/atlassian/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/atlassian/audit_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.065798 grove-1.2.2/grove/connectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/github/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/github/audit_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/gsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/gsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/gsuite/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/gsuite/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/local/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/local/heartbeat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/okta/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/okta/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/okta/system_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/onepassword/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/onepassword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/onepassword/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/onepassword/events_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/onepassword/events_itemusages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/onepassword/events_signinattempts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/oomnitza/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/oomnitza/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/oomnitza/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/oomnitza/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/pagerduty/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/pagerduty/audit_records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/sf/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sf/event_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.069798 grove-1.2.2/grove/connectors/sfmc/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sfmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sfmc/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sfmc/audit_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/sfmc/security_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/slack/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/slack/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/tfc/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tfc/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tfc/audit_trails.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/tines/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tines/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/tines/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/torq/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/torq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/torq/activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/torq/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/torq/audit_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/twilio/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/twilio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/twilio/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/twilio/monitor_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/workday/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/workday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/workday/activity_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/workday/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.073798 grove-1.2.2/grove/connectors/zoom/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/zoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/zoom/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/zoom/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2023-12-11 16:09:11.000000 grove-1.2.2/grove/connectors/zoom/operationlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-12-11 16:09:11.000000 grove-1.2.2/grove/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/grove/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-11 16:09:11.000000 grove-1.2.2/grove/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-12-11 16:09:11.000000 grove-1.2.2/grove/entrypoints/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2023-12-11 16:09:11.000000 grove-1.2.2/grove/entrypoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-11 16:09:11.000000 grove-1.2.2/grove/entrypoints/local_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-12-11 16:09:11.000000 grove-1.2.2/grove/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/grove/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-11 16:09:11.000000 grove-1.2.2/grove/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-11 16:09:11.000000 grove-1.2.2/grove/helpers/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-12-11 16:09:11.000000 grove-1.2.2/grove/helpers/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-11 16:09:11.000000 grove-1.2.2/grove/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2023-12-11 16:09:11.000000 grove-1.2.2/grove/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/grove/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-12-11 16:09:11.000000 grove-1.2.2/grove/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2023-12-11 16:09:11.000000 grove-1.2.2/grove/outputs/aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2023-12-11 16:09:11.000000 grove-1.2.2/grove/outputs/local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-12-11 16:09:11.000000 grove-1.2.2/grove/outputs/local_stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/grove/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/extract_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/filter_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/filter_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/split_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-12-11 16:09:11.000000 grove-1.2.2/grove/processors/zip_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/grove/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-12-11 16:09:11.000000 grove-1.2.2/grove/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-12-11 16:09:11.000000 grove-1.2.2/grove/secrets/aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2023-12-11 16:09:11.000000 grove-1.2.2/grove/secrets/hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-12-11 16:09:11.000000 grove-1.2.2/grove/secrets/local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-11 16:09:11.000000 grove-1.2.2/grove/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.113798 grove-1.2.2/grove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-12-11 16:09:25.000000 grove-1.2.2/grove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12247 2023-12-11 16:09:26.000000 grove-1.2.2/grove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 16:09:25.000000 grove-1.2.2/grove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-12-11 16:09:25.000000 grove-1.2.2/grove.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-11 16:09:25.000000 grove-1.2.2/grove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-11 16:09:25.000000 grove-1.2.2/grove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2023-12-11 16:09:11.000000 grove-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 16:09:26.113798 grove-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.077798 grove-1.2.2/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-11 16:09:11.000000 grove-1.2.2/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/scripts/run_cookiecutter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.045798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/example_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-12-11 16:09:11.000000 grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/templates/configuration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.081798 grove-1.2.2/templates/configuration/1password/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/1password/events_audit.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/1password/events_itemusages.json
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/1password/events_signinattempts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/atlassian/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/atlassian/audit_events.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/github/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/github/enterprise_audit_log.json
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/github/orgs_audit_log.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/github/self-hosted_orgs_audit_log.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/gsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/gsuite/activities.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/gsuite/alerts.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/gsuite/flattened_drive_activities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/okta/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/okta/preview_system_log.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/okta/system_log.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/oomnitza/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/oomnitza/activities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/pagerduty/audit_records.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/salesforce/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/salesforce/event_log.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/slack/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/tfc/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/tfc/audit_trails.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/tines/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/tines/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/torq/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/torq/activity_logs.json
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/torq/audit_logs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/twilio/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/twilio/messages.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/twilio/monitor_events.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/workday/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/workday/activity_logging.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.085798 grove-1.2.2/templates/configuration/zoom/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/zoom/activities.json
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-11 16:09:11.000000 grove-1.2.2/templates/configuration/zoom/operationlogs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/templates/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.089798 grove-1.2.2/templates/deployment/local-quick-start/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/local-quick-start/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.089798 grove-1.2.2/templates/deployment/local-quick-start/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/local-quick-start/connectors/local_heartbeat.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/local-quick-start/test_entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.089798 grove-1.2.2/templates/deployment/terraform-aws-ecs/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/templates/deployment/terraform-aws-ecs/connectors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.089798 grove-1.2.2/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/local_heartbeat.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.089798 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/cloudwatch.tf
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/compute.tf
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/dynamodb.tf
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/iam.tf
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/network.tf
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/output.tf
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/s3.tf
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/variables.tf
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/output.tf
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/providers.tf
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-11 16:09:11.000000 grove-1.2.2/templates/deployment/terraform-aws-ecs/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.097798 grove-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-11 16:09:11.000000 grove-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.097798 grove-1.2.2/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-11 16:09:11.000000 grove-1.2.2/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-11 16:09:11.000000 grove-1.2.2/tests/connectors/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/tests/fixtures/atlassian/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.097798 grove-1.2.2/tests/fixtures/atlassian/event_audit/
--rw-r--r--   0 runner    (1001) docker     (127)    76068 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/atlassian/event_audit/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/atlassian/event_audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/tests/fixtures/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.097798 grove-1.2.2/tests/fixtures/github/audit/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/github/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/github/audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/github/git/
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/github/git/001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/tests/fixtures/grove/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/grove/chronological/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/chronological/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/chronological/002.json
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/chronological/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/grove/reverse_chronological/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/reverse_chronological/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/reverse_chronological/002.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/grove/reverse_chronological/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/tests/fixtures/gsuite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/gsuite/activities/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/gsuite/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/gsuite/activities/002.json
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/gsuite/activities/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/gsuite/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/gsuite/alerts/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/gsuite/alerts/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.049798 grove-1.2.2/tests/fixtures/okta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/okta/system_log/
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/okta/system_log/001.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/okta/system_log/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/onepassword/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/onepassword/events_audit/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_audit/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_audit/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_audit/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.101798 grove-1.2.2/tests/fixtures/onepassword/events_itemusages/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_itemusages/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_itemusages/002.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_itemusages/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/002.json
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/oomnitza/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/oomnitza/activities/
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/oomnitza/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (127)    77536 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/oomnitza/activities/002.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/oomnitza/activities/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/pagerduty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/pagerduty/audit_records/
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/pagerduty/audit_records/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/pagerduty/audit_records/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/pagerduty/audit_records/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/sf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/sf/event_log/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sf/event_log/001.csv
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sf/event_log/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sf/event_log/error.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sf/event_log/login.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/sfmc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/sfmc/audit_events/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/audit_events/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/audit_events/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/audit_events/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.105798 grove-1.2.2/tests/fixtures/sfmc/security_events/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/security_events/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/security_events/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/sfmc/security_events/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/slack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/slack/audit/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/slack/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/slack/audit/002.json
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/slack/audit/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/tfc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/tfc/audit_trails/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tfc/audit_trails/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tfc/audit_trails/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tfc/audit_trails/003.json
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tfc/audit_trails/004.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/tines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/tines/audit_logs/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tines/audit_logs/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tines/audit_logs/002.json
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/tines/audit_logs/003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/torq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/torq/activity/
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/torq/activity/001.json
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/torq/activity/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/torq/audit/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/torq/audit/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/torq/audit/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/torq/client/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/torq/client/001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/workday/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/workday/activity_logging/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/workday/activity_logging/001.json
--rw-r--r--   0 runner    (1001) docker     (127)    39041 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/workday/activity_logging/002.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/workday/activity_logging/003.json
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/workday/activity_logging/004.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/workday/activity_logging/005.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.053798 grove-1.2.2/tests/fixtures/zoom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.109798 grove-1.2.2/tests/fixtures/zoom/activities/
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/zoom/activities/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/zoom/activities/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.113798 grove-1.2.2/tests/fixtures/zoom/client/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/zoom/client/001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.113798 grove-1.2.2/tests/fixtures/zoom/operation/
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/zoom/operation/001.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-11 16:09:11.000000 grove-1.2.2/tests/fixtures/zoom/operation/002.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:09:26.113798 grove-1.2.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-12-11 16:09:11.000000 grove-1.2.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-11 16:09:11.000000 grove-1.2.2/tests/mocks/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_caches_local_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_configs_aws_ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_atlassian_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_github_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_github_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_gsuite_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_gsuite_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_okta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_okta_system_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_onepassword_events_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_onepassword_events_itemusages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_onepassword_events_signinattempts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_oomnitza_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_pagerduty_audit_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_sf_event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_sfmc_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_sfmc_security_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_slack_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_tfc_audit_trails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_tines_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_torq_activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_torq_audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_torq_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_workday_activity_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_zoom_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_zoom_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_connectors_zoom_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_e2e_grove_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_helpers_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_outputs_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_outputs_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_processors_extract_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_processors_filter_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_processors_filter_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_processors_split_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_processors_zip_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_secrets_hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-11 16:09:11.000000 grove-1.2.2/tests/test_secrets_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.052591 grove-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.996590 grove-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 14:47:18.000000 grove-1.3.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.996590 grove-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-29 14:47:18.000000 grove-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 14:47:18.000000 grove-1.3.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-29 14:47:18.000000 grove-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-29 14:47:18.000000 grove-1.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.996590 grove-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 14:47:18.000000 grove-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 14:47:18.000000 grove-1.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-29 14:47:18.000000 grove-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 14:47:18.000000 grove-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 14:47:30.052591 grove-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-29 14:47:18.000000 grove-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 14:47:18.000000 grove-1.3.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.000590 grove-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 14:47:18.000000 grove-1.3.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.000590 grove-1.3.0/docs/_generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:18.000000 grove-1.3.0/docs/_generated/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-29 14:47:18.000000 grove-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-29 14:47:18.000000 grove-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-29 14:47:18.000000 grove-1.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-29 14:47:18.000000 grove-1.3.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-29 14:47:18.000000 grove-1.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-29 14:47:18.000000 grove-1.3.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-29 14:47:18.000000 grove-1.3.0/docs/grove.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-29 14:47:18.000000 grove-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-04-29 14:47:18.000000 grove-1.3.0/docs/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 14:47:18.000000 grove-1.3.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-29 14:47:18.000000 grove-1.3.0/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.000590 grove-1.3.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/flow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-logo-small-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73194 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-support-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78562 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove-support.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53548 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/grove.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41033 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/plugin_structure.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69230 2024-04-29 14:47:18.000000 grove-1.3.0/docs/static/pointers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-29 14:47:18.000000 grove-1.3.0/docs/style.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-29 14:47:18.000000 grove-1.3.0/grove/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 14:47:18.000000 grove-1.3.0/grove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-29 14:47:18.000000 grove-1.3.0/grove/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-04-29 14:47:18.000000 grove-1.3.0/grove/caches/aws_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-29 14:47:18.000000 grove-1.3.0/grove/caches/local_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-29 14:47:18.000000 grove-1.3.0/grove/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-29 14:47:18.000000 grove-1.3.0/grove/configs/aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-29 14:47:18.000000 grove-1.3.0/grove/configs/local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)    38204 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/connectors/atlassian/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/atlassian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/atlassian/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/atlassian/audit_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/connectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/github/audit_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.004590 grove-1.3.0/grove/connectors/gsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/gsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/gsuite/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/gsuite/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/local/heartbeat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/okta/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/okta/system_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/onepassword/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/onepassword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/onepassword/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/onepassword/events_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/onepassword/events_itemusages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/onepassword/events_signinattempts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/oomnitza/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/oomnitza/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/oomnitza/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/oomnitza/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/pagerduty/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/pagerduty/audit_records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/sf/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sf/event_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/sfmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sfmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sfmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sfmc/audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/sfmc/security_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.008590 grove-1.3.0/grove/connectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/slack/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/slack/audit_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/stripe/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/stripe/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/tfc/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tfc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tfc/audit_trails.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/tines/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tines/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/tines/audit_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/torq/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/torq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/torq/activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/torq/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/torq/audit_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/twilio/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/twilio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/twilio/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/twilio/monitor_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/workday/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/workday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/workday/activity_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/workday/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.012590 grove-1.3.0/grove/connectors/zoom/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/zoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/zoom/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/zoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-29 14:47:18.000000 grove-1.3.0/grove/connectors/zoom/operationlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-29 14:47:18.000000 grove-1.3.0/grove/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/grove/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 14:47:18.000000 grove-1.3.0/grove/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-29 14:47:18.000000 grove-1.3.0/grove/entrypoints/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-29 14:47:18.000000 grove-1.3.0/grove/entrypoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-29 14:47:18.000000 grove-1.3.0/grove/entrypoints/local_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-29 14:47:18.000000 grove-1.3.0/grove/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/grove/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 14:47:18.000000 grove-1.3.0/grove/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-29 14:47:18.000000 grove-1.3.0/grove/helpers/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-29 14:47:18.000000 grove-1.3.0/grove/helpers/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-29 14:47:18.000000 grove-1.3.0/grove/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-29 14:47:18.000000 grove-1.3.0/grove/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/grove/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-29 14:47:18.000000 grove-1.3.0/grove/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-29 14:47:18.000000 grove-1.3.0/grove/outputs/aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-29 14:47:18.000000 grove-1.3.0/grove/outputs/local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-29 14:47:18.000000 grove-1.3.0/grove/outputs/local_stdout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/grove/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/extract_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/filter_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/filter_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/split_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-29 14:47:18.000000 grove-1.3.0/grove/processors/zip_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/grove/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-29 14:47:18.000000 grove-1.3.0/grove/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-29 14:47:18.000000 grove-1.3.0/grove/secrets/aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-29 14:47:18.000000 grove-1.3.0/grove/secrets/hashicorp_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-29 14:47:18.000000 grove-1.3.0/grove/secrets/local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-29 14:47:18.000000 grove-1.3.0/grove/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/grove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 14:47:29.000000 grove-1.3.0/grove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-29 14:47:18.000000 grove-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:47:30.052591 grove-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 14:47:18.000000 grove-1.3.0/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/templates/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/templates/code/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.016590 grove-1.3.0/templates/code/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/scripts/run_cookiecutter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.984590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/example_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 14:47:18.000000 grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/templates/configuration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/configuration/1password/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/1password/events_audit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/1password/events_itemusages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/1password/events_signinattempts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/configuration/atlassian/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/atlassian/audit_events.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.020590 grove-1.3.0/templates/configuration/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/github/enterprise_audit_log.json
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/github/orgs_audit_log.json
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/github/self-hosted_orgs_audit_log.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/gsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/gsuite/activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/gsuite/alerts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/gsuite/flattened_drive_activities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/okta/preview_system_log.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/okta/system_log.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/oomnitza/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/oomnitza/activities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/pagerduty/audit_records.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/salesforce/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/salesforce/event_log.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/slack/audit_logs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/stripe/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/stripe/events.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/tfc/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/tfc/audit_trails.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/tines/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/tines/audit_logs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/torq/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/torq/activity_logs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/torq/audit_logs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/twilio/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/twilio/messages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/twilio/monitor_events.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/workday/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/workday/activity_logging.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/configuration/zoom/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/zoom/activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 14:47:18.000000 grove-1.3.0/templates/configuration/zoom/operationlogs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/templates/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/deployment/local-quick-start/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/local-quick-start/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.024590 grove-1.3.0/templates/deployment/local-quick-start/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/local-quick-start/connectors/local_heartbeat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/local-quick-start/test_entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.028591 grove-1.3.0/templates/deployment/terraform-aws-ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/templates/deployment/terraform-aws-ecs/connectors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.028591 grove-1.3.0/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/connectors/local_heartbeat/local_heartbeat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.028591 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/cloudwatch.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/compute.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/dynamodb.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/iam.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/network.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/output.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/s3.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/variables.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/output.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/providers.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 14:47:18.000000 grove-1.3.0/templates/deployment/terraform-aws-ecs/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 14:47:18.000000 grove-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 14:47:18.000000 grove-1.3.0/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-29 14:47:18.000000 grove-1.3.0/tests/connectors/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/tests/fixtures/atlassian/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/atlassian/event_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)    76068 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/atlassian/event_audit/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/atlassian/event_audit/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.988590 grove-1.3.0/tests/fixtures/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/github/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/github/audit/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/github/audit/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/github/git/
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/github/git/001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/grove/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/grove/chronological/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/chronological/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/chronological/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/chronological/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/grove/reverse_chronological/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/reverse_chronological/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/reverse_chronological/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/grove/reverse_chronological/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/gsuite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.036590 grove-1.3.0/tests/fixtures/gsuite/activities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/gsuite/activities/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/gsuite/activities/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/gsuite/activities/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/gsuite/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/gsuite/alerts/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/gsuite/alerts/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/okta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/okta/system_log/
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/okta/system_log/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/okta/system_log/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/onepassword/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/onepassword/events_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_audit/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_audit/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_audit/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/onepassword/events_itemusages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_itemusages/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_itemusages/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_itemusages/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/oomnitza/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/oomnitza/activities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/oomnitza/activities/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/oomnitza/activities/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/oomnitza/activities/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/pagerduty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/pagerduty/audit_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/pagerduty/audit_records/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/pagerduty/audit_records/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/pagerduty/audit_records/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/sf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.040591 grove-1.3.0/tests/fixtures/sf/event_log/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sf/event_log/001.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sf/event_log/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sf/event_log/error.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sf/event_log/login.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/sfmc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/sfmc/audit_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/audit_events/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/audit_events/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/audit_events/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/sfmc/security_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/security_events/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/security_events/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/sfmc/security_events/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/slack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/slack/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/slack/audit/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/slack/audit/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/slack/audit/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/stripe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/stripe/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/stripe/events/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/stripe/events/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/tfc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/tfc/audit_trails/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tfc/audit_trails/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tfc/audit_trails/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tfc/audit_trails/003.json
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tfc/audit_trails/004.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/tines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/tines/audit_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tines/audit_logs/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tines/audit_logs/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/tines/audit_logs/003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/torq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/torq/activity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/torq/activity/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/torq/activity/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/torq/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/torq/audit/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/torq/audit/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.044591 grove-1.3.0/tests/fixtures/torq/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/torq/client/001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.992590 grove-1.3.0/tests/fixtures/workday/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/tests/fixtures/workday/activity_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/workday/activity_logging/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39041 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/workday/activity_logging/002.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/workday/activity_logging/003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/workday/activity_logging/004.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/workday/activity_logging/005.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:29.996590 grove-1.3.0/tests/fixtures/zoom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/tests/fixtures/zoom/activities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/zoom/activities/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/zoom/activities/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/tests/fixtures/zoom/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/zoom/client/001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/tests/fixtures/zoom/operation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/zoom/operation/001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-29 14:47:18.000000 grove-1.3.0/tests/fixtures/zoom/operation/002.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:47:30.048591 grove-1.3.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-29 14:47:18.000000 grove-1.3.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 14:47:18.000000 grove-1.3.0/tests/mocks/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_caches_local_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_configs_aws_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_atlassian_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_github_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_github_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_gsuite_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_gsuite_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_okta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_okta_system_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_onepassword_events_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_onepassword_events_itemusages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_onepassword_events_signinattempts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_oomnitza_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_pagerduty_audit_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_sf_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_sfmc_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_sfmc_security_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_slack_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_stripe_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_tfc_audit_trails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_tines_audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_torq_activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_torq_audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_torq_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_workday_activity_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_zoom_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_zoom_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_connectors_zoom_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_e2e_grove_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_helpers_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_outputs_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_outputs_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_processors_extract_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_processors_filter_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_processors_filter_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_processors_split_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_processors_zip_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_secrets_hashicorp_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-29 14:47:18.000000 grove-1.3.0/tests/test_secrets_local_file.py
```

### Comparing `grove-1.2.2/.github/workflows/ci.yml` & `grove-1.3.0/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 jobs:
   tox:
     name: tox
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ macos-latest, ubuntu-latest ]
-        python-version: [ '3.9', '3.10' ]
+        python-version: [ '3.9', '3.10', '3.12' ]
+        exclude:
+          - os: macos-latest
+            python-version: '3.9'
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: pip install --upgrade pip setuptools wheel tox
       - run: pip install . # required for e2e tests
```

### Comparing `grove-1.2.2/.github/workflows/documentation.yml` & `grove-1.3.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/.github/workflows/release.yml` & `grove-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/.gitignore` & `grove-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/.vscode/settings.json` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/LICENSE` & `grove-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/PKG-INFO` & `grove-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grove
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Software as a Service (SaaS) log collection framework.
 Author: HashiCorp Security (TDR)
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: boto3<2.0,>=1.26
 Requires-Dist: requests<3.0,>=2.28
 Requires-Dist: google-api-python-client<3.0,>=2.68
 Requires-Dist: simple-salesforce<2.0,>=1.12
 Requires-Dist: twilio<8.0,>=7.15
 Requires-Dist: pydantic<2.0,>=1.10
 Requires-Dist: jmespath<2.0,>=1.0.0
+Requires-Dist: stripe<9.0,>=8.4.0
 Provides-Extra: tests
 Requires-Dist: black; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: mypy; extra == "tests"
@@ -29,15 +30,15 @@
 Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: responses; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: sphinx; extra == "tests"
 Requires-Dist: furo; extra == "tests"
-Requires-Dist: moto[s3,ssm]; extra == "tests"
+Requires-Dist: moto[s3,ssm]<5.0,>=4.0; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 
 <p align="center">
     <br /><br />
     <picture>
       <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/hashicorp-forge/grove/main/docs/static/grove-logo-small-light.png?raw=True">
       <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/hashicorp-forge/grove/main/docs/static/grove-logo-small.png?raw=True">
```

### Comparing `grove-1.2.2/README.md` & `grove-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/api.rst` & `grove-1.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/conf.py` & `grove-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/configuration.rst` & `grove-1.3.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/development.rst` & `grove-1.3.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/examples.rst` & `grove-1.3.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/faq.rst` & `grove-1.3.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/grove.rst` & `grove-1.3.0/docs/grove.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/index.rst` & `grove-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/internals.rst` & `grove-1.3.0/docs/internals.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/quickstart.rst` & `grove-1.3.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/custom.css` & `grove-1.3.0/docs/static/custom.css`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/flow.png` & `grove-1.3.0/docs/static/flow.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-logo-light.png` & `grove-1.3.0/docs/static/grove-logo-light.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-logo-small-light.png` & `grove-1.3.0/docs/static/grove-logo-small-light.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-logo-small.png` & `grove-1.3.0/docs/static/grove-logo-small.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-logo.png` & `grove-1.3.0/docs/static/grove-logo.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-support-light.png` & `grove-1.3.0/docs/static/grove-support-light.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove-support.png` & `grove-1.3.0/docs/static/grove-support.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/grove.png` & `grove-1.3.0/docs/static/grove.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/plugin_structure.png` & `grove-1.3.0/docs/static/plugin_structure.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/static/pointers.png` & `grove-1.3.0/docs/static/pointers.png`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/docs/style.rst` & `grove-1.3.0/docs/style.rst`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/__init__.py` & `grove-1.3.0/grove/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/caches/__init__.py` & `grove-1.3.0/grove/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/caches/aws_dynamodb.py` & `grove-1.3.0/grove/caches/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/caches/local_memory.py` & `grove-1.3.0/grove/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/configs/__init__.py` & `grove-1.3.0/grove/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/configs/aws_ssm.py` & `grove-1.3.0/grove/configs/aws_ssm.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/configs/local_file.py` & `grove-1.3.0/grove/configs/local_file.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/__init__.py` & `grove-1.3.0/grove/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/atlassian/api.py` & `grove-1.3.0/grove/connectors/atlassian/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/atlassian/audit_events.py` & `grove-1.3.0/grove/connectors/atlassian/audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/github/api.py` & `grove-1.3.0/grove/connectors/github/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/github/audit_log.py` & `grove-1.3.0/grove/connectors/github/audit_log.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/gsuite/activities.py` & `grove-1.3.0/grove/connectors/gsuite/activities.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/gsuite/alerts.py` & `grove-1.3.0/grove/connectors/gsuite/alerts.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/local/heartbeat.py` & `grove-1.3.0/grove/connectors/local/heartbeat.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/okta/api.py` & `grove-1.3.0/grove/connectors/okta/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/okta/system_log.py` & `grove-1.3.0/grove/connectors/okta/system_log.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/onepassword/api.py` & `grove-1.3.0/grove/connectors/onepassword/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/onepassword/events_audit.py` & `grove-1.3.0/grove/connectors/onepassword/events_audit.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/onepassword/events_itemusages.py` & `grove-1.3.0/grove/connectors/onepassword/events_itemusages.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/onepassword/events_signinattempts.py` & `grove-1.3.0/grove/connectors/onepassword/events_signinattempts.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/oomnitza/activities.py` & `grove-1.3.0/grove/connectors/oomnitza/activities.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/oomnitza/api.py` & `grove-1.3.0/grove/connectors/oomnitza/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/pagerduty/api.py` & `grove-1.3.0/grove/connectors/pagerduty/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/pagerduty/audit_records.py` & `grove-1.3.0/grove/connectors/pagerduty/audit_records.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/sf/event_log.py` & `grove-1.3.0/grove/connectors/sf/event_log.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/sfmc/api.py` & `grove-1.3.0/grove/connectors/sfmc/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/sfmc/audit_events.py` & `grove-1.3.0/grove/connectors/sfmc/audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/sfmc/security_events.py` & `grove-1.3.0/grove/connectors/sfmc/security_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/slack/api.py` & `grove-1.3.0/grove/connectors/slack/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/slack/audit_logs.py` & `grove-1.3.0/grove/connectors/slack/audit_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/tfc/api.py` & `grove-1.3.0/grove/connectors/tfc/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/tfc/audit_trails.py` & `grove-1.3.0/grove/connectors/tfc/audit_trails.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/tines/api.py` & `grove-1.3.0/grove/connectors/tines/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/tines/audit_logs.py` & `grove-1.3.0/grove/connectors/tines/audit_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/torq/activity_logs.py` & `grove-1.3.0/grove/connectors/torq/activity_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/torq/api.py` & `grove-1.3.0/grove/connectors/torq/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/torq/audit_logs.py` & `grove-1.3.0/grove/connectors/torq/audit_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/twilio/messages.py` & `grove-1.3.0/grove/connectors/twilio/messages.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/twilio/monitor_events.py` & `grove-1.3.0/grove/connectors/twilio/monitor_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/workday/activity_logging.py` & `grove-1.3.0/grove/connectors/workday/activity_logging.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/workday/api.py` & `grove-1.3.0/grove/connectors/workday/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/zoom/activities.py` & `grove-1.3.0/grove/connectors/zoom/activities.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/zoom/api.py` & `grove-1.3.0/grove/connectors/zoom/api.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/connectors/zoom/operationlogs.py` & `grove-1.3.0/grove/connectors/zoom/operationlogs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/constants.py` & `grove-1.3.0/grove/constants.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/entrypoints/aws_lambda.py` & `grove-1.3.0/grove/entrypoints/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/entrypoints/base.py` & `grove-1.3.0/grove/entrypoints/base.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/entrypoints/local_process.py` & `grove-1.3.0/grove/entrypoints/local_process.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/exceptions.py` & `grove-1.3.0/grove/exceptions.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/helpers/parsing.py` & `grove-1.3.0/grove/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/helpers/plugin.py` & `grove-1.3.0/grove/helpers/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     use by Grove.
 
     :param name: The name of the handler to load (e.g. 'aws_ssm').
     :param group: The group the handler belongs to (e.g. 'grove.outputs').
 
     :raises ConfigurationException: The specified handler could not be located.
     """
-    # The 'group' kwarg for entry_points was added in Python 3.10, in order to support
-    # older versions of Python 3 we will not be using this feature. Additionally, using
-    # get() will raise deprecation warnings to use select() instead. However, select()
-    # was also added in Python 3.10, which would break backwards compatibility...
-    eps = entry_points()
+    # Handle differences between importlib in Python 3.9, 3.10, and Python 3.12.
+    try:
+        entrypoints = entry_points().select(group=group)
+    except AttributeError:
+        entrypoints = entry_points().get(group, ())  # type: ignore
 
-    for candidate in eps.get(group, []):
+    for candidate in entrypoints:
         if candidate.name == name:
             return candidate
 
     raise ConfigurationException(
         f"Requested handler could not be found with name '{name}' (group '{group}')"
     )
```

### Comparing `grove-1.2.2/grove/logging.py` & `grove-1.3.0/grove/logging.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/models.py` & `grove-1.3.0/grove/models.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/outputs/__init__.py` & `grove-1.3.0/grove/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/outputs/aws_s3.py` & `grove-1.3.0/grove/outputs/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/outputs/local_file.py` & `grove-1.3.0/grove/outputs/local_file.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/outputs/local_stdout.py` & `grove-1.3.0/grove/outputs/local_stdout.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/__init__.py` & `grove-1.3.0/grove/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/extract_paths.py` & `grove-1.3.0/grove/processors/extract_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/filter_entries.py` & `grove-1.3.0/grove/processors/filter_entries.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/filter_paths.py` & `grove-1.3.0/grove/processors/filter_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/split_path.py` & `grove-1.3.0/grove/processors/split_path.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/processors/zip_paths.py` & `grove-1.3.0/grove/processors/zip_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/secrets/__init__.py` & `grove-1.3.0/grove/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/secrets/aws_ssm.py` & `grove-1.3.0/grove/secrets/aws_ssm.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/secrets/hashicorp_vault.py` & `grove-1.3.0/grove/secrets/hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/secrets/local_file.py` & `grove-1.3.0/grove/secrets/local_file.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove/types.py` & `grove-1.3.0/grove/types.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/grove.egg-info/PKG-INFO` & `grove-1.3.0/grove.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grove
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Software as a Service (SaaS) log collection framework.
 Author: HashiCorp Security (TDR)
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: boto3<2.0,>=1.26
 Requires-Dist: requests<3.0,>=2.28
 Requires-Dist: google-api-python-client<3.0,>=2.68
 Requires-Dist: simple-salesforce<2.0,>=1.12
 Requires-Dist: twilio<8.0,>=7.15
 Requires-Dist: pydantic<2.0,>=1.10
 Requires-Dist: jmespath<2.0,>=1.0.0
+Requires-Dist: stripe<9.0,>=8.4.0
 Provides-Extra: tests
 Requires-Dist: black; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: mypy; extra == "tests"
@@ -29,15 +30,15 @@
 Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: responses; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: sphinx; extra == "tests"
 Requires-Dist: furo; extra == "tests"
-Requires-Dist: moto[s3,ssm]; extra == "tests"
+Requires-Dist: moto[s3,ssm]<5.0,>=4.0; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 
 <p align="center">
     <br /><br />
     <picture>
       <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/hashicorp-forge/grove/main/docs/static/grove-logo-small-light.png?raw=True">
       <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/hashicorp-forge/grove/main/docs/static/grove-logo-small.png?raw=True">
```

### Comparing `grove-1.2.2/grove.egg-info/SOURCES.txt` & `grove-1.3.0/grove.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 grove/connectors/sfmc/__init__.py
 grove/connectors/sfmc/api.py
 grove/connectors/sfmc/audit_events.py
 grove/connectors/sfmc/security_events.py
 grove/connectors/slack/__init__.py
 grove/connectors/slack/api.py
 grove/connectors/slack/audit_logs.py
+grove/connectors/stripe/__init__.py
+grove/connectors/stripe/events.py
 grove/connectors/tfc/__init__.py
 grove/connectors/tfc/api.py
 grove/connectors/tfc/audit_trails.py
 grove/connectors/tines/__init__.py
 grove/connectors/tines/api.py
 grove/connectors/tines/audit_logs.py
 grove/connectors/torq/__init__.py
@@ -164,14 +166,15 @@
 templates/configuration/gsuite/flattened_drive_activities.json
 templates/configuration/okta/preview_system_log.json
 templates/configuration/okta/system_log.json
 templates/configuration/oomnitza/activities.json
 templates/configuration/pagerduty/audit_records.json
 templates/configuration/salesforce/event_log.json
 templates/configuration/slack/audit_logs.json
+templates/configuration/stripe/events.json
 templates/configuration/tfc/audit_trails.json
 templates/configuration/tines/audit_logs.json
 templates/configuration/torq/activity_logs.json
 templates/configuration/torq/audit_logs.json
 templates/configuration/twilio/messages.json
 templates/configuration/twilio/monitor_events.json
 templates/configuration/workday/activity_logging.json
@@ -212,14 +215,15 @@
 tests/test_connectors_onepassword_events_signinattempts.py
 tests/test_connectors_oomnitza_activities.py
 tests/test_connectors_pagerduty_audit_records.py
 tests/test_connectors_sf_event_log.py
 tests/test_connectors_sfmc_audit_events.py
 tests/test_connectors_sfmc_security_events.py
 tests/test_connectors_slack_audit.py
+tests/test_connectors_stripe_events.py
 tests/test_connectors_tfc_audit_trails.py
 tests/test_connectors_tines_audit_logs.py
 tests/test_connectors_torq_activity_logs.py
 tests/test_connectors_torq_audit_logs.py
 tests/test_connectors_torq_clients.py
 tests/test_connectors_workday_activity_logging.py
 tests/test_connectors_zoom_activities.py
@@ -280,14 +284,16 @@
 tests/fixtures/sfmc/audit_events/003.json
 tests/fixtures/sfmc/security_events/001.json
 tests/fixtures/sfmc/security_events/002.json
 tests/fixtures/sfmc/security_events/003.json
 tests/fixtures/slack/audit/001.json
 tests/fixtures/slack/audit/002.json
 tests/fixtures/slack/audit/003.json
+tests/fixtures/stripe/events/001.json
+tests/fixtures/stripe/events/002.json
 tests/fixtures/tfc/audit_trails/001.json
 tests/fixtures/tfc/audit_trails/002.json
 tests/fixtures/tfc/audit_trails/003.json
 tests/fixtures/tfc/audit_trails/004.json
 tests/fixtures/tines/audit_logs/001.json
 tests/fixtures/tines/audit_logs/002.json
 tests/fixtures/tines/audit_logs/003.json
```

### Comparing `grove-1.2.2/grove.egg-info/entry_points.txt` & `grove-1.3.0/grove.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 onepassword_events_signinattempts = grove.connectors.onepassword.events_signinattempts:Connector
 oomnitza_activities = grove.connectors.oomnitza.activities:Connector
 pagerduty_audit_records = grove.connectors.pagerduty.audit_records:Connector
 sf_event_log = grove.connectors.sf.event_log:Connector
 sfmc_audit_events = grove.connectors.sfmc.audit_events:Connector
 sfmc_security_events = grove.connectors.sfmc.security_events:Connector
 slack_audit_logs = grove.connectors.slack.audit_logs:Connector
+stripe_events = grove.connectors.stripe.events:Connector
 tfc_audit_trails = grove.connectors.tfc.audit_trails:Connector
 tines_audit_logs = grove.connectors.tines.audit_logs:Connector
 torq_activity_logs = grove.connectors.torq.activity_logs:Connector
 torq_audit_logs = grove.connectors.torq.audit_logs:Connector
 twilio_messages = grove.connectors.twilio.messages:Connector
 twilio_monitor_events = grove.connectors.twilio.monitor_events:Connector
 workday_activity_logging = grove.connectors.workday.activity_logging:Connector
```

### Comparing `grove-1.2.2/pyproject.toml` & `grove-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "boto3>=1.26,<2.0",
     "requests>=2.28,<3.0",
     "google-api-python-client>=2.68,<3.0",
     "simple-salesforce>=1.12,<2.0",
     "twilio>=7.15,<8.0",
     "pydantic>=1.10,<2.0",
     "jmespath>=1.0.0,<2.0",
+    "stripe>=8.4.0,<9.0",
 ]
 
 [project.optional-dependencies]
 tests = [
     "black",
     "coverage",
     "ruff",
@@ -38,15 +39,15 @@
     "mock",
     "pytest",
     "pytest-cov",
     "responses",
     "tox",
     "sphinx",
     "furo",
-    "moto[s3,ssm]",
+    "moto[s3,ssm]>=4.0,<5.0",
     "types-requests",
 ]
 
 [tool.setuptools.packages.find]
 include = ["grove*"]
 
 [tool.setuptools.dynamic]
@@ -70,14 +71,15 @@
 onepassword_events_signinattempts = "grove.connectors.onepassword.events_signinattempts:Connector"
 onepassword_events_audit = "grove.connectors.onepassword.events_audit:Connector"
 pagerduty_audit_records = "grove.connectors.pagerduty.audit_records:Connector"
 sf_event_log = "grove.connectors.sf.event_log:Connector"
 sfmc_audit_events = "grove.connectors.sfmc.audit_events:Connector"
 sfmc_security_events = "grove.connectors.sfmc.security_events:Connector"
 slack_audit_logs = "grove.connectors.slack.audit_logs:Connector"
+stripe_events = "grove.connectors.stripe.events:Connector"
 tines_audit_logs = "grove.connectors.tines.audit_logs:Connector"
 tfc_audit_trails = "grove.connectors.tfc.audit_trails:Connector"
 torq_activity_logs = "grove.connectors.torq.activity_logs:Connector"
 torq_audit_logs = "grove.connectors.torq.audit_logs:Connector"
 twilio_monitor_events = "grove.connectors.twilio.monitor_events:Connector"
 twilio_messages = "grove.connectors.twilio.messages:Connector"
 workday_activity_logging = "grove.connectors.workday.activity_logging:Connector"
@@ -111,15 +113,15 @@
 zip_paths = "grove.processors.zip_paths:Handler"
 
 [tool.mypy]
 files = [
     "./grove/**/*.py",
     "./tests/**/*.py"
 ]
-disable_error_code = "attr-defined, union-attr"
+disable_error_code = "attr-defined, union-attr, unused-ignore"
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_untyped_calls = false
 ignore_errors = false
 ignore_missing_imports = true
 implicit_reexport = false
```

### Comparing `grove-1.2.2/templates/README.md` & `grove-1.3.0/templates/README.md`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/README.md` & `grove-1.3.0/templates/code/README.md`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/cookiecutter.json` & `grove-1.3.0/templates/code/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/hooks/post_gen_project.py` & `grove-1.3.0/templates/code/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.github/workflows/release.yml` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.gitignore` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/.vscode/settings.json` & `grove-1.3.0/.vscode/settings.json`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {
     "python.linting.enabled": true,
     "python.formatting.provider": "none",
     "[python]": {
         "editor.formatOnSave": true,
         "editor.codeActionsOnSave": {
-            "source.organizeImports": true,
+            "source.organizeImports": "explicit"
         },
         "editor.defaultFormatter": "ms-python.black-formatter",
     },
     "editor.rulers": [
         88
     ],
     "[terraform]": {
```

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/pyproject.toml` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/example_logs.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/example_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/caches.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/caches.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/configs.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/configs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/outputs.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/outputs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/processors.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/processors.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/secrets.py` & `grove-1.3.0/templates/code/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/inits/secrets.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/configuration/gsuite/flattened_drive_activities.json` & `grove-1.3.0/templates/configuration/gsuite/flattened_drive_activities.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/README.md` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/README.md`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/main.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/main.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/cloudwatch.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/cloudwatch.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/compute.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/compute.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/iam.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/iam.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/network.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/network.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/s3.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/s3.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/templates/deployment/terraform-aws-ecs/modules/grove/variables.tf` & `grove-1.3.0/templates/deployment/terraform-aws-ecs/modules/grove/variables.tf`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/connectors/test.py` & `grove-1.3.0/tests/connectors/test.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/atlassian/event_audit/001.json` & `grove-1.3.0/tests/fixtures/atlassian/event_audit/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/atlassian/event_audit/002.json` & `grove-1.3.0/tests/fixtures/atlassian/event_audit/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/github/audit/001.json` & `grove-1.3.0/tests/fixtures/github/audit/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/github/audit/002.json` & `grove-1.3.0/tests/fixtures/github/audit/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/github/git/001.json` & `grove-1.3.0/tests/fixtures/github/git/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/gsuite/activities/001.json` & `grove-1.3.0/tests/fixtures/gsuite/activities/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/gsuite/activities/002.json` & `grove-1.3.0/tests/fixtures/gsuite/activities/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/gsuite/activities/003.json` & `grove-1.3.0/tests/fixtures/gsuite/activities/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/gsuite/alerts/001.json` & `grove-1.3.0/tests/fixtures/gsuite/alerts/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/gsuite/alerts/002.json` & `grove-1.3.0/tests/fixtures/gsuite/alerts/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/okta/system_log/001.json` & `grove-1.3.0/tests/fixtures/okta/system_log/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_audit/001.json` & `grove-1.3.0/tests/fixtures/onepassword/events_audit/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_audit/002.json` & `grove-1.3.0/tests/fixtures/onepassword/events_audit/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_audit/003.json` & `grove-1.3.0/tests/fixtures/onepassword/events_audit/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_itemusages/001.json` & `grove-1.3.0/tests/fixtures/onepassword/events_itemusages/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_itemusages/002.json` & `grove-1.3.0/tests/fixtures/onepassword/events_itemusages/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_itemusages/003.json` & `grove-1.3.0/tests/fixtures/onepassword/events_itemusages/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/001.json` & `grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/002.json` & `grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/onepassword/events_signinattempts/003.json` & `grove-1.3.0/tests/fixtures/onepassword/events_signinattempts/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/oomnitza/activities/001.json` & `grove-1.3.0/tests/fixtures/oomnitza/activities/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/oomnitza/activities/002.json` & `grove-1.3.0/tests/fixtures/oomnitza/activities/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/pagerduty/audit_records/001.json` & `grove-1.3.0/tests/fixtures/pagerduty/audit_records/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/pagerduty/audit_records/002.json` & `grove-1.3.0/tests/fixtures/pagerduty/audit_records/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/pagerduty/audit_records/003.json` & `grove-1.3.0/tests/fixtures/pagerduty/audit_records/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sf/event_log/001.csv` & `grove-1.3.0/tests/fixtures/sf/event_log/001.csv`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sf/event_log/login.xml` & `grove-1.3.0/tests/fixtures/sf/event_log/login.xml`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/audit_events/001.json` & `grove-1.3.0/tests/fixtures/sfmc/audit_events/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/audit_events/002.json` & `grove-1.3.0/tests/fixtures/sfmc/audit_events/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/audit_events/003.json` & `grove-1.3.0/tests/fixtures/sfmc/audit_events/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/security_events/001.json` & `grove-1.3.0/tests/fixtures/sfmc/security_events/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/security_events/002.json` & `grove-1.3.0/tests/fixtures/sfmc/security_events/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/sfmc/security_events/003.json` & `grove-1.3.0/tests/fixtures/sfmc/security_events/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/slack/audit/001.json` & `grove-1.3.0/tests/fixtures/slack/audit/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/slack/audit/002.json` & `grove-1.3.0/tests/fixtures/slack/audit/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/slack/audit/003.json` & `grove-1.3.0/tests/fixtures/slack/audit/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tfc/audit_trails/001.json` & `grove-1.3.0/tests/fixtures/tfc/audit_trails/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tfc/audit_trails/002.json` & `grove-1.3.0/tests/fixtures/tfc/audit_trails/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tfc/audit_trails/003.json` & `grove-1.3.0/tests/fixtures/tfc/audit_trails/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tfc/audit_trails/004.json` & `grove-1.3.0/tests/fixtures/tfc/audit_trails/004.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tines/audit_logs/001.json` & `grove-1.3.0/tests/fixtures/tines/audit_logs/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tines/audit_logs/002.json` & `grove-1.3.0/tests/fixtures/tines/audit_logs/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/tines/audit_logs/003.json` & `grove-1.3.0/tests/fixtures/tines/audit_logs/003.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/torq/activity/001.json` & `grove-1.3.0/tests/fixtures/torq/activity/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/torq/activity/002.json` & `grove-1.3.0/tests/fixtures/torq/activity/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/torq/audit/001.json` & `grove-1.3.0/tests/fixtures/torq/audit/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/torq/audit/002.json` & `grove-1.3.0/tests/fixtures/torq/audit/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/workday/activity_logging/002.json` & `grove-1.3.0/tests/fixtures/workday/activity_logging/002.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/workday/activity_logging/004.json` & `grove-1.3.0/tests/fixtures/workday/activity_logging/004.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/zoom/activities/001.json` & `grove-1.3.0/tests/fixtures/zoom/activities/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/fixtures/zoom/operation/001.json` & `grove-1.3.0/tests/fixtures/zoom/operation/001.json`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/mocks/__init__.py` & `grove-1.3.0/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_caches_local_memory.py` & `grove-1.3.0/tests/test_caches_local_memory.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_configs_aws_ssm.py` & `grove-1.3.0/tests/test_configs_aws_ssm.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_atlassian_audit_events.py` & `grove-1.3.0/tests/test_connectors_atlassian_audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_base.py` & `grove-1.3.0/tests/test_connectors_base.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_deduplicate.py` & `grove-1.3.0/tests/test_connectors_deduplicate.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_github_audit.py` & `grove-1.3.0/tests/test_connectors_github_audit.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_github_client.py` & `grove-1.3.0/tests/test_connectors_github_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_gsuite_activities.py` & `grove-1.3.0/tests/test_connectors_okta_system_log.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements integration tests for the GSuite Activities collector."""
+"""Implements unit tests for the Okta SystemLog API collector."""
 
 import os
+import re
 import unittest
 from unittest.mock import patch
 
-from googleapiclient.http import HttpMockSequence
+import responses
 
-from grove.connectors.gsuite.activities import Connector
+from grove.connectors.okta.system_log import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class MockSequence(HttpMockSequence):
-    def close(self, *args, **kwargs):
-        pass
-
-
-class GSuiteActivitiesTestCase(unittest.TestCase):
-    """Implements integration tests for the GSuite Activities collector."""
+class OktaAuditTestCase(unittest.TestCase):
+    """Implements unit tests for the Okta SystemLog Audit collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="1FEEDFEED1",
-                key="{}",
-                name="test",
+                identity="example",
+                key="token",
+                name="examplecorp",
                 connector="test",
-                operation="admin",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
-    @patch("google.oauth2.service_account.Credentials.from_service_account_info")
-    @patch("googleapiclient.discovery.build")
-    @patch("grove.connectors.gsuite.activities.Connector.get_http_transport")
-    def test_collect_pagination(self, mock_transport, mock_request, mock_auth):
-        """Ensure collection works as expected."""
-        mock_transport.return_value = MockSequence(
-            [
-                (
-                    {"status": "200"},
-                    open(
-                        os.path.join(self.dir, "fixtures/gsuite/activities/001.json"),
-                        "r",
-                    ).read(),
-                ),
-                (
-                    {"status": "200"},
-                    open(
-                        os.path.join(self.dir, "fixtures/gsuite/activities/002.json"),
-                        "r",
-                    ).read(),
-                ),
-            ],
+    @responses.activate
+    def test_client_rate_limit(self):
+        """Ensure ratelimit waiting is working as expected."""
+        # Rate limit the first request.
+        responses.add(
+            responses.GET,
+            re.compile(r"https://.*"),
+            status=429,
+            content_type="application/json",
+            body=bytes(),
+            headers={
+                "X-Rate-Limit-Remaining": "0",
+                "X-Rate-Limit-Reset": "0",  # Unix-time, so definitely in the past :)
+            },
+        )
+
+    @responses.activate
+    def test_collect_no_pagination(self):
+        """Ensure collection without pagination is working as expected."""
+        responses.add(
+            responses.GET,
+            re.compile(r"https://.*"),
+            status=200,
+            content_type="application/json",
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/okta/system_log/001.json"), "r"
+                ).read(),
+                "utf-8",
+            ),
         )
+        # Ensure only a single value is returned, and the pointer is properly set.
         self.connector.run()
+        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector.pointer, "2021-06-24T00:04:08.123Z")
 
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2021-10-27T23:59:31.657Z")
+    @responses.activate
+    def test_collect_no_results(self):
+        """Ensure break occurs when there is no results returned."""
+        responses.add(
+            responses.GET,
+            re.compile(r"https://.*"),
+            status=200,
+            content_type="application/json",
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/okta/system_log/002.json"), "r"
+                ).read(),
+                "utf-8",
+            ),
+        )
```

### Comparing `grove-1.2.2/tests/test_connectors_gsuite_alerts.py` & `grove-1.3.0/tests/test_connectors_gsuite_alerts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
 """Implements integration tests for the GSuite Alerts collector."""
 
 import os
 import unittest
-from unittest.mock import patch
+from unittest.mock import Mock, patch
 
+from google.auth.credentials import Credentials
 from googleapiclient.http import HttpMockSequence
 
 from grove.connectors.gsuite.alerts import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
@@ -35,19 +36,23 @@
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
-    @patch("google.oauth2.service_account.Credentials.from_service_account_info")
     @patch("googleapiclient.discovery.build")
+    @patch("grove.connectors.gsuite.alerts.Connector.get_credentials")
     @patch("grove.connectors.gsuite.alerts.Connector.get_http_transport")
-    def test_collect_pagination(self, mock_transport, mock_request, mock_auth):
+    def test_collect_pagination(self, mock_transport, mock_auth, mock_request):
         """Ensure collection works as expected."""
+        credentials = Mock(spec=Credentials)
+        credentials.universe_domain = "googleapis.com"
+        mock_auth.return_value = credentials
+
         mock_transport.return_value = MockSequence(
             [
                 (
                     {"status": "200"},
                     open(
                         os.path.join(self.dir, "fixtures/gsuite/alerts/001.json"),
                         "r",
```

### Comparing `grove-1.2.2/tests/test_connectors_lock.py` & `grove-1.3.0/tests/test_connectors_lock.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_okta_client.py` & `grove-1.3.0/tests/test_connectors_okta_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_okta_system_log.py` & `grove-1.3.0/tests/test_connectors_tines_audit_logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,91 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements unit tests for the Okta SystemLog API collector."""
+"""Implements integration tests for the Tines Audit Log collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.okta.system_log import Connector
+from grove.connectors.tines.audit_logs import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class OktaAuditTestCase(unittest.TestCase):
-    """Implements unit tests for the Okta SystemLog Audit collector."""
+class TinesAuditTestCase(unittest.TestCase):
+    """Implements integration tests for the Tines Audit collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
-                identity="example",
+                identity="1FEEDFEED1",
                 key="token",
-                name="examplecorp",
+                name="test",
                 connector="test",
             ),
             context={
                 "runtime": "test_harness",
                 "runtime_id": "NA",
             },
         )
 
     @responses.activate
-    def test_client_rate_limit(self):
-        """Ensure ratelimit waiting is working as expected."""
-        # Rate limit the first request.
+    def test_collect_pagination(self):
+        """Ensure pagination is working as expected."""
+        # Succeed with a cursor returned (to indicate paging is required).
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
-            status=429,
+            status=200,
             content_type="application/json",
-            body=bytes(),
-            headers={
-                "X-Rate-Limit-Remaining": "0",
-                "X-Rate-Limit-Reset": "0",  # Unix-time, so definitely in the past :)
-            },
+            body=bytes(
+                open(
+                    os.path.join(self.dir, "fixtures/tines/audit_logs/001.json"), "r"
+                ).read(),
+                "utf-8",
+            ),
         )
 
-    @responses.activate
-    def test_collect_no_pagination(self):
-        """Ensure collection without pagination is working as expected."""
+        # The last "page" returns an empty cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/okta/system_log/001.json"), "r"
+                    os.path.join(self.dir, "fixtures/tines/audit_logs/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
-        # Ensure only a single value is returned, and the pointer is properly set.
+
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 1)
-        self.assertEqual(self.connector.pointer, "2021-06-24T00:04:08.123Z")
+        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector.pointer, "2023-07-21T14:21:30Z")
 
     @responses.activate
-    def test_collect_no_results(self):
-        """Ensure break occurs when there is no results returned."""
+    def test_collect_no_pagination(self):
+        """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/okta/system_log/002.json"), "r"
+                    os.path.join(self.dir, "fixtures/tines/audit_logs/003.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
+
+        self.connector.run()
+        self.assertEqual(self.connector._saved["logs"], 2)
+        self.assertEqual(self.connector.pointer, "2023-07-21T10:32:37Z")
```

### Comparing `grove-1.2.2/tests/test_connectors_onepassword_events_audit.py` & `grove-1.3.0/tests/test_connectors_onepassword_events_audit.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_onepassword_events_itemusages.py` & `grove-1.3.0/tests/test_connectors_onepassword_events_itemusages.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_onepassword_events_signinattempts.py` & `grove-1.3.0/tests/test_connectors_onepassword_events_signinattempts.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_oomnitza_activities.py` & `grove-1.3.0/tests/test_connectors_oomnitza_activities.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_pagerduty_audit_records.py` & `grove-1.3.0/tests/test_connectors_pagerduty_audit_records.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_sf_event_log.py` & `grove-1.3.0/tests/test_connectors_sf_event_log.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_sfmc_audit_events.py` & `grove-1.3.0/tests/test_connectors_sfmc_audit_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_sfmc_security_events.py` & `grove-1.3.0/tests/test_connectors_sfmc_security_events.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_slack_audit.py` & `grove-1.3.0/tests/test_connectors_slack_audit.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_tfc_audit_trails.py` & `grove-1.3.0/tests/test_connectors_tfc_audit_trails.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_tines_audit_logs.py` & `grove-1.3.0/tests/test_connectors_stripe_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) HashiCorp, Inc.
 # SPDX-License-Identifier: MPL-2.0
 
-"""Implements integration tests for the Tines Audit Log collector."""
+"""Implements integration tests for the Stripe Events collector."""
 
 import os
 import re
 import unittest
 from unittest.mock import patch
 
 import responses
 
-from grove.connectors.tines.audit_logs import Connector
+from grove.connectors.stripe.events import Connector
 from grove.models import ConnectorConfig
 from tests import mocks
 
 
-class TinesAuditTestCase(unittest.TestCase):
-    """Implements integration tests for the Tines Audit collector."""
+class StripeEventsTestCase(unittest.TestCase):
+    """Implements integration tests for the Stripe Events collector."""
 
     @patch("grove.helpers.plugin.load_handler", mocks.load_handler)
     def setUp(self):
         """Ensure the application is setup for testing."""
         self.dir = os.path.dirname(os.path.abspath(__file__))
         self.connector = Connector(
             config=ConnectorConfig(
@@ -42,50 +42,50 @@
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/001.json"), "r"
+                    os.path.join(self.dir, "fixtures/stripe/events/001.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         # The last "page" returns an empty cursor.
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/002.json"), "r"
+                    os.path.join(self.dir, "fixtures/stripe/events/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
         self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2023-07-21T14:21:30Z")
+        self.assertEqual(self.connector.pointer, "evt_1OonDcGsC9LSOJDcarfWbL08")
 
     @responses.activate
     def test_collect_no_pagination(self):
         """Ensure collection without pagination is working as expected."""
         responses.add(
             responses.GET,
             re.compile(r"https://.*"),
             status=200,
             content_type="application/json",
             body=bytes(
                 open(
-                    os.path.join(self.dir, "fixtures/tines/audit_logs/003.json"), "r"
+                    os.path.join(self.dir, "fixtures/stripe/events/002.json"), "r"
                 ).read(),
                 "utf-8",
             ),
         )
 
         self.connector.run()
-        self.assertEqual(self.connector._saved["logs"], 2)
-        self.assertEqual(self.connector.pointer, "2023-07-21T10:32:37Z")
+        self.assertEqual(self.connector._saved["logs"], 1)
+        self.assertEqual(self.connector.pointer, "evt_1OonDcGsC9LSOJDcarfWbL10")
```

### Comparing `grove-1.2.2/tests/test_connectors_torq_activity_logs.py` & `grove-1.3.0/tests/test_connectors_torq_activity_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_torq_audit_logs.py` & `grove-1.3.0/tests/test_connectors_torq_audit_logs.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_torq_clients.py` & `grove-1.3.0/tests/test_connectors_torq_clients.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_workday_activity_logging.py` & `grove-1.3.0/tests/test_connectors_workday_activity_logging.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_zoom_activities.py` & `grove-1.3.0/tests/test_connectors_zoom_activities.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_zoom_client.py` & `grove-1.3.0/tests/test_connectors_zoom_client.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_connectors_zoom_operation.py` & `grove-1.3.0/tests/test_connectors_zoom_operation.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_e2e_grove_cli.py` & `grove-1.3.0/tests/test_e2e_grove_cli.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_helpers_parsing.py` & `grove-1.3.0/tests/test_helpers_parsing.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_outputs_aws_s3.py` & `grove-1.3.0/tests/test_outputs_aws_s3.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_outputs_base.py` & `grove-1.3.0/tests/test_outputs_base.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_processors_extract_paths.py` & `grove-1.3.0/tests/test_processors_extract_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_processors_filter_entries.py` & `grove-1.3.0/tests/test_processors_filter_entries.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_processors_filter_paths.py` & `grove-1.3.0/tests/test_processors_filter_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_processors_split_path.py` & `grove-1.3.0/tests/test_processors_split_path.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_processors_zip_paths.py` & `grove-1.3.0/tests/test_processors_zip_paths.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_secrets_hashicorp_vault.py` & `grove-1.3.0/tests/test_secrets_hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `grove-1.2.2/tests/test_secrets_local_file.py` & `grove-1.3.0/tests/test_secrets_local_file.py`

 * *Files identical despite different names*

