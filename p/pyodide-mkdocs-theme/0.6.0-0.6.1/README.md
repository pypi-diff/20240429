# Comparing `tmp/pyodide_mkdocs_theme-0.6.0.tar.gz` & `tmp/pyodide_mkdocs_theme-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.6.0.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.6.1.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.6.0.tar` & `pyodide_mkdocs_theme-0.6.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.6.0/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.6.0/README.md
--rw-r--r--   0        0        0     1347 2024-04-27 20:26:28.022032 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-27 20:25:34.956498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-27 20:26:28.054032 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4996 2024-04-27 20:25:34.976498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    22407 2024-04-27 20:25:34.976498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    16081 2024-04-27 20:25:34.976498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:25:34.980498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     3861 2024-04-27 20:25:34.980498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11723 2024-04-27 20:25:34.980498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13163 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4485 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    12435 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11736 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     6420 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0    10204 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8198 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-27 20:26:28.010031 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6909 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3979 2024-04-27 20:26:28.022032 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5565 2024-04-27 20:25:34.992498 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3791 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6642 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9830 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6607 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16619 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0    10269 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9297 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3740 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5379 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4203 2024-04-25 15:11:28.669398 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1761 2024-04-27 20:26:25.521959 pyodide_mkdocs_theme-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.6.1/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.6.1/README.md
+-rw-r--r--   0        0        0     1347 2024-04-29 14:09:17.377380 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-29 14:09:17.421381 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4996 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    22407 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    16081 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     3861 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11723 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13163 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4485 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    12267 2024-04-27 23:06:40.767927 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11736 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     6420 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0    10204 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     8198 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0      374 2024-04-28 09:15:25.683143 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6909 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3979 2024-04-29 14:09:17.373380 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5565 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     5387 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7420 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1702 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6642 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9831 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6753 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16617 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0    11246 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9195 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3740 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5379 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4201 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1761 2024-04-29 14:09:14.657299 pyodide_mkdocs_theme-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.6.1/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.6.0/LICENSE` & `pyodide_mkdocs_theme-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/README.md` & `pyodide_mkdocs_theme-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,14 @@
 
     load_yaml_encoding = C.Type(str, default='utf-8')
     """
     Encoding to use when loading yaml data with the original MacrosPlugin functionalities :
 
     The original method doesn't use any encoding argument, which can lead to different behaviors
     between Windows and Linux (typically: during a pipeline!).
-
-    ??? note "Should be removed in the future"
-        PR has been posted with the change on their repo. If ever it gets merged, this will
-        have to be updated.
     """
 
 
     macros_with_indents = C.ListOfItems(C.Type(str), default=[])
     """
     Allow to register external macros, as a list of strings, that will need to insert properly
     indented multiline contents in the page.
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,12 +13,7 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-""" Generated file, do not modify """
-
-SCRIPTS_TEMPLATES = {
-    "pyodide": "<link rel=\"stylesheet\" href=\"{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/perPageScripts/start-pyodide.css\">\n<script type=\"application/javascript\" src=\"{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/perPageScripts/start-pyodide.js\"></script>"
-}
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -136,14 +136,17 @@
 
 
     cutFeedback: true,
 
     COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
     // HDR_TOKEN_PATTERN:   /#\s*-[\s-]*HDR\s*-[\s-]*#/i,           // not used anymore
 
+    MODULE_REG: /File "<(env|exec|console)>", line (\d+)($|, in (?!await_fut))/,
+    TRACE_REG: /  File "<(env|exec|console)>"/,
+    TRACE_NUM_LINE: /File "<(?:env|exec|console)>", line (\d+)/,
 
     ACE_COLOR_THEME: {
         customTheme: undefined,
         customThemeDefaultKey: "",
         aceStyle: undefined,
     },
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -131,23 +131,25 @@
 
 
 
 
 
 
 /**Square brackets in "rich text format" must be escaped, otherwise they are messing up the
- * terminal formatting informations
+ * terminal formatting informations.
  * */
-const escapeSquareBrackets = msg => {
+function escapeSquareBrackets(msg) {
     return msg.replace(/\[/g, CONFIG.MSG.leftSafeSqbr)
         .replace(/\]/g, CONFIG.MSG.rightSafeSqbr)
 }
 
 
 /**Formatting factory function, for messages used in the jquery terminal.
+ *
+ * WARNING: the input message will be "escapeSquareBrackets"-ed.
  * */
 function richTextFormat(content, style, color = "", background = "") {
     content = escapeSquareBrackets(content)
     return `[[${ style };${ color };${ background }]${ content }]`;
 }
 
 let error = (content) => richTextFormat(content, "b", "red");
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -19,14 +19,15 @@
 
 /** The options can be modified at runtime on user's side, to ease debugging.
  * */
 CONFIG.loggerOptions = {
     ACTIVATE: false,
     all: false,
 
+    AroundSearch: false,
     Feature: false,
     HourGlass: false,
     LOCK: false,
     MathJax: false,
     Paint_ACEs: false,
     QCM: true,
     Scroll: false,
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,40 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
+
+// Insertion of the placeholders, around the search bar.
+
+subscribeWhenReady(
+    "AroundSearch",
+    function() {
+        jsLogger('[AroundSearch]', 'left')
+        const wrappingDivL = `<div id="${ CONFIG.element.searchBtnsLeft.slice(1)  }"></div>`
+        $(wrappingDivL).insertBefore(CONFIG.element.dayNight)
+    }, {
+        waitFor: CONFIG.element.dayNight
+    },
+)
+subscribeWhenReady(
+    "AroundSearch",
+    function() {
+        jsLogger('[AroundSearch]', 'right')
+        const wrappingDivR = `<div id="${ CONFIG.element.searchBtnsRight.slice(1) }"></div>`
+        $(wrappingDivR).insertAfter(CONFIG.element.searchBlock)
+    }, {
+        waitFor: CONFIG.element.searchBlock
+    },
+)
+
+
+
 /**Insertion of the trash icon/button
  * */
 subscribeWhenReady(
     "TrashCan",
     function() {
         jsLogger('[TrashCan]')
 
@@ -38,16 +64,15 @@
         const trashBtnOptions = {
             shift: 90,
             tipText: CONFIG.lang.tipTrash.msg,
             tipWidth: CONFIG.lang.tipTrash.em
         }
 
         const trashButtonCode = buttonWithTooltip(trashBtnOptions, TRASH_SVG)
-        const wrappingDiv = `<div id="${ CONFIG.element.searchBtnsRight.slice(1) }">${ trashButtonCode }</div>`
-        $(wrappingDiv).insertAfter(CONFIG.element.searchBlock).on('click', function() {
+        $(trashButtonCode).insertAfter(CONFIG.element.searchBlock).on('click', function() {
 
             const data = Object.keys(localStorage)
             const codes = data.filter(s => /^editor_[\da-f]{16,}$/.test(s))
             const cmds = data.filter(s => /^\d+_commands$/.test(s))
 
 
             if (!codes.length) {
@@ -61,10 +86,10 @@
             }
 
             cmds.forEach(k => {
                 localStorage.setItem(k, "[]")
             })
         })
     }, {
-        waitFor: CONFIG.element.searchBlock
+        waitFor: CONFIG.element.searchBtnsRight
     },
 )
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text*

 * *Files 1% similar despite different names*

```diff
@@ -54,562 +54,562 @@
 00000350: 2865 2026 2620 652e 7072 6576 656e 7444  (e && e.preventD
 00000360: 6566 6175 6c74 2920 652e 7072 6576 656e  efault) e.preven
 00000370: 7444 6566 6175 6c74 2829 0a0a 2020 2020  tDefault()..    
 00000380: 6177 6169 7420 7761 6974 466f 7250 796f  await waitForPyo
 00000390: 6469 6465 5265 6164 7928 293b 0a20 2020  dideReady();.   
 000003a0: 206a 734c 6f67 6765 7228 225b 506c 6179   jsLogger("[Play
 000003b0: 5d22 290a 0a20 2020 206c 6574 205b 636f  ]")..    let [co
-000003c0: 6465 2c74 6572 6d69 6e61 6c2c 206f 7074  de,terminal, opt
-000003d0: 696f 6e73 5d20 3d20 6177 6169 7420 7365  ions] = await se
-000003e0: 7475 7052 756e 7469 6d65 416e 6454 6572  tupRuntimeAndTer
-000003f0: 6d69 6e61 6c28 6564 6974 6f72 4e61 6d65  minal(editorName
-00000400: 293b 0a20 2020 206c 6574 2073 7464 4572  );.    let stdEr
-00000410: 723d 2222 0a0a 2020 2020 7472 797b 0a20  r=""..    try{. 
-00000420: 2020 2020 2020 2073 7464 4572 7220 3d20         stdErr = 
-00000430: 6177 6169 7420 7275 6e50 7974 686f 6e43  await runPythonC
-00000440: 6f64 6557 6974 684f 7074 696f 6e73 2863  odeWithOptions(c
-00000450: 6f64 652c 2074 6572 6d69 6e61 6c2c 206f  ode, terminal, o
-00000460: 7074 696f 6e73 2c20 7472 7565 290a 2020  ptions, true).  
-00000470: 2020 7d66 696e 616c 6c79 7b0a 2020 2020    }finally{.    
-00000480: 2020 2020 7465 6172 446f 776e 5275 6e74      tearDownRunt
-00000490: 696d 6541 6e64 5465 726d 696e 616c 2874  imeAndTerminal(t
-000004a0: 6572 6d69 6e61 6c2c 2073 7464 4572 7229  erminal, stdErr)
-000004b0: 0a20 2020 207d 0a20 2020 2024 2e74 6572  .    }.    $.ter
-000004c0: 6d69 6e61 6c2e 6163 7469 7665 2829 2e66  minal.active().f
-000004d0: 6f63 7573 2829 0a0a 7d2c 2770 6c61 7927  ocus()..},'play'
-000004e0: 290a 0a0a 0a0a 0a2f 2a2a 5472 6967 6765  )....../**Trigge
-000004f0: 7220 7468 6520 7661 6c69 6461 7469 6f6e  r the validation
-00000500: 2074 6573 7473 0a20 2a20 4065 6469 746f   tests. * @edito
-00000510: 724e 616d 6520 2873 7472 696e 6720 293a  rName (string ):
-00000520: 2022 6564 6974 6f72 5f7b 6861 7368 7d22   "editor_{hash}"
-00000530: 0a20 2a20 2a2f 0a63 6f6e 7374 2076 616c  . * */.const val
-00000540: 6964 6174 6520 3d20 2865 6469 746f 724e  idate = (editorN
-00000550: 616d 6529 203d 3e20 7769 7468 5079 6f64  ame) => withPyod
-00000560: 6964 6541 7379 6e63 4c6f 636b 2820 6173  ideAsyncLock( as
-00000570: 796e 6320 6675 6e63 7469 6f6e 2865 297b  ync function(e){
-00000580: 0a20 2020 2069 6628 6520 2626 2065 2e70  .    if(e && e.p
-00000590: 7265 7665 6e74 4465 6661 756c 7429 2065  reventDefault) e
-000005a0: 2e70 7265 7665 6e74 4465 6661 756c 7428  .preventDefault(
-000005b0: 290a 0a20 2020 2061 7761 6974 2077 6169  )..    await wai
-000005c0: 7446 6f72 5079 6f64 6964 6552 6561 6479  tForPyodideReady
-000005d0: 2829 3b0a 2020 2020 6a73 4c6f 6767 6572  ();.    jsLogger
-000005e0: 2822 5b56 616c 6964 6174 655d 2229 0a0a  ("[Validate]")..
-000005f0: 2020 2020 6c65 7420 5b63 6f64 652c 2074      let [code, t
-00000600: 6572 6d69 6e61 6c2c 206f 7074 696f 6e73  erminal, options
-00000610: 5d20 3d20 6177 6169 7420 7365 7475 7052  ] = await setupR
-00000620: 756e 7469 6d65 416e 6454 6572 6d69 6e61  untimeAndTermina
-00000630: 6c28 6564 6974 6f72 4e61 6d65 293b 0a20  l(editorName);. 
-00000640: 2020 206c 6574 2066 696e 616c 4d73 673d     let finalMsg=
-00000650: 2222 2c20 7374 6445 7272 3d22 220a 2020  "", stdErr="".  
-00000660: 2020 6c65 7420 6465 6372 6561 7365 5f63    let decrease_c
-00000670: 6f75 6e74 203d 2066 616c 7365 0a0a 2020  ount = false..  
-00000680: 2020 7472 797b 0a20 2020 2020 2020 202f    try{.        /
-00000690: 2f20 4465 6669 6e65 2074 6865 2075 7365  / Define the use
-000006a0: 7227 7320 636f 6465 2069 6e20 7468 6520  r's code in the 
-000006b0: 656e 7669 726f 6e6d 656e 7420 616e 6420  environment and 
-000006c0: 7275 6e20 7468 6520 7075 626c 6963 2074  run the public t
-000006d0: 6573 7473 2028 6966 2061 6e79 290a 2020  ests (if any).  
-000006e0: 2020 2020 2020 7374 6445 7272 203d 2061        stdErr = a
-000006f0: 7761 6974 2072 756e 5079 7468 6f6e 436f  wait runPythonCo
-00000700: 6465 5769 7468 4f70 7469 6f6e 7328 636f  deWithOptions(co
-00000710: 6465 2c20 7465 726d 696e 616c 2c20 6f70  de, terminal, op
-00000720: 7469 6f6e 732c 2074 7275 6529 0a0a 2020  tions, true)..  
-00000730: 2020 2020 2020 6465 6372 6561 7365 5f63        decrease_c
-00000740: 6f75 6e74 203d 2043 4f4e 4649 472e 6465  ount = CONFIG.de
-00000750: 6372 6561 7365 4174 7465 6d70 7473 4f6e  creaseAttemptsOn
-00000760: 5573 6572 436f 6465 4661 696c 7572 6520  UserCodeFailure 
-00000770: 2626 2073 7464 4572 720a 0a20 2020 2020  && stdErr..     
-00000780: 2020 202f 2f20 5275 6e20 7468 6520 7661     // Run the va
-00000790: 6c69 6461 7469 6f6e 2074 6573 7473 206f  lidation tests o
-000007a0: 6e6c 7920 6966 2074 6865 2075 7365 7227  nly if the user'
-000007b0: 7320 636f 6465 2073 7563 6365 6564 6564  s code succeeded
-000007c0: 2061 7420 7468 6520 7072 6576 696f 7573   at the previous
-000007d0: 2073 7465 700a 2020 2020 2020 2020 6966   step.        if
-000007e0: 2821 7374 6445 7272 297b 0a0a 2020 2020  (!stdErr){..    
-000007f0: 2020 2020 2020 2020 2f2f 2049 6620 7374          // If st
-00000800: 696c 6c20 7275 6e6e 696e 672c 2072 756e  ill running, run
-00000810: 2074 6865 206f 7269 6769 6e61 6c20 7075   the original pu
-00000820: 626c 6963 2074 6573 7473 2061 6e64 2074  blic tests and t
-00000830: 6865 2073 6563 7265 7420 6f6e 6573 2e2e  he secret ones..
-00000840: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00000850: 6e73 7420 7075 626c 6963 5465 7374 7320  nst publicTests 
-00000860: 3d20 7365 6375 7265 6445 7874 7261 6374  = securedExtract
-00000870: 696f 6e28 6564 6974 6f72 4e61 6d65 2c20  ion(editorName, 
-00000880: 434f 4e46 4947 2e69 6465 5072 6f70 2e70  CONFIG.ideProp.p
-00000890: 7562 6c69 6354 6573 7473 290a 2020 2020  ublicTests).    
-000008a0: 2020 2020 2020 2020 636f 6e73 7420 7365          const se
-000008b0: 6372 6574 5465 7374 7320 3d20 7365 6375  cretTests = secu
-000008c0: 7265 6445 7874 7261 6374 696f 6e28 6564  redExtraction(ed
-000008d0: 6974 6f72 4e61 6d65 2c20 434f 4e46 4947  itorName, CONFIG
-000008e0: 2e69 6465 5072 6f70 2e73 6563 7265 7454  .ideProp.secretT
-000008f0: 6573 7473 290a 0a20 2020 2020 2020 2020  ests)..         
-00000900: 2020 202f 2f20 2e2e 2e75 6e6c 6573 7320     // ...unless 
-00000910: 7468 6572 6520 6172 6520 6e6f 2073 6563  there are no sec
-00000920: 7265 7420 7465 7374 7320 2874 6869 7320  ret tests (this 
-00000930: 6d61 7920 6861 7070 656e 2077 6865 6e20  may happen when 
-00000940: 7573 696e 6720 4b42 2073 686f 7274 6375  using KB shortcu
-00000950: 7473 2c20 7768 696c 650a 2020 2020 2020  ts, while.      
-00000960: 2020 2020 2020 2f2f 2074 6865 7265 2069        // there i
-00000970: 7320 6e6f 2076 616c 6964 6174 696f 6e20  s no validation 
-00000980: 746f 2064 6f20 3d3e 206a 7573 7420 7175  to do => just qu
-00000990: 6974 2074 6865 2074 6573 7469 6e67 2070  it the testing p
-000009a0: 726f 6365 7373 2072 6967 6874 2061 7761  rocess right awa
-000009b0: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
-000009c0: 6628 2173 6563 7265 7454 6573 7473 2920  f(!secretTests) 
-000009d0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-000009e0: 2020 2020 636f 6e73 7420 6175 746f 4c6f      const autoLo
-000009f0: 6741 7373 6572 7420 2020 3d20 7365 6375  gAssert   = secu
-00000a00: 7265 6445 7874 7261 6374 696f 6e28 6564  redExtraction(ed
-00000a10: 6974 6f72 4e61 6d65 2c20 434f 4e46 4947  itorName, CONFIG
-00000a20: 2e69 6465 5072 6f70 2e61 7574 6f4c 6f67  .ideProp.autoLog
-00000a30: 4173 7365 7274 290a 2020 2020 2020 2020  Assert).        
-00000a40: 2020 2020 6f70 7469 6f6e 732e 6175 746f      options.auto
-00000a50: 4c6f 6741 7373 6572 7420 3d20 6175 746f  LogAssert = auto
-00000a60: 4c6f 6741 7373 6572 7421 3d3d 6e75 6c6c  LogAssert!==null
-00000a70: 203f 2061 7574 6f4c 6f67 4173 7365 7274   ? autoLogAssert
-00000a80: 203a 2043 4f4e 4649 472e 7368 6f77 4173   : CONFIG.showAs
-00000a90: 7365 7274 696f 6e43 6f64 654f 6e46 6169  sertionCodeOnFai
-00000aa0: 6c65 6454 6573 740a 2020 2020 2020 2020  ledTest.        
-00000ab0: 2020 2020 6f70 7469 6f6e 732e 7769 7468      options.with
-00000ac0: 5374 644f 7574 2020 2020 3d20 2143 4f4e  StdOut    = !CON
-00000ad0: 4649 472e 6465 6163 7469 7661 7465 5374  FIG.deactivateSt
-00000ae0: 646f 7574 466f 7253 6563 7265 7473 0a0a  doutForSecrets..
-00000af0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00000b00: 7420 6675 6c6c 5465 7374 7320 3d20 6024  t fullTests = `$
-00000b10: 7b20 7075 626c 6963 5465 7374 7320 7d5c  { publicTests }\
-00000b20: 6e5c 6e24 7b20 7365 6372 6574 5465 7374  n\n${ secretTest
-00000b30: 7320 7d60 0a20 2020 2020 2020 2020 2020  s }`.           
-00000b40: 2064 6563 7265 6173 655f 636f 756e 7420   decrease_count 
-00000b50: 203d 2073 7464 4572 7220 3d20 6177 6169   = stdErr = awai
-00000b60: 7420 7275 6e50 7974 686f 6e43 6f64 6557  t runPythonCodeW
-00000b70: 6974 684f 7074 696f 6e73 2866 756c 6c54  ithOptions(fullT
-00000b80: 6573 7473 2c20 7465 726d 696e 616c 2c20  ests, terminal, 
-00000b90: 6f70 7469 6f6e 732c 2066 616c 7365 290a  options, false).
-00000ba0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00000bb0: 2020 202f 2f20 4f6e 2065 7272 6f72 2c20     // On error, 
-00000bc0: 6d61 6e61 6765 2074 6865 2063 6f75 6e74  manage the count
-00000bd0: 6572 206f 6620 7472 6965 7320 616e 6420  er of tries and 
-00000be0: 7468 6520 7265 7665 6c61 7469 6f6e 206f  the revelation o
-00000bf0: 6620 7468 6520 736f 6c75 7469 6f6e 2c20  f the solution, 
-00000c00: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
-00000c10: 2020 2f2f 2072 6576 6561 6c20 7468 6520    // reveal the 
-00000c20: 736f 6c75 7469 6f6e 7320 2b20 7365 7475  solutions + setu
-00000c30: 7020 7375 6363 6573 7320 6d65 7373 6167  p success messag
-00000c40: 6520 2864 6973 706c 6179 6564 2069 6e20  e (displayed in 
-00000c50: 7465 6172 646f 776e 2073 7465 7029 3a0a  teardown step):.
-00000c60: 2020 2020 2020 2020 6966 2821 7374 6445          if(!stdE
-00000c70: 7272 297b 0a20 2020 2020 2020 2020 2020  rr){.           
-00000c80: 2075 6e68 6964 6553 6f6c 7574 696f 6e41   unhideSolutionA
-00000c90: 6e64 5265 6d28 6564 6974 6f72 4e61 6d65  ndRem(editorName
-00000ca0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00000cb0: 2867 6574 4174 7465 6d70 7473 4c65 6674  (getAttemptsLeft
-00000cc0: 2865 6469 746f 724e 616d 6529 203e 2030  (editorName) > 0
-00000cd0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
-00000ce0: 2020 2066 696e 616c 4d73 6720 3d20 6275     finalMsg = bu
-00000cf0: 696c 6453 7563 6365 7373 4d65 7373 6167  ildSuccessMessag
-00000d00: 6528 6564 6974 6f72 4e61 6d65 290a 2020  e(editorName).  
-00000d10: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
-00000d20: 2020 2020 207d 656c 7365 2069 6628 6465       }else if(de
-00000d30: 6372 6561 7365 5f63 6f75 6e74 297b 0a20  crease_count){. 
-00000d40: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00000d50: 206e 4174 7465 6d70 7473 4c65 6674 203d   nAttemptsLeft =
-00000d60: 2075 7064 6174 6549 6465 436f 756e 7465   updateIdeCounte
-00000d70: 7228 6564 6974 6f72 4e61 6d65 290a 2020  r(editorName).  
-00000d80: 2020 2020 2020 2020 2020 6966 2875 6e68            if(unh
-00000d90: 6964 6553 6f6c 7574 696f 6e41 6e64 5265  ideSolutionAndRe
-00000da0: 6d28 6564 6974 6f72 4e61 6d65 2c20 6e41  m(editorName, nA
-00000db0: 7474 656d 7074 734c 6566 742c 2066 616c  ttemptsLeft, fal
-00000dc0: 7365 2929 7b0a 2020 2020 2020 2020 2020  se)){.          
-00000dd0: 2020 2020 2020 6669 6e61 6c4d 7367 203d        finalMsg =
-00000de0: 2065 6e68 616e 6365 4661 696c 7572 654d   enhanceFailureM
-00000df0: 7367 2865 6469 746f 724e 616d 652c 2073  sg(editorName, s
-00000e00: 7464 4572 7229 0a20 2020 2020 2020 2020  tdErr).         
-00000e10: 2020 207d 0a20 2020 2020 2020 207d 0a0a     }.        }..
-00000e20: 2020 2020 7d66 696e 616c 6c79 7b0a 2020      }finally{.  
-00000e30: 2020 2020 2020 7465 6172 446f 776e 5275        tearDownRu
-00000e40: 6e74 696d 6541 6e64 5465 726d 696e 616c  ntimeAndTerminal
-00000e50: 2874 6572 6d69 6e61 6c2c 2073 7464 4572  (terminal, stdEr
-00000e60: 722c 2066 696e 616c 4d73 6729 0a20 2020  r, finalMsg).   
-00000e70: 207d 0a20 2020 2024 2e74 6572 6d69 6e61   }.    $.termina
-00000e80: 6c2e 6163 7469 7665 2829 2e66 6f63 7573  l.active().focus
-00000e90: 2829 0a0a 7d2c 2776 616c 6964 6174 6527  ()..},'validate'
-00000ea0: 290a 0a0a 0a2f 2f2d 2d2d 2d2d 2d2d 2d2d  )....//---------
+000003c0: 6465 2c20 7465 726d 696e 616c 2c20 6f70  de, terminal, op
+000003d0: 7469 6f6e 735d 203d 2061 7761 6974 2073  tions] = await s
+000003e0: 6574 7570 5275 6e74 696d 6541 6e64 5465  etupRuntimeAndTe
+000003f0: 726d 696e 616c 2865 6469 746f 724e 616d  rminal(editorNam
+00000400: 6529 3b0a 2020 2020 6c65 7420 7374 6445  e);.    let stdE
+00000410: 7272 3d22 220a 0a20 2020 2074 7279 7b0a  rr=""..    try{.
+00000420: 2020 2020 2020 2020 7374 6445 7272 203d          stdErr =
+00000430: 2061 7761 6974 2072 756e 5079 7468 6f6e   await runPython
+00000440: 436f 6465 5769 7468 4f70 7469 6f6e 7328  CodeWithOptions(
+00000450: 636f 6465 2c20 7465 726d 696e 616c 2c20  code, terminal, 
+00000460: 6f70 7469 6f6e 732c 2074 7275 6529 0a20  options, true). 
+00000470: 2020 207d 6669 6e61 6c6c 797b 0a20 2020     }finally{.   
+00000480: 2020 2020 2074 6561 7244 6f77 6e52 756e       tearDownRun
+00000490: 7469 6d65 416e 6454 6572 6d69 6e61 6c28  timeAndTerminal(
+000004a0: 7465 726d 696e 616c 2c20 7374 6445 7272  terminal, stdErr
+000004b0: 290a 2020 2020 7d0a 2020 2020 242e 7465  ).    }.    $.te
+000004c0: 726d 696e 616c 2e61 6374 6976 6528 292e  rminal.active().
+000004d0: 666f 6375 7328 290a 0a7d 2c27 706c 6179  focus()..},'play
+000004e0: 2729 0a0a 0a0a 0a0a 2f2a 2a54 7269 6767  ')....../**Trigg
+000004f0: 6572 2074 6865 2076 616c 6964 6174 696f  er the validatio
+00000500: 6e20 7465 7374 730a 202a 2040 6564 6974  n tests. * @edit
+00000510: 6f72 4e61 6d65 2028 7374 7269 6e67 2029  orName (string )
+00000520: 3a20 2265 6469 746f 725f 7b68 6173 687d  : "editor_{hash}
+00000530: 220a 202a 202a 2f0a 636f 6e73 7420 7661  ". * */.const va
+00000540: 6c69 6461 7465 203d 2028 6564 6974 6f72  lidate = (editor
+00000550: 4e61 6d65 2920 3d3e 2077 6974 6850 796f  Name) => withPyo
+00000560: 6469 6465 4173 796e 634c 6f63 6b28 2061  dideAsyncLock( a
+00000570: 7379 6e63 2066 756e 6374 696f 6e28 6529  sync function(e)
+00000580: 7b0a 2020 2020 6966 2865 2026 2620 652e  {.    if(e && e.
+00000590: 7072 6576 656e 7444 6566 6175 6c74 2920  preventDefault) 
+000005a0: 652e 7072 6576 656e 7444 6566 6175 6c74  e.preventDefault
+000005b0: 2829 0a0a 2020 2020 6177 6169 7420 7761  ()..    await wa
+000005c0: 6974 466f 7250 796f 6469 6465 5265 6164  itForPyodideRead
+000005d0: 7928 293b 0a20 2020 206a 734c 6f67 6765  y();.    jsLogge
+000005e0: 7228 225b 5661 6c69 6461 7465 5d22 290a  r("[Validate]").
+000005f0: 0a20 2020 206c 6574 205b 636f 6465 2c20  .    let [code, 
+00000600: 7465 726d 696e 616c 2c20 6f70 7469 6f6e  terminal, option
+00000610: 735d 203d 2061 7761 6974 2073 6574 7570  s] = await setup
+00000620: 5275 6e74 696d 6541 6e64 5465 726d 696e  RuntimeAndTermin
+00000630: 616c 2865 6469 746f 724e 616d 6529 3b0a  al(editorName);.
+00000640: 2020 2020 6c65 7420 6669 6e61 6c4d 7367      let finalMsg
+00000650: 3d22 222c 2073 7464 4572 723d 2222 0a20  ="", stdErr="". 
+00000660: 2020 206c 6574 2064 6563 7265 6173 655f     let decrease_
+00000670: 636f 756e 7420 3d20 6661 6c73 650a 0a20  count = false.. 
+00000680: 2020 2074 7279 7b0a 2020 2020 2020 2020     try{.        
+00000690: 2f2f 2044 6566 696e 6520 7468 6520 7573  // Define the us
+000006a0: 6572 2773 2063 6f64 6520 696e 2074 6865  er's code in the
+000006b0: 2065 6e76 6972 6f6e 6d65 6e74 2061 6e64   environment and
+000006c0: 2072 756e 2074 6865 2070 7562 6c69 6320   run the public 
+000006d0: 7465 7374 7320 2869 6620 616e 7929 0a20  tests (if any). 
+000006e0: 2020 2020 2020 2073 7464 4572 7220 3d20         stdErr = 
+000006f0: 6177 6169 7420 7275 6e50 7974 686f 6e43  await runPythonC
+00000700: 6f64 6557 6974 684f 7074 696f 6e73 2863  odeWithOptions(c
+00000710: 6f64 652c 2074 6572 6d69 6e61 6c2c 206f  ode, terminal, o
+00000720: 7074 696f 6e73 2c20 7472 7565 290a 0a20  ptions, true).. 
+00000730: 2020 2020 2020 2064 6563 7265 6173 655f         decrease_
+00000740: 636f 756e 7420 3d20 434f 4e46 4947 2e64  count = CONFIG.d
+00000750: 6563 7265 6173 6541 7474 656d 7074 734f  ecreaseAttemptsO
+00000760: 6e55 7365 7243 6f64 6546 6169 6c75 7265  nUserCodeFailure
+00000770: 2026 2620 7374 6445 7272 0a0a 2020 2020   && stdErr..    
+00000780: 2020 2020 2f2f 2052 756e 2074 6865 2076      // Run the v
+00000790: 616c 6964 6174 696f 6e20 7465 7374 7320  alidation tests 
+000007a0: 6f6e 6c79 2069 6620 7468 6520 7573 6572  only if the user
+000007b0: 2773 2063 6f64 6520 7375 6363 6565 6465  's code succeede
+000007c0: 6420 6174 2074 6865 2070 7265 7669 6f75  d at the previou
+000007d0: 7320 7374 6570 0a20 2020 2020 2020 2069  s step.        i
+000007e0: 6628 2173 7464 4572 7229 7b0a 0a20 2020  f(!stdErr){..   
+000007f0: 2020 2020 2020 2020 202f 2f20 4966 2073           // If s
+00000800: 7469 6c6c 2072 756e 6e69 6e67 2c20 7275  till running, ru
+00000810: 6e20 7468 6520 6f72 6967 696e 616c 2070  n the original p
+00000820: 7562 6c69 6320 7465 7374 7320 616e 6420  ublic tests and 
+00000830: 7468 6520 7365 6372 6574 206f 6e65 732e  the secret ones.
+00000840: 2e2e 0a20 2020 2020 2020 2020 2020 2063  ...            c
+00000850: 6f6e 7374 2070 7562 6c69 6354 6573 7473  onst publicTests
+00000860: 203d 2073 6563 7572 6564 4578 7472 6163   = securedExtrac
+00000870: 7469 6f6e 2865 6469 746f 724e 616d 652c  tion(editorName,
+00000880: 2043 4f4e 4649 472e 6964 6550 726f 702e   CONFIG.ideProp.
+00000890: 7075 626c 6963 5465 7374 7329 0a20 2020  publicTests).   
+000008a0: 2020 2020 2020 2020 2063 6f6e 7374 2073           const s
+000008b0: 6563 7265 7454 6573 7473 203d 2073 6563  ecretTests = sec
+000008c0: 7572 6564 4578 7472 6163 7469 6f6e 2865  uredExtraction(e
+000008d0: 6469 746f 724e 616d 652c 2043 4f4e 4649  ditorName, CONFI
+000008e0: 472e 6964 6550 726f 702e 7365 6372 6574  G.ideProp.secret
+000008f0: 5465 7374 7329 0a0a 2020 2020 2020 2020  Tests)..        
+00000900: 2020 2020 2f2f 202e 2e2e 756e 6c65 7373      // ...unless
+00000910: 2074 6865 7265 2061 7265 206e 6f20 7365   there are no se
+00000920: 6372 6574 2074 6573 7473 2028 7468 6973  cret tests (this
+00000930: 206d 6179 2068 6170 7065 6e20 7768 656e   may happen when
+00000940: 2075 7369 6e67 204b 4220 7368 6f72 7463   using KB shortc
+00000950: 7574 732c 2077 6869 6c65 0a20 2020 2020  uts, while.     
+00000960: 2020 2020 2020 202f 2f20 7468 6572 6520         // there 
+00000970: 6973 206e 6f20 7661 6c69 6461 7469 6f6e  is no validation
+00000980: 2074 6f20 646f 203d 3e20 6a75 7374 2071   to do => just q
+00000990: 7569 7420 7468 6520 7465 7374 696e 6720  uit the testing 
+000009a0: 7072 6f63 6573 7320 7269 6768 7420 6177  process right aw
+000009b0: 6179 290a 2020 2020 2020 2020 2020 2020  ay).            
+000009c0: 6966 2821 7365 6372 6574 5465 7374 7329  if(!secretTests)
+000009d0: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
+000009e0: 2020 2020 2063 6f6e 7374 2061 7574 6f4c       const autoL
+000009f0: 6f67 4173 7365 7274 2020 203d 2073 6563  ogAssert   = sec
+00000a00: 7572 6564 4578 7472 6163 7469 6f6e 2865  uredExtraction(e
+00000a10: 6469 746f 724e 616d 652c 2043 4f4e 4649  ditorName, CONFI
+00000a20: 472e 6964 6550 726f 702e 6175 746f 4c6f  G.ideProp.autoLo
+00000a30: 6741 7373 6572 7429 0a20 2020 2020 2020  gAssert).       
+00000a40: 2020 2020 206f 7074 696f 6e73 2e61 7574       options.aut
+00000a50: 6f4c 6f67 4173 7365 7274 203d 2061 7574  oLogAssert = aut
+00000a60: 6f4c 6f67 4173 7365 7274 213d 3d6e 756c  oLogAssert!==nul
+00000a70: 6c20 3f20 6175 746f 4c6f 6741 7373 6572  l ? autoLogAsser
+00000a80: 7420 3a20 434f 4e46 4947 2e73 686f 7741  t : CONFIG.showA
+00000a90: 7373 6572 7469 6f6e 436f 6465 4f6e 4661  ssertionCodeOnFa
+00000aa0: 696c 6564 5465 7374 0a20 2020 2020 2020  iledTest.       
+00000ab0: 2020 2020 206f 7074 696f 6e73 2e77 6974       options.wit
+00000ac0: 6853 7464 4f75 7420 2020 203d 2021 434f  hStdOut    = !CO
+00000ad0: 4e46 4947 2e64 6561 6374 6976 6174 6553  NFIG.deactivateS
+00000ae0: 7464 6f75 7446 6f72 5365 6372 6574 730a  tdoutForSecrets.
+00000af0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00000b00: 7374 2066 756c 6c54 6573 7473 203d 2060  st fullTests = `
+00000b10: 247b 2070 7562 6c69 6354 6573 7473 207d  ${ publicTests }
+00000b20: 5c6e 5c6e 247b 2073 6563 7265 7454 6573  \n\n${ secretTes
+00000b30: 7473 207d 600a 2020 2020 2020 2020 2020  ts }`.          
+00000b40: 2020 6465 6372 6561 7365 5f63 6f75 6e74    decrease_count
+00000b50: 2020 3d20 7374 6445 7272 203d 2061 7761    = stdErr = awa
+00000b60: 6974 2072 756e 5079 7468 6f6e 436f 6465  it runPythonCode
+00000b70: 5769 7468 4f70 7469 6f6e 7328 6675 6c6c  WithOptions(full
+00000b80: 5465 7374 732c 2074 6572 6d69 6e61 6c2c  Tests, terminal,
+00000b90: 206f 7074 696f 6e73 2c20 6661 6c73 6529   options, false)
+00000ba0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00000bb0: 2020 2020 2f2f 204f 6e20 6572 726f 722c      // On error,
+00000bc0: 206d 616e 6167 6520 7468 6520 636f 756e   manage the coun
+00000bd0: 7465 7220 6f66 2074 7269 6573 2061 6e64  ter of tries and
+00000be0: 2074 6865 2072 6576 656c 6174 696f 6e20   the revelation 
+00000bf0: 6f66 2074 6865 2073 6f6c 7574 696f 6e2c  of the solution,
+00000c00: 206f 7468 6572 7769 7365 0a20 2020 2020   otherwise.     
+00000c10: 2020 202f 2f20 7265 7665 616c 2074 6865     // reveal the
+00000c20: 2073 6f6c 7574 696f 6e73 202b 2073 6574   solutions + set
+00000c30: 7570 2073 7563 6365 7373 206d 6573 7361  up success messa
+00000c40: 6765 2028 6469 7370 6c61 7965 6420 696e  ge (displayed in
+00000c50: 2074 6561 7264 6f77 6e20 7374 6570 293a   teardown step):
+00000c60: 0a20 2020 2020 2020 2069 6628 2173 7464  .        if(!std
+00000c70: 4572 7229 7b0a 2020 2020 2020 2020 2020  Err){.          
+00000c80: 2020 756e 6869 6465 536f 6c75 7469 6f6e    unhideSolution
+00000c90: 416e 6452 656d 2865 6469 746f 724e 616d  AndRem(editorNam
+00000ca0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00000cb0: 6628 6765 7441 7474 656d 7074 734c 6566  f(getAttemptsLef
+00000cc0: 7428 6564 6974 6f72 4e61 6d65 2920 3e20  t(editorName) > 
+00000cd0: 3029 7b0a 2020 2020 2020 2020 2020 2020  0){.            
+00000ce0: 2020 2020 6669 6e61 6c4d 7367 203d 2062      finalMsg = b
+00000cf0: 7569 6c64 5375 6363 6573 734d 6573 7361  uildSuccessMessa
+00000d00: 6765 2865 6469 746f 724e 616d 6529 0a20  ge(editorName). 
+00000d10: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
+00000d20: 2020 2020 2020 7d65 6c73 6520 6966 2864        }else if(d
+00000d30: 6563 7265 6173 655f 636f 756e 7429 7b0a  ecrease_count){.
+00000d40: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000d50: 7420 6e41 7474 656d 7074 734c 6566 7420  t nAttemptsLeft 
+00000d60: 3d20 7570 6461 7465 4964 6543 6f75 6e74  = updateIdeCount
+00000d70: 6572 2865 6469 746f 724e 616d 6529 0a20  er(editorName). 
+00000d80: 2020 2020 2020 2020 2020 2069 6628 756e             if(un
+00000d90: 6869 6465 536f 6c75 7469 6f6e 416e 6452  hideSolutionAndR
+00000da0: 656d 2865 6469 746f 724e 616d 652c 206e  em(editorName, n
+00000db0: 4174 7465 6d70 7473 4c65 6674 2c20 6661  AttemptsLeft, fa
+00000dc0: 6c73 6529 297b 0a20 2020 2020 2020 2020  lse)){.         
+00000dd0: 2020 2020 2020 2066 696e 616c 4d73 6720         finalMsg 
+00000de0: 3d20 656e 6861 6e63 6546 6169 6c75 7265  = enhanceFailure
+00000df0: 4d73 6728 6564 6974 6f72 4e61 6d65 2c20  Msg(editorName, 
+00000e00: 7374 6445 7272 290a 2020 2020 2020 2020  stdErr).        
+00000e10: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00000e20: 0a20 2020 207d 6669 6e61 6c6c 797b 0a20  .    }finally{. 
+00000e30: 2020 2020 2020 2074 6561 7244 6f77 6e52         tearDownR
+00000e40: 756e 7469 6d65 416e 6454 6572 6d69 6e61  untimeAndTermina
+00000e50: 6c28 7465 726d 696e 616c 2c20 7374 6445  l(terminal, stdE
+00000e60: 7272 2c20 6669 6e61 6c4d 7367 290a 2020  rr, finalMsg).  
+00000e70: 2020 7d0a 2020 2020 242e 7465 726d 696e    }.    $.termin
+00000e80: 616c 2e61 6374 6976 6528 292e 666f 6375  al.active().focu
+00000e90: 7328 290a 0a7d 2c27 7661 6c69 6461 7465  s()..},'validate
+00000ea0: 2729 0a0a 0a0a 2f2f 2d2d 2d2d 2d2d 2d2d  ')....//--------
 00000eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000ef0: 0a63 6f6e 7374 205f 6765 6e65 7261 7465  .const _generate
-00000f00: 446f 776e 6c6f 6164 4e61 6d65 203d 2028  DownloadName = (
-00000f10: 7363 7269 7074 4e61 6d65 2920 3d3e 207b  scriptName) => {
-00000f20: 0a20 2020 2069 6620 2873 6372 6970 744e  .    if (scriptN
-00000f30: 616d 6521 3d22 2229 7b0a 2020 2020 2020  ame!=""){.      
-00000f40: 2020 7265 7475 726e 2060 247b 7363 7269    return `${scri
-00000f50: 7074 4e61 6d65 7d2e 7079 600a 2020 2020  ptName}.py`.    
-00000f60: 7d0a 2020 2020 2f2f 2048 616e 646c 6520  }.    // Handle 
-00000f70: 6564 6974 6f72 7320 7769 7468 6f75 7420  editors without 
-00000f80: 7265 6c61 7465 6420 7079 7468 6f6e 2066  related python f
-00000f90: 696c 653a 0a20 2020 206c 6574 205b 6461  ile:.    let [da
-00000fa0: 792c 2074 696d 655d 203d 206e 6577 2044  y, time] = new D
-00000fb0: 6174 6528 292e 746f 4953 4f53 7472 696e  ate().toISOStrin
-00000fc0: 6728 292e 7370 6c69 7428 2254 2229 3b0a  g().split("T");.
-00000fd0: 2020 2020 6c65 7420 6868 6d6d 7373 203d      let hhmmss =
-00000fe0: 2074 696d 652e 7370 6c69 7428 222e 2229   time.split(".")
-00000ff0: 5b30 5d2e 7265 706c 6163 6528 2f3a 2f67  [0].replace(/:/g
-00001000: 2c20 222d 2229 3b0a 2020 2020 7265 7475  , "-");.    retu
-00001010: 726e 2060 7363 7269 7074 5f24 7b64 6179  rn `script_${day
-00001020: 7d2d 247b 6868 6d6d 7373 7d2e 7079 603b  }-${hhmmss}.py`;
-00001030: 0a7d 3b0a 0a0a 2f2a 2a44 6f77 6e6c 6f61  .};.../**Downloa
-00001040: 6420 7468 6520 6375 7272 656e 7420 636f  d the current co
-00001050: 6e74 656e 7420 6f66 2074 6865 2065 6469  ntent of the edi
-00001060: 746f 7220 746f 2074 6865 2064 6f77 6e6c  tor to the downl
-00001070: 6f61 6420 666f 6c64 6572 206f 6620 7468  oad folder of th
-00001080: 6520 7573 6572 2e0a 202a 202a 2f0a 636f  e user.. * */.co
-00001090: 6e73 7420 646f 776e 6c6f 6164 203d 2028  nst download = (
-000010a0: 6564 6974 6f72 4e61 6d65 2920 3d3e 2077  editorName) => w
-000010b0: 6974 6850 796f 6469 6465 4173 796e 634c  ithPyodideAsyncL
-000010c0: 6f63 6b28 6173 796e 6320 6675 6e63 7469  ock(async functi
-000010d0: 6f6e 2829 7b0a 2020 2020 6177 6169 7420  on(){.    await 
-000010e0: 7761 6974 466f 7250 796f 6469 6465 5265  waitForPyodideRe
-000010f0: 6164 7928 293b 0a20 2020 206a 734c 6f67  ady();.    jsLog
-00001100: 6765 7228 225b 446f 776e 6c6f 6164 5d22  ger("[Download]"
-00001110: 290a 0a20 2020 2063 6f6e 7374 2065 6469  )..    const edi
-00001120: 746f 7220 3d20 6163 652e 6564 6974 2865  tor = ace.edit(e
-00001130: 6469 746f 724e 616d 6529 0a20 2020 2063  ditorName).    c
-00001140: 6f6e 7374 2073 6372 6970 744e 616d 6520  onst scriptName 
-00001150: 3d20 6564 6974 6f72 2e63 6f6e 7461 696e  = editor.contain
-00001160: 6572 2e67 6574 4174 7472 6962 7574 6528  er.getAttribute(
-00001170: 2770 795f 6e61 6d65 2729 0a20 2020 2063  'py_name').    c
-00001180: 6f6e 7374 2066 696c 654e 616d 6520 3d20  onst fileName = 
-00001190: 5f67 656e 6572 6174 6544 6f77 6e6c 6f61  _generateDownloa
-000011a0: 644e 616d 6528 7363 7269 7074 4e61 6d65  dName(scriptName
-000011b0: 290a 2020 2020 6c65 7420 6964 6543 6f6e  ).    let ideCon
-000011c0: 7465 6e74 203d 2065 6469 746f 722e 6765  tent = editor.ge
-000011d0: 7456 616c 7565 2829 202b 2022 2220 2020  tValue() + ""   
-000011e0: 2020 2f2f 2065 6e66 6f72 6365 2073 7472    // enforce str
-000011f0: 696e 6769 6669 6361 7469 6f6e 2069 6e20  ingification in 
-00001200: 616e 7920 6361 7365 0a0a 2020 2020 6c65  any case..    le
-00001210: 7420 6c69 6e6b 203d 2064 6f63 756d 656e  t link = documen
-00001220: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
-00001230: 2261 2229 3b0a 2020 2020 6c65 7420 626c  "a");.    let bl
-00001240: 6f62 203d 206e 6577 2042 6c6f 6228 5b69  ob = new Blob([i
-00001250: 6465 436f 6e74 656e 745d 2c20 7b20 7479  deContent], { ty
-00001260: 7065 3a20 2274 6578 742f 706c 6169 6e22  pe: "text/plain"
-00001270: 207d 293b 0a20 2020 206c 696e 6b2e 6872   });.    link.hr
-00001280: 6566 203d 2055 524c 2e63 7265 6174 654f  ef = URL.createO
-00001290: 626a 6563 7455 524c 2862 6c6f 6229 3b0a  bjectURL(blob);.
-000012a0: 2020 2020 6c69 6e6b 2e64 6f77 6e6c 6f61      link.downloa
-000012b0: 6420 3d20 6669 6c65 4e61 6d65 0a0a 2020  d = fileName..  
-000012c0: 2020 6c69 6e6b 2e63 6c69 636b 2829 3b0a    link.click();.
-000012d0: 2020 2020 5552 4c2e 7265 766f 6b65 4f62      URL.revokeOb
-000012e0: 6a65 6374 5552 4c28 6c69 6e6b 2e68 7265  jectURL(link.hre
-000012f0: 6629 3b0a 2020 2020 6c69 6e6b 2e72 656d  f);.    link.rem
-00001300: 6f76 6528 290a 2020 2020 666f 6375 7345  ove().    focusE
-00001310: 6469 746f 7228 6564 6974 6f72 4e61 6d65  ditor(editorName
-00001320: 290a 0a7d 2c27 646f 776e 6c6f 6164 2729  )..},'download')
-00001330: 0a0a 0a0a 2f2a 2a20 5570 6c6f 6164 2072  ..../** Upload r
-00001340: 6f75 7469 6e65 2028 666f 7220 7468 6520  outine (for the 
-00001350: 696e 7075 7420 7468 6174 2069 7320 7472  input that is tr
-00001360: 6967 6765 7265 6420 6279 2074 6865 2075  iggered by the u
-00001370: 706c 6f61 6420 6275 7474 6f6e 2e2e 2e29  pload button...)
-00001380: 202a 2f0a 636f 6e73 7420 7570 6c6f 6164   */.const upload
-00001390: 526f 7574 696e 6520 3d5f 3d3e 2077 6974  Routine =_=> wit
-000013a0: 6850 796f 6469 6465 4173 796e 634c 6f63  hPyodideAsyncLoc
-000013b0: 6b28 6173 796e 6320 6675 6e63 7469 6f6e  k(async function
-000013c0: 2829 207b 0a20 2020 2061 7761 6974 2077  () {.    await w
-000013d0: 6169 7446 6f72 5079 6f64 6964 6552 6561  aitForPyodideRea
-000013e0: 6479 2829 3b0a 2020 2020 6a73 4c6f 6767  dy();.    jsLogg
-000013f0: 6572 2822 5b55 706c 6f61 645d 2229 0a0a  er("[Upload]")..
-00001400: 2020 2020 6c65 7420 6e75 6d62 6572 203d      let number =
-00001410: 2074 6869 732e 6964 2e73 706c 6974 2822   this.id.split("
-00001420: 5f22 292e 706f 7028 293b 0a20 2020 206c  _").pop();.    l
-00001430: 6574 2069 6445 6469 746f 7220 3d20 2265  et idEditor = "e
-00001440: 6469 746f 725f 2220 2b20 6e75 6d62 6572  ditor_" + number
-00001450: 3b0a 2020 2020 636f 6e73 7420 7570 6c6f  ;.    const uplo
-00001460: 6164 496e 7075 7420 3d20 646f 6375 6d65  adInput = docume
-00001470: 6e74 2e67 6574 456c 656d 656e 7442 7949  nt.getElementByI
-00001480: 6428 2269 6e70 7574 5f22 202b 2069 6445  d("input_" + idE
-00001490: 6469 746f 7229 0a20 2020 2075 706c 6f61  ditor).    uploa
-000014a0: 6449 6e70 7574 2e61 6464 4576 656e 744c  dInput.addEventL
-000014b0: 6973 7465 6e65 7228 2022 6368 616e 6765  istener( "change
-000014c0: 222c 2066 756e 6374 696f 6e20 2865 7674  ", function (evt
-000014d0: 2920 7b0a 2020 2020 2020 2020 6c65 7420  ) {.        let 
-000014e0: 6669 6c65 203d 2065 7674 2e74 6172 6765  file = evt.targe
-000014f0: 742e 6669 6c65 735b 305d 3b0a 2020 2020  t.files[0];.    
-00001500: 2020 2020 6c65 7420 7265 6164 6572 203d      let reader =
-00001510: 206e 6577 2046 696c 6552 6561 6465 7228   new FileReader(
-00001520: 293b 0a20 2020 2020 2020 2076 6172 2065  );.        var e
-00001530: 6469 746f 7220 3d20 6163 652e 6564 6974  ditor = ace.edit
-00001540: 2869 6445 6469 746f 7229 3b0a 2020 2020  (idEditor);.    
-00001550: 2020 2020 7265 6164 6572 2e6f 6e6c 6f61      reader.onloa
-00001560: 6420 3d20 6675 6e63 7469 6f6e 2028 6576  d = function (ev
-00001570: 656e 7429 207b 0a20 2020 2020 2020 2020  ent) {.         
-00001580: 2065 6469 746f 722e 6765 7453 6573 7369   editor.getSessi
-00001590: 6f6e 2829 2e73 6574 5661 6c75 6528 6576  on().setValue(ev
-000015a0: 656e 742e 7461 7267 6574 2e72 6573 756c  ent.target.resul
-000015b0: 7429 3b0a 2020 2020 2020 2020 7d3b 0a20  t);.        };. 
-000015c0: 2020 2020 2020 2072 6561 6465 722e 7265         reader.re
-000015d0: 6164 4173 5465 7874 2866 696c 6529 3b0a  adAsText(file);.
-000015e0: 2020 2020 2020 7d2c 0a20 2020 2020 2066        },.      f
-000015f0: 616c 7365 0a20 2020 2029 0a20 2020 2066  alse.    ).    f
-00001600: 6f63 7573 4564 6974 6f72 2869 6445 6469  ocusEditor(idEdi
-00001610: 746f 7229 0a0a 7d2c 2775 706c 6f61 6427  tor)..},'upload'
-00001620: 290a 0a0a 0a0a 0a2f 2f2d 2d2d 2d2d 2d2d  )......//-------
+00000ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00000ef0: 0a0a 636f 6e73 7420 5f67 656e 6572 6174  ..const _generat
+00000f00: 6544 6f77 6e6c 6f61 644e 616d 6520 3d20  eDownloadName = 
+00000f10: 2873 6372 6970 744e 616d 6529 203d 3e20  (scriptName) => 
+00000f20: 7b0a 2020 2020 6966 2028 7363 7269 7074  {.    if (script
+00000f30: 4e61 6d65 213d 2222 297b 0a20 2020 2020  Name!=""){.     
+00000f40: 2020 2072 6574 7572 6e20 6024 7b73 6372     return `${scr
+00000f50: 6970 744e 616d 657d 2e70 7960 0a20 2020  iptName}.py`.   
+00000f60: 207d 0a20 2020 202f 2f20 4861 6e64 6c65   }.    // Handle
+00000f70: 2065 6469 746f 7273 2077 6974 686f 7574   editors without
+00000f80: 2072 656c 6174 6564 2070 7974 686f 6e20   related python 
+00000f90: 6669 6c65 3a0a 2020 2020 6c65 7420 5b64  file:.    let [d
+00000fa0: 6179 2c20 7469 6d65 5d20 3d20 6e65 7720  ay, time] = new 
+00000fb0: 4461 7465 2829 2e74 6f49 534f 5374 7269  Date().toISOStri
+00000fc0: 6e67 2829 2e73 706c 6974 2822 5422 293b  ng().split("T");
+00000fd0: 0a20 2020 206c 6574 2068 686d 6d73 7320  .    let hhmmss 
+00000fe0: 3d20 7469 6d65 2e73 706c 6974 2822 2e22  = time.split("."
+00000ff0: 295b 305d 2e72 6570 6c61 6365 282f 3a2f  )[0].replace(/:/
+00001000: 672c 2022 2d22 293b 0a20 2020 2072 6574  g, "-");.    ret
+00001010: 7572 6e20 6073 6372 6970 745f 247b 6461  urn `script_${da
+00001020: 797d 2d24 7b68 686d 6d73 737d 2e70 7960  y}-${hhmmss}.py`
+00001030: 3b0a 7d3b 0a0a 0a2f 2a2a 446f 776e 6c6f  ;.};.../**Downlo
+00001040: 6164 2074 6865 2063 7572 7265 6e74 2063  ad the current c
+00001050: 6f6e 7465 6e74 206f 6620 7468 6520 6564  ontent of the ed
+00001060: 6974 6f72 2074 6f20 7468 6520 646f 776e  itor to the down
+00001070: 6c6f 6164 2066 6f6c 6465 7220 6f66 2074  load folder of t
+00001080: 6865 2075 7365 722e 0a20 2a20 2a2f 0a63  he user.. * */.c
+00001090: 6f6e 7374 2064 6f77 6e6c 6f61 6420 3d20  onst download = 
+000010a0: 2865 6469 746f 724e 616d 6529 203d 3e20  (editorName) => 
+000010b0: 7769 7468 5079 6f64 6964 6541 7379 6e63  withPyodideAsync
+000010c0: 4c6f 636b 2861 7379 6e63 2066 756e 6374  Lock(async funct
+000010d0: 696f 6e28 297b 0a20 2020 2061 7761 6974  ion(){.    await
+000010e0: 2077 6169 7446 6f72 5079 6f64 6964 6552   waitForPyodideR
+000010f0: 6561 6479 2829 3b0a 2020 2020 6a73 4c6f  eady();.    jsLo
+00001100: 6767 6572 2822 5b44 6f77 6e6c 6f61 645d  gger("[Download]
+00001110: 2229 0a0a 2020 2020 636f 6e73 7420 6564  ")..    const ed
+00001120: 6974 6f72 203d 2061 6365 2e65 6469 7428  itor = ace.edit(
+00001130: 6564 6974 6f72 4e61 6d65 290a 2020 2020  editorName).    
+00001140: 636f 6e73 7420 7363 7269 7074 4e61 6d65  const scriptName
+00001150: 203d 2065 6469 746f 722e 636f 6e74 6169   = editor.contai
+00001160: 6e65 722e 6765 7441 7474 7269 6275 7465  ner.getAttribute
+00001170: 2827 7079 5f6e 616d 6527 290a 2020 2020  ('py_name').    
+00001180: 636f 6e73 7420 6669 6c65 4e61 6d65 203d  const fileName =
+00001190: 205f 6765 6e65 7261 7465 446f 776e 6c6f   _generateDownlo
+000011a0: 6164 4e61 6d65 2873 6372 6970 744e 616d  adName(scriptNam
+000011b0: 6529 0a20 2020 206c 6574 2069 6465 436f  e).    let ideCo
+000011c0: 6e74 656e 7420 3d20 6564 6974 6f72 2e67  ntent = editor.g
+000011d0: 6574 5661 6c75 6528 2920 2b20 2222 2020  etValue() + ""  
+000011e0: 2020 202f 2f20 656e 666f 7263 6520 7374     // enforce st
+000011f0: 7269 6e67 6966 6963 6174 696f 6e20 696e  ringification in
+00001200: 2061 6e79 2063 6173 650a 0a20 2020 206c   any case..    l
+00001210: 6574 206c 696e 6b20 3d20 646f 6375 6d65  et link = docume
+00001220: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
+00001230: 2822 6122 293b 0a20 2020 206c 6574 2062  ("a");.    let b
+00001240: 6c6f 6220 3d20 6e65 7720 426c 6f62 285b  lob = new Blob([
+00001250: 6964 6543 6f6e 7465 6e74 5d2c 207b 2074  ideContent], { t
+00001260: 7970 653a 2022 7465 7874 2f70 6c61 696e  ype: "text/plain
+00001270: 2220 7d29 3b0a 2020 2020 6c69 6e6b 2e68  " });.    link.h
+00001280: 7265 6620 3d20 5552 4c2e 6372 6561 7465  ref = URL.create
+00001290: 4f62 6a65 6374 5552 4c28 626c 6f62 293b  ObjectURL(blob);
+000012a0: 0a20 2020 206c 696e 6b2e 646f 776e 6c6f  .    link.downlo
+000012b0: 6164 203d 2066 696c 654e 616d 650a 0a20  ad = fileName.. 
+000012c0: 2020 206c 696e 6b2e 636c 6963 6b28 293b     link.click();
+000012d0: 0a20 2020 2055 524c 2e72 6576 6f6b 654f  .    URL.revokeO
+000012e0: 626a 6563 7455 524c 286c 696e 6b2e 6872  bjectURL(link.hr
+000012f0: 6566 293b 0a20 2020 206c 696e 6b2e 7265  ef);.    link.re
+00001300: 6d6f 7665 2829 0a20 2020 2066 6f63 7573  move().    focus
+00001310: 4564 6974 6f72 2865 6469 746f 724e 616d  Editor(editorNam
+00001320: 6529 0a0a 7d2c 2764 6f77 6e6c 6f61 6427  e)..},'download'
+00001330: 290a 0a0a 0a2f 2a2a 2055 706c 6f61 6420  )..../** Upload 
+00001340: 726f 7574 696e 6520 2866 6f72 2074 6865  routine (for the
+00001350: 2069 6e70 7574 2074 6861 7420 6973 2074   input that is t
+00001360: 7269 6767 6572 6564 2062 7920 7468 6520  riggered by the 
+00001370: 7570 6c6f 6164 2062 7574 746f 6e2e 2e2e  upload button...
+00001380: 2920 2a2f 0a63 6f6e 7374 2075 706c 6f61  ) */.const uploa
+00001390: 6452 6f75 7469 6e65 203d 5f3d 3e20 7769  dRoutine =_=> wi
+000013a0: 7468 5079 6f64 6964 6541 7379 6e63 4c6f  thPyodideAsyncLo
+000013b0: 636b 2861 7379 6e63 2066 756e 6374 696f  ck(async functio
+000013c0: 6e28 2920 7b0a 2020 2020 6177 6169 7420  n() {.    await 
+000013d0: 7761 6974 466f 7250 796f 6469 6465 5265  waitForPyodideRe
+000013e0: 6164 7928 293b 0a20 2020 206a 734c 6f67  ady();.    jsLog
+000013f0: 6765 7228 225b 5570 6c6f 6164 5d22 290a  ger("[Upload]").
+00001400: 0a20 2020 206c 6574 206e 756d 6265 7220  .    let number 
+00001410: 3d20 7468 6973 2e69 642e 7370 6c69 7428  = this.id.split(
+00001420: 225f 2229 2e70 6f70 2829 3b0a 2020 2020  "_").pop();.    
+00001430: 6c65 7420 6964 4564 6974 6f72 203d 2022  let idEditor = "
+00001440: 6564 6974 6f72 5f22 202b 206e 756d 6265  editor_" + numbe
+00001450: 723b 0a20 2020 2063 6f6e 7374 2075 706c  r;.    const upl
+00001460: 6f61 6449 6e70 7574 203d 2064 6f63 756d  oadInput = docum
+00001470: 656e 742e 6765 7445 6c65 6d65 6e74 4279  ent.getElementBy
+00001480: 4964 2822 696e 7075 745f 2220 2b20 6964  Id("input_" + id
+00001490: 4564 6974 6f72 290a 2020 2020 7570 6c6f  Editor).    uplo
+000014a0: 6164 496e 7075 742e 6164 6445 7665 6e74  adInput.addEvent
+000014b0: 4c69 7374 656e 6572 2820 2263 6861 6e67  Listener( "chang
+000014c0: 6522 2c20 6675 6e63 7469 6f6e 2028 6576  e", function (ev
+000014d0: 7429 207b 0a20 2020 2020 2020 206c 6574  t) {.        let
+000014e0: 2066 696c 6520 3d20 6576 742e 7461 7267   file = evt.targ
+000014f0: 6574 2e66 696c 6573 5b30 5d3b 0a20 2020  et.files[0];.   
+00001500: 2020 2020 206c 6574 2072 6561 6465 7220       let reader 
+00001510: 3d20 6e65 7720 4669 6c65 5265 6164 6572  = new FileReader
+00001520: 2829 3b0a 2020 2020 2020 2020 7661 7220  ();.        var 
+00001530: 6564 6974 6f72 203d 2061 6365 2e65 6469  editor = ace.edi
+00001540: 7428 6964 4564 6974 6f72 293b 0a20 2020  t(idEditor);.   
+00001550: 2020 2020 2072 6561 6465 722e 6f6e 6c6f       reader.onlo
+00001560: 6164 203d 2066 756e 6374 696f 6e20 2865  ad = function (e
+00001570: 7665 6e74 2920 7b0a 2020 2020 2020 2020  vent) {.        
+00001580: 2020 6564 6974 6f72 2e67 6574 5365 7373    editor.getSess
+00001590: 696f 6e28 292e 7365 7456 616c 7565 2865  ion().setValue(e
+000015a0: 7665 6e74 2e74 6172 6765 742e 7265 7375  vent.target.resu
+000015b0: 6c74 293b 0a20 2020 2020 2020 207d 3b0a  lt);.        };.
+000015c0: 2020 2020 2020 2020 7265 6164 6572 2e72          reader.r
+000015d0: 6561 6441 7354 6578 7428 6669 6c65 293b  eadAsText(file);
+000015e0: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
+000015f0: 6661 6c73 650a 2020 2020 290a 2020 2020  false.    ).    
+00001600: 666f 6375 7345 6469 746f 7228 6964 4564  focusEditor(idEd
+00001610: 6974 6f72 290a 0a7d 2c27 7570 6c6f 6164  itor)..},'upload
+00001620: 2729 0a0a 0a0a 0a0a 2f2f 2d2d 2d2d 2d2d  ')......//------
 00001630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001670: 0a0a 0a0a 2f2a 2a52 6573 6574 2074 6865  ..../**Reset the
-00001680: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-00001690: 6564 6974 6f72 2074 6f20 6974 7320 696e  editor to its in
-000016a0: 6974 6961 6c20 636f 6e74 656e 742c 2061  itial content, a
-000016b0: 6e64 2072 6573 6574 2074 6865 206c 6f63  nd reset the loc
-000016c0: 616c 6553 746f 7261 6765 2066 6f72 0a20  aleStorage for. 
-000016d0: 2a20 7468 6973 2065 6469 746f 7220 6f6e  * this editor on
-000016e0: 2074 6865 2077 6179 2e0a 202a 202a 2f0a   the way.. * */.
-000016f0: 636f 6e73 7420 7265 7374 6172 7420 3d20  const restart = 
-00001700: 2865 6469 746f 724e 616d 6529 203d 3e20  (editorName) => 
-00001710: 7769 7468 5079 6f64 6964 6541 7379 6e63  withPyodideAsync
-00001720: 4c6f 636b 2861 7379 6e63 2066 756e 6374  Lock(async funct
-00001730: 696f 6e28 297b 0a20 2020 2061 7761 6974  ion(){.    await
-00001740: 2077 6169 7446 6f72 5079 6f64 6964 6552   waitForPyodideR
-00001750: 6561 6479 2829 3b0a 2020 2020 6a73 4c6f  eady();.    jsLo
-00001760: 6767 6572 2822 5b52 6573 7461 7274 5d22  gger("[Restart]"
-00001770: 290a 0a20 2020 2063 6f6e 7374 2065 7865  )..    const exe
-00001780: 7263 6973 6543 6f64 6520 3d20 6765 7453  rciseCode = getS
-00001790: 7461 7274 436f 6465 2865 6469 746f 724e  tartCode(editorN
-000017a0: 616d 6529 0a20 2020 2061 7070 6c79 436f  ame).    applyCo
-000017b0: 6465 546f 4564 6974 6f72 416e 6453 6176  deToEditorAndSav
-000017c0: 6528 6564 6974 6f72 4e61 6d65 2c20 6578  e(editorName, ex
-000017d0: 6572 6369 7365 436f 6465 290a 2020 2020  erciseCode).    
-000017e0: 666f 6375 7345 6469 746f 7228 6564 6974  focusEditor(edit
-000017f0: 6f72 4e61 6d65 290a 0a7d 2c27 7265 7374  orName)..},'rest
-00001800: 6172 7427 290a 0a0a 0a2f 2a2a 5361 7665  art')..../**Save
-00001810: 2074 6865 2063 7572 7265 6e74 2049 4445   the current IDE
-00001820: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-00001830: 7573 6572 2c20 6f72 2074 6865 2067 6976  user, or the giv
-00001840: 656e 2063 6f64 652c 2069 6e74 6f20 7468  en code, into th
-00001850: 6520 6c6f 6361 6c65 5374 6f72 6167 650a  e localeStorage.
-00001860: 202a 206f 6620 7468 6520 6e61 7669 6761   * of the naviga
-00001870: 746f 722e 0a20 2a20 2a2f 0a63 6f6e 7374  tor.. * */.const
-00001880: 2073 6176 6520 3d20 2865 6469 746f 724e   save = (editorN
-00001890: 616d 652c 2065 7865 7263 6973 6543 6f64  ame, exerciseCod
-000018a0: 653d 2222 2920 3d3e 2077 6974 6850 796f  e="") => withPyo
-000018b0: 6469 6465 4173 796e 634c 6f63 6b28 6173  dideAsyncLock(as
-000018c0: 796e 6320 6675 6e63 7469 6f6e 2829 7b0a  ync function(){.
-000018d0: 2020 2020 6177 6169 7420 7761 6974 466f      await waitFo
-000018e0: 7250 796f 6469 6465 5265 6164 7928 293b  rPyodideReady();
-000018f0: 0a20 2020 206a 734c 6f67 6765 7228 225b  .    jsLogger("[
-00001900: 5361 7665 5d22 290a 0a20 2020 205f 7361  Save]")..    _sa
-00001910: 7665 2865 6469 746f 724e 616d 652c 2065  ve(editorName, e
-00001920: 7865 7263 6973 6543 6f64 6529 0a20 2020  xerciseCode).   
-00001930: 2066 6f63 7573 4564 6974 6f72 2865 6469   focusEditor(edi
-00001940: 746f 724e 616d 6529 0a0a 7d2c 2773 6176  torName)..},'sav
-00001950: 6527 290a 0a63 6f6e 7374 205f 7361 7665  e')..const _save
-00001960: 203d 2028 6564 6974 6f72 4e61 6d65 2c20   = (editorName, 
-00001970: 6578 6572 6369 7365 436f 6465 3d22 2229  exerciseCode="")
-00001980: 203d 3e20 7b0a 2020 2020 636f 6e73 7420   => {.    const 
-00001990: 6375 7272 656e 7443 6f64 6520 3d20 6578  currentCode = ex
-000019a0: 6572 6369 7365 436f 6465 207c 7c20 6163  erciseCode || ac
-000019b0: 652e 6564 6974 2865 6469 746f 724e 616d  e.edit(editorNam
-000019c0: 6529 2e67 6574 5365 7373 696f 6e28 292e  e).getSession().
-000019d0: 6765 7456 616c 7565 2829 0a20 2020 206c  getValue().    l
-000019e0: 6f63 616c 5374 6f72 6167 652e 7365 7449  ocalStorage.setI
-000019f0: 7465 6d28 6564 6974 6f72 4e61 6d65 2c20  tem(editorName, 
-00001a00: 6375 7272 656e 7443 6f64 6529 3b0a 7d0a  currentCode);.}.
-00001a10: 0a0a 0a0a 0a0a 2f2f 2d2d 2d2d 2d2d 2d2d  ......//--------
+00001670: 2d0a 0a0a 0a2f 2a2a 5265 7365 7420 7468  -..../**Reset th
+00001680: 6520 636f 6e74 656e 7420 6f66 2074 6865  e content of the
+00001690: 2065 6469 746f 7220 746f 2069 7473 2069   editor to its i
+000016a0: 6e69 7469 616c 2063 6f6e 7465 6e74 2c20  nitial content, 
+000016b0: 616e 6420 7265 7365 7420 7468 6520 6c6f  and reset the lo
+000016c0: 6361 6c65 5374 6f72 6167 6520 666f 720a  caleStorage for.
+000016d0: 202a 2074 6869 7320 6564 6974 6f72 206f   * this editor o
+000016e0: 6e20 7468 6520 7761 792e 0a20 2a20 2a2f  n the way.. * */
+000016f0: 0a63 6f6e 7374 2072 6573 7461 7274 203d  .const restart =
+00001700: 2028 6564 6974 6f72 4e61 6d65 2920 3d3e   (editorName) =>
+00001710: 2077 6974 6850 796f 6469 6465 4173 796e   withPyodideAsyn
+00001720: 634c 6f63 6b28 6173 796e 6320 6675 6e63  cLock(async func
+00001730: 7469 6f6e 2829 7b0a 2020 2020 6177 6169  tion(){.    awai
+00001740: 7420 7761 6974 466f 7250 796f 6469 6465  t waitForPyodide
+00001750: 5265 6164 7928 293b 0a20 2020 206a 734c  Ready();.    jsL
+00001760: 6f67 6765 7228 225b 5265 7374 6172 745d  ogger("[Restart]
+00001770: 2229 0a0a 2020 2020 636f 6e73 7420 6578  ")..    const ex
+00001780: 6572 6369 7365 436f 6465 203d 2067 6574  erciseCode = get
+00001790: 5374 6172 7443 6f64 6528 6564 6974 6f72  StartCode(editor
+000017a0: 4e61 6d65 290a 2020 2020 6170 706c 7943  Name).    applyC
+000017b0: 6f64 6554 6f45 6469 746f 7241 6e64 5361  odeToEditorAndSa
+000017c0: 7665 2865 6469 746f 724e 616d 652c 2065  ve(editorName, e
+000017d0: 7865 7263 6973 6543 6f64 6529 0a20 2020  xerciseCode).   
+000017e0: 2066 6f63 7573 4564 6974 6f72 2865 6469   focusEditor(edi
+000017f0: 746f 724e 616d 6529 0a0a 7d2c 2772 6573  torName)..},'res
+00001800: 7461 7274 2729 0a0a 0a0a 2f2a 2a53 6176  tart')..../**Sav
+00001810: 6520 7468 6520 6375 7272 656e 7420 4944  e the current ID
+00001820: 4520 636f 6e74 656e 7420 6f66 2074 6865  E content of the
+00001830: 2075 7365 722c 206f 7220 7468 6520 6769   user, or the gi
+00001840: 7665 6e20 636f 6465 2c20 696e 746f 2074  ven code, into t
+00001850: 6865 206c 6f63 616c 6553 746f 7261 6765  he localeStorage
+00001860: 0a20 2a20 6f66 2074 6865 206e 6176 6967  . * of the navig
+00001870: 6174 6f72 2e0a 202a 202a 2f0a 636f 6e73  ator.. * */.cons
+00001880: 7420 7361 7665 203d 2028 6564 6974 6f72  t save = (editor
+00001890: 4e61 6d65 2c20 6578 6572 6369 7365 436f  Name, exerciseCo
+000018a0: 6465 3d22 2229 203d 3e20 7769 7468 5079  de="") => withPy
+000018b0: 6f64 6964 6541 7379 6e63 4c6f 636b 2861  odideAsyncLock(a
+000018c0: 7379 6e63 2066 756e 6374 696f 6e28 297b  sync function(){
+000018d0: 0a20 2020 2061 7761 6974 2077 6169 7446  .    await waitF
+000018e0: 6f72 5079 6f64 6964 6552 6561 6479 2829  orPyodideReady()
+000018f0: 3b0a 2020 2020 6a73 4c6f 6767 6572 2822  ;.    jsLogger("
+00001900: 5b53 6176 655d 2229 0a0a 2020 2020 5f73  [Save]")..    _s
+00001910: 6176 6528 6564 6974 6f72 4e61 6d65 2c20  ave(editorName, 
+00001920: 6578 6572 6369 7365 436f 6465 290a 2020  exerciseCode).  
+00001930: 2020 666f 6375 7345 6469 746f 7228 6564    focusEditor(ed
+00001940: 6974 6f72 4e61 6d65 290a 0a7d 2c27 7361  itorName)..},'sa
+00001950: 7665 2729 0a0a 636f 6e73 7420 5f73 6176  ve')..const _sav
+00001960: 6520 3d20 2865 6469 746f 724e 616d 652c  e = (editorName,
+00001970: 2065 7865 7263 6973 6543 6f64 653d 2222   exerciseCode=""
+00001980: 2920 3d3e 207b 0a20 2020 2063 6f6e 7374  ) => {.    const
+00001990: 2063 7572 7265 6e74 436f 6465 203d 2065   currentCode = e
+000019a0: 7865 7263 6973 6543 6f64 6520 7c7c 2061  xerciseCode || a
+000019b0: 6365 2e65 6469 7428 6564 6974 6f72 4e61  ce.edit(editorNa
+000019c0: 6d65 292e 6765 7453 6573 7369 6f6e 2829  me).getSession()
+000019d0: 2e67 6574 5661 6c75 6528 290a 2020 2020  .getValue().    
+000019e0: 6c6f 6361 6c53 746f 7261 6765 2e73 6574  localStorage.set
+000019f0: 4974 656d 2865 6469 746f 724e 616d 652c  Item(editorName,
+00001a00: 2063 7572 7265 6e74 436f 6465 293b 0a7d   currentCode);.}
+00001a10: 0a0a 0a0a 0a0a 0a2f 2f2d 2d2d 2d2d 2d2d  .......//-------
 00001a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a60: 2d2d 2d2d 2d2d 2d2d 0a0a 0a0a 0a0a 0a0a  --------........
-00001a70: 2f2a 2a45 7874 7261 6374 2074 6865 2063  /**Extract the c
-00001a80: 7572 7265 6e74 2063 6f6e 7465 6e74 206f  urrent content o
-00001a90: 6620 7468 6520 6769 7665 6e20 6564 6974  f the given edit
-00001aa0: 6f72 2c20 6578 706c 6f72 6520 6974 2c20  or, explore it, 
-00001ab0: 616e 6420 746f 6767 6c65 2061 6c6c 2074  and toggle all t
-00001ac0: 6865 206c 696e 6573 0a20 2a20 666f 756e  he lines. * foun
-00001ad0: 6420 6166 7465 7220 7468 6520 6023 2054  d after the `# T
-00001ae0: 6573 7460 2074 6f6b 656e 2e0a 202a 2052  est` token.. * R
-00001af0: 756c 6573 2066 6f72 2074 6f67 676c 696e  ules for togglin
-00001b00: 6720 6f72 206e 6f74 2061 7265 3a0a 202a  g or not are:. *
-00001b10: 2020 2020 2020 2d20 6c65 6164 696e 6720        - leading 
-00001b20: 7370 6163 6573 2061 7265 2069 676e 6f72  spaces are ignor
-00001b30: 6564 2e0a 202a 2020 2020 2020 2d20 636f  ed.. *      - co
-00001b40: 6d6d 656e 7420 6f75 7420 6966 2074 6865  mment out if the
-00001b50: 2066 6972 7374 2063 6861 7261 6374 6572   first character
-00001b60: 2069 7320 6e6f 7420 2223 222e 0a20 2a20   is not "#".. * 
-00001b70: 2020 2020 202d 2069 6620 7468 6520 6669       - if the fi
-00001b80: 7273 7420 6368 6172 2069 7320 2223 2220  rst char is "#" 
-00001b90: 616e 6420 7468 6572 6520 6973 206e 6f20  and there is no 
-00001ba0: 7370 6163 6573 2062 6568 696e 642c 2075  spaces behind, u
-00001bb0: 6e63 6f6d 6d65 6e74 2e0a 202a 202a 2f0a  ncomment.. * */.
-00001bc0: 6675 6e63 7469 6f6e 2074 6f67 676c 6543  function toggleC
-00001bd0: 6f6d 6d65 6e74 7328 6564 6974 6f72 2920  omments(editor) 
-00001be0: 7b0a 2020 2020 636f 6e73 7420 636f 6465  {.    const code
-00001bf0: 4c69 6e65 7320 3d20 6564 6974 6f72 2e67  Lines = editor.g
-00001c00: 6574 5365 7373 696f 6e28 292e 6765 7456  etSession().getV
-00001c10: 616c 7565 2829 2e73 706c 6974 2827 5c6e  alue().split('\n
-00001c20: 2729 0a20 2020 2063 6f6e 7374 2070 6174  ').    const pat
-00001c30: 7465 726e 2020 203d 2043 4f4e 4649 472e  tern   = CONFIG.
-00001c40: 6c61 6e67 2e74 6573 7473 2e61 735f 7061  lang.tests.as_pa
-00001c50: 7474 6572 6e0a 2020 2020 636f 6e73 7420  ttern.    const 
-00001c60: 6954 6573 7473 546f 6b65 6e20 3d20 636f  iTestsToken = co
-00001c70: 6465 4c69 6e65 732e 6669 6e64 496e 6465  deLines.findInde
-00001c80: 7828 733d 3e70 6174 7465 726e 2e74 6573  x(s=>pattern.tes
-00001c90: 7428 7329 290a 0a20 2020 202f 2f2f 204e  t(s))..    /// N
-00001ca0: 6f20 7465 7374 7320 666f 756e 643a 0a20  o tests found:. 
-00001cb0: 2020 2069 6628 6954 6573 7473 546f 6b65     if(iTestsToke
-00001cc0: 6e3c 3029 2072 6574 7572 6e3b 0a0a 2020  n<0) return;..  
-00001cd0: 2020 636f 6e73 7420 746f 6767 6c65 6420    const toggled 
-00001ce0: 3d20 636f 6465 4c69 6e65 732e 736c 6963  = codeLines.slic
-00001cf0: 6528 6954 6573 7473 546f 6b65 6e2b 3129  e(iTestsToken+1)
-00001d00: 2e6d 6170 2873 3d3e 7b0a 2020 2020 2020  .map(s=>{.      
-00001d10: 2020 7265 7475 726e 2073 2e72 6570 6c61    return s.repla
-00001d20: 6365 2843 4f4e 4649 472e 434f 4d4d 454e  ce(CONFIG.COMMEN
-00001d30: 5445 445f 5041 5454 4552 4e2c 2028 5f2c  TED_PATTERN, (_,
-00001d40: 7370 6163 6573 2c68 6561 642c 7461 696c  spaces,head,tail
-00001d50: 293d 3e7b 0a20 2020 2020 2020 2020 2020  )=>{.           
-00001d60: 2069 6628 6865 6164 3d3d 2723 2720 2626   if(head=='#' &&
-00001d70: 2074 6169 6c21 3d27 2027 2920 7265 7475   tail!=' ') retu
-00001d80: 726e 2073 7061 6365 732b 7461 696c 0a20  rn spaces+tail. 
-00001d90: 2020 2020 2020 2020 2020 2069 6628 6865             if(he
-00001da0: 6164 213d 2723 2729 2072 6574 7572 6e20  ad!='#') return 
-00001db0: 7370 6163 6573 2b27 2327 2b68 6561 642b  spaces+'#'+head+
-00001dc0: 7461 696c 0a20 2020 2020 2020 2020 2020  tail.           
-00001dd0: 2072 6574 7572 6e20 5f0a 2020 2020 2020   return _.      
-00001de0: 2020 7d29 0a20 2020 207d 290a 2020 2020    }).    }).    
-00001df0: 636f 6465 4c69 6e65 732e 7370 6c69 6365  codeLines.splice
-00001e00: 2869 5465 7374 7354 6f6b 656e 2b31 2c20  (iTestsToken+1, 
-00001e10: 746f 6767 6c65 642e 6c65 6e67 7468 2c20  toggled.length, 
-00001e20: 2e2e 2e74 6f67 676c 6564 290a 2020 2020  ...toggled).    
-00001e30: 636f 6e73 7420 7265 706c 203d 2063 6f64  const repl = cod
-00001e40: 654c 696e 6573 2e6a 6f69 6e28 275c 6e27  eLines.join('\n'
-00001e50: 290a 2020 2020 6170 706c 7943 6f64 6554  ).    applyCodeT
-00001e60: 6f45 6469 746f 7241 6e64 5361 7665 2865  oEditorAndSave(e
-00001e70: 6469 746f 722c 2072 6570 6c29 0a20 2020  ditor, repl).   
-00001e80: 2066 6f63 7573 4564 6974 6f72 2865 6469   focusEditor(edi
-00001e90: 746f 722e 636f 6e74 6169 6e65 722e 6964  tor.container.id
-00001ea0: 290a 2020 7d0a 0a0a 0a2f 2a2a 5461 6b65  ).  }..../**Take
-00001eb0: 7320 696e 2074 6865 2069 6420 7374 7269  s in the id stri
-00001ec0: 6e67 206f 6620 616e 2065 6469 746f 722c  ng of an editor,
-00001ed0: 206f 7220 616e 2041 4345 2065 6469 746f   or an ACE edito
-00001ee0: 7220 6173 2066 6972 7374 2061 7267 756d  r as first argum
-00001ef0: 656e 742c 2061 6e64 2074 6865 0a20 2a20  ent, and the. * 
-00001f00: 636f 6465 2073 7472 696e 6720 746f 2061  code string to a
-00001f10: 7070 6c79 2074 6f20 6974 2c20 616e 643a  pply to it, and:
-00001f20: 0a20 2a20 2020 2020 202d 2073 6574 2074  . *      - set t
-00001f30: 6865 2065 6469 746f 7220 636f 6e74 656e  he editor conten
-00001f40: 7420 746f 2074 6861 7420 7374 7269 6e67  t to that string
-00001f50: 0a20 2a20 2020 2020 202d 2073 6176 6520  . *      - save 
-00001f60: 7468 6520 636f 6465 2074 6f20 7468 6520  the code to the 
-00001f70: 6c6f 6361 6c65 5374 6f72 6167 650a 202a  localeStorage. *
-00001f80: 202a 2f0a 6675 6e63 7469 6f6e 2061 7070   */.function app
-00001f90: 6c79 436f 6465 546f 4564 6974 6f72 416e  lyCodeToEditorAn
-00001fa0: 6453 6176 6528 6564 6974 6f72 4f72 4e61  dSave(editorOrNa
-00001fb0: 6d65 2c20 6578 6572 6369 7365 436f 6465  me, exerciseCode
-00001fc0: 297b 0a20 2020 2065 7865 7263 6973 6543  ){.    exerciseC
-00001fd0: 6f64 6520 7c7c 3d20 225c 6e22 2e72 6570  ode ||= "\n".rep
-00001fe0: 6561 7428 3629 0a20 2020 2063 6f6e 7374  eat(6).    const
-00001ff0: 205b 6564 6974 6f72 2c20 6564 6974 6f72   [editor, editor
-00002000: 4e61 6d65 5d0a 2020 2020 2020 2020 3d20  Name].        = 
-00002010: 7479 7065 6f66 2865 6469 746f 724f 724e  typeof(editorOrN
-00002020: 616d 6529 3d3d 2773 7472 696e 6727 203f  ame)=='string' ?
-00002030: 205b 6163 652e 6564 6974 2865 6469 746f   [ace.edit(edito
-00002040: 724f 724e 616d 6529 2c20 6564 6974 6f72  rOrName), editor
-00002050: 4f72 4e61 6d65 5d0a 2020 2020 2020 2020  OrName].        
+00001a60: 2d2d 2d2d 2d2d 2d2d 2d0a 0a0a 0a0a 0a0a  ---------.......
+00001a70: 0a2f 2a2a 4578 7472 6163 7420 7468 6520  ./**Extract the 
+00001a80: 6375 7272 656e 7420 636f 6e74 656e 7420  current content 
+00001a90: 6f66 2074 6865 2067 6976 656e 2065 6469  of the given edi
+00001aa0: 746f 722c 2065 7870 6c6f 7265 2069 742c  tor, explore it,
+00001ab0: 2061 6e64 2074 6f67 676c 6520 616c 6c20   and toggle all 
+00001ac0: 7468 6520 6c69 6e65 730a 202a 2066 6f75  the lines. * fou
+00001ad0: 6e64 2061 6674 6572 2074 6865 2060 2320  nd after the `# 
+00001ae0: 5465 7374 6020 746f 6b65 6e2e 0a20 2a20  Test` token.. * 
+00001af0: 5275 6c65 7320 666f 7220 746f 6767 6c69  Rules for toggli
+00001b00: 6e67 206f 7220 6e6f 7420 6172 653a 0a20  ng or not are:. 
+00001b10: 2a20 2020 2020 202d 206c 6561 6469 6e67  *      - leading
+00001b20: 2073 7061 6365 7320 6172 6520 6967 6e6f   spaces are igno
+00001b30: 7265 642e 0a20 2a20 2020 2020 202d 2063  red.. *      - c
+00001b40: 6f6d 6d65 6e74 206f 7574 2069 6620 7468  omment out if th
+00001b50: 6520 6669 7273 7420 6368 6172 6163 7465  e first characte
+00001b60: 7220 6973 206e 6f74 2022 2322 2e0a 202a  r is not "#".. *
+00001b70: 2020 2020 2020 2d20 6966 2074 6865 2066        - if the f
+00001b80: 6972 7374 2063 6861 7220 6973 2022 2322  irst char is "#"
+00001b90: 2061 6e64 2074 6865 7265 2069 7320 6e6f   and there is no
+00001ba0: 2073 7061 6365 7320 6265 6869 6e64 2c20   spaces behind, 
+00001bb0: 756e 636f 6d6d 656e 742e 0a20 2a20 2a2f  uncomment.. * */
+00001bc0: 0a66 756e 6374 696f 6e20 746f 6767 6c65  .function toggle
+00001bd0: 436f 6d6d 656e 7473 2865 6469 746f 7229  Comments(editor)
+00001be0: 207b 0a20 2020 2063 6f6e 7374 2063 6f64   {.    const cod
+00001bf0: 654c 696e 6573 203d 2065 6469 746f 722e  eLines = editor.
+00001c00: 6765 7453 6573 7369 6f6e 2829 2e67 6574  getSession().get
+00001c10: 5661 6c75 6528 292e 7370 6c69 7428 275c  Value().split('\
+00001c20: 6e27 290a 2020 2020 636f 6e73 7420 7061  n').    const pa
+00001c30: 7474 6572 6e20 2020 3d20 434f 4e46 4947  ttern   = CONFIG
+00001c40: 2e6c 616e 672e 7465 7374 732e 6173 5f70  .lang.tests.as_p
+00001c50: 6174 7465 726e 0a20 2020 2063 6f6e 7374  attern.    const
+00001c60: 2069 5465 7374 7354 6f6b 656e 203d 2063   iTestsToken = c
+00001c70: 6f64 654c 696e 6573 2e66 696e 6449 6e64  odeLines.findInd
+00001c80: 6578 2873 3d3e 7061 7474 6572 6e2e 7465  ex(s=>pattern.te
+00001c90: 7374 2873 2929 0a0a 2020 2020 2f2f 2f20  st(s))..    /// 
+00001ca0: 4e6f 2074 6573 7473 2066 6f75 6e64 3a0a  No tests found:.
+00001cb0: 2020 2020 6966 2869 5465 7374 7354 6f6b      if(iTestsTok
+00001cc0: 656e 3c30 2920 7265 7475 726e 3b0a 0a20  en<0) return;.. 
+00001cd0: 2020 2063 6f6e 7374 2074 6f67 676c 6564     const toggled
+00001ce0: 203d 2063 6f64 654c 696e 6573 2e73 6c69   = codeLines.sli
+00001cf0: 6365 2869 5465 7374 7354 6f6b 656e 2b31  ce(iTestsToken+1
+00001d00: 292e 6d61 7028 733d 3e7b 0a20 2020 2020  ).map(s=>{.     
+00001d10: 2020 2072 6574 7572 6e20 732e 7265 706c     return s.repl
+00001d20: 6163 6528 434f 4e46 4947 2e43 4f4d 4d45  ace(CONFIG.COMME
+00001d30: 4e54 4544 5f50 4154 5445 524e 2c20 285f  NTED_PATTERN, (_
+00001d40: 2c73 7061 6365 732c 6865 6164 2c74 6169  ,spaces,head,tai
+00001d50: 6c29 3d3e 7b0a 2020 2020 2020 2020 2020  l)=>{.          
+00001d60: 2020 6966 2868 6561 643d 3d27 2327 2026    if(head=='#' &
+00001d70: 2620 7461 696c 213d 2720 2729 2072 6574  & tail!=' ') ret
+00001d80: 7572 6e20 7370 6163 6573 2b74 6169 6c0a  urn spaces+tail.
+00001d90: 2020 2020 2020 2020 2020 2020 6966 2868              if(h
+00001da0: 6561 6421 3d27 2327 2920 7265 7475 726e  ead!='#') return
+00001db0: 2073 7061 6365 732b 2723 272b 6865 6164   spaces+'#'+head
+00001dc0: 2b74 6169 6c0a 2020 2020 2020 2020 2020  +tail.          
+00001dd0: 2020 7265 7475 726e 205f 0a20 2020 2020    return _.     
+00001de0: 2020 207d 290a 2020 2020 7d29 0a20 2020     }).    }).   
+00001df0: 2063 6f64 654c 696e 6573 2e73 706c 6963   codeLines.splic
+00001e00: 6528 6954 6573 7473 546f 6b65 6e2b 312c  e(iTestsToken+1,
+00001e10: 2074 6f67 676c 6564 2e6c 656e 6774 682c   toggled.length,
+00001e20: 202e 2e2e 746f 6767 6c65 6429 0a20 2020   ...toggled).   
+00001e30: 2063 6f6e 7374 2072 6570 6c20 3d20 636f   const repl = co
+00001e40: 6465 4c69 6e65 732e 6a6f 696e 2827 5c6e  deLines.join('\n
+00001e50: 2729 0a20 2020 2061 7070 6c79 436f 6465  ').    applyCode
+00001e60: 546f 4564 6974 6f72 416e 6453 6176 6528  ToEditorAndSave(
+00001e70: 6564 6974 6f72 2c20 7265 706c 290a 2020  editor, repl).  
+00001e80: 2020 666f 6375 7345 6469 746f 7228 6564    focusEditor(ed
+00001e90: 6974 6f72 2e63 6f6e 7461 696e 6572 2e69  itor.container.i
+00001ea0: 6429 0a20 207d 0a0a 0a0a 2f2a 2a54 616b  d).  }..../**Tak
+00001eb0: 6573 2069 6e20 7468 6520 6964 2073 7472  es in the id str
+00001ec0: 696e 6720 6f66 2061 6e20 6564 6974 6f72  ing of an editor
+00001ed0: 2c20 6f72 2061 6e20 4143 4520 6564 6974  , or an ACE edit
+00001ee0: 6f72 2061 7320 6669 7273 7420 6172 6775  or as first argu
+00001ef0: 6d65 6e74 2c20 616e 6420 7468 650a 202a  ment, and the. *
+00001f00: 2063 6f64 6520 7374 7269 6e67 2074 6f20   code string to 
+00001f10: 6170 706c 7920 746f 2069 742c 2061 6e64  apply to it, and
+00001f20: 3a0a 202a 2020 2020 2020 2d20 7365 7420  :. *      - set 
+00001f30: 7468 6520 6564 6974 6f72 2063 6f6e 7465  the editor conte
+00001f40: 6e74 2074 6f20 7468 6174 2073 7472 696e  nt to that strin
+00001f50: 670a 202a 2020 2020 2020 2d20 7361 7665  g. *      - save
+00001f60: 2074 6865 2063 6f64 6520 746f 2074 6865   the code to the
+00001f70: 206c 6f63 616c 6553 746f 7261 6765 0a20   localeStorage. 
+00001f80: 2a20 2a2f 0a66 756e 6374 696f 6e20 6170  * */.function ap
+00001f90: 706c 7943 6f64 6554 6f45 6469 746f 7241  plyCodeToEditorA
+00001fa0: 6e64 5361 7665 2865 6469 746f 724f 724e  ndSave(editorOrN
+00001fb0: 616d 652c 2065 7865 7263 6973 6543 6f64  ame, exerciseCod
+00001fc0: 6529 7b0a 2020 2020 6578 6572 6369 7365  e){.    exercise
+00001fd0: 436f 6465 207c 7c3d 2022 5c6e 222e 7265  Code ||= "\n".re
+00001fe0: 7065 6174 2836 290a 2020 2020 636f 6e73  peat(6).    cons
+00001ff0: 7420 5b65 6469 746f 722c 2065 6469 746f  t [editor, edito
+00002000: 724e 616d 655d 0a20 2020 2020 2020 203d  rName].        =
+00002010: 2074 7970 656f 6628 6564 6974 6f72 4f72   typeof(editorOr
+00002020: 4e61 6d65 293d 3d27 7374 7269 6e67 2720  Name)=='string' 
+00002030: 3f20 5b61 6365 2e65 6469 7428 6564 6974  ? [ace.edit(edit
+00002040: 6f72 4f72 4e61 6d65 292c 2065 6469 746f  orOrName), edito
+00002050: 724f 724e 616d 655d 0a20 2020 2020 2020  rOrName].       
 00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 203a 205b 6564 6974 6f72 4f72 4e61 6d65   : [editorOrName
-00002090: 2c20 6564 6974 6f72 4f72 4e61 6d65 2e63  , editorOrName.c
-000020a0: 6f6e 7461 696e 6572 2e69 645d 0a20 2020  ontainer.id].   
-000020b0: 2065 6469 746f 722e 6765 7453 6573 7369   editor.getSessi
-000020c0: 6f6e 2829 2e73 6574 5661 6c75 6528 6578  on().setValue(ex
-000020d0: 6572 6369 7365 436f 6465 293b 0a20 2020  erciseCode);.   
-000020e0: 205f 7361 7665 2865 6469 746f 724e 616d   _save(editorNam
-000020f0: 652c 2065 7865 7263 6973 6543 6f64 6529  e, exerciseCode)
-00002100: 0a7d 0a0a 0a0a 0a63 6f6e 7374 2073 6574  .}.....const set
-00002110: 7570 476c 6f62 616c 4964 6543 6f6d 706f  upGlobalIdeCompo
-00002120: 6e65 6e74 7357 6974 6854 6865 6d65 3d28  nentsWithTheme=(
-00002130: 7468 656d 6529 3d3e 6675 6e63 7469 6f6e  theme)=>function
-00002140: 2829 207b 0a0a 2020 2020 636f 6e73 7420  () {..    const 
-00002150: 6a71 5468 6973 203d 2024 2874 6869 7329  jqThis = $(this)
-00002160: 2020 2020 2020 2f2f 2054 6865 2023 676c        // The #gl
-00002170: 6f62 616c 5f65 6469 746f 725f 7878 7820  obal_editor_xxx 
-00002180: 6469 760a 2020 2020 636f 6e73 7420 6564  div.    const ed
-00002190: 6974 6f72 4e61 6d65 203d 2074 6869 732e  itorName = this.
-000021a0: 6964 2e73 6c69 6365 2827 676c 6f62 616c  id.slice('global
-000021b0: 5f27 2e6c 656e 6774 6829 0a0a 2020 2020  _'.length)..    
-000021c0: 636f 6e73 7420 6964 6520 3d20 6a71 5468  const ide = jqTh
-000021d0: 6973 2e66 696e 6428 2223 222b 6564 6974  is.find("#"+edit
-000021e0: 6f72 4e61 6d65 295b 305d 0a20 2020 2063  orName)[0].    c
-000021f0: 6f6e 7374 2061 6365 4564 6974 6f72 203d  onst aceEditor =
-00002200: 2073 6574 7570 4163 6545 6469 746f 722e   setupAceEditor.
-00002210: 6361 6c6c 2869 6465 2c20 7468 656d 6529  call(ide, theme)
-00002220: 0a0a 2020 2020 636f 6e73 7420 746f 6767  ..    const togg
-00002230: 6c65 7220 3d20 6a71 5468 6973 2e66 696e  ler = jqThis.fin
-00002240: 6428 225b 6964 5e3d 636f 6d6d 656e 745f  d("[id^=comment_
-00002250: 5d22 295b 305d 0a20 2020 2074 6f67 676c  ]")[0].    toggl
-00002260: 6572 2e61 6464 4576 656e 744c 6973 7465  er.addEventListe
-00002270: 6e65 7228 2263 6c69 636b 222c 2028 293d  ner("click", ()=
-00002280: 3e74 6f67 676c 6543 6f6d 6d65 6e74 7328  >toggleComments(
-00002290: 6163 6545 6469 746f 7229 293b 0a0a 2020  aceEditor));..  
-000022a0: 2020 6a71 5468 6973 2e66 696e 6428 2262    jqThis.find("b
-000022b0: 7574 746f 6e22 292e 6561 6368 2866 756e  utton").each(fun
-000022c0: 6374 696f 6e28 297b 0a20 2020 2020 2020  ction(){.       
-000022d0: 2063 6f6e 7374 2062 746e 203d 2024 2874   const btn = $(t
-000022e0: 6869 7329 0a20 2020 2020 2020 2063 6f6e  his).        con
-000022f0: 7374 206b 696e 6420 3d20 6274 6e2e 6174  st kind = btn.at
-00002300: 7472 2827 6274 6e5f 6b69 6e64 2729 0a0a  tr('btn_kind')..
-00002310: 2020 2020 2020 2020 6c65 7420 6361 6c6c          let call
-00002320: 6261 636b 0a20 2020 2020 2020 2073 7769  back.        swi
-00002330: 7463 6828 6b69 6e64 297b 0a20 2020 2020  tch(kind){.     
-00002340: 2020 2020 2020 2063 6173 6520 2770 6c61         case 'pla
-00002350: 7927 3a20 2020 2020 2063 616c 6c62 6163  y':      callbac
-00002360: 6b20 3d20 706c 6179 2865 6469 746f 724e  k = play(editorN
-00002370: 616d 6529 203b 2062 7265 616b 0a20 2020  ame) ; break.   
-00002380: 2020 2020 2020 2020 2063 6173 6520 2776           case 'v
-00002390: 616c 6964 6174 6527 3a20 2063 616c 6c62  alidate':  callb
-000023a0: 6163 6b20 3d20 7661 6c69 6461 7465 2865  ack = validate(e
-000023b0: 6469 746f 724e 616d 6529 203b 2062 7265  ditorName) ; bre
-000023c0: 616b 0a20 2020 2020 2020 2020 2020 2063  ak.            c
-000023d0: 6173 6520 2764 6f77 6e6c 6f61 6427 3a20  ase 'download': 
-000023e0: 2063 616c 6c62 6163 6b20 3d20 646f 776e   callback = down
-000023f0: 6c6f 6164 2865 6469 746f 724e 616d 6529  load(editorName)
-00002400: 203b 2062 7265 616b 0a20 2020 2020 2020   ; break.       
-00002410: 2020 2020 2063 6173 6520 2775 706c 6f61       case 'uploa
-00002420: 6427 3a20 2020 2063 6f6e 7374 2069 6e70  d':    const inp
-00002430: 7574 3d62 746e 2e63 6869 6c64 7265 6e28  ut=btn.children(
-00002440: 2769 6e70 7574 2729 5b30 5d0a 2020 2020  'input')[0].    
+00002080: 2020 3a20 5b65 6469 746f 724f 724e 616d    : [editorOrNam
+00002090: 652c 2065 6469 746f 724f 724e 616d 652e  e, editorOrName.
+000020a0: 636f 6e74 6169 6e65 722e 6964 5d0a 2020  container.id].  
+000020b0: 2020 6564 6974 6f72 2e67 6574 5365 7373    editor.getSess
+000020c0: 696f 6e28 292e 7365 7456 616c 7565 2865  ion().setValue(e
+000020d0: 7865 7263 6973 6543 6f64 6529 3b0a 2020  xerciseCode);.  
+000020e0: 2020 5f73 6176 6528 6564 6974 6f72 4e61    _save(editorNa
+000020f0: 6d65 2c20 6578 6572 6369 7365 436f 6465  me, exerciseCode
+00002100: 290a 7d0a 0a0a 0a0a 636f 6e73 7420 7365  ).}.....const se
+00002110: 7475 7047 6c6f 6261 6c49 6465 436f 6d70  tupGlobalIdeComp
+00002120: 6f6e 656e 7473 5769 7468 5468 656d 653d  onentsWithTheme=
+00002130: 2874 6865 6d65 293d 3e66 756e 6374 696f  (theme)=>functio
+00002140: 6e28 2920 7b0a 0a20 2020 2063 6f6e 7374  n() {..    const
+00002150: 206a 7154 6869 7320 3d20 2428 7468 6973   jqThis = $(this
+00002160: 2920 2020 2020 202f 2f20 5468 6520 2367  )      // The #g
+00002170: 6c6f 6261 6c5f 6564 6974 6f72 5f78 7878  lobal_editor_xxx
+00002180: 2064 6976 0a20 2020 2063 6f6e 7374 2065   div.    const e
+00002190: 6469 746f 724e 616d 6520 3d20 7468 6973  ditorName = this
+000021a0: 2e69 642e 736c 6963 6528 2767 6c6f 6261  .id.slice('globa
+000021b0: 6c5f 272e 6c65 6e67 7468 290a 0a20 2020  l_'.length)..   
+000021c0: 2063 6f6e 7374 2069 6465 203d 206a 7154   const ide = jqT
+000021d0: 6869 732e 6669 6e64 2822 2322 2b65 6469  his.find("#"+edi
+000021e0: 746f 724e 616d 6529 5b30 5d0a 2020 2020  torName)[0].    
+000021f0: 636f 6e73 7420 6163 6545 6469 746f 7220  const aceEditor 
+00002200: 3d20 7365 7475 7041 6365 4564 6974 6f72  = setupAceEditor
+00002210: 2e63 616c 6c28 6964 652c 2074 6865 6d65  .call(ide, theme
+00002220: 290a 0a20 2020 2063 6f6e 7374 2074 6f67  )..    const tog
+00002230: 676c 6572 203d 206a 7154 6869 732e 6669  gler = jqThis.fi
+00002240: 6e64 2822 5b69 645e 3d63 6f6d 6d65 6e74  nd("[id^=comment
+00002250: 5f5d 2229 5b30 5d0a 2020 2020 746f 6767  _]")[0].    togg
+00002260: 6c65 722e 6164 6445 7665 6e74 4c69 7374  ler.addEventList
+00002270: 656e 6572 2822 636c 6963 6b22 2c20 2829  ener("click", ()
+00002280: 3d3e 746f 6767 6c65 436f 6d6d 656e 7473  =>toggleComments
+00002290: 2861 6365 4564 6974 6f72 2929 3b0a 0a20  (aceEditor));.. 
+000022a0: 2020 206a 7154 6869 732e 6669 6e64 2822     jqThis.find("
+000022b0: 6275 7474 6f6e 2229 2e65 6163 6828 6675  button").each(fu
+000022c0: 6e63 7469 6f6e 2829 7b0a 2020 2020 2020  nction(){.      
+000022d0: 2020 636f 6e73 7420 6274 6e20 3d20 2428    const btn = $(
+000022e0: 7468 6973 290a 2020 2020 2020 2020 636f  this).        co
+000022f0: 6e73 7420 6b69 6e64 203d 2062 746e 2e61  nst kind = btn.a
+00002300: 7474 7228 2762 746e 5f6b 696e 6427 290a  ttr('btn_kind').
+00002310: 0a20 2020 2020 2020 206c 6574 2063 616c  .        let cal
+00002320: 6c62 6163 6b0a 2020 2020 2020 2020 7377  lback.        sw
+00002330: 6974 6368 286b 696e 6429 7b0a 2020 2020  itch(kind){.    
+00002340: 2020 2020 2020 2020 6361 7365 2027 706c          case 'pl
+00002350: 6179 273a 2020 2020 2020 6361 6c6c 6261  ay':      callba
+00002360: 636b 203d 2070 6c61 7928 6564 6974 6f72  ck = play(editor
+00002370: 4e61 6d65 2920 3b20 6272 6561 6b0a 2020  Name) ; break.  
+00002380: 2020 2020 2020 2020 2020 6361 7365 2027            case '
+00002390: 7661 6c69 6461 7465 273a 2020 6361 6c6c  validate':  call
+000023a0: 6261 636b 203d 2076 616c 6964 6174 6528  back = validate(
+000023b0: 6564 6974 6f72 4e61 6d65 2920 3b20 6272  editorName) ; br
+000023c0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+000023d0: 6361 7365 2027 646f 776e 6c6f 6164 273a  case 'download':
+000023e0: 2020 6361 6c6c 6261 636b 203d 2064 6f77    callback = dow
+000023f0: 6e6c 6f61 6428 6564 6974 6f72 4e61 6d65  nload(editorName
+00002400: 2920 3b20 6272 6561 6b0a 2020 2020 2020  ) ; break.      
+00002410: 2020 2020 2020 6361 7365 2027 7570 6c6f        case 'uplo
+00002420: 6164 273a 2020 2020 636f 6e73 7420 696e  ad':    const in
+00002430: 7075 743d 6274 6e2e 6368 696c 6472 656e  put=btn.children
+00002440: 2827 696e 7075 7427 295b 305d 0a20 2020  ('input')[0].   
 00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-00002470: 636b 203d 2069 6e70 7574 2e63 6c69 636b  ck = input.click
-00002480: 2e62 696e 6428 696e 7075 7429 203b 2062  .bind(input) ; b
-00002490: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-000024a0: 2063 6173 6520 2772 6573 7461 7274 273a   case 'restart':
-000024b0: 2020 2063 616c 6c62 6163 6b20 3d20 7265     callback = re
-000024c0: 7374 6172 7428 6564 6974 6f72 4e61 6d65  start(editorName
-000024d0: 2920 3b20 6272 6561 6b0a 2020 2020 2020  ) ; break.      
-000024e0: 2020 2020 2020 6361 7365 2027 7361 7665        case 'save
-000024f0: 273a 2020 2020 2020 6361 6c6c 6261 636b  ':      callback
-00002500: 203d 2073 6176 6528 6564 6974 6f72 4e61   = save(editorNa
-00002510: 6d65 2920 3b20 6272 6561 6b0a 2020 2020  me) ; break.    
-00002520: 2020 2020 2020 2020 6465 6661 756c 743a          default:
-00002530: 2020 2020 2020 2020 2020 7468 726f 7720            throw 
-00002540: 6e65 7720 4572 726f 7228 6059 2773 686f  new Error(`Y'sho
-00002550: 756c 6420 6e65 7665 7220 6765 7420 7468  uld never get th
-00002560: 6572 652c 206d 6174 652e 2e2e 2028 247b  ere, mate... (${
-00002570: 206b 696e 6420 7d29 6029 0a20 2020 2020   kind })`).     
-00002580: 2020 207d 0a20 2020 2020 2020 2062 746e     }.        btn
-00002590: 2e6f 6e28 2763 6c69 636b 272c 2063 616c  .on('click', cal
-000025a0: 6c62 6163 6b29 0a20 2020 207d 290a 0a20  lback).    }).. 
-000025b0: 2020 202f 2f20 496e 6974 6961 7465 2061     // Initiate a
-000025c0: 6c6c 2074 6572 6d69 6e61 6c73 2069 6e20  ll terminals in 
-000025d0: 7468 6520 7061 6765 0a20 2020 206a 7154  the page.    jqT
-000025e0: 6869 732e 6669 6e64 2822 2374 6572 6d5f  his.find("#term_
-000025f0: 222b 6564 6974 6f72 4e61 6d65 292e 6561  "+editorName).ea
-00002600: 6368 2861 7379 6e63 2066 756e 6374 696f  ch(async functio
-00002610: 6e28 297b 0a20 2020 2020 2020 2063 6f6e  n(){.        con
-00002620: 7374 2069 6420 3d20 7468 6973 2e69 640a  st id = this.id.
-00002630: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00002640: 7475 704f 7247 6574 5465 726d 696e 616c  tupOrGetTerminal
-00002650: 416e 6450 7945 6e76 2869 6429 0a20 2020  AndPyEnv(id).   
-00002660: 207d 290a 7d0a                            }).}.
+00002460: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
+00002470: 6163 6b20 3d20 696e 7075 742e 636c 6963  ack = input.clic
+00002480: 6b2e 6269 6e64 2869 6e70 7574 2920 3b20  k.bind(input) ; 
+00002490: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+000024a0: 2020 6361 7365 2027 7265 7374 6172 7427    case 'restart'
+000024b0: 3a20 2020 6361 6c6c 6261 636b 203d 2072  :   callback = r
+000024c0: 6573 7461 7274 2865 6469 746f 724e 616d  estart(editorNam
+000024d0: 6529 203b 2062 7265 616b 0a20 2020 2020  e) ; break.     
+000024e0: 2020 2020 2020 2063 6173 6520 2773 6176         case 'sav
+000024f0: 6527 3a20 2020 2020 2063 616c 6c62 6163  e':      callbac
+00002500: 6b20 3d20 7361 7665 2865 6469 746f 724e  k = save(editorN
+00002510: 616d 6529 203b 2062 7265 616b 0a20 2020  ame) ; break.   
+00002520: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00002530: 3a20 2020 2020 2020 2020 2074 6872 6f77  :          throw
+00002540: 206e 6577 2045 7272 6f72 2860 5927 7368   new Error(`Y'sh
+00002550: 6f75 6c64 206e 6576 6572 2067 6574 2074  ould never get t
+00002560: 6865 7265 2c20 6d61 7465 2e2e 2e20 2824  here, mate... ($
+00002570: 7b20 6b69 6e64 207d 2960 290a 2020 2020  { kind })`).    
+00002580: 2020 2020 7d0a 2020 2020 2020 2020 6274      }.        bt
+00002590: 6e2e 6f6e 2827 636c 6963 6b27 2c20 6361  n.on('click', ca
+000025a0: 6c6c 6261 636b 290a 2020 2020 7d29 0a0a  llback).    })..
+000025b0: 2020 2020 2f2f 2049 6e69 7469 6174 6520      // Initiate 
+000025c0: 616c 6c20 7465 726d 696e 616c 7320 696e  all terminals in
+000025d0: 2074 6865 2070 6167 650a 2020 2020 6a71   the page.    jq
+000025e0: 5468 6973 2e66 696e 6428 2223 7465 726d  This.find("#term
+000025f0: 5f22 2b65 6469 746f 724e 616d 6529 2e65  _"+editorName).e
+00002600: 6163 6828 6173 796e 6320 6675 6e63 7469  ach(async functi
+00002610: 6f6e 2829 7b0a 2020 2020 2020 2020 636f  on(){.        co
+00002620: 6e73 7420 6964 203d 2074 6869 732e 6964  nst id = this.id
+00002630: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+00002640: 6574 7570 4f72 4765 7454 6572 6d69 6e61  etupOrGetTermina
+00002650: 6c41 6e64 5079 456e 7628 6964 290a 2020  lAndPyEnv(id).  
+00002660: 2020 7d29 0a7d 0a                          }).}.
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,29 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
 
+
+/**Extract the content of the header code for the given editorName, and run its content
+ * into pyodide environment.
+ * */
+async function runHdrContent(editorName, options, terminal) {
+    const headerContent = securedExtraction(editorName, CONFIG.ideProp.hdrContent)
+    if (headerContent) {
+        await installAndImportMissingModules(headerContent, options, terminal)
+        await pyodide.runPythonAsync(headerContent, {
+            filename: '<env>'
+        })
+    }
+}
+
+
 /**Prepare the runtime python environment:
  *  - Save the current code in the editor to LocaleStorage
  *  - Refresh the basic functionalities
  *  - Refresh any HDR content in the environment
  *  - Refresh any exclusion logistic, by defining extra functions in the environment
  *  - Returns the modified code, with the active terminal
  */
@@ -33,34 +48,37 @@
 
     // save before anything else, in case an error occur somewhere...
     _save(editorName, aceCode)
 
 
     // Build the default configuration options to use to run the user's code:
     const options = buildOptionsForPyodideRun(editorName)
-
-    // Refresh the pyodide environment, before running anything, and pause it (so that
-    // the ">>>" are not displayed during the executions):
     const terminal = await setupOrGetTerminalAndPyEnv("term_" + editorName, true);
-    terminal.pause()
-    terminal.clear()
-    terminal.echo(CONFIG.lang.runScript.msg)
-    await sleep() // Enforce UI refresh
 
-    // Run before clearing the terminal, in case someone forgot a print:
+    terminal.pause() // Pause is to avoid ">>>" showing up during executions
+    terminal.clear() // Erase previous content
+    terminal.echo(CONFIG.lang.runScript.msg) // tell the user it started to run
+    await sleep() // Make sure the change is noticeable
+
+    let stdErr = '',
+        gotErr
     setupStdIO()
-    let stdErr = ''
     try {
         await runHdrContent(editorName, options, terminal)
     } catch (err) {
+        gotErr = err
         stdErr = generateErrorLog(err, "", false, false)
     } finally {
-        let someMsg = (getFullStdIO() || "") + stdErr
+        let someMsg = getFullStdIO() + stdErr
         if (someMsg) terminal.echo(someMsg)
     }
+    if (gotErr) {
+        terminal.resume()
+        throw gotErr // Reraise, stopping executions if error
+    }
 
     return [aceCode, terminal, options]
 }
 
 
 
 /**Actions performed once all the running code steps have been completed.
@@ -96,26 +114,14 @@
 
 
 
 
 
 
 
-/**Extract the content of the header code for the given editorName, and run its content
- * into pyodide environment.
- * */
-async function runHdrContent(editorName, options, terminal) {
-    const headerContent = securedExtraction(editorName, CONFIG.ideProp.hdrContent)
-    if (headerContent) {
-        await installAndImportMissingModules(headerContent, options, terminal)
-        pyodide.runPython(headerContent)
-    }
-}
-
-
 
 function getAttemptsLeft(editorName) {
     return securedExtraction(editorName, CONFIG.ideProp.attemptsLeft)
 }
 
 
 
@@ -158,15 +164,15 @@
 
 
 
 
 /**Build an additional final message to add after an error message (which has already been
  * displayed in the terminal.
  * */
-function enhanceFailureMsg(editorName, stdErr) {
+function enhanceFailureMsg(editorName, _stdErr) {
     let out = getSolRemTxt(editorName, false)
     return out
 }
 
 
 
 /**Build the full success message
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -159,19 +159,19 @@
 
             // Now only, compute the error message if needed.
             if (delayedErr) {
                 stdErr = generateErrorLog(delayedErr, code, options.autoLogAssert, !isPublicRun)
             }
 
             // Always extract the stdout and close the buffer (avoid memory leaks)
-            let captured = getFullStdIO() || ""
+            let captured = getFullStdIO()
 
             // Send stdout feedback to the user only if allowed:
             if (options.withStdOut) {
-                stdOut = escapeSquareBrackets(textShortener(captured))
+                stdOut = textShortener(captured)
             }
 
         } catch (err) {
             // This second catch is there so that the user can see the JS error in the terminal.
             // (Note: maybe I should actually throw them again...?)
             stdErr = generateErrorLog(err, code, true, false)
 
@@ -281,24 +281,24 @@
     def _hack():
         import sys, io
         sys.stdout = io.StringIO()
     _hack()
     del _hack
 `)
 
-const getFullStdIO = _ => pyodide.runPython(`
+const getFullStdIO = _ => escapeSquareBrackets(pyodide.runPython(`
     def _hack():
         import sys
         __builtins__._stdout = sys.stdout.getvalue()
         sys.stdout.close()
 
     _hack()
     del _hack
     __builtins__._stdout
-`)
+`) || '')
 
 
 
 
 /*
 ------------------------------------------------------------------
                       Manage code exclusions
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -37,14 +37,15 @@
  * - "Legit" errors are studied and cleaned up in various ways. Mostly:
  *   - remove any lines related to pyodide environment (unless the error is identified as "legit",
  *     but also problematic)
  *   - possibly add the assertion code (if allowed) for bare AssertionErrors.
  *   - reduce the size of the stacktrace and/or the error message if they are too big (to avoid
  *     having the terminal lagging like hell...)
  *
+ *
  * ## Searching for AssertionError:
  *
  * This is not totally trivial, because it must be made sure that the code finds the actual error
  * type declaration in the string, and not a false positive:
  *
  *      ```python
  *      raise ValueError("should be AssertionError")
@@ -60,44 +61,63 @@
  *      -> Forbids simple `startsWith` checks.
  *
  * To avoid this, "AssertionError" is searched at the beginning of a line, with the previous line
  * starting with '  File "<exec>"'.
  *
  * Note: the online REPL show a '  File "<console>"' instead, but the behavior stays the same.
  *
+ *
  * ---
  *
+ *
  * Example of an input error message in pyodide 0.23.1:
  *
  *      PythonError: Traceback (most recent call last):
  *        File "/lib/python3.10/site-packages/_pyodide/_base.py", line 435, in eval_code
  *          .run(globals, locals)
  *        File "/lib/python3.10/site-packages/_pyodide/_base.py", line 304, in run
  *          coroutine = eval(self.code, globals, locals)
  *        File "<exec>", line 4, in <module>
  *        File "<exec>", line 7, in ecrete
  *        File "<exec>", line 12, in limite_amplitude
  *      ValueError: blabla
  *
+ *
  * Example of an input error message in pyodide 0.25.0:
  *
  *      PythonError: Traceback (most recent call last):
  *        File "/lib/python311.zip/_pyodide/_base.py", line 501, in eval_code
  *          .run(globals, locals)
  *           ^^^^^^^^^^^^^^^^^^^^
  *        File "/lib/python311.zip/_pyodide/_base.py", line 339, in run
  *          coroutine = eval(self.code, globals, locals)
  *                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  *        File "<exec>", line 1, in <module>
  *      AssertionError: This message...
  *
+ *
+ * Example of error involving RecursionError with repeated lines:
+ *
+ *     PythonError: Traceback (most recent call last):
+ *       File "/lib/python311.zip/_pyodide/_base.py", line 501, in eval_code
+ *         .run(globals, locals)
+ *          ^^^^^^^^^^^^^^^^^^^^
+ *       File "/lib/python311.zip/_pyodide/_base.py", line 339, in run
+ *         coroutine = eval(self.code, globals, locals)
+ *                     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+ *       File "<exec>", line 2, in <module>
+ *       File "<env>", line 10, in essai
+ *       File "<env>", line 10, in essai
+ *       File "<env>", line 10, in essai
+ *       [Previous line repeated 44 more times]
+ *     RecursionError: maximum recursion depth exceeded
  * */
 function generateErrorLog(err, code, allowAssertionCodeExtraction, purgeErr) {
 
-    const msg = String(err).trimEnd() // Note: err has a trailing linefeed, s trim it...
+    const msg = String(err).trimEnd() // Note: err has a trailing linefeed, so, trim it...
 
     // Return directly non python errors. => allows to also see JS errors.
     if (!msg.startsWith('PythonError')) {
         return youAreInTroubles(err)
     }
 
     const errLines = msg.split("\n")
@@ -105,16 +125,15 @@
     /*
     Search for the first line after the pyodide-specific infos, avoiding false positives for
     terminals, where the second line is: ""  File "<exec>", line dd, in await_fut".
     Also, in case of SyntaxError, there is no indication after the line number (REMINDER: the
     negative lookahead CANNOT start just after the number or the await_fut thing is matched
     when the line number has more than 1 digit..., so must use another strategy).
     */
-    const moduleReg = /File "<(exec|console)>", line (\d+)($|, in (?!await_fut))/
-    const iModule = errLines.findIndex(s => moduleReg.test(s))
+    const iModule = errLines.findIndex(s => CONFIG.MODULE_REG.test(s))
 
     /*
     Python errors may sometimes be coming from side effects of restrictions: those may not come
     from the execution of the user's code and the stacktrace, may then not content the desired
     pattern, aka, the "file" may be neither exec nor console. (this happens for example with a
     recursion limit set too low: the error is raised when extracting stdout only).
     */
@@ -203,20 +222,30 @@
 
 /**Travel through the lines of an error message from the end, and spot the line index of the
  * raised Error, assuming it will be preceded by a line starting with `  File "<(exec|console)>"`
  * and return the index of the error line, and a boolean saying if the error was or not an
  * AssertionError.
  * */
 const getErrorKindInfos = (arr) => {
-    const traceReg = /  File "<(exec|console)>"/
     for (let i = arr.length - 1; i > 0; i--) {
         const previousLine = arr[i - 1] // Always defined, see loop stop
         const line = arr[i]
-        const isLastTrace = traceReg.test(previousLine)
+
+        const isLastTrace = CONFIG.TRACE_REG.test(previousLine)
         if (isLastTrace) {
+            // RecursionError may return a message with an extra line
+            if (line.startsWith("  [Previous line repeated")) {
+                if (!arr[++i] || !arr[i].startsWith('RecursionError')) {
+                    throw new Error(
+                        `Expected RecursionError, but found something else:\n\n${ arr.join('\n') }`
+                    )
+                }
+                return [i, false]
+            }
+
             return [i, line.startsWith('AssertionError')]
         }
     }
     return [arr.length - 1, false]
 }
 
 
@@ -226,15 +255,15 @@
  * through the use of the ast module in pyodide, then mutate the array representing
  * the error message accordingly.
  * */
 function buildAssertionMsg(code, errLines, iAssertionError) {
 
     const callLine = errLines[iAssertionError - 1] || ""
 
-    const numMatch = callLine.match(/File "<(?:exec|console)>", line (\d+)/)
+    const numMatch = callLine.match(CONFIG.TRACE_NUM_LINE)
     if (!numMatch) {
         throw new Error(`
 Couldn't determine the line number of the assertion in:
       ${ callLine }
     Error message:\n${ errLines.join('\n') }`)
     }
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -39,19 +39,17 @@
             <path class="st0" d="M256,248.674c10.017,0,18.131-8.122,18.131-18.139c3.032-12.051,9.397-23.161,18.578-31.757l42.542-39.888 c13.592-12.739,21.602-30.448,22.446-48.984H154.302c0.844,18.536,8.854,36.245,22.438,48.984l42.541,39.888 c9.19,8.596,15.547,19.706,18.579,31.757C237.861,240.552,245.983,248.674,256,248.674z"></path>
             <path class="st0" d="M256,267.796c-10.017,0-18.139,8.122-18.139,18.139c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,275.918,266.017,267.796,256,267.796z"></path>
             <path class="st0" d="M256,332.137c-10.017,0-18.139,8.122-18.139,18.14c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,340.259,266.017,332.137,256,332.137z"></path>
             <path class="st0" d="M239.876,389.742l-66.538,66.538h165.315l-66.537-66.538C263.21,380.845,248.782,380.845,239.876,389.742z"></path>
         </g>
     </g>
 </svg>`
-
-        const wrappingDiv = `<div id="${ CONFIG.element.searchBtnsLeft.slice(1) }">${ hourGlassSvg }</div>`
-        $(wrappingDiv).insertBefore(CONFIG.element.dayNight)
+        $(CONFIG.element.searchBtnsLeft).prepend($(hourGlassSvg))
     }, {
-        waitFor: CONFIG.element.dayNight
+        waitFor: CONFIG.element.searchBtnsLeft
     },
 )
 
 
 
 
 
@@ -77,15 +75,15 @@
 /**This is what's triggering the huge lag, when loading the page, so do it only when an ide or
  * or terminal is needed, and do it on next tick, so that all the scripts are actually loaded first
  * */
 setTimeout(async () => {
 
     globalThis.pyodide = await loadPyodide()
 
-    globalThis.pyFuncs = extractPyodideConsoleCallbacks()
+    globalThis.pyFuncs = setupPyodideEnvironmentTools()
 
     pyodide._module.on_fatal = withPyodideAsyncLock(async (e) => {
         const term = $.terminal.active()
         term.error(
             "Pyodide has suffered a fatal error. Please report this to the Pyodide maintainers."
         )
         term.error("The cause of the fatal error was:")
@@ -104,15 +102,15 @@
 /**Creates the console: the variable pyconsole, which is the runtime tool behind the  "terminal
  * process" is created here.
  * Returns the PyodideConsoleManager which handles the python functions needed to control the
  * python console from the JS layer
  *
  * https://pyodide.org/en/stable/usage/api/python-api/console.html#pyodide.console.PyodideConsole
  * */
-function extractPyodideConsoleCallbacks() {
+function setupPyodideEnvironmentTools() {
 
     // Indentation does matter a bit: 1 extra indent is ok, but 2 fails (whatever... :rolleyes: )
     const pythonRoutinesExtractionCode = `
     def _hack():
         import js
         import __main__
         from pyodide.console import PyodideConsole, repr_shorten
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -55,15 +55,15 @@
     } else {
         jsLogger("[Terminal] - Initiate " + termId)
 
         // Create the jQuery terminal, then bind the python stdout/err:
         term = buildInteractiveTerminalSession(termId)
     }
 
-    setupAdditionalPythonEnvironmentFeatures()
+    setupOrRefreshPythonEnvironmentFeatures()
 
     CONFIG.terms[termId] = term;
     // ...To avoid garbage collection? (apparently not!!)
     // But useful to avoid creating a new one on the next execution...!
 
     // Enforce vertical scroll position by focusing on the #py_mk_pin_scroll_input
     jsLogger("[Terminal] - isCreation && !focus =", isCreation && !focus)
@@ -74,15 +74,15 @@
 
 
 
 
 
 /**Add recursion limiter features to the python environment.
  * */
-const setupAdditionalPythonEnvironmentFeatures = (options = {}) => {
+const setupOrRefreshPythonEnvironmentFeatures = (options = {}) => {
 
     options = {
         exclusionsTools: true,
         inputPrompt: true,
         version: true,
         ...options
     };
```

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.0/pyproject.toml` & `pyodide_mkdocs_theme-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.6.0"
+version = "0.6.1"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.6.0/PKG-INFO` & `pyodide_mkdocs_theme-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.6.0
+Version: 0.6.1
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

