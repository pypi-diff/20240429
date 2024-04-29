# Comparing `tmp/parityos-2.4.0.tar.gz` & `tmp/parityos-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parityos-2.4.0.tar", last modified: Thu Feb 22 16:13:13 2024, max compression
+gzip compressed data, was "parityos-2.5.0.tar", last modified: Mon Apr 29 13:19:40 2024, max compression
```

## Comparing `parityos-2.4.0.tar` & `parityos-2.5.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1892 2024-02-22 15:13:41.000000 parityos-2.4.0/License.txt
--rw-r--r--   0 root         (0) root         (0)      531 2024-02-22 16:13:13.873875 parityos-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4307 2024-02-22 15:13:41.000000 parityos-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.853875 parityos-2.4.0/parityos/
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.857875 parityos-2.4.0/parityos/api_interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:13:03.000000 parityos-2.4.0/parityos/api_interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/api_interface/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     3976 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/api_interface/compiler_run.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/api_interface/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/api_interface/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.857875 parityos-2.4.0/parityos/base/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8227 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     4344 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    18260 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/gates.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/problem_representation.py
--rw-rw-rw-   0 root         (0) root         (0)     1983 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/qubits.py
--rw-rw-rw-   0 root         (0) root         (0)     4312 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/base/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6248 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/compiler_client.py
--rw-rw-rw-   0 root         (0) root         (0)     6990 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/device_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.857875 parityos-2.4.0/parityos/encodings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:13:03.000000 parityos-2.4.0/parityos/encodings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/encodings/mappings.py
--rw-rw-rw-   0 root         (0) root         (0)    12750 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/encodings/parity_decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/encodings/parity_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)    11356 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos/encodings/parityos_output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/parityos.egg-info/
--rw-r--r--   0 root         (0) root         (0)      531 2024-02-22 16:13:13.000000 parityos-2.4.0/parityos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5893 2024-02-22 16:13:13.000000 parityos-2.4.0/parityos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 16:13:13.000000 parityos-2.4.0/parityos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-02-22 16:13:13.000000 parityos-2.4.0/parityos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-02-22 16:13:13.000000 parityos-2.4.0/parityos.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.857875 parityos-2.4.0/parityos_addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.857875 parityos-2.4.0/parityos_addons/documentation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:13:03.000000 parityos-2.4.0/parityos_addons/documentation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/_images/
--rw-r--r--   0 root         (0) root         (0)   188899 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_images/hypergraph_solution_tutorial.png
--rw-r--r--   0 root         (0) root         (0)   187919 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_images/hypergraph_tutorial.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/_sources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/
--rw-r--r--   0 root         (0) root         (0)      121 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/api_interface.rst.txt
--rw-r--r--   0 root         (0) root         (0)      243 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/base.rst.txt
--rw-r--r--   0 root         (0) root         (0)      224 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/encodings.rst.txt
--rw-r--r--   0 root         (0) root         (0)      151 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/index.rst.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/parityos.rst.txt
--rw-r--r--   0 root         (0) root         (0)      253 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/api_reference/parityos_addons.rst.txt
--rw-r--r--   0 root         (0) root         (0)     2738 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/asynchronous_submission.rst.txt
--rw-r--r--   0 root         (0) root         (0)     8557 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/custom_device_models.rst.txt
--rw-r--r--   0 root         (0) root         (0)      262 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/index.rst.txt
--rw-r--r--   0 root         (0) root         (0)     1454 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/installation.rst.txt
--rw-r--r--   0 root         (0) root         (0)     3486 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/parity_decoder.rst.txt
--rw-r--r--   0 root         (0) root         (0)     9548 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/quickstart.rst.txt
--rw-r--r--   0 root         (0) root         (0)    17652 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/html/_sources/tutorial.rst.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/_static/
--rw-r--r--   0 root         (0) root         (0)     4289 2024-02-22 16:12:51.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 root         (0) root         (0)    15094 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/basic.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.861875 parityos-2.4.0/parityos_addons/documentation/html/_static/css/
--rw-r--r--   0 root         (0) root         (0)     3229 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/badge_only.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.869875 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/
--rw-r--r--   0 root         (0) root         (0)    87624 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 root         (0) root         (0)    67312 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 root         (0) root         (0)    86288 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 root         (0) root         (0)    66444 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 root         (0) root         (0)   165742 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)   323344 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 root         (0) root         (0)   193308 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 root         (0) root         (0)   309728 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 root         (0) root         (0)   184912 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 root         (0) root         (0)   328412 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 root         (0) root         (0)   195704 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 root         (0) root         (0)   309192 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 root         (0) root         (0)   182708 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 root         (0) root         (0)   135314 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     4472 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      328 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)    89501 2024-02-22 16:12:51.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/jquery.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.869875 parityos-2.4.0/parityos_addons/documentation/html/_static/js/
--rw-r--r--   0 root         (0) root         (0)      934 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/js/badge_only.js
--rw-r--r--   0 root         (0) root         (0)     4370 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 root         (0) root         (0)     2734 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/js/html5shiv.min.js
--rw-r--r--   0 root         (0) root         (0)     5023 2024-02-10 21:11:56.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)     4758 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4902 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18732 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     5123 2024-02-10 21:11:55.000000 parityos-2.4.0/parityos_addons/documentation/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/parityos_addons/documentation/html/api_reference/
--rw-r--r--   0 root         (0) root         (0)     5808 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/api_interface.html
--rw-r--r--   0 root         (0) root         (0)   135553 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/base.html
--rw-r--r--   0 root         (0) root         (0)    44306 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/encodings.html
--rw-r--r--   0 root         (0) root         (0)     6188 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/index.html
--rw-r--r--   0 root         (0) root         (0)    88197 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/parityos.html
--rw-r--r--   0 root         (0) root         (0)    36442 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/api_reference/parityos_addons.html
--rw-r--r--   0 root         (0) root         (0)    12710 2024-02-22 16:12:55.000000 parityos-2.4.0/parityos_addons/documentation/html/asynchronous_submission.html
--rw-r--r--   0 root         (0) root         (0)    38130 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/custom_device_models.html
--rw-r--r--   0 root         (0) root         (0)    31551 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/genindex.html
--rw-r--r--   0 root         (0) root         (0)     5742 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/index.html
--rw-r--r--   0 root         (0) root         (0)     8105 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/installation.html
--rw-r--r--   0 root         (0) root         (0)     2530 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/objects.inv
--rw-r--r--   0 root         (0) root         (0)    13212 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/parity_decoder.html
--rw-r--r--   0 root         (0) root         (0)     7610 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/py-modindex.html
--rw-r--r--   0 root         (0) root         (0)    30133 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/quickstart.html
--rw-r--r--   0 root         (0) root         (0)     4536 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/search.html
--rw-r--r--   0 root         (0) root         (0)    45769 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/searchindex.js
--rw-r--r--   0 root         (0) root         (0)    47140 2024-02-22 16:12:56.000000 parityos-2.4.0/parityos_addons/documentation/html/tutorial.html
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/documentation/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/parityos_addons/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 16:13:03.000000 parityos-2.4.0/parityos_addons/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/example1.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/example2.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/example3.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/example4.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/example5.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/examples/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/parityos_addons/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4643 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/interfaces/cirq_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)    16268 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/interfaces/openqasm_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     4602 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/interfaces/qiskit_exporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 16:13:13.873875 parityos-2.4.0/parityos_addons/qaoa/
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/qaoa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/qaoa/qaoa_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     4318 2024-02-22 15:13:41.000000 parityos-2.4.0/parityos_addons/spin_hamiltonians.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 16:13:13.873875 parityos-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-02-22 15:13:41.000000 parityos-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.052405 parityos-2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2024-04-29 11:56:24.000000 parityos-2.5.0/License.txt
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-29 13:19:40.052405 parityos-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2024-04-29 11:56:24.000000 parityos-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.004405 parityos-2.5.0/parityos/
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.008405 parityos-2.5.0/parityos/api_interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 13:19:31.000000 parityos-2.5.0/parityos/api_interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/api_interface/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3976 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/api_interface/compiler_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/api_interface/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/api_interface/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.012405 parityos-2.5.0/parityos/base/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8430 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23002 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/gates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/problem_representation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/qubits.py
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/base/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/compiler_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6990 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/device_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.012405 parityos-2.5.0/parityos/encodings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 13:19:31.000000 parityos-2.5.0/parityos/encodings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/encodings/mappings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12750 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/encodings/parity_decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/encodings/parity_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    11356 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos/encodings/parityos_output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.048406 parityos-2.5.0/parityos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-29 13:19:39.000000 parityos-2.5.0/parityos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-29 13:19:39.000000 parityos-2.5.0/parityos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 13:19:39.000000 parityos-2.5.0/parityos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-29 13:19:39.000000 parityos-2.5.0/parityos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-29 13:19:39.000000 parityos-2.5.0/parityos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.012405 parityos-2.5.0/parityos_addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.012405 parityos-2.5.0/parityos_addons/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 13:19:31.000000 parityos-2.5.0/parityos_addons/documentation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.020405 parityos-2.5.0/parityos_addons/documentation/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.020405 parityos-2.5.0/parityos_addons/documentation/html/_images/
+-rw-r--r--   0 root         (0) root         (0)   188899 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_images/hypergraph_solution_tutorial.png
+-rw-r--r--   0 root         (0) root         (0)   187919 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_images/hypergraph_tutorial.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.024405 parityos-2.5.0/parityos_addons/documentation/html/_sources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.024405 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/api_interface.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/base.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/encodings.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/index.rst.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/parityos.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/api_reference/parityos_addons.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/asynchronous_submission.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     8557 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/custom_device_models.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/index.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/installation.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     3486 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/parity_decoder.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     9548 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/quickstart.rst.txt
+-rw-r--r--   0 root         (0) root         (0)    17652 2024-04-29 11:56:11.000000 parityos-2.5.0/parityos_addons/documentation/html/_sources/tutorial.rst.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.028406 parityos-2.5.0/parityos_addons/documentation/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     4289 2024-04-29 13:19:16.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 root         (0) root         (0)    15094 2024-04-29 13:19:20.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/basic.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.028406 parityos-2.5.0/parityos_addons/documentation/html/_static/css/
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/badge_only.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.040405 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/
+-rw-r--r--   0 root         (0) root         (0)    87624 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 root         (0) root         (0)    67312 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 root         (0) root         (0)    86288 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 root         (0) root         (0)    66444 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 root         (0) root         (0)   165742 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)   323344 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 root         (0) root         (0)   193308 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 root         (0) root         (0)   309728 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 root         (0) root         (0)   184912 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 root         (0) root         (0)   328412 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 root         (0) root         (0)   195704 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 root         (0) root         (0)   309192 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 root         (0) root         (0)   182708 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 root         (0) root         (0)   135314 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      328 2024-04-29 13:19:20.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)    89501 2024-04-29 13:19:16.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/jquery.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.044406 parityos-2.5.0/parityos_addons/documentation/html/_static/js/
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/js/badge_only.js
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     5023 2024-04-10 20:11:44.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2024-04-29 13:19:20.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-29 13:19:20.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    20731 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     5123 2024-04-29 13:19:14.000000 parityos-2.5.0/parityos_addons/documentation/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.044406 parityos-2.5.0/parityos_addons/documentation/html/api_reference/
+-rw-r--r--   0 root         (0) root         (0)     5808 2024-04-29 13:19:20.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/api_interface.html
+-rw-r--r--   0 root         (0) root         (0)   174422 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/base.html
+-rw-r--r--   0 root         (0) root         (0)    44306 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/encodings.html
+-rw-r--r--   0 root         (0) root         (0)     6294 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/index.html
+-rw-r--r--   0 root         (0) root         (0)    88197 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/parityos.html
+-rw-r--r--   0 root         (0) root         (0)    35919 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/api_reference/parityos_addons.html
+-rw-r--r--   0 root         (0) root         (0)    12710 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/asynchronous_submission.html
+-rw-r--r--   0 root         (0) root         (0)    38130 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/custom_device_models.html
+-rw-r--r--   0 root         (0) root         (0)    34250 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/genindex.html
+-rw-r--r--   0 root         (0) root         (0)     5848 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/index.html
+-rw-r--r--   0 root         (0) root         (0)     8105 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/installation.html
+-rw-r--r--   0 root         (0) root         (0)     2629 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/objects.inv
+-rw-r--r--   0 root         (0) root         (0)    13212 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/parity_decoder.html
+-rw-r--r--   0 root         (0) root         (0)     7610 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/py-modindex.html
+-rw-r--r--   0 root         (0) root         (0)    30133 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/quickstart.html
+-rw-r--r--   0 root         (0) root         (0)     4536 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/search.html
+-rw-r--r--   0 root         (0) root         (0)    49622 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/searchindex.js
+-rw-r--r--   0 root         (0) root         (0)    47140 2024-04-29 13:19:21.000000 parityos-2.5.0/parityos_addons/documentation/html/tutorial.html
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/documentation/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.048406 parityos-2.5.0/parityos_addons/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 13:19:31.000000 parityos-2.5.0/parityos_addons/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/example1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/example2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/example3.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/example4.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/example5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/examples/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.048406 parityos-2.5.0/parityos_addons/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4945 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/interfaces/cirq_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    16500 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/interfaces/openqasm_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/interfaces/qiskit_exporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:19:40.048406 parityos-2.5.0/parityos_addons/qaoa/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/qaoa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/qaoa/qaoa_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     4318 2024-04-29 11:56:24.000000 parityos-2.5.0/parityos_addons/spin_hamiltonians.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 13:19:40.052405 parityos-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-04-29 11:59:31.000000 parityos-2.5.0/setup.py
```

### Comparing `parityos-2.4.0/License.txt` & `parityos-2.5.0/License.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/PKG-INFO` & `parityos-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: parityos
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python bindings to the ParityOS API
 Home-page: https://parityqc.com/
 Requires-Python: >=3.9
 License-File: License.txt
 Requires-Dist: requests
 Provides-Extra: cirq
 Requires-Dist: cirq-core; extra == "cirq"
 Provides-Extra: qiskit
-Requires-Dist: qiskit<1; extra == "qiskit"
+Requires-Dist: qiskit; extra == "qiskit"
 Provides-Extra: spinz
 Requires-Dist: sympy; extra == "spinz"
 Provides-Extra: all
-Requires-Dist: qiskit<1; extra == "all"
-Requires-Dist: cirq-core; extra == "all"
 Requires-Dist: sympy; extra == "all"
+Requires-Dist: cirq-core; extra == "all"
+Requires-Dist: qiskit; extra == "all"
```

### Comparing `parityos-2.4.0/README.md` & `parityos-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/api_interface/authentication.py` & `parityos-2.5.0/parityos/api_interface/authentication.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/api_interface/compiler_run.py` & `parityos-2.5.0/parityos/api_interface/compiler_run.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/api_interface/connection.py` & `parityos-2.5.0/parityos/api_interface/connection.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/api_interface/exceptions.py` & `parityos-2.5.0/parityos/api_interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/base/circuit.py` & `parityos-2.5.0/parityos/base/circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,19 @@
 
     def __mul__(self, other):
         return type(self)(list.__mul__(self, other))
 
     def __rmul__(self, other):
         return type(self)(list.__rmul__(self, other))
 
+    def __getitem__(self, key):
+        # Convert slices of circuits to again to Circuits
+        item = list.__getitem__(self, key)
+        return type(self)(item) if isinstance(key, slice) else item
+
 
 CircuitElement = Union[Gate, Circuit]
 HALF_PI = 0.5 * pi
 
 
 def convert_cnots_to_rzzs(circuit: Circuit) -> Circuit:
     """
@@ -194,15 +199,15 @@
     # Representing a Cnot as a ZZ interaction requires the injection of a moment before and two
     # moments after the original moment.
     for gate in circuit:
         if not isinstance(gate, CNOT):
             # Copy the other gates directly to the new moment.
             moment.append(gate)
         else:
-            control, target = gate.qubit_list
+            control, target = gate.make_args()
             # Add the necessary rotation before the ZZ interaction.
             before.append(Ry(target, -HALF_PI))
             # Replace the CNOT with a ZZ rotation.
             moment.append(Rzz(control, target, -HALF_PI))
             # Add the remaining rotations after the ZZ interaction.
             after1.append(Rx(target, HALF_PI))
             after2.append(Rz(control, HALF_PI))
```

### Comparing `parityos-2.4.0/parityos/base/constraints.py` & `parityos-2.5.0/parityos/base/constraints.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/base/gates.py` & `parityos-2.5.0/parityos/base/gates.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,65 +11,85 @@
 from abc import ABC
 from collections.abc import Mapping, Sequence
 from typing import Union
 
 from parityos.base.qubits import Qubit
 from parityos.base.utils import json_wrap, JSONType
 
-
 DEFAULT_PARAMETER_NAME = "parameter"
 
 
 class Gate(ABC):
     """
     Base class from which all gates inherit.
 
     The Gate subclasses are intended to store the information received from the compiler.
     They do not implement any methods to simulate the gates, nor do they contain any information
     on the (anti-) commutation relations between them or other mathematical properties.
     For those uses we recommend more elaborate frameworks like Qutip, Cirq or Qiskit.
     """
 
-    _gate_map = {}  # a Dict that maps gate names onto gate classes (used by from_json)
+    gate_map = {}  # a Dict that maps gate names onto gate classes (used by from_json)
     aliases = tuple()  # Alternative names for the class that could appear in JSON representations.
 
+    _gate_map = gate_map  # For backwards compatibility. Will be removed in a future release.
+
     def __init__(self, *qubit_args: Qubit):
         """
         Set up the list of qubits on which the gate acts.
         """
-        self.qubit_list = list(qubit_args)
+        self.target_qubits = tuple(qubit_args)
 
     def __init_subclass__(cls):
         """
         Update the gate map when a new subclass is defined.
         This is used by the `from_json` method to map the JSON data on the correct gate class.
         """
         super().__init_subclass__()
-        Gate._gate_map[cls.__name__] = cls
-        Gate._gate_map.update({alias: cls for alias in cls.aliases})
+        Gate.gate_map[cls.__name__] = cls
+        Gate.gate_map.update({alias: cls for alias in cls.aliases})
+
+    @property
+    def qubit_list(self) -> list[Qubit]:
+        return list(self.target_qubits)
 
     @property
     def qubits(self) -> set[Qubit]:
         """
         :return: the set of qubits on which the gate acts (including possible control qubits).
         """
         return set(self.qubit_list)
 
+    @property
+    def n_qubits(self):
+        return len(self.qubit_list)
+
     def get_hermitian_conjugate(self) -> "Self":
         """
         :return: the Hermitian conjugate of the gate
         """
         raise NotImplementedError(f"hermitian_conjugate for {type(self)} is not implemented.")
 
     def make_args(self) -> tuple[Qubit]:
         """
         :return: the sequence of arguments that would be needed to instantiate a copy of self
             (does not include keyword only arguments).
         """
-        return tuple(self.qubit_list)
+        return self.target_qubits
+
+    @staticmethod
+    def make_args_and_kwargs_from_json(data: Sequence[JSONType]) -> tuple[list, dict]:
+        """
+        :return: the sequence of arguments keyword arguments derived from the given json data
+                 that would be needed to create an instance of the class.
+        """
+        class_name, *gate_data = data
+        init_args = [Qubit(label) for label in gate_data]
+        init_kwargs = {}
+        return init_args, init_kwargs
 
     def to_json(self) -> list[JSONType]:
         """
         :return: a json compatible object with all the information about the gate.
         """
         return json_wrap([type(self).__name__, *self.make_args()])
 
@@ -78,25 +98,25 @@
         """
         Creates a gate from a json compatible object.
 
         :param data: gate parameters in json compatible format
         :return: a Gate instance
         """
         # This method redirects the Gate.from_json method to the cls.from_json method,
-        # where cls is taken from Gate._gate_map based on the first value in the data.
+        # where cls is taken from Gate.gate_map based on the first value in the data.
         gate_class_name, *gate_data = data
-        gate_class = cls._gate_map[gate_class_name]
+        gate_class = cls.gate_map[gate_class_name]
         if cls is Gate:
             # For the abstract class, we delegate to the concrete class.
             return gate_class.from_json(data)
         elif cls is gate_class:
             # Here we define the standard behavior for concrete subclasses.
             # Subclasses can overwrite this if they need more elaborate gate data processing.
-            qubit_args = (Qubit(label) for label in gate_data)
-            return cls(*qubit_args)
+            init_args, init_kwargs = cls.make_args_and_kwargs_from_json(data)
+            return cls(*init_args, **init_kwargs)
         else:
             raise ValueError(f"Incorrect gate class for {gate_class_name} gate")
 
     def remap(self, *args, **kwargs) -> "Self":
         """
         The `RMixin.remap` method is used to remap the parameter name of parametrized gates to new
         values. For other gates (the subject of this version), a simple copy of the gate is
@@ -117,15 +137,15 @@
         return type(self)(*self.make_args())
 
     def __repr__(self):
         arguments = ", ".join(repr(arg) for arg in self.make_args())
         return f"{type(self).__name__}({arguments})"
 
     def __eq__(self, other):
-        return (type(self) == type(other)) and (self.make_args() == other.make_args())
+        return (type(self) is type(other)) and (self.make_args() == other.make_args())
 
     def __hash__(self):
         return hash((type(self), self.make_args()))
 
 
 class Gate1(Gate):
     """
@@ -136,21 +156,21 @@
         """
         :param Qubit qubit: qubit on which the gate acts.
         """
         # We implement __init__ to enforce a single qubit argument
         super().__init__(qubit)
 
     @property
-    def qubit(self) -> Qubit:
+    def target_qubit(self) -> Qubit:
         """
         Return the qubit on which this gate acts.
 
         :returns: The qubit on which the gate acts.
         """
-        return self.qubit_list[0]
+        return self.target_qubits[0]
 
 
 class Gate2(Gate):
     """
     A Gate that acts on two qubits.
     """
 
@@ -184,14 +204,111 @@
         """
         :param Qubit qubit1, qubit2, qubit3, qubit4: qubits on which the gate acts.
         """
         # We implement __init__ to enforce exactly four qubit arguments
         super().__init__(qubit1, qubit2, qubit3, qubit4)
 
 
+class CMixin(ABC):
+    """
+    Adds a single control qubit to a gate. This mixin must come before the gate parent class in the
+    new class definition.
+
+    Example:
+        class CNOT(CMixin, X):  # Creates a class that stores information for a CNOT gate.
+
+    Attributes:
+        control_qubits: The tuple of control qubits that can block the operation of the underlying
+                        gate.
+    """
+
+    def __init__(self, control: Qubit, target: Qubit, *args, **kwargs):
+        """
+        :param Qubit control: The qubit that controls whether the gate will act
+            (if Z_control == -1) or not (if Z_control == 1).
+        :param Qubit target: The target qubit on which the controlled operation will act.
+                             If the controlled operation acts on more qubits, then these
+                             can be provided as additional arguments.
+        """
+        super().__init__(target, *args, **kwargs)
+        self.control_qubits = (control,)
+
+    def make_args(self) -> tuple:
+        return *self.control_qubits, *super().make_args()
+
+    @property
+    def qubit_list(self) -> list[Qubit]:
+        return [*self.control_qubits, *self.target_qubits]
+
+
+class CCMixin(CMixin, ABC):
+    """
+    Adds two control qubits to a gate. This mixin must come before the gate parent class in the
+    new class definition.
+
+    Example:
+        class CCNOT(CCMixin, X):  # Creates a class that stores information for a CCNOT gate.
+
+    Attributes:
+        control_qubits: The tuple of control qubits that can block the operation of the underlying
+                        gate.
+    """
+
+    def __init__(self, control1: Qubit, control2: Qubit, target: Qubit, *args, **kwargs):
+        """
+        :param Qubit control1:
+        :param Qubit control2: The qubits that control whether the gate will act
+            (if Z_control1 == Z_control2 == -1) or not (any other Z_control values).
+        :param Qubit target: The target qubit on which the controlled operation will act.
+                             If the controlled operation acts on more qubits, then these
+                             can be provided as additional arguments.
+        """
+        # We have to call super().__init__ with the correct arguments to make sure that
+        # the __init__ methods on all parent classes are consumed in the right order.
+        # We skip CMixin.__init__ because that would set the wrong control_qubits attribute.
+        super(CMixin, self).__init__(target, *args, **kwargs)
+        self.control_qubits = (control1, control2)
+
+
+class MultiControlMixin(ABC):
+    """
+    Adds an arbitrary control sequence to a gate. This mixin must come before the gate parent
+    class in the new class definition.
+
+    Example:
+        class MultiControlledH(MultiControlMixin, H):  # Creates a class that stores information for
+        a multi-controlled Hadamard gate.
+    """
+
+    def __init__(self, control_qubits: Sequence[Qubit], target: Qubit, *args, **kwargs):
+        """
+        :param control_qubits: A sequence of control qubits that can block the operation of the
+                               underlying gate.
+        :param target: The qubit on which the underlying gate should act. If more qubits are
+                       targeted, then they can be added as additional arguments.
+        """
+        super().__init__(target, *args, **kwargs)
+        self.control_qubits = tuple(control_qubits)
+
+    @property
+    def qubit_list(self) -> list[Qubit]:
+        return [*self.control_qubits, *self.target_qubits]
+
+    def make_args(self) -> tuple:
+        return self.control_qubits, *super().make_args()
+
+    @classmethod  # Can not be a staticmethod because of `super`.
+    def make_args_and_kwargs_from_json(cls, data: Sequence[JSONType]) -> tuple[list, dict]:
+        class_name, control_qubits_data, *target_data = data
+        control_qubits = [Qubit(label) for label in control_qubits_data]
+        super_data = [class_name, *target_data]
+        target_args, target_kwargs = super().make_args_and_kwargs_from_json(super_data)
+        return [control_qubits, *target_args], target_kwargs
+
+
 class HermitianGateMixin(Gate, ABC):
     """
     A mixin that implements hermitian_conjugate method for Hermitian gates.
     """
 
     def get_hermitian_conjugate(self) -> "Self":
         """
@@ -250,16 +367,16 @@
         """
         return {self.parameter_name} if self.parameter_name else set()
 
     def get_hermitian_conjugate(self) -> "Self":
         """
         :return: the Hermitian conjugate of the gate
         """
-        cls = type(self)
-        return cls(*self.qubit_list, -self.angle, parameter_name=self.parameter_name)
+        *init_args, angle = self.make_args()
+        return  type(self)(*init_args, -angle, parameter_name=self.parameter_name)
 
     def remap(self, context: Mapping = None, **kwargs) -> Gate:
         """
         Creates a copy of the gate with an updated parameter or parameter name.
 
         Updates for the parameter should be provided either as a context mapping or as a keyword
         argument. If a keyword argument is given, its key must match the parameter_name defined
@@ -373,26 +490,27 @@
         elif self.parameter_name == self._DEFAULT_PARAMETER_NAME:
             return json_wrap([type(self).__name__ + self._PARAMETRIZED, *args])
         else:
             # For gates with a non-standard parameter value we should include the parameter.
             return json_wrap([type(self).__name__, *args, self.parameter_name])
 
     @classmethod
-    def from_json(cls, data: Sequence[JSONType]) -> "Self":
+    def make_args_and_kwargs_from_json(cls, data: Sequence[JSONType]) -> tuple[list, dict]:
         class_name, *gate_data = data
         if isinstance(gate_data[-1], str):
-            *gate_data, parameter_name = gate_data
+            *data, parameter_name = data
         elif class_name.endswith(cls._PARAMETRIZED):
             parameter_name = cls._DEFAULT_PARAMETER_NAME
         else:
             parameter_name = None
 
-        *qubit_data, angle = gate_data
-        qubit_args = (Qubit(label) for label in qubit_data)
-        return cls(*qubit_args, angle, parameter_name=parameter_name)
+        *super_data, angle = data
+        init_args, init_kwargs = super().make_args_and_kwargs_from_json(super_data)
+        init_kwargs.update(angle=angle, parameter_name=parameter_name)
+        return init_args, init_kwargs
 
     def __repr__(self):
         arguments = ", ".join(repr(arg) for arg in self.make_args())
         if self.parameter_name is not None:
             arguments += f", parameter_name='{self.parameter_name}'"
 
         return f"{type(self).__name__}({arguments})"
@@ -422,64 +540,93 @@
     """Represents a Z gate"""
 
 
 class H(HermitianGateMixin, Gate1):
     """Represents a Hadamard gate"""
 
 
-class CNOT(HermitianGateMixin, Gate2):
+class Swap(Gate2):
+    """Represents a Swap gate"""
+
+
+class ISwap(Gate2):
+    """Represents an iSwap gate"""
+
+
+class CH(CMixin, H):
+    """Represents a CH gate"""
+
+
+class CNOT(CMixin, X):
     """Represents a CNOT gate"""
 
     aliases = ("CX",)
 
-    def __init__(self, control: Qubit, target: Qubit):
-        """
-        :param Qubit control: The qubit that controls whether the gate will act
-               (if Z_control == -1) or not (if Z_control == 1).
-        :param Qubit target: The qubit that will be flipped if Z_control == -1.
-        """
-        super().__init__(control, target)
 
+class CY(CMixin, Y):
+    """Represents a CY gate"""
 
-class CZ(HermitianGateMixin, Gate2):
-    """Represents a CZ gate"""
 
-    def __init__(self, control: Qubit, target: Qubit):
-        """
-        :param Qubit control: The qubit that controls whether the gate will act
-               (if Z_control == -1) or not (if Z_control == 1).
-        :param Qubit target: The qubit phase that will be flipped if Z_control == -1.
-        """
-        super().__init__(control, target)
+class CZ(CMixin, Z):
+    """Represents a CZ gate"""
 
 
 class Rx(RMixin, Gate1):
     """Represents an RX gate"""
 
 
 class Ry(RMixin, Gate1):
     """Represents an RY gate"""
 
 
 class Rz(RMixin, Gate1):
     """Represents an RZ gate"""
 
 
+class Rxx(RMixin, Gate2):
+    """Represents an RXX gate"""
+
+
+class Ryy(RMixin, Gate2):
+    """Represents an RYY gate"""
+
+
 class Rzz(RMixin, Gate2):
     """Represents an RZZ gate"""
 
 
-class CCNOT(HermitianGateMixin, Gate3):
+class Rzzzz(RMixin, Gate4):
+    """Represents an RZZZZ gate"""
+
+
+class CRx(CMixin, Rx):
+    """Represents a controlled Rx gate"""
+
+
+class CRy(CMixin, Ry):
+    """Represents a controlled Ry gate"""
+
+
+class CRz(CMixin, Rz):
+    """Represents a controlled Rz gate"""
+
+
+class CCNOT(CCMixin, X):
     """Represents a CCNOT gate"""
 
     aliases = ("CCX",)
 
-    def __init__(self, control_1: Qubit, control_2: Qubit, target: Qubit):
-        """
-        :param Qubit control_1: The first qubit that controls whether the gate will act
-               (if Z_control_1 == -1) or not (if Z_control_1 == 1).
-        :param Qubit control_2: The second qubit that controls whether the gate will act
-               (if Z_control_2 == -1) or not (if Z_control_2 == 1).
-        :param Qubit target: The qubit that will be flipped if Z_control_1 and Z_control_2 are
-                             equal to -1.
-        """
-        super().__init__(control_1, control_2, target)
+
+class MultiControlledRx(MultiControlMixin, Rx):
+    """Represents a controlled Rx gate with arbitrary control sequence"""
+
+
+class MultiControlledRy(MultiControlMixin, Ry):
+    """Represents a controlled Ry gate with arbitrary control sequence"""
+
+
+class MultiControlledRz(MultiControlMixin, Rz):
+    """Represents a controlled Rz gate with arbitrary control sequence"""
+
+
+class MultiControlledH(MultiControlMixin, H):
+    """Represents a controlled Hadamard gate with arbitrary control sequence"""
```

### Comparing `parityos-2.4.0/parityos/base/problem_representation.py` & `parityos-2.5.0/parityos/base/problem_representation.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/base/utils.py` & `parityos-2.5.0/parityos/base/utils.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/compiler_client.py` & `parityos-2.5.0/parityos/compiler_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             ``analog_default`` and ``digital_default`` are available for everyone;
             other allowed presets are communicated on a per-customer basis.
             Optional. If no value is provided, ``device_model.preset`` is used instead.
         :param timeout: time in seconds after which this function is aborted.
         :return: ParityOSOutput object containing all information about the compiled problem
         """
         submission_id = self.submit(optimization_problem, device_model, preset=preset, **kwargs)
+        print(f"Compiling submission {submission_id}")
 
         compiler_runs = []
         stop_time = time.time() + timeout
         while time.time() <= stop_time:
             # Wait for two seconds before contacting the server again.
             time.sleep(TIME_BETWEEN_TRIALS)
             compiler_runs = self.get_compiler_runs(submission_id)
```

### Comparing `parityos-2.4.0/parityos/device_model.py` & `parityos-2.5.0/parityos/device_model.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/encodings/mappings.py` & `parityos-2.5.0/parityos/encodings/mappings.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/encodings/parity_decoder.py` & `parityos-2.5.0/parityos/encodings/parity_decoder.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/encodings/parity_encoder.py` & `parityos-2.5.0/parityos/encodings/parity_encoder.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos/encodings/parityos_output.py` & `parityos-2.5.0/parityos/encodings/parityos_output.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos.egg-info/PKG-INFO` & `parityos-2.5.0/parityos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: parityos
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python bindings to the ParityOS API
 Home-page: https://parityqc.com/
 Requires-Python: >=3.9
 License-File: License.txt
 Requires-Dist: requests
 Provides-Extra: cirq
 Requires-Dist: cirq-core; extra == "cirq"
 Provides-Extra: qiskit
-Requires-Dist: qiskit<1; extra == "qiskit"
+Requires-Dist: qiskit; extra == "qiskit"
 Provides-Extra: spinz
 Requires-Dist: sympy; extra == "spinz"
 Provides-Extra: all
-Requires-Dist: qiskit<1; extra == "all"
-Requires-Dist: cirq-core; extra == "all"
 Requires-Dist: sympy; extra == "all"
+Requires-Dist: cirq-core; extra == "all"
+Requires-Dist: qiskit; extra == "all"
```

### Comparing `parityos-2.4.0/parityos.egg-info/SOURCES.txt` & `parityos-2.5.0/parityos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_images/hypergraph_solution_tutorial.png` & `parityos-2.5.0/parityos_addons/documentation/html/_images/hypergraph_solution_tutorial.png`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_images/hypergraph_tutorial.png` & `parityos-2.5.0/parityos_addons/documentation/html/_images/hypergraph_tutorial.png`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/asynchronous_submission.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/asynchronous_submission.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/custom_device_models.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/custom_device_models.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/installation.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/parity_decoder.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/parity_decoder.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/quickstart.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_sources/tutorial.rst.txt` & `parityos-2.5.0/parityos_addons/documentation/html/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/_sphinx_javascript_frameworks_compat.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/basic.css` & `parityos-2.5.0/parityos_addons/documentation/html/_static/basic.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/badge_only.css` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.eot` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.svg` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.ttf` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff2` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/css/theme.css` & `parityos-2.5.0/parityos_addons/documentation/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/doctools.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/doctools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * doctools.js
  * ~~~~~~~~~~~
  *
  * Base JavaScript utilities for all Sphinx HTML documentation.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 const BLACKLISTED_KEY_CONTROL_ELEMENTS = new Set([
     "TEXTAREA",
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/jquery.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/js/badge_only.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/js/html5shiv-printshiv.min.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/js/html5shiv.min.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/js/theme.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/language_data.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/language_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
 
 
-/* Non-minified version is copied as a separate JS file, is available */
+/* Non-minified version is copied as a separate JS file, if available */
 
 /**
  * Porter Stemmer
  */
 var Stemmer = function() {
 
     var step2list = {
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/pygments.css` & `parityos-2.5.0/parityos_addons/documentation/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/searchtools.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/searchtools.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -94,15 +94,15 @@
             highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
     } else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms)
+                    Search.makeSearchSummary(data, searchTerms, anchor)
                 );
             // highlight search terms in the summary
             if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
                 highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
         });
     Search.output.appendChild(listItem);
 };
@@ -111,16 +111,16 @@
     Search.title.innerText = _("Search Results");
     if (!resultCount)
         Search.status.innerText = Documentation.gettext(
             "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
         );
     else
         Search.status.innerText = _(
-            `Search finished, found ${resultCount} page(s) matching the search query.`
-        );
+            "Search finished, found ${resultCount} page(s) matching the search query."
+        ).replace('${resultCount}', resultCount);
 };
 const _displayNextItem = (
     results,
     resultCount,
     searchTerms,
     highlightTerms,
 ) => {
@@ -132,14 +132,30 @@
             () => _displayNextItem(results, resultCount, searchTerms, highlightTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
+// Helper function used by query() to order search results.
+// Each input is an array of [docname, title, anchor, descr, score, filename].
+// Order the results by score (in opposite order of appearance, since the
+// `_displayNextItem` function uses pop() to retrieve items) and then alphabetically.
+const _orderResultsByScoreThenName = (a, b) => {
+    const leftScore = a[4];
+    const rightScore = b[4];
+    if (leftScore === rightScore) {
+        // same score: sort alphabetically
+        const leftTitle = a[1].toLowerCase();
+        const rightTitle = b[1].toLowerCase();
+        if (leftTitle === rightTitle) return 0;
+        return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
+    }
+    return leftScore > rightScore ? 1 : -1;
+};
 
 /**
  * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
  * custom function per language.
  *
  * The regular expression works by splitting the string on consecutive characters
  * that are not Unicode letters, numbers, underscores, or emoji characters.
@@ -155,23 +171,36 @@
  * Search Module
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: (htmlString) => {
+    htmlToText: (htmlString, anchor) => {
         const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
-        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
-            el.remove()
-        });
+        for (const removalQuery of [".headerlinks", "script", "style"]) {
+            htmlElement.querySelectorAll(removalQuery).forEach((el) => {
+                el.remove()
+            });
+        }
+        if (anchor) {
+            const anchorContent = htmlElement.querySelector(`[role="main"] ${anchor}`);
+            if (anchorContent) return anchorContent.textContent;
+
+            console.warn(
+                `Anchored content block not found. Sphinx search tries to obtain it via DOM query '[role=main] ${anchor}'. Check your theme or template.`
+            );
+        }
+
+        // if anchor not specified or not found, fall back to main content
         const docContent = htmlElement.querySelector('[role="main"]');
-        if (docContent !== undefined) return docContent.textContent;
+        if (docContent) return docContent.textContent;
+
         console.warn(
-            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+            "Content block not found. Sphinx search tries to obtain it via DOM query '[role=main]'. Check your theme or template."
         );
         return "";
     },
 
     init: () => {
         const query = new URLSearchParams(window.location.search).get("q");
         document
@@ -236,24 +265,15 @@
         Search.startPulse();
 
         // index already loaded, the browser was quick!
         if (Search.hasIndex()) Search.query(query);
         else Search.deferQuery(query);
     },
 
-    /**
-     * execute search (requires search index to be loaded)
-     */
-    query: (query) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-        const allTitles = Search._index.alltitles;
-        const indexEntries = Search._index.indexentries;
-
+    _parseQuery: (query) => {
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -281,92 +301,114 @@
             localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
         }
 
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
-        // array of [docname, title, anchor, descr, score, filename]
-        let results = [];
+        return [query, searchTerms, excludedTerms, highlightTerms, objectTerms];
+    },
+
+    /**
+     * execute search (requires search index to be loaded)
+     */
+    _performSearch: (query, searchTerms, excludedTerms, highlightTerms, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // Collect multiple result groups to be sorted separately and then ordered.
+        // Each is an array of [docname, title, anchor, descr, score, filename].
+        const normalResults = [];
+        const nonMainIndexResults = [];
+
         _removeChildren(document.getElementById("search-progress"));
 
-        const queryLower = query.toLowerCase();
+        const queryLower = query.toLowerCase().trim();
         for (const [title, foundTitles] of Object.entries(allTitles)) {
-            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+            if (title.toLowerCase().trim().includes(queryLower) && (queryLower.length >= title.length / 2)) {
                 for (const [file, id] of foundTitles) {
                     let score = Math.round(100 * queryLower.length / title.length)
-                    results.push([
+                    normalResults.push([
                         docNames[file],
                         titles[file] !== title ? `${titles[file]} > ${title}` : title,
                         id !== null ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
                     ]);
                 }
             }
         }
 
         // search for explicit entries in index directives
         for (const [entry, foundEntries] of Object.entries(indexEntries)) {
             if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
-                for (const [file, id] of foundEntries) {
-                    let score = Math.round(100 * queryLower.length / entry.length)
-                    results.push([
+                for (const [file, id, isMain] of foundEntries) {
+                    const score = Math.round(100 * queryLower.length / entry.length);
+                    const result = [
                         docNames[file],
                         titles[file],
                         id ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
-                    ]);
+                    ];
+                    if (isMain) {
+                        normalResults.push(result);
+                    } else {
+                        nonMainIndexResults.push(result);
+                    }
                 }
             }
         }
 
         // lookup as object
         objectTerms.forEach((term) =>
-            results.push(...Search.performObjectSearch(term, objectTerms))
+            normalResults.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
-        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
+        normalResults.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
+        if (Scorer.score) {
+            normalResults.forEach((item) => (item[4] = Scorer.score(item)));
+            nonMainIndexResults.forEach((item) => (item[4] = Scorer.score(item)));
+        }
 
-        // now sort the results by score (in opposite order of appearance, since the
-        // display function below uses pop() to retrieve items) and then
-        // alphabetically
-        results.sort((a, b) => {
-            const leftScore = a[4];
-            const rightScore = b[4];
-            if (leftScore === rightScore) {
-                // same score: sort alphabetically
-                const leftTitle = a[1].toLowerCase();
-                const rightTitle = b[1].toLowerCase();
-                if (leftTitle === rightTitle) return 0;
-                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
-            }
-            return leftScore > rightScore ? 1 : -1;
-        });
+        // Sort each group of results by score and then alphabetically by name.
+        normalResults.sort(_orderResultsByScoreThenName);
+        nonMainIndexResults.sort(_orderResultsByScoreThenName);
+
+        // Combine the result groups in (reverse) order.
+        // Non-main index entries are typically arbitrary cross-references,
+        // so display them after other results.
+        let results = [...nonMainIndexResults, ...normalResults];
 
         // remove duplicate search results
         // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
         let seen = new Set();
         results = results.reverse().reduce((acc, result) => {
             let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
             if (!seen.has(resultStr)) {
                 acc.push(result);
                 seen.add(resultStr);
             }
             return acc;
         }, []);
 
-        results = results.reverse();
+        return results.reverse();
+    },
+
+    query: (query) => {
+        const [searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms] = Search._parseQuery(query);
+        const results = Search._performSearch(searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms);
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
         _displayNextItem(results, results.length, searchTerms, highlightTerms);
@@ -466,28 +508,32 @@
             }, {
                 files: titleTerms[word],
                 score: Scorer.title
             }, ];
             // add support for partial matches
             if (word.length > 2) {
                 const escapedWord = _escapeRegExp(word);
-                Object.keys(terms).forEach((term) => {
-                    if (term.match(escapedWord) && !terms[word])
-                        arr.push({
-                            files: terms[term],
-                            score: Scorer.partialTerm
-                        });
-                });
-                Object.keys(titleTerms).forEach((term) => {
-                    if (term.match(escapedWord) && !titleTerms[word])
-                        arr.push({
-                            files: titleTerms[word],
-                            score: Scorer.partialTitle
-                        });
-                });
+                if (!terms.hasOwnProperty(word)) {
+                    Object.keys(terms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: terms[term],
+                                score: Scorer.partialTerm
+                            });
+                    });
+                }
+                if (!titleTerms.hasOwnProperty(word)) {
+                    Object.keys(titleTerms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: titleTerms[term],
+                                score: Scorer.partialTitle
+                            });
+                    });
+                }
             }
 
             // no match but word was a required one
             if (arr.every((record) => record.files === undefined)) return;
 
             // found search word in contents
             arr.forEach((record) => {
@@ -502,17 +548,16 @@
                     if (!scoreMap.has(file)) scoreMap.set(file, {});
                     scoreMap.get(file)[word] = record.score;
                 });
             });
 
             // create the mapping
             files.forEach((file) => {
-                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
-                    fileMap.get(file).push(word);
-                else fileMap.set(file, [word]);
+                if (!fileMap.has(file)) fileMap.set(file, [word]);
+                else if (fileMap.get(file).indexOf(word) === -1) fileMap.get(file).push(word);
             });
         });
 
         // now check if the files don't contain excluded terms
         const results = [];
         for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
@@ -555,16 +600,16 @@
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
      * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords) => {
-        const text = Search.htmlToText(htmlText);
+    makeSearchSummary: (htmlText, keywords, anchor) => {
+        const text = Search.htmlToText(htmlText, anchor);
         if (text === "") return null;
 
         const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
             .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/_static/sphinx_highlight.js` & `parityos-2.5.0/parityos_addons/documentation/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/api_interface.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/api_interface.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="parityos.encodings" href="encodings.html" />
     <link rel="prev" title="parityos.base" href="base.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/base.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
         <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="parityos.api_interface" href="api_interface.html" />
     <link rel="prev" title="parityos" href="parityos.html" /> 
@@ -76,40 +76,45 @@
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.circuit.Circuit.parameters"><code class="docutils literal notranslate"><span class="pre">Circuit.parameters</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.circuit.Circuit.qubits"><code class="docutils literal notranslate"><span class="pre">Circuit.qubits</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.circuit.Circuit.remap"><code class="docutils literal notranslate"><span class="pre">Circuit.remap()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.circuit.Circuit.to_json"><code class="docutils literal notranslate"><span class="pre">Circuit.to_json()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.circuit.convert_cnots_to_rzzs"><code class="docutils literal notranslate"><span class="pre">convert_cnots_to_rzzs()</span></code></a></li>
-<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CCNOT"><code class="docutils literal notranslate"><span class="pre">CCNOT</span></code></a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.CCNOT.__init__"><code class="docutils literal notranslate"><span class="pre">CCNOT.__init__()</span></code></a></li>
-</ul>
-</li>
-<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CNOT"><code class="docutils literal notranslate"><span class="pre">CNOT</span></code></a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.CNOT.__init__"><code class="docutils literal notranslate"><span class="pre">CNOT.__init__()</span></code></a></li>
-</ul>
-</li>
-<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CZ"><code class="docutils literal notranslate"><span class="pre">CZ</span></code></a><ul>
-<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.CZ.__init__"><code class="docutils literal notranslate"><span class="pre">CZ.__init__()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CCMixin"><code class="docutils literal notranslate"><span class="pre">CCMixin</span></code></a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.CCMixin.__init__"><code class="docutils literal notranslate"><span class="pre">CCMixin.__init__()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CCNOT"><code class="docutils literal notranslate"><span class="pre">CCNOT</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CH"><code class="docutils literal notranslate"><span class="pre">CH</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CMixin"><code class="docutils literal notranslate"><span class="pre">CMixin</span></code></a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.CMixin.__init__"><code class="docutils literal notranslate"><span class="pre">CMixin.__init__()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CNOT"><code class="docutils literal notranslate"><span class="pre">CNOT</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CRx"><code class="docutils literal notranslate"><span class="pre">CRx</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CRy"><code class="docutils literal notranslate"><span class="pre">CRy</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CRz"><code class="docutils literal notranslate"><span class="pre">CRz</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CY"><code class="docutils literal notranslate"><span class="pre">CY</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.CZ"><code class="docutils literal notranslate"><span class="pre">CZ</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Gate"><code class="docutils literal notranslate"><span class="pre">Gate</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.__init__"><code class="docutils literal notranslate"><span class="pre">Gate.__init__()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.from_json"><code class="docutils literal notranslate"><span class="pre">Gate.from_json()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.get_hermitian_conjugate"><code class="docutils literal notranslate"><span class="pre">Gate.get_hermitian_conjugate()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.make_args"><code class="docutils literal notranslate"><span class="pre">Gate.make_args()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.make_args_and_kwargs_from_json"><code class="docutils literal notranslate"><span class="pre">Gate.make_args_and_kwargs_from_json()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.modify_angle"><code class="docutils literal notranslate"><span class="pre">Gate.modify_angle()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.qubits"><code class="docutils literal notranslate"><span class="pre">Gate.qubits</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.remap"><code class="docutils literal notranslate"><span class="pre">Gate.remap()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate.to_json"><code class="docutils literal notranslate"><span class="pre">Gate.to_json()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Gate1"><code class="docutils literal notranslate"><span class="pre">Gate1</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate1.__init__"><code class="docutils literal notranslate"><span class="pre">Gate1.__init__()</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate1.qubit"><code class="docutils literal notranslate"><span class="pre">Gate1.qubit</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate1.target_qubit"><code class="docutils literal notranslate"><span class="pre">Gate1.target_qubit</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Gate2"><code class="docutils literal notranslate"><span class="pre">Gate2</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.Gate2.__init__"><code class="docutils literal notranslate"><span class="pre">Gate2.__init__()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Gate3"><code class="docutils literal notranslate"><span class="pre">Gate3</span></code></a><ul>
@@ -121,29 +126,42 @@
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.H"><code class="docutils literal notranslate"><span class="pre">H</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.HermitianGateMixin"><code class="docutils literal notranslate"><span class="pre">HermitianGateMixin</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.HermitianGateMixin.get_hermitian_conjugate"><code class="docutils literal notranslate"><span class="pre">HermitianGateMixin.get_hermitian_conjugate()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.ISwap"><code class="docutils literal notranslate"><span class="pre">ISwap</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.MultiControlMixin"><code class="docutils literal notranslate"><span class="pre">MultiControlMixin</span></code></a><ul>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.MultiControlMixin.__init__"><code class="docutils literal notranslate"><span class="pre">MultiControlMixin.__init__()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.MultiControlledH"><code class="docutils literal notranslate"><span class="pre">MultiControlledH</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.MultiControlledRx"><code class="docutils literal notranslate"><span class="pre">MultiControlledRx</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.MultiControlledRy"><code class="docutils literal notranslate"><span class="pre">MultiControlledRy</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.MultiControlledRz"><code class="docutils literal notranslate"><span class="pre">MultiControlledRz</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.RMixin"><code class="docutils literal notranslate"><span class="pre">RMixin</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.__init__"><code class="docutils literal notranslate"><span class="pre">RMixin.__init__()</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.from_json"><code class="docutils literal notranslate"><span class="pre">RMixin.from_json()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.get_hermitian_conjugate"><code class="docutils literal notranslate"><span class="pre">RMixin.get_hermitian_conjugate()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.make_args"><code class="docutils literal notranslate"><span class="pre">RMixin.make_args()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.make_args_and_kwargs_from_json"><code class="docutils literal notranslate"><span class="pre">RMixin.make_args_and_kwargs_from_json()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.modify_angle"><code class="docutils literal notranslate"><span class="pre">RMixin.modify_angle()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.parameters"><code class="docutils literal notranslate"><span class="pre">RMixin.parameters</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.remap"><code class="docutils literal notranslate"><span class="pre">RMixin.remap()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.gates.RMixin.to_json"><code class="docutils literal notranslate"><span class="pre">RMixin.to_json()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Rx"><code class="docutils literal notranslate"><span class="pre">Rx</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Rxx"><code class="docutils literal notranslate"><span class="pre">Rxx</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Ry"><code class="docutils literal notranslate"><span class="pre">Ry</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Ryy"><code class="docutils literal notranslate"><span class="pre">Ryy</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Rz"><code class="docutils literal notranslate"><span class="pre">Rz</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Rzz"><code class="docutils literal notranslate"><span class="pre">Rzz</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Rzzzz"><code class="docutils literal notranslate"><span class="pre">Rzzzz</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Swap"><code class="docutils literal notranslate"><span class="pre">Swap</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.X"><code class="docutils literal notranslate"><span class="pre">X</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Y"><code class="docutils literal notranslate"><span class="pre">Y</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.gates.Z"><code class="docutils literal notranslate"><span class="pre">Z</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos.base.utils.JSONLoadSaveMixin"><code class="docutils literal notranslate"><span class="pre">JSONLoadSaveMixin</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.utils.JSONLoadSaveMixin.from_json"><code class="docutils literal notranslate"><span class="pre">JSONLoadSaveMixin.from_json()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.utils.JSONLoadSaveMixin.load"><code class="docutils literal notranslate"><span class="pre">JSONLoadSaveMixin.load()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos.base.utils.JSONLoadSaveMixin.save"><code class="docutils literal notranslate"><span class="pre">JSONLoadSaveMixin.save()</span></code></a></li>
@@ -432,77 +450,127 @@
 <dt class="field-odd">Return type<span class="colon">:</span></dt>
 <dd class="field-odd"><p><a class="reference internal" href="#parityos.base.circuit.Circuit" title="parityos.base.circuit.Circuit">Circuit</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py class" id="module-parityos.base.gates">
-<dt class="sig sig-object py" id="parityos.base.gates.CCNOT">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CCNOT</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">control_2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CCNOT" title="Link to this definition"></a></dt>
-<dd><p>Represents a CCNOT gate</p>
+<dt class="sig sig-object py" id="parityos.base.gates.CCMixin">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CCMixin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">control2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CCMixin" title="Link to this definition"></a></dt>
+<dd><p>Adds two control qubits to a gate. This mixin must come before the gate parent class in the
+new class definition.</p>
+<dl class="simple">
+<dt>Example:</dt><dd><p>class CCNOT(CCMixin, X):  # Creates a class that stores information for a CCNOT gate.</p>
+</dd>
+<dt>Attributes:</dt><dd><dl class="simple">
+<dt>control_qubits: The tuple of control qubits that can block the operation of the underlying</dt><dd><p>gate.</p>
+</dd>
+</dl>
+</dd>
+</dl>
 <dl class="py method">
-<dt class="sig sig-object py" id="parityos.base.gates.CCNOT.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">control_2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CCNOT.__init__" title="Link to this definition"></a></dt>
+<dt class="sig sig-object py" id="parityos.base.gates.CCMixin.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">control2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CCMixin.__init__" title="Link to this definition"></a></dt>
 <dd><dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>control_1</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The first qubit that controls whether the gate will act
-(if Z_control_1 == -1) or not (if Z_control_1 == 1).</p></li>
-<li><p><strong>control_2</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The second qubit that controls whether the gate will act
-(if Z_control_2 == -1) or not (if Z_control_2 == 1).</p></li>
-<li><p><strong>target</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubit that will be flipped if Z_control_1 and Z_control_2 are
-equal to -1.</p></li>
+<li><p><strong>control1</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>)</p></li>
+<li><p><strong>control2</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubits that control whether the gate will act
+(if Z_control1 == Z_control2 == -1) or not (any other Z_control values).</p></li>
+<li><p><strong>target</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The target qubit on which the controlled operation will act.
+If the controlled operation acts on more qubits, then these
+can be provided as additional arguments.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
-<dt class="sig sig-object py" id="parityos.base.gates.CNOT">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CNOT</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CNOT" title="Link to this definition"></a></dt>
-<dd><p>Represents a CNOT gate</p>
-<dl class="py method">
-<dt class="sig sig-object py" id="parityos.base.gates.CNOT.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CNOT.__init__" title="Link to this definition"></a></dt>
-<dd><dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>control</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubit that controls whether the gate will act
-(if Z_control == -1) or not (if Z_control == 1).</p></li>
-<li><p><strong>target</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubit that will be flipped if Z_control == -1.</p></li>
-</ul>
-</dd>
-</dl>
+<dt class="sig sig-object py" id="parityos.base.gates.CCNOT">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CCNOT</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">control2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CCNOT" title="Link to this definition"></a></dt>
+<dd><p>Represents a CCNOT gate</p>
 </dd></dl>
 
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CH">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CH</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CH" title="Link to this definition"></a></dt>
+<dd><p>Represents a CH gate</p>
 </dd></dl>
 
 <dl class="py class">
-<dt class="sig sig-object py" id="parityos.base.gates.CZ">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CZ</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CZ" title="Link to this definition"></a></dt>
-<dd><p>Represents a CZ gate</p>
+<dt class="sig sig-object py" id="parityos.base.gates.CMixin">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CMixin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CMixin" title="Link to this definition"></a></dt>
+<dd><p>Adds a single control qubit to a gate. This mixin must come before the gate parent class in the
+new class definition.</p>
+<dl class="simple">
+<dt>Example:</dt><dd><p>class CNOT(CMixin, X):  # Creates a class that stores information for a CNOT gate.</p>
+</dd>
+<dt>Attributes:</dt><dd><dl class="simple">
+<dt>control_qubits: The tuple of control qubits that can block the operation of the underlying</dt><dd><p>gate.</p>
+</dd>
+</dl>
+</dd>
+</dl>
 <dl class="py method">
-<dt class="sig sig-object py" id="parityos.base.gates.CZ.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CZ.__init__" title="Link to this definition"></a></dt>
+<dt class="sig sig-object py" id="parityos.base.gates.CMixin.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CMixin.__init__" title="Link to this definition"></a></dt>
 <dd><dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>control</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubit that controls whether the gate will act
 (if Z_control == -1) or not (if Z_control == 1).</p></li>
-<li><p><strong>target</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The qubit phase that will be flipped if Z_control == -1.</p></li>
+<li><p><strong>target</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – The target qubit on which the controlled operation will act.
+If the controlled operation acts on more qubits, then these
+can be provided as additional arguments.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CNOT">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CNOT</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CNOT" title="Link to this definition"></a></dt>
+<dd><p>Represents a CNOT gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CRx">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CRx</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CRx" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Rx gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CRy">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CRy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CRy" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Ry gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CRz">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CRz</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CRz" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Rz gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CY">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CY</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CY" title="Link to this definition"></a></dt>
+<dd><p>Represents a CY gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.CZ">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">CZ</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.CZ" title="Link to this definition"></a></dt>
+<dd><p>Represents a CZ gate</p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Gate">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Gate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">qubit_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Gate" title="Link to this definition"></a></dt>
 <dd><p>Base class from which all gates inherit.</p>
 <p>The Gate subclasses are intended to store the information received from the compiler.
 They do not implement any methods to simulate the gates, nor do they contain any information
 on the (anti-) commutation relations between them or other mathematical properties.
 For those uses we recommend more elaborate frameworks like Qutip, Cirq or Qiskit.</p>
@@ -544,14 +612,25 @@
 <dd class="field-odd"><p>the sequence of arguments that would be needed to instantiate a copy of self
 (does not include keyword only arguments).</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="parityos.base.gates.Gate.make_args_and_kwargs_from_json">
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">make_args_and_kwargs_from_json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">list</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#parityos.base.gates.Gate.make_args_and_kwargs_from_json" title="Link to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>the sequence of arguments keyword arguments derived from the given json data
+that would be needed to create an instance of the class.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="parityos.base.gates.Gate.modify_angle">
 <span class="sig-name descname"><span class="pre">modify_angle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span><a class="headerlink" href="#parityos.base.gates.Gate.modify_angle" title="Link to this definition"></a></dt>
 <dd><p>The <cite>RMixin.modify_angle</cite> method is used to create a new version of the gate, with the same
 arguments except for the angle, which might get a new value.
 For other gates (the subject of this version), a simple copy of the gate is returned.</p>
 </dd></dl>
 
@@ -596,16 +675,16 @@
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><strong>qubit</strong> (<a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.Qubit"><em>Qubit</em></a>) – qubit on which the gate acts.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
-<dt class="sig sig-object py" id="parityos.base.gates.Gate1.qubit">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">qubit</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></em><a class="headerlink" href="#parityos.base.gates.Gate1.qubit" title="Link to this definition"></a></dt>
+<dt class="sig sig-object py" id="parityos.base.gates.Gate1.target_qubit">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">target_qubit</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></em><a class="headerlink" href="#parityos.base.gates.Gate1.target_qubit" title="Link to this definition"></a></dt>
 <dd><p>Return the qubit on which this gate acts.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>The qubit on which the gate acts.</p>
 </dd>
 </dl>
 </dd></dl>
@@ -680,14 +759,71 @@
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.ISwap">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">ISwap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">qubit1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">qubit2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.ISwap" title="Link to this definition"></a></dt>
+<dd><p>Represents an iSwap gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlMixin">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">MultiControlMixin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlMixin" title="Link to this definition"></a></dt>
+<dd><p>Adds an arbitrary control sequence to a gate. This mixin must come before the gate parent
+class in the new class definition.</p>
+<dl class="simple">
+<dt>Example:</dt><dd><p>class MultiControlledH(MultiControlMixin, H):  # Creates a class that stores information for
+a multi-controlled Hadamard gate.</p>
+</dd>
+</dl>
+<dl class="py method">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlMixin.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlMixin.__init__" title="Link to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>control_qubits</strong> – A sequence of control qubits that can block the operation of the
+underlying gate.</p></li>
+<li><p><strong>target</strong> – The qubit on which the underlying gate should act. If more qubits are
+targeted, then they can be added as additional arguments.</p></li>
+</ul>
+</dd>
+</dl>
+</dd></dl>
+
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlledH">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">MultiControlledH</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlledH" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Hadamard gate with arbitrary control sequence</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlledRx">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">MultiControlledRx</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlledRx" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Rx gate with arbitrary control sequence</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlledRy">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">MultiControlledRy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlledRy" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Ry gate with arbitrary control sequence</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.MultiControlledRz">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">MultiControlledRz</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">control_qubits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.MultiControlledRz" title="Link to this definition"></a></dt>
+<dd><p>Represents a controlled Rz gate with arbitrary control sequence</p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.RMixin">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">RMixin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.RMixin" title="Link to this definition"></a></dt>
 <dd><p>A mixin that converts a gate into a rotated gate.</p>
 <dl class="simple">
 <dt>Attributes:</dt><dd><p>angle: the angle for the gate rotation
 parameter_name: a label that identifies the parameter with which to multiply
 the angle when implementing it. If no parameter name is given, then the gate is
@@ -708,28 +844,14 @@
 the angle when implementing it.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="parityos.base.gates.RMixin.from_json">
-<em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">from_json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span><a class="headerlink" href="#parityos.base.gates.RMixin.from_json" title="Link to this definition"></a></dt>
-<dd><p>Creates a gate from a json compatible object.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>data</strong> – gate parameters in json compatible format</p>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>a Gate instance</p>
-</dd>
-</dl>
-</dd></dl>
-
-<dl class="py method">
 <dt class="sig sig-object py" id="parityos.base.gates.RMixin.get_hermitian_conjugate">
 <span class="sig-name descname"><span class="pre">get_hermitian_conjugate</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span><a class="headerlink" href="#parityos.base.gates.RMixin.get_hermitian_conjugate" title="Link to this definition"></a></dt>
 <dd><dl class="field-list simple">
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>the Hermitian conjugate of the gate</p>
 </dd>
 </dl>
@@ -742,14 +864,25 @@
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>the sequence of arguments that would be needed to instantiate a copy of self.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="parityos.base.gates.RMixin.make_args_and_kwargs_from_json">
+<em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">make_args_and_kwargs_from_json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">JSONType</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">list</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">dict</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#parityos.base.gates.RMixin.make_args_and_kwargs_from_json" title="Link to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>the sequence of arguments keyword arguments derived from the given json data
+that would be needed to create an instance of the class.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="parityos.base.gates.RMixin.modify_angle">
 <span class="sig-name descname"><span class="pre">modify_angle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">angle_map</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">frozenset</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">float</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">gate_type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#parityos.base.gates.Gate" title="parityos.base.gates.Gate"><span class="pre">Gate</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#parityos.base.gates.Gate" title="parityos.base.gates.Gate"><span class="pre">Gate</span></a></span></span><a class="headerlink" href="#parityos.base.gates.RMixin.modify_angle" title="Link to this definition"></a></dt>
 <dd><p>Create a new gate with the same arguments as this one, except for rotation gates of the
 given gate type and with the given parameter_name as parameter,
 for which the angle will be changed to the value given by the angle map, in function
 of the qubit(s) on which the gate acts. If the qubit(s) are not included in the angle map,
 then the angle is left unchanged.</p>
@@ -835,32 +968,56 @@
 <dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Rx">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Rx</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Rx" title="Link to this definition"></a></dt>
 <dd><p>Represents an RX gate</p>
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.Rxx">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Rxx</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Rxx" title="Link to this definition"></a></dt>
+<dd><p>Represents an RXX gate</p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Ry">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Ry</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Ry" title="Link to this definition"></a></dt>
 <dd><p>Represents an RY gate</p>
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.Ryy">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Ryy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Ryy" title="Link to this definition"></a></dt>
+<dd><p>Represents an RYY gate</p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Rz">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Rz</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Rz" title="Link to this definition"></a></dt>
 <dd><p>Represents an RZ gate</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Rzz">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Rzz</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Rzz" title="Link to this definition"></a></dt>
 <dd><p>Represents an RZZ gate</p>
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.Rzzzz">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Rzzzz</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parameter_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Rzzzz" title="Link to this definition"></a></dt>
+<dd><p>Represents an RZZZZ gate</p>
+</dd></dl>
+
+<dl class="py class">
+<dt class="sig sig-object py" id="parityos.base.gates.Swap">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">Swap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">qubit1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">qubit2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.Swap" title="Link to this definition"></a></dt>
+<dd><p>Represents a Swap gate</p>
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.X">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">parityos.base.gates.</span></span><span class="sig-name descname"><span class="pre">X</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">qubit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="parityos.html#parityos.Qubit" title="parityos.base.qubits.Qubit"><span class="pre">Qubit</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos.base.gates.X" title="Link to this definition"></a></dt>
 <dd><p>Represents an X gate</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="parityos.base.gates.Y">
```

#### html2text {}

```diff
@@ -24,54 +24,72 @@
                       # _C_i_r_c_u_i_t_._g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)
                       # _C_i_r_c_u_i_t_._m_o_d_i_f_y___a_n_g_l_e_(_)
                       # _C_i_r_c_u_i_t_._p_a_r_a_m_e_t_e_r_s
                       # _C_i_r_c_u_i_t_._q_u_b_i_t_s
                       # _C_i_r_c_u_i_t_._r_e_m_a_p_(_)
                       # _C_i_r_c_u_i_t_._t_o___j_s_o_n_(_)
                 # _c_o_n_v_e_r_t___c_n_o_t_s___t_o___r_z_z_s_(_)
+                # _C_C_M_i_x_i_n
+                      # _C_C_M_i_x_i_n_._____i_n_i_t_____(_)
                 # _C_C_N_O_T
-                      # _C_C_N_O_T_._____i_n_i_t_____(_)
+                # _C_H
+                # _C_M_i_x_i_n
+                      # _C_M_i_x_i_n_._____i_n_i_t_____(_)
                 # _C_N_O_T
-                      # _C_N_O_T_._____i_n_i_t_____(_)
+                # _C_R_x
+                # _C_R_y
+                # _C_R_z
+                # _C_Y
                 # _C_Z
-                      # _C_Z_._____i_n_i_t_____(_)
                 # _G_a_t_e
                       # _G_a_t_e_._____i_n_i_t_____(_)
                       # _G_a_t_e_._f_r_o_m___j_s_o_n_(_)
                       # _G_a_t_e_._g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)
                       # _G_a_t_e_._m_a_k_e___a_r_g_s_(_)
+                      # _G_a_t_e_._m_a_k_e___a_r_g_s___a_n_d___k_w_a_r_g_s___f_r_o_m___j_s_o_n_(_)
                       # _G_a_t_e_._m_o_d_i_f_y___a_n_g_l_e_(_)
                       # _G_a_t_e_._q_u_b_i_t_s
                       # _G_a_t_e_._r_e_m_a_p_(_)
                       # _G_a_t_e_._t_o___j_s_o_n_(_)
                 # _G_a_t_e_1
                       # _G_a_t_e_1_._____i_n_i_t_____(_)
-                      # _G_a_t_e_1_._q_u_b_i_t
+                      # _G_a_t_e_1_._t_a_r_g_e_t___q_u_b_i_t
                 # _G_a_t_e_2
                       # _G_a_t_e_2_._____i_n_i_t_____(_)
                 # _G_a_t_e_3
                       # _G_a_t_e_3_._____i_n_i_t_____(_)
                 # _G_a_t_e_4
                       # _G_a_t_e_4_._____i_n_i_t_____(_)
                 # _H
                 # _H_e_r_m_i_t_i_a_n_G_a_t_e_M_i_x_i_n
                       # _H_e_r_m_i_t_i_a_n_G_a_t_e_M_i_x_i_n_._g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)
+                # _I_S_w_a_p
+                # _M_u_l_t_i_C_o_n_t_r_o_l_M_i_x_i_n
+                      # _M_u_l_t_i_C_o_n_t_r_o_l_M_i_x_i_n_._____i_n_i_t_____(_)
+                # _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_H
+                # _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_x
+                # _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_y
+                # _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_z
                 # _R_M_i_x_i_n
                       # _R_M_i_x_i_n_._____i_n_i_t_____(_)
-                      # _R_M_i_x_i_n_._f_r_o_m___j_s_o_n_(_)
                       # _R_M_i_x_i_n_._g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)
                       # _R_M_i_x_i_n_._m_a_k_e___a_r_g_s_(_)
+                      # _R_M_i_x_i_n_._m_a_k_e___a_r_g_s___a_n_d___k_w_a_r_g_s___f_r_o_m___j_s_o_n_(_)
                       # _R_M_i_x_i_n_._m_o_d_i_f_y___a_n_g_l_e_(_)
                       # _R_M_i_x_i_n_._p_a_r_a_m_e_t_e_r_s
                       # _R_M_i_x_i_n_._r_e_m_a_p_(_)
                       # _R_M_i_x_i_n_._t_o___j_s_o_n_(_)
                 # _R_x
+                # _R_x_x
                 # _R_y
+                # _R_y_y
                 # _R_z
                 # _R_z_z
+                # _R_z_z_z_z
+                # _S_w_a_p
                 # _X
                 # _Y
                 # _Z
                 # _J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n
                       # _J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_._f_r_o_m___j_s_o_n_(_)
                       # _J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_._l_o_a_d_(_)
                       # _J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_._s_a_v_e_(_)
@@ -220,45 +238,77 @@
         Parameters:
             cciirrccuuiitt (_CC_ii_rr_cc_uu_ii_tt) – a circuit containing moments with CNOT gates.
         Returns:
             a new circuit where all CNOTs have been replaced by ZZ and local
             rotations.
         Return type:
             _C_i_r_c_u_i_t
-  ccllaassss parityos.base.gates.CCNOT(ccoonnttrrooll__11:: _QQ_uu_bb_ii_tt, ccoonnttrrooll__22:: _QQ_uu_bb_ii_tt, ttaarrggeett::
-  _QQ_uu_bb_ii_tt)_
-      Represents a CCNOT gate
-        __init__(ccoonnttrrooll__11:: _QQ_uu_bb_ii_tt, ccoonnttrrooll__22:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt)_
+  ccllaassss parityos.base.gates.CCMixin(ccoonnttrrooll11:: _QQ_uu_bb_ii_tt, ccoonnttrrooll22:: _QQ_uu_bb_ii_tt, ttaarrggeett::
+  _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Adds two control qubits to a gate. This mixin must come before the gate
+      parent class in the new class definition.
+        Example:
+            class CCNOT(CCMixin, X): # Creates a class that stores information
+            for a CCNOT gate.
+        Attributes:
+              control_qubits: The tuple of control qubits that can block the
+              operation of the underlying
+                  gate.
+        __init__(ccoonnttrrooll11:: _QQ_uu_bb_ii_tt, ccoonnttrrooll22:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+        ****kkwwaarrggss)_
               Parameters:
-                      * ccoonnttrrooll__11 (_QQ_uu_bb_ii_tt) – The first qubit that controls
-                        whether the gate will act (if Z_control_1 == -1) or not
-                        (if Z_control_1 == 1).
-                      * ccoonnttrrooll__22 (_QQ_uu_bb_ii_tt) – The second qubit that controls
-                        whether the gate will act (if Z_control_2 == -1) or not
-                        (if Z_control_2 == 1).
-                      * ttaarrggeett (_QQ_uu_bb_ii_tt) – The qubit that will be flipped if
-                        Z_control_1 and Z_control_2 are equal to -1.
-  ccllaassss parityos.base.gates.CNOT(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt)_
-      Represents a CNOT gate
-        __init__(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt)_
+                      * ccoonnttrrooll11 (_QQ_uu_bb_ii_tt)
+                      * ccoonnttrrooll22 (_QQ_uu_bb_ii_tt) – The qubits that control whether the
+                        gate will act (if Z_control1 == Z_control2 == -1) or
+                        not (any other Z_control values).
+                      * ttaarrggeett (_QQ_uu_bb_ii_tt) – The target qubit on which the
+                        controlled operation will act. If the controlled
+                        operation acts on more qubits, then these can be
+                        provided as additional arguments.
+  ccllaassss parityos.base.gates.CCNOT(ccoonnttrrooll11:: _QQ_uu_bb_ii_tt, ccoonnttrrooll22:: _QQ_uu_bb_ii_tt, ttaarrggeett::
+  _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a CCNOT gate
+  ccllaassss parityos.base.gates.CH(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a CH gate
+  ccllaassss parityos.base.gates.CMixin(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+  ****kkwwaarrggss)_
+      Adds a single control qubit to a gate. This mixin must come before the
+      gate parent class in the new class definition.
+        Example:
+            class CNOT(CMixin, X): # Creates a class that stores information
+            for a CNOT gate.
+        Attributes:
+              control_qubits: The tuple of control qubits that can block the
+              operation of the underlying
+                  gate.
+        __init__(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
               Parameters:
                       * ccoonnttrrooll (_QQ_uu_bb_ii_tt) – The qubit that controls whether the
                         gate will act (if Z_control == -1) or not (if Z_control
                         == 1).
-                      * ttaarrggeett (_QQ_uu_bb_ii_tt) – The qubit that will be flipped if
-                        Z_control == -1.
-  ccllaassss parityos.base.gates.CZ(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt)_
+                      * ttaarrggeett (_QQ_uu_bb_ii_tt) – The target qubit on which the
+                        controlled operation will act. If the controlled
+                        operation acts on more qubits, then these can be
+                        provided as additional arguments.
+  ccllaassss parityos.base.gates.CNOT(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+  ****kkwwaarrggss)_
+      Represents a CNOT gate
+  ccllaassss parityos.base.gates.CRx(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+  ****kkwwaarrggss)_
+      Represents a controlled Rx gate
+  ccllaassss parityos.base.gates.CRy(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+  ****kkwwaarrggss)_
+      Represents a controlled Ry gate
+  ccllaassss parityos.base.gates.CRz(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+  ****kkwwaarrggss)_
+      Represents a controlled Rz gate
+  ccllaassss parityos.base.gates.CY(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a CY gate
+  ccllaassss parityos.base.gates.CZ(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
       Represents a CZ gate
-        __init__(ccoonnttrrooll:: _QQ_uu_bb_ii_tt, ttaarrggeett:: _QQ_uu_bb_ii_tt)_
-              Parameters:
-                      * ccoonnttrrooll (_QQ_uu_bb_ii_tt) – The qubit that controls whether the
-                        gate will act (if Z_control == -1) or not (if Z_control
-                        == 1).
-                      * ttaarrggeett (_QQ_uu_bb_ii_tt) – The qubit phase that will be flipped
-                        if Z_control == -1.
   ccllaassss parityos.base.gates.Gate(**qquubbiitt__aarrggss:: _QQ_uu_bb_ii_tt)_
       Base class from which all gates inherit.
       The Gate subclasses are intended to store the information received from
       the compiler. They do not implement any methods to simulate the gates,
       nor do they contain any information on the (anti-) commutation relations
       between them or other mathematical properties. For those uses we
       recommend more elaborate frameworks like Qutip, Cirq or Qiskit.
@@ -274,14 +324,22 @@
         get_hermitian_conjugate() → Self_
               Returns:
                   the Hermitian conjugate of the gate
         make_args() → tuple[_Q_u_b_i_t]_
               Returns:
                   the sequence of arguments that would be needed to instantiate
                   a copy of self (does not include keyword only arguments).
+        ssttaattiicc make_args_and_kwargs_from_json(ddaattaa:: SSeeqquueennccee[[ssttrr || iinntt || ffllooaatt
+        || bbooooll || NNoonnee || ddiicctt[[ssttrr,, ssttrr || iinntt || ffllooaatt || bbooooll || NNoonnee || ddiicctt[[ssttrr,,
+        JJSSOONNTTyyppee]] || lliisstt[[JJSSOONNTTyyppee]]]] || lliisstt[[ssttrr || iinntt || ffllooaatt || bbooooll || NNoonnee ||
+        ddiicctt[[ssttrr,, JJSSOONNTTyyppee]] || lliisstt[[JJSSOONNTTyyppee]]]]]]) → tuple[list, dict]_
+              Returns:
+                  the sequence of arguments keyword arguments derived from the
+                  given json data that would be needed to create an instance of
+                  the class.
         modify_angle(**aarrggss, ****kkwwaarrggss) → Self_
             TheRMixin.modify_anglemethod is used to create a new version of the
             gate, with the same arguments except for the angle, which might get
             a new value. For other gates (the subject of this version), a
             simple copy of the gate is returned.
         pprrooppeerrttyy qubits:: sseett[[_QQ_uu_bb_ii_tt]]_
               Returns:
@@ -299,15 +357,15 @@
                   a json compatible object with all the information about the
                   gate.
   ccllaassss parityos.base.gates.Gate1(qquubbiitt:: _QQ_uu_bb_ii_tt)_
       A Gate that acts on a single qubit.
         __init__(qquubbiitt:: _QQ_uu_bb_ii_tt)_
               Parameters:
                   qquubbiitt (_QQ_uu_bb_ii_tt) – qubit on which the gate acts.
-        pprrooppeerrttyy qubit:: _QQ_uu_bb_ii_tt_
+        pprrooppeerrttyy target_qubit:: _QQ_uu_bb_ii_tt_
             Return the qubit on which this gate acts.
               Returns:
                   The qubit on which the gate acts.
   ccllaassss parityos.base.gates.Gate2(qquubbiitt11:: _QQ_uu_bb_ii_tt, qquubbiitt22:: _QQ_uu_bb_ii_tt)_
       A Gate that acts on two qubits.
         __init__(qquubbiitt11:: _QQ_uu_bb_ii_tt, qquubbiitt22:: _QQ_uu_bb_ii_tt)_
               Parameters:
@@ -329,14 +387,43 @@
       Represents a Hadamard gate
   ccllaassss parityos.base.gates.HermitianGateMixin(**qquubbiitt__aarrggss:: _QQ_uu_bb_ii_tt)_
       A mixin that implements hermitian_conjugate method for Hermitian gates.
         get_hermitian_conjugate() → Self_
               Returns:
                   the Hermitian conjugate of the gate, which is the copy of
                   itself for Hermitian gates
+  ccllaassss parityos.base.gates.ISwap(qquubbiitt11:: _QQ_uu_bb_ii_tt, qquubbiitt22:: _QQ_uu_bb_ii_tt)_
+      Represents an iSwap gate
+  ccllaassss parityos.base.gates.MultiControlMixin(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]],
+  ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Adds an arbitrary control sequence to a gate. This mixin must come before
+      the gate parent class in the new class definition.
+        Example:
+            class MultiControlledH(MultiControlMixin, H): # Creates a class
+            that stores information for a multi-controlled Hadamard gate.
+        __init__(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]], ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss,
+        ****kkwwaarrggss)_
+              Parameters:
+                      * ccoonnttrrooll__qquubbiittss – A sequence of control qubits that can
+                        block the operation of the underlying gate.
+                      * ttaarrggeett – The qubit on which the underlying gate should
+                        act. If more qubits are targeted, then they can be
+                        added as additional arguments.
+  ccllaassss parityos.base.gates.MultiControlledH(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]],
+  ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a controlled Hadamard gate with arbitrary control sequence
+  ccllaassss parityos.base.gates.MultiControlledRx(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]],
+  ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a controlled Rx gate with arbitrary control sequence
+  ccllaassss parityos.base.gates.MultiControlledRy(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]],
+  ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a controlled Ry gate with arbitrary control sequence
+  ccllaassss parityos.base.gates.MultiControlledRz(ccoonnttrrooll__qquubbiittss:: SSeeqquueennccee[[_QQ_uu_bb_ii_tt]],
+  ttaarrggeett:: _QQ_uu_bb_ii_tt, **aarrggss, ****kkwwaarrggss)_
+      Represents a controlled Rz gate with arbitrary control sequence
   ccllaassss parityos.base.gates.RMixin(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
   NNoonnee, ****kkwwaarrggss)_
       A mixin that converts a gate into a rotated gate.
         Attributes:
             angle: the angle for the gate rotation parameter_name: a label that
             identifies the parameter with which to multiply the angle when
             implementing it. If no parameter name is given, then the gate is
@@ -347,28 +434,29 @@
         __init__(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr == NNoonnee, ****kkwwaarrggss)_
               Parameters:
                       * aarrggss (_QQ_uu_bb_ii_tt) – a list of Qubits on which the gate acts
                       * aannggllee (ffllooaatt) – the angle for the gate rotation
                       * ppaarraammeetteerr__nnaammee (ssttrr) – a label that identifies the
                         parameter with which to multiply the angle when
                         implementing it.
-        ccllaassssmmeetthhoodd from_json(ddaattaa:: SSeeqquueennccee[[ssttrr || iinntt || ffllooaatt || bbooooll || NNoonnee ||
-        ddiicctt[[ssttrr,, JJSSOONNTTyyppee]] || lliisstt[[JJSSOONNTTyyppee]]]]) → Self_
-            Creates a gate from a json compatible object.
-              Parameters:
-                  ddaattaa – gate parameters in json compatible format
-              Returns:
-                  a Gate instance
         get_hermitian_conjugate() → Self_
               Returns:
                   the Hermitian conjugate of the gate
         make_args() → tuple_
               Returns:
                   the sequence of arguments that would be needed to instantiate
                   a copy of self.
+        ccllaassssmmeetthhoodd make_args_and_kwargs_from_json(ddaattaa:: SSeeqquueennccee[[ssttrr || iinntt ||
+        ffllooaatt || bbooooll || NNoonnee || ddiicctt[[ssttrr,, ssttrr || iinntt || ffllooaatt || bbooooll || NNoonnee || ddiicctt
+        [[ssttrr,, JJSSOONNTTyyppee]] || lliisstt[[JJSSOONNTTyyppee]]]] || lliisstt[[ssttrr || iinntt || ffllooaatt || bbooooll ||
+        NNoonnee || ddiicctt[[ssttrr,, JJSSOONNTTyyppee]] || lliisstt[[JJSSOONNTTyyppee]]]]]]) → tuple[list, dict]_
+              Returns:
+                  the sequence of arguments keyword arguments derived from the
+                  given json data that would be needed to create an instance of
+                  the class.
         modify_angle(aannggllee__mmaapp:: MMaappppiinngg[[ffrroozzeennsseett[[_QQ_uu_bb_ii_tt]],, ffllooaatt]], ggaattee__ttyyppee::
         ttyyppee[[_GG_aa_tt_ee]] == NNoonnee, ppaarraammeetteerr__nnaammee:: ssttrr == NNoonnee) → _G_a_t_e_
             Create a new gate with the same arguments as this one, except for
             rotation gates of the given gate type and with the given
             parameter_name as parameter, for which the angle will be changed to
             the value given by the angle map, in function of the qubit(s) on
             which the gate acts. If the qubit(s) are not included in the angle
@@ -429,23 +517,34 @@
         [JSONType]]]_
               Returns:
                   a json compatible object with all the information about the
                   gate.
   ccllaassss parityos.base.gates.Rx(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
   NNoonnee, ****kkwwaarrggss)_
       Represents an RX gate
+  ccllaassss parityos.base.gates.Rxx(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
+  NNoonnee, ****kkwwaarrggss)_
+      Represents an RXX gate
   ccllaassss parityos.base.gates.Ry(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
   NNoonnee, ****kkwwaarrggss)_
       Represents an RY gate
+  ccllaassss parityos.base.gates.Ryy(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
+  NNoonnee, ****kkwwaarrggss)_
+      Represents an RYY gate
   ccllaassss parityos.base.gates.Rz(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
   NNoonnee, ****kkwwaarrggss)_
       Represents an RZ gate
   ccllaassss parityos.base.gates.Rzz(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
   NNoonnee, ****kkwwaarrggss)_
       Represents an RZZ gate
+  ccllaassss parityos.base.gates.Rzzzz(**aarrggss:: _QQ_uu_bb_ii_tt || ffllooaatt, ppaarraammeetteerr__nnaammee:: ssttrr ==
+  NNoonnee, ****kkwwaarrggss)_
+      Represents an RZZZZ gate
+  ccllaassss parityos.base.gates.Swap(qquubbiitt11:: _QQ_uu_bb_ii_tt, qquubbiitt22:: _QQ_uu_bb_ii_tt)_
+      Represents a Swap gate
   ccllaassss parityos.base.gates.X(qquubbiitt:: _QQ_uu_bb_ii_tt)_
       Represents an X gate
   ccllaassss parityos.base.gates.Y(qquubbiitt:: _QQ_uu_bb_ii_tt)_
       Represents a Y gate
   ccllaassss parityos.base.gates.Z(qquubbiitt:: _QQ_uu_bb_ii_tt)_
       Represents a Z gate
   ccllaassss parityos.base.utils.JSONLoadSaveMixin_
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/encodings.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/encodings.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="parityos_addons" href="parityos_addons.html" />
     <link rel="prev" title="parityos.api_interface" href="api_interface.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/index.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
+        <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="parityos" href="parityos.html" />
     <link rel="prev" title="Solving Optimization Problems" href="../tutorial.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/parityos.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/parityos.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
         <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="parityos.base" href="base.html" />
     <link rel="prev" title="API Reference" href="index.html" />
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/api_reference/parityos_addons.html` & `parityos-2.5.0/parityos_addons/documentation/html/api_reference/parityos_addons.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="../_static/documentation_options.js?v=841abef3"></script>
-        <script src="../_static/doctools.js?v=888ff710"></script>
+        <script src="../_static/doctools.js?v=9a2dae69"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="prev" title="parityos.encodings" href="encodings.html" /> 
 </head>
 
@@ -61,15 +61,15 @@
 <li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.CirqExporter.__init__"><code class="docutils literal notranslate"><span class="pre">CirqExporter.__init__()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.CirqExporter.gate_to_cirq"><code class="docutils literal notranslate"><span class="pre">CirqExporter.gate_to_cirq()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.CirqExporter.to_cirq"><code class="docutils literal notranslate"><span class="pre">CirqExporter.to_cirq()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos_addons.interfaces.QiskitExporter"><code class="docutils literal notranslate"><span class="pre">QiskitExporter</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.QiskitExporter.__init__"><code class="docutils literal notranslate"><span class="pre">QiskitExporter.__init__()</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.QiskitExporter.gate_to_qiskit"><code class="docutils literal notranslate"><span class="pre">QiskitExporter.gate_to_qiskit()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.QiskitExporter.append_qiskit_gate"><code class="docutils literal notranslate"><span class="pre">QiskitExporter.append_qiskit_gate()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#parityos_addons.interfaces.QiskitExporter.to_qiskit"><code class="docutils literal notranslate"><span class="pre">QiskitExporter.to_qiskit()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos_addons.qaoa.generate_qaoa"><code class="docutils literal notranslate"><span class="pre">generate_qaoa()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos_addons.spin_hamiltonians.SpinZ"><code class="docutils literal notranslate"><span class="pre">SpinZ</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos_addons.spin_hamiltonians.spinz_to_constraint"><code class="docutils literal notranslate"><span class="pre">spinz_to_constraint()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#parityos_addons.spin_hamiltonians.spinz_to_hamiltonian"><code class="docutils literal notranslate"><span class="pre">spinz_to_hamiltonian()</span></code></a></li>
@@ -201,25 +201,20 @@
 Either a <cite>qubit_map</cite> or a <cite>qubits</cite> iterable must be given.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="parityos_addons.interfaces.QiskitExporter.gate_to_qiskit">
-<span class="sig-name descname"><span class="pre">gate_to_qiskit</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">gate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="base.html#parityos.base.gates.Gate" title="parityos.base.gates.Gate"><span class="pre">Gate</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Gate</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#parityos_addons.interfaces.QiskitExporter.gate_to_qiskit" title="Link to this definition"></a></dt>
-<dd><p>Converts a gate to a (Qiskit instruction, qubit_indices) tuple.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>gate</strong> – a ParityOS gate instance.</p>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>a (Qiskit instruction, qubit_indices) tuple.</p>
-</dd>
-</dl>
+<dt class="sig sig-object py" id="parityos_addons.interfaces.QiskitExporter.append_qiskit_gate">
+<span class="sig-name descname"><span class="pre">append_qiskit_gate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">qiskit_circuit:</span> <span class="pre">&lt;module</span> <span class="pre">'qiskit.circuit'</span> <span class="pre">from</span> <span class="pre">'/usr/local/lib/python3.11/site-packages/qiskit/circuit/__init__.py'&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">gate:</span> <span class="pre">~parityos.base.gates.Gate</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#parityos_addons.interfaces.QiskitExporter.append_qiskit_gate" title="Link to this definition"></a></dt>
+<dd><p>Creates a qiskit gate corresponding to the ParityOS Gate instance and appends it to the
+qiskit circuit.
+:param qiskit_circuit: the qiskit circuit to which we want to append the gate
+:param gate: the ParityOS Gate that is appended to the circuit</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="parityos_addons.interfaces.QiskitExporter.to_qiskit">
 <span class="sig-name descname"><span class="pre">to_qiskit</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">circuit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="base.html#parityos.base.gates.Gate" title="parityos.base.gates.Gate"><span class="pre">Gate</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="base.html#parityos.base.circuit.Circuit" title="parityos.base.circuit.Circuit"><span class="pre">Circuit</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">QuantumCircuit</span></span></span><a class="headerlink" href="#parityos_addons.interfaces.QiskitExporter.to_qiskit" title="Link to this definition"></a></dt>
 <dd><p>Converts the circuit to a Qiskit quantum circuit.</p>
 <dl class="field-list simple">
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
           o _p_a_r_i_t_y_o_s___a_d_d_o_n_s
                 # _C_i_r_q_E_x_p_o_r_t_e_r
                       # _C_i_r_q_E_x_p_o_r_t_e_r_._____i_n_i_t_____(_)
                       # _C_i_r_q_E_x_p_o_r_t_e_r_._g_a_t_e___t_o___c_i_r_q_(_)
                       # _C_i_r_q_E_x_p_o_r_t_e_r_._t_o___c_i_r_q_(_)
                 # _Q_i_s_k_i_t_E_x_p_o_r_t_e_r
                       # _Q_i_s_k_i_t_E_x_p_o_r_t_e_r_._____i_n_i_t_____(_)
-                      # _Q_i_s_k_i_t_E_x_p_o_r_t_e_r_._g_a_t_e___t_o___q_i_s_k_i_t_(_)
+                      # _Q_i_s_k_i_t_E_x_p_o_r_t_e_r_._a_p_p_e_n_d___q_i_s_k_i_t___g_a_t_e_(_)
                       # _Q_i_s_k_i_t_E_x_p_o_r_t_e_r_._t_o___q_i_s_k_i_t_(_)
                 # _g_e_n_e_r_a_t_e___q_a_o_a_(_)
                 # _S_p_i_n_Z
                 # _s_p_i_n_z___t_o___c_o_n_s_t_r_a_i_n_t_(_)
                 # _s_p_i_n_z___t_o___h_a_m_i_l_t_o_n_i_a_n_(_)
                 # _u_n_t_i_e___s_p_i_n_z___p_r_o_d_u_c_t_(_)
 _P_a_r_i_t_y_O_S
@@ -97,20 +97,21 @@
                       * qquubbiitt__mmaapp – a mapping of the form {ParityOS_qubit:
                         qubit_index}, where qubit_index is the integer index of
                         the qubit in the Qiskit qubit register. Optional.
                       * qquubbiittss – an iterable of ParityOS qubits. This is used
                         to generate a qubit_map where each qubit is mapped onto
                         its index in the sequence. Optional. Either
                         aqubit_mapor aqubitsiterable must be given.
-        gate_to_qiskit(ggaattee:: _GG_aa_tt_ee) → tuple[Gate, list[int]]_
-            Converts a gate to a (Qiskit instruction, qubit_indices) tuple.
-              Parameters:
-                  ggaattee – a ParityOS gate instance.
-              Returns:
-                  a (Qiskit instruction, qubit_indices) tuple.
+        append_qiskit_gate(qqiisskkiitt__cciirrccuuiitt:: <<mmoodduullee ''qqiisskkiitt..cciirrccuuiitt'' ffrroomm ''//uussrr//
+        llooccaall//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//qqiisskkiitt//cciirrccuuiitt//____iinniitt____..ppyy''>>, ggaattee::
+        ~~ppaarriittyyooss..bbaassee..ggaatteess..GGaattee)_
+            Creates a qiskit gate corresponding to the ParityOS Gate instance
+            and appends it to the qiskit circuit. :param qiskit_circuit: the
+            qiskit circuit to which we want to append the gate :param gate: the
+            ParityOS Gate that is appended to the circuit
         to_qiskit(cciirrccuuiitt:: _GG_aa_tt_ee || _CC_ii_rr_cc_uu_ii_tt) → QuantumCircuit_
             Converts the circuit to a Qiskit quantum circuit.
               Parameters:
                   cciirrccuuiitt – a ParityOS circuit of quantum gates.
               Returns:
                   a Qiskit QuantumCircuit object.
   parityos_addons.qaoa.generate_qaoa(ppaarriittyyooss__oouuttppuutt:: _PP_aa_rr_ii_tt_yy_OO_SS_OO_uu_tt_pp_uu_tt,
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/asynchronous_submission.html` & `parityos-2.5.0/parityos_addons/documentation/html/asynchronous_submission.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="The Parity Decoder" href="parity_decoder.html" />
     <link rel="prev" title="Making a custom device model" href="custom_device_models.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/custom_device_models.html` & `parityos-2.5.0/parityos_addons/documentation/html/custom_device_models.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Asynchronous submissions" href="asynchronous_submission.html" />
     <link rel="prev" title="Quickstart" href="quickstart.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/genindex.html` & `parityos-2.5.0/parityos_addons/documentation/html/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
@@ -76,14 +76,15 @@
            <div itemprop="articleBody">
              
 
 <h1 id="index">Index</h1>
 
 <div class="genindex-jumpbox">
  <a href="#_"><strong>_</strong></a>
+ | <a href="#A"><strong>A</strong></a>
  | <a href="#C"><strong>C</strong></a>
  | <a href="#D"><strong>D</strong></a>
  | <a href="#E"><strong>E</strong></a>
  | <a href="#F"><strong>F</strong></a>
  | <a href="#G"><strong>G</strong></a>
  | <a href="#H"><strong>H</strong></a>
  | <a href="#I"><strong>I</strong></a>
@@ -105,30 +106,30 @@
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.constraints.EqualityConstraint.__init__">__init__() (parityos.base.constraints.EqualityConstraint method)</a>
 
       <ul>
         <li><a href="api_reference/base.html#parityos.base.constraints.ParityConstraint.__init__">(parityos.base.constraints.ParityConstraint method)</a>
 </li>
-        <li><a href="api_reference/base.html#parityos.base.gates.CCNOT.__init__">(parityos.base.gates.CCNOT method)</a>
+        <li><a href="api_reference/base.html#parityos.base.gates.CCMixin.__init__">(parityos.base.gates.CCMixin method)</a>
 </li>
-        <li><a href="api_reference/base.html#parityos.base.gates.CNOT.__init__">(parityos.base.gates.CNOT method)</a>
-</li>
-        <li><a href="api_reference/base.html#parityos.base.gates.CZ.__init__">(parityos.base.gates.CZ method)</a>
+        <li><a href="api_reference/base.html#parityos.base.gates.CMixin.__init__">(parityos.base.gates.CMixin method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate.__init__">(parityos.base.gates.Gate method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate1.__init__">(parityos.base.gates.Gate1 method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate2.__init__">(parityos.base.gates.Gate2 method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate3.__init__">(parityos.base.gates.Gate3 method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate4.__init__">(parityos.base.gates.Gate4 method)</a>
 </li>
+        <li><a href="api_reference/base.html#parityos.base.gates.MultiControlMixin.__init__">(parityos.base.gates.MultiControlMixin method)</a>
+</li>
         <li><a href="api_reference/base.html#parityos.base.gates.RMixin.__init__">(parityos.base.gates.RMixin method)</a>
 </li>
         <li><a href="api_reference/encodings.html#parityos.encodings.mappings.Mappings.__init__">(parityos.encodings.mappings.Mappings method)</a>
 </li>
         <li><a href="api_reference/encodings.html#parityos.encodings.mappings.ParityMap.__init__">(parityos.encodings.mappings.ParityMap method)</a>
 </li>
         <li><a href="api_reference/parityos.html#parityos.Hamiltonian.__init__">(parityos.Hamiltonian method)</a>
@@ -147,35 +148,57 @@
 </li>
         <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.QiskitExporter.__init__">(parityos_addons.interfaces.QiskitExporter method)</a>
 </li>
       </ul></li>
   </ul></td>
 </tr></table>
 
+<h2 id="A">A</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.QiskitExporter.append_qiskit_gate">append_qiskit_gate() (parityos_addons.interfaces.QiskitExporter method)</a>
+</li>
+  </ul></td>
+</tr></table>
+
 <h2 id="C">C</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api_reference/base.html#parityos.base.gates.CCMixin">CCMixin (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.gates.CCNOT">CCNOT (class in parityos.base.gates)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CH">CH (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit">Circuit (class in parityos.base.circuit)</a>
 </li>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.CirqExporter">CirqExporter (class in parityos_addons.interfaces)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CMixin">CMixin (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.gates.CNOT">CNOT (class in parityos.base.gates)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos.html#parityos.CompilerClient.compile">compile() (parityos.CompilerClient method)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos.html#parityos.CompilerClient">CompilerClient (class in parityos)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.circuit.convert_cnots_to_rzzs">convert_cnots_to_rzzs() (in module parityos.base.circuit)</a>
 </li>
       <li><a href="api_reference/parityos.html#parityos.ParityOSOutput.create_default_problem_circuit">create_default_problem_circuit() (parityos.ParityOSOutput method)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CRx">CRx (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CRy">CRy (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CRz">CRz (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.CY">CY (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.gates.CZ">CZ (class in parityos.base.gates)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -215,16 +238,14 @@
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.from_json">from_json() (parityos.base.circuit.Circuit class method)</a>
 
       <ul>
         <li><a href="api_reference/base.html#parityos.base.constraints.EqualityConstraint.from_json">(parityos.base.constraints.EqualityConstraint class method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate.from_json">(parityos.base.gates.Gate class method)</a>
 </li>
-        <li><a href="api_reference/base.html#parityos.base.gates.RMixin.from_json">(parityos.base.gates.RMixin class method)</a>
-</li>
         <li><a href="api_reference/base.html#parityos.base.utils.JSONLoadSaveMixin.from_json">(parityos.base.utils.JSONLoadSaveMixin class method)</a>
 </li>
         <li><a href="api_reference/encodings.html#parityos.encodings.mappings.Mappings.from_json">(parityos.encodings.mappings.Mappings class method)</a>
 </li>
         <li><a href="api_reference/encodings.html#parityos.encodings.mappings.ParityMap.from_json">(parityos.encodings.mappings.ParityMap class method)</a>
 </li>
         <li><a href="api_reference/parityos.html#parityos.ParityOSOutput.from_json">(parityos.ParityOSOutput class method)</a>
@@ -252,16 +273,14 @@
 </li>
       <li><a href="api_reference/base.html#parityos.base.gates.Gate3">Gate3 (class in parityos.base.gates)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.gates.Gate4">Gate4 (class in parityos.base.gates)</a>
 </li>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.CirqExporter.gate_to_cirq">gate_to_cirq() (parityos_addons.interfaces.CirqExporter method)</a>
 </li>
-      <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.QiskitExporter.gate_to_qiskit">gate_to_qiskit() (parityos_addons.interfaces.QiskitExporter method)</a>
-</li>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.generate_flat_gate_sequence">generate_flat_gate_sequence() (parityos.base.circuit.Circuit method)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.qaoa.generate_qaoa">generate_qaoa() (in module parityos_addons.qaoa)</a>
 </li>
       <li><a href="api_reference/parityos.html#parityos.CompilerClient.get_compiler_runs">get_compiler_runs() (parityos.CompilerClient method)</a>
@@ -299,14 +318,18 @@
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.constraints.EqualityConstraint.is_satisfied">is_satisfied() (parityos.base.constraints.EqualityConstraint method)</a>
 </li>
   </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api_reference/base.html#parityos.base.gates.ISwap">ISwap (class in parityos.base.gates)</a>
+</li>
+  </ul></td>
 </tr></table>
 
 <h2 id="J">J</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.utils.json_wrap">json_wrap() (in module parityos.base.utils)</a>
 </li>
@@ -336,14 +359,20 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.gates.Gate.make_args">make_args() (parityos.base.gates.Gate method)</a>
 
       <ul>
         <li><a href="api_reference/base.html#parityos.base.gates.RMixin.make_args">(parityos.base.gates.RMixin method)</a>
 </li>
       </ul></li>
+      <li><a href="api_reference/base.html#parityos.base.gates.Gate.make_args_and_kwargs_from_json">make_args_and_kwargs_from_json() (parityos.base.gates.Gate static method)</a>
+
+      <ul>
+        <li><a href="api_reference/base.html#parityos.base.gates.RMixin.make_args_and_kwargs_from_json">(parityos.base.gates.RMixin class method)</a>
+</li>
+      </ul></li>
       <li><a href="api_reference/encodings.html#parityos.encodings.parity_decoder.ParityDecoderExtension.make_full_configuration_from_partial">make_full_configuration_from_partial() (parityos.encodings.parity_decoder.ParityDecoderExtension method)</a>
 </li>
       <li><a href="api_reference/encodings.html#parityos.encodings.mappings.Mappings">Mappings (class in parityos.encodings.mappings)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.modify_angle">modify_angle() (parityos.base.circuit.Circuit method)</a>
 
       <ul>
@@ -378,14 +407,26 @@
 </li>
         <li><a href="api_reference/parityos_addons.html#module-parityos_addons.qaoa">parityos_addons.qaoa</a>
 </li>
         <li><a href="api_reference/parityos_addons.html#module-parityos_addons.spin_hamiltonians">parityos_addons.spin_hamiltonians</a>
 </li>
       </ul></li>
   </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api_reference/base.html#parityos.base.gates.MultiControlledH">MultiControlledH (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.MultiControlledRx">MultiControlledRx (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.MultiControlledRy">MultiControlledRy (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.MultiControlledRz">MultiControlledRz (class in parityos.base.gates)</a>
+</li>
+      <li><a href="api_reference/base.html#parityos.base.gates.MultiControlMixin">MultiControlMixin (class in parityos.base.gates)</a>
+</li>
+  </ul></td>
 </tr></table>
 
 <h2 id="P">P</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.parameters">parameters (parityos.base.circuit.Circuit property)</a>
 
@@ -501,16 +542,14 @@
 <h2 id="Q">Q</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.QiskitExporter">QiskitExporter (class in parityos_addons.interfaces)</a>
 </li>
       <li><a href="api_reference/parityos.html#parityos.Qubit">Qubit (class in parityos)</a>
 </li>
-      <li><a href="api_reference/base.html#parityos.base.gates.Gate1.qubit">qubit (parityos.base.gates.Gate1 property)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.qubits">qubits (parityos.base.circuit.Circuit property)</a>
 
       <ul>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate.qubits">(parityos.base.gates.Gate property)</a>
 </li>
@@ -531,28 +570,34 @@
 
       <ul>
         <li><a href="api_reference/base.html#parityos.base.gates.Gate.remap">(parityos.base.gates.Gate method)</a>
 </li>
         <li><a href="api_reference/base.html#parityos.base.gates.RMixin.remap">(parityos.base.gates.RMixin method)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos.html#parityos.ParityOSOutput.replace_cnots_by_rzzs">replace_cnots_by_rzzs() (parityos.ParityOSOutput method)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.gates.RMixin">RMixin (class in parityos.base.gates)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.gates.Rx">Rx (class in parityos.base.gates)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.Rxx">Rxx (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.gates.Ry">Ry (class in parityos.base.gates)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.Ryy">Ryy (class in parityos.base.gates)</a>
+</li>
       <li><a href="api_reference/base.html#parityos.base.gates.Rz">Rz (class in parityos.base.gates)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.gates.Rzz">Rzz (class in parityos.base.gates)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.Rzzzz">Rzzzz (class in parityos.base.gates)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/base.html#parityos.base.utils.JSONLoadSaveMixin.save">save() (parityos.base.utils.JSONLoadSaveMixin method)</a>
@@ -565,20 +610,24 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.spin_hamiltonians.spinz_to_constraint">spinz_to_constraint() (in module parityos_addons.spin_hamiltonians)</a>
 </li>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.spin_hamiltonians.spinz_to_hamiltonian">spinz_to_hamiltonian() (in module parityos_addons.spin_hamiltonians)</a>
 </li>
       <li><a href="api_reference/parityos.html#parityos.CompilerClient.submit">submit() (parityos.CompilerClient method)</a>
 </li>
+      <li><a href="api_reference/base.html#parityos.base.gates.Swap">Swap (class in parityos.base.gates)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="T">T</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api_reference/base.html#parityos.base.gates.Gate1.target_qubit">target_qubit (parityos.base.gates.Gate1 property)</a>
+</li>
       <li><a href="api_reference/parityos.html#parityos.ProblemRepresentation.terms">terms (parityos.ProblemRepresentation property)</a>
 </li>
       <li><a href="api_reference/parityos_addons.html#parityos_addons.interfaces.CirqExporter.to_cirq">to_cirq() (parityos_addons.interfaces.CirqExporter method)</a>
 </li>
       <li><a href="api_reference/base.html#parityos.base.circuit.Circuit.to_json">to_json() (parityos.base.circuit.Circuit method)</a>
 
       <ul>
```

#### html2text {}

```diff
@@ -8,46 +8,56 @@
     * _T_h_e_ _P_a_r_i_t_y_ _D_e_c_o_d_e_r
     * _S_o_l_v_i_n_g_ _O_p_t_i_m_i_z_a_t_i_o_n_ _P_r_o_b_l_e_m_s
     * _A_P_I_ _R_e_f_e_r_e_n_c_e
 _P_a_r_i_t_y_O_S
     * Index
 ===============================================================================
 ************ IInnddeexx ************
-___ | _CC | _DD | _EE | _FF | _GG | _HH | _II | _JJ | _LL | _MM | _PP | _QQ | _RR | _SS | _TT | _UU | _XX | _YY | _ZZ
+___ | _AA | _CC | _DD | _EE | _FF | _GG | _HH | _II | _JJ | _LL | _MM | _PP | _QQ | _RR | _SS | _TT | _UU | _XX | _YY |
+_ZZ
 ********** __ **********
     * _____i_n_i_t_____(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._P_a_r_i_t_y_C_o_n_s_t_r_a_i_n_t_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._C_C_N_O_T_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._C_N_O_T_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._C_Z_ _m_e_t_h_o_d_)
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._C_C_M_i_x_i_n_ _m_e_t_h_o_d_)
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._C_M_i_x_i_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_1_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_2_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_3_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_4_ _m_e_t_h_o_d_)
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._M_u_l_t_i_C_o_n_t_r_o_l_M_i_x_i_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_._M_a_p_p_i_n_g_s_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_._P_a_r_i_t_y_M_a_p_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._H_a_m_i_l_t_o_n_i_a_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._Q_u_b_i_t_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._R_e_c_t_a_n_g_u_l_a_r_A_n_a_l_o_g_D_e_v_i_c_e_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._R_e_c_t_a_n_g_u_l_a_r_D_i_g_i_t_a_l_D_e_v_i_c_e_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._C_i_r_q_E_x_p_o_r_t_e_r_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._Q_i_s_k_i_t_E_x_p_o_r_t_e_r_ _m_e_t_h_o_d_)
+********** AA **********
+    * _a_p_p_e_n_d___q_i_s_k_i_t___g_a_t_e_(_)_ _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._Q_i_s_k_i_t_E_x_p_o_r_t_e_r_ _m_e_t_h_o_d_)
 ********** CC **********
-    * _C_C_N_O_T_ _(_c_l_a_s_s_ _i_n                 * _c_o_m_p_i_l_e_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
-      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)              _m_e_t_h_o_d_)
-    * _C_i_r_c_u_i_t_ _(_c_l_a_s_s_ _i_n               * _C_o_m_p_i_l_e_r_C_l_i_e_n_t_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_)
-      _p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_)          * _c_o_n_v_e_r_t___c_n_o_t_s___t_o___r_z_z_s_(_)_ _(_i_n_ _m_o_d_u_l_e
-    * _C_i_r_q_E_x_p_o_r_t_e_r_ _(_c_l_a_s_s_ _i_n            _p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_)
-      _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_)     * _c_r_e_a_t_e___d_e_f_a_u_l_t___p_r_o_b_l_e_m___c_i_r_c_u_i_t_(_)_ 
-    * _C_N_O_T_ _(_c_l_a_s_s_ _i_n                    _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _m_e_t_h_o_d_)
-      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)            * _C_Z_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _C_C_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n                     * _C_o_m_p_i_l_e_r_C_l_i_e_n_t_ _(_c_l_a_s_s_ _i_n
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)                    _p_a_r_i_t_y_o_s_)
+    * _C_C_N_O_T_ _(_c_l_a_s_s_ _i_n                       * _c_o_n_v_e_r_t___c_n_o_t_s___t_o___r_z_z_s_(_)_ _(_i_n
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)                    _m_o_d_u_l_e_ _p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_)
+    * _C_H_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)     * _c_r_e_a_t_e___d_e_f_a_u_l_t___p_r_o_b_l_e_m___c_i_r_c_u_i_t_(_)_ 
+    * _C_i_r_c_u_i_t_ _(_c_l_a_s_s_ _i_n                       _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _m_e_t_h_o_d_)
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_)                * _C_R_x_ _(_c_l_a_s_s_ _i_n
+    * _C_i_r_q_E_x_p_o_r_t_e_r_ _(_c_l_a_s_s_ _i_n                  _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_)           * _C_R_y_ _(_c_l_a_s_s_ _i_n
+    * _C_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n                        _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)                  * _C_R_z_ _(_c_l_a_s_s_ _i_n
+    * _C_N_O_T_ _(_c_l_a_s_s_ _i_n                          _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)                  * _C_Y_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _c_o_m_p_i_l_e_(_)_                             * _C_Z_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t_ _m_e_t_h_o_d_)
 ********** DD **********
     * _d_e_c_o_d_e_(_)_                                                      * _d_i_c_t___f_i_l_t_e_r_(_)_ _(_i_n
       _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r_._P_a_r_i_t_y_D_e_c_o_d_e_r_E_x_t_e_n_s_i_o_n       _m_o_d_u_l_e
       _m_e_t_h_o_d_)                                                         _p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_)
 ********** EE **********
     * _e_n_c_o_d_e_(_)_                                                      * _e_r_r_o_r___c_o_r_r_e_c_t_(_)_ 
       _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___e_n_c_o_d_e_r_._P_a_r_i_t_y_E_n_c_o_d_e_r_E_x_t_e_n_s_i_o_n       _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r_._P_a_r_i_t_y_D_e_c_o_d_e_r_E_x_t_e_n_s_i_o_n
@@ -56,66 +66,71 @@
     * _E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_)       * _e_v_a_l_u_a_t_e___p_a_r_i_t_y_(_)_ _(_i_n_ _m_o_d_u_l_e_ _p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_)
 ********** FF **********
     * _f_r_o_m___j_s_o_n_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _c_l_a_s_s        * _f_r_o_m___n_x___g_r_a_p_h_(_)_ 
       _m_e_t_h_o_d_)                                                   _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t       _c_l_a_s_s_ _m_e_t_h_o_d_)
             _c_l_a_s_s_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_._J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_ _c_l_a_s_s
             _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_._M_a_p_p_i_n_g_s_ _c_l_a_s_s
             _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_._P_a_r_i_t_y_M_a_p_ _c_l_a_s_s
             _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._Q_u_b_i_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)
 ********** GG **********
-    * _G_a_t_e_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)            * _g_e_n_e_r_a_t_e___q_a_o_a_(_)_ _(_i_n_ _m_o_d_u_l_e
-    * _G_a_t_e_1_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)             _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._q_a_o_a_)
-    * _G_a_t_e_2_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)           * _g_e_t___c_o_m_p_i_l_e_r___r_u_n_s_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
-    * _G_a_t_e_3_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)             _m_e_t_h_o_d_)
-    * _G_a_t_e_4_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)           * _g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)_ 
-    * _g_a_t_e___t_o___c_i_r_q_(_)_                                   _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)
-      _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._C_i_r_q_E_x_p_o_r_t_e_r             o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                              o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._H_e_r_m_i_t_i_a_n_G_a_t_e_M_i_x_i_n
-    * _g_a_t_e___t_o___q_i_s_k_i_t_(_)_                                       _m_e_t_h_o_d_)
-      _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._Q_i_s_k_i_t_E_x_p_o_r_t_e_r           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                        * _g_e_t___s_o_l_u_t_i_o_n_s_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
-    * _g_e_n_e_r_a_t_e___f_l_a_t___g_a_t_e___s_e_q_u_e_n_c_e_(_)_                    _m_e_t_h_o_d_)
-      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)         * _g_e_t___s_u_b_m_i_s_s_i_o_n_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
-                                                       _m_e_t_h_o_d_)
+    * _G_a_t_e_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)          * _g_e_n_e_r_a_t_e___q_a_o_a_(_)_ _(_i_n_ _m_o_d_u_l_e
+    * _G_a_t_e_1_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)           _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._q_a_o_a_)
+    * _G_a_t_e_2_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)         * _g_e_t___c_o_m_p_i_l_e_r___r_u_n_s_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
+    * _G_a_t_e_3_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)           _m_e_t_h_o_d_)
+    * _G_a_t_e_4_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)         * _g_e_t___h_e_r_m_i_t_i_a_n___c_o_n_j_u_g_a_t_e_(_)_ 
+    * _g_a_t_e___t_o___c_i_r_q_(_)_                                 _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)
+      _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._C_i_r_q_E_x_p_o_r_t_e_r           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                            o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._H_e_r_m_i_t_i_a_n_G_a_t_e_M_i_x_i_n
+    * _g_e_n_e_r_a_t_e___f_l_a_t___g_a_t_e___s_e_q_u_e_n_c_e_(_)_                        _m_e_t_h_o_d_)
+      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)             o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
+                                                   * _g_e_t___s_o_l_u_t_i_o_n_s_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
+                                                     _m_e_t_h_o_d_)
+                                                   * _g_e_t___s_u_b_m_i_s_s_i_o_n_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
+                                                     _m_e_t_h_o_d_)
 ********** HH **********
     * _H_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)     * _H_a_m_i_l_t_o_n_i_a_n_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_)
                                            * _H_e_r_m_i_t_i_a_n_G_a_t_e_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n
                                              _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
 ********** II **********
-    * _i_s___s_a_t_i_s_f_i_e_d_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t_ _m_e_t_h_o_d_)
+    * _i_s___s_a_t_i_s_f_i_e_d_(_)_                                    * _I_S_w_a_p_ _(_c_l_a_s_s_ _i_n
+      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t       _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _m_e_t_h_o_d_)
 ********** JJ **********
     * _j_s_o_n___w_r_a_p_(_)_ _(_i_n_ _m_o_d_u_l_e     * _J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n
       _p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_)         _p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_)
 ********** LL **********
     * _l_o_a_d_(_)_                                     * _l_o_g_i_c_a_l___d_e_g_e_n_e_r_a_c_i_e_s_ 
       _(_p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_._J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n       _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_._M_a_p_p_i_n_g_s
       _c_l_a_s_s_ _m_e_t_h_o_d_)                                _p_r_o_p_e_r_t_y_)
                                                  * _l_o_g_i_c_a_l___p_r_o_b_l_e_m___c_i_r_c_u_i_t_ 
                                                    _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _p_r_o_p_e_r_t_y_)
 ********** MM **********
-    * _m_a_k_e___a_r_g_s_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
-    * _m_a_k_e___f_u_l_l___c_o_n_f_i_g_u_r_a_t_i_o_n___f_r_o_m___p_a_r_t_i_a_l_(_)_ 
-      _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r_._P_a_r_i_t_y_D_e_c_o_d_e_r_E_x_t_e_n_s_i_o_n_ _m_e_t_h_o_d_)
-    * _M_a_p_p_i_n_g_s_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_)
-    * _m_o_d_i_f_y___a_n_g_l_e_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
-    * module
-          o _p_a_r_i_t_y_o_s
-          o _p_a_r_i_t_y_o_s_._a_p_i___i_n_t_e_r_f_a_c_e
+    * _m_a_k_e___a_r_g_s_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)                 * _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_H_ 
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)                       _(_c_l_a_s_s_ _i_n
+    * _m_a_k_e___a_r_g_s___a_n_d___k_w_a_r_g_s___f_r_o_m___j_s_o_n_(_)_                                _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _s_t_a_t_i_c_ _m_e_t_h_o_d_)                      * _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_x_ 
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)                 _(_c_l_a_s_s_ _i_n
+    * _m_a_k_e___f_u_l_l___c_o_n_f_i_g_u_r_a_t_i_o_n___f_r_o_m___p_a_r_t_i_a_l_(_)_                          _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r_._P_a_r_i_t_y_D_e_c_o_d_e_r_E_x_t_e_n_s_i_o_n     * _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_y_ 
+      _m_e_t_h_o_d_)                                                         _(_c_l_a_s_s_ _i_n
+    * _M_a_p_p_i_n_g_s_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s_)                 _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _m_o_d_i_f_y___a_n_g_l_e_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)         * _M_u_l_t_i_C_o_n_t_r_o_l_l_e_d_R_z_ 
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)                         _(_c_l_a_s_s_ _i_n
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)                       _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * module                                                        * _M_u_l_t_i_C_o_n_t_r_o_l_M_i_x_i_n_ 
+          o _p_a_r_i_t_y_o_s                                                  _(_c_l_a_s_s_ _i_n
+          o _p_a_r_i_t_y_o_s_._a_p_i___i_n_t_e_r_f_a_c_e                                    _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
           o _p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t
           o _p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s
           o _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s
           o _p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s
           o _p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._m_a_p_p_i_n_g_s
           o _p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r
           o _p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___e_n_c_o_d_e_r
@@ -148,40 +163,47 @@
           o _m_o_d_u_l_e
     * parityos.base.utils
           o _m_o_d_u_l_e
 ********** QQ **********
     * _Q_i_s_k_i_t_E_x_p_o_r_t_e_r_ _(_c_l_a_s_s_ _i_n        * _q_u_b_i_t_s_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t
       _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_)       _p_r_o_p_e_r_t_y_)
     * _Q_u_b_i_t_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_)             o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e
-    * _q_u_b_i_t_                                   _p_r_o_p_e_r_t_y_)
-      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_1            o _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n
-      _p_r_o_p_e_r_t_y_)                               _p_r_o_p_e_r_t_y_)
+                                              _p_r_o_p_e_r_t_y_)
+                                            o _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n
+                                              _p_r_o_p_e_r_t_y_)
 ********** RR **********
-    * _R_e_c_t_a_n_g_u_l_a_r_A_n_a_l_o_g_D_e_v_i_c_e_ _(_c_l_a_s_s_ _i_n     * _r_e_p_l_a_c_e___c_n_o_t_s___b_y___r_z_z_s_(_)_ 
-      _p_a_r_i_t_y_o_s_)                               _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _m_e_t_h_o_d_)
-    * _R_e_c_t_a_n_g_u_l_a_r_D_i_g_i_t_a_l_D_e_v_i_c_e_ _(_c_l_a_s_s       * _R_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n
-      _i_n_ _p_a_r_i_t_y_o_s_)                            _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
-    * _r_e_m_a_p_(_)_                               * _R_x_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
-      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t        * _R_y_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _R_e_c_t_a_n_g_u_l_a_r_A_n_a_l_o_g_D_e_v_i_c_e_ _(_c_l_a_s_s_ _i_n     * _R_x_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _p_a_r_i_t_y_o_s_)                             * _R_x_x_ _(_c_l_a_s_s_ _i_n
+    * _R_e_c_t_a_n_g_u_l_a_r_D_i_g_i_t_a_l_D_e_v_i_c_e_ _(_c_l_a_s_s         _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+      _i_n_ _p_a_r_i_t_y_o_s_)                          * _R_y_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _r_e_m_a_p_(_)_                               * _R_y_y_ _(_c_l_a_s_s_ _i_n
+      _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t          _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
       _m_e_t_h_o_d_)                               * _R_z_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e       * _R_z_z_ _(_c_l_a_s_s_ _i_n
             _m_e_t_h_o_d_)                           _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
-          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n
-            _m_e_t_h_o_d_)
+          o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n     * _R_z_z_z_z_ _(_c_l_a_s_s_ _i_n
+            _m_e_t_h_o_d_)                           _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
+    * _r_e_p_l_a_c_e___c_n_o_t_s___b_y___r_z_z_s_(_)_ 
+      _(_p_a_r_i_t_y_o_s_._P_a_r_i_t_y_O_S_O_u_t_p_u_t_ _m_e_t_h_o_d_)
+    * _R_M_i_x_i_n_ _(_c_l_a_s_s_ _i_n
+      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
 ********** SS **********
     * _s_a_v_e_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_._J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n_ _m_e_t_h_o_d_)         * _s_p_i_n_z___t_o___c_o_n_s_t_r_a_i_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e
     * _s_e_l_e_c_t___r_e_d_u_c_e_d___r_e_a_d_o_u_t___q_u_b_i_t_s_(_)_                                 _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._s_p_i_n___h_a_m_i_l_t_o_n_i_a_n_s_)
       _(_p_a_r_i_t_y_o_s_._e_n_c_o_d_i_n_g_s_._p_a_r_i_t_y___d_e_c_o_d_e_r_._P_a_r_i_t_y_D_e_c_o_d_e_r_E_x_t_e_n_s_i_o_n     * _s_p_i_n_z___t_o___h_a_m_i_l_t_o_n_i_a_n_(_)_ _(_i_n_ _m_o_d_u_l_e
       _m_e_t_h_o_d_)                                                         _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._s_p_i_n___h_a_m_i_l_t_o_n_i_a_n_s_)
     * _S_p_i_n_Z_ _(_c_l_a_s_s_ _i_n_ _p_a_r_i_t_y_o_s___a_d_d_o_n_s_._s_p_i_n___h_a_m_i_l_t_o_n_i_a_n_s_)            * _s_u_b_m_i_t_(_)_ _(_p_a_r_i_t_y_o_s_._C_o_m_p_i_l_e_r_C_l_i_e_n_t
                                                                       _m_e_t_h_o_d_)
+                                                                    * _S_w_a_p_ _(_c_l_a_s_s_ _i_n
+                                                                      _p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_)
 ********** TT **********
-    * _t_e_r_m_s_ _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n_ _p_r_o_p_e_r_t_y_)         * _t_o___q_i_s_k_i_t_(_)_ 
-    * _t_o___c_i_r_q_(_)_ _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._C_i_r_q_E_x_p_o_r_t_e_r        _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._Q_i_s_k_i_t_E_x_p_o_r_t_e_r
-      _m_e_t_h_o_d_)                                                   _m_e_t_h_o_d_)
+    * _t_a_r_g_e_t___q_u_b_i_t_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_1_ _p_r_o_p_e_r_t_y_)       * _t_o___q_i_s_k_i_t_(_)_ 
+    * _t_e_r_m_s_ _(_p_a_r_i_t_y_o_s_._P_r_o_b_l_e_m_R_e_p_r_e_s_e_n_t_a_t_i_o_n_ _p_r_o_p_e_r_t_y_)           _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._Q_i_s_k_i_t_E_x_p_o_r_t_e_r
+    * _t_o___c_i_r_q_(_)_ _(_p_a_r_i_t_y_o_s___a_d_d_o_n_s_._i_n_t_e_r_f_a_c_e_s_._C_i_r_q_E_x_p_o_r_t_e_r        _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)
     * _t_o___j_s_o_n_(_)_ _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_i_r_c_u_i_t_._C_i_r_c_u_i_t_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._c_o_n_s_t_r_a_i_n_t_s_._E_q_u_a_l_i_t_y_C_o_n_s_t_r_a_i_n_t
             _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._G_a_t_e_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._g_a_t_e_s_._R_M_i_x_i_n_ _m_e_t_h_o_d_)
           o _(_p_a_r_i_t_y_o_s_._b_a_s_e_._u_t_i_l_s_._J_S_O_N_L_o_a_d_S_a_v_e_M_i_x_i_n
             _m_e_t_h_o_d_)
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/index.html` & `parityos-2.5.0/parityos_addons/documentation/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
+        <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installation" href="installation.html" /> 
 </head>
 
 <body class="wy-body-for-nav">
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/installation.html` & `parityos-2.5.0/parityos_addons/documentation/html/installation.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Quickstart" href="quickstart.html" />
     <link rel="prev" title="Welcome to ParityOS’s documentation!" href="index.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/parity_decoder.html` & `parityos-2.5.0/parityos_addons/documentation/html/parity_decoder.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Solving Optimization Problems" href="tutorial.html" />
     <link rel="prev" title="Asynchronous submissions" href="asynchronous_submission.html" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/py-modindex.html` & `parityos-2.5.0/parityos_addons/documentation/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/quickstart.html` & `parityos-2.5.0/parityos_addons/documentation/html/quickstart.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
         <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Making a custom device model" href="custom_device_models.html" />
     <link rel="prev" title="Installation" href="installation.html" />
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/search.html` & `parityos-2.5.0/parityos_addons/documentation/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" /> 
 </head>
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/searchindex.js` & `parityos-2.5.0/parityos_addons/documentation/html/searchindex.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1098 +1,629 @@
 Search.setIndex({
+    "alltitles": {
+        "API Reference": [
+            [3, "api-reference"]
+        ],
+        "Analog device model": [
+            [7, "analog-device-model"]
+        ],
+        "Asynchronous submissions": [
+            [6, "asynchronous-submissions"]
+        ],
+        "Basic example": [
+            [10, "basic-example"]
+        ],
+        "Classical Optimization": [
+            [12, "classical-optimization"]
+        ],
+        "Contents:": [
+            [8, null]
+        ],
+        "Defining a Target Device": [
+            [11, "defining-a-target-device"]
+        ],
+        "Defining an optimization problem": [
+            [11, "defining-an-optimization-problem"]
+        ],
+        "Device models": [
+            [7, "device-models"]
+        ],
+        "Digital device model": [
+            [7, "digital-device-model"]
+        ],
+        "Error correction": [
+            [10, "error-correction"]
+        ],
+        "Examples": [
+            [6, "examples"],
+            [11, "examples"]
+        ],
+        "Initializing the Client": [
+            [11, "initializing-the-client"]
+        ],
+        "Installation": [
+            [9, "installation"]
+        ],
+        "Making a custom device model": [
+            [7, "making-a-custom-device-model"]
+        ],
+        "Obtaining results": [
+            [6, "obtaining-results"]
+        ],
+        "Parity Mapping and Compilation": [
+            [12, "parity-mapping-and-compilation"]
+        ],
+        "Problem Formulation": [
+            [12, "problem-formulation"]
+        ],
+        "QAOA Optimization and Simulation": [
+            [12, "qaoa-optimization-and-simulation"]
+        ],
+        "Quickstart": [
+            [11, "quickstart"]
+        ],
+        "Reduced read-out": [
+            [10, "reduced-read-out"]
+        ],
+        "Selecting qubits for read-out": [
+            [10, "selecting-qubits-for-read-out"]
+        ],
+        "Solutions of the QAOA algorithm and decoding": [
+            [12, "solutions-of-the-qaoa-algorithm-and-decoding"]
+        ],
+        "Solving Optimization Problems": [
+            [12, "solving-optimization-problems"]
+        ],
+        "Submission": [
+            [6, "submission"]
+        ],
+        "Submitting a Job to the Compiler": [
+            [11, "submitting-a-job-to-the-compiler"]
+        ],
+        "The Parity Decoder": [
+            [10, "the-parity-decoder"]
+        ],
+        "The ParityOS output": [
+            [11, "the-parityos-output"]
+        ],
+        "The QAOA circuit": [
+            [12, "the-qaoa-circuit"]
+        ],
+        "Welcome to ParityOS\u2019s documentation!": [
+            [8, "welcome-to-parityos-s-documentation"]
+        ],
+        "parityos": [
+            [4, "module-parityos"]
+        ],
+        "parityos.api_interface": [
+            [0, "module-parityos.api_interface"]
+        ],
+        "parityos.base": [
+            [1, "module-parityos.base.constraints"]
+        ],
+        "parityos.encodings": [
+            [2, "module-parityos.encodings.mappings"]
+        ],
+        "parityos_addons": [
+            [5, "module-parityos_addons.interfaces"]
+        ]
+    },
     "docnames": ["api_reference/api_interface", "api_reference/base", "api_reference/encodings", "api_reference/index", "api_reference/parityos", "api_reference/parityos_addons", "asynchronous_submission", "custom_device_models", "index", "installation", "parity_decoder", "quickstart", "tutorial"],
+    "envversion": {
+        "sphinx": 61,
+        "sphinx.domains.c": 3,
+        "sphinx.domains.changeset": 1,
+        "sphinx.domains.citation": 1,
+        "sphinx.domains.cpp": 9,
+        "sphinx.domains.index": 1,
+        "sphinx.domains.javascript": 3,
+        "sphinx.domains.math": 2,
+        "sphinx.domains.python": 4,
+        "sphinx.domains.rst": 2,
+        "sphinx.domains.std": 2
+    },
     "filenames": ["api_reference/api_interface.rst", "api_reference/base.rst", "api_reference/encodings.rst", "api_reference/index.rst", "api_reference/parityos.rst", "api_reference/parityos_addons.rst", "asynchronous_submission.rst", "custom_device_models.rst", "index.rst", "installation.rst", "parity_decoder.rst", "quickstart.rst", "tutorial.rst"],
-    "titles": ["parityos.api_interface", "parityos.base", "parityos.encodings", "API Reference", "parityos", "parityos_addons", "Asynchronous submissions", "Making a custom device model", "Welcome to ParityOS\u2019s documentation!", "Installation", "The Parity Decoder", "Quickstart", "Solving Optimization Problems"],
-    "terms": {
-        "class": [1, 2, 4, 5, 7, 11, 12],
-        "constraint": [1, 2, 4, 5, 7, 10, 11, 12],
-        "equalityconstraint": [1, 4, 5],
-        "oper": [1, 4, 5],
-        "iter": [1, 4, 5, 11],
-        "qubit": [1, 2, 4, 5, 6, 7, 11, 12],
-        "valu": [1, 2, 4, 5, 7, 10, 12],
-        "int": [1, 2, 4, 5, 12],
-        "repres": [1, 2, 4, 5, 11, 12],
-        "an": [1, 4, 5, 6, 7, 9, 10, 12],
-        "equal": [1, 2, 4],
-        "form": [1, 4, 5, 10, 11, 12],
-        "s_1": [1, 11, 12],
-        "cdot": [1, 11],
-        "s_2": [1, 11],
-        "dot": [1, 7, 12],
-        "s_n": 1,
-        "pm": 1,
-        "1": [1, 2, 4, 5, 6, 7, 10, 11, 12],
-        "where": [1, 2, 4, 5, 6, 7, 10, 11, 12],
-        "ar": [1, 2, 4, 5, 7, 9, 10, 11, 12],
-        "spin": [1, 2, 4, 5, 11, 12],
-        "variabl": [1, 4, 10, 11, 12],
-        "__init__": [1, 2, 4, 5],
-        "paramet": [1, 2, 4, 5, 7, 12],
-        "The": [1, 2, 4, 5, 6, 7, 8],
-        "defin": [1, 4, 5, 7, 12],
-        "given": [1, 2, 4, 5, 10, 11, 12],
-        "collect": [1, 4, 7, 11],
-        "i": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
-        "product": [1, 4, 5, 11, 12],
-        "z": [1, 2, 4, 5, 7, 12],
-        "each": [1, 2, 4, 5, 7, 9, 10, 11, 12],
-        "pariti": [1, 2, 4, 5, 8, 11],
-        "must": [1, 4, 5],
-        "classmethod": [1, 2, 4],
-        "from_json": [1, 2, 4],
-        "constraint_data": 1,
-        "sequenc": [1, 2, 4, 5, 11],
-        "str": [1, 2, 4, 5, 12],
-        "float": [1, 2, 4, 5],
-        "bool": [1, 2, 4],
-        "none": [1, 2, 4, 5, 12],
-        "dict": [1, 2, 4, 5],
-        "jsontyp": [1, 2, 4],
-        "list": [1, 2, 4, 5, 6, 7, 10, 11],
-        "self": [1, 2, 4],
-        "initi": [1, 2, 4, 6, 12],
-        "object": [1, 2, 4, 5, 6, 10, 11],
-        "from": [1, 2, 4, 5, 6, 7, 10, 11, 12],
-        "json": [1, 2, 4],
-        "format": [1, 2, 4, 12],
-        "return": [1, 2, 4, 5, 6, 10, 11, 12],
-        "instanc": [1, 2, 4, 5, 12],
-        "is_satisfi": 1,
-        "configur": [1, 2, 4, 10, 12],
-        "evalu": [1, 4, 12],
-        "whether": 1,
-        "satisfi": [1, 2, 4, 10, 12],
-        "A": [1, 2, 4, 5, 7, 11, 12],
-        "map": [1, 2, 4, 5, 11],
-        "onto": [1, 5, 11],
-        "eigenvalu": [1, 5],
-        "all": [1, 2, 4, 5, 6, 7, 10, 11, 12],
-        "present": 1,
-        "true": [1, 2, 4, 12],
-        "fals": [1, 2],
-        "otherwis": [1, 4],
-        "to_json": [1, 2, 4],
-        "convert": [1, 2, 4, 5, 12],
-        "parityconstraint": [1, 4, 11],
-        "deprec": [1, 4],
-        "version": [1, 4, 11, 12],
-        "which": [1, 2, 4, 6, 7, 10, 11, 12],
-        "mean": [1, 4, 6],
-        "condit": [1, 4],
-        "make": [1, 4, 6, 8, 10, 11],
-        "up": [1, 2, 12],
-        "thi": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
-        "evaluate_par": 1,
-        "pauli": [1, 4, 5],
-        "either": [1, 2, 4, 5, 7],
-        "contain": [1, 2, 4, 5, 10, 11, 12],
-        "circuit": [1, 4, 5, 11],
-        "gate": [1, 4, 5, 7, 11, 12],
-        "data": [1, 2, 4, 6],
-        "creat": [1, 4, 5, 7, 9, 11, 12],
-        "element": [1, 6, 7],
-        "generate_flat_gate_sequ": 1,
-        "gener": [1, 2, 4, 5, 12],
-        "its": [1, 5],
-        "subcircuit": 1,
-        "loop": 1,
-        "over": [1, 11, 12],
-        "get_hermitian_conjug": 1,
-        "hermitian": 1,
-        "conjug": 1,
-        "invers": 1,
-        "new": [1, 4, 7],
-        "modify_angl": 1,
-        "angle_map": 1,
-        "frozenset": [1, 2, 4, 5],
-        "gate_typ": 1,
-        "type": [1, 4, 7],
-        "rmixin": 1,
-        "parameter_nam": [1, 5],
-        "same": [1, 4, 5, 6, 12],
-        "one": [1, 2, 4, 6, 7, 9, 12],
-        "except": [1, 4, 6],
-        "rotat": [1, 4],
-        "angl": [1, 4],
-        "chang": 1,
-        "function": [1, 4, 6, 12],
-        "": [1, 10, 11],
-        "act": 1,
-        "If": [1, 2, 4, 5, 7, 10, 11],
-        "includ": [1, 2, 4, 6, 11],
-        "left": [1, 5, 7, 12],
-        "unchang": 1,
-        "specifi": [1, 4, 7, 10, 12],
-        "might": [1, 4, 12],
-        "affect": 1,
-        "name": [1, 5, 9, 12],
-        "also": [1, 4, 6, 7, 10, 11, 12],
-        "without": 1,
-        "provid": [1, 4, 7, 11, 12],
-        "set": [1, 2, 4, 7, 10, 11, 12],
-        "option": [1, 2, 4, 5, 9, 11, 12],
-        "onli": [1, 2, 5, 6, 7, 9, 10, 12],
-        "updat": [1, 4, 12],
-        "other": [1, 4, 5, 12],
-        "copi": [1, 4, 11],
-        "default": [1, 2, 4, 6, 7, 11, 12],
-        "current": [1, 12],
-        "select": [1, 2, 12],
-        "have": [1, 2, 4, 6, 7, 11, 12],
-        "been": [1, 4, 6, 12],
-        "modifi": 1,
-        "properti": [1, 2, 4],
-        "string": [1, 4, 5, 7],
-        "remap": 1,
-        "context": 1,
-        "kwarg": [1, 4],
-        "ha": [1, 2, 4, 5, 7, 9, 10, 11, 12],
-        "appli": [1, 2, 10, 12],
-        "parametr": [1, 4, 12],
-        "see": [1, 6, 7, 9, 11, 12],
-        "detail": [1, 11],
-        "number": [1, 2, 4, 5, 12],
-        "like": [1, 2, 4, 5, 6, 11],
-        "convert_cnots_to_rzz": 1,
-        "zz": [1, 4],
-        "instead": [1, 2, 4, 5, 11],
-        "cnot": [1, 4, 7, 11],
-        "replac": [1, 4],
-        "standard": [1, 2, 4, 7, 9, 11],
-        "optim": [1, 4, 5, 6, 7, 8, 10],
-        "equival": [1, 2, 11],
-        "implement": [1, 4, 7, 11, 12],
-        "local": [1, 4, 7, 11, 12],
-        "result": [1, 4, 7, 10, 11, 12],
-        "addit": [1, 5],
-        "account": 1,
-        "necessari": [1, 4],
-        "rx": [1, 4],
-        "ry": 1,
-        "rz": [1, 4],
-        "moment": 1,
-        "ccnot": 1,
-        "control_1": 1,
-        "control_2": 1,
-        "target": [1, 4, 12],
-        "first": [1, 5, 7, 11, 12],
-        "control": 1,
-        "z_control_1": 1,
-        "second": [1, 4, 5, 12],
-        "z_control_2": 1,
-        "flip": 1,
-        "z_control": 1,
-        "cz": 1,
-        "phase": 1,
-        "qubit_arg": 1,
-        "inherit": 1,
-        "subclass": 1,
-        "intend": 1,
-        "store": [1, 6, 10, 11],
-        "inform": [1, 4, 5, 6, 7, 9, 10, 11, 12],
-        "receiv": [1, 11],
-        "compil": [1, 2, 4, 5, 6, 7, 10],
-        "thei": [1, 4, 12],
-        "do": [1, 4, 6, 7, 10, 11],
-        "ani": [1, 2, 4, 6, 10, 12],
-        "method": [1, 2, 4, 5, 10, 11, 12],
-        "simul": [1, 10],
-        "nor": 1,
-        "anti": 1,
-        "commut": [1, 12],
-        "relat": [1, 4, 5, 9],
-        "between": [1, 4, 11, 12],
-        "them": [1, 4, 11, 12],
-        "mathemat": 1,
-        "For": [1, 4, 6, 7, 9, 10, 11, 12],
-        "those": 1,
-        "us": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
-        "we": [1, 2, 6, 7, 10, 11, 12],
-        "recommend": [1, 7, 9],
-        "more": [1, 9, 11, 12],
-        "elabor": 1,
-        "framework": [1, 12],
-        "qutip": 1,
-        "cirq": [1, 5, 9, 12],
-        "qiskit": [1, 5, 9, 12],
-        "compat": [1, 4],
-        "make_arg": 1,
-        "tupl": [1, 4, 5],
-        "argument": [1, 4],
-        "would": [1, 4, 6, 7],
-        "need": [1, 6, 7, 9, 11, 12],
-        "instanti": [1, 5, 12],
-        "doe": [1, 2, 7, 10, 11],
-        "keyword": 1,
-        "arg": [1, 4],
-        "get": [1, 4, 6, 7, 12],
-        "subject": 1,
-        "simpl": 1,
-        "possibl": [1, 2, 4, 6, 7, 10, 11, 12],
-        "about": [1, 4, 5, 6, 9, 11],
-        "gate1": 1,
-        "singl": [1, 4, 6, 7, 10, 11, 12],
-        "gate2": 1,
-        "qubit1": 1,
-        "qubit2": 1,
-        "two": [1, 7, 10, 12],
-        "gate3": 1,
-        "qubit3": 1,
-        "three": [1, 10, 11],
-        "gate4": 1,
-        "qubit4": 1,
-        "four": [1, 11, 12],
-        "h": [1, 4, 11, 12],
-        "hadamard": [1, 4],
-        "hermitiangatemixin": 1,
-        "mixin": 1,
-        "hermitian_conjug": 1,
-        "itself": 1,
-        "attribut": [1, 4, 7, 11],
-        "label": [1, 4, 5, 7, 12],
-        "identifi": 1,
-        "multipli": [1, 2],
-        "when": [1, 2, 10, 11, 12],
-        "consid": 1,
-        "fix": [1, 4, 11],
-        "reflect": 1,
-        "output": [1, 4, 5, 10, 12],
-        "should": [1, 4, 5, 6, 7],
-        "kei": [1, 2, 4, 12],
-        "match": 1,
-        "error": [1, 2],
-        "rais": [1, 2, 6, 11],
-        "look": [1, 12],
-        "found": [1, 4, 11],
-        "correspond": [1, 2, 4, 12],
-        "interpret": [1, 4],
-        "again": 1,
-        "numpi": [1, 5, 12],
-        "even": [1, 2, 12],
-        "sympi": [1, 5],
-        "symbol": [1, 5],
-        "can": [1, 2, 4, 6, 7, 9, 10, 11, 12],
-        "Then": [1, 5, 6, 7, 11],
-        "take": [1, 7, 12],
-        "preced": 1,
-        "exampl": [1, 4, 5, 7, 12],
-        "rz_gate": 1,
-        "math": 1,
-        "pi": 1,
-        "theta": [1, 4, 5, 11],
-        "rz_theta": 1,
-        "other_paramet": 1,
-        "gamma": [1, 5, 12],
-        "divid": 1,
-        "rz_fix": 1,
-        "0": [1, 4, 6, 7, 10, 11, 12],
-        "5": [1, 4, 6, 7, 11, 12],
-        "2": [1, 4, 5, 6, 7, 11, 12],
-        "rzz": 1,
-        "x": [1, 5, 6, 11, 12],
-        "y": [1, 6, 11, 12],
-        "util": 1,
-        "jsonloadsavemixin": 1,
-        "add": [1, 5, 7, 9, 11, 12],
-        "load": [1, 11],
-        "save": [1, 12],
-        "represent": [1, 4, 5, 11, 12],
-        "file": [1, 6],
-        "write": 1,
-        "abstract": 1,
-        "construct": [1, 2, 4, 10, 12],
-        "filenam": 1,
-        "read": [1, 2, 12],
-        "builtin": 1,
-        "python": [1, 6, 9],
-        "serializ": [1, 4],
-        "dict_filt": 1,
-        "hashabl": [1, 4],
-        "filter": 1,
-        "dictionari": [1, 2, 4, 5, 10, 12],
-        "pair": [1, 4, 12],
-        "both": [1, 4, 7, 12],
-        "origin": [1, 2, 4, 11],
-        "json_wrap": 1,
-        "item": [1, 5, 12],
-        "param": [1, 5],
-        "unord": 1,
-        "e": [1, 2, 4, 7, 11, 12],
-        "g": [1, 7, 12],
-        "sort": [1, 12],
-        "alwai": [1, 4, 11, 12],
-        "note": [1, 2, 10, 12],
-        "fulli": 1,
-        "compliant": 1,
-        "translat": 1,
-        "null": 1,
-        "boolean": 1,
-        "encoding_map": [2, 11],
-        "paritymap": 2,
-        "decoding_map": [2, 11],
-        "hold": [2, 6],
-        "architectur": [2, 11, 12],
-        "decod": [2, 8],
-        "api": [2, 4, 6, 8, 11],
-        "tell": [2, 4],
-        "you": [2, 4, 6, 7, 9, 10, 11, 12],
-        "how": [2, 4, 6, 7, 9, 10, 11, 12],
-        "go": [2, 9, 10, 12],
-        "physic": [2, 4, 10, 11, 12],
-        "logic": [2, 4, 10, 11, 12],
-        "logical_degeneraci": [2, 11],
-        "degeneraci": [2, 11],
-        "symmetri": 2,
-        "hamiltonian": [2, 4, 5, 11, 12],
-        "show": [2, 7, 11, 12],
-        "entri": 2,
-        "out": [2, 7, 11],
-        "trivial": 2,
-        "facilit": 2,
-        "serial": 2,
-        "parity_encod": 2,
-        "parityencoderextens": 2,
-        "extend": [2, 4],
-        "parityosoutput": [2, 4, 5, 6, 10, 11],
-        "transform": [2, 10],
-        "system": [2, 10],
-        "bitstr": [2, 12],
-        "refer": [2, 8],
-        "parity_decod": 2,
-        "paritydecoderextens": 2,
-        "error_correct": [2, 10],
-        "select_reduced_readout_qubit": [2, 10],
-        "make_full_configuration_from_parti": 2,
-        "These": [2, 12],
-        "It": [2, 4, 6, 9, 11, 12],
-        "partial": [2, 4],
-        "full": [2, 4, 10, 11],
-        "base": [2, 3, 9, 11, 12],
-        "redund": [2, 10],
-        "offer": 2,
-        "especi": 2,
-        "limit": 2,
-        "hardwar": [2, 7, 12],
-        "setup": 2,
-        "fail": 2,
-        "some": [2, 6, 12],
-        "back": [2, 6, 12],
-        "import": [2, 5, 6, 7, 10, 11, 12],
-        "enough": [2, 10],
-        "reconstruct": 2,
-        "state": [2, 4, 10, 11, 12],
-        "parityosexcept": [2, 4, 11],
-        "devic": [2, 4, 5, 6, 8, 12],
-        "similar": [2, 6],
-        "correct": 2,
-        "nearest": [2, 11],
-        "neighbor": [2, 11],
-        "algorithm": [2, 4, 11],
-        "henc": 2,
-        "part": [2, 12],
-        "code": [2, 4, 6, 7, 11],
-        "subspac": 2,
-        "were": [2, 6, 12],
-        "obtain": [2, 4, 10, 12],
-        "smallest": 2,
-        "ham": 2,
-        "distanc": 2,
-        "return_incomplet": 2,
-        "problem": [2, 4, 5, 6, 7, 8, 9, 10],
-        "flag": 2,
-        "could": [2, 4],
-        "case": [2, 4, 6, 9, 10, 11, 12],
-        "deduc": 2,
-        "random_gener": 2,
-        "random": [2, 12],
-        "minim": [2, 10, 12],
-        "still": [2, 10],
-        "recov": [2, 10],
-        "choic": 2,
-        "librari": 2,
-        "parityo": [3, 5, 6, 7, 9, 10, 12],
-        "api_interfac": 3,
-        "encod": [3, 4, 12],
-        "parityos_addon": [3, 12],
-        "compilercli": [4, 6, 11, 12],
-        "usernam": [4, 11, 12],
-        "host": 4,
-        "parityqc": [4, 7, 11],
-        "com": 4,
-        "url_prefix": 4,
-        "v1": 4,
-        "http_retri": 4,
-        "3": [4, 5, 7, 9, 12],
-        "http_timeout": 4,
-        "10": [4, 5, 12],
-        "http_backoff_factor": 4,
-        "02": 4,
-        "intent": 4,
-        "request": [4, 6, 7],
-        "problemrepresent": [4, 5, 6, 7, 11, 12],
-        "synchron": [4, 6, 11],
-        "asynchron": [4, 8, 11],
-        "give": [4, 12],
-        "access": [4, 10, 11],
-        "servic": 4,
-        "optimization_problem": [4, 6, 7, 11, 12],
-        "device_model": [4, 6, 7, 11, 12],
-        "devicemodelbas": [4, 7],
-        "preset": [4, 7, 11],
-        "timeout": 4,
-        "900": 4,
-        "model": [4, 6, 8, 11],
-        "devicemodel": [4, 7, 11],
-        "analog_default": [4, 7],
-        "digital_default": [4, 7],
-        "avail": [4, 11, 12],
-        "everyon": 4,
-        "allow": [4, 11, 12],
-        "commun": 4,
-        "per": [4, 6, 12],
-        "custom": [4, 8, 11],
-        "basi": 4,
-        "time": [4, 5, 6, 9, 11, 12],
-        "after": [4, 6, 7, 10, 11],
-        "abort": 4,
-        "get_compiler_run": [4, 6],
-        "submission_id": [4, 6],
-        "compilerrun": [4, 6],
-        "run": [4, 6, 7, 10, 11, 12],
-        "spawn": 4,
-        "submiss": [4, 7, 8, 11],
-        "id": 4,
-        "get_solut": [4, 6],
-        "compiler_run": [4, 6],
-        "solut": [4, 6, 10],
-        "get_submiss": 4,
-        "submit": [4, 6, 7, 9, 10, 12],
-        "pass": [4, 7, 10, 11, 12],
-        "now": [4, 6, 7, 11, 12],
-        "just": [4, 7, 11],
-        "upon": [4, 7],
-        "associ": [4, 12],
-        "interact": [4, 5, 6, 7, 11, 12],
-        "coeffici": [4, 5, 6, 7, 11, 12],
-        "diagon": 4,
-        "togeth": [4, 9],
-        "align": [4, 12],
-        "work": [4, 6, 12],
-        "non": [4, 11],
-        "numer": 4,
-        "hard": [4, 12],
-        "8": [4, 7],
-        "thrown": 4,
-        "parityosimporterror": 4,
-        "importerror": 4,
-        "uninstal": 4,
-        "depend": 4,
-        "compiled_problem": [4, 11, 12],
-        "constraint_circuit": [4, 11, 12],
-        "problem_circuit": 4,
-        "driver_circuit": [4, 11],
-        "initial_state_preparation_circuit": [4, 11],
-        "produc": 4,
-        "mai": [4, 10, 11, 12],
-        "extra": 4,
-        "featur": [4, 7, 9],
-        "futur": [4, 12],
-        "digit": [4, 11, 12],
-        "z_1": [4, 11],
-        "z_2": [4, 11],
-        "z_3": [4, 11],
-        "z_4": [4, 11],
-        "analog": [4, 6, 11, 12],
-        "driver": [4, 5, 11, 12],
-        "prepar": 4,
-        "start": [4, 7, 11, 12],
-        "comput": [4, 7, 10, 11, 12],
-        "langl": [4, 12],
-        "k": [4, 12],
-        "normal": [4, 12],
-        "qaoa": [4, 5, 11],
-        "want": [4, 7, 9, 10, 11, 12],
-        "so": [4, 6, 7, 12],
-        "combin": [4, 12],
-        "execut": [4, 11, 12],
-        "exact": 4,
-        "create_default_problem_circuit": 4,
-        "exp": [4, 12],
-        "mbox": 4,
-        "absorb": 4,
-        "separ": 4,
-        "exponenti": 4,
-        "encode_problem": 4,
-        "problem_represent": [4, 11],
-        "express": [4, 5, 12],
-        "term": [4, 5, 11, 12],
-        "whose": [4, 11],
-        "ones": 4,
-        "respons": [4, 5],
-        "schema": [4, 5],
-        "logical_problem_circuit": 4,
-        "replace_cnots_by_rzz": 4,
-        "nativ": [4, 11, 12],
-        "place": 4,
-        "repackag": 4,
-        "bodi": [4, 5, 7, 11, 12],
-        "constraint_strength": [4, 12],
-        "inf": 4,
-        "particular": 4,
-        "paritydecod": [4, 10],
-        "strength": [4, 11],
-        "By": [4, 12],
-        "In": [4, 6, 7, 11, 12],
-        "violat": [4, 12],
-        "unconstrain": [4, 12],
-        "energi": [4, 12],
-        "zero": [4, 12],
-        "check": 4,
-        "soft": 4,
-        "bonu": 4,
-        "proport": 4,
-        "valid": [4, 5],
-        "penalti": 4,
-        "size": 4,
-        "field": [4, 7, 11],
-        "from_nx_graph": 4,
-        "graph": [4, 11, 12],
-        "networkx": [4, 11],
-        "node": [4, 12],
-        "binari": [4, 12],
-        "edg": [4, 12],
-        "weight": 4,
-        "appear": [4, 12],
-        "integ": [4, 5, 7],
-        "coordin": [4, 7, 10],
-        "export": [4, 12],
-        "directli": [4, 10, 11],
-        "qubit_in_json": 4,
-        "rectangularanalogdevic": [4, 6, 11, 12],
-        "length": [4, 7],
-        "width": 4,
-        "include_triangl": 4,
-        "describ": [4, 7, 11, 12],
-        "rectangular": [4, 11],
-        "quantum": [4, 5, 7, 10, 11, 12],
-        "qubit_connect": [4, 7],
-        "connect": [4, 5, 7, 11, 12],
-        "direct": [4, 7],
-        "device_typ": [4, 7],
-        "plaquett": [4, 7, 11],
-        "determin": [4, 7, 12],
-        "order": [4, 5, 7, 10, 11, 12],
-        "specif": [4, 7, 9, 11, 12],
-        "shape": 4,
-        "triangl": [4, 7, 10],
-        "lattic": 4,
-        "rectangulardigitaldevic": [4, 11, 12],
-        "interfac": [5, 12],
-        "cirqexport": 5,
-        "parameter_map": [5, 12],
-        "qubit_map": [5, 12],
-        "namedqubit": 5,
-        "tool": 5,
-        "to_cirq": 5,
-        "rang": [5, 12],
-        "cirq_export": 5,
-        "cirq_circuit": 5,
-        "parityos_circuit": 5,
-        "parameter_valu": 5,
-        "empti": [5, 11],
-        "parityos_qubit": 5,
-        "cirq_qubit": 5,
-        "automat": 5,
-        "gate_to_cirq": 5,
-        "gateoper": 5,
-        "qiskitexport": [5, 12],
-        "to_qiskit": [5, 12],
-        "qiskit_export": [5, 12],
-        "qiskit_circuit": 5,
-        "qubit_index": 5,
-        "index": 5,
-        "regist": 5,
-        "gate_to_qiskit": 5,
-        "instruct": 5,
-        "qubit_indic": 5,
-        "quantumcircuit": 5,
-        "generate_qaoa": [5, 12],
-        "parityos_output": [5, 6, 10, 11, 12],
-        "unitary_pattern": [5, 12],
-        "bound": [5, 12],
-        "compos": 5,
-        "sever": 5,
-        "unitari": [5, 12],
-        "propag": [5, 11],
-        "lower": [5, 12],
-        "upper": 5,
-        "classic": [5, 10],
-        "raw": 5,
-        "assumpt": 5,
-        "explicit": 5,
-        "pattern": [5, 12],
-        "repetit": 5,
-        "follow": [5, 6, 7, 9, 10, 11, 12],
-        "charact": 5,
-        "c": [5, 12],
-        "right": [5, 7, 12],
-        "To": [5, 9, 10, 12],
-        "p": [5, 12],
-        "qaoa_circuit": [5, 12],
-        "parameter_bound": [5, 12],
-        "xczxczxcz": 5,
-        "spin_hamiltonian": [5, 9],
-        "spinz": [5, 9],
-        "Ising": 5,
-        "spinz_to_constraint": 5,
-        "mul": 5,
-        "factor": 5,
-        "spinz_to_hamiltonian": 5,
-        "expr": 5,
-        "spinz_constraint": 5,
-        "sum": [5, 12],
-        "untie_spinz_product": 5,
-        "spilt": 5,
-        "pure": 5,
-        "remain": [5, 12],
-        "client": [6, 12],
-        "call": [6, 10, 11, 12],
-        "block": [6, 11],
-        "consol": 6,
-        "until": [6, 11],
-        "sent": 6,
-        "cannot": [6, 10, 11],
-        "meantim": 6,
-        "wait": 6,
-        "explain": 6,
-        "process": [6, 11],
-        "quickstart": [6, 7, 8, 9],
-        "section": [6, 7, 9, 11, 12],
-        "made": [6, 11],
-        "compiler_cli": [6, 11, 12],
-        "At": 6,
-        "point": 6,
-        "insid": [6, 9],
-        "went": 6,
-        "failur": 6,
-        "exactli": [6, 12],
-        "howev": [6, 10],
-        "here": [6, 7, 10, 11, 12],
-        "asyncron": 6,
-        "7": [6, 7, 9, 11, 12],
-        "dimens": [6, 11, 12],
-        "break": 6,
-        "discuss": [7, 11],
-        "document": 7,
-        "scratch": 7,
-        "nevertheless": 7,
-        "strongli": 7,
-        "contact": [7, 11],
-        "your": [7, 11, 12],
-        "maximum": 7,
-        "advantag": [7, 12],
-        "deriv": 7,
-        "mydevicemodel": 7,
-        "my": 7,
-        "splendid": 7,
-        "relev": 7,
-        "dimension": [7, 12],
-        "j": [7, 12],
-        "layout": [7, 11, 12],
-        "squar": 7,
-        "4": [7, 11, 12],
-        "well": 7,
-        "On": [7, 12],
-        "abil": 7,
-        "site": [7, 11],
-        "assign": [7, 12],
-        "uniqu": 7,
-        "abov": [7, 11, 12],
-        "qubit_sit": 7,
-        "becom": 7,
-        "local_field": 7,
-        "next": [7, 12],
-        "step": [7, 10, 11, 12],
-        "matter": 7,
-        "constraint_connect": 7,
-        "final": [7, 11, 12],
-        "default_analog": 7,
-        "my_device_model": 7,
-        "try": [7, 10, 11, 12],
-        "job": 7,
-        "line": 7,
-        "assum": [7, 10],
-        "perform": [7, 12],
-        "default_digit": 7,
-        "mydigitaldevicemodel": 7,
-        "my_digital_device_model": 7,
-        "instal": [8, 11],
-        "solv": 8,
-        "packag": 9,
-        "environ": [9, 11, 12],
-        "pip": 9,
-        "via": [9, 11, 12],
-        "respect": [9, 12],
-        "addon": 9,
-        "correctli": 9,
-        "virtual": 9,
-        "venv": 9,
-        "enter": [9, 11],
-        "command": [9, 11],
-        "befor": [9, 12],
-        "m": 9,
-        "my_new_venv": 9,
-        "sourc": 9,
-        "bin": 9,
-        "activ": 9,
-        "conda": 9,
-        "my_new_conda_env": 9,
-        "rememb": 9,
-        "find": [10, 12],
-        "wa": [10, 11, 12],
-        "done": 10,
-        "physical_configur": [10, 12],
-        "logical_configur": 10,
-        "closest": 10,
-        "independ": [10, 12],
-        "handl": [10, 12],
-        "incomplet": 10,
-        "long": 10,
-        "third": 10,
-        "fewer": 10,
-        "suppli": 10,
-        "becaus": [10, 12],
-        "expens": 10,
-        "resourc": [10, 12],
-        "few": [10, 11, 12],
-        "while": 10,
-        "being": 10,
-        "abl": [10, 12],
-        "let": [11, 12],
-        "walk": 11,
-        "through": 11,
-        "easi": 11,
-        "past": 11,
-        "snippet": 11,
-        "below": 11,
-        "end": [11, 12],
-        "successfulli": 11,
-        "password": [11, 12],
-        "There": 11,
-        "wai": [11, 12],
-        "constructor": 11,
-        "secur": 11,
-        "reason": 11,
-        "avoid": 11,
-        "plain": 11,
-        "text": 11,
-        "codebas": 11,
-        "parityos_us": [11, 12],
-        "parityos_pass": 11,
-        "therefor": 11,
-        "credenti": 11,
-        "prompt": 11,
-        "manual": 11,
-        "multipl": [11, 12],
-        "s_0": 11,
-        "thu": 11,
-        "s_4": 11,
-        "possibli": 11,
-        "quadrat": [11, 12],
-        "topologi": 11,
-        "most": [11, 12],
-        "probabl": 11,
-        "coincid": 11,
-        "asid": 11,
-        "coupler": 11,
-        "everi": [11, 12],
-        "similarli": 11,
-        "easili": 11,
-        "vertic": 11,
-        "horizont": 11,
-        "server": 11,
-        "internet": 11,
-        "success": 11,
-        "person": 11,
-        "interest": 11,
-        "u": [11, 12],
-        "know": 11,
-        "finish": 11,
-        "retriev": 11,
-        "side": 11,
-        "compon": 11,
-        "decompos": 11,
-        "frac": [11, 12],
-        "suitabl": [11, 12],
-        "sure": 11,
-        "print": [11, 12],
-        "And": 11,
-        "tutori": 12,
-        "demonstr": 12,
-        "help": 12,
-        "cover": 12,
-        "entir": 12,
-        "workflow": 12,
-        "reformul": 12,
-        "ground": 12,
-        "tackl": 12,
-        "maxcut": 12,
-        "hypergraph": 12,
-        "mani": 12,
-        "applic": 12,
-        "design": 12,
-        "v": 12,
-        "than": 12,
-        "goal": 12,
-        "split": 12,
-        "cut": 12,
-        "least": 12,
-        "sinc": 12,
-        "np": 12,
-        "approxim": 12,
-        "arbitrari": 12,
-        "precis": 12,
-        "heurist": 12,
-        "our": 12,
-        "green": 12,
-        "circl": 12,
-        "hyper": 12,
-        "color": 12,
-        "s_i": 12,
-        "belong": 12,
-        "maximis": 12,
-        "h_e": 12,
-        "prod_": 12,
-        "sum_": 12,
-        "delta_i": 12,
-        "delta_j": 12,
-        "reward": 12,
-        "2a": 12,
-        "suffic": 12,
-        "subset": 12,
-        "onc": 12,
-        "total": 12,
-        "begin": 12,
-        "bigg": 12,
-        "s_5": 12,
-        "s_2s_4": 12,
-        "s_3s_4": 12,
-        "s_1s_3": 12,
-        "s_2s_3": 12,
-        "s_2s_5": 12,
-        "s_1s_2": 12,
-        "s_3s_5": 12,
-        "s_1s_2s_3s_5": 12,
-        "625": 12,
-        "125": 12,
-        "higher": 12,
-        "rank": 12,
-        "j_": 12,
-        "s_is_js_k": 12,
-        "real": 12,
-        "s_": 12,
-        "s_j": 12,
-        "s_k": 12,
-        "complet": 12,
-        "addition": 12,
-        "enforc": 12,
-        "remov": 12,
-        "reduc": 12,
-        "qubo": 12,
-        "caus": 12,
-        "overhead": 12,
-        "depth": 12,
-        "explan": 12,
-        "lechner15": 12,
-        "fellner21": 12,
-        "put": 12,
-        "choos": 12,
-        "pick": 12,
-        "suit": 12,
-        "5x5": 12,
-        "locat": 12,
-        "enabl": 12,
-        "cf": 12,
-        "readi": 12,
-        "varieti": 12,
-        "latter": 12,
-        "task": 12,
-        "eas": 12,
-        "benefit": 12,
-        "paralleliz": 12,
-        "scalabl": 12,
-        "emploi": 12,
-        "hybrid": 12,
-        "guarante": 12,
-        "farhi14": 12,
-        "main": 12,
-        "idea": 12,
-        "h_": 12,
-        "mathrm": 12,
-        "phy": 12,
-        "expect": 12,
-        "parameter": 12,
-        "trial": 12,
-        "f": 12,
-        "vec": 12,
-        "beta": 12,
-        "psi": 12,
-        "rangl": 12,
-        "evolut": 12,
-        "under": 12,
-        "altern": 12,
-        "round": 12,
-        "mix": 12,
-        "h_m": 12,
-        "beta_p": 12,
-        "gamma_p": 12,
-        "beta_1": 12,
-        "gamma_1": 12,
-        "psi_0": 12,
-        "motiv": 12,
-        "adiabat": 12,
-        "formula": 12,
-        "view": 12,
-        "finit": 12,
-        "expans": 12,
-        "eigenst": 12,
-        "basic": 12,
-        "zcx": 12,
-        "denot": 12,
-        "repeat": 12,
-        "mutual": 12,
-        "simpli": 12,
-        "accord": 12,
-        "enumer": 12,
-        "With": 12,
-        "qaoa_circuit_qiskit": 12,
-        "measur": 12,
-        "measure_al": 12,
-        "conveni": 12,
-        "helper": 12,
-        "count": 12,
-        "def": 12,
-        "get_physical_configur": 12,
-        "bit": 12,
-        "zip": 12,
-        "cost_expect": 12,
-        "expectation_sum": 12,
-        "cost": 12,
-        "crucial": 12,
-        "certain": 12,
-        "front": 12,
-        "quit": 12,
-        "tricki": 12,
-        "larg": 12,
-        "increas": 12,
-        "gap": 12,
-        "highest": 12,
-        "excit": 12,
-        "decreas": 12,
-        "hand": 12,
-        "small": 12,
-        "lead": 12,
-        "favor": 12,
-        "qiskit_a": 12,
-        "aer": 12,
-        "execute_circuit": 12,
-        "backend": 12,
-        "get_backend": 12,
-        "qasm_simul": 12,
-        "bind_paramet": 12,
-        "chosen": 12,
-        "512": 12,
-        "seed": 12,
-        "ensur": 12,
-        "reproduc": 12,
-        "seed_simul": 12,
-        "nshot": 12,
-        "get_count": 12,
-        "n_starting_point": 12,
-        "initial_parameter_list": 12,
-        "uniform": 12,
-        "_": 12,
-        "improv": 12,
-        "invok": 12,
-        "scipi": 12,
-        "initial_paramet": 12,
-        "optimized_paramet": 12,
-        "nelder": 12,
-        "mead": 12,
-        "fun": 12,
-        "previou": 12,
-        "best": 12,
-        "optimal_paramet": 12,
-        "cours": 12,
-        "differ": 12,
-        "far": 12,
-        "optimal_qaoa_circuit": 12,
-        "aer_simul": 12,
-        "shot": 12,
-        "frequent": 12,
-        "outcom": 12,
-        "n_best_solut": 12,
-        "best_physical_bitstr": 12,
-        "revers": 12,
-        "candid": 12,
-        "best_physical_configur": 12,
-        "physical_bitstr": 12,
-        "bistr": 12,
-        "best_logical_bitstr": 12,
-        "itertool": 12,
-        "chain": 12,
-        "logical_bitstr": 12,
-        "cost_of_bitstr": 12,
-        "logical_solut": 12,
-        "As": 12,
-        "longer": 12,
-        "too": 12,
-        "high": 12,
-        "readili": 12,
-        "off": 12,
-        "partit": 12,
-        "turquois": 12,
-        "yellow": 12,
-        "light": 12,
-        "red": 12,
-        "degener": 12,
-        "advanc": 12,
-        "lechner": 12,
-        "wolfgang": 12,
-        "philipp": 12,
-        "hauk": 12,
-        "peter": 12,
-        "zoller": 12,
-        "anneal": 12,
-        "scienc": 12,
-        "9": 12,
-        "2015": 12,
-        "e1500838": 12,
-        "fellner": 12,
-        "michael": 12,
-        "et": 12,
-        "al": 12,
-        "benchmark": 12,
-        "arxiv": 12,
-        "preprint": 12,
-        "2105": 12,
-        "06240": 12,
-        "2021": 12,
-        "http": 12,
-        "org": 12,
-        "farhi": 12,
-        "edward": 12,
-        "jeffrei": 12,
-        "goldston": 12,
-        "sam": 12,
-        "gutmann": 12,
-        "1411": 12,
-        "4028": 12,
-        "2014": 12
+    "indexentries": {
+        "__init__() (parityos.base.constraints.equalityconstraint method)": [
+            [1, "parityos.base.constraints.EqualityConstraint.__init__", false]
+        ],
+        "__init__() (parityos.base.constraints.parityconstraint method)": [
+            [1, "parityos.base.constraints.ParityConstraint.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.ccmixin method)": [
+            [1, "parityos.base.gates.CCMixin.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.cmixin method)": [
+            [1, "parityos.base.gates.CMixin.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.gate1 method)": [
+            [1, "parityos.base.gates.Gate1.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.gate2 method)": [
+            [1, "parityos.base.gates.Gate2.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.gate3 method)": [
+            [1, "parityos.base.gates.Gate3.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.gate4 method)": [
+            [1, "parityos.base.gates.Gate4.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.multicontrolmixin method)": [
+            [1, "parityos.base.gates.MultiControlMixin.__init__", false]
+        ],
+        "__init__() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.__init__", false]
+        ],
+        "__init__() (parityos.encodings.mappings.mappings method)": [
+            [2, "parityos.encodings.mappings.Mappings.__init__", false]
+        ],
+        "__init__() (parityos.encodings.mappings.paritymap method)": [
+            [2, "parityos.encodings.mappings.ParityMap.__init__", false]
+        ],
+        "__init__() (parityos.hamiltonian method)": [
+            [4, "parityos.Hamiltonian.__init__", false]
+        ],
+        "__init__() (parityos.parityosoutput method)": [
+            [4, "parityos.ParityOSOutput.__init__", false]
+        ],
+        "__init__() (parityos.problemrepresentation method)": [
+            [4, "parityos.ProblemRepresentation.__init__", false]
+        ],
+        "__init__() (parityos.qubit method)": [
+            [4, "parityos.Qubit.__init__", false]
+        ],
+        "__init__() (parityos.rectangularanalogdevice method)": [
+            [4, "parityos.RectangularAnalogDevice.__init__", false]
+        ],
+        "__init__() (parityos.rectangulardigitaldevice method)": [
+            [4, "parityos.RectangularDigitalDevice.__init__", false]
+        ],
+        "__init__() (parityos_addons.interfaces.cirqexporter method)": [
+            [5, "parityos_addons.interfaces.CirqExporter.__init__", false]
+        ],
+        "__init__() (parityos_addons.interfaces.qiskitexporter method)": [
+            [5, "parityos_addons.interfaces.QiskitExporter.__init__", false]
+        ],
+        "append_qiskit_gate() (parityos_addons.interfaces.qiskitexporter method)": [
+            [5, "parityos_addons.interfaces.QiskitExporter.append_qiskit_gate", false]
+        ],
+        "ccmixin (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CCMixin", false]
+        ],
+        "ccnot (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CCNOT", false]
+        ],
+        "ch (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CH", false]
+        ],
+        "circuit (class in parityos.base.circuit)": [
+            [1, "parityos.base.circuit.Circuit", false]
+        ],
+        "cirqexporter (class in parityos_addons.interfaces)": [
+            [5, "parityos_addons.interfaces.CirqExporter", false]
+        ],
+        "cmixin (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CMixin", false]
+        ],
+        "cnot (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CNOT", false]
+        ],
+        "compile() (parityos.compilerclient method)": [
+            [4, "parityos.CompilerClient.compile", false]
+        ],
+        "compilerclient (class in parityos)": [
+            [4, "parityos.CompilerClient", false]
+        ],
+        "convert_cnots_to_rzzs() (in module parityos.base.circuit)": [
+            [1, "parityos.base.circuit.convert_cnots_to_rzzs", false]
+        ],
+        "create_default_problem_circuit() (parityos.parityosoutput method)": [
+            [4, "parityos.ParityOSOutput.create_default_problem_circuit", false]
+        ],
+        "crx (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CRx", false]
+        ],
+        "cry (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CRy", false]
+        ],
+        "crz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CRz", false]
+        ],
+        "cy (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CY", false]
+        ],
+        "cz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.CZ", false]
+        ],
+        "decode() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
+            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.decode", false]
+        ],
+        "dict_filter() (in module parityos.base.utils)": [
+            [1, "parityos.base.utils.dict_filter", false]
+        ],
+        "encode() (parityos.encodings.parity_encoder.parityencoderextension method)": [
+            [2, "parityos.encodings.parity_encoder.ParityEncoderExtension.encode", false]
+        ],
+        "encode_problem() (parityos.parityosoutput method)": [
+            [4, "parityos.ParityOSOutput.encode_problem", false]
+        ],
+        "equalityconstraint (class in parityos.base.constraints)": [
+            [1, "parityos.base.constraints.EqualityConstraint", false]
+        ],
+        "error_correct() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
+            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.error_correct", false]
+        ],
+        "evaluate() (parityos.problemrepresentation method)": [
+            [4, "parityos.ProblemRepresentation.evaluate", false]
+        ],
+        "evaluate_parity() (in module parityos.base.constraints)": [
+            [1, "parityos.base.constraints.evaluate_parity", false]
+        ],
+        "from_json() (parityos.base.circuit.circuit class method)": [
+            [1, "parityos.base.circuit.Circuit.from_json", false]
+        ],
+        "from_json() (parityos.base.constraints.equalityconstraint class method)": [
+            [1, "parityos.base.constraints.EqualityConstraint.from_json", false]
+        ],
+        "from_json() (parityos.base.gates.gate class method)": [
+            [1, "parityos.base.gates.Gate.from_json", false]
+        ],
+        "from_json() (parityos.base.utils.jsonloadsavemixin class method)": [
+            [1, "parityos.base.utils.JSONLoadSaveMixin.from_json", false]
+        ],
+        "from_json() (parityos.encodings.mappings.mappings class method)": [
+            [2, "parityos.encodings.mappings.Mappings.from_json", false]
+        ],
+        "from_json() (parityos.encodings.mappings.paritymap class method)": [
+            [2, "parityos.encodings.mappings.ParityMap.from_json", false]
+        ],
+        "from_json() (parityos.parityosoutput class method)": [
+            [4, "parityos.ParityOSOutput.from_json", false]
+        ],
+        "from_json() (parityos.problemrepresentation class method)": [
+            [4, "parityos.ProblemRepresentation.from_json", false]
+        ],
+        "from_json() (parityos.qubit class method)": [
+            [4, "parityos.Qubit.from_json", false]
+        ],
+        "from_nx_graph() (parityos.problemrepresentation class method)": [
+            [4, "parityos.ProblemRepresentation.from_nx_graph", false]
+        ],
+        "gate (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Gate", false]
+        ],
+        "gate1 (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Gate1", false]
+        ],
+        "gate2 (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Gate2", false]
+        ],
+        "gate3 (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Gate3", false]
+        ],
+        "gate4 (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Gate4", false]
+        ],
+        "gate_to_cirq() (parityos_addons.interfaces.cirqexporter method)": [
+            [5, "parityos_addons.interfaces.CirqExporter.gate_to_cirq", false]
+        ],
+        "generate_flat_gate_sequence() (parityos.base.circuit.circuit method)": [
+            [1, "parityos.base.circuit.Circuit.generate_flat_gate_sequence", false]
+        ],
+        "generate_qaoa() (in module parityos_addons.qaoa)": [
+            [5, "parityos_addons.qaoa.generate_qaoa", false]
+        ],
+        "get_compiler_runs() (parityos.compilerclient method)": [
+            [4, "parityos.CompilerClient.get_compiler_runs", false]
+        ],
+        "get_hermitian_conjugate() (parityos.base.circuit.circuit method)": [
+            [1, "parityos.base.circuit.Circuit.get_hermitian_conjugate", false]
+        ],
+        "get_hermitian_conjugate() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.get_hermitian_conjugate", false]
+        ],
+        "get_hermitian_conjugate() (parityos.base.gates.hermitiangatemixin method)": [
+            [1, "parityos.base.gates.HermitianGateMixin.get_hermitian_conjugate", false]
+        ],
+        "get_hermitian_conjugate() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.get_hermitian_conjugate", false]
+        ],
+        "get_solutions() (parityos.compilerclient method)": [
+            [4, "parityos.CompilerClient.get_solutions", false]
+        ],
+        "get_submission() (parityos.compilerclient method)": [
+            [4, "parityos.CompilerClient.get_submission", false]
+        ],
+        "h (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.H", false]
+        ],
+        "hamiltonian (class in parityos)": [
+            [4, "parityos.Hamiltonian", false]
+        ],
+        "hermitiangatemixin (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.HermitianGateMixin", false]
+        ],
+        "is_satisfied() (parityos.base.constraints.equalityconstraint method)": [
+            [1, "parityos.base.constraints.EqualityConstraint.is_satisfied", false]
+        ],
+        "iswap (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.ISwap", false]
+        ],
+        "json_wrap() (in module parityos.base.utils)": [
+            [1, "parityos.base.utils.json_wrap", false]
+        ],
+        "jsonloadsavemixin (class in parityos.base.utils)": [
+            [1, "parityos.base.utils.JSONLoadSaveMixin", false]
+        ],
+        "load() (parityos.base.utils.jsonloadsavemixin class method)": [
+            [1, "parityos.base.utils.JSONLoadSaveMixin.load", false]
+        ],
+        "logical_degeneracies (parityos.encodings.mappings.mappings property)": [
+            [2, "parityos.encodings.mappings.Mappings.logical_degeneracies", false]
+        ],
+        "logical_problem_circuit (parityos.parityosoutput property)": [
+            [4, "parityos.ParityOSOutput.logical_problem_circuit", false]
+        ],
+        "make_args() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.make_args", false]
+        ],
+        "make_args() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.make_args", false]
+        ],
+        "make_args_and_kwargs_from_json() (parityos.base.gates.gate static method)": [
+            [1, "parityos.base.gates.Gate.make_args_and_kwargs_from_json", false]
+        ],
+        "make_args_and_kwargs_from_json() (parityos.base.gates.rmixin class method)": [
+            [1, "parityos.base.gates.RMixin.make_args_and_kwargs_from_json", false]
+        ],
+        "make_full_configuration_from_partial() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
+            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.make_full_configuration_from_partial", false]
+        ],
+        "mappings (class in parityos.encodings.mappings)": [
+            [2, "parityos.encodings.mappings.Mappings", false]
+        ],
+        "modify_angle() (parityos.base.circuit.circuit method)": [
+            [1, "parityos.base.circuit.Circuit.modify_angle", false]
+        ],
+        "modify_angle() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.modify_angle", false]
+        ],
+        "modify_angle() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.modify_angle", false]
+        ],
+        "module": [
+            [0, "module-parityos.api_interface", false],
+            [1, "module-parityos.base.circuit", false],
+            [1, "module-parityos.base.constraints", false],
+            [1, "module-parityos.base.gates", false],
+            [1, "module-parityos.base.utils", false],
+            [2, "module-parityos.encodings.mappings", false],
+            [2, "module-parityos.encodings.parity_decoder", false],
+            [2, "module-parityos.encodings.parity_encoder", false],
+            [4, "module-parityos", false],
+            [5, "module-parityos_addons.interfaces", false],
+            [5, "module-parityos_addons.qaoa", false],
+            [5, "module-parityos_addons.spin_hamiltonians", false]
+        ],
+        "multicontrolledh (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.MultiControlledH", false]
+        ],
+        "multicontrolledrx (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.MultiControlledRx", false]
+        ],
+        "multicontrolledry (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.MultiControlledRy", false]
+        ],
+        "multicontrolledrz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.MultiControlledRz", false]
+        ],
+        "multicontrolmixin (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.MultiControlMixin", false]
+        ],
+        "parameters (parityos.base.circuit.circuit property)": [
+            [1, "parityos.base.circuit.Circuit.parameters", false]
+        ],
+        "parameters (parityos.base.gates.rmixin property)": [
+            [1, "parityos.base.gates.RMixin.parameters", false]
+        ],
+        "parityconstraint (class in parityos.base.constraints)": [
+            [1, "parityos.base.constraints.ParityConstraint", false]
+        ],
+        "paritydecoderextension (class in parityos.encodings.parity_decoder)": [
+            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension", false]
+        ],
+        "parityencoderextension (class in parityos.encodings.parity_encoder)": [
+            [2, "parityos.encodings.parity_encoder.ParityEncoderExtension", false]
+        ],
+        "paritymap (class in parityos.encodings.mappings)": [
+            [2, "parityos.encodings.mappings.ParityMap", false]
+        ],
+        "parityos": [
+            [4, "module-parityos", false]
+        ],
+        "parityos.api_interface": [
+            [0, "module-parityos.api_interface", false]
+        ],
+        "parityos.base.circuit": [
+            [1, "module-parityos.base.circuit", false]
+        ],
+        "parityos.base.constraints": [
+            [1, "module-parityos.base.constraints", false]
+        ],
+        "parityos.base.gates": [
+            [1, "module-parityos.base.gates", false]
+        ],
+        "parityos.base.utils": [
+            [1, "module-parityos.base.utils", false]
+        ],
+        "parityos.encodings.mappings": [
+            [2, "module-parityos.encodings.mappings", false]
+        ],
+        "parityos.encodings.parity_decoder": [
+            [2, "module-parityos.encodings.parity_decoder", false]
+        ],
+        "parityos.encodings.parity_encoder": [
+            [2, "module-parityos.encodings.parity_encoder", false]
+        ],
+        "parityos_addons.interfaces": [
+            [5, "module-parityos_addons.interfaces", false]
+        ],
+        "parityos_addons.qaoa": [
+            [5, "module-parityos_addons.qaoa", false]
+        ],
+        "parityos_addons.spin_hamiltonians": [
+            [5, "module-parityos_addons.spin_hamiltonians", false]
+        ],
+        "parityosexception": [
+            [4, "parityos.ParityOSException", false]
+        ],
+        "parityosimporterror": [
+            [4, "parityos.ParityOSImportError", false]
+        ],
+        "parityosoutput (class in parityos)": [
+            [4, "parityos.ParityOSOutput", false]
+        ],
+        "problemrepresentation (class in parityos)": [
+            [4, "parityos.ProblemRepresentation", false]
+        ],
+        "qiskitexporter (class in parityos_addons.interfaces)": [
+            [5, "parityos_addons.interfaces.QiskitExporter", false]
+        ],
+        "qubit (class in parityos)": [
+            [4, "parityos.Qubit", false]
+        ],
+        "qubits (parityos.base.circuit.circuit property)": [
+            [1, "parityos.base.circuit.Circuit.qubits", false]
+        ],
+        "qubits (parityos.base.gates.gate property)": [
+            [1, "parityos.base.gates.Gate.qubits", false]
+        ],
+        "qubits (parityos.problemrepresentation property)": [
+            [4, "parityos.ProblemRepresentation.qubits", false]
+        ],
+        "rectangularanalogdevice (class in parityos)": [
+            [4, "parityos.RectangularAnalogDevice", false]
+        ],
+        "rectangulardigitaldevice (class in parityos)": [
+            [4, "parityos.RectangularDigitalDevice", false]
+        ],
+        "remap() (parityos.base.circuit.circuit method)": [
+            [1, "parityos.base.circuit.Circuit.remap", false]
+        ],
+        "remap() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.remap", false]
+        ],
+        "remap() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.remap", false]
+        ],
+        "replace_cnots_by_rzzs() (parityos.parityosoutput method)": [
+            [4, "parityos.ParityOSOutput.replace_cnots_by_rzzs", false]
+        ],
+        "rmixin (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.RMixin", false]
+        ],
+        "rx (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Rx", false]
+        ],
+        "rxx (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Rxx", false]
+        ],
+        "ry (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Ry", false]
+        ],
+        "ryy (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Ryy", false]
+        ],
+        "rz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Rz", false]
+        ],
+        "rzz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Rzz", false]
+        ],
+        "rzzzz (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Rzzzz", false]
+        ],
+        "save() (parityos.base.utils.jsonloadsavemixin method)": [
+            [1, "parityos.base.utils.JSONLoadSaveMixin.save", false]
+        ],
+        "select_reduced_readout_qubits() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
+            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.select_reduced_readout_qubits", false]
+        ],
+        "spinz (class in parityos_addons.spin_hamiltonians)": [
+            [5, "parityos_addons.spin_hamiltonians.SpinZ", false]
+        ],
+        "spinz_to_constraint() (in module parityos_addons.spin_hamiltonians)": [
+            [5, "parityos_addons.spin_hamiltonians.spinz_to_constraint", false]
+        ],
+        "spinz_to_hamiltonian() (in module parityos_addons.spin_hamiltonians)": [
+            [5, "parityos_addons.spin_hamiltonians.spinz_to_hamiltonian", false]
+        ],
+        "submit() (parityos.compilerclient method)": [
+            [4, "parityos.CompilerClient.submit", false]
+        ],
+        "swap (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Swap", false]
+        ],
+        "target_qubit (parityos.base.gates.gate1 property)": [
+            [1, "parityos.base.gates.Gate1.target_qubit", false]
+        ],
+        "terms (parityos.problemrepresentation property)": [
+            [4, "parityos.ProblemRepresentation.terms", false]
+        ],
+        "to_cirq() (parityos_addons.interfaces.cirqexporter method)": [
+            [5, "parityos_addons.interfaces.CirqExporter.to_cirq", false]
+        ],
+        "to_json() (parityos.base.circuit.circuit method)": [
+            [1, "parityos.base.circuit.Circuit.to_json", false]
+        ],
+        "to_json() (parityos.base.constraints.equalityconstraint method)": [
+            [1, "parityos.base.constraints.EqualityConstraint.to_json", false]
+        ],
+        "to_json() (parityos.base.gates.gate method)": [
+            [1, "parityos.base.gates.Gate.to_json", false]
+        ],
+        "to_json() (parityos.base.gates.rmixin method)": [
+            [1, "parityos.base.gates.RMixin.to_json", false]
+        ],
+        "to_json() (parityos.base.utils.jsonloadsavemixin method)": [
+            [1, "parityos.base.utils.JSONLoadSaveMixin.to_json", false]
+        ],
+        "to_json() (parityos.encodings.mappings.mappings method)": [
+            [2, "parityos.encodings.mappings.Mappings.to_json", false]
+        ],
+        "to_json() (parityos.encodings.mappings.paritymap method)": [
+            [2, "parityos.encodings.mappings.ParityMap.to_json", false]
+        ],
+        "to_json() (parityos.parityosoutput method)": [
+            [4, "parityos.ParityOSOutput.to_json", false]
+        ],
+        "to_json() (parityos.problemrepresentation method)": [
+            [4, "parityos.ProblemRepresentation.to_json", false]
+        ],
+        "to_json() (parityos.qubit method)": [
+            [4, "parityos.Qubit.to_json", false]
+        ],
+        "to_qiskit() (parityos_addons.interfaces.qiskitexporter method)": [
+            [5, "parityos_addons.interfaces.QiskitExporter.to_qiskit", false]
+        ],
+        "untie_spinz_product() (in module parityos_addons.spin_hamiltonians)": [
+            [5, "parityos_addons.spin_hamiltonians.untie_spinz_product", false]
+        ],
+        "x (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.X", false]
+        ],
+        "y (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Y", false]
+        ],
+        "z (class in parityos.base.gates)": [
+            [1, "parityos.base.gates.Z", false]
+        ]
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "parityos"]
         ],
         "parityos": [
             [4, 1, 1, "", "CompilerClient"],
@@ -1176,73 +707,91 @@
             [1, 2, 1, "", "is_satisfied"],
             [1, 2, 1, "", "to_json"]
         ],
         "parityos.base.constraints.ParityConstraint": [
             [1, 2, 1, "", "__init__"]
         ],
         "parityos.base.gates": [
+            [1, 1, 1, "", "CCMixin"],
             [1, 1, 1, "", "CCNOT"],
+            [1, 1, 1, "", "CH"],
+            [1, 1, 1, "", "CMixin"],
             [1, 1, 1, "", "CNOT"],
+            [1, 1, 1, "", "CRx"],
+            [1, 1, 1, "", "CRy"],
+            [1, 1, 1, "", "CRz"],
+            [1, 1, 1, "", "CY"],
             [1, 1, 1, "", "CZ"],
             [1, 1, 1, "", "Gate"],
             [1, 1, 1, "", "Gate1"],
             [1, 1, 1, "", "Gate2"],
             [1, 1, 1, "", "Gate3"],
             [1, 1, 1, "", "Gate4"],
             [1, 1, 1, "", "H"],
             [1, 1, 1, "", "HermitianGateMixin"],
+            [1, 1, 1, "", "ISwap"],
+            [1, 1, 1, "", "MultiControlMixin"],
+            [1, 1, 1, "", "MultiControlledH"],
+            [1, 1, 1, "", "MultiControlledRx"],
+            [1, 1, 1, "", "MultiControlledRy"],
+            [1, 1, 1, "", "MultiControlledRz"],
             [1, 1, 1, "", "RMixin"],
             [1, 1, 1, "", "Rx"],
+            [1, 1, 1, "", "Rxx"],
             [1, 1, 1, "", "Ry"],
+            [1, 1, 1, "", "Ryy"],
             [1, 1, 1, "", "Rz"],
             [1, 1, 1, "", "Rzz"],
+            [1, 1, 1, "", "Rzzzz"],
+            [1, 1, 1, "", "Swap"],
             [1, 1, 1, "", "X"],
             [1, 1, 1, "", "Y"],
             [1, 1, 1, "", "Z"]
         ],
-        "parityos.base.gates.CCNOT": [
-            [1, 2, 1, "", "__init__"]
-        ],
-        "parityos.base.gates.CNOT": [
+        "parityos.base.gates.CCMixin": [
             [1, 2, 1, "", "__init__"]
         ],
-        "parityos.base.gates.CZ": [
+        "parityos.base.gates.CMixin": [
             [1, 2, 1, "", "__init__"]
         ],
         "parityos.base.gates.Gate": [
             [1, 2, 1, "", "__init__"],
             [1, 2, 1, "", "from_json"],
             [1, 2, 1, "", "get_hermitian_conjugate"],
             [1, 2, 1, "", "make_args"],
+            [1, 2, 1, "", "make_args_and_kwargs_from_json"],
             [1, 2, 1, "", "modify_angle"],
             [1, 4, 1, "", "qubits"],
             [1, 2, 1, "", "remap"],
             [1, 2, 1, "", "to_json"]
         ],
         "parityos.base.gates.Gate1": [
             [1, 2, 1, "", "__init__"],
-            [1, 4, 1, "", "qubit"]
+            [1, 4, 1, "", "target_qubit"]
         ],
         "parityos.base.gates.Gate2": [
             [1, 2, 1, "", "__init__"]
         ],
         "parityos.base.gates.Gate3": [
             [1, 2, 1, "", "__init__"]
         ],
         "parityos.base.gates.Gate4": [
             [1, 2, 1, "", "__init__"]
         ],
         "parityos.base.gates.HermitianGateMixin": [
             [1, 2, 1, "", "get_hermitian_conjugate"]
         ],
+        "parityos.base.gates.MultiControlMixin": [
+            [1, 2, 1, "", "__init__"]
+        ],
         "parityos.base.gates.RMixin": [
             [1, 2, 1, "", "__init__"],
-            [1, 2, 1, "", "from_json"],
             [1, 2, 1, "", "get_hermitian_conjugate"],
             [1, 2, 1, "", "make_args"],
+            [1, 2, 1, "", "make_args_and_kwargs_from_json"],
             [1, 2, 1, "", "modify_angle"],
             [1, 4, 1, "", "parameters"],
             [1, 2, 1, "", "remap"],
             [1, 2, 1, "", "to_json"]
         ],
         "parityos.base.utils": [
             [1, 1, 1, "", "JSONLoadSaveMixin"],
@@ -1302,660 +851,1213 @@
         "parityos_addons.interfaces.CirqExporter": [
             [5, 2, 1, "", "__init__"],
             [5, 2, 1, "", "gate_to_cirq"],
             [5, 2, 1, "", "to_cirq"]
         ],
         "parityos_addons.interfaces.QiskitExporter": [
             [5, 2, 1, "", "__init__"],
-            [5, 2, 1, "", "gate_to_qiskit"],
+            [5, 2, 1, "", "append_qiskit_gate"],
             [5, 2, 1, "", "to_qiskit"]
         ],
         "parityos_addons.qaoa": [
             [5, 5, 1, "", "generate_qaoa"]
         ],
         "parityos_addons.spin_hamiltonians": [
             [5, 1, 1, "", "SpinZ"],
             [5, 5, 1, "", "spinz_to_constraint"],
             [5, 5, 1, "", "spinz_to_hamiltonian"],
             [5, 5, 1, "", "untie_spinz_product"]
         ]
     },
+    "objnames": {
+        "0": ["py", "module", "Python module"],
+        "1": ["py", "class", "Python class"],
+        "2": ["py", "method", "Python method"],
+        "3": ["py", "exception", "Python exception"],
+        "4": ["py", "property", "Python property"],
+        "5": ["py", "function", "Python function"]
+    },
     "objtypes": {
         "0": "py:module",
         "1": "py:class",
         "2": "py:method",
         "3": "py:exception",
         "4": "py:property",
         "5": "py:function"
     },
-    "objnames": {
-        "0": ["py", "module", "Python module"],
-        "1": ["py", "class", "Python class"],
-        "2": ["py", "method", "Python method"],
-        "3": ["py", "exception", "Python exception"],
-        "4": ["py", "property", "Python property"],
-        "5": ["py", "function", "Python function"]
+    "terms": {
+        "": [1, 10, 11],
+        "0": [1, 4, 6, 7, 10, 11, 12],
+        "02": 4,
+        "06240": 12,
+        "1": [1, 2, 4, 5, 6, 7, 10, 11, 12],
+        "10": [4, 5, 12],
+        "11": 5,
+        "125": 12,
+        "1411": 12,
+        "2": [1, 4, 5, 6, 7, 11, 12],
+        "2014": 12,
+        "2015": 12,
+        "2021": 12,
+        "2105": 12,
+        "2a": 12,
+        "3": [4, 5, 7, 9, 12],
+        "4": [7, 11, 12],
+        "4028": 12,
+        "5": [1, 4, 6, 7, 11, 12],
+        "512": 12,
+        "5x5": 12,
+        "625": 12,
+        "7": [6, 7, 9, 11, 12],
+        "8": [4, 7],
+        "9": 12,
+        "900": 4,
+        "A": [1, 2, 4, 5, 7, 11, 12],
+        "And": 11,
+        "As": 12,
+        "At": 6,
+        "By": [4, 12],
+        "For": [1, 4, 6, 7, 9, 10, 11, 12],
+        "If": [1, 2, 4, 5, 7, 10, 11],
+        "In": [4, 6, 7, 11, 12],
+        "Ising": 5,
+        "It": [2, 4, 6, 9, 11, 12],
+        "On": [7, 12],
+        "The": [1, 2, 4, 5, 6, 7, 8],
+        "Then": [1, 5, 6, 7, 11],
+        "There": 11,
+        "These": [2, 12],
+        "To": [5, 9, 10, 12],
+        "With": 12,
+        "_": 12,
+        "__init__": [1, 2, 4, 5],
+        "abil": 7,
+        "abl": [10, 12],
+        "abort": 4,
+        "about": [1, 4, 5, 6, 9, 11],
+        "abov": [7, 11, 12],
+        "absorb": 4,
+        "abstract": 1,
+        "access": [4, 10, 11],
+        "accord": 12,
+        "account": 1,
+        "act": 1,
+        "activ": 9,
+        "ad": 1,
+        "add": [1, 5, 7, 9, 11, 12],
+        "addit": [1, 5],
+        "addition": 12,
+        "addon": 9,
+        "adiabat": 12,
+        "advanc": 12,
+        "advantag": [7, 12],
+        "aer": 12,
+        "aer_simul": 12,
+        "affect": 1,
+        "after": [4, 6, 7, 10, 11],
+        "again": 1,
+        "al": 12,
+        "algorithm": [2, 4, 11],
+        "align": [4, 12],
+        "all": [1, 2, 4, 5, 6, 7, 10, 11, 12],
+        "allow": [4, 11, 12],
+        "also": [1, 4, 6, 7, 10, 11, 12],
+        "altern": 12,
+        "alwai": [1, 4, 11, 12],
+        "an": [1, 4, 5, 6, 7, 9, 10, 12],
+        "analog": [4, 6, 11, 12],
+        "analog_default": [4, 7],
+        "angl": [1, 4],
+        "angle_map": 1,
+        "ani": [1, 2, 4, 6, 10, 12],
+        "anneal": 12,
+        "anti": 1,
+        "api": [2, 4, 6, 8, 11],
+        "api_interfac": 3,
+        "appear": [4, 12],
+        "append": 5,
+        "append_qiskit_g": 5,
+        "appli": [1, 2, 10, 12],
+        "applic": 12,
+        "approxim": 12,
+        "ar": [1, 2, 4, 5, 7, 9, 10, 11, 12],
+        "arbitrari": [1, 12],
+        "architectur": [2, 11, 12],
+        "arg": [1, 4],
+        "argument": [1, 4],
+        "arxiv": 12,
+        "asid": 11,
+        "assign": [7, 12],
+        "associ": [4, 12],
+        "assum": [7, 10],
+        "assumpt": 5,
+        "asynchron": [4, 8, 11],
+        "asyncron": 6,
+        "attribut": [1, 4, 7, 11],
+        "automat": 5,
+        "avail": [4, 11, 12],
+        "avoid": 11,
+        "back": [2, 6, 12],
+        "backend": 12,
+        "base": [2, 3, 5, 9, 11, 12],
+        "basi": 4,
+        "basic": 12,
+        "becaus": [10, 12],
+        "becom": 7,
+        "been": [1, 4, 6, 12],
+        "befor": [1, 9, 12],
+        "begin": 12,
+        "being": 10,
+        "belong": 12,
+        "below": 11,
+        "benchmark": 12,
+        "benefit": 12,
+        "best": 12,
+        "best_logical_bitstr": 12,
+        "best_physical_bitstr": 12,
+        "best_physical_configur": 12,
+        "beta": 12,
+        "beta_1": 12,
+        "beta_p": 12,
+        "between": [1, 4, 11, 12],
+        "bigg": 12,
+        "bin": 9,
+        "binari": [4, 12],
+        "bind_paramet": 12,
+        "bistr": 12,
+        "bit": 12,
+        "bitstr": [2, 12],
+        "block": [1, 6, 11],
+        "bodi": [4, 5, 7, 11, 12],
+        "bonu": 4,
+        "bool": [1, 2, 4],
+        "boolean": 1,
+        "both": [1, 4, 7, 12],
+        "bound": [5, 12],
+        "break": 6,
+        "builtin": 1,
+        "c": [5, 12],
+        "call": [6, 10, 11, 12],
+        "can": [1, 2, 4, 6, 7, 9, 10, 11, 12],
+        "candid": 12,
+        "cannot": [6, 10, 11],
+        "case": [2, 4, 6, 9, 10, 11, 12],
+        "caus": 12,
+        "ccmixin": 1,
+        "ccnot": 1,
+        "cdot": [1, 11],
+        "certain": 12,
+        "cf": 12,
+        "ch": 1,
+        "chain": 12,
+        "chang": 1,
+        "charact": 5,
+        "check": 4,
+        "choic": 2,
+        "choos": 12,
+        "chosen": 12,
+        "circl": 12,
+        "circuit": [1, 4, 5, 11],
+        "cirq": [1, 5, 9, 12],
+        "cirq_circuit": 5,
+        "cirq_export": 5,
+        "cirq_qubit": 5,
+        "cirqexport": 5,
+        "class": [1, 2, 4, 5, 7, 11, 12],
+        "classic": [5, 10],
+        "classmethod": [1, 2, 4],
+        "client": [6, 12],
+        "closest": 10,
+        "cmixin": 1,
+        "cnot": [1, 4, 7, 11],
+        "code": [2, 4, 6, 7, 11],
+        "codebas": 11,
+        "coeffici": [4, 5, 6, 7, 11, 12],
+        "coincid": 11,
+        "collect": [1, 4, 7, 11],
+        "color": 12,
+        "com": 4,
+        "combin": [4, 12],
+        "come": 1,
+        "command": [9, 11],
+        "commun": 4,
+        "commut": [1, 12],
+        "compat": [1, 4],
+        "compil": [1, 2, 4, 5, 6, 7, 10],
+        "compiled_problem": [4, 11, 12],
+        "compiler_cli": [6, 11, 12],
+        "compiler_run": [4, 6],
+        "compilercli": [4, 6, 11, 12],
+        "compilerrun": [4, 6],
+        "complet": 12,
+        "compliant": 1,
+        "compon": 11,
+        "compos": 5,
+        "comput": [4, 7, 10, 11, 12],
+        "conda": 9,
+        "condit": [1, 4],
+        "configur": [1, 2, 4, 10, 12],
+        "conjug": 1,
+        "connect": [4, 5, 7, 11, 12],
+        "consid": 1,
+        "consol": 6,
+        "constraint": [1, 2, 4, 5, 7, 10, 11, 12],
+        "constraint_circuit": [4, 11, 12],
+        "constraint_connect": 7,
+        "constraint_data": 1,
+        "constraint_strength": [4, 12],
+        "construct": [1, 2, 4, 10, 12],
+        "constructor": 11,
+        "contact": [7, 11],
+        "contain": [1, 2, 4, 5, 10, 11, 12],
+        "context": 1,
+        "control": 1,
+        "control1": 1,
+        "control2": 1,
+        "control_qubit": 1,
+        "conveni": 12,
+        "convert": [1, 2, 4, 5, 12],
+        "convert_cnots_to_rzz": 1,
+        "coordin": [4, 7, 10],
+        "copi": [1, 4, 11],
+        "correct": 2,
+        "correctli": 9,
+        "correspond": [1, 2, 4, 5, 12],
+        "cost": 12,
+        "cost_expect": 12,
+        "cost_of_bitstr": 12,
+        "could": [2, 4],
+        "count": 12,
+        "coupler": 11,
+        "cours": 12,
+        "cover": 12,
+        "creat": [1, 4, 5, 7, 9, 11, 12],
+        "create_default_problem_circuit": 4,
+        "credenti": 11,
+        "crucial": 12,
+        "crx": 1,
+        "cry": 1,
+        "crz": 1,
+        "current": [1, 12],
+        "custom": [4, 8, 11],
+        "cut": 12,
+        "cy": 1,
+        "cz": 1,
+        "data": [1, 2, 4, 6],
+        "decod": [2, 8],
+        "decoding_map": [2, 11],
+        "decompos": 11,
+        "decreas": 12,
+        "deduc": 2,
+        "def": 12,
+        "default": [1, 2, 4, 6, 7, 11, 12],
+        "default_analog": 7,
+        "default_digit": 7,
+        "defin": [1, 4, 5, 7, 12],
+        "definit": 1,
+        "degener": 12,
+        "degeneraci": [2, 11],
+        "delta_i": 12,
+        "delta_j": 12,
+        "demonstr": 12,
+        "denot": 12,
+        "depend": 4,
+        "deprec": [1, 4],
+        "depth": 12,
+        "deriv": [1, 7],
+        "describ": [4, 7, 11, 12],
+        "design": 12,
+        "detail": [1, 11],
+        "determin": [4, 7, 12],
+        "devic": [2, 4, 5, 6, 8, 12],
+        "device_model": [4, 6, 7, 11, 12],
+        "device_typ": [4, 7],
+        "devicemodel": [4, 7, 11],
+        "devicemodelbas": [4, 7],
+        "diagon": 4,
+        "dict": [1, 2, 4, 5],
+        "dict_filt": 1,
+        "dictionari": [1, 2, 4, 5, 10, 12],
+        "differ": 12,
+        "digit": [4, 11, 12],
+        "digital_default": [4, 7],
+        "dimens": [6, 11, 12],
+        "dimension": [7, 12],
+        "direct": [4, 7],
+        "directli": [4, 10, 11],
+        "discuss": [7, 11],
+        "distanc": 2,
+        "divid": 1,
+        "do": [1, 4, 6, 7, 10, 11],
+        "document": 7,
+        "doe": [1, 2, 7, 10, 11],
+        "done": 10,
+        "dot": [1, 7, 12],
+        "driver": [4, 5, 11, 12],
+        "driver_circuit": [4, 11],
+        "e": [1, 2, 4, 7, 11, 12],
+        "e1500838": 12,
+        "each": [1, 2, 4, 5, 7, 9, 10, 11, 12],
+        "eas": 12,
+        "easi": 11,
+        "easili": 11,
+        "edg": [4, 12],
+        "edward": 12,
+        "eigenst": 12,
+        "eigenvalu": [1, 5],
+        "either": [1, 2, 4, 5, 7],
+        "elabor": 1,
+        "element": [1, 6, 7],
+        "emploi": 12,
+        "empti": [5, 11],
+        "enabl": 12,
+        "encod": [3, 4, 12],
+        "encode_problem": 4,
+        "encoding_map": [2, 11],
+        "end": [11, 12],
+        "energi": [4, 12],
+        "enforc": 12,
+        "enough": [2, 10],
+        "ensur": 12,
+        "enter": [9, 11],
+        "entir": 12,
+        "entri": 2,
+        "enumer": 12,
+        "environ": [9, 11, 12],
+        "equal": [1, 2, 4],
+        "equalityconstraint": [1, 4, 5],
+        "equival": [1, 2, 11],
+        "error": [1, 2],
+        "error_correct": [2, 10],
+        "especi": 2,
+        "et": 12,
+        "evalu": [1, 4, 12],
+        "evaluate_par": 1,
+        "even": [1, 2, 12],
+        "everi": [11, 12],
+        "everyon": 4,
+        "evolut": 12,
+        "exact": 4,
+        "exactli": [6, 12],
+        "exampl": [1, 4, 5, 7, 12],
+        "except": [1, 4, 6],
+        "excit": 12,
+        "execut": [4, 11, 12],
+        "execute_circuit": 12,
+        "exp": [4, 12],
+        "expans": 12,
+        "expect": 12,
+        "expectation_sum": 12,
+        "expens": 10,
+        "explain": 6,
+        "explan": 12,
+        "explicit": 5,
+        "exponenti": 4,
+        "export": [4, 12],
+        "expr": 5,
+        "express": [4, 5, 12],
+        "extend": [2, 4],
+        "extra": 4,
+        "f": 12,
+        "facilit": 2,
+        "factor": 5,
+        "fail": 2,
+        "failur": 6,
+        "fals": [1, 2],
+        "far": 12,
+        "farhi": 12,
+        "farhi14": 12,
+        "favor": 12,
+        "featur": [4, 7, 9],
+        "fellner": 12,
+        "fellner21": 12,
+        "few": [10, 11, 12],
+        "fewer": 10,
+        "field": [4, 7, 11],
+        "file": [1, 6],
+        "filenam": 1,
+        "filter": 1,
+        "final": [7, 11, 12],
+        "find": [10, 12],
+        "finish": 11,
+        "finit": 12,
+        "first": [5, 7, 11, 12],
+        "fix": [1, 4, 11],
+        "flag": 2,
+        "float": [1, 2, 4, 5],
+        "follow": [5, 6, 7, 9, 10, 11, 12],
+        "form": [1, 4, 5, 10, 11, 12],
+        "format": [1, 2, 4, 12],
+        "formula": 12,
+        "found": [1, 4, 11],
+        "four": [1, 11, 12],
+        "frac": [11, 12],
+        "framework": [1, 12],
+        "frequent": 12,
+        "from": [1, 2, 4, 5, 6, 7, 10, 11, 12],
+        "from_json": [1, 2, 4],
+        "from_nx_graph": 4,
+        "front": 12,
+        "frozenset": [1, 2, 4, 5],
+        "full": [2, 4, 10, 11],
+        "fulli": 1,
+        "fun": 12,
+        "function": [1, 4, 6, 12],
+        "futur": [4, 12],
+        "g": [1, 7, 12],
+        "gamma": [1, 5, 12],
+        "gamma_1": 12,
+        "gamma_p": 12,
+        "gap": 12,
+        "gate": [1, 4, 5, 7, 11, 12],
+        "gate1": 1,
+        "gate2": 1,
+        "gate3": 1,
+        "gate4": 1,
+        "gate_to_cirq": 5,
+        "gate_typ": 1,
+        "gateoper": 5,
+        "gener": [1, 2, 4, 5, 12],
+        "generate_flat_gate_sequ": 1,
+        "generate_qaoa": [5, 12],
+        "get": [1, 4, 6, 7, 12],
+        "get_backend": 12,
+        "get_compiler_run": [4, 6],
+        "get_count": 12,
+        "get_hermitian_conjug": 1,
+        "get_physical_configur": 12,
+        "get_solut": [4, 6],
+        "get_submiss": 4,
+        "give": [4, 12],
+        "given": [1, 2, 4, 5, 10, 11, 12],
+        "go": [2, 9, 10, 12],
+        "goal": 12,
+        "goldston": 12,
+        "graph": [4, 11, 12],
+        "green": 12,
+        "ground": 12,
+        "guarante": 12,
+        "gutmann": 12,
+        "h": [1, 4, 11, 12],
+        "h_": 12,
+        "h_e": 12,
+        "h_m": 12,
+        "ha": [1, 2, 4, 5, 7, 9, 10, 11, 12],
+        "hadamard": [1, 4],
+        "ham": 2,
+        "hamiltonian": [2, 4, 5, 11, 12],
+        "hand": 12,
+        "handl": [10, 12],
+        "hard": [4, 12],
+        "hardwar": [2, 7, 12],
+        "hashabl": [1, 4],
+        "hauk": 12,
+        "have": [1, 2, 4, 6, 7, 11, 12],
+        "help": 12,
+        "helper": 12,
+        "henc": 2,
+        "here": [6, 7, 10, 11, 12],
+        "hermitian": 1,
+        "hermitian_conjug": 1,
+        "hermitiangatemixin": 1,
+        "heurist": 12,
+        "high": 12,
+        "higher": 12,
+        "highest": 12,
+        "hold": [2, 6],
+        "horizont": 11,
+        "host": 4,
+        "how": [2, 4, 6, 7, 9, 10, 11, 12],
+        "howev": [6, 10],
+        "http": 12,
+        "http_backoff_factor": 4,
+        "http_retri": 4,
+        "http_timeout": 4,
+        "hybrid": 12,
+        "hyper": 12,
+        "hypergraph": 12,
+        "i": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
+        "id": 4,
+        "idea": 12,
+        "identifi": 1,
+        "implement": [1, 4, 7, 11, 12],
+        "import": [2, 5, 6, 7, 10, 11, 12],
+        "importerror": 4,
+        "improv": 12,
+        "includ": [1, 2, 4, 6, 11],
+        "include_triangl": 4,
+        "incomplet": 10,
+        "increas": 12,
+        "independ": [10, 12],
+        "index": 5,
+        "inf": 4,
+        "inform": [1, 4, 5, 6, 7, 9, 10, 11, 12],
+        "inherit": 1,
+        "initi": [1, 2, 4, 6, 12],
+        "initial_paramet": 12,
+        "initial_parameter_list": 12,
+        "initial_state_preparation_circuit": [4, 11],
+        "insid": [6, 9],
+        "instal": [8, 11],
+        "instanc": [1, 2, 4, 5, 12],
+        "instanti": [1, 5, 12],
+        "instead": [1, 2, 4, 5, 11],
+        "int": [1, 2, 4, 5, 12],
+        "integ": [4, 5, 7],
+        "intend": 1,
+        "intent": 4,
+        "interact": [4, 5, 6, 7, 11, 12],
+        "interest": 11,
+        "interfac": [5, 12],
+        "internet": 11,
+        "interpret": [1, 4],
+        "invers": 1,
+        "invok": 12,
+        "is_satisfi": 1,
+        "iswap": 1,
+        "item": [1, 5, 12],
+        "iter": [1, 4, 5, 11],
+        "itertool": 12,
+        "its": [1, 5],
+        "itself": 1,
+        "j": [7, 12],
+        "j_": 12,
+        "jeffrei": 12,
+        "job": 7,
+        "json": [1, 2, 4],
+        "json_wrap": 1,
+        "jsonloadsavemixin": 1,
+        "jsontyp": [1, 2, 4],
+        "just": [4, 7, 11],
+        "k": [4, 12],
+        "kei": [1, 2, 4, 12],
+        "keyword": 1,
+        "know": 11,
+        "kwarg": [1, 4],
+        "label": [1, 4, 5, 7, 12],
+        "langl": [4, 12],
+        "larg": 12,
+        "latter": 12,
+        "lattic": 4,
+        "layout": [7, 11, 12],
+        "lead": 12,
+        "least": 12,
+        "lechner": 12,
+        "lechner15": 12,
+        "left": [1, 5, 7, 12],
+        "length": [4, 7],
+        "let": [11, 12],
+        "lib": 5,
+        "librari": 2,
+        "light": 12,
+        "like": [1, 2, 4, 5, 6, 11],
+        "limit": 2,
+        "line": 7,
+        "list": [1, 2, 4, 6, 7, 10, 11],
+        "load": [1, 11],
+        "local": [1, 4, 5, 7, 11, 12],
+        "local_field": 7,
+        "locat": 12,
+        "logic": [2, 4, 10, 11, 12],
+        "logical_bitstr": 12,
+        "logical_configur": 10,
+        "logical_degeneraci": [2, 11],
+        "logical_problem_circuit": 4,
+        "logical_solut": 12,
+        "long": 10,
+        "longer": 12,
+        "look": [1, 12],
+        "loop": 1,
+        "lower": [5, 12],
+        "m": 9,
+        "made": [6, 11],
+        "mai": [4, 10, 11, 12],
+        "main": 12,
+        "make": [1, 4, 6, 8, 10, 11],
+        "make_arg": 1,
+        "make_args_and_kwargs_from_json": 1,
+        "make_full_configuration_from_parti": 2,
+        "mani": 12,
+        "manual": 11,
+        "map": [1, 2, 4, 5, 11],
+        "match": 1,
+        "math": 1,
+        "mathemat": 1,
+        "mathrm": 12,
+        "matter": 7,
+        "maxcut": 12,
+        "maximis": 12,
+        "maximum": 7,
+        "mbox": 4,
+        "mead": 12,
+        "mean": [1, 4, 6],
+        "meantim": 6,
+        "measur": 12,
+        "measure_al": 12,
+        "method": [1, 2, 4, 5, 10, 11, 12],
+        "michael": 12,
+        "might": [1, 4, 12],
+        "minim": [2, 10, 12],
+        "mix": 12,
+        "mixin": 1,
+        "model": [4, 6, 8, 11],
+        "modifi": 1,
+        "modify_angl": 1,
+        "modul": 5,
+        "moment": 1,
+        "more": [1, 9, 11, 12],
+        "most": [11, 12],
+        "motiv": 12,
+        "mul": 5,
+        "multi": 1,
+        "multicontrolledh": 1,
+        "multicontrolledri": 1,
+        "multicontrolledrx": 1,
+        "multicontrolledrz": 1,
+        "multicontrolmixin": 1,
+        "multipl": [11, 12],
+        "multipli": [1, 2],
+        "must": [1, 4, 5],
+        "mutual": 12,
+        "my": 7,
+        "my_device_model": 7,
+        "my_digital_device_model": 7,
+        "my_new_conda_env": 9,
+        "my_new_venv": 9,
+        "mydevicemodel": 7,
+        "mydigitaldevicemodel": 7,
+        "n_best_solut": 12,
+        "n_starting_point": 12,
+        "name": [1, 5, 9, 12],
+        "namedqubit": 5,
+        "nativ": [4, 11, 12],
+        "nearest": [2, 11],
+        "necessari": [1, 4],
+        "need": [1, 6, 7, 9, 11, 12],
+        "neighbor": [2, 11],
+        "nelder": 12,
+        "networkx": [4, 11],
+        "nevertheless": 7,
+        "new": [1, 4, 7],
+        "next": [7, 12],
+        "node": [4, 12],
+        "non": [4, 11],
+        "none": [1, 2, 4, 5, 12],
+        "nor": 1,
+        "normal": [4, 12],
+        "note": [1, 2, 10, 12],
+        "now": [4, 6, 7, 11, 12],
+        "np": 12,
+        "nshot": 12,
+        "null": 1,
+        "number": [1, 2, 4, 5, 12],
+        "numer": 4,
+        "numpi": [1, 5, 12],
+        "object": [1, 2, 4, 5, 6, 10, 11],
+        "obtain": [2, 4, 10, 12],
+        "off": 12,
+        "offer": 2,
+        "onc": 12,
+        "one": [1, 2, 4, 6, 7, 9, 12],
+        "ones": 4,
+        "onli": [1, 2, 5, 6, 7, 9, 10, 12],
+        "onto": [1, 5, 11],
+        "oper": [1, 4, 5],
+        "optim": [1, 4, 5, 6, 7, 8, 10],
+        "optimal_paramet": 12,
+        "optimal_qaoa_circuit": 12,
+        "optimization_problem": [4, 6, 7, 11, 12],
+        "optimized_paramet": 12,
+        "option": [1, 2, 4, 5, 9, 11, 12],
+        "order": [4, 5, 7, 10, 11, 12],
+        "org": 12,
+        "origin": [1, 2, 4, 11],
+        "other": [1, 4, 5, 12],
+        "other_paramet": 1,
+        "otherwis": [1, 4],
+        "our": 12,
+        "out": [2, 7, 11],
+        "outcom": 12,
+        "output": [1, 4, 5, 10, 12],
+        "over": [1, 11, 12],
+        "overhead": 12,
+        "p": [5, 12],
+        "packag": [5, 9],
+        "pair": [1, 4, 12],
+        "paralleliz": 12,
+        "param": [1, 5],
+        "paramet": [1, 2, 4, 5, 7, 12],
+        "parameter": 12,
+        "parameter_bound": [5, 12],
+        "parameter_map": [5, 12],
+        "parameter_nam": [1, 5],
+        "parameter_valu": 5,
+        "parametr": [1, 4, 12],
+        "parent": 1,
+        "pariti": [1, 2, 4, 5, 8, 11],
+        "parity_decod": 2,
+        "parity_encod": 2,
+        "parityconstraint": [1, 4, 11],
+        "paritydecod": [4, 10],
+        "paritydecoderextens": 2,
+        "parityencoderextens": 2,
+        "paritymap": 2,
+        "parityo": [3, 5, 6, 7, 9, 10, 12],
+        "parityos_addon": [3, 12],
+        "parityos_circuit": 5,
+        "parityos_output": [5, 6, 10, 11, 12],
+        "parityos_pass": 11,
+        "parityos_qubit": 5,
+        "parityos_us": [11, 12],
+        "parityosexcept": [2, 4, 11],
+        "parityosimporterror": 4,
+        "parityosoutput": [2, 4, 5, 6, 10, 11],
+        "parityqc": [4, 7, 11],
+        "part": [2, 12],
+        "partial": [2, 4],
+        "particular": 4,
+        "partit": 12,
+        "pass": [4, 7, 10, 11, 12],
+        "password": [11, 12],
+        "past": 11,
+        "pattern": [5, 12],
+        "pauli": [1, 4, 5],
+        "penalti": 4,
+        "per": [4, 6, 12],
+        "perform": [7, 12],
+        "person": 11,
+        "peter": 12,
+        "philipp": 12,
+        "phy": 12,
+        "physic": [2, 4, 10, 11, 12],
+        "physical_bitstr": 12,
+        "physical_configur": [10, 12],
+        "pi": 1,
+        "pick": 12,
+        "pip": 9,
+        "place": 4,
+        "plain": 11,
+        "plaquett": [4, 7, 11],
+        "pm": 1,
+        "point": 6,
+        "possibl": [1, 2, 4, 6, 7, 10, 11, 12],
+        "possibli": 11,
+        "preced": 1,
+        "precis": 12,
+        "prepar": 4,
+        "preprint": 12,
+        "present": 1,
+        "preset": [4, 7, 11],
+        "previou": 12,
+        "print": [11, 12],
+        "probabl": 11,
+        "problem": [2, 4, 5, 6, 7, 8, 9, 10],
+        "problem_circuit": 4,
+        "problem_represent": [4, 11],
+        "problemrepresent": [4, 5, 6, 7, 11, 12],
+        "process": [6, 11],
+        "prod_": 12,
+        "produc": 4,
+        "product": [1, 4, 5, 11, 12],
+        "prompt": 11,
+        "propag": [5, 11],
+        "properti": [1, 2, 4],
+        "proport": 4,
+        "provid": [1, 4, 7, 11, 12],
+        "psi": 12,
+        "psi_0": 12,
+        "pure": 5,
+        "put": 12,
+        "py": 5,
+        "python": [1, 6, 9],
+        "python3": 5,
+        "qaoa": [4, 5, 11],
+        "qaoa_circuit": [5, 12],
+        "qaoa_circuit_qiskit": 12,
+        "qasm_simul": 12,
+        "qiskit": [1, 5, 9, 12],
+        "qiskit_a": 12,
+        "qiskit_circuit": 5,
+        "qiskit_export": [5, 12],
+        "qiskitexport": [5, 12],
+        "quadrat": [11, 12],
+        "quantum": [4, 5, 7, 10, 11, 12],
+        "quantumcircuit": 5,
+        "qubit": [1, 2, 4, 5, 6, 7, 11, 12],
+        "qubit1": 1,
+        "qubit2": 1,
+        "qubit3": 1,
+        "qubit4": 1,
+        "qubit_arg": 1,
+        "qubit_connect": [4, 7],
+        "qubit_in_json": 4,
+        "qubit_index": 5,
+        "qubit_map": [5, 12],
+        "qubit_sit": 7,
+        "qubo": 12,
+        "quickstart": [6, 7, 8, 9],
+        "quit": 12,
+        "qutip": 1,
+        "rais": [1, 2, 6, 11],
+        "random": [2, 12],
+        "random_gener": 2,
+        "rang": [5, 12],
+        "rangl": 12,
+        "rank": 12,
+        "raw": 5,
+        "read": [1, 2, 12],
+        "readi": 12,
+        "readili": 12,
+        "real": 12,
+        "reason": 11,
+        "receiv": [1, 11],
+        "recommend": [1, 7, 9],
+        "reconstruct": 2,
+        "recov": [2, 10],
+        "rectangular": [4, 11],
+        "rectangularanalogdevic": [4, 6, 11, 12],
+        "rectangulardigitaldevic": [4, 11, 12],
+        "red": 12,
+        "reduc": 12,
+        "redund": [2, 10],
+        "refer": [2, 8],
+        "reflect": 1,
+        "reformul": 12,
+        "regist": 5,
+        "relat": [1, 4, 5, 9],
+        "relev": 7,
+        "remain": [5, 12],
+        "remap": 1,
+        "rememb": 9,
+        "remov": 12,
+        "repackag": 4,
+        "repeat": 12,
+        "repetit": 5,
+        "replac": [1, 4],
+        "replace_cnots_by_rzz": 4,
+        "repres": [1, 2, 4, 5, 11, 12],
+        "represent": [1, 4, 5, 11, 12],
+        "reproduc": 12,
+        "request": [4, 6, 7],
+        "resourc": [10, 12],
+        "respect": [9, 12],
+        "respons": [4, 5],
+        "result": [1, 4, 7, 10, 11, 12],
+        "retriev": 11,
+        "return": [1, 2, 4, 5, 6, 10, 11, 12],
+        "return_incomplet": 2,
+        "revers": 12,
+        "reward": 12,
+        "right": [5, 7, 12],
+        "rmixin": 1,
+        "rotat": [1, 4],
+        "round": 12,
+        "run": [4, 6, 7, 10, 11, 12],
+        "rx": [1, 4],
+        "rxx": 1,
+        "ry": 1,
+        "ryi": 1,
+        "rz": [1, 4],
+        "rz_fix": 1,
+        "rz_gate": 1,
+        "rz_theta": 1,
+        "rzz": 1,
+        "rzzzz": 1,
+        "s_": 12,
+        "s_0": 11,
+        "s_1": [1, 11, 12],
+        "s_1s_2": 12,
+        "s_1s_2s_3s_5": 12,
+        "s_1s_3": 12,
+        "s_2": [1, 11],
+        "s_2s_3": 12,
+        "s_2s_4": 12,
+        "s_2s_5": 12,
+        "s_3s_4": 12,
+        "s_3s_5": 12,
+        "s_4": 11,
+        "s_5": 12,
+        "s_i": 12,
+        "s_is_js_k": 12,
+        "s_j": 12,
+        "s_k": 12,
+        "s_n": 1,
+        "sam": 12,
+        "same": [1, 4, 5, 6, 12],
+        "satisfi": [1, 2, 4, 10, 12],
+        "save": [1, 12],
+        "scalabl": 12,
+        "schema": [4, 5],
+        "scienc": 12,
+        "scipi": 12,
+        "scratch": 7,
+        "second": [4, 5, 12],
+        "section": [6, 7, 9, 11, 12],
+        "secur": 11,
+        "see": [1, 6, 7, 9, 11, 12],
+        "seed": 12,
+        "seed_simul": 12,
+        "select": [1, 2, 12],
+        "select_reduced_readout_qubit": [2, 10],
+        "self": [1, 2, 4],
+        "sent": 6,
+        "separ": 4,
+        "sequenc": [1, 2, 4, 5, 11],
+        "serial": 2,
+        "serializ": [1, 4],
+        "server": 11,
+        "servic": 4,
+        "set": [1, 2, 4, 7, 10, 11, 12],
+        "setup": 2,
+        "sever": 5,
+        "shape": 4,
+        "shot": 12,
+        "should": [1, 4, 5, 6, 7],
+        "show": [2, 7, 11, 12],
+        "side": 11,
+        "similar": [2, 6],
+        "similarli": 11,
+        "simpl": 1,
+        "simpli": 12,
+        "simul": [1, 10],
+        "sinc": 12,
+        "singl": [1, 4, 6, 7, 10, 11, 12],
+        "site": [5, 7, 11],
+        "size": 4,
+        "small": 12,
+        "smallest": 2,
+        "snippet": 11,
+        "so": [4, 6, 7, 12],
+        "soft": 4,
+        "solut": [4, 6, 10],
+        "solv": 8,
+        "some": [2, 6, 12],
+        "sort": [1, 12],
+        "sourc": 9,
+        "spawn": 4,
+        "specif": [4, 7, 9, 11, 12],
+        "specifi": [1, 4, 7, 10, 12],
+        "spilt": 5,
+        "spin": [1, 2, 4, 5, 11, 12],
+        "spin_hamiltonian": [5, 9],
+        "spinz": [5, 9],
+        "spinz_constraint": 5,
+        "spinz_to_constraint": 5,
+        "spinz_to_hamiltonian": 5,
+        "splendid": 7,
+        "split": 12,
+        "squar": 7,
+        "standard": [1, 2, 4, 7, 9, 11],
+        "start": [4, 7, 11, 12],
+        "state": [2, 4, 10, 11, 12],
+        "static": 1,
+        "step": [7, 10, 11, 12],
+        "still": [2, 10],
+        "store": [1, 6, 10, 11],
+        "str": [1, 2, 4, 5, 12],
+        "strength": [4, 11],
+        "string": [1, 4, 5, 7],
+        "strongli": 7,
+        "subcircuit": 1,
+        "subclass": 1,
+        "subject": 1,
+        "submiss": [4, 7, 8, 11],
+        "submission_id": [4, 6],
+        "submit": [4, 6, 7, 9, 10, 12],
+        "subset": 12,
+        "subspac": 2,
+        "success": 11,
+        "successfulli": 11,
+        "suffic": 12,
+        "suit": 12,
+        "suitabl": [11, 12],
+        "sum": [5, 12],
+        "sum_": 12,
+        "suppli": 10,
+        "sure": 11,
+        "swap": 1,
+        "symbol": [1, 5],
+        "symmetri": 2,
+        "sympi": [1, 5],
+        "synchron": [4, 6, 11],
+        "system": [2, 10],
+        "tackl": 12,
+        "take": [1, 7, 12],
+        "target": [1, 4, 12],
+        "target_qubit": 1,
+        "task": 12,
+        "tell": [2, 4],
+        "term": [4, 5, 11, 12],
+        "text": 11,
+        "than": 12,
+        "thei": [1, 4, 12],
+        "them": [1, 4, 11, 12],
+        "therefor": 11,
+        "theta": [1, 4, 5, 11],
+        "thi": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
+        "third": 10,
+        "those": 1,
+        "three": [1, 10, 11],
+        "through": 11,
+        "thrown": 4,
+        "thu": 11,
+        "time": [4, 5, 6, 9, 11, 12],
+        "timeout": 4,
+        "to_cirq": 5,
+        "to_json": [1, 2, 4],
+        "to_qiskit": [5, 12],
+        "togeth": [4, 9],
+        "too": 12,
+        "tool": 5,
+        "topologi": 11,
+        "total": 12,
+        "transform": [2, 10],
+        "translat": 1,
+        "trial": 12,
+        "triangl": [4, 7, 10],
+        "tricki": 12,
+        "trivial": 2,
+        "true": [1, 2, 4, 12],
+        "try": [7, 10, 11, 12],
+        "tupl": [1, 4, 5],
+        "turquois": 12,
+        "tutori": 12,
+        "two": [1, 7, 10, 12],
+        "type": [1, 4, 7],
+        "u": [11, 12],
+        "unchang": 1,
+        "unconstrain": [4, 12],
+        "under": 12,
+        "underli": 1,
+        "uniform": 12,
+        "uninstal": 4,
+        "uniqu": 7,
+        "unitari": [5, 12],
+        "unitary_pattern": [5, 12],
+        "unord": 1,
+        "untie_spinz_product": 5,
+        "until": [6, 11],
+        "up": [1, 2, 12],
+        "updat": [1, 4, 12],
+        "upon": [4, 7],
+        "upper": 5,
+        "url_prefix": 4,
+        "us": [1, 2, 4, 5, 6, 7, 9, 10, 11, 12],
+        "usernam": [4, 11, 12],
+        "usr": 5,
+        "util": 1,
+        "v": 12,
+        "v1": 4,
+        "valid": [4, 5],
+        "valu": [1, 2, 4, 5, 7, 10, 12],
+        "variabl": [1, 4, 10, 11, 12],
+        "varieti": 12,
+        "vec": 12,
+        "venv": 9,
+        "version": [1, 4, 11, 12],
+        "vertic": 11,
+        "via": [9, 11, 12],
+        "view": 12,
+        "violat": [4, 12],
+        "virtual": 9,
+        "wa": [10, 11, 12],
+        "wai": [11, 12],
+        "wait": 6,
+        "walk": 11,
+        "want": [4, 5, 7, 9, 10, 11, 12],
+        "we": [1, 2, 5, 6, 7, 10, 11, 12],
+        "weight": 4,
+        "well": 7,
+        "went": 6,
+        "were": [2, 6, 12],
+        "when": [1, 2, 10, 11, 12],
+        "where": [1, 2, 4, 5, 6, 7, 10, 11, 12],
+        "whether": 1,
+        "which": [1, 2, 4, 5, 6, 7, 10, 11, 12],
+        "while": 10,
+        "whose": [4, 11],
+        "width": 4,
+        "without": 1,
+        "wolfgang": 12,
+        "work": [4, 6, 12],
+        "workflow": 12,
+        "would": [1, 4, 6, 7],
+        "write": 1,
+        "x": [1, 5, 6, 11, 12],
+        "xczxczxcz": 5,
+        "y": [1, 6, 11, 12],
+        "yellow": 12,
+        "you": [2, 4, 6, 7, 9, 10, 11, 12],
+        "your": [7, 11, 12],
+        "z": [1, 2, 4, 5, 7, 12],
+        "z_1": [4, 11],
+        "z_2": [4, 11],
+        "z_3": [4, 11],
+        "z_4": [4, 11],
+        "z_control": 1,
+        "z_control1": 1,
+        "z_control2": 1,
+        "zcx": 12,
+        "zero": [4, 12],
+        "zip": 12,
+        "zoller": 12,
+        "zz": [1, 4]
     },
+    "titles": ["parityos.api_interface", "parityos.base", "parityos.encodings", "API Reference", "parityos", "parityos_addons", "Asynchronous submissions", "Making a custom device model", "Welcome to ParityOS\u2019s documentation!", "Installation", "The Parity Decoder", "Quickstart", "Solving Optimization Problems"],
     "titleterms": {
-        "parityo": [0, 1, 2, 4, 8, 11],
-        "api_interfac": 0,
-        "base": 1,
-        "encod": 2,
+        "": 8,
+        "The": [10, 11, 12],
+        "algorithm": 12,
+        "an": 11,
+        "analog": 7,
         "api": 3,
-        "refer": 3,
-        "parityos_addon": 5,
+        "api_interfac": 0,
         "asynchron": 6,
-        "submiss": 6,
-        "obtain": 6,
-        "result": 6,
-        "exampl": [6, 10, 11],
-        "make": 7,
+        "base": 1,
+        "basic": 10,
+        "circuit": 12,
+        "classic": 12,
+        "client": 11,
+        "compil": [11, 12],
+        "content": 8,
+        "correct": 10,
         "custom": 7,
+        "decod": [10, 12],
+        "defin": 11,
         "devic": [7, 11],
-        "model": 7,
-        "analog": 7,
         "digit": 7,
-        "welcom": 8,
-        "": 8,
         "document": 8,
-        "content": 8,
-        "instal": 9,
-        "The": [10, 11, 12],
-        "pariti": [10, 12],
-        "decod": [10, 12],
-        "basic": 10,
+        "encod": 2,
         "error": 10,
-        "correct": 10,
-        "reduc": 10,
-        "read": 10,
-        "out": 10,
-        "select": 10,
-        "qubit": 10,
-        "quickstart": 11,
+        "exampl": [6, 10, 11],
+        "formul": 12,
         "initi": 11,
-        "client": 11,
-        "defin": 11,
-        "an": 11,
-        "optim": [11, 12],
-        "problem": [11, 12],
-        "target": 11,
-        "submit": 11,
+        "instal": 9,
         "job": 11,
-        "compil": [11, 12],
-        "output": 11,
-        "solv": 12,
-        "formul": 12,
+        "make": 7,
         "map": 12,
+        "model": 7,
+        "obtain": 6,
+        "optim": [11, 12],
+        "out": 10,
+        "output": 11,
+        "pariti": [10, 12],
+        "parityo": [0, 1, 2, 4, 8, 11],
+        "parityos_addon": 5,
+        "problem": [11, 12],
         "qaoa": 12,
+        "qubit": 10,
+        "quickstart": 11,
+        "read": 10,
+        "reduc": 10,
+        "refer": 3,
+        "result": 6,
+        "select": 10,
         "simul": 12,
-        "circuit": 12,
-        "classic": 12,
         "solut": 12,
-        "algorithm": 12
-    },
-    "envversion": {
-        "sphinx.domains.c": 3,
-        "sphinx.domains.changeset": 1,
-        "sphinx.domains.citation": 1,
-        "sphinx.domains.cpp": 9,
-        "sphinx.domains.index": 1,
-        "sphinx.domains.javascript": 3,
-        "sphinx.domains.math": 2,
-        "sphinx.domains.python": 4,
-        "sphinx.domains.rst": 2,
-        "sphinx.domains.std": 2,
-        "sphinx": 60
-    },
-    "alltitles": {
-        "parityos.api_interface": [
-            [0, "module-parityos.api_interface"]
-        ],
-        "parityos.base": [
-            [1, "module-parityos.base.constraints"]
-        ],
-        "parityos.encodings": [
-            [2, "module-parityos.encodings.mappings"]
-        ],
-        "API Reference": [
-            [3, "api-reference"]
-        ],
-        "parityos": [
-            [4, "module-parityos"]
-        ],
-        "parityos_addons": [
-            [5, "module-parityos_addons.interfaces"]
-        ],
-        "Asynchronous submissions": [
-            [6, "asynchronous-submissions"]
-        ],
-        "Submission": [
-            [6, "submission"]
-        ],
-        "Obtaining results": [
-            [6, "obtaining-results"]
-        ],
-        "Examples": [
-            [6, "examples"],
-            [11, "examples"]
-        ],
-        "Making a custom device model": [
-            [7, "making-a-custom-device-model"]
-        ],
-        "Device models": [
-            [7, "device-models"]
-        ],
-        "Analog device model": [
-            [7, "analog-device-model"]
-        ],
-        "Digital device model": [
-            [7, "digital-device-model"]
-        ],
-        "Welcome to ParityOS\u2019s documentation!": [
-            [8, "welcome-to-parityos-s-documentation"]
-        ],
-        "Contents:": [
-            [8, null]
-        ],
-        "Installation": [
-            [9, "installation"]
-        ],
-        "The Parity Decoder": [
-            [10, "the-parity-decoder"]
-        ],
-        "Basic example": [
-            [10, "basic-example"]
-        ],
-        "Error correction": [
-            [10, "error-correction"]
-        ],
-        "Reduced read-out": [
-            [10, "reduced-read-out"]
-        ],
-        "Selecting qubits for read-out": [
-            [10, "selecting-qubits-for-read-out"]
-        ],
-        "Quickstart": [
-            [11, "quickstart"]
-        ],
-        "Initializing the Client": [
-            [11, "initializing-the-client"]
-        ],
-        "Defining an optimization problem": [
-            [11, "defining-an-optimization-problem"]
-        ],
-        "Defining a Target Device": [
-            [11, "defining-a-target-device"]
-        ],
-        "Submitting a Job to the Compiler": [
-            [11, "submitting-a-job-to-the-compiler"]
-        ],
-        "The ParityOS output": [
-            [11, "the-parityos-output"]
-        ],
-        "Solving Optimization Problems": [
-            [12, "solving-optimization-problems"]
-        ],
-        "Problem Formulation": [
-            [12, "problem-formulation"]
-        ],
-        "Parity Mapping and Compilation": [
-            [12, "parity-mapping-and-compilation"]
-        ],
-        "QAOA Optimization and Simulation": [
-            [12, "qaoa-optimization-and-simulation"]
-        ],
-        "The QAOA circuit": [
-            [12, "the-qaoa-circuit"]
-        ],
-        "Classical Optimization": [
-            [12, "classical-optimization"]
-        ],
-        "Solutions of the QAOA algorithm and decoding": [
-            [12, "solutions-of-the-qaoa-algorithm-and-decoding"]
-        ]
-    },
-    "indexentries": {
-        "module": [
-            [0, "module-parityos.api_interface"],
-            [1, "module-parityos.base.circuit"],
-            [1, "module-parityos.base.constraints"],
-            [1, "module-parityos.base.gates"],
-            [1, "module-parityos.base.utils"],
-            [2, "module-parityos.encodings.mappings"],
-            [2, "module-parityos.encodings.parity_decoder"],
-            [2, "module-parityos.encodings.parity_encoder"],
-            [4, "module-parityos"],
-            [5, "module-parityos_addons.interfaces"],
-            [5, "module-parityos_addons.qaoa"],
-            [5, "module-parityos_addons.spin_hamiltonians"]
-        ],
-        "parityos.api_interface": [
-            [0, "module-parityos.api_interface"]
-        ],
-        "ccnot (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.CCNOT"]
-        ],
-        "cnot (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.CNOT"]
-        ],
-        "cz (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.CZ"]
-        ],
-        "circuit (class in parityos.base.circuit)": [
-            [1, "parityos.base.circuit.Circuit"]
-        ],
-        "equalityconstraint (class in parityos.base.constraints)": [
-            [1, "parityos.base.constraints.EqualityConstraint"]
-        ],
-        "gate (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Gate"]
-        ],
-        "gate1 (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Gate1"]
-        ],
-        "gate2 (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Gate2"]
-        ],
-        "gate3 (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Gate3"]
-        ],
-        "gate4 (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Gate4"]
-        ],
-        "h (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.H"]
-        ],
-        "hermitiangatemixin (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.HermitianGateMixin"]
-        ],
-        "jsonloadsavemixin (class in parityos.base.utils)": [
-            [1, "parityos.base.utils.JSONLoadSaveMixin"]
-        ],
-        "parityconstraint (class in parityos.base.constraints)": [
-            [1, "parityos.base.constraints.ParityConstraint"]
-        ],
-        "rmixin (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.RMixin"]
-        ],
-        "rx (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Rx"]
-        ],
-        "ry (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Ry"]
-        ],
-        "rz (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Rz"]
-        ],
-        "rzz (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Rzz"]
-        ],
-        "x (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.X"]
-        ],
-        "y (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Y"]
-        ],
-        "z (class in parityos.base.gates)": [
-            [1, "parityos.base.gates.Z"]
-        ],
-        "__init__() (parityos.base.constraints.equalityconstraint method)": [
-            [1, "parityos.base.constraints.EqualityConstraint.__init__"]
-        ],
-        "__init__() (parityos.base.constraints.parityconstraint method)": [
-            [1, "parityos.base.constraints.ParityConstraint.__init__"]
-        ],
-        "__init__() (parityos.base.gates.ccnot method)": [
-            [1, "parityos.base.gates.CCNOT.__init__"]
-        ],
-        "__init__() (parityos.base.gates.cnot method)": [
-            [1, "parityos.base.gates.CNOT.__init__"]
-        ],
-        "__init__() (parityos.base.gates.cz method)": [
-            [1, "parityos.base.gates.CZ.__init__"]
-        ],
-        "__init__() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.__init__"]
-        ],
-        "__init__() (parityos.base.gates.gate1 method)": [
-            [1, "parityos.base.gates.Gate1.__init__"]
-        ],
-        "__init__() (parityos.base.gates.gate2 method)": [
-            [1, "parityos.base.gates.Gate2.__init__"]
-        ],
-        "__init__() (parityos.base.gates.gate3 method)": [
-            [1, "parityos.base.gates.Gate3.__init__"]
-        ],
-        "__init__() (parityos.base.gates.gate4 method)": [
-            [1, "parityos.base.gates.Gate4.__init__"]
-        ],
-        "__init__() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.__init__"]
-        ],
-        "convert_cnots_to_rzzs() (in module parityos.base.circuit)": [
-            [1, "parityos.base.circuit.convert_cnots_to_rzzs"]
-        ],
-        "dict_filter() (in module parityos.base.utils)": [
-            [1, "parityos.base.utils.dict_filter"]
-        ],
-        "evaluate_parity() (in module parityos.base.constraints)": [
-            [1, "parityos.base.constraints.evaluate_parity"]
-        ],
-        "from_json() (parityos.base.circuit.circuit class method)": [
-            [1, "parityos.base.circuit.Circuit.from_json"]
-        ],
-        "from_json() (parityos.base.constraints.equalityconstraint class method)": [
-            [1, "parityos.base.constraints.EqualityConstraint.from_json"]
-        ],
-        "from_json() (parityos.base.gates.gate class method)": [
-            [1, "parityos.base.gates.Gate.from_json"]
-        ],
-        "from_json() (parityos.base.gates.rmixin class method)": [
-            [1, "parityos.base.gates.RMixin.from_json"]
-        ],
-        "from_json() (parityos.base.utils.jsonloadsavemixin class method)": [
-            [1, "parityos.base.utils.JSONLoadSaveMixin.from_json"]
-        ],
-        "generate_flat_gate_sequence() (parityos.base.circuit.circuit method)": [
-            [1, "parityos.base.circuit.Circuit.generate_flat_gate_sequence"]
-        ],
-        "get_hermitian_conjugate() (parityos.base.circuit.circuit method)": [
-            [1, "parityos.base.circuit.Circuit.get_hermitian_conjugate"]
-        ],
-        "get_hermitian_conjugate() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.get_hermitian_conjugate"]
-        ],
-        "get_hermitian_conjugate() (parityos.base.gates.hermitiangatemixin method)": [
-            [1, "parityos.base.gates.HermitianGateMixin.get_hermitian_conjugate"]
-        ],
-        "get_hermitian_conjugate() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.get_hermitian_conjugate"]
-        ],
-        "is_satisfied() (parityos.base.constraints.equalityconstraint method)": [
-            [1, "parityos.base.constraints.EqualityConstraint.is_satisfied"]
-        ],
-        "json_wrap() (in module parityos.base.utils)": [
-            [1, "parityos.base.utils.json_wrap"]
-        ],
-        "load() (parityos.base.utils.jsonloadsavemixin class method)": [
-            [1, "parityos.base.utils.JSONLoadSaveMixin.load"]
-        ],
-        "make_args() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.make_args"]
-        ],
-        "make_args() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.make_args"]
-        ],
-        "modify_angle() (parityos.base.circuit.circuit method)": [
-            [1, "parityos.base.circuit.Circuit.modify_angle"]
-        ],
-        "modify_angle() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.modify_angle"]
-        ],
-        "modify_angle() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.modify_angle"]
-        ],
-        "parameters (parityos.base.circuit.circuit property)": [
-            [1, "parityos.base.circuit.Circuit.parameters"]
-        ],
-        "parameters (parityos.base.gates.rmixin property)": [
-            [1, "parityos.base.gates.RMixin.parameters"]
-        ],
-        "parityos.base.circuit": [
-            [1, "module-parityos.base.circuit"]
-        ],
-        "parityos.base.constraints": [
-            [1, "module-parityos.base.constraints"]
-        ],
-        "parityos.base.gates": [
-            [1, "module-parityos.base.gates"]
-        ],
-        "parityos.base.utils": [
-            [1, "module-parityos.base.utils"]
-        ],
-        "qubit (parityos.base.gates.gate1 property)": [
-            [1, "parityos.base.gates.Gate1.qubit"]
-        ],
-        "qubits (parityos.base.circuit.circuit property)": [
-            [1, "parityos.base.circuit.Circuit.qubits"]
-        ],
-        "qubits (parityos.base.gates.gate property)": [
-            [1, "parityos.base.gates.Gate.qubits"]
-        ],
-        "remap() (parityos.base.circuit.circuit method)": [
-            [1, "parityos.base.circuit.Circuit.remap"]
-        ],
-        "remap() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.remap"]
-        ],
-        "remap() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.remap"]
-        ],
-        "save() (parityos.base.utils.jsonloadsavemixin method)": [
-            [1, "parityos.base.utils.JSONLoadSaveMixin.save"]
-        ],
-        "to_json() (parityos.base.circuit.circuit method)": [
-            [1, "parityos.base.circuit.Circuit.to_json"]
-        ],
-        "to_json() (parityos.base.constraints.equalityconstraint method)": [
-            [1, "parityos.base.constraints.EqualityConstraint.to_json"]
-        ],
-        "to_json() (parityos.base.gates.gate method)": [
-            [1, "parityos.base.gates.Gate.to_json"]
-        ],
-        "to_json() (parityos.base.gates.rmixin method)": [
-            [1, "parityos.base.gates.RMixin.to_json"]
-        ],
-        "to_json() (parityos.base.utils.jsonloadsavemixin method)": [
-            [1, "parityos.base.utils.JSONLoadSaveMixin.to_json"]
-        ],
-        "mappings (class in parityos.encodings.mappings)": [
-            [2, "parityos.encodings.mappings.Mappings"]
-        ],
-        "paritydecoderextension (class in parityos.encodings.parity_decoder)": [
-            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension"]
-        ],
-        "parityencoderextension (class in parityos.encodings.parity_encoder)": [
-            [2, "parityos.encodings.parity_encoder.ParityEncoderExtension"]
-        ],
-        "paritymap (class in parityos.encodings.mappings)": [
-            [2, "parityos.encodings.mappings.ParityMap"]
-        ],
-        "__init__() (parityos.encodings.mappings.mappings method)": [
-            [2, "parityos.encodings.mappings.Mappings.__init__"]
-        ],
-        "__init__() (parityos.encodings.mappings.paritymap method)": [
-            [2, "parityos.encodings.mappings.ParityMap.__init__"]
-        ],
-        "decode() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
-            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.decode"]
-        ],
-        "encode() (parityos.encodings.parity_encoder.parityencoderextension method)": [
-            [2, "parityos.encodings.parity_encoder.ParityEncoderExtension.encode"]
-        ],
-        "error_correct() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
-            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.error_correct"]
-        ],
-        "from_json() (parityos.encodings.mappings.mappings class method)": [
-            [2, "parityos.encodings.mappings.Mappings.from_json"]
-        ],
-        "from_json() (parityos.encodings.mappings.paritymap class method)": [
-            [2, "parityos.encodings.mappings.ParityMap.from_json"]
-        ],
-        "logical_degeneracies (parityos.encodings.mappings.mappings property)": [
-            [2, "parityos.encodings.mappings.Mappings.logical_degeneracies"]
-        ],
-        "make_full_configuration_from_partial() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
-            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.make_full_configuration_from_partial"]
-        ],
-        "parityos.encodings.mappings": [
-            [2, "module-parityos.encodings.mappings"]
-        ],
-        "parityos.encodings.parity_decoder": [
-            [2, "module-parityos.encodings.parity_decoder"]
-        ],
-        "parityos.encodings.parity_encoder": [
-            [2, "module-parityos.encodings.parity_encoder"]
-        ],
-        "select_reduced_readout_qubits() (parityos.encodings.parity_decoder.paritydecoderextension method)": [
-            [2, "parityos.encodings.parity_decoder.ParityDecoderExtension.select_reduced_readout_qubits"]
-        ],
-        "to_json() (parityos.encodings.mappings.mappings method)": [
-            [2, "parityos.encodings.mappings.Mappings.to_json"]
-        ],
-        "to_json() (parityos.encodings.mappings.paritymap method)": [
-            [2, "parityos.encodings.mappings.ParityMap.to_json"]
-        ],
-        "compilerclient (class in parityos)": [
-            [4, "parityos.CompilerClient"]
-        ],
-        "hamiltonian (class in parityos)": [
-            [4, "parityos.Hamiltonian"]
-        ],
-        "parityosexception": [
-            [4, "parityos.ParityOSException"]
-        ],
-        "parityosimporterror": [
-            [4, "parityos.ParityOSImportError"]
-        ],
-        "parityosoutput (class in parityos)": [
-            [4, "parityos.ParityOSOutput"]
-        ],
-        "problemrepresentation (class in parityos)": [
-            [4, "parityos.ProblemRepresentation"]
-        ],
-        "qubit (class in parityos)": [
-            [4, "parityos.Qubit"]
-        ],
-        "rectangularanalogdevice (class in parityos)": [
-            [4, "parityos.RectangularAnalogDevice"]
-        ],
-        "rectangulardigitaldevice (class in parityos)": [
-            [4, "parityos.RectangularDigitalDevice"]
-        ],
-        "__init__() (parityos.hamiltonian method)": [
-            [4, "parityos.Hamiltonian.__init__"]
-        ],
-        "__init__() (parityos.parityosoutput method)": [
-            [4, "parityos.ParityOSOutput.__init__"]
-        ],
-        "__init__() (parityos.problemrepresentation method)": [
-            [4, "parityos.ProblemRepresentation.__init__"]
-        ],
-        "__init__() (parityos.qubit method)": [
-            [4, "parityos.Qubit.__init__"]
-        ],
-        "__init__() (parityos.rectangularanalogdevice method)": [
-            [4, "parityos.RectangularAnalogDevice.__init__"]
-        ],
-        "__init__() (parityos.rectangulardigitaldevice method)": [
-            [4, "parityos.RectangularDigitalDevice.__init__"]
-        ],
-        "compile() (parityos.compilerclient method)": [
-            [4, "parityos.CompilerClient.compile"]
-        ],
-        "create_default_problem_circuit() (parityos.parityosoutput method)": [
-            [4, "parityos.ParityOSOutput.create_default_problem_circuit"]
-        ],
-        "encode_problem() (parityos.parityosoutput method)": [
-            [4, "parityos.ParityOSOutput.encode_problem"]
-        ],
-        "evaluate() (parityos.problemrepresentation method)": [
-            [4, "parityos.ProblemRepresentation.evaluate"]
-        ],
-        "from_json() (parityos.parityosoutput class method)": [
-            [4, "parityos.ParityOSOutput.from_json"]
-        ],
-        "from_json() (parityos.problemrepresentation class method)": [
-            [4, "parityos.ProblemRepresentation.from_json"]
-        ],
-        "from_json() (parityos.qubit class method)": [
-            [4, "parityos.Qubit.from_json"]
-        ],
-        "from_nx_graph() (parityos.problemrepresentation class method)": [
-            [4, "parityos.ProblemRepresentation.from_nx_graph"]
-        ],
-        "get_compiler_runs() (parityos.compilerclient method)": [
-            [4, "parityos.CompilerClient.get_compiler_runs"]
-        ],
-        "get_solutions() (parityos.compilerclient method)": [
-            [4, "parityos.CompilerClient.get_solutions"]
-        ],
-        "get_submission() (parityos.compilerclient method)": [
-            [4, "parityos.CompilerClient.get_submission"]
-        ],
-        "logical_problem_circuit (parityos.parityosoutput property)": [
-            [4, "parityos.ParityOSOutput.logical_problem_circuit"]
-        ],
-        "parityos": [
-            [4, "module-parityos"]
-        ],
-        "qubits (parityos.problemrepresentation property)": [
-            [4, "parityos.ProblemRepresentation.qubits"]
-        ],
-        "replace_cnots_by_rzzs() (parityos.parityosoutput method)": [
-            [4, "parityos.ParityOSOutput.replace_cnots_by_rzzs"]
-        ],
-        "submit() (parityos.compilerclient method)": [
-            [4, "parityos.CompilerClient.submit"]
-        ],
-        "terms (parityos.problemrepresentation property)": [
-            [4, "parityos.ProblemRepresentation.terms"]
-        ],
-        "to_json() (parityos.parityosoutput method)": [
-            [4, "parityos.ParityOSOutput.to_json"]
-        ],
-        "to_json() (parityos.problemrepresentation method)": [
-            [4, "parityos.ProblemRepresentation.to_json"]
-        ],
-        "to_json() (parityos.qubit method)": [
-            [4, "parityos.Qubit.to_json"]
-        ],
-        "cirqexporter (class in parityos_addons.interfaces)": [
-            [5, "parityos_addons.interfaces.CirqExporter"]
-        ],
-        "qiskitexporter (class in parityos_addons.interfaces)": [
-            [5, "parityos_addons.interfaces.QiskitExporter"]
-        ],
-        "spinz (class in parityos_addons.spin_hamiltonians)": [
-            [5, "parityos_addons.spin_hamiltonians.SpinZ"]
-        ],
-        "__init__() (parityos_addons.interfaces.cirqexporter method)": [
-            [5, "parityos_addons.interfaces.CirqExporter.__init__"]
-        ],
-        "__init__() (parityos_addons.interfaces.qiskitexporter method)": [
-            [5, "parityos_addons.interfaces.QiskitExporter.__init__"]
-        ],
-        "gate_to_cirq() (parityos_addons.interfaces.cirqexporter method)": [
-            [5, "parityos_addons.interfaces.CirqExporter.gate_to_cirq"]
-        ],
-        "gate_to_qiskit() (parityos_addons.interfaces.qiskitexporter method)": [
-            [5, "parityos_addons.interfaces.QiskitExporter.gate_to_qiskit"]
-        ],
-        "generate_qaoa() (in module parityos_addons.qaoa)": [
-            [5, "parityos_addons.qaoa.generate_qaoa"]
-        ],
-        "parityos_addons.interfaces": [
-            [5, "module-parityos_addons.interfaces"]
-        ],
-        "parityos_addons.qaoa": [
-            [5, "module-parityos_addons.qaoa"]
-        ],
-        "parityos_addons.spin_hamiltonians": [
-            [5, "module-parityos_addons.spin_hamiltonians"]
-        ],
-        "spinz_to_constraint() (in module parityos_addons.spin_hamiltonians)": [
-            [5, "parityos_addons.spin_hamiltonians.spinz_to_constraint"]
-        ],
-        "spinz_to_hamiltonian() (in module parityos_addons.spin_hamiltonians)": [
-            [5, "parityos_addons.spin_hamiltonians.spinz_to_hamiltonian"]
-        ],
-        "to_cirq() (parityos_addons.interfaces.cirqexporter method)": [
-            [5, "parityos_addons.interfaces.CirqExporter.to_cirq"]
-        ],
-        "to_qiskit() (parityos_addons.interfaces.qiskitexporter method)": [
-            [5, "parityos_addons.interfaces.QiskitExporter.to_qiskit"]
-        ],
-        "untie_spinz_product() (in module parityos_addons.spin_hamiltonians)": [
-            [5, "parityos_addons.spin_hamiltonians.untie_spinz_product"]
-        ]
+        "solv": 12,
+        "submiss": 6,
+        "submit": 11,
+        "target": 11,
+        "welcom": 8
     }
 })
```

### Comparing `parityos-2.4.0/parityos_addons/documentation/html/tutorial.html` & `parityos-2.5.0/parityos_addons/documentation/html/tutorial.html`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
         <script src="_static/documentation_options.js?v=841abef3"></script>
-        <script src="_static/doctools.js?v=888ff710"></script>
+        <script src="_static/doctools.js?v=9a2dae69"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
         <script async="async" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="API Reference" href="api_reference/index.html" />
     <link rel="prev" title="The Parity Decoder" href="parity_decoder.html" />
```

### Comparing `parityos-2.4.0/parityos_addons/examples/example1.py` & `parityos-2.5.0/parityos_addons/examples/example1.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/examples/example2.py` & `parityos-2.5.0/parityos_addons/examples/example2.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/examples/example3.py` & `parityos-2.5.0/parityos_addons/examples/example3.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/examples/example4.py` & `parityos-2.5.0/parityos_addons/examples/example4.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/examples/example5.py` & `parityos-2.5.0/parityos_addons/examples/example5.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/examples/runner.py` & `parityos-2.5.0/parityos_addons/examples/runner.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/interfaces/__init__.py` & `parityos-2.5.0/parityos_addons/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/interfaces/cirq_exporter.py` & `parityos-2.5.0/parityos_addons/interfaces/cirq_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,62 @@
 Tools to export ParityOS circuits to Cirq.
 """
 from collections.abc import Mapping
 from math import pi
 from typing import Union
 
 from parityos.base.circuit import CircuitElement
-from parityos.base.gates import Qubit, Gate, RMixin, CNOT, H, X, Y, Z, Rx, Ry, Rz, Rzz, CCNOT, CZ
+from parityos.base.gates import (
+    CCNOT,
+    CNOT,
+    CZ,
+    Gate,
+    H,
+    ISwap,
+    Qubit,
+    RMixin,
+    Rx,
+    Rxx,
+    Ry,
+    Ryy,
+    Rz,
+    Rzz,
+    Swap,
+    X,
+    Y,
+    Z,
+)
 from parityos.base.exceptions import ParityOSImportError
 
 try:
     import cirq
 except ImportError:
     raise ParityOSImportError("The Cirq exporter requires the installation of Cirq.")
 
 
 GATE_MAP: dict[type(Gate), cirq.Gate] = {
     Gate: NotImplemented,  # Added to improve the type checking in PyCharm
     # All keys must be subclasses of the Gate class.
+    # CH: NotImplemented,
+    # CY: NotImplemented,
+    CCNOT: cirq.CCNOT,
     CNOT: cirq.CNOT,
-    X: cirq.X,
-    Y: cirq.Y,
-    Z: cirq.Z,
+    CZ: cirq.CZ,
     H: cirq.H,
+    ISwap: cirq.ISWAP,
     Rx: cirq.XPowGate,  # We use _PowGate for consistency with Rzz: ZZPowGate
+    Rxx: cirq.XXPowGate,  # cirq.Rzz does not exist.
     Ry: cirq.YPowGate,  # We use _PowGate for consistency with Rzz: ZZPowGate
+    Ryy: cirq.YYPowGate,  # cirq.Rzz does not exist.
     Rz: cirq.ZPowGate,  # We use _PowGate for consistency with Rzz: ZZPowGate
     Rzz: cirq.ZZPowGate,  # cirq.Rzz does not exist.
-    CCNOT: cirq.CCNOT,
-    CZ: cirq.CZ,
+    Swap: cirq.SWAP,
+    X: cirq.X,
+    Y: cirq.Y,
+    Z: cirq.Z,
 }
 
 CirqCircuitElement = Union[cirq.GateOperation, "CirqCircuitElement"]
 
 
 class CirqExporter:
     """
```

### Comparing `parityos-2.4.0/parityos_addons/interfaces/openqasm_exporter.py` & `parityos-2.5.0/parityos_addons/interfaces/openqasm_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,56 @@
 
 Tools to export ParityOS circuits to OpenQASM.
 """
 from collections.abc import Iterable, Mapping
 import re
 
 from parityos.base.circuit import CircuitElement
-from parityos.base.gates import Gate, CCNOT, CNOT, H, RMixin, Rx, Ry, Rz, X, Y, Z, CZ
+from parityos.base.gates import (
+    CCNOT,
+    CH,
+    CNOT,
+    CRz,
+    CY,
+    CZ,
+    Gate,
+    H,
+    RMixin,
+    Rx,
+    Ry,
+    Rz,
+    Swap,
+    X,
+    Y,
+    Z,
+)
 from parityos.base.qubits import Qubit, QubitLabel
 
 
 GATE_MAP: dict[type[Gate], str] = {
     CCNOT: "ccx",
+    CH: "ch",
     CNOT: "CX",
     # In OpenQASM 2, "CX" is a built-in statement, "cx" is an alias from "qelib1.inc".
     # In OpenQASM 3, both "CX" and "cx" are defined in the standard gates library "stdgates.inc".
+    CY: "cy",
+    CZ: "cz",
+    # CRx: NotImplemented,
+    # CRy: NotImplemented,
+    CRz: "crz",
     H: "h",
+    # ISwap: NotImplemented,
     Rx: "rx",
     Ry: "ry",
     Rz: "rz",
     # Rzz: NotImplemented,
+    Swap: "swap",
     X: "x",
     Y: "y",
     Z: "z",
-    CZ: "CZ",
 }
 
 # A qubit map should map the ParityOS Qubit instances onto valid OpenQASM string identifiers,
 # either as individual identifiers "q1", "q2", ..., or indexed registers "qa[1]", "qb[2]", ...
 QubitMap = Mapping[Qubit, str]  # type: TypeAlias
 
 
@@ -255,15 +279,15 @@
                 )
             )
             openqasm_instruction = f"{openqasm_gate}({angle})"
         else:
             openqasm_instruction = openqasm_gate
 
         qubit_indices = ",".join(
-            qubit_map[qubit] for qubit in gate.make_args() if isinstance(qubit, Qubit)
+            qubit_map[qubit] for qubit in gate.qubit_list if isinstance(qubit, Qubit)
         )
         return f"{openqasm_instruction} {qubit_indices};"
 
     def _get_openqasm_header_lines(self) -> list[str]:
         """Helper method that generates a list with the header lines of the OpenQASM program."""
         standard_library = "qelib1.inc" if self.openqasm_version == "2.0" else "stdgates.inc"
         return [
```

### Comparing `parityos-2.4.0/parityos_addons/interfaces/qiskit_exporter.py` & `parityos-2.5.0/parityos_addons/interfaces/qiskit_exporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,36 +7,75 @@
 All rights reserved.
 
 Tools to export ParityOS circuits to Qiskit.
 """
 from collections.abc import Iterable, Mapping
 
 from parityos.base.circuit import CircuitElement
-from parityos.base.gates import Qubit, Gate, RMixin, CNOT, H, X, Y, Z, Rx, Ry, Rz, Rzz, CCNOT, CZ
+from parityos.base.gates import (
+    CCNOT,
+    CNOT,
+    CRx,
+    CRy,
+    CRz,
+    CY,
+    CZ,
+    Gate,
+    H,
+    ISwap,
+    MultiControlMixin,
+    MultiControlledH,
+    MultiControlledRx,
+    MultiControlledRy,
+    MultiControlledRz,
+    Qubit,
+    RMixin,
+    Rx,
+    Rxx,
+    Ry,
+    Ryy,
+    Rz,
+    Rzz,
+    Swap,
+    X,
+    Y,
+    Z,
+)
 from parityos.base.exceptions import ParityOSImportError
 
 try:
     import qiskit
     import qiskit.circuit.library as qiskit_library
 except ImportError:
     raise ParityOSImportError("The Qiskit exporter requires the installation of Qiskit")
 
-
 GATE_MAP: dict[type[Gate], type[qiskit.circuit.gate.Gate]] = {
+    CCNOT: qiskit_library.CCXGate,
     CNOT: qiskit_library.CXGate,
+    CRx: qiskit_library.CRXGate,
+    CRy: qiskit_library.CRYGate,
+    CRz: qiskit_library.CRZGate,
+    CY: qiskit_library.CYGate,
+    CZ: qiskit_library.CZGate,
     H: qiskit_library.HGate,
-    X: qiskit_library.XGate,
-    Y: qiskit_library.YGate,
-    Z: qiskit_library.ZGate,
+    ISwap: qiskit_library.iSwapGate,
+    MultiControlledH: qiskit_library.HGate,  # Will be remapped by qiskit_library.MCMT.
+    MultiControlledRx: qiskit_library.RXGate,  # Will be remapped by qiskit_library.MCMT.
+    MultiControlledRy: qiskit_library.RYGate,  # Will be remapped by qiskit_library.MCMT.
+    MultiControlledRz: qiskit_library.RZGate,  # Will be remapped by qiskit_library.MCMT.
     Rx: qiskit_library.RXGate,
+    Rxx: qiskit_library.RXXGate,
     Ry: qiskit_library.RYGate,
+    Ryy: qiskit_library.RYYGate,
     Rz: qiskit_library.RZGate,
     Rzz: qiskit_library.RZZGate,
-    CCNOT: qiskit_library.CCXGate,
-    CZ: qiskit_library.CZGate,
+    Swap: qiskit_library.SwapGate,
+    X: qiskit_library.XGate,
+    Y: qiskit_library.YGate,
+    Z: qiskit_library.ZGate,
 }
 
 
 class QiskitExporter:
     """
     Tool to convert ParityOS circuits to Qiskit quantum circuits.
 
@@ -87,37 +126,56 @@
         :return: a Qiskit QuantumCircuit object.
         """
         qiskit_circuit = qiskit.QuantumCircuit(len(self.qubit_map))
 
         def _qiskit_circuit_append(element: CircuitElement):
             """Recursive helper method for the to_qiskit method."""
             if isinstance(element, Gate):
-                qiskit_circuit.append(*self.gate_to_qiskit(element))
+                self.append_qiskit_gate(qiskit_circuit, element)
             else:
                 for item in element:
                     _qiskit_circuit_append(item)
 
         _qiskit_circuit_append(circuit)
         return qiskit_circuit
 
-    def gate_to_qiskit(self, gate: Gate) -> tuple[qiskit.circuit.gate.Gate, list[int]]:
+    def append_qiskit_gate(self, qiskit_circuit: qiskit.circuit, gate: Gate):
         """
-        Converts a gate to a (Qiskit instruction, qubit_indices) tuple.
-
-        :param gate: a ParityOS gate instance.
-        :return: a (Qiskit instruction, qubit_indices) tuple.
+        Creates a qiskit gate corresponding to the ParityOS Gate instance and appends it to the
+        qiskit circuit.
+        :param qiskit_circuit: the qiskit circuit to which we want to append the gate
+        :param gate: the ParityOS Gate that is appended to the circuit
         """
         qiskit_class = GATE_MAP[type(gate)]
+        qubits = [qiskit_circuit.qubits[self.qubit_map[qubit]] for qubit in gate.qubit_list]
+
+        if isinstance(gate, MultiControlMixin):
+            qiskit_gate = self._get_qiskit_instruction(gate, qiskit_class)
+            qiskit_instruction = qiskit_library.MCMT(
+                gate=qiskit_gate,
+                num_ctrl_qubits=len(gate.control_qubits),
+                num_target_qubits=len(gate.target_qubits),
+            )
+        else:
+            qiskit_instruction = self._get_qiskit_instruction(gate, qiskit_class)
+
+        qiskit_circuit.append(qiskit_instruction, qargs=qubits)
+
+    def _get_qiskit_instruction(self, gate: Gate, qiskit_class: type) -> qiskit.circuit.gate.Gate:
+        """
+        Instantiates the qiskit instruction for a gate using the associated qiskit class.
+
+        :param gate: A ParityOS gate instance
+        :param qiskit_class: The qiskit gate class corresponding to the gate
+        :return: A qiskit gate instance
+        """
         if isinstance(gate, RMixin):
             angle = (
                 gate.angle
                 if gate.parameter_name is None
                 else gate.angle * self.parameter_map[gate.parameter_name]
             )
             qiskit_instruction = qiskit_class(angle)
         else:
             qiskit_instruction = qiskit_class()
 
-        qubit_indices = [
-            self.qubit_map[qubit] for qubit in gate.make_args() if isinstance(qubit, Qubit)
-        ]
-        return qiskit_instruction, qubit_indices
+        return qiskit_instruction
```

### Comparing `parityos-2.4.0/parityos_addons/qaoa/qaoa_scheduler.py` & `parityos-2.5.0/parityos_addons/qaoa/qaoa_scheduler.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/parityos_addons/spin_hamiltonians.py` & `parityos-2.5.0/parityos_addons/spin_hamiltonians.py`

 * *Files identical despite different names*

### Comparing `parityos-2.4.0/setup.py` & `parityos-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 else:
     job_id = os.environ.get("CI_JOB_ID", 0)
     version = f"0.0rc{job_id}+test"
 
 # Here we specify the dependencies of optional packages in parityos_addons.
 extras_require = {
     "cirq": ["cirq-core"],
-    "qiskit": ["qiskit<1"],
+    "qiskit": ["qiskit"],
     "spinz": ["sympy"],
 }
 # The option [all] will install all optional dependencies.
 extras_require["all"] = list(set(chain(*extras_require.values())))
 
 setup(
     name="parityos",
```

