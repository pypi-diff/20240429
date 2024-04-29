# Comparing `tmp/Nikola-8.3.0.tar.gz` & `tmp/Nikola-8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nikola-8.3.0.tar", last modified: Wed Jan 10 20:48:00 2024, max compression
+gzip compressed data, was "Nikola-8.3.1.tar", last modified: Mon Apr 29 12:05:37 2024, max compression
```

## Comparing `Nikola-8.3.0.tar` & `Nikola-8.3.1.tar`

### file list

```diff
@@ -1,1327 +1,1326 @@
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.971876 Nikola-8.3.0/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7211 2024-01-10 19:41:36.000000 Nikola-8.3.0/AUTHORS.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   119961 2024-01-10 20:47:45.000000 Nikola-8.3.0/CHANGES.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4583 2023-12-02 08:56:57.000000 Nikola-8.3.0/CONTRIBUTING.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1074 2024-01-10 19:43:39.000000 Nikola-8.3.0/LICENSE.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      201 2023-12-02 08:56:57.000000 Nikola-8.3.0/MANIFEST.in
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.691876 Nikola-8.3.0/Nikola.egg-info/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3718 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/PKG-INFO
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    55184 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/SOURCES.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        1 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/dependency_links.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       48 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/entry_points.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      831 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/requires.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        7 2024-01-10 20:48:00.000000 Nikola-8.3.0/Nikola.egg-info/top_level.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3718 2024-01-10 20:48:00.971876 Nikola-8.3.0/PKG-INFO
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2308 2023-12-02 08:56:57.000000 Nikola-8.3.0/README.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.691876 Nikola-8.3.0/docs/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.691876 Nikola-8.3.0/docs/architecture/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   163583 2024-01-10 20:17:15.000000 Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.png
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    63954 2024-01-10 20:17:15.000000 Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.svg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20865 2024-01-10 20:17:15.000000 Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6121 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/creating-a-site.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/creating-a-theme.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/extending.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/internals.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.691876 Nikola-8.3.0/docs/man/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1787 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/man/nikola.1.gz
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3228 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/man/nikola.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   122233 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/manual.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-01-10 20:47:46.000000 Nikola-8.3.0/docs/path_handlers.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/social_buttons.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/docs/sphinx/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6762 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/Makefile
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8534 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/conf.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6121 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/creating-a-site.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/creating-a-theme.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/extending.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      752 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/index.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/internals.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6701 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/make.bat
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   122233 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/manual.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       55 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/modules.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.packages.datecond.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.packages.pygments_better_html.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      259 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.packages.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      171 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.command.auto.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3214 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.command.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      183 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.command.rst2html.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      854 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.markdown.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2118 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.rest.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      987 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      565 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.misc.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      508 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3620 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.task.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      531 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.plugins.template.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1897 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1060 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/nikola_titles_for_sphinx.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-01-10 20:47:46.000000 Nikola-8.3.0/docs/sphinx/path_handlers.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       31 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/requirements-docs.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/social_buttons.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3209 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/support.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36291 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/template-variables.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/sphinx/theming.rst
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)       46 2023-12-02 08:56:57.000000 Nikola-8.3.0/docs/sphinx/update-modules.sh
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3209 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/support.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36291 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/template-variables.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-01-10 20:47:45.000000 Nikola-8.3.0/docs/theming.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1488 2023-12-02 08:56:57.000000 Nikola-8.3.0/dodo.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/logo/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7004 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/favicon.png
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2612 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/favicon.svg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1750 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/nikola-50px-grey.png
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2031 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/nikola-50px-transparent.png
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15268 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/nikola.png
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1734 2023-12-02 08:56:57.000000 Nikola-8.3.0/logo/nikola.svg
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1507 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16687 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/__main__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    54048 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/conf.py.in
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      309 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/README.txt
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/files/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   432254 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/files/favicon.ico
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/files/images/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1750 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/files/images/nikola.png
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/samplesite/galleries/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       14 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/exclude.meta
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      138 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/index.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      204 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/metadata.sample.yml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21032 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla2_lg.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29468 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla4_lg.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9838 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_conducts_lg.webp
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    40380 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_lightning1_lg.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36277 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_lightning2_lg.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17374 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_tower1_lg.jpg
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/images/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    80761 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/images/frontispiece.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   156895 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/images/illus_001.jpg
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/listings/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/listings/hello.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/pages/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      274 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/1.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    45357 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/bootstrap-demo.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2132 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/charts.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/creating-a-theme.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21458 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/dr-nikolas-vendetta.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/extending.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/internals.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      211 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/listings-demo.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   122233 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/manual.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-01-10 20:47:46.000000 Nikola-8.3.0/nikola/data/samplesite/pages/path_handlers.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    57207 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/quickref.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11533 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/pages/quickstart.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/social_buttons.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-01-10 20:47:45.000000 Nikola-8.3.0/nikola/data/samplesite/pages/theming.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/posts/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      884 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/posts/1.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/samplesite/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3373 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/samplesite/templates/book.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/shortcodes/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/shortcodes/jinja/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       10 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/shortcodes/jinja/raw.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/shortcodes/mako/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        7 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/shortcodes/mako/raw.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/symlink-test-link.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/symlink-test-orig.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1655 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/symlinked.txt
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/themes/base/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      177 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/base/assets/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.711876 Nikola-8.3.0/nikola/data/themes/base/assets/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3609 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/baguetteBox.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       29 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/html4css1.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18579 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/ipython.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/nikola_ipython.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2173 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/nikola_rst.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       60 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/rst.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13110 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/rst_base.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7441 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/data/themes/base/assets/css/theme.css
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.711876 Nikola-8.3.0/nikola/data/themes/base/assets/js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9511 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/baguetteBox.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      677 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/fancydates.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      340 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/fancydates.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1399 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/gallery.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      893 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/gallery.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/html5.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/html5shiv-printshiv.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11161 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/justified-layout.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    73302 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/js/luxon.min.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.711876 Nikola-8.3.0/nikola/data/themes/base/assets/xml/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1771 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/xml/atom.xsl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1848 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/assets/xml/rss.xsl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      156 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/base.theme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      345 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/bundles
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/base/messages/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1804 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_af.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2231 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ar.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1905 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_az.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2387 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_bg.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_bn.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_br.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1777 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_bs.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1884 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ca.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1726 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_cs.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1726 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_cz.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1665 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_da.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1916 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_de.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2588 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_el.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1735 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_en.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1839 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_eo.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1949 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_es.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1853 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_et.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1895 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_eu.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2251 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_fa.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1931 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_fi.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1907 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_fr.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1857 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_fur.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1803 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_gl.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2012 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_he.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2579 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_hi.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1760 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_hr.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1858 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_hu.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1889 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ia.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1881 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_id.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1869 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_it.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2012 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ja.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1927 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ko.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_lt.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_mi.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3092 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ml.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2677 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_mr.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1687 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_nb.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1850 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_nl.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1943 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_oc.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2538 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_pa.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1843 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_pl.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2009 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_pt.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1844 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_pt_br.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2333 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ru.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1945 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sk.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1638 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sl.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1833 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sq.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2120 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sr.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1725 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sr_latin.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1702 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_sv.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ta.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2802 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_te.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2581 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_th.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1901 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_tr.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1238 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_tzm.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2353 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_uk.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2158 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_ur.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2116 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_vi.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1817 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_zh_cn.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1733 2024-01-10 20:47:58.000000 Nikola-8.3.0/nikola/data/themes/base/messages/messages_zh_tw.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/base/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      519 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/annotation_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       34 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/archive.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      973 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/archive_navigation_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      665 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/archiveindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      936 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/author.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      602 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/authorindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      727 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/authors.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1293 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      228 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/base_footer.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2192 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/base_header.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5108 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      458 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      343 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_commento.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      888 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_discourse.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1760 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_disqus.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      184 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_dummy.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1747 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_facebook.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      853 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_intensedebate.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      842 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_isso.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      357 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_muut.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      632 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_utterances.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6515 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/feeds_translations_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2966 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/gallery.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3049 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/index.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      722 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/index_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      837 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/list.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      940 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/list_post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      579 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/listing.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2724 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/math_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       30 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/page.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      617 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/pagination_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3002 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/post_header.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3217 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/post_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      499 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/post_list_directive.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      945 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/story.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1198 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/tag.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      822 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/tagindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1518 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/tags.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      423 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base/templates/ui_helper.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.701876 Nikola-8.3.0/nikola/data/themes/base-jinja/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      177 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      164 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/base-jinja.theme
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.711876 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      529 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/annotation_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       31 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/archive.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1064 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/archive_navigation_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      658 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/archiveindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      983 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/author.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      612 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/authorindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      760 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/authors.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1325 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      252 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base_footer.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2382 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base_header.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5412 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      480 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      371 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_commento.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      937 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_discourse.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1830 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_disqus.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      203 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_dummy.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1778 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_facebook.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      896 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_intensedebate.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      935 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_isso.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      385 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_muut.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      701 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_utterances.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6989 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/feeds_translations_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3171 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/gallery.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3204 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/index.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      784 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/index_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/list.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      977 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/list_post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      648 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/listing.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2848 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/math_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       27 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/page.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      665 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/pagination_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1940 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3190 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_header.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3506 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      538 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_list_directive.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      989 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/story.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1275 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tag.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      859 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tagindex.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1620 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tags.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      474 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/base-jinja/templates/ui_helper.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      297 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/bootblog4/assets/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4/assets/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3810 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/assets/css/bootblog.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      329 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/bootblog4.theme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      529 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/bundles
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4034 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7102 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7838 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4/templates/index.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      297 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/assets/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/assets/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3810 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/assets/css/bootblog.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      330 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/bootblog4-jinja.theme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      529 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/bundles
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4153 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7519 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8139 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/index.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootstrap4/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/css/bootstrap.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3741 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/css/theme.css
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/bootstrap.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/jquery.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/popper.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/bootstrap4.theme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      492 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/bundles
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      655 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/authors.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3343 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6917 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      440 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/index_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      668 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/listing.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2318 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/pagination_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1998 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1124 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/tags.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      662 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/ui_helper.tmpl
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.671876 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/css/bootstrap.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3741 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/css/theme.css
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.721876 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/bootstrap.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/jquery.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/popper.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/bootstrap4-jinja.theme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      492 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/bundles
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      693 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/authors.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3488 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/base.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7337 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/base_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      488 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/index_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      748 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/listing.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2455 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/pagination_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2114 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/post.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1227 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/tags.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      724 2024-01-10 20:47:47.000000 Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/ui_helper.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19199 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/filters.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11019 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/hierarchy_utils.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9588 2024-01-10 19:45:41.000000 Nikola-8.3.0/nikola/image_processing.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4438 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/log.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9223 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/metadata_extractors.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   126102 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/nikola.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/packages/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      417 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       39 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/__init__.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/packages/datecond/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1526 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/packages/datecond/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3749 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/packages/datecond/__init__.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/packages/pygments_better_html/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1526 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/packages/pygments_better_html/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1331 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/pygments_better_html/LICENSE.pygments
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9279 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/packages/pygments_better_html/__init__.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/packages/tzlocal/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7048 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/tzlocal/LICENSE.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      253 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/tzlocal/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4515 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/tzlocal/unix.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3074 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/tzlocal/win32.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33455 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/packages/tzlocal/windows_tz.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33838 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugin_categories.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10960 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugin_manager.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/plugins/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       51 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7264 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/basic_import.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/plugins/command/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1169 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/__init__.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/plugins/command/auto/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    23973 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/auto/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38927 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/auto/livereload.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      250 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/auto.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      198 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/check.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22078 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/check.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      225 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/console.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5906 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/console.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/default_config.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1965 2024-01-10 20:42:05.000000 Nikola-8.3.0/nikola/plugins/command/default_config.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      191 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/deploy.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5476 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/deploy.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      224 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/github_deploy.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6428 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/github_deploy.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      256 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/import_wordpress.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    55631 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/import_wordpress.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/init.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21669 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/init.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/new_page.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3759 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/new_page.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      198 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/new_post.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21475 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/new_post.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/orphans.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1819 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/orphans.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      215 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/plugin.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13634 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/plugin.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.731876 Nikola-8.3.0/nikola/plugins/command/rst2html/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2933 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/rst2html/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      139 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/rst2html/rst2html.tmpl
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      241 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/rst2html.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      192 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/serve.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10347 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/serve.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      192 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/status.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7224 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/status.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      246 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/subtheme.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6153 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/subtheme.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/theme.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14493 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/theme.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/command/version.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2320 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/command/version.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/compile/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1170 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/html.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4663 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/html.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      284 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/ipynb.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7302 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/ipynb.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/compile/markdown/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7259 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_gist.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6764 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_gist.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_nikola.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3232 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_nikola.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      280 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_podcast.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3644 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_podcast.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      230 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/markdown.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      236 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/pandoc.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4656 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/pandoc.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/php.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3533 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/php.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/compile/rest/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16468 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      235 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/chart.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6334 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/chart.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      248 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/doc.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4586 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/doc.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/gist.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2407 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/gist.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      238 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/listing.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8327 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/listing.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/media.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2410 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/media.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      268 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/post_list.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4281 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/post_list.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      235 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/soundcloud.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3427 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/soundcloud.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/template.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      275 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/thumbnail.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2854 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/thumbnail.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      149 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/vimeo.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4486 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/vimeo.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      169 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest/youtube.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3384 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/compile/rest/youtube.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/compile/rest.plugin
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/misc/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1178 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/misc/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/misc/scan_posts.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5021 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/misc/scan_posts.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/misc/taxonomies_classifier.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18945 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/misc/taxonomies_classifier.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/shortcode/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/chart.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3156 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/shortcode/chart.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/shortcode/emoji/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1358 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/__init__.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.741876 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8371 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Activity.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19256 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Flags.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4737 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Food.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1158 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10965 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Nature.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12968 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Objects.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    39457 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/People.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21368 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Symbols.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8319 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Travel.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/emoji.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/gist.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1698 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/shortcode/gist.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/listing.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3087 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/shortcode/listing.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/post_list.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9277 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/shortcode/post_list.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      207 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/shortcode/thumbnail.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2677 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/shortcode/thumbnail.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/nikola/plugins/task/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1166 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/archive.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11575 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/archive.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      218 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/authors.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6674 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/authors.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      199 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/task/bundles.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5029 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/bundles.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      229 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/categories.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12004 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/categories.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/copy_assets.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5449 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/copy_assets.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      215 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/copy_files.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2163 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/copy_files.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/galleries.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33845 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/galleries.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/task/gzip.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3048 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/gzip.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      220 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/indexes.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5375 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/indexes.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      216 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/listings.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14943 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/listings.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/page_index.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4462 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/page_index.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      205 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/pages.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3367 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/pages.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/posts.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5190 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/posts.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      199 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/redirect.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2347 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/redirect.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/task/robots.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3601 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/robots.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      225 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/scale_images.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4563 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/scale_images.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      203 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/task/sitemap.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13762 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/sitemap.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      216 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/sources.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3120 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/sources.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/tags.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6851 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/tags.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/nikola/plugins/task/taxonomies.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    25038 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/task/taxonomies.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/nikola/plugins/template/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1185 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/template/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      210 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/template/jinja.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5848 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/template/jinja.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      206 2024-01-10 19:41:36.000000 Nikola-8.3.0/nikola/plugins/template/mako.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5910 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/plugins/template/mako.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    54604 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/post.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14869 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/shortcodes.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2822 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/state.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    79106 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/utils.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4630 2024-01-10 19:44:21.000000 Nikola-8.3.0/nikola/winutils.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      305 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/README-baguetteBox.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/node_modules/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3598 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/.package-lock.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1070 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9197 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4839 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27973 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3609 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9511 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2248 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/src/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27894 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/src/baguetteBox.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3769 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/src/baguetteBox.scss
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.751876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1131 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11743 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.681876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.771876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    67472 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   163856 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    50636 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   115091 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4784 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    78154 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3922 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33156 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   200387 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   515619 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   654593 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.791876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   230599 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   426918 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    83376 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   308871 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   137714 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   271784 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   185257 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.681876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.791876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5503 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/alert.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8011 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/alert.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7827 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/button.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13441 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/button.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20871 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/carousel.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38793 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/carousel.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13394 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/collapse.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    24048 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/collapse.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18530 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/dropdown.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32722 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/dropdown.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      880 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/index.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22815 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/modal.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    41141 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/modal.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7253 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/popover.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9209 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/popover.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11210 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20080 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8813 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tab.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15336 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tab.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7802 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/toast.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12019 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/toast.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27521 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tooltip.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53579 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tooltip.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6631 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/util.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12040 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/util.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.801876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3189 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/alert.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5730 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/button.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15927 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/carousel.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9721 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/collapse.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14056 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/dropdown.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16934 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/modal.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3815 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/popover.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8160 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/scrollspy.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6171 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tab.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4718 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/toast.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.801876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tools/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3420 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tools/sanitizer.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18232 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tooltip.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5071 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/util.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7858 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.811876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1164 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_alert.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1121 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_badge.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1326 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3626 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_button-group.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2685 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_buttons.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5940 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_card.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4843 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_carousel.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      940 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_close.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1012 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_code.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15700 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_custom-forms.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4436 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_dropdown.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9246 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_forms.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5391 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_functions.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1745 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_grid.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1158 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_images.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6521 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_input-group.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      406 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_jumbotron.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3870 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_list-group.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       83 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_media.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1050 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_mixins.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6310 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_modal.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2344 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_nav.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7529 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_navbar.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1823 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_pagination.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4720 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_popover.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2838 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_print.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1171 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_progress.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11539 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_reboot.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      572 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_root.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1287 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_spinners.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3544 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_tables.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1132 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_toasts.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2518 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_tooltip.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      363 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_transitions.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2222 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_type.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      536 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_utilities.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    48615 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_variables.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      598 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      918 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/bootstrap.scss
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.811876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      242 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      695 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_background-variant.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      320 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_badge.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1828 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      532 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4482 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3525 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1422 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       93 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      613 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      392 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_float.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5815 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2050 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2089 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_grid-framework.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2086 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      757 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_hover.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1155 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      433 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      170 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      369 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_nav-divider.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      462 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      481 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      827 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_screen-reader.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      148 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_size.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      794 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_table-row.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      474 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_text-emphasis.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      326 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_text-hide.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      168 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      681 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      189 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_visibility.scss
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.811876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      420 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_align.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_background.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1771 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_borders.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       37 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_clearfix.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      519 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_display.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      853 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_embed.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2769 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_flex.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      376 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_float.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      142 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_interactions.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      133 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_overflow.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      484 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_position.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      115 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_screenreaders.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_shadows.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      498 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_sizing.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2108 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_spacing.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      431 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_stretched-link.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2106 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_text.scss
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_visibility.scss
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.811876 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/vendor/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7067 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/vendor/_rfs.scss
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       11 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/.gitattributes
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       22 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/.npmignore
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1177 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/Gruntfile.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19536 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/MIT and GPL2 licenses.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      193 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/bower.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      438 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/composer.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16272 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10318 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2734 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      352 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/package.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8391 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/readme.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/src/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16272 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/src/html5shiv-printshiv.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10318 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/src/html5shiv.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      429 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/body-crash.jpg
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2247 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/iframed-tests.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      165 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/inline-mixed-media.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      130 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/inline-print-media.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      136 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/no-print.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5841 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/paramtracer.swf
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      129 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/print-styles.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       43 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/print.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      149 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/screen.css
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/highcharts/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2547 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/highcharts/area-basic.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    86203 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/highcharts/highcharts.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1913 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/html5shiv.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      299 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/iframe.1-1.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      323 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/iframe.1-2.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      619 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/iframe.1.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1010 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/index.html
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.821876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.831876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      298 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/dashboard.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/iframe.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       78 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/test.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3386 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testinit.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      770 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testrunner.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2720 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testsuite.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      295 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/versioncheck.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11126 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/index.html
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.831876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    44525 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/core.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    64131 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/manipulation.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    35493 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/traversing.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2389 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/mixed-test.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2351 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/object-test.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1668 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/perf.1.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      726 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/perf.2.html
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.831876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/qunit/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4517 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/qunit/qunit.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    41024 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/qunit/qunit.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      374 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/style.all.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       57 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/style.css
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       54 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/style.print.css
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.831876 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/unit/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9259 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/unit/tests.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.831876 Nikola-8.3.0/npm_assets/node_modules/jquery/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13035 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/AUTHORS.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1117 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/LICENSE.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2001 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/bower.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.841876 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   292458 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   138351 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.min.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   239159 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    72666 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   110701 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.min.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.681876 Nikola-8.3.0/npm_assets/node_modules/jquery/external/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.841876 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1641 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/LICENSE.txt
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.841876 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    72087 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20366 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    31265 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3260 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.841876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.841876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2753 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/jsonp.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1904 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/load.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1637 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/script.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       67 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/var/location.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       72 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/var/nonce.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       60 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/var/rquery.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4355 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/xhr.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22924 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3272 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/attr.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4527 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/classes.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2857 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/prop.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      786 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/support.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4261 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/val.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5552 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/callbacks.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1160 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/DOMEval.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1314 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/access.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      550 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/camelCase.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3345 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/init.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      789 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/isAttached.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      176 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/nodeName.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1604 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/parseHTML.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      739 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/parseXML.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2268 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/ready-no-deferred.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2101 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/ready.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      168 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/readyException.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      362 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/stripAndCollapse.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      631 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/support.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      379 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/toType.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      244 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/var/rsingleTag.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9183 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/core.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      530 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/addGetHookIf.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2002 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/adjustCSS.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3305 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/curCSS.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      870 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/finalPropName.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      317 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/hiddenVisibleSelectors.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2304 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/showHide.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4829 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/support.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       88 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/cssExpand.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/getStyles.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1284 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/isHiddenWithinTree.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      123 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/rboxStyle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       57 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/rcustomProp.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      131 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/rnumnonpx.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      501 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/swap.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14195 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/css.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3956 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/Data.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      318 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/var/acceptData.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       84 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/var/dataPriv.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       84 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/var/dataUser.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4325 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/data.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deferred/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      640 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deferred/exceptionHook.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11007 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deferred.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      296 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated/ajax-event-alias.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1140 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated/event.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2406 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1756 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/dimensions.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3291 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects/Tween.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      244 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects/animatedSelector.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17417 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1665 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/focusin.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      133 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/support.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5438 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/trigger.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    24505 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/event.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/exports/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1024 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/exports/amd.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      628 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/exports/global.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      646 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/jquery.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      690 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/_evalUrl.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2490 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/buildFragment.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      654 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/getAll.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      381 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/setGlobalEval.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1244 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/support.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       92 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/var/rscriptType.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      304 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/var/rtagName.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      823 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/wrapMap.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12674 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6828 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/offset.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/queue/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      534 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/queue/delay.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3091 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/queue.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6406 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/selector-native.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      411 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/selector-sizzle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       66 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/selector.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3236 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/serialize.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2352 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/findFilter.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.851876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      371 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/var/dir.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      128 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/var/rneedsContext.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      218 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/var/siblings.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4692 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      110 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/ObjectFunctionString.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       54 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/arr.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       82 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/class2type.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       67 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/document.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      105 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/documentElement.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      372 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/flat.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       92 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/fnToString.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       73 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/getProto.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      110 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/hasOwn.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       82 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/indexOf.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      674 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/isFunction.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      126 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/isWindow.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      100 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/pnum.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       79 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/push.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       79 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/rcheckableType.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      136 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/rcssNum.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/rnothtmlwhite.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/rtrimCSS.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       80 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/slice.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/support.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      104 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/toString.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      125 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/whitespace.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1477 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/jquery/src/wrap.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/justified-layout/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1075 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1679 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1770 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/demo.html
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/justified-layout/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    23065 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/dist/justified-layout.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11161 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/dist/justified-layout.min.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/justified-layout/lib/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8115 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/lib/index.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11381 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/lib/row.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2173 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/justified-layout/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/livereload-js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1064 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10651 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/livereload-js/dist/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38927 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/dist/livereload.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        0 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/.keepme
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5268 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/connector.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1206 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/customevents.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1704 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/less.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7532 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/livereload.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1636 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/options.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3231 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/protocol.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15736 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/reloader.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      765 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/startup.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/timer.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1674 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/livereload-js/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/luxon/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1076 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/LICENSE.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2051 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.861876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.871876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/amd/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   277835 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/amd/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479476 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/amd/luxon.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.871876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/cjs-browser/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   262915 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479472 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.881876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/es6/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   226157 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/es6/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   428684 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/es6/luxon.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.891876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   277851 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479479 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    73302 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   122652 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.min.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.891876 Nikola-8.3.0/npm_assets/node_modules/luxon/build/node/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   226256 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/node/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   444782 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/node/luxon.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       98 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/build/readme.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2801 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.901876 Nikola-8.3.0/npm_assets/node_modules/luxon/src/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    83972 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/datetime.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    30961 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/duration.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1047 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/errors.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.901876 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4633 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/conversions.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2000 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/diff.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1917 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/digits.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5820 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/english.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2249 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/formats.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12478 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/formatter.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      282 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/invalid.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14423 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/locale.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10509 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/regexParser.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11447 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/tokenParser.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6933 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/util.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1246 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/zoneUtil.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7581 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/info.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21571 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/interval.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      586 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/luxon.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       45 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/package.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4397 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/settings.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2132 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zone.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.901876 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4565 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/IANAZone.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2175 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/fixedOffsetZone.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      763 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/invalidZone.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1147 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/systemZone.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.901876 Nikola-8.3.0/npm_assets/node_modules/merge/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1092 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/LICENSE
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1155 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      525 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/bower.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2914 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/merge.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1011 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/merge.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1477 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/merge/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.911876 Nikola-8.3.0/npm_assets/node_modules/popper.js/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11127 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.911876 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.921876 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    35566 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61746 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10654 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53959 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    88482 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140737 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21204 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   125307 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33894 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61481 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10201 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53753 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    84861 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140064 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19903 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   125107 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.min.js.map
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.921876 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36668 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61788 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10813 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53756 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    88736 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3114 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js.flow
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140747 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.min.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   123754 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.min.js.map
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4744 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/index.d.ts
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3114 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/index.js.flow
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2606 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/package.json
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.931876 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5393 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/index.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.931876 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1942 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/defaults.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      989 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/destroy.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      511 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/disableEventListeners.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      444 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/enableEventListeners.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1109 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/placements.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2046 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/update.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.931876 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2752 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/applyStyle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3262 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/arrow.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4016 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/computeStyle.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5094 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/flip.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1207 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/hide.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14372 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/index.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      922 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/inner.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      895 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/keepTogether.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5943 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/offset.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2849 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/preventOverflow.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      999 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/shift.js
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.941876 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      773 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/clockwise.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1714 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/computeAutoPlacement.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1121 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/debounce.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      397 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/find.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1681 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/findCommonOffsetParent.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      534 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/findIndex.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      564 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBordersSize.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3000 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBoundaries.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2028 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBoundingClientRect.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      363 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getClientRect.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      756 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getFixedPositionOffsetParent.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1271 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetParent.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      801 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetRect.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2315 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetRectRelativeToArbitraryNode.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      382 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOppositePlacement.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      382 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOppositeVariation.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      652 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOuterSizes.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      315 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getParentNode.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1696 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getPopperOffsets.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      401 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getReferenceNode.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1017 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getReferenceOffsets.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      309 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getRoot.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1754 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getRoundedOffsets.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      668 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getScroll.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      910 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getScrollParent.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      455 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getStyleComputedProperty.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      676 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getSupportedPropertyName.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      898 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getViewportOffsetRectRelativeToArtbitraryNode.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      261 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getWindow.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      785 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getWindowSizes.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      825 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/includeScroll.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2910 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/index.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isBrowser.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      700 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isFixed.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      377 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isFunction.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      511 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isIE.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      285 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isModifierEnabled.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1095 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isModifierRequired.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      233 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isNumeric.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      286 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isOffsetContainer.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      653 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/removeEventListeners.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1323 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/runModifiers.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      559 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setAttributes.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      695 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setStyles.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1218 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setupEventListeners.js
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4081 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/package-lock.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      469 2023-12-02 08:56:57.000000 Nikola-8.3.0/npm_assets/package.json
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      251 2023-12-02 08:56:57.000000 Nikola-8.3.0/requirements-extras.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      126 2023-12-02 08:56:57.000000 Nikola-8.3.0/requirements-tests.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      243 2024-01-10 19:41:36.000000 Nikola-8.3.0/requirements.txt
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.941876 Nikola-8.3.0/scripts/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        0 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/INTERNAL USE ONLY
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1289 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/baseline.sh
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     2868 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/capty
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.941876 Nikola-8.3.0/scripts/debug_rebuilds/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      868 2024-01-10 19:44:21.000000 Nikola-8.3.0/scripts/debug_rebuilds/README.md
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1259 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/debug_rebuilds/step1_build_and_dumpdb.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1564 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/debug_rebuilds/step2_analyze_py_files.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      883 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/document_path_handlers.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      408 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/generate_symlinked_list.sh
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      543 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/getpyver.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      880 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/github-release.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1229 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/import_po.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)    10154 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/jinjify.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      607 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/langmatrix.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      666 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/langstatus.py
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     5097 2024-01-10 19:44:21.000000 Nikola-8.3.0/scripts/release
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.941876 Nikola-8.3.0/scripts/snapcraft/
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      457 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/snapcraft/nikola.sh
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      638 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/theme_snapshot
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1970 2023-12-02 08:56:57.000000 Nikola-8.3.0/scripts/update-npm-assets.sh
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      238 2024-01-10 20:48:00.971876 Nikola-8.3.0/setup.cfg
--rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     5506 2024-01-10 20:47:45.000000 Nikola-8.3.0/setup.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       24 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      456 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/conftest.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      872 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/1-nolinks.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/dev_server_sample_output_folder/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      214 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/dev_server_sample_output_folder/index.html
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/metadata_extractors/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-html-1-compiler.html
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      568 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-ipynb-1-compiler.ipynb
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      160 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-markdown-1-compiler.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      230 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-markdown-1-nikola.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-markdown-2-nikola.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-markdown-2-nikola.meta
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      166 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-1-compiler.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-1-nikola.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      155 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-1-toml.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      160 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-1-yaml.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-nikola.meta
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-nikola.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      123 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-toml.meta
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-toml.rst
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      128 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-yaml.meta
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/metadata_extractors/f-rest-2-yaml.rst
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/plugin_manager/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/broken.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1578 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/broken.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/first.plugin
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1614 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/one.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/plugin_manager/second/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/second/second.plugin
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/plugin_manager/second/two/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1459 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/data/plugin_manager/second/two/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27095 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/rss-2_0.xsd
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/test_config/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      635 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/test_config/conf.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       88 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/test_config/config.with+illegal(module)name.characters.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       85 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/test_config/prod.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/translated_titles/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1949 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/translated_titles/conf.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.951876 Nikola-8.3.0/tests/data/translated_titles/pages/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       30 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/translated_titles/pages/1.pl.txt
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       59 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/translated_titles/pages/1.txt
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.961876 Nikola-8.3.0/tests/data/wordpress_import/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19897 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/wordpress_import/wordpress_export_example.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1955 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/wordpress_import/wordpress_qtranslate_item_modernized.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1995 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/wordpress_import/wordpress_qtranslate_item_raw_export.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6184 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/data/wordpress_import/wordpress_unicode_export.xml
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3342 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/helper.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.961876 Nikola-8.3.0/tests/integration/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      419 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/__init__.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1598 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/conftest.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1772 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/helper.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1142 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_archive_full.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      868 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_archive_per_day.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      883 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_archive_per_month.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      648 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_building_in_subdir.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2586 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_category_destpath.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1264 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_check_absolute_subfolder.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1196 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_check_failure.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      893 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_check_full_path_subfolder.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5992 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_demo_build.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9010 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/integration/test_dev_server.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1410 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_empty_build.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3040 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_future_post.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6419 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_page_index_normal_urls.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1387 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_page_index_pretty_urls.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3287 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_redirection.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1604 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/integration/test_relative_links.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1810 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/integration/test_relative_links_with_pages_in_root.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      764 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_repeated_posts_setting.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1833 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_translated_content.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1102 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_translated_content_secondary_language.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1545 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_translation_patterns.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1451 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/integration/test_wordpress_import.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17184 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_command_import_wordpress.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5515 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_command_import_wordpress_translation.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3351 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_command_init.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2273 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_compile_markdown.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1983 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_config.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6986 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_locale.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7224 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_metadata_extractors.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3855 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_path_handlers.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5847 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/test_plugin_manager.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      429 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_plugins.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5526 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_rss_feeds.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6484 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_rst_compiler.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4622 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_scheduling.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7030 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_shortcodes.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2219 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_slugify.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3401 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_task_scale_images.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2219 2024-01-10 19:41:36.000000 Nikola-8.3.0/tests/test_template_shortcodes.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      575 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_test_helper.py
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17309 2023-12-02 08:56:57.000000 Nikola-8.3.0/tests/test_utils.py
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.961876 Nikola-8.3.0/translations/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/README.md
-drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-01-10 20:48:00.971876 Nikola-8.3.0/translations/nikola.messages/
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/README.md
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3155 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/af.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3900 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ar.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3290 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/az.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3798 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/bg.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2495 2024-01-10 20:46:35.000000 Nikola-8.3.0/translations/nikola.messages/bn.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2785 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/br.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3185 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/bs.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3492 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ca.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3325 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/cs.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3069 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/da.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3733 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/de.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4168 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/el.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3132 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/en.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3339 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/eo.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3622 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/es.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3329 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/et.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3360 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/eu.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3827 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/fa.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3445 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/fi.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3749 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/fr.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3167 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/fur.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3139 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/gl.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3464 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/he.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3984 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/hi.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3251 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/hr.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3304 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/hu.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3266 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ia.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3315 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/id.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3533 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/it.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3709 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ja.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3393 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ko.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3303 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/lt.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3208 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/mi.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4427 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ml.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3996 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/mr.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3070 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/nb.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3264 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/nl.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3263 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/oc.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4017 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/pa.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3447 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/pl.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3491 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/pt.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3788 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/pt_BR.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4154 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ru.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3574 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sk.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3090 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sl.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3165 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sq.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3626 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sr.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3155 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sr@latin.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3094 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/sv.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2493 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ta.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4214 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/te.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4109 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/th.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3463 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/tr.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2664 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/tzm.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4075 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/uk.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3687 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/ur.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3462 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/vi.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3488 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/zh_CN.po
--rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3156 2023-12-02 08:56:57.000000 Nikola-8.3.0/translations/nikola.messages/zh_TW.po
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.071660 Nikola-8.3.1/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7211 2024-01-10 19:41:36.000000 Nikola-8.3.1/AUTHORS.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   120865 2024-04-29 12:03:29.000000 Nikola-8.3.1/CHANGES.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4859 2024-04-29 11:27:23.000000 Nikola-8.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1074 2024-01-10 19:43:39.000000 Nikola-8.3.1/LICENSE.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      201 2023-12-02 08:56:57.000000 Nikola-8.3.1/MANIFEST.in
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.831660 Nikola-8.3.1/Nikola.egg-info/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3512 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/PKG-INFO
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    55103 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/SOURCES.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        1 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/dependency_links.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       48 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/entry_points.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      846 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/requires.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        7 2024-04-29 12:05:36.000000 Nikola-8.3.1/Nikola.egg-info/top_level.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3512 2024-04-29 12:05:37.071660 Nikola-8.3.1/PKG-INFO
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2152 2024-04-29 11:27:23.000000 Nikola-8.3.1/README.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.831660 Nikola-8.3.1/docs/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.831660 Nikola-8.3.1/docs/architecture/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   163583 2024-01-10 20:17:15.000000 Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.png
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    63954 2024-01-10 20:17:15.000000 Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.svg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20865 2024-01-10 20:17:15.000000 Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6121 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/creating-a-site.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/creating-a-theme.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/extending.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/internals.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.831660 Nikola-8.3.1/docs/man/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1787 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/man/nikola.1.gz
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3228 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/man/nikola.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   121711 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/manual.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-04-29 12:03:30.000000 Nikola-8.3.1/docs/path_handlers.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5188 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/python-version-support-policy.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/social_buttons.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/docs/sphinx/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6762 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/Makefile
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8534 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/conf.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6121 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/creating-a-site.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/creating-a-theme.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/extending.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      752 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/index.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/internals.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6701 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/make.bat
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   121711 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/manual.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       55 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/modules.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.packages.datecond.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.packages.pygments_better_html.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      259 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.packages.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      171 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.command.auto.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3214 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.command.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      183 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.command.rst2html.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      854 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.markdown.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2118 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.rest.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      987 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      565 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.misc.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      508 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3620 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.task.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      531 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.plugins.template.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1897 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1060 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/nikola_titles_for_sphinx.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-04-29 12:03:30.000000 Nikola-8.3.1/docs/sphinx/path_handlers.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       31 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/requirements-docs.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/social_buttons.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3209 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/support.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36291 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/template-variables.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/sphinx/theming.rst
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)       46 2023-12-02 08:56:57.000000 Nikola-8.3.1/docs/sphinx/update-modules.sh
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3209 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/support.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36291 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/template-variables.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-04-29 12:03:29.000000 Nikola-8.3.1/docs/theming.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1488 2023-12-02 08:56:57.000000 Nikola-8.3.1/dodo.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/logo/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7004 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/favicon.png
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2612 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/favicon.svg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1750 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/nikola-50px-grey.png
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2031 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/nikola-50px-transparent.png
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15268 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/nikola.png
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1734 2023-12-02 08:56:57.000000 Nikola-8.3.1/logo/nikola.svg
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1507 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16687 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/__main__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    54048 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/conf.py.in
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/samplesite/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      309 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/README.txt
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/samplesite/files/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   432254 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/files/favicon.ico
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/samplesite/files/images/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1750 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/files/images/nikola.png
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/samplesite/galleries/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       14 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/exclude.meta
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      138 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/index.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      204 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/metadata.sample.yml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21032 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla2_lg.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29468 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla4_lg.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9838 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_conducts_lg.webp
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    40380 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_lightning1_lg.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36277 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_lightning2_lg.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17374 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_tower1_lg.jpg
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.841660 Nikola-8.3.1/nikola/data/samplesite/images/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    80761 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/images/frontispiece.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   156895 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/images/illus_001.jpg
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/samplesite/listings/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/listings/hello.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/samplesite/pages/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      274 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/1.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    45357 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/bootstrap-demo.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2132 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/charts.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32264 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/creating-a-theme.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21458 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/dr-nikolas-vendetta.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    29072 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/extending.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6191 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/internals.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      211 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/listings-demo.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   121711 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/manual.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4878 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/samplesite/pages/path_handlers.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    57207 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/quickref.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11533 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/pages/quickstart.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7848 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/social_buttons.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19202 2024-04-29 12:03:29.000000 Nikola-8.3.1/nikola/data/samplesite/pages/theming.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/samplesite/posts/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      884 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/posts/1.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/samplesite/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3373 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/samplesite/templates/book.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/shortcodes/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/shortcodes/jinja/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       10 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/shortcodes/jinja/raw.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/shortcodes/mako/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        7 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/shortcodes/mako/raw.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/symlink-test-link.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/symlink-test-orig.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1655 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/symlinked.txt
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/themes/base/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      177 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/base/assets/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/themes/base/assets/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3609 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/baguetteBox.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       29 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/html4css1.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18579 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/ipython.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/nikola_ipython.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2173 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/nikola_rst.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       60 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/rst.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13110 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/rst_base.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7441 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/data/themes/base/assets/css/theme.css
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/base/assets/js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9511 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/baguetteBox.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      677 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/fancydates.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      340 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/fancydates.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1399 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/gallery.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      893 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/gallery.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/html5.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11161 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/justified-layout.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    73302 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/js/luxon.min.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/base/assets/xml/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1771 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/xml/atom.xsl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1848 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/assets/xml/rss.xsl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      156 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/base.theme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      345 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/bundles
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/base/messages/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1804 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_af.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2231 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ar.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1905 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_az.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2387 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_bg.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_bn.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_br.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1777 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_bs.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1884 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ca.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1726 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_cs.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1726 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_cz.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1665 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_da.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1916 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_de.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2588 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_el.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1735 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_en.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1839 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_eo.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1949 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_es.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1853 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_et.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1895 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_eu.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2251 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_fa.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1931 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_fi.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1907 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_fr.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1857 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_fur.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1803 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_gl.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2012 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_he.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2579 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_hi.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1760 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_hr.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1858 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_hu.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1889 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ia.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1881 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_id.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1869 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_it.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2012 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ja.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1927 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ko.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_lt.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_mi.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3092 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ml.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2677 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_mr.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1687 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_nb.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1850 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_nl.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1943 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_oc.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2538 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_pa.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1843 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_pl.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2009 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_pt.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1844 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_pt_br.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2333 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ru.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1945 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sk.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1638 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sl.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1833 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sq.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2120 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sr.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1725 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sr_latin.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1702 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_sv.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1189 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ta.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2802 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_te.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2581 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_th.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1901 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_tr.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1238 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_tzm.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2353 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_uk.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2158 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_ur.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2116 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_vi.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1817 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_zh_cn.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1733 2024-04-29 12:04:48.000000 Nikola-8.3.1/nikola/data/themes/base/messages/messages_zh_tw.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/base/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       34 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/archive.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      973 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/archive_navigation_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      665 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/archiveindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      936 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/author.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      602 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/authorindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      727 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/authors.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1293 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      228 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/base_footer.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2192 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/base_header.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4921 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/data/themes/base/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      458 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      343 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_commento.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      888 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_discourse.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1760 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_disqus.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      184 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_dummy.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1747 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_facebook.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      853 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_intensedebate.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      842 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_isso.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      357 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_muut.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      632 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_utterances.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6515 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/feeds_translations_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2966 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/gallery.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3049 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/index.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      722 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/index_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      837 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/list.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      940 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/list_post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      579 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/listing.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2724 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/math_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       30 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/page.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      617 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/pagination_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1838 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3002 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/post_header.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3217 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/post_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      499 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/post_list_directive.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      945 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/story.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1198 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/tag.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      822 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/tagindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1518 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/tags.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      423 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base/templates/ui_helper.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/themes/base-jinja/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      177 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      164 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/base-jinja.theme
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.851660 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       31 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/archive.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1064 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/archive_navigation_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      658 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/archiveindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      983 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/author.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      612 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/authorindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      760 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/authors.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1325 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      252 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base_footer.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2382 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base_header.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5215 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      480 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      371 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_commento.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      937 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_discourse.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1830 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_disqus.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      203 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_dummy.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1778 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_facebook.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      896 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_intensedebate.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      935 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_isso.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      385 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_muut.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      701 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_utterances.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6989 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/feeds_translations_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3171 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/gallery.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3204 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/index.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      784 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/index_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/list.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      977 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/list_post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      648 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/listing.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2848 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/math_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       27 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/page.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      665 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/pagination_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1940 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3190 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_header.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3506 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      538 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_list_directive.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      989 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/story.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1275 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tag.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      859 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tagindex.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1620 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tags.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      474 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/base-jinja/templates/ui_helper.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/bootblog4/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      297 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/bootblog4/assets/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootblog4/assets/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3810 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/assets/css/bootblog.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      329 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/bootblog4.theme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      529 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/bundles
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootblog4/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3965 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6917 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7838 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4/templates/index.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      297 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/assets/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.861660 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/assets/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3810 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/assets/css/bootblog.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      330 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/bootblog4-jinja.theme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      529 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/bundles
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4093 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7322 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8139 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/index.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/css/bootstrap.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3741 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/css/theme.css
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/bootstrap.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/jquery.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/popper.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/bootstrap4.theme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      492 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/bundles
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      655 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/authors.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3274 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6732 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      440 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/index_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      668 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/listing.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2318 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/pagination_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1998 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1124 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/tags.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      662 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/ui_helper.tmpl
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/css/bootstrap.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3741 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/css/theme.css
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/bootstrap.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/jquery.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/popper.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/bootstrap4-jinja.theme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      492 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/bundles
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      693 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/authors.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3428 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/base.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7140 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/base_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      488 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/index_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      748 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/listing.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2455 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/pagination_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2114 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/post.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1227 2024-04-29 12:03:30.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/tags.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      724 2024-04-29 12:03:31.000000 Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/ui_helper.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19199 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/filters.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11019 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/hierarchy_utils.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9588 2024-01-10 19:45:41.000000 Nikola-8.3.1/nikola/image_processing.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4438 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/log.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9223 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/metadata_extractors.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   126133 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/nikola.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/packages/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      417 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       39 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/__init__.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/packages/datecond/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1526 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/packages/datecond/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3749 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/packages/datecond/__init__.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/packages/pygments_better_html/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1526 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/packages/pygments_better_html/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1331 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/pygments_better_html/LICENSE.pygments
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9279 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/packages/pygments_better_html/__init__.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/packages/tzlocal/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7048 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/tzlocal/LICENSE.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      253 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/tzlocal/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4515 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/tzlocal/unix.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3074 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/tzlocal/win32.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33455 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/packages/tzlocal/windows_tz.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33871 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugin_categories.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11762 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugin_manager.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.871660 Nikola-8.3.1/nikola/plugins/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       51 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7227 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/basic_import.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/command/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1169 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/__init__.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/command/auto/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    24231 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/auto/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38927 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/auto/livereload.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      250 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/auto.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      198 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/check.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22078 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/check.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      225 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/console.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5906 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/console.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/default_config.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1930 2024-01-10 20:59:42.000000 Nikola-8.3.1/nikola/plugins/command/default_config.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      191 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/deploy.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5476 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/deploy.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      224 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/github_deploy.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6428 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/github_deploy.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      256 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/import_wordpress.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    56000 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/import_wordpress.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/init.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21648 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/init.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/new_page.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3759 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/new_page.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      198 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/new_post.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21344 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/new_post.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/orphans.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1819 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/orphans.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      215 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/plugin.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12560 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/plugin.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/command/rst2html/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2935 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/rst2html/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      139 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/rst2html/rst2html.tmpl
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      241 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/rst2html.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      192 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/serve.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10347 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/serve.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      192 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/status.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7224 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/status.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      246 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/subtheme.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6153 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/subtheme.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/theme.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14456 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/plugins/command/theme.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/command/version.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2320 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/command/version.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/compile/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1170 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/html.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4663 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/html.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      284 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/ipynb.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7302 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/ipynb.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/compile/markdown/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7259 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_gist.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6764 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_gist.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_nikola.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3232 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_nikola.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      280 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_podcast.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3644 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_podcast.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      230 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/markdown.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      236 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/pandoc.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4656 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/pandoc.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/php.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3533 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/php.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/compile/rest/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16468 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      235 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/chart.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6334 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/chart.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      248 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/doc.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4586 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/doc.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/gist.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2407 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/gist.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      238 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/listing.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8327 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/listing.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/media.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2410 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/media.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      268 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/post_list.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4281 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/post_list.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      235 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/soundcloud.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3427 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/soundcloud.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      114 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/template.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      275 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/thumbnail.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2854 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/thumbnail.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      149 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/vimeo.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4486 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/vimeo.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      169 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest/youtube.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3384 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/compile/rest/youtube.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/compile/rest.plugin
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/misc/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1178 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/misc/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/misc/scan_posts.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5021 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/misc/scan_posts.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/misc/taxonomies_classifier.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18945 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/misc/taxonomies_classifier.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/shortcode/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/chart.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3156 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/shortcode/chart.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/shortcode/emoji/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1358 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/__init__.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.881660 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8371 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Activity.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19256 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Flags.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4737 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Food.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1158 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10965 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Nature.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12968 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Objects.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    39457 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/People.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21368 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Symbols.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8319 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Travel.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/emoji.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/gist.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1698 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/shortcode/gist.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/listing.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3087 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/shortcode/listing.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      245 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/post_list.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9277 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/shortcode/post_list.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      207 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/shortcode/thumbnail.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2677 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/shortcode/thumbnail.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/nikola/plugins/task/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1166 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/archive.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11575 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/archive.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      218 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/authors.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6674 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/authors.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      199 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/task/bundles.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5029 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/bundles.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      229 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/categories.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12004 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/categories.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/copy_assets.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5449 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/copy_assets.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      215 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/copy_files.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2163 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/copy_files.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      223 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/galleries.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33845 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/galleries.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/task/gzip.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3048 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/gzip.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      220 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/indexes.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5375 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/indexes.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      216 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/listings.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14943 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/listings.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      226 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/page_index.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4462 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/page_index.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      205 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/pages.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3367 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/pages.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      213 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/posts.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5190 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/posts.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      199 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/redirect.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2347 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/redirect.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/task/robots.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3601 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/robots.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      225 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/scale_images.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4563 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/scale_images.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      203 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/task/sitemap.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13762 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/sitemap.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      216 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/sources.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3120 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/sources.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      212 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/tags.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6851 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/tags.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/nikola/plugins/task/taxonomies.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    25038 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/task/taxonomies.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/nikola/plugins/template/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1185 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/template/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      210 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/template/jinja.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5848 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/template/jinja.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      206 2024-01-10 19:41:36.000000 Nikola-8.3.1/nikola/plugins/template/mako.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5910 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/plugins/template/mako.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    54604 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/post.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14869 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/shortcodes.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2822 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/state.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    79540 2024-04-29 11:27:23.000000 Nikola-8.3.1/nikola/utils.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4630 2024-01-10 19:44:21.000000 Nikola-8.3.1/nikola/winutils.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      305 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/README-baguetteBox.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/node_modules/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3598 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/.package-lock.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1070 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9197 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4839 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27973 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3609 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9511 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2248 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/src/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27894 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/src/baguetteBox.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3769 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/src/baguetteBox.scss
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.891660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1131 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11743 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.901660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    67472 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   163856 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    50636 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   115091 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4784 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    78154 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3922 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33156 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   200387 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   515619 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   162264 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   654593 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.911660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   230599 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   426918 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    83376 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   308871 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   137714 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   271784 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    62563 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   185257 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.911660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5503 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/alert.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8011 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/alert.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7827 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/button.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13441 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/button.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20871 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/carousel.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38793 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/carousel.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13394 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/collapse.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    24048 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/collapse.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18530 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    32722 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/dropdown.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      880 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/index.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22815 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/modal.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    41141 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/modal.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7253 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/popover.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9209 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/popover.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11210 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20080 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8813 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tab.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15336 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tab.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7802 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/toast.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12019 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/toast.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27521 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tooltip.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53579 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tooltip.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6631 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/util.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12040 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/util.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.911660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3189 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/alert.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5730 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/button.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15927 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/carousel.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9721 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/collapse.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14056 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/dropdown.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16934 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/modal.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3815 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/popover.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8160 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6171 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tab.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4718 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/toast.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.911660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tools/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3420 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tools/sanitizer.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    18232 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tooltip.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5071 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/util.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7858 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.941660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1164 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_alert.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1121 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_badge.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1326 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3626 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_button-group.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2685 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_buttons.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5940 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_card.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4843 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_carousel.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      940 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_close.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1012 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_code.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15700 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_custom-forms.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4436 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9246 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_forms.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5391 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_functions.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1745 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_grid.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1158 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_images.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6521 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_input-group.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      406 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_jumbotron.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3870 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_list-group.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       83 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_media.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1050 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_mixins.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6310 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_modal.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2344 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_nav.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7529 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_navbar.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1823 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_pagination.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4720 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_popover.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2838 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_print.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1171 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_progress.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11539 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_reboot.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      572 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_root.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1287 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_spinners.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3544 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_tables.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1132 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_toasts.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2518 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      363 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_transitions.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2222 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_type.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      536 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_utilities.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    48615 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_variables.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      598 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      918 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/bootstrap.scss
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      242 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      695 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_background-variant.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      320 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_badge.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1828 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      532 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4482 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3525 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1422 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       93 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      613 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_deprecate.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      392 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_float.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5815 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2050 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2089 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_grid-framework.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2086 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      757 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_hover.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1155 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      433 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      170 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      369 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_nav-divider.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      462 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      481 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      827 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_screen-reader.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      148 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_size.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      794 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_table-row.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      474 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_text-emphasis.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      326 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_text-hide.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      168 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      681 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      189 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_visibility.scss
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      420 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_align.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_background.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1771 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_borders.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       37 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_clearfix.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      519 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_display.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      853 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_embed.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2769 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_flex.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      376 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_float.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      142 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_interactions.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      133 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_overflow.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      484 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_position.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      115 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_screenreaders.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      249 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_shadows.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      498 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_sizing.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2108 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_spacing.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      431 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_stretched-link.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2106 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_text.scss
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_visibility.scss
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/vendor/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7067 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/vendor/_rfs.scss
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       11 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/.gitattributes
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       22 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/.npmignore
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1177 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/Gruntfile.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19536 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/MIT and GPL2 licenses.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      193 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/bower.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      438 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/composer.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16272 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4370 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10318 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2734 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      352 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/package.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8391 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/readme.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.951660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/src/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    16272 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/src/html5shiv-printshiv.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10318 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/src/html5shiv.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      429 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/body-crash.jpg
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2247 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/iframed-tests.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      165 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/inline-mixed-media.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      130 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/inline-print-media.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      136 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/no-print.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5841 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/paramtracer.swf
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      129 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/print-styles.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       43 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/print.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      149 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/screen.css
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/highcharts/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2547 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/highcharts/area-basic.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    86203 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/highcharts/highcharts.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1913 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/html5shiv.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      299 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/iframe.1-1.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      323 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/iframe.1-2.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      619 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/iframe.1.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1010 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/index.html
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      298 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/dashboard.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/iframe.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       78 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/test.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3386 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testinit.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      770 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testrunner.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2720 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testsuite.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      295 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/versioncheck.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11126 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/index.html
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    44525 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/core.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    64131 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/manipulation.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    35493 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/traversing.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2389 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/mixed-test.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2351 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/object-test.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1668 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/perf.1.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      726 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/perf.2.html
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/qunit/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4517 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/qunit/qunit.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    41024 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/qunit/qunit.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      374 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/style.all.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       57 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/style.css
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       54 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/style.print.css
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/unit/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9259 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/unit/tests.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.961660 Nikola-8.3.1/npm_assets/node_modules/jquery/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    13035 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/AUTHORS.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1117 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/LICENSE.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2001 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/bower.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.971660 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   292458 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    89795 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   138351 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.min.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   239159 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    72666 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   110701 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.min.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.821660 Nikola-8.3.1/npm_assets/node_modules/jquery/external/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.971660 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1641 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/LICENSE.txt
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.971660 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    72087 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    20366 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    31265 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3260 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2753 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/jsonp.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1904 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/load.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1637 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/script.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       67 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/var/location.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       72 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/var/nonce.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       60 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/var/rquery.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4355 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/xhr.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    22924 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3272 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/attr.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4527 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/classes.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2857 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/prop.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      786 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/support.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4261 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/val.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      217 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5552 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/callbacks.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1160 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/DOMEval.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1314 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/access.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      550 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/camelCase.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3345 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/init.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      789 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/isAttached.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      176 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/nodeName.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1604 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/parseHTML.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      739 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/parseXML.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2268 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/ready-no-deferred.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2101 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/ready.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      168 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/readyException.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      362 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/stripAndCollapse.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      631 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/support.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      379 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/toType.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      244 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/var/rsingleTag.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     9183 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/core.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.981660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      530 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/addGetHookIf.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2002 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/adjustCSS.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3305 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/curCSS.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      870 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/finalPropName.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      317 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/hiddenVisibleSelectors.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2304 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/showHide.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4829 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/support.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       88 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/cssExpand.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      409 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/getStyles.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1284 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/isHiddenWithinTree.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      123 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/rboxStyle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       57 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/rcustomProp.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      131 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/rnumnonpx.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      501 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/swap.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14195 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/css.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3956 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/Data.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      318 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/var/acceptData.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       84 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/var/dataPriv.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       84 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/var/dataUser.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4325 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/data.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deferred/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      640 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deferred/exceptionHook.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11007 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deferred.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      296 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated/ajax-event-alias.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1140 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated/event.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2406 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1756 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/dimensions.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3291 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects/Tween.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      244 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects/animatedSelector.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17417 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1665 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/focusin.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      133 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/support.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5438 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/trigger.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    24505 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/event.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/exports/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1024 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/exports/amd.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      628 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/exports/global.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      646 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/jquery.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      690 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/_evalUrl.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2490 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/buildFragment.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      654 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/getAll.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      381 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/setGlobalEval.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1244 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/support.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       92 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/var/rscriptType.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      304 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/var/rtagName.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      823 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/wrapMap.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12674 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6828 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/offset.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/queue/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      534 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/queue/delay.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3091 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/queue.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6406 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/selector-native.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      411 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/selector-sizzle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       66 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/selector.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3236 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/serialize.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2352 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/findFilter.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      371 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/var/dir.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      128 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/var/rneedsContext.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      218 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/var/siblings.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4692 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:36.991660 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      110 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/ObjectFunctionString.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       54 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/arr.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       82 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/class2type.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       67 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/document.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      105 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/documentElement.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      372 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/flat.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       92 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/fnToString.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       73 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/getProto.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      110 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/hasOwn.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       82 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/indexOf.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      674 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/isFunction.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      126 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/isWindow.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      100 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/pnum.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       79 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/push.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       79 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/rcheckableType.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      136 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/rcssNum.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      202 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/rnothtmlwhite.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/rtrimCSS.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       80 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/slice.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/support.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      104 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/toString.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      125 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/whitespace.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1477 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/jquery/src/wrap.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/justified-layout/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1075 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1679 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1770 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/demo.html
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/justified-layout/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    23065 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/dist/justified-layout.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11161 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/dist/justified-layout.min.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/justified-layout/lib/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     8115 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/lib/index.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11381 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/lib/row.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2173 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/justified-layout/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/livereload-js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1064 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10651 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/livereload-js/dist/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    38927 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/dist/livereload.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        0 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/.keepme
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5268 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/connector.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1206 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/customevents.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1704 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/less.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7532 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/livereload.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1636 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/options.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3231 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/protocol.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    15736 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/reloader.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      765 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/startup.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      875 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/timer.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1674 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/livereload-js/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/luxon/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1076 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/LICENSE.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2051 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/amd/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   277835 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/amd/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479476 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/amd/luxon.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.001660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/cjs-browser/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   262915 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479472 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.011660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/es6/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   226157 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/es6/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   428684 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/es6/luxon.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.011660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   277851 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   479479 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    73302 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   122652 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.min.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.011660 Nikola-8.3.1/npm_assets/node_modules/luxon/build/node/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   226256 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/node/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   444782 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/node/luxon.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       98 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/build/readme.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2801 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.011660 Nikola-8.3.1/npm_assets/node_modules/luxon/src/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    83972 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/datetime.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    30961 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/duration.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1047 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/errors.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.021660 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4633 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/conversions.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2000 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/diff.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1917 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/digits.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5820 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/english.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2249 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/formats.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    12478 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/formatter.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      282 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/invalid.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14423 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/locale.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10509 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/regexParser.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11447 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/tokenParser.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6933 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/util.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1246 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/zoneUtil.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7581 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/info.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21571 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/interval.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      586 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/luxon.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       45 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/package.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4397 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/settings.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2132 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zone.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.021660 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4565 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/IANAZone.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2175 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/fixedOffsetZone.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      763 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/invalidZone.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1147 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/systemZone.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.021660 Nikola-8.3.1/npm_assets/node_modules/merge/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1092 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/LICENSE
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1155 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      525 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/bower.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2914 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/merge.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1011 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/merge.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1477 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/merge/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.021660 Nikola-8.3.1/npm_assets/node_modules/popper.js/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    11127 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.021660 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.031660 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    35566 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61746 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10654 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53959 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    88482 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140737 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21204 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   125307 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    33894 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61481 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10201 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53753 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    84861 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140064 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19903 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   125107 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.min.js.map
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.031660 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    36668 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    61788 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    10813 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    53756 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    88736 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3114 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js.flow
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   140747 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    21233 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.min.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)   123754 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.min.js.map
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4744 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/index.d.ts
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3114 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/index.js.flow
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2606 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/package.json
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.031660 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5393 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/index.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.041660 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1942 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/defaults.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      989 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/destroy.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      511 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/disableEventListeners.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      444 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/enableEventListeners.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1109 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/placements.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2046 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/update.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.041660 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2752 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/applyStyle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3262 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/arrow.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4016 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/computeStyle.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5094 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/flip.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1207 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/hide.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    14372 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/index.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      922 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/inner.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      895 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/keepTogether.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5943 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/offset.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2849 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/preventOverflow.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      999 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/shift.js
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      773 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/clockwise.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1714 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/computeAutoPlacement.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1121 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/debounce.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      397 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/find.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1681 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/findCommonOffsetParent.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      534 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/findIndex.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      564 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBordersSize.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3000 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBoundaries.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2028 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBoundingClientRect.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      363 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getClientRect.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      756 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getFixedPositionOffsetParent.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1271 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetParent.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      801 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetRect.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2315 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetRectRelativeToArbitraryNode.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      382 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOppositePlacement.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      382 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOppositeVariation.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      652 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOuterSizes.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      315 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getParentNode.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1696 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getPopperOffsets.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      401 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getReferenceNode.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1017 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getReferenceOffsets.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      309 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getRoot.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1754 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getRoundedOffsets.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      668 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getScroll.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      910 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getScrollParent.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      455 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getStyleComputedProperty.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      676 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getSupportedPropertyName.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      898 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getViewportOffsetRectRelativeToArtbitraryNode.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      261 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getWindow.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      785 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getWindowSizes.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      825 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/includeScroll.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2910 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/index.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      117 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isBrowser.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      700 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isFixed.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      377 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isFunction.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      511 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isIE.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      285 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isModifierEnabled.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1095 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isModifierRequired.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      233 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isNumeric.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      286 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isOffsetContainer.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      653 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/removeEventListeners.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1323 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/runModifiers.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      559 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setAttributes.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      695 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setStyles.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1218 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setupEventListeners.js
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4081 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/package-lock.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      469 2023-12-02 08:56:57.000000 Nikola-8.3.1/npm_assets/package.json
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      258 2024-04-29 11:27:23.000000 Nikola-8.3.1/requirements-extras.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      126 2024-04-29 11:27:23.000000 Nikola-8.3.1/requirements-tests.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      244 2024-04-29 11:27:23.000000 Nikola-8.3.1/requirements.txt
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/scripts/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)        0 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/INTERNAL USE ONLY
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1289 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/baseline.sh
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     2868 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/capty
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/scripts/debug_rebuilds/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      868 2024-01-10 19:44:21.000000 Nikola-8.3.1/scripts/debug_rebuilds/README.md
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1259 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/debug_rebuilds/step1_build_and_dumpdb.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1564 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/debug_rebuilds/step2_analyze_py_files.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      883 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/document_path_handlers.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      408 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/generate_symlinked_list.sh
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      543 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/getpyver.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      880 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/github-release.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1229 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/import_po.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)    10154 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/jinjify.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      607 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/langmatrix.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      666 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/langstatus.py
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     5037 2024-01-10 20:54:08.000000 Nikola-8.3.1/scripts/release
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/scripts/snapcraft/
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      457 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/snapcraft/nikola.sh
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)      638 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/theme_snapshot
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     1970 2023-12-02 08:56:57.000000 Nikola-8.3.1/scripts/update-npm-assets.sh
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      238 2024-04-29 12:05:37.071660 Nikola-8.3.1/setup.cfg
+-rwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)     5446 2024-04-29 12:03:29.000000 Nikola-8.3.1/setup.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/tests/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       24 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      456 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/conftest.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/tests/data/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      872 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/1-nolinks.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.051660 Nikola-8.3.1/tests/data/dev_server_sample_output_folder/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      214 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/dev_server_sample_output_folder/index.html
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/metadata_extractors/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      239 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-html-1-compiler.html
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      568 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-ipynb-1-compiler.ipynb
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      160 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-markdown-1-compiler.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      230 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-markdown-1-nikola.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-markdown-2-nikola.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      174 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-markdown-2-nikola.meta
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      166 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-1-compiler.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      209 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-1-nikola.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      155 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-1-toml.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      160 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-1-yaml.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      162 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-nikola.meta
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-nikola.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      123 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-toml.meta
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-toml.rst
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      128 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-yaml.meta
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       32 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/metadata_extractors/f-rest-2-yaml.rst
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/plugin_manager/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/broken.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1578 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/broken.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      197 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/first.plugin
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1614 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/one.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/plugin_manager/second/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      190 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/second/second.plugin
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/plugin_manager/second/two/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1459 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/data/plugin_manager/second/two/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    27095 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/rss-2_0.xsd
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/test_config/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      635 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/test_config/conf.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       88 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/test_config/config.with+illegal(module)name.characters.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       85 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/test_config/prod.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/translated_titles/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1949 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/translated_titles/conf.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/translated_titles/pages/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       30 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/translated_titles/pages/1.pl.txt
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)       59 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/translated_titles/pages/1.txt
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/data/wordpress_import/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    19897 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/wordpress_import/wordpress_export_example.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1955 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/wordpress_import/wordpress_qtranslate_item_modernized.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1995 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/wordpress_import/wordpress_qtranslate_item_raw_export.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6184 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/data/wordpress_import/wordpress_unicode_export.xml
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3342 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/helper.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.061660 Nikola-8.3.1/tests/integration/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      419 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/__init__.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1598 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/conftest.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1772 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/helper.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1142 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_archive_full.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      868 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_archive_per_day.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      883 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_archive_per_month.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      648 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_building_in_subdir.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2586 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_category_destpath.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1264 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_check_absolute_subfolder.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1196 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_check_failure.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      893 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_check_full_path_subfolder.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5992 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_demo_build.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7623 2024-04-29 11:27:23.000000 Nikola-8.3.1/tests/integration/test_dev_server.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1410 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_empty_build.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3040 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_future_post.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6419 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_page_index_normal_urls.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1387 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_page_index_pretty_urls.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3287 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_redirection.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1604 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/integration/test_relative_links.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1810 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/integration/test_relative_links_with_pages_in_root.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      764 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_repeated_posts_setting.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1833 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_translated_content.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1102 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_translated_content_secondary_language.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1545 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_translation_patterns.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1451 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/integration/test_wordpress_import.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17141 2024-04-29 11:27:23.000000 Nikola-8.3.1/tests/test_command_import_wordpress.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5515 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_command_import_wordpress_translation.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3351 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_command_init.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2273 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_compile_markdown.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     1983 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_config.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6986 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_locale.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7224 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_metadata_extractors.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3855 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_path_handlers.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5847 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/test_plugin_manager.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      429 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_plugins.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     5526 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_rss_feeds.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     6484 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_rst_compiler.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4622 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_scheduling.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     7030 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_shortcodes.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2219 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_slugify.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3401 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_task_scale_images.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2219 2024-01-10 19:41:36.000000 Nikola-8.3.1/tests/test_template_shortcodes.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      575 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_test_helper.py
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)    17309 2023-12-02 08:56:57.000000 Nikola-8.3.1/tests/test_utils.py
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.071660 Nikola-8.3.1/translations/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/README.md
+drwxr-xr-x   0 kwpolska  (1000) kwpolska  (1000)        0 2024-04-29 12:05:37.071660 Nikola-8.3.1/translations/nikola.messages/
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)      194 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/README.md
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3155 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/af.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3900 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ar.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3290 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/az.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3798 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/bg.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2495 2024-01-10 20:46:35.000000 Nikola-8.3.1/translations/nikola.messages/bn.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2785 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/br.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3185 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/bs.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3492 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ca.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3325 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/cs.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3069 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/da.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3733 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/de.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4168 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/el.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3132 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/en.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3339 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/eo.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3622 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/es.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3329 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/et.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3360 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/eu.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3827 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/fa.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3445 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/fi.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3749 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/fr.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3167 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/fur.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3139 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/gl.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3464 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/he.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3984 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/hi.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3251 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/hr.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3304 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/hu.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3266 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ia.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3315 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/id.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3533 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/it.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3709 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ja.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3393 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ko.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3303 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/lt.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3208 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/mi.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4427 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ml.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3996 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/mr.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3070 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/nb.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3264 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/nl.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3263 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/oc.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4017 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/pa.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3447 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/pl.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3491 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/pt.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3788 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/pt_BR.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4154 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ru.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3574 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sk.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3090 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sl.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3165 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sq.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3626 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sr.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3155 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sr@latin.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3094 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/sv.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2493 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ta.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4214 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/te.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4109 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/th.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3463 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/tr.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     2664 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/tzm.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     4075 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/uk.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3687 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/ur.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3462 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/vi.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3488 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/zh_CN.po
+-rw-r--r--   0 kwpolska  (1000) kwpolska  (1000)     3156 2023-12-02 08:56:57.000000 Nikola-8.3.1/translations/nikola.messages/zh_TW.po
```

### Comparing `Nikola-8.3.0/AUTHORS.txt` & `Nikola-8.3.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/CHANGES.txt` & `Nikola-8.3.1/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+New in v8.3.1
+=============
+
+Features
+--------
+
+* Support passing ``--poll`` to ``nikola auto`` to better deal with symlink farms.
+
+Bugfixes
+--------
+
+* Remove insecure HTTP fallback from ``nikola plugin``
+* Fix the ``nikola plugin`` command not working (Issue #3736, #3737)
+* Fix ``nikola new_post --available-formats`` crashing with TypeError
+  (Issue #3750)
+* Fix the new plugin manager not loading plugins if the plugin folder is a symlink (Issue #3741)
+* Fix the ``nikola plugin`` command not working (Issue #3736)
+* Remove no longer used leftovers of annotations support (Issue #3764)
+
+Other
+-----
+
+* Nikola now requires Python 3.8 or newer.
+* Nikola has adopted a policy for Python version support,
+  promising support for versions supported by the Python core team,
+  Ubuntu LTS, or Debian stable, and taking into consideration
+  Debian oldstable and PyPy.
+* Remove polyfill from `polyfill.io`.
+
 New in v8.3.0
 =============
 
 Features
 --------
 
 * Implement a new plugin manager from scratch to replace Yapsy,
```

### Comparing `Nikola-8.3.0/CONTRIBUTING.rst` & `Nikola-8.3.1/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,21 @@
       and find a bugfix that doesn’t *require* new feature X, **make a new
       distinct branch and PR** for the bugfix.
 
 * You may want to use the `Tim Pope’s Git commit messages standard
   <http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html>`_.
   It’s not necessary, but if you are doing something big, we recommend
   describing it in the commit message.
+* Your Pull Request should have an informative title and description.
 * While working, rebase instead of merging (if possible). You can use rebase
   instead of merge by default with ``git config pull.rebase true``. If rebases
   fail, you can just use ``git pull --no-rebase``.
+* We will squash your commits when merging the pull request. This means
+  you don’t need to do this yourself (and it’s easier for us to review pull requests
+  which don’t squash things on their own).
 * **Make sure documentation is updated** — at the very least, keep docstrings
   current, and if necessary, update the reStructuredText documentation in ``docs/``.
 * **Add a CHANGELOG entry** at the *top* of ``CHANGES.txt`` mentioning the
   issue number in parentheses and in the correct Features/Bugfixes section. Put
   it under *New in master*.  Create that section if it does not exist yet. Do
   not add an entry if the change is trivial (documentation, typo fixes) or if
   the change is internal (not noticeable to end users in any way).
```

### Comparing `Nikola-8.3.0/LICENSE.txt` & `Nikola-8.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/Nikola.egg-info/PKG-INFO` & `Nikola-8.3.1/Nikola.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nikola
-Version: 8.3.0
+Version: 8.3.1
 Summary: A modular, fast, simple, static website and blog generator
 Home-page: https://getnikola.com/
 Author: Roberto Alsina and others
 Author-email: ralsina@netmanagers.com.ar
 License: MIT
 Keywords: website,blog,static
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,41 +16,37 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: extras
 Provides-Extra: full
 Provides-Extra: tests
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 Nikola, a Static Site and Blog Generator
 ========================================
 
 In goes content, out comes a website, ready to deploy.
 
 .. image:: http://img.shields.io/pypi/v/Nikola.svg
    :target: https://pypi.python.org/pypi/Nikola
 
-.. image:: https://img.shields.io/requires/github/getnikola/nikola.svg
-   :target: https://requires.io/github/getnikola/nikola/requirements/?branch=master
-
 .. image:: https://github.com/getnikola/nikola/workflows/Nikola%20CI/badge.svg
    :target: https://github.com/getnikola/nikola/actions
 
 .. image:: http://img.shields.io/badge/license-MIT-green.svg
    :target: https://github.com/getnikola/nikola/blob/master/LICENSE.txt
 
 Why Static Websites?
@@ -71,15 +67,15 @@
 * Flexible, extensible via the dozens of `available plugins`_
 * Small codebase (programmers can understand all of Nikola core in a day)
 * `reStructuredText`_ or Markdown as input language (also Wiki, BBCode, Textile, and HTML)
 * Easy `image galleries`_ (just drop files in a folder!)
 * Syntax highlighting for almost any programming language or markup
 * Multilingual sites, `translated to 50 languages.`__
 * Doesn't reinvent wheels, leverages existing tools.
-* Python 3.7+ compatible.
+* Python 3.8+ compatible.
 
 .. _Nikola Handbook: https://getnikola.com/handbook.html#why-static
 __ https://users.getnikola.com/
 .. _Themable: https://themes.getnikola.com
 .. _doit: https://pydoit.org
 .. _available plugins: https://plugins.getnikola.com/
 .. _reStructuredText: https://getnikola.com/quickstart.html
```

### Comparing `Nikola-8.3.0/Nikola.egg-info/SOURCES.txt` & `Nikola-8.3.1/Nikola.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Nikola.egg-info/top_level.txt
 docs/creating-a-site.rst
 docs/creating-a-theme.rst
 docs/extending.rst
 docs/internals.rst
 docs/manual.rst
 docs/path_handlers.rst
+docs/python-version-support-policy.rst
 docs/social_buttons.rst
 docs/support.rst
 docs/template-variables.rst
 docs/theming.rst
 docs/architecture/nikola-architecture-draw-io.png
 docs/architecture/nikola-architecture-draw-io.svg
 docs/architecture/nikola-architecture-draw-io.xml
@@ -122,15 +123,14 @@
 nikola/data/shortcodes/jinja/raw.tmpl
 nikola/data/shortcodes/mako/raw.tmpl
 nikola/data/themes/base/README.md
 nikola/data/themes/base/base.theme
 nikola/data/themes/base/bundles
 nikola/data/themes/base-jinja/README.md
 nikola/data/themes/base-jinja/base-jinja.theme
-nikola/data/themes/base-jinja/templates/annotation_helper.tmpl
 nikola/data/themes/base-jinja/templates/archive.tmpl
 nikola/data/themes/base-jinja/templates/archive_navigation_helper.tmpl
 nikola/data/themes/base-jinja/templates/archiveindex.tmpl
 nikola/data/themes/base-jinja/templates/author.tmpl
 nikola/data/themes/base-jinja/templates/authorindex.tmpl
 nikola/data/themes/base-jinja/templates/authors.tmpl
 nikola/data/themes/base-jinja/templates/base.tmpl
@@ -241,15 +241,14 @@
 nikola/data/themes/base/messages/messages_tr.py
 nikola/data/themes/base/messages/messages_tzm.py
 nikola/data/themes/base/messages/messages_uk.py
 nikola/data/themes/base/messages/messages_ur.py
 nikola/data/themes/base/messages/messages_vi.py
 nikola/data/themes/base/messages/messages_zh_cn.py
 nikola/data/themes/base/messages/messages_zh_tw.py
-nikola/data/themes/base/templates/annotation_helper.tmpl
 nikola/data/themes/base/templates/archive.tmpl
 nikola/data/themes/base/templates/archive_navigation_helper.tmpl
 nikola/data/themes/base/templates/archiveindex.tmpl
 nikola/data/themes/base/templates/author.tmpl
 nikola/data/themes/base/templates/authorindex.tmpl
 nikola/data/themes/base/templates/authors.tmpl
 nikola/data/themes/base/templates/base.tmpl
```

### Comparing `Nikola-8.3.0/PKG-INFO` & `Nikola-8.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nikola
-Version: 8.3.0
+Version: 8.3.1
 Summary: A modular, fast, simple, static website and blog generator
 Home-page: https://getnikola.com/
 Author: Roberto Alsina and others
 Author-email: ralsina@netmanagers.com.ar
 License: MIT
 Keywords: website,blog,static
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,41 +16,37 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: extras
 Provides-Extra: full
 Provides-Extra: tests
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 Nikola, a Static Site and Blog Generator
 ========================================
 
 In goes content, out comes a website, ready to deploy.
 
 .. image:: http://img.shields.io/pypi/v/Nikola.svg
    :target: https://pypi.python.org/pypi/Nikola
 
-.. image:: https://img.shields.io/requires/github/getnikola/nikola.svg
-   :target: https://requires.io/github/getnikola/nikola/requirements/?branch=master
-
 .. image:: https://github.com/getnikola/nikola/workflows/Nikola%20CI/badge.svg
    :target: https://github.com/getnikola/nikola/actions
 
 .. image:: http://img.shields.io/badge/license-MIT-green.svg
    :target: https://github.com/getnikola/nikola/blob/master/LICENSE.txt
 
 Why Static Websites?
@@ -71,15 +67,15 @@
 * Flexible, extensible via the dozens of `available plugins`_
 * Small codebase (programmers can understand all of Nikola core in a day)
 * `reStructuredText`_ or Markdown as input language (also Wiki, BBCode, Textile, and HTML)
 * Easy `image galleries`_ (just drop files in a folder!)
 * Syntax highlighting for almost any programming language or markup
 * Multilingual sites, `translated to 50 languages.`__
 * Doesn't reinvent wheels, leverages existing tools.
-* Python 3.7+ compatible.
+* Python 3.8+ compatible.
 
 .. _Nikola Handbook: https://getnikola.com/handbook.html#why-static
 __ https://users.getnikola.com/
 .. _Themable: https://themes.getnikola.com
 .. _doit: https://pydoit.org
 .. _available plugins: https://plugins.getnikola.com/
 .. _reStructuredText: https://getnikola.com/quickstart.html
```

### Comparing `Nikola-8.3.0/README.rst` & `Nikola-8.3.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 ========================================
 
 In goes content, out comes a website, ready to deploy.
 
 .. image:: http://img.shields.io/pypi/v/Nikola.svg
    :target: https://pypi.python.org/pypi/Nikola
 
-.. image:: https://img.shields.io/requires/github/getnikola/nikola.svg
-   :target: https://requires.io/github/getnikola/nikola/requirements/?branch=master
-
 .. image:: https://github.com/getnikola/nikola/workflows/Nikola%20CI/badge.svg
    :target: https://github.com/getnikola/nikola/actions
 
 .. image:: http://img.shields.io/badge/license-MIT-green.svg
    :target: https://github.com/getnikola/nikola/blob/master/LICENSE.txt
 
 Why Static Websites?
@@ -33,15 +30,15 @@
 * Flexible, extensible via the dozens of `available plugins`_
 * Small codebase (programmers can understand all of Nikola core in a day)
 * `reStructuredText`_ or Markdown as input language (also Wiki, BBCode, Textile, and HTML)
 * Easy `image galleries`_ (just drop files in a folder!)
 * Syntax highlighting for almost any programming language or markup
 * Multilingual sites, `translated to 50 languages.`__
 * Doesn't reinvent wheels, leverages existing tools.
-* Python 3.7+ compatible.
+* Python 3.8+ compatible.
 
 .. _Nikola Handbook: https://getnikola.com/handbook.html#why-static
 __ https://users.getnikola.com/
 .. _Themable: https://themes.getnikola.com
 .. _doit: https://pydoit.org
 .. _available plugins: https://plugins.getnikola.com/
 .. _reStructuredText: https://getnikola.com/quickstart.html
```

### Comparing `Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.png` & `Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.svg` & `Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.svg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/architecture/nikola-architecture-draw-io.xml` & `Nikola-8.3.1/docs/architecture/nikola-architecture-draw-io.xml`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/creating-a-site.rst` & `Nikola-8.3.1/docs/creating-a-site.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/creating-a-theme.rst` & `Nikola-8.3.1/docs/creating-a-theme.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/extending.rst` & `Nikola-8.3.1/docs/extending.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: extending
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
```

### Comparing `Nikola-8.3.0/docs/internals.rst` & `Nikola-8.3.1/docs/internals.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/man/nikola.rst` & `Nikola-8.3.1/docs/man/nikola.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Nikola
 ======
 
 --------------------------------
 A Static Site and Blog Generator
 --------------------------------
 
-:Version: Nikola 8.3.0
+:Version: Nikola 8.3.1
 :Manual section: 1
 :Manual group: User Commands
 
 SYNOPSIS
 ========
 
 Create an empty site (with a setup wizard):
```

### Comparing `Nikola-8.3.0/docs/manual.rst` & `Nikola-8.3.1/docs/manual.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. link:
 .. description:
 .. tags:
 .. has_math: true
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 All You Need to Know
@@ -130,15 +130,15 @@
     Also, in the longer term, the very foundations of dynamic sites shift. Can you
     still deploy a blog software based on Django 0.96? What happens when your
     host stops supporting the PHP version you rely on? And so on.
 
     You may say those are long term issues, or that they won't matter for years. Well,
     I believe things should work forever, or as close to it as we can make them.
     Nikola's static output and its input files will work as long as you can install
-    Python 3.7 or newer under Linux, Windows, or macOS and can find a server
+    Python 3.8 or newer under Linux, Windows, or macOS and can find a server
     that sends files over HTTP. That's probably 10 or 15 years at least.
 
     Also, static sites are easily handled by the Internet Archive.
 
 Cost and Performance
     On dynamic sites, every time a reader wants a page, a whole lot of database
     queries are made. Then a whole pile of code chews that data, and HTML is
@@ -1686,18 +1686,14 @@
 In order to use fancy dates, your theme must support them.  The built-in Bootstrap family supports it, but other themes might not by default.
 
 For Mako:
 
 .. code:: html
 
     % if date_fanciness != 0:
-    %if date_fanciness == 2:
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-    %endif
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "${luxon_locales[lang]}";
@@ -1708,18 +1704,14 @@
 
 
 For Jinja2:
 
 .. code:: html
 
     {% if date_fanciness != 0 %}
-    {% if date_fanciness == 2 %}
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-    {% endif %}
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "{{ luxon_locales[lang] }}";
```

### Comparing `Nikola-8.3.0/docs/path_handlers.rst` & `Nikola-8.3.1/docs/path_handlers.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/social_buttons.rst` & `Nikola-8.3.1/docs/social_buttons.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: social_buttons
 .. date: 2013-08-19 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 The Default
```

### Comparing `Nikola-8.3.0/docs/sphinx/Makefile` & `Nikola-8.3.1/docs/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/conf.py` & `Nikola-8.3.1/docs/sphinx/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 copyright = '2012-2024, The Nikola Contributors'
 
 # The version info for the project yo're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '8.3.0'
+version = '8.3.1'
 # The full version, including alpha/beta/rc tags.
-release = '8.3.0'
+release = '8.3.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `Nikola-8.3.0/docs/sphinx/creating-a-site.rst` & `Nikola-8.3.1/docs/sphinx/creating-a-site.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/creating-a-theme.rst` & `Nikola-8.3.1/docs/sphinx/creating-a-theme.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/extending.rst` & `Nikola-8.3.1/docs/sphinx/extending.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: extending
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
```

### Comparing `Nikola-8.3.0/docs/sphinx/index.rst` & `Nikola-8.3.1/docs/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/internals.rst` & `Nikola-8.3.1/docs/sphinx/internals.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/make.bat` & `Nikola-8.3.1/docs/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/manual.rst` & `Nikola-8.3.1/docs/sphinx/manual.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. link:
 .. description:
 .. tags:
 .. has_math: true
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 All You Need to Know
@@ -130,15 +130,15 @@
     Also, in the longer term, the very foundations of dynamic sites shift. Can you
     still deploy a blog software based on Django 0.96? What happens when your
     host stops supporting the PHP version you rely on? And so on.
 
     You may say those are long term issues, or that they won't matter for years. Well,
     I believe things should work forever, or as close to it as we can make them.
     Nikola's static output and its input files will work as long as you can install
-    Python 3.7 or newer under Linux, Windows, or macOS and can find a server
+    Python 3.8 or newer under Linux, Windows, or macOS and can find a server
     that sends files over HTTP. That's probably 10 or 15 years at least.
 
     Also, static sites are easily handled by the Internet Archive.
 
 Cost and Performance
     On dynamic sites, every time a reader wants a page, a whole lot of database
     queries are made. Then a whole pile of code chews that data, and HTML is
@@ -1686,18 +1686,14 @@
 In order to use fancy dates, your theme must support them.  The built-in Bootstrap family supports it, but other themes might not by default.
 
 For Mako:
 
 .. code:: html
 
     % if date_fanciness != 0:
-    %if date_fanciness == 2:
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-    %endif
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "${luxon_locales[lang]}";
@@ -1708,18 +1704,14 @@
 
 
 For Jinja2:
 
 .. code:: html
 
     {% if date_fanciness != 0 %}
-    {% if date_fanciness == 2 %}
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-    {% endif %}
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "{{ luxon_locales[lang] }}";
```

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.command.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.command.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.markdown.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.markdown.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.rest.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.rest.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.compile.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.compile.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.misc.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.misc.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.task.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.task.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.plugins.template.rst` & `Nikola-8.3.1/docs/sphinx/nikola.plugins.template.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola.rst` & `Nikola-8.3.1/docs/sphinx/nikola.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/nikola_titles_for_sphinx.py` & `Nikola-8.3.1/docs/sphinx/nikola_titles_for_sphinx.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/path_handlers.rst` & `Nikola-8.3.1/docs/sphinx/path_handlers.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/docs/sphinx/social_buttons.rst` & `Nikola-8.3.1/docs/sphinx/social_buttons.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: social_buttons
 .. date: 2013-08-19 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 The Default
```

### Comparing `Nikola-8.3.0/docs/sphinx/support.rst` & `Nikola-8.3.1/docs/sphinx/support.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. title: Support and Contact
 .. slug: contact
 .. date: 1970-01-01 15:00:00
 .. description: Get help using Nikola, or contact us.
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 Help and Support
 ================
```

### Comparing `Nikola-8.3.0/docs/sphinx/template-variables.rst` & `Nikola-8.3.1/docs/sphinx/template-variables.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. title: Template variables
 .. slug: template-variables
 .. date: 2017-04-13 12:00:00
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Chris Warrick <chris@getnikola.com>
 
 Variables available in templates are listed below.
 
 * This list is maintained by humans, so it may not always be perfect.
 * Variables whose types are marked with ``?`` may not always be available or may be None in some cases.
 * Templates usually do not have access to the original TranslatableSetting
```

### Comparing `Nikola-8.3.0/docs/sphinx/theming.rst` & `Nikola-8.3.1/docs/sphinx/theming.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: theming
 .. date: 2012-03-13 12:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 .. class:: lead
```

### Comparing `Nikola-8.3.0/docs/support.rst` & `Nikola-8.3.1/docs/support.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. title: Support and Contact
 .. slug: contact
 .. date: 1970-01-01 15:00:00
 .. description: Get help using Nikola, or contact us.
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 Help and Support
 ================
```

### Comparing `Nikola-8.3.0/docs/template-variables.rst` & `Nikola-8.3.1/docs/template-variables.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. title: Template variables
 .. slug: template-variables
 .. date: 2017-04-13 12:00:00
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Chris Warrick <chris@getnikola.com>
 
 Variables available in templates are listed below.
 
 * This list is maintained by humans, so it may not always be perfect.
 * Variables whose types are marked with ``?`` may not always be available or may be None in some cases.
 * Templates usually do not have access to the original TranslatableSetting
```

### Comparing `Nikola-8.3.0/docs/theming.rst` & `Nikola-8.3.1/docs/theming.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: theming
 .. date: 2012-03-13 12:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 .. class:: lead
```

### Comparing `Nikola-8.3.0/dodo.py` & `Nikola-8.3.1/dodo.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/favicon.png` & `Nikola-8.3.1/logo/favicon.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/favicon.svg` & `Nikola-8.3.1/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/nikola-50px-grey.png` & `Nikola-8.3.1/logo/nikola-50px-grey.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/nikola-50px-transparent.png` & `Nikola-8.3.1/logo/nikola-50px-transparent.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/nikola.png` & `Nikola-8.3.1/logo/nikola.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/logo/nikola.svg` & `Nikola-8.3.1/logo/nikola.svg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/__init__.py` & `Nikola-8.3.1/nikola/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Nikola -- a modular, fast, simple, static website generator."""
 
 import os
 import sys
 
-__version__ = '8.3.0'
+__version__ = '8.3.1'
 DEBUG = bool(os.getenv('NIKOLA_DEBUG'))
 SHOW_TRACEBACKS = bool(os.getenv('NIKOLA_SHOW_TRACEBACKS'))
 
 if sys.version_info[0] == 2:
     raise Exception("Nikola does not support Python 2.")
 
 from .nikola import Nikola  # NOQA
```

### Comparing `Nikola-8.3.0/nikola/__main__.py` & `Nikola-8.3.1/nikola/__main__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 # OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 # OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """The main function of Nikola."""
 
-import importlib.util
-import os
-import shutil
-import sys
-import textwrap
-import traceback
-import doit.cmd_base
+from blinker import signal
 from collections import defaultdict
 
-from blinker import signal
+import doit.cmd_base
 from doit.cmd_base import TaskLoader2, _wrap
 from doit.cmd_clean import Clean as DoitClean
 from doit.cmd_completion import TabCompletion
 from doit.cmd_help import Help as DoitHelp
 from doit.cmd_run import Run as DoitRun
 from doit.doit_cmd import DoitMain
 from doit.loader import generate_tasks
 from doit.reporter import ExecutedOnlyReporter
 
+import importlib.util
+import os
+import shutil
+import sys
+import textwrap
+import traceback
+
 from . import __version__
 from .nikola import Nikola
 from .plugin_categories import Command
 from .log import configure_logging, LOGGER, ColorfulFormatter, LoggingMode
 from .utils import get_root_dir, req_missing, sys_decode
 
 try:
     import readline  # NOQA
 except ImportError:
     pass  # This is only so raw_input/input does nicer things if it's available
 
-
 config = {}
 
 # DO NOT USE unless you know what you are doing!
 _RETURN_DOITNIKOLA = False
 
 
 def main(args=None):
```

### Comparing `Nikola-8.3.0/nikola/conf.py.in` & `Nikola-8.3.1/nikola/conf.py.in`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/files/favicon.ico` & `Nikola-8.3.1/nikola/data/samplesite/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/files/images/nikola.png` & `Nikola-8.3.1/nikola/data/samplesite/files/images/nikola.png`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla2_lg.jpg` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla2_lg.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla4_lg.jpg` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla4_lg.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_conducts_lg.webp` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_conducts_lg.webp`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_lightning1_lg.jpg` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_lightning1_lg.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_lightning2_lg.jpg` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_lightning2_lg.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/galleries/demo/tesla_tower1_lg.jpg` & `Nikola-8.3.1/nikola/data/samplesite/galleries/demo/tesla_tower1_lg.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/images/frontispiece.jpg` & `Nikola-8.3.1/nikola/data/samplesite/images/frontispiece.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/images/illus_001.jpg` & `Nikola-8.3.1/nikola/data/samplesite/images/illus_001.jpg`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/bootstrap-demo.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/bootstrap-demo.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/charts.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/charts.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/creating-a-theme.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/creating-a-theme.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/dr-nikolas-vendetta.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/dr-nikolas-vendetta.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/extending.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/extending.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: extending
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
```

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/internals.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/internals.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/manual.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/manual.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. date: 2012-03-30 23:00:00 UTC-03:00
 .. link:
 .. description:
 .. tags:
 .. has_math: true
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 All You Need to Know
@@ -130,15 +130,15 @@
     Also, in the longer term, the very foundations of dynamic sites shift. Can you
     still deploy a blog software based on Django 0.96? What happens when your
     host stops supporting the PHP version you rely on? And so on.
 
     You may say those are long term issues, or that they won't matter for years. Well,
     I believe things should work forever, or as close to it as we can make them.
     Nikola's static output and its input files will work as long as you can install
-    Python 3.7 or newer under Linux, Windows, or macOS and can find a server
+    Python 3.8 or newer under Linux, Windows, or macOS and can find a server
     that sends files over HTTP. That's probably 10 or 15 years at least.
 
     Also, static sites are easily handled by the Internet Archive.
 
 Cost and Performance
     On dynamic sites, every time a reader wants a page, a whole lot of database
     queries are made. Then a whole pile of code chews that data, and HTML is
@@ -1686,18 +1686,14 @@
 In order to use fancy dates, your theme must support them.  The built-in Bootstrap family supports it, but other themes might not by default.
 
 For Mako:
 
 .. code:: html
 
     % if date_fanciness != 0:
-    %if date_fanciness == 2:
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-    %endif
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "${luxon_locales[lang]}";
@@ -1708,18 +1704,14 @@
 
 
 For Jinja2:
 
 .. code:: html
 
     {% if date_fanciness != 0 %}
-    {% if date_fanciness == 2 %}
-        <!-- Polyfill for relative dates in Safari -- best handled with a CDN -->
-        <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-    {% endif %}
     <!-- required scripts -- best handled with bundles -->
     <script src="/assets/js/luxon.min.js"></script>
     <script src="/assets/js/fancydates.js"></script>
 
     <!-- fancy dates code -->
     <script>
     luxon.Settings.defaultLocale = "{{ luxon_locales[lang] }}";
```

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/path_handlers.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/path_handlers.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/quickref.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/quickref.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/quickstart.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/social_buttons.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/social_buttons.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: social_buttons
 .. date: 2013-08-19 23:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 
 The Default
```

### Comparing `Nikola-8.3.0/nikola/data/samplesite/pages/theming.rst` & `Nikola-8.3.1/nikola/data/samplesite/pages/theming.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. slug: theming
 .. date: 2012-03-13 12:00:00 UTC-03:00
 .. tags:
 .. link:
 .. description:
 .. author: The Nikola Team
 
-:Version: 8.3.0
+:Version: 8.3.1
 :Author: Roberto Alsina <ralsina@netmanagers.com.ar>
 
 .. class:: alert alert-primary float-md-right
 
 .. contents::
 
 .. class:: lead
```

### Comparing `Nikola-8.3.0/nikola/data/samplesite/posts/1.rst` & `Nikola-8.3.1/nikola/data/samplesite/posts/1.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/samplesite/templates/book.tmpl` & `Nikola-8.3.1/nikola/data/samplesite/templates/book.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/symlinked.txt` & `Nikola-8.3.1/nikola/data/symlinked.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/baguetteBox.min.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/baguetteBox.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/ipython.min.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/ipython.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/nikola_ipython.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/nikola_ipython.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/nikola_rst.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/nikola_rst.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/rst_base.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/rst_base.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/css/theme.css` & `Nikola-8.3.1/nikola/data/themes/base/assets/css/theme.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/baguetteBox.min.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/baguetteBox.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/fancydates.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/fancydates.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/gallery.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/gallery.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/gallery.min.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/gallery.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/html5.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/html5.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/html5shiv-printshiv.min.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/justified-layout.min.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/justified-layout.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/js/luxon.min.js` & `Nikola-8.3.1/nikola/data/themes/base/assets/js/luxon.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/xml/atom.xsl` & `Nikola-8.3.1/nikola/data/themes/base/assets/xml/atom.xsl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/assets/xml/rss.xsl` & `Nikola-8.3.1/nikola/data/themes/base/assets/xml/rss.xsl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_af.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_af.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ar.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ar.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_az.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_az.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_bg.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_bg.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_bn.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_bn.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_br.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_br.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_bs.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_bs.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ca.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ca.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_cs.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_cs.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_cz.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_cz.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_da.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_da.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_de.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_de.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_el.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_el.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_en.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_en.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_eo.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_eo.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_es.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_es.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_et.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_et.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_eu.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_eu.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_fa.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_fa.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_fi.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_fi.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_fr.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_fr.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_fur.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_fur.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_gl.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_gl.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_he.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_he.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_hi.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_hi.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_hr.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_hr.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_hu.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_hu.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ia.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ia.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_id.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_id.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_it.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_it.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ja.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ja.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ko.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ko.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_lt.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_lt.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_mi.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_mi.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ml.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ml.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_mr.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_mr.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_nb.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_nb.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_nl.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_nl.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_oc.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_oc.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_pa.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_pa.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_pl.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_pl.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_pt.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_pt.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_pt_br.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_pt_br.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ru.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ru.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sk.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sk.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sl.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sl.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sq.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sq.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sr.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sr.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sr_latin.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sr_latin.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_sv.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_sv.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ta.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ta.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_te.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_te.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_th.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_th.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_tr.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_tr.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_tzm.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_tzm.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_uk.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_uk.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_ur.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_ur.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_vi.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_vi.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_zh_cn.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_zh_cn.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/messages/messages_zh_tw.py` & `Nikola-8.3.1/nikola/data/themes/base/messages/messages_zh_tw.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/archive_navigation_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/archive_navigation_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/archiveindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/archiveindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/author.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/author.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/authorindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/authorindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/authors.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/authors.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/base.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/base_header.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/base_header.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/base_helper.tmpl`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,14 @@
         % if use_cdn:
             <script src="https://cdnjs.cloudflare.com/ajax/libs/baguettebox.js/1.11.1/baguetteBox.min.js" integrity="sha256-ULQV01VS9LCI2ePpLsmka+W0mawFpEA0rtxnezUj4A4=" crossorigin="anonymous"></script>
         % else:
             <script src="/assets/js/baguetteBox.min.js"></script>
         % endif
     % endif
     % if date_fanciness != 0:
-        % if date_fanciness == 2:
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-        % endif
         % if use_cdn:
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         % else:
             <script src="/assets/js/luxon.min.js"></script>
         % endif
         % if not use_bundles:
             <script src="/assets/js/fancydates.min.js"></script>
```

#### html2text {}

```diff
@@ -17,16 +17,15 @@
 % endif %if prevlink:
 %endif %if nextlink:
 %endif %if use_cdn: %else: %endif ${extra_head_data}
 def> <%def name="late_load_js()"> % if use_bundles: % if use_cdn:
 % else:
 % endif % else: % if use_cdn:
 % else:
-% endif % endif % if date_fanciness != 0: % if date_fanciness == 2:
-% endif % if use_cdn:
+% endif % endif % if date_fanciness != 0: % if use_cdn:
 % else:
 % endif % if not use_bundles:
 % endif % endif ${social_buttons_code}
 def> <%def name="html_stylesheets()"> %if use_bundles: %if use_cdn:
 %else:
 %endif %else:
 %if has_custom_css:
```

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_discourse.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_discourse.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_disqus.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_disqus.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_facebook.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_facebook.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_intensedebate.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_intensedebate.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_isso.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_isso.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/comments_helper_utterances.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/comments_helper_utterances.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/feeds_translations_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/feeds_translations_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/gallery.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/gallery.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/index.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/index.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/index_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/index_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/list.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/list.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/list_post.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/list_post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/listing.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/listing.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/math_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/math_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/pagination_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/pagination_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/post.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/post_header.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/post_header.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/post_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/post_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/story.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/story.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/tag.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/tag.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/tagindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/tagindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base/templates/tags.tmpl` & `Nikola-8.3.1/nikola/data/themes/base/templates/tags.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/archive_navigation_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/archive_navigation_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/archiveindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/archiveindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/author.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/author.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/authorindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/authorindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/authors.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/authors.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base_header.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base_header.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/base_helper.tmpl`

 * *Files 3% similar despite different names*

```diff
@@ -74,17 +74,14 @@
         {% if use_cdn %}
             <script src="https://cdnjs.cloudflare.com/ajax/libs/baguettebox.js/1.11.1/baguetteBox.min.js" integrity="sha256-ULQV01VS9LCI2ePpLsmka+W0mawFpEA0rtxnezUj4A4=" crossorigin="anonymous"></script>
         {% else %}
             <script src="/assets/js/baguetteBox.min.js"></script>
         {% endif %}
     {% endif %}
     {% if date_fanciness != 0 %}
-        {% if date_fanciness == 2 %}
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-        {% endif %}
         {% if use_cdn %}
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         {% else %}
             <script src="/assets/js/luxon.min.js"></script>
         {% endif %}
         {% if not use_bundles %}
             <script src="/assets/js/fancydates.min.js"></script>
```

#### html2text {}

```diff
@@ -17,17 +17,15 @@
 {% endif %} {% if prevlink %}
 {% endif %} {% if nextlink %}
 {% endif %} {% if use_cdn %} {% else %} {% endif %} {{ extra_head_data }} {%
 endmacro %} {% macro late_load_js() %} {% if use_bundles %} {% if use_cdn %}
 {% else %}
 {% endif %} {% else %} {% if use_cdn %}
 {% else %}
-{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if date_fanciness == 2
-%}
-{% endif %} {% if use_cdn %}
+{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if use_cdn %}
 {% else %}
 {% endif %} {% if not use_bundles %}
 {% endif %} {% endif %} {{ social_buttons_code }} {% endmacro %} {% macro
 html_stylesheets() %} {% if use_bundles %} {% if use_cdn %}
 {% else %}
 {% endif %} {% else %}
 {% if has_custom_css %}
```

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_discourse.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_discourse.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_disqus.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_disqus.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_facebook.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_facebook.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_intensedebate.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_intensedebate.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_isso.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_isso.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/comments_helper_utterances.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/comments_helper_utterances.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/feeds_translations_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/feeds_translations_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/gallery.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/gallery.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/index.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/index.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/index_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/index_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/list.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/list.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/list_post.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/list_post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/listing.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/listing.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/math_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/math_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/pagination_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/pagination_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_header.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_header.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/post_list_directive.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/post_list_directive.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/story.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/story.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tag.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tag.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tagindex.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tagindex.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/base-jinja/templates/tags.tmpl` & `Nikola-8.3.1/nikola/data/themes/base-jinja/templates/tags.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4/assets/css/bootblog.css` & `Nikola-8.3.1/nikola/data/themes/bootblog4/assets/css/bootblog.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4/bundles` & `Nikola-8.3.1/nikola/data/themes/bootblog4/bundles`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4/templates/base.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ## -*- coding: utf-8 -*-
 <%namespace name="base" file="base_helper.tmpl" import="*" />
-<%namespace name="notes" file="annotation_helper.tmpl" import="*" />
 ${set_locale(lang)}
 ${base.html_headstart()}
 <%block name="extra_head">
 ### Leave this block alone.
 </%block>
 ${template_hooks['extra_head']()}
 </head>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 ## -*- coding: utf-8 -*- <%namespace name="base" file="base_helper.tmpl"
-import="*" /> <%namespace name="notes" file="annotation_helper.tmpl" import="*"
-/> ${set_locale(lang)} ${base.html_headstart()} <%block name="extra_head"> ###
-Leave this block alone.
+import="*" /> ${set_locale(lang)} ${base.html_headstart()} <%block
+name="extra_head"> ### Leave this block alone.
 block> ${template_hooks['extra_head']()}
 _$_{_m_e_s_s_a_g_e_s_(_"_S_k_i_p_ _t_o_ _m_a_i_n_ _c_o_n_t_e_n_t_"_)_}
 ${search_form}
 _%_i_f_ _l_o_g_o___u_r_l_:_ _[_$_{_b_l_o_g___t_i_t_l_e_|_h_}_]_%_e_n_d_i_f_ _%_ _i_f_ _s_h_o_w___b_l_o_g___t_i_t_l_e_:_ _$_{_b_l_o_g___t_i_t_l_e_|_h_}_ _%
 _e_n_d_i_f
     * ${base.html_navigation_links_entries(navigation_alt_links)} <%block
       name="belowtitle"> %if len(translations) > 1: ${base.html_translations()}
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4/templates/base_helper.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             <script src="/assets/js/jquery.min.js"></script>
             <script src="/assets/js/popper.min.js"></script>
             <script src="/assets/js/bootstrap.min.js"></script>
             <script src="/assets/js/baguetteBox.min.js"></script>
         %endif
     %endif
     %if date_fanciness != 0:
-        %if date_fanciness == 2:
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-        %endif
         %if use_cdn:
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         %else:
             <script src="/assets/js/luxon.min.js"></script>
         %endif
         %if not use_bundles:
             <script src="/assets/js/fancydates.min.js"></script>
```

#### html2text {}

```diff
@@ -16,16 +16,15 @@
 % endif %if prevlink:
 %endif %if nextlink:
 %endif %if use_cdn: %else: %endif ${extra_head_data}
 def> <%def name="late_load_js()"> %if use_cdn:
 % endif %if use_bundles and use_cdn:
 %elif use_bundles:
 %else: %if not use_cdn:
-%endif %endif %if date_fanciness != 0: %if date_fanciness == 2:
-%endif %if use_cdn:
+%endif %endif %if date_fanciness != 0: %if use_cdn:
 %else:
 %endif %if not use_bundles:
 %endif %endif ${social_buttons_code}
 def> <%def name="html_stylesheets()"> % if use_cdn:
 % endif %if use_bundles and use_cdn:
 %elif use_bundles:
 %else: %if not use_cdn:
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4/templates/index.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4/templates/index.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/assets/css/bootblog.css` & `Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/assets/css/bootblog.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/bundles` & `Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/bundles`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/base.tmpl`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {#  -*- coding: utf-8 -*- #}
 {% import 'base_helper.tmpl' as base with context %}
-{% import 'annotation_helper.tmpl' as notes with context %}
 {{ set_locale(lang) }}
 {{ base.html_headstart() }}
 {% block extra_head %}
 {#  Leave this block alone. #}
 {% endblock %}
 {{ template_hooks['extra_head']() }}
 </head>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 {# -*- coding: utf-8 -*- #} {% import 'base_helper.tmpl' as base with context
-%} {% import 'annotation_helper.tmpl' as notes with context %} {{ set_locale
-(lang) }} {{ base.html_headstart() }} {% block extra_head %} {# Leave this
-block alone. #} {% endblock %} {{ template_hooks['extra_head']() }}
+%} {{ set_locale(lang) }} {{ base.html_headstart() }} {% block extra_head %} {#
+Leave this block alone. #} {% endblock %} {{ template_hooks['extra_head']() }}
 _{_{_ _m_e_s_s_a_g_e_s_(_"_S_k_i_p_ _t_o_ _m_a_i_n_ _c_o_n_t_e_n_t_"_)_ _}_}
 {{ search_form }}
 }"> {% if logo_url %} [{{ blog_title|e }}]{% endif %} {% if show_blog_title %}
 {{ blog_title|e }} {% endif %}
     * {{ base.html_navigation_links_entries(navigation_alt_links) }} {% block
       belowtitle %} {% if translations|length > 1 %} {{ base.html_translations
       () }} {% endif %} {% endblock %} {% block sourcelink %}{% endblock %} {
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/base_helper.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             <script src="/assets/js/jquery.min.js"></script>
             <script src="/assets/js/popper.min.js"></script>
             <script src="/assets/js/bootstrap.min.js"></script>
             <script src="/assets/js/baguetteBox.min.js"></script>
         {% endif %}
     {% endif %}
     {% if date_fanciness != 0 %}
-        {% if date_fanciness == 2 %}
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-        {% endif %}
         {% if use_cdn %}
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         {% else %}
             <script src="/assets/js/luxon.min.js"></script>
         {% endif %}
         {% if not use_bundles %}
             <script src="/assets/js/fancydates.min.js"></script>
@@ -111,24 +108,22 @@
         {% if not use_cdn %}
             <link href="/assets/css/bootstrap.min.css" rel="stylesheet" type="text/css">
             <link href="/assets/css/baguetteBox.min.css" rel="stylesheet" type="text/css">
         {% endif %}
         <link href="/assets/css/rst.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/code.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/theme.css" rel="stylesheet" type="text/css">
-        <link href="/assets/css/bootblog.css" rel="stylesheet" type="text/css">
         {% if has_custom_css %}
             <link href="/assets/css/custom.css" rel="stylesheet" type="text/css">
         {% endif %}
     {% endif %}
     {% if needs_ipython_css %}
         <link href="/assets/css/ipython.min.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/nikola_ipython.css" rel="stylesheet" type="text/css">
     {% endif %}
-    <link href="https://fonts.googleapis.com/css?family=Playfair+Display:700,900" rel="stylesheet">
 {% endmacro %}
 
 {% macro html_navigation_links() %}
     {{ html_navigation_links_entries(navigation_links) }}
 {% endmacro %}
 
 {% macro html_navigation_links_entries(navigation_links_source) %}
@@ -150,16 +145,14 @@
             {% else %}
                 <li class="nav-item"><a href="{{ url }}" class="nav-link">{{ text }}</a>
             {% endif %}
         {% endif %}
     {% endfor %}
 {% endmacro %}
 
-
-
 {% macro html_feedlinks() %}
     {{ feeds_translations.head(classification=None, kind='index', other=False) }}
 {% endmacro %}
 
 {% macro html_translations() %}
     {% for langname in translations|sort %}
         {% if langname != lang %}
```

#### html2text {}

```diff
@@ -14,29 +14,26 @@
 {% endif %} {% if prevlink %}
 {% endif %} {% if nextlink %}
 {% endif %} {% if use_cdn %} {% else %} {% endif %} {{ extra_head_data }} {%
 endmacro %} {% macro late_load_js() %} {% if use_cdn %}
 {% endif %} {% if use_bundles and use_cdn %}
 {% elif use_bundles %}
 {% else %} {% if not use_cdn %}
-{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if date_fanciness == 2
-%}
-{% endif %} {% if use_cdn %}
+{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if use_cdn %}
 {% else %}
 {% endif %} {% if not use_bundles %}
 {% endif %} {% endif %} {{ social_buttons_code }} {% endmacro %} {% macro
 html_stylesheets() %} {% if use_cdn %}
 {% endif %} {% if use_bundles and use_cdn %}
 {% elif use_bundles %}
 {% else %} {% if not use_cdn %}
 {% endif %}
 {% if has_custom_css %}
 {% endif %} {% endif %} {% if needs_ipython_css %}
-{% endif %}
-{% endmacro %} {% macro html_navigation_links() %} {
+{% endif %} {% endmacro %} {% macro html_navigation_links() %} {
 { html_navigation_links_entries(navigation_links) }} {% endmacro %} {% macro
 html_navigation_links_entries(navigation_links_source) %} {% for url, text in
 navigation_links_source[lang] %} {% if isinstance(url, tuple) %}
 _{_{_ _t_e_x_t_ _}_}
 {% for suburl, text in url %} {% if rel_link(permalink, suburl) == "#" %} _{
 _{_ _t_e_x_t_ _}_}_ _{_{_ _m_e_s_s_a_g_e_s_(_"_(_a_c_t_i_v_e_)_"_,_ _l_a_n_g_)_ _}_} {% else %} _{_{_ _t_e_x_t_ _}_} {% endif %} {%
 endfor %}
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootblog4-jinja/templates/index.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/index.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/css/bootstrap.min.css` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/css/theme.css` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/css/theme.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/bootstrap.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/jquery.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/assets/js/popper.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/assets/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/authors.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/authors.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/base.tmpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ## -*- coding: utf-8 -*-
 <%namespace name="base" file="base_helper.tmpl" import="*" />
-<%namespace name="notes" file="annotation_helper.tmpl" import="*" />
 ${set_locale(lang)}
 ${base.html_headstart()}
 <%block name="extra_head">
 ### Leave this block alone.
 </%block>
 ${template_hooks['extra_head']()}
 </head>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 ## -*- coding: utf-8 -*- <%namespace name="base" file="base_helper.tmpl"
-import="*" /> <%namespace name="notes" file="annotation_helper.tmpl" import="*"
-/> ${set_locale(lang)} ${base.html_headstart()} <%block name="extra_head"> ###
-Leave this block alone.
+import="*" /> ${set_locale(lang)} ${base.html_headstart()} <%block
+name="extra_head"> ### Leave this block alone.
 block> ${template_hooks['extra_head']()}
 _$_{_m_e_s_s_a_g_e_s_(_"_S_k_i_p_ _t_o_ _m_a_i_n_ _c_o_n_t_e_n_t_"_)_}
 _%_i_f_ _l_o_g_o___u_r_l_:_ _[_$_{_b_l_o_g___t_i_t_l_e_|_h_}_]_%_e_n_d_i_f_ _%_ _i_f_ _s_h_o_w___b_l_o_g___t_i_t_l_e_:_ _$_{_b_l_o_g___t_i_t_l_e_|_h_}_ _%
 _e_n_d_i_f
     * ${base.html_navigation_links_entries(navigation_links)} ${template_hooks
       ['menu']()}
 %if search_form: ${search_form} %endif
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/base_helper.tmpl`

 * *Files 5% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             <script src="/assets/js/jquery.min.js"></script>
             <script src="/assets/js/popper.min.js"></script>
             <script src="/assets/js/bootstrap.min.js"></script>
             <script src="/assets/js/baguetteBox.min.js"></script>
         %endif
     %endif
     %if date_fanciness != 0:
-        %if date_fanciness == 2:
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.${luxon_locales[lang]}"></script>
-        %endif
         %if use_cdn:
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         %else:
             <script src="/assets/js/luxon.min.js"></script>
         %endif
         %if not use_bundles:
             <script src="/assets/js/fancydates.min.js"></script>
```

#### html2text {}

```diff
@@ -16,16 +16,15 @@
 % endif %if prevlink:
 %endif %if nextlink:
 %endif %if use_cdn: %else: %endif ${extra_head_data}
 def> <%def name="late_load_js()"> %if use_cdn:
 % endif %if use_bundles and use_cdn:
 %elif use_bundles:
 %else: %if not use_cdn:
-%endif %endif %if date_fanciness != 0: %if date_fanciness == 2:
-%endif %if use_cdn:
+%endif %endif %if date_fanciness != 0: %if use_cdn:
 %else:
 %endif %if not use_bundles:
 %endif %endif ${social_buttons_code}
 def> <%def name="html_stylesheets()"> %if use_cdn:
 % endif %if use_bundles and use_cdn:
 %elif use_bundles:
 %else: %if not use_cdn:
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/listing.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/listing.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/pagination_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/pagination_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/post.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/tags.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/tags.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4/templates/ui_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4/templates/ui_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/css/bootstrap.min.css` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/css/theme.css` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/css/theme.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/bootstrap.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/jquery.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/assets/js/popper.min.js` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/assets/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/authors.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/authors.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/base.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/base.tmpl`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {#  -*- coding: utf-8 -*- #}
 {% import 'base_helper.tmpl' as base with context %}
-{% import 'annotation_helper.tmpl' as notes with context %}
 {{ set_locale(lang) }}
 {{ base.html_headstart() }}
 {% block extra_head %}
 {#  Leave this block alone. #}
 {% endblock %}
 {{ template_hooks['extra_head']() }}
 </head>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 {# -*- coding: utf-8 -*- #} {% import 'base_helper.tmpl' as base with context
-%} {% import 'annotation_helper.tmpl' as notes with context %} {{ set_locale
-(lang) }} {{ base.html_headstart() }} {% block extra_head %} {# Leave this
-block alone. #} {% endblock %} {{ template_hooks['extra_head']() }}
+%} {{ set_locale(lang) }} {{ base.html_headstart() }} {% block extra_head %} {#
+Leave this block alone. #} {% endblock %} {{ template_hooks['extra_head']() }}
 _{_{_ _m_e_s_s_a_g_e_s_(_"_S_k_i_p_ _t_o_ _m_a_i_n_ _c_o_n_t_e_n_t_"_)_ _}_}
 }"> {% if logo_url %} [{{ blog_title|e }}]{% endif %} {% if show_blog_title %}
 {{ blog_title|e }} {% endif %}
     * {{ base.html_navigation_links_entries(navigation_links) }} {
       { template_hooks['menu']() }}
 {% if search_form %} {{ search_form }} {% endif %}
     * {{ base.html_navigation_links_entries(navigation_alt_links) }} {% block
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/base_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootblog4-jinja/templates/base_helper.tmpl`

 * *Files 3% similar despite different names*

```diff
@@ -78,17 +78,14 @@
             <script src="/assets/js/jquery.min.js"></script>
             <script src="/assets/js/popper.min.js"></script>
             <script src="/assets/js/bootstrap.min.js"></script>
             <script src="/assets/js/baguetteBox.min.js"></script>
         {% endif %}
     {% endif %}
     {% if date_fanciness != 0 %}
-        {% if date_fanciness == 2 %}
-            <script src="https://polyfill.io/v3/polyfill.js?features=Intl.RelativeTimeFormat.%7Elocale.{{ luxon_locales[lang] }}"></script>
-        {% endif %}
         {% if use_cdn %}
             <script src="https://cdn.jsdelivr.net/npm/luxon@3.3.0/build/global/luxon.min.js" integrity="sha256-Nn+JGDrq3PuTxcDfJmmI0Srj5LpfOFlKqEiPwQK7y40=" crossorigin="anonymous"></script>
         {% else %}
             <script src="/assets/js/luxon.min.js"></script>
         {% endif %}
         {% if not use_bundles %}
             <script src="/assets/js/fancydates.min.js"></script>
@@ -111,22 +108,24 @@
         {% if not use_cdn %}
             <link href="/assets/css/bootstrap.min.css" rel="stylesheet" type="text/css">
             <link href="/assets/css/baguetteBox.min.css" rel="stylesheet" type="text/css">
         {% endif %}
         <link href="/assets/css/rst.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/code.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/theme.css" rel="stylesheet" type="text/css">
+        <link href="/assets/css/bootblog.css" rel="stylesheet" type="text/css">
         {% if has_custom_css %}
             <link href="/assets/css/custom.css" rel="stylesheet" type="text/css">
         {% endif %}
     {% endif %}
     {% if needs_ipython_css %}
         <link href="/assets/css/ipython.min.css" rel="stylesheet" type="text/css">
         <link href="/assets/css/nikola_ipython.css" rel="stylesheet" type="text/css">
     {% endif %}
+    <link href="https://fonts.googleapis.com/css?family=Playfair+Display:700,900" rel="stylesheet">
 {% endmacro %}
 
 {% macro html_navigation_links() %}
     {{ html_navigation_links_entries(navigation_links) }}
 {% endmacro %}
 
 {% macro html_navigation_links_entries(navigation_links_source) %}
@@ -148,14 +147,16 @@
             {% else %}
                 <li class="nav-item"><a href="{{ url }}" class="nav-link">{{ text }}</a>
             {% endif %}
         {% endif %}
     {% endfor %}
 {% endmacro %}
 
+
+
 {% macro html_feedlinks() %}
     {{ feeds_translations.head(classification=None, kind='index', other=False) }}
 {% endmacro %}
 
 {% macro html_translations() %}
     {% for langname in translations|sort %}
         {% if langname != lang %}
```

#### html2text {}

```diff
@@ -14,28 +14,27 @@
 {% endif %} {% if prevlink %}
 {% endif %} {% if nextlink %}
 {% endif %} {% if use_cdn %} {% else %} {% endif %} {{ extra_head_data }} {%
 endmacro %} {% macro late_load_js() %} {% if use_cdn %}
 {% endif %} {% if use_bundles and use_cdn %}
 {% elif use_bundles %}
 {% else %} {% if not use_cdn %}
-{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if date_fanciness == 2
-%}
-{% endif %} {% if use_cdn %}
+{% endif %} {% endif %} {% if date_fanciness != 0 %} {% if use_cdn %}
 {% else %}
 {% endif %} {% if not use_bundles %}
 {% endif %} {% endif %} {{ social_buttons_code }} {% endmacro %} {% macro
 html_stylesheets() %} {% if use_cdn %}
 {% endif %} {% if use_bundles and use_cdn %}
 {% elif use_bundles %}
 {% else %} {% if not use_cdn %}
 {% endif %}
 {% if has_custom_css %}
 {% endif %} {% endif %} {% if needs_ipython_css %}
-{% endif %} {% endmacro %} {% macro html_navigation_links() %} {
+{% endif %}
+{% endmacro %} {% macro html_navigation_links() %} {
 { html_navigation_links_entries(navigation_links) }} {% endmacro %} {% macro
 html_navigation_links_entries(navigation_links_source) %} {% for url, text in
 navigation_links_source[lang] %} {% if isinstance(url, tuple) %}
 _{_{_ _t_e_x_t_ _}_}
 {% for suburl, text in url %} {% if rel_link(permalink, suburl) == "#" %} _{
 _{_ _t_e_x_t_ _}_}_ _{_{_ _m_e_s_s_a_g_e_s_(_"_(_a_c_t_i_v_e_)_"_,_ _l_a_n_g_)_ _}_} {% else %} _{_{_ _t_e_x_t_ _}_} {% endif %} {%
 endfor %}
```

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/listing.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/listing.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/pagination_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/pagination_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/post.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/post.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/tags.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/tags.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/data/themes/bootstrap4-jinja/templates/ui_helper.tmpl` & `Nikola-8.3.1/nikola/data/themes/bootstrap4-jinja/templates/ui_helper.tmpl`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/filters.py` & `Nikola-8.3.1/nikola/filters.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/hierarchy_utils.py` & `Nikola-8.3.1/nikola/hierarchy_utils.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/image_processing.py` & `Nikola-8.3.1/nikola/image_processing.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/log.py` & `Nikola-8.3.1/nikola/log.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/metadata_extractors.py` & `Nikola-8.3.1/nikola/metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/nikola.py` & `Nikola-8.3.1/nikola/nikola.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 from urllib.parse import urlparse, urlsplit, urlunsplit, urljoin, unquote, parse_qs
 
 import dateutil.tz
 import lxml.etree
 import lxml.html
 import natsort
 import PyRSS2Gen as rss
-from pkg_resources import resource_filename
 from blinker import signal
 
 from . import DEBUG, SHOW_TRACEBACKS, filters, utils, hierarchy_utils, shortcodes
 from . import metadata_extractors
 from .metadata_extractors import default_metadata_extractors_by
 from .post import Post  # NOQA
 from .plugin_manager import PluginCandidate, PluginInfo, PluginManager
@@ -1027,15 +1026,15 @@
         return result
 
     def init_plugins(self, commands_only=False, load_all=False):
         """Load plugins as needed."""
         extra_plugins_dirs = self.config['EXTRA_PLUGINS_DIRS']
         self._loading_commands_only = commands_only
         self._plugin_places = [
-            resource_filename('nikola', 'plugins'),
+            utils.pkg_resources_path('nikola', 'plugins'),
             os.path.expanduser(os.path.join('~', '.nikola', 'plugins')),
             os.path.join(os.getcwd(), 'plugins'),
         ] + [path for path in extra_plugins_dirs if path]
         self._plugin_places = [pathlib.Path(p) for p in self._plugin_places]
 
         self.plugin_manager = PluginManager(plugin_places=self._plugin_places)
 
@@ -1053,16 +1052,19 @@
         # needed by any PostScanner plugin and put them into self.disabled_compilers
         # (respectively self.disabled_compiler_extensions).
         self.config['COMPILERS'] = {}
         self.disabled_compilers = {}
         self.disabled_compiler_extensions = defaultdict(list)
 
         candidates = self.plugin_manager.locate_plugins()
-        good_candidates = set()
-        if not load_all:
+
+        if load_all:
+            good_candidates = set(candidates)
+        else:
+            good_candidates = set()
             for p in candidates:
                 if commands_only:
                     if p.category != 'Command':
                         continue
                 elif self.configured:  # Not commands-only, and configured
                     # Remove blacklisted plugins
                     if p.name in self.config['DISABLED_PLUGINS']:
@@ -1687,15 +1689,15 @@
 
         This will register a shortcode for any template found in shortcodes/
         folders and a generic "template" shortcode which will consider the
         content in the shortcode as a template in itself.
         """
         self.register_shortcode('template', self._template_shortcode_handler)
 
-        builtin_sc_dir = resource_filename(
+        builtin_sc_dir = utils.pkg_resources_path(
             'nikola',
             os.path.join('data', 'shortcodes', utils.get_template_engine(self.THEMES)))
 
         for sc_dir in [builtin_sc_dir, 'shortcodes']:
             if not os.path.isdir(sc_dir):
                 continue
```

### Comparing `Nikola-8.3.0/nikola/packages/datecond/LICENSE` & `Nikola-8.3.1/nikola/packages/datecond/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/datecond/__init__.py` & `Nikola-8.3.1/nikola/packages/datecond/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/pygments_better_html/LICENSE` & `Nikola-8.3.1/nikola/packages/pygments_better_html/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/pygments_better_html/LICENSE.pygments` & `Nikola-8.3.1/nikola/packages/pygments_better_html/LICENSE.pygments`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/pygments_better_html/__init__.py` & `Nikola-8.3.1/nikola/packages/pygments_better_html/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/tzlocal/LICENSE.txt` & `Nikola-8.3.1/nikola/packages/tzlocal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/tzlocal/unix.py` & `Nikola-8.3.1/nikola/packages/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/tzlocal/win32.py` & `Nikola-8.3.1/nikola/packages/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/packages/tzlocal/windows_tz.py` & `Nikola-8.3.1/nikola/packages/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugin_categories.py` & `Nikola-8.3.1/nikola/plugin_categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 )
 
 
 class BasePlugin:
     """Base plugin class."""
 
     logger = None
+    site: 'nikola.nikola.Nikola'
 
     def set_site(self, site):
         """Set site, which is a Nikola instance."""
         self.site = site
         self.logger = get_logger(self.name)
         if not site.debug:
             self.logger.level = logging.INFO
```

### Comparing `Nikola-8.3.0/nikola/plugin_manager.py` & `Nikola-8.3.1/nikola/plugin_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 """The Nikola plugin manager. Inspired by yapsy."""
 
 import configparser
 import importlib
 import importlib.util
 import time
 import sys
+
+from collections import deque
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Optional, Type, TYPE_CHECKING, Set
 
 from .plugin_categories import BasePlugin, CATEGORIES
 from .utils import get_logger
 
@@ -53,31 +55,34 @@
 
 @dataclass(frozen=True)
 class PluginCandidate:
     """A candidate plugin that was located but not yet loaded (imported)."""
 
     name: str
     description: Optional[str]
+    friendly_name: str
     plugin_id: str
     category: str
     compiler: Optional[str]
     source_dir: Path
     module_name: str
 
 
 @dataclass(frozen=True)
 class PluginInfo:
     """A plugin that was loaded (imported)."""
 
     name: str
     description: Optional[str]
+    friendly_name: str
     plugin_id: str
     category: str
     compiler: Optional[str]
     source_dir: Path
+    py_file_location: Path
     module_name: str
     module_object: object
     plugin_object: BasePlugin
 
 
 class PluginManager:
     """The Nikola plugin manager."""
@@ -98,17 +103,21 @@
         self._plugins_by_category = {}
         self.logger = get_logger("PluginManager")
 
     def locate_plugins(self) -> List[PluginCandidate]:
         """Locate plugins in plugin_places."""
         self.candidates = []
 
+        plugin_folders: deque = deque([place for place in self.plugin_places if place.exists() and place.is_dir()])
         plugin_files: List[Path] = []
-        for place in self.plugin_places:
-            plugin_files += place.rglob("*.plugin")
+        while plugin_folders:
+            base_folder = plugin_folders.popleft()
+            items = list(base_folder.iterdir())
+            plugin_folders.extend([item for item in items if item.is_dir() and item.name != "__pycache__"])
+            plugin_files.extend([item for item in items if item.suffix == ".plugin" and not item.is_dir()])
 
         for plugin_file in plugin_files:
             source_dir = plugin_file.parent
             config = configparser.ConfigParser()
             config.read(plugin_file)
             name = config["Core"]["name"]
             module_name = config["Core"]["module"]
@@ -119,14 +128,15 @@
             if "Nikola" not in config:
                 self.logger.warning(f"{plugin_id} does not specify Nikola configuration - plugin will not be loaded")
                 self.logger.warning("Please add a [Nikola] section to the {plugin_file} file with a PluginCategory entry")
                 self.has_warnings = True
                 continue
             category = config["Nikola"].get("PluginCategory")
             compiler = config["Nikola"].get("Compiler")
+            friendly_name = config["Nikola"].get("friendlyname") or name
             if not category:
                 self.logger.warning(f"{plugin_id} does not specify any category (Nikola.PluginCategory is missing in .plugin file) - plugin will not be loaded")
                 self.has_warnings = True
                 continue
             if category in LEGACY_PLUGIN_NAMES:
                 category = LEGACY_PLUGIN_NAMES[category]
             if category not in CATEGORY_NAMES:
@@ -134,26 +144,28 @@
                 self.has_warnings = True
                 continue
             self.logger.debug(f"Discovered {plugin_id}")
             self.candidates.append(
                 PluginCandidate(
                     name=name,
                     description=description,
+                    friendly_name=friendly_name,
                     plugin_id=plugin_id,
                     category=category,
                     compiler=compiler,
                     source_dir=source_dir,
                     module_name=module_name,
                 )
             )
         return self.candidates
 
-    def load_plugins(self, candidates: List[PluginCandidate]) -> None:
+    def load_plugins(self, candidates: List[PluginCandidate]) -> List[PluginInfo]:
         """Load selected candidate plugins."""
         plugins_root = Path(__file__).parent.parent
+        new_plugins = []
 
         for candidate in candidates:
             name = candidate.name
             module_name = candidate.module_name
             source_dir = candidate.source_dir
             py_file_location = source_dir / f"{module_name}.py"
             plugin_id = candidate.plugin_id
@@ -215,35 +227,40 @@
                 self.logger.exception(f"{plugin_id} threw an exception while creating the instance")
                 self.has_warnings = True
                 continue
             self.logger.debug(f"Loaded {plugin_id}")
             info = PluginInfo(
                 name=name,
                 description=candidate.description,
+                friendly_name=candidate.friendly_name,
                 plugin_id=candidate.plugin_id,
                 category=candidate.category,
                 compiler=candidate.compiler,
                 source_dir=source_dir,
+                py_file_location=py_file_location,
                 module_name=module_name,
                 module_object=module_object,
                 plugin_object=plugin_object,
             )
             self.plugins.append(info)
+            new_plugins.append(info)
 
         self._plugins_by_category = {category: [] for category in CATEGORY_NAMES}
         for plugin_info in self.plugins:
             self._plugins_by_category[plugin_info.category].append(plugin_info)
 
         if self.has_warnings:
             self.logger.warning("Some plugins failed to load. Please review the above warning messages.")
             # TODO remove following messages and delay in v8.3.1
             self.logger.warning("You may need to update some plugins (from plugins.getnikola.com) or to fix their .plugin files.")
             self.logger.warning("Waiting 2 seconds before continuing.")
             time.sleep(2)
 
+        return new_plugins
+
     def get_plugins_of_category(self, category: str) -> List[PluginInfo]:
         """Get loaded plugins of a given category."""
         return self._plugins_by_category.get(category, [])
 
     def get_plugin_by_name(self, name: str, category: Optional[str] = None) -> Optional[PluginInfo]:
         """Get a loaded plugin by name and optionally by category. Returns None if no such plugin is loaded."""
         for p in self.plugins:
```

### Comparing `Nikola-8.3.0/nikola/plugins/basic_import.py` & `Nikola-8.3.1/nikola/plugins/basic_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import csv
 import datetime
 import os
 from urllib.parse import urlparse
 
 from lxml import etree, html
 from mako.template import Template
-from pkg_resources import resource_filename
 
 from nikola import utils
 
 links = {}
 
 
 class ImportMixin(object):
@@ -94,15 +93,15 @@
         if not os.path.exists(self.output_folder):
             os.system('nikola init -q ' + self.output_folder)
         else:
             self.import_into_existing_site = True
             utils.LOGGER.warning('The folder {0} already exists - assuming that this is a '
                                  'already existing Nikola site.'.format(self.output_folder))
 
-        filename = resource_filename('nikola', 'conf.py.in')
+        filename = utils.pkg_resources_path('nikola', 'conf.py.in')
         # The 'strict_undefined=True' will give the missing symbol name if any,
         # (ex: NameError: 'THEME' is not defined )
         # for other errors from mako/runtime.py, you can add format_extensions=True ,
         # then more info will be writen to *somefile* (most probably conf.py)
         conf_template = Template(filename=filename, strict_undefined=True)
 
         return conf_template
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/__init__.py` & `Nikola-8.3.1/nikola/plugins/command/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/auto/__init__.py` & `Nikola-8.3.1/nikola/plugins/command/auto/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,44 +33,43 @@
 import re
 import stat
 import subprocess
 import sys
 import typing
 import urllib.parse
 import webbrowser
+from pathlib import Path
 
 import blinker
-import pkg_resources
 
 from nikola.plugin_categories import Command
-from nikola.utils import dns_sd, req_missing, get_theme_path, makedirs
+from nikola.utils import dns_sd, req_missing, get_theme_path, makedirs, pkg_resources_path
 
 try:
     import aiohttp
     from aiohttp import web
     from aiohttp.web_urldispatcher import StaticResource
     from aiohttp.web_exceptions import HTTPNotFound, HTTPForbidden, HTTPMovedPermanently
     from aiohttp.web_response import Response
     from aiohttp.web_fileresponse import FileResponse
 except ImportError:
     aiohttp = web = None
     StaticResource = HTTPNotFound = HTTPForbidden = Response = FileResponse = object
 
 try:
     from watchdog.observers import Observer
+    from watchdog.observers.polling import PollingObserver
 except ImportError:
     Observer = None
+    PollingObserver = None
 
 LRJS_PATH = os.path.join(os.path.dirname(__file__), 'livereload.js')
 REBUILDING_REFRESH_DELAY = 0.35
 IDLE_REFRESH_DELAY = 0.05
 
-if sys.platform == 'win32':
-    asyncio.set_event_loop(asyncio.ProactorEventLoop())
-
 
 def base_path_from_siteuri(siteuri: str) -> str:
     """Extract the path part from a URI such as site['SITE_URL'].
 
     The path never ends with a "/". (If only "/" is intended, it is empty.)
     """
     path = urllib.parse.urlsplit(siteuri).path
@@ -158,14 +157,24 @@
         {
             'name': 'backend',
             'long': 'backend',
             'default': 'dbm',
             'type': str,
             'help': "Database backend ('dbm', 'json', 'sqlite3')",
             'section': 'Arguments passed to `nikola build`'
+        },
+        {
+            # We might be able to improve on this
+            # if and when https://github.com/gorakhargosh/watchdog/issues/365
+            # is ever fixed.
+            'name': 'poll',
+            'long': 'poll',
+            'default': False,
+            'type': bool,
+            'help': 'Use polling to notice changes behind symbolic links. This may reduce performance.'
         }
     ]
 
     def _execute(self, options, args):
         """Start the watcher."""
         self.sockets = []
         self.rebuild_queue = asyncio.Queue()
@@ -219,15 +228,15 @@
             watched.add(item)
         for item in self.site.config['IMAGE_FOLDERS']:
             watched.add(item)
         for item in self.site._plugin_places:
             watched.add(item)
         watched |= self.site.registered_auto_watched_folders
         # Nikola itself (useful for developers)
-        watched.add(pkg_resources.resource_filename('nikola', ''))
+        watched.add(pkg_resources_path('nikola', ''))
 
         out_folder = self.site.config['OUTPUT_FOLDER']
         if not os.path.exists(out_folder):
             makedirs(out_folder)
 
         if options and options.get('browser'):
             browser = True
@@ -255,15 +264,15 @@
 
         if self.has_server:
             loop.run_until_complete(self.set_up_server(host, port, base_path, out_folder))
 
         # Run an initial build so we are up-to-date. The server is running, but we are not watching yet.
         loop.run_until_complete(self.run_initial_rebuild())
 
-        self.wd_observer = Observer()
+        self.wd_observer = Observer() if not options['poll'] else PollingObserver()
         # Watch output folders and trigger reloads
         if self.has_server:
             self.wd_observer.schedule(NikolaEventHandler(self.reload_page, loop), out_folder, recursive=True)
 
         # Watch input folders and trigger rebuilds
         for p in watched:
             if os.path.exists(p):
@@ -271,35 +280,26 @@
 
         # Watch config file (a bit of a hack, but we need a directory)
         _conf_fn = os.path.abspath(self.site.configuration_filename or 'conf.py')
         _conf_dn = os.path.dirname(_conf_fn)
         self.wd_observer.schedule(ConfigEventHandler(_conf_fn, self.queue_rebuild, loop), _conf_dn, recursive=False)
         self.wd_observer.start()
 
-        win_sleeper = None
-        # https://bugs.python.org/issue23057 (fixed in Python 3.8)
-        if sys.platform == 'win32' and sys.version_info < (3, 8):
-            win_sleeper = asyncio.ensure_future(windows_ctrlc_workaround())
-
         if not self.has_server:
             self.logger.info("Watching for changes...")
             # Run the event loop forever (no server mode).
             try:
                 # Run rebuild queue
                 loop.run_until_complete(self.run_rebuild_queue())
-
                 loop.run_forever()
             except KeyboardInterrupt:
                 pass
             finally:
-                if win_sleeper:
-                    win_sleeper.cancel()
                 self.wd_observer.stop()
                 self.wd_observer.join()
-            loop.close()
             return
 
         if options['ipv6'] or '::' in host:
             server_url = "http://[{0}]:{1}/".format(host, port)
         else:
             server_url = "http://{0}:{1}/".format(host, port)
         self.logger.info("Serving on {0} ...".format(server_url))
@@ -322,24 +322,25 @@
 
             self.dns_sd = dns_sd(port, (options['ipv6'] or '::' in host))
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         finally:
             self.logger.info("Server is shutting down.")
-            if win_sleeper:
-                win_sleeper.cancel()
             if self.dns_sd:
                 self.dns_sd.Reset()
             rebuild_queue_fut.cancel()
             reload_queue_fut.cancel()
+
+            # Not sure why this isn't done by the web_runner.cleanup() code:
+            loop.run_until_complete(self.remove_websockets(None))
+
             loop.run_until_complete(self.web_runner.cleanup())
             self.wd_observer.stop()
             self.wd_observer.join()
-        loop.close()
 
     async def set_up_server(self, host: str, port: int, base_path: str, out_folder: str) -> None:
         """Set up aiohttp server and start it."""
         webapp = web.Application()
         webapp.router.add_get('/livereload.js', self.serve_livereload_js)
         webapp.router.add_get('/robots.txt', self.serve_robots_txt)
         webapp.router.add_route('*', '/livereload', self.websocket_handler)
@@ -478,15 +479,15 @@
                 self.logger.warning("Received unknown message: {0}".format(msg))
 
         self.sockets.remove(ws)
         self.logger.debug("WebSocket connection closed: {0}".format(ws))
 
         return ws
 
-    async def remove_websockets(self, app) -> None:
+    async def remove_websockets(self, _app) -> None:
         """Remove all websockets."""
         for ws in self.sockets:
             await ws.close()
         self.sockets.clear()
 
     async def send_to_websockets(self, message: dict) -> None:
         """Send a message to all open WebSockets."""
@@ -508,21 +509,14 @@
                 else:
                     raise
 
         for ws in to_delete:
             self.sockets.remove(ws)
 
 
-async def windows_ctrlc_workaround() -> None:
-    """Work around bpo-23057."""
-    # https://bugs.python.org/issue23057
-    while True:
-        await asyncio.sleep(1)
-
-
 class IndexHtmlStaticResource(StaticResource):
     """A StaticResource implementation that serves /index.html in directory roots."""
 
     modify_html = True
     snippet = "</head>"
 
     def __init__(self, modify_html=True, snippet="</head>", *args, **kwargs):
@@ -535,16 +529,21 @@
         """Handle incoming requests (pass to handle_file)."""
         filename = request.match_info['filename']
         return await self.handle_file(request, filename)
 
     async def handle_file(self, request: 'web.Request', filename: str, from_index=None) -> 'web.Response':
         """Handle file requests."""
         try:
-            filepath = self._directory.joinpath(filename).resolve()
-            if not self._follow_symlinks:
+            unresolved_path = self._directory.joinpath(filename)
+            if self._follow_symlinks:
+                normalized_path = Path(os.path.normpath(unresolved_path))
+                normalized_path.relative_to(self._directory)
+                filepath = normalized_path.resolve()
+            else:
+                filepath = unresolved_path.resolve()
                 filepath.relative_to(self._directory)
         except (ValueError, FileNotFoundError) as error:
             # relatively safe
             raise HTTPNotFound() from error
         except Exception as error:
             # perm error or other kind!
             request.app.logger.exception(error)
@@ -617,9 +616,9 @@
     def __init__(self, configuration_filename, function, loop):
         """Initialize the handler."""
         super().__init__(function, loop)
         self.configuration_filename = configuration_filename
 
     def dispatch(self, event):
         """Handle file events if they concern the configuration file."""
-        if event._src_path == self.configuration_filename:
+        if event.src_path == self.configuration_filename:
             super().dispatch(event)
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/auto/livereload.js` & `Nikola-8.3.1/nikola/plugins/command/auto/livereload.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/check.py` & `Nikola-8.3.1/nikola/plugins/command/check.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/console.py` & `Nikola-8.3.1/nikola/plugins/command/console.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/default_config.py` & `Nikola-8.3.1/nikola/plugins/command/default_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Show the default configuration."""
 
 import sys
 
-import nikola.plugins.command.init
 from nikola.plugin_categories import Command
 from nikola.utils import get_logger
 
 
 LOGGER = get_logger('default_config')
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/deploy.py` & `Nikola-8.3.1/nikola/plugins/command/deploy.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/github_deploy.py` & `Nikola-8.3.1/nikola/plugins/command/github_deploy.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/import_wordpress.py` & `Nikola-8.3.1/nikola/plugins/command/import_wordpress.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import sys
 from collections import defaultdict
 from urllib.parse import urlparse, unquote
 
 import requests
 from lxml import etree
 
-from nikola.plugin_categories import Command
+from nikola.plugin_categories import Command, CompilerExtension
 from nikola import utils, hierarchy_utils
 from nikola.nikola import DEFAULT_TRANSLATIONS_PATTERN
 from nikola.utils import req_missing
 from nikola.plugins.basic_import import ImportMixin, links
 from nikola.plugins.command.init import (
     SAMPLE_CONF, prepare_config,
     format_default_translations_config,
@@ -64,34 +64,37 @@
 
 def install_plugin(site, plugin_name, output_dir=None, show_install_notes=False):
     """Install a Nikola plugin."""
     LOGGER.info("Installing plugin '{0}'".format(plugin_name))
     # Get hold of the 'plugin' plugin
     plugin_installer_info = site.plugin_manager.get_plugin_by_name('plugin', 'Command')
     if plugin_installer_info is None:
-        LOGGER.error('Internal error: cannot find the "plugin" plugin which is supposed to come with Nikola!')
+        LOGGER.error('Internal error: cannot find the "plugin" plugin which is supposed to come with Nikola - it might be disabled in conf.py')
         return False
-    if not plugin_installer_info.is_activated:
-        # Someone might have disabled the plugin in the `conf.py` used
-        site.plugin_manager.activatePluginByName(plugin_installer_info.name)
-        plugin_installer_info.plugin_object.set_site(site)
     plugin_installer = plugin_installer_info.plugin_object
     # Try to install the requested plugin
     options = {}
     for option in plugin_installer.cmd_options:
         options[option['name']] = option['default']
     options['install'] = plugin_name
     options['output_dir'] = output_dir
     options['show_install_notes'] = show_install_notes
     if plugin_installer.execute(options=options) > 0:
         return False
     # Let the plugin manager find newly installed plugins
-    site.plugin_manager.collectPlugins()
-    # Re-scan for compiler extensions
-    site.compiler_extensions = site._activate_plugins_of_category("CompilerExtension")
+    old_candidates = set(site.plugin_manager.candidates)
+    new_candidates = set(site.plugin_manager.locate_plugins())
+    missing_candidates = list(new_candidates - old_candidates)
+    new_plugins = site.plugin_manager.load_plugins(missing_candidates)
+
+    # Activate new plugins
+    for p in new_plugins:
+        site._activate_plugin(p)
+        if isinstance(p.plugin_object, CompilerExtension):
+            site.compiler_extensions.append(p)
     return True
 
 
 class CommandImportWordpress(Command, ImportMixin):
     """Import a WordPress dump."""
 
     name = "import_wordpress"
@@ -244,19 +247,25 @@
         else:
             LOGGER.error("Can't find markdown post compiler.")
 
     def _find_wordpress_compiler(self):
         """Find WordPress compiler plugin."""
         if self.wordpress_page_compiler is not None:
             return
+
         plugin_info = self.site.plugin_manager.get_plugin_by_name('wordpress', 'PageCompiler')
-        if plugin_info is not None:
-            if not plugin_info.is_activated:
-                self.site.plugin_manager.activatePluginByName(plugin_info.name)
-                plugin_info.plugin_object.set_site(self.site)
+        if plugin_info is None:
+            candidates = self.site.plugin_manager.locate_plugins()
+            wordpress_candidates = [c for c in candidates if c.name == "wordpress" and c.category == "PageCompiler"]
+            if wordpress_candidates:
+                new_plugins = self.site.plugin_manager.load_plugins(wordpress_candidates)
+                for p in new_plugins:
+                    self.site._activate_plugin(p)
+                    self.wordpress_page_compiler = p.plugin_object
+        else:
             self.wordpress_page_compiler = plugin_info.plugin_object
 
     def _read_options(self, options, args):
         """Read command-line options."""
         options['filename'] = args.pop(0)
 
         if args and ('output_folder' not in args or
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/init.py` & `Nikola-8.3.1/nikola/plugins/command/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,19 @@
 import textwrap
 import unidecode
 from urllib.parse import urlsplit, urlunsplit
 
 import dateutil.tz
 import dateutil.zoneinfo
 from mako.template import Template
-from pkg_resources import resource_filename
 
 import nikola
 from nikola.nikola import DEFAULT_INDEX_READ_MORE_LINK, DEFAULT_FEED_READ_MORE_LINK, LEGAL_VALUES
 from nikola.plugin_categories import Command
-from nikola.utils import ask, ask_yesno, get_logger, makedirs, load_messages
+from nikola.utils import ask, ask_yesno, get_logger, makedirs, load_messages, pkg_resources_path
 from nikola.packages.tzlocal import get_localzone
 
 
 LOGGER = get_logger('init')
 
 SAMPLE_CONF = {
     'BLOG_AUTHOR': "Your Name",
@@ -269,30 +268,30 @@
             'help': "Create a site filled with example data.",
         }
     ]
 
     @classmethod
     def copy_sample_site(cls, target):
         """Copy sample site data to target directory."""
-        src = resource_filename('nikola', os.path.join('data', 'samplesite'))
+        src = pkg_resources_path('nikola', os.path.join('data', 'samplesite'))
         shutil.copytree(src, target)
 
     @staticmethod
     def create_configuration(target):
         """Create configuration file."""
-        template_path = resource_filename('nikola', 'conf.py.in')
+        template_path = pkg_resources_path('nikola', 'conf.py.in')
         conf_template = Template(filename=template_path)
         conf_path = os.path.join(target, 'conf.py')
         with io.open(conf_path, 'w+', encoding='utf8') as fd:
             fd.write(conf_template.render(**prepare_config(SAMPLE_CONF)))
 
     @staticmethod
     def create_configuration_to_string():
         """Return configuration file as a string."""
-        template_path = resource_filename('nikola', 'conf.py.in')
+        template_path = pkg_resources_path('nikola', 'conf.py.in')
         conf_template = Template(filename=template_path)
         return conf_template.render(**prepare_config(SAMPLE_CONF))
 
     @classmethod
     def create_empty_site(cls, target):
         """Create an empty site with directories only."""
         for folder in ('files', 'galleries', 'images', 'listings', 'posts', 'pages'):
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/new_page.py` & `Nikola-8.3.1/nikola/plugins/command/new_page.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/new_post.py` & `Nikola-8.3.1/nikola/plugins/command/new_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,30 +516,26 @@
                 disabled_compilers.append([
                     name,
                     plugin.friendly_name or name,
                     (),
                     False
                 ])
 
-        for name, (_, _, pi) in self.site.disabled_compilers.items():
-            if pi.details.has_option('Nikola', 'Friendlyname'):
-                f_name = pi.details.get('Nikola', 'Friendlyname')
-            else:
-                f_name = name
-            if name in compilers_raw:
+        for plugin in self.site.disabled_compilers.values():
+            if plugin.name in compilers_raw:
                 unused_compilers.append([
-                    name,
-                    f_name,
-                    compilers_raw[name],
+                    plugin.name,
+                    plugin.friendly_name,
+                    compilers_raw[plugin.name],
                     False
                 ])
             else:
                 disabled_compilers.append([
-                    name,
-                    f_name,
+                    plugin.name,
+                    plugin.friendly_name,
                     (),
                     False
                 ])
 
         used_compilers.sort(key=operator.itemgetter(0))
         unused_compilers.sort(key=operator.itemgetter(0))
         disabled_compilers.sort(key=operator.itemgetter(0))
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/orphans.py` & `Nikola-8.3.1/nikola/plugins/command/orphans.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/plugin.py` & `Nikola-8.3.1/nikola/plugins/command/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Manage plugins."""
 
 import io
 import json.decoder
-import os
+import pathlib
 import sys
 import shutil
 import subprocess
-import time
+import typing
+
 import requests
 
 import pygments
 from pygments.lexers import PythonLexer
 from pygments.formatters import TerminalFormatter
 
 from nikola.plugin_categories import Command
@@ -48,16 +49,17 @@
 class CommandPlugin(Command):
     """Manage plugins."""
 
     json = None
     name = "plugin"
     doc_usage = "[-u url] [--user] [-i name] [-r name] [--upgrade] [-l] [--list-installed]"
     doc_purpose = "manage plugins"
-    output_dir = None
+    output_dir: pathlib.Path = None
     needs_config = False
+    never_upgrade = {'emoji'}  # plugin with the same name is shipped with Nikola
     cmd_options = [
         {
             'name': 'install',
             'short': 'i',
             'long': 'install',
             'type': str,
             'default': '',
@@ -129,24 +131,24 @@
             list_available,
             list_installed)].count(True)
         if command_count > 1 or command_count == 0:
             print(self.help())
             return 2
 
         if options.get('output_dir') is not None:
-            self.output_dir = options.get('output_dir')
+            self.output_dir = pathlib.Path(options.get('output_dir'))
         else:
             if not self.site.configured and not user_mode and install:
                 LOGGER.warning('No site found, assuming --user')
                 user_mode = True
 
             if user_mode:
-                self.output_dir = os.path.expanduser(os.path.join('~', '.nikola', 'plugins'))
+                self.output_dir = pathlib.Path.home() / ".nikola" / "plugins"
             else:
-                self.output_dir = 'plugins'
+                self.output_dir = pathlib.Path("plugins")
 
         if list_available:
             return self.list_available(url)
         elif list_installed:
             return self.list_installed()
         elif upgrade:
             return self.do_upgrade(url)
@@ -162,22 +164,15 @@
         print("------------------")
         for plugin in sorted(data.keys()):
             print(plugin)
         return 0
 
     def list_installed(self):
         """List installed plugins."""
-        plugins = []
-        for plugin in self.site.plugin_manager.getAllPlugins():
-            p = plugin.path
-            if os.path.isdir(p):
-                p = p + os.sep
-            else:
-                p = p + '.py'
-            plugins.append([plugin.name, p])
+        plugins = self.get_plugins()
 
         plugins.sort()
         print('Installed Plugins:')
         print('------------------')
         maxlength = max(len(i[0]) for i in plugins)
         if self.site.colorful:
             formatstring = '\x1b[1m{0:<{2}}\x1b[0m  at {1}'
@@ -192,163 +187,140 @@
             print('\n\nNo plugins are disabled.')
         return 0
 
     def do_upgrade(self, url):
         """Upgrade all installed plugins."""
         LOGGER.warning('This is not very smart, it just reinstalls some plugins and hopes for the best')
         data = self.get_json(url)
-        plugins = []
-        for plugin in self.site.plugin_manager.getAllPlugins():
-            p = plugin.path
-            if os.path.isdir(p):
-                p = p + os.sep
-            else:
-                p = p + '.py'
-            if plugin.name in data:
-                plugins.append([plugin.name, p])
-        print('Will upgrade {0} plugins: {1}'.format(len(plugins), ', '.join(n for n, _ in plugins)))
+        plugins = [(n, p) for n, p in self.get_plugins() if n in data and n not in self.never_upgrade]
+        LOGGER.info('Will upgrade {0} plugins: {1}'.format(len(plugins), ', '.join(n for n, _ in plugins)))
         for name, path in plugins:
-            print('Upgrading {0}'.format(name))
+            path: pathlib.Path
+            LOGGER.info('Upgrading {0}'.format(name))
             p = path
             while True:
-                tail, head = os.path.split(path)
+                tail, head = path.parent, path.name
                 if head == 'plugins':
                     self.output_dir = path
                     break
-                elif tail == '':
+                elif path == tail:
                     LOGGER.error("Can't find the plugins folder for path: {0}".format(p))
                     return 1
                 else:
                     path = tail
             self.do_install(url, name)
         return 0
 
     def do_install(self, url, name, show_install_notes=True):
         """Download and install a plugin."""
         data = self.get_json(url)
         if name in data:
             utils.makedirs(self.output_dir)
             url = data[name]
             LOGGER.info("Downloading '{0}'".format(url))
-            try:
-                zip_data = requests.get(url).content
-            except requests.exceptions.SSLError:
-                LOGGER.warning("SSL error, using http instead of https (press ^C to abort)")
-                time.sleep(1)
-                url = url.replace('https', 'http', 1)
-                zip_data = requests.get(url).content
+            zip_data = requests.get(url).content
 
             zip_file = io.BytesIO()
             zip_file.write(zip_data)
             LOGGER.info('Extracting: {0} into {1}/'.format(name, self.output_dir))
             utils.extract_all(zip_file, self.output_dir)
-            dest_path = os.path.join(self.output_dir, name)
+            dest_path = self.output_dir / name
         else:
             LOGGER.error("Can't find plugin " + name)
             return 1
 
-        reqpath = os.path.join(dest_path, 'requirements.txt')
-        if os.path.exists(reqpath):
+        requirements_path = dest_path / 'requirements.txt'
+        if requirements_path.exists():
             LOGGER.warning('This plugin has Python dependencies.')
             LOGGER.info('Installing dependencies with pip...')
             try:
-                subprocess.check_call((sys.executable, '-m', 'pip', 'install', '-r', reqpath))
+                subprocess.check_call((sys.executable, '-m', 'pip', 'install', '-r', str(requirements_path)))
             except subprocess.CalledProcessError:
                 LOGGER.error('Could not install the dependencies.')
                 print('Contents of the requirements.txt file:\n')
-                with io.open(reqpath, 'r', encoding='utf-8-sig') as fh:
-                    print(utils.indent(fh.read(), 4 * ' '))
-                print('You have to install those yourself or through a '
-                      'package manager.')
+                print(utils.indent(requirements_path.read_text(), 4 * ' '))
+                print('You have to install those yourself or through a package manager.')
             else:
                 LOGGER.info('Dependency installation succeeded.')
 
-        reqnpypath = os.path.join(dest_path, 'requirements-nonpy.txt')
-        if os.path.exists(reqnpypath):
-            LOGGER.warning('This plugin has third-party '
-                           'dependencies you need to install '
-                           'manually.')
+        requirements_nonpy_path = dest_path / 'requirements-nonpy.txt'
+        if requirements_nonpy_path.exists():
+            LOGGER.warning('This plugin has third-party dependencies you need to install manually.')
             print('Contents of the requirements-nonpy.txt file:\n')
-            with io.open(reqnpypath, 'r', encoding='utf-8-sig') as fh:
-                for l in fh.readlines():
-                    i, j = l.split('::')
-                    print(utils.indent(i.strip(), 4 * ' '))
-                    print(utils.indent(j.strip(), 8 * ' '))
-                    print()
+            for l in requirements_nonpy_path.read_text().strip().splitlines():
+                i, j = l.split('::')
+                print(utils.indent(i.strip(), 4 * ' '))
+                print(utils.indent(j.strip(), 8 * ' '))
+                print()
 
             print('You have to install those yourself or through a package '
                   'manager.')
 
-        req_plug_path = os.path.join(dest_path, 'requirements-plugins.txt')
-        if os.path.exists(req_plug_path):
+        requirements_plugins_path = dest_path / 'requirements-plugins.txt'
+        if requirements_plugins_path.exists():
             LOGGER.info('This plugin requires other Nikola plugins.')
             LOGGER.info('Installing plugins...')
             plugin_failure = False
             try:
-                with io.open(req_plug_path, 'r', encoding='utf-8-sig') as inf:
-                    for plugname in inf.readlines():
-                        plugin_failure = self.do_install(url, plugname.strip(), show_install_notes) != 0
+                for plugin_name in requirements_plugins_path.read_text().strip().splitlines():
+                    plugin_failure = self.do_install(url, plugin_name.strip(), show_install_notes) != 0
             except Exception:
                 plugin_failure = True
             if plugin_failure:
                 LOGGER.error('Could not install a plugin.')
                 print('Contents of the requirements-plugins.txt file:\n')
-                with io.open(req_plug_path, 'r', encoding='utf-8-sig') as fh:
-                    print(utils.indent(fh.read(), 4 * ' '))
+                print(utils.indent(requirements_plugins_path.read_text(), 4 * ' '))
                 print('You have to install those yourself manually.')
             else:
                 LOGGER.info('Dependency installation succeeded.')
 
-        confpypath = os.path.join(dest_path, 'conf.py.sample')
-        if os.path.exists(confpypath) and show_install_notes:
+        confpy_path = dest_path / 'conf.py.sample'
+        if confpy_path.exists() and show_install_notes:
             LOGGER.warning('This plugin has a sample config file.  Integrate it with yours in order to make this plugin work!')
             print('Contents of the conf.py.sample file:\n')
-            with io.open(confpypath, 'r', encoding='utf-8-sig') as fh:
-                if self.site.colorful:
-                    print(pygments.highlight(fh.read(), PythonLexer(), TerminalFormatter()))
-                else:
-                    print(fh.read())
+            if self.site.colorful:
+                print(pygments.highlight(confpy_path.read_text(), PythonLexer(), TerminalFormatter()))
+            else:
+                print(confpy_path.read_text())
         return 0
 
     def do_uninstall(self, name):
         """Uninstall a plugin."""
-        for plugin in self.site.plugin_manager.getAllPlugins():  # FIXME: this is repeated thrice
-            if name == plugin.name:  # Uninstall this one
-                p = plugin.path
-                if os.path.isdir(p):
-                    # Plugins that have a package in them need to delete parent
-                    # Issue #2356
-                    p = p + os.sep
-                    p = os.path.abspath(os.path.join(p, os.pardir))
-                else:
-                    p = os.path.dirname(p)
+        for found_name, path in self.get_plugins():
+            if name == found_name:  # Uninstall this one
+                to_delete = path.parent  # Delete parent of .py file or parent of package
                 LOGGER.warning('About to uninstall plugin: {0}'.format(name))
-                LOGGER.warning('This will delete {0}'.format(p))
+                LOGGER.warning('This will delete {0}'.format(to_delete))
                 sure = utils.ask_yesno('Are you sure?')
                 if sure:
-                    LOGGER.warning('Removing {0}'.format(p))
-                    shutil.rmtree(p)
+                    LOGGER.warning('Removing {0}'.format(to_delete))
+                    shutil.rmtree(to_delete)
                     return 0
                 return 1
         LOGGER.error('Unknown plugin: {0}'.format(name))
         return 1
 
     def get_json(self, url):
         """Download the JSON file with all plugins."""
         if self.json is None:
             try:
-                try:
-                    self.json = requests.get(url).json()
-                except requests.exceptions.SSLError:
-                    LOGGER.warning("SSL error, using http instead of https (press ^C to abort)")
-                    time.sleep(1)
-                    url = url.replace('https', 'http', 1)
-                    self.json = requests.get(url).json()
+                self.json = requests.get(url).json()
             except json.decoder.JSONDecodeError as e:
                 LOGGER.error("Failed to decode JSON data in response from server.")
                 LOGGER.error("JSON error encountered: " + str(e))
-                LOGGER.error("This issue might be caused by server-side issues, or by to unusual activity in your "
+                LOGGER.error("This issue might be caused by server-side issues, or by unusual activity in your "
                              "network (as determined by CloudFlare). Please visit https://plugins.getnikola.com/ in "
                              "a browser.")
                 sys.exit(2)
 
         return self.json
+
+    def get_plugins(self) -> typing.List[typing.Tuple[str, pathlib.Path]]:
+        """Get currently installed plugins in site."""
+        plugins = []
+        for plugin in self.site.plugin_manager.plugins:
+            if plugin.py_file_location.name == "__init__.py":
+                path = plugin.py_file_location.parent
+            else:
+                path = plugin.py_file_location
+            plugins.append((plugin.name, path))
+        return plugins
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/rst2html/__init__.py` & `Nikola-8.3.1/nikola/plugins/command/rst2html/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """Compile reStructuredText to HTML, using Nikola architecture."""
 
 
 import io
 import lxml.html
-from pkg_resources import resource_filename
 from mako.template import Template
 from nikola.plugin_categories import Command
+from nikola.utils import pkg_resources_path
 
 
 class CommandRst2Html(Command):
     """Compile reStructuredText to HTML, using Nikola architecture."""
 
     name = "rst2html"
     doc_usage = "infile"
@@ -49,19 +49,19 @@
             print("This command takes only one argument (input file name).")
             return 2
         source = args[0]
         with io.open(source, "r", encoding="utf-8-sig") as in_file:
             data = in_file.read()
             output, error_level, deps, shortcode_deps = compiler.compile_string(data, source, True)
 
-        rstcss_path = resource_filename('nikola', 'data/themes/base/assets/css/rst_base.css')
+        rstcss_path = pkg_resources_path('nikola', 'data/themes/base/assets/css/rst_base.css')
         with io.open(rstcss_path, "r", encoding="utf-8-sig") as fh:
             rstcss = fh.read()
 
-        template_path = resource_filename('nikola', 'plugins/command/rst2html/rst2html.tmpl')
+        template_path = pkg_resources_path('nikola', 'plugins/command/rst2html/rst2html.tmpl')
         template = Template(filename=template_path)
         template_output = template.render(rstcss=rstcss, output=output)
         parser = lxml.html.HTMLParser(remove_blank_text=True)
         doc = lxml.html.document_fromstring(template_output, parser)
         html = b'<!DOCTYPE html>\n' + lxml.html.tostring(doc, encoding='utf8', method='html', pretty_print=True)
         print(html.decode('utf-8'))
         if error_level < 3:
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/serve.py` & `Nikola-8.3.1/nikola/plugins/command/serve.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/status.py` & `Nikola-8.3.1/nikola/plugins/command/status.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/subtheme.py` & `Nikola-8.3.1/nikola/plugins/command/subtheme.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/command/theme.py` & `Nikola-8.3.1/nikola/plugins/command/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 import sys
 import time
 
 import requests
 import pygments
 from pygments.lexers import PythonLexer
 from pygments.formatters import TerminalFormatter
-from pkg_resources import resource_filename
 
 from nikola.plugin_categories import Command
 from nikola import utils
 
 LOGGER = utils.get_logger('theme')
 
 
@@ -283,15 +282,15 @@
         return 0
 
     def list_installed(self):
         """List all installed themes."""
         print("Installed Themes:")
         print("-----------------")
         themes = []
-        themes_dirs = self.site.themes_dirs + [resource_filename('nikola', os.path.join('data', 'themes'))]
+        themes_dirs = self.site.themes_dirs + [utils.pkg_resources_path('nikola', os.path.join('data', 'themes'))]
         for tdir in themes_dirs:
             if os.path.isdir(tdir):
                 themes += [(i, os.path.join(tdir, i)) for i in os.listdir(tdir)]
 
         for tname, tpath in sorted(set(themes)):
             if os.path.isdir(tpath):
                 print("{0} at {1}".format(tname, tpath))
```

### Comparing `Nikola-8.3.0/nikola/plugins/command/version.py` & `Nikola-8.3.1/nikola/plugins/command/version.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/__init__.py` & `Nikola-8.3.1/nikola/plugins/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/html.py` & `Nikola-8.3.1/nikola/plugins/compile/html.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/ipynb.py` & `Nikola-8.3.1/nikola/plugins/compile/ipynb.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/markdown/__init__.py` & `Nikola-8.3.1/nikola/plugins/compile/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_gist.py` & `Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_gist.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_nikola.py` & `Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_nikola.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/markdown/mdx_podcast.py` & `Nikola-8.3.1/nikola/plugins/compile/markdown/mdx_podcast.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/pandoc.py` & `Nikola-8.3.1/nikola/plugins/compile/pandoc.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/php.py` & `Nikola-8.3.1/nikola/plugins/compile/php.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/__init__.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/chart.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/chart.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/doc.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/doc.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/gist.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/gist.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/listing.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/listing.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/media.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/media.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/post_list.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/post_list.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/soundcloud.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/soundcloud.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/thumbnail.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/vimeo.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/vimeo.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/compile/rest/youtube.py` & `Nikola-8.3.1/nikola/plugins/compile/rest/youtube.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/misc/__init__.py` & `Nikola-8.3.1/nikola/plugins/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/misc/scan_posts.py` & `Nikola-8.3.1/nikola/plugins/misc/scan_posts.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/misc/taxonomies_classifier.py` & `Nikola-8.3.1/nikola/plugins/misc/taxonomies_classifier.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/chart.py` & `Nikola-8.3.1/nikola/plugins/shortcode/chart.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/__init__.py` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Activity.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Activity.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Flags.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Flags.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Food.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Food.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/LICENSE` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Nature.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Nature.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Objects.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Objects.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/People.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/People.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Symbols.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Symbols.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/emoji/data/Travel.json` & `Nikola-8.3.1/nikola/plugins/shortcode/emoji/data/Travel.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/gist.py` & `Nikola-8.3.1/nikola/plugins/shortcode/gist.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/listing.py` & `Nikola-8.3.1/nikola/plugins/shortcode/listing.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/post_list.py` & `Nikola-8.3.1/nikola/plugins/shortcode/post_list.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/shortcode/thumbnail.py` & `Nikola-8.3.1/nikola/plugins/shortcode/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/__init__.py` & `Nikola-8.3.1/nikola/plugins/task/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/archive.py` & `Nikola-8.3.1/nikola/plugins/task/archive.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/authors.py` & `Nikola-8.3.1/nikola/plugins/task/authors.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/bundles.py` & `Nikola-8.3.1/nikola/plugins/task/bundles.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/categories.py` & `Nikola-8.3.1/nikola/plugins/task/categories.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/copy_assets.py` & `Nikola-8.3.1/nikola/plugins/task/copy_assets.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/copy_files.py` & `Nikola-8.3.1/nikola/plugins/task/copy_files.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/galleries.py` & `Nikola-8.3.1/nikola/plugins/task/galleries.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/gzip.py` & `Nikola-8.3.1/nikola/plugins/task/gzip.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/indexes.py` & `Nikola-8.3.1/nikola/plugins/task/indexes.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/listings.py` & `Nikola-8.3.1/nikola/plugins/task/listings.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/page_index.py` & `Nikola-8.3.1/nikola/plugins/task/page_index.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/pages.py` & `Nikola-8.3.1/nikola/plugins/task/pages.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/posts.py` & `Nikola-8.3.1/nikola/plugins/task/posts.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/redirect.py` & `Nikola-8.3.1/nikola/plugins/task/redirect.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/robots.py` & `Nikola-8.3.1/nikola/plugins/task/robots.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/scale_images.py` & `Nikola-8.3.1/nikola/plugins/task/scale_images.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/sitemap.py` & `Nikola-8.3.1/nikola/plugins/task/sitemap.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/sources.py` & `Nikola-8.3.1/nikola/plugins/task/sources.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/tags.py` & `Nikola-8.3.1/nikola/plugins/task/tags.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/task/taxonomies.py` & `Nikola-8.3.1/nikola/plugins/task/taxonomies.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/template/__init__.py` & `Nikola-8.3.1/nikola/plugins/template/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/template/jinja.py` & `Nikola-8.3.1/nikola/plugins/template/jinja.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/plugins/template/mako.py` & `Nikola-8.3.1/nikola/plugins/template/mako.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/post.py` & `Nikola-8.3.1/nikola/post.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/shortcodes.py` & `Nikola-8.3.1/nikola/shortcodes.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/state.py` & `Nikola-8.3.1/nikola/state.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/nikola/utils.py` & `Nikola-8.3.1/nikola/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,36 +45,40 @@
 from collections.abc import Callable, Iterable
 from html import unescape as html_unescape
 from importlib import reload as _reload
 from unicodedata import normalize as unicodenormalize
 from urllib.parse import quote as urlquote
 from urllib.parse import unquote as urlunquote
 from urllib.parse import urlparse, urlunparse
-from zipfile import ZipFile as zipf
+from zipfile import ZipFile
 
 import babel.dates
 import dateutil.parser
 import dateutil.tz
 import pygments.formatters
 import pygments.formatters._mapping
 import PyRSS2Gen as rss
 from blinker import signal
 from doit import tools
 from doit.cmdparse import CmdParse
-from pkg_resources import resource_filename
 from nikola.packages.pygments_better_html import BetterHtmlFormatter
 from typing import List
 from unidecode import unidecode
 
 # Renames
 from nikola import DEBUG  # NOQA
 from .log import LOGGER, get_logger  # NOQA
 from .hierarchy_utils import TreeNode, clone_treenode, flatten_tree_structure, sort_classifications
 from .hierarchy_utils import join_hierarchical_category_path, parse_escaped_hierarchical_category_name
 
+if sys.version_info.minor <= 8:
+    from pkg_resources import resource_filename
+else:
+    from importlib import resources
+
 try:
     import toml
 except ImportError:
     toml = None
 
 try:
     from ruamel.yaml import YAML
@@ -573,24 +577,32 @@
     def __repr__(self):
         """Provide a representation of config_changed."""
         return "Change with config: {0}".format(json.dumps(self.config,
                                                            cls=CustomEncoder,
                                                            sort_keys=True))
 
 
+def pkg_resources_path(package, resource):
+    """Return path to a resource from the package with the given name."""
+    if sys.version_info.minor <= 8:
+        return resource_filename(package, resource)
+    else:
+        return str(resources.files(package).joinpath(resource))
+
+
 def get_theme_path_real(theme, themes_dirs):
     """Return the path where the given theme's files are located.
 
     Looks in ./themes and in the place where themes go when installed.
     """
     for themes_dir in themes_dirs:
         dir_name = os.path.join(themes_dir, theme)
         if os.path.isdir(dir_name):
             return dir_name
-    dir_name = resource_filename('nikola', os.path.join('data', 'themes', theme))
+    dir_name = pkg_resources_path('nikola', os.path.join('data', 'themes', theme))
     if os.path.isdir(dir_name):
         return dir_name
     raise Exception("Can't find theme '{0}'".format(theme))
 
 
 def get_theme_path(theme):
     """Return the theme's path, which equals the theme's name."""
@@ -900,28 +912,30 @@
     pass
 
 
 def extract_all(zipfile, path='themes'):
     """Extract all files from a zip file."""
     pwd = os.getcwd()
     makedirs(path)
-    os.chdir(path)
-    z = zipf(zipfile)
-    namelist = z.namelist()
-    for f in namelist:
-        if f.endswith('/') and '..' in f:
-            raise UnsafeZipException('The zip file contains ".." and is '
-                                     'not safe to expand.')
-    for f in namelist:
-        if f.endswith('/'):
-            makedirs(f)
-        else:
-            z.extract(f)
-    z.close()
-    os.chdir(pwd)
+    try:
+        os.chdir(path)
+        z = ZipFile(zipfile)
+        namelist = z.namelist()
+        for f in namelist:
+            if f.endswith('/') and '..' in f:
+                raise UnsafeZipException('The zip file contains ".." and is '
+                                         'not safe to expand.')
+        for f in namelist:
+            if f.endswith('/'):
+                makedirs(f)
+            else:
+                z.extract(f)
+        z.close()
+    finally:
+        os.chdir(pwd)
 
 
 def to_datetime(value, tzinfo=None):
     """Convert string to datetime."""
     try:
         if type(value) is datetime.date:
             # type() instead of isinstance() is expected here, since we don’t
```

### Comparing `Nikola-8.3.0/nikola/winutils.py` & `Nikola-8.3.1/nikola/winutils.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/.package-lock.json` & `Nikola-8.3.1/npm_assets/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/LICENSE` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/README.md` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.css` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.js` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.css` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.js` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/dist/baguetteBox.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/package.json` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/src/baguetteBox.js` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/src/baguetteBox.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/baguettebox.js/src/baguetteBox.scss` & `Nikola-8.3.1/npm_assets/node_modules/baguettebox.js/src/baguetteBox.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/LICENSE` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/README.md` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/alert.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/alert.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/alert.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/alert.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/button.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/button.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/button.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/button.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/carousel.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/carousel.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/carousel.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/carousel.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/collapse.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/collapse.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/collapse.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/collapse.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/dropdown.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/dropdown.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/dropdown.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/dropdown.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/index.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/index.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/modal.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/modal.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/modal.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/modal.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/popover.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/popover.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/popover.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/popover.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/scrollspy.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tab.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tab.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tab.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tab.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/toast.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/toast.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/toast.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/toast.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tooltip.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tooltip.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/tooltip.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/tooltip.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/util.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/util.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/dist/util.js.map` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/dist/util.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/alert.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/button.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/carousel.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/collapse.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/dropdown.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/modal.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/popover.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/scrollspy.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tab.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/toast.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tools/sanitizer.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tools/sanitizer.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/tooltip.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/js/src/util.js` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/js/src/util.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/package.json` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_alert.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_badge.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_breadcrumb.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_button-group.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_buttons.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_card.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_carousel.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_close.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_code.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_code.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_custom-forms.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_dropdown.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_forms.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_forms.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_functions.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_grid.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_images.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_input-group.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_input-group.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_list-group.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_mixins.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_modal.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_nav.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_navbar.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_pagination.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_popover.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_print.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_print.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_progress.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_reboot.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_root.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_spinners.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_tables.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_toasts.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_tooltip.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_type.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_utilities.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/_variables.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/bootstrap-grid.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/bootstrap.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_background-variant.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_background-variant.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_border-radius.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_box-shadow.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_box-shadow.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_breakpoints.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_buttons.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_caret.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_deprecate.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_forms.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_gradients.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_grid-framework.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_grid.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_hover.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_image.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_screen-reader.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_table-row.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/mixins/_transition.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_borders.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_display.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_embed.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_flex.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_spacing.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/utilities/_text.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/bootstrap/scss/vendor/_rfs.scss` & `Nikola-8.3.1/npm_assets/node_modules/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/Gruntfile.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/MIT and GPL2 licenses.md` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/MIT and GPL2 licenses.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.min.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/dist/html5shiv.min.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/dist/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/readme.md` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/readme.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/src/html5shiv-printshiv.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/src/html5shiv-printshiv.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/src/html5shiv.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/src/html5shiv.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/iframed-tests.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/iframed-tests.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/data/paramtracer.swf` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/data/paramtracer.swf`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/highcharts/area-basic.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/highcharts/area-basic.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/highcharts/highcharts.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/highcharts/highcharts.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/html5shiv.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/html5shiv.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/iframe.1.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/iframe.1.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/index.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/index.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testinit.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testinit.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testrunner.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testrunner.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testsuite.css` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/data/testsuite.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/index.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/index.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/core.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/core.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/manipulation.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/manipulation.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/traversing.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/jquery-1.7.1/unit/traversing.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/mixed-test.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/mixed-test.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/object-test.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/object-test.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/perf.1.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/perf.1.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/perf.2.html` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/perf.2.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/qunit/qunit.css` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/qunit/qunit.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/html5shiv/test/unit/tests.js` & `Nikola-8.3.1/npm_assets/node_modules/html5shiv/test/unit/tests.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/AUTHORS.txt` & `Nikola-8.3.1/npm_assets/node_modules/jquery/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/LICENSE.txt` & `Nikola-8.3.1/npm_assets/node_modules/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/README.md` & `Nikola-8.3.1/npm_assets/node_modules/jquery/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.min.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.min.map` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.min.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/dist/jquery.slim.min.map` & `Nikola-8.3.1/npm_assets/node_modules/jquery/dist/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/LICENSE.txt` & `Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.map` & `Nikola-8.3.1/npm_assets/node_modules/jquery/external/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/package.json` & `Nikola-8.3.1/npm_assets/node_modules/jquery/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/jsonp.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/load.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/script.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax/xhr.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/ajax.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/attr.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/classes.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/prop.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/support.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/attributes/val.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/callbacks.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/DOMEval.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/DOMEval.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/access.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/camelCase.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/camelCase.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/init.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/isAttached.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/isAttached.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/parseHTML.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/parseXML.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/parseXML.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/ready-no-deferred.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/ready-no-deferred.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/ready.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core/support.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core/support.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/core.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/addGetHookIf.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/adjustCSS.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/adjustCSS.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/curCSS.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/finalPropName.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/finalPropName.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/showHide.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/showHide.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/support.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css/var/isHiddenWithinTree.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css/var/isHiddenWithinTree.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/css.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/data/Data.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/data.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/deferred/exceptionHook.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/deferred/exceptionHook.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/deferred.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated/event.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated/event.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/deprecated.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/deprecated.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/dimensions.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects/Tween.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/effects.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/focusin.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/focusin.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/event/trigger.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/event/trigger.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/event.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/exports/amd.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/exports/global.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/jquery.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/_evalUrl.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/_evalUrl.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/buildFragment.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/buildFragment.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/getAll.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/getAll.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/support.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation/wrapMap.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation/wrapMap.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/manipulation.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/offset.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/queue/delay.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/queue.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/selector-native.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/serialize.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing/findFilter.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/traversing.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/var/isFunction.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/var/isFunction.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/jquery/src/wrap.js` & `Nikola-8.3.1/npm_assets/node_modules/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/LICENSE` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/README.md` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/demo.html` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/demo.html`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/dist/justified-layout.js` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/dist/justified-layout.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/dist/justified-layout.min.js` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/dist/justified-layout.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/lib/index.js` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/lib/index.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/lib/row.js` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/lib/row.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/justified-layout/package.json` & `Nikola-8.3.1/npm_assets/node_modules/justified-layout/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/LICENSE` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/README.md` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/dist/livereload.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/dist/livereload.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/connector.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/connector.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/customevents.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/customevents.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/less.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/less.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/livereload.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/livereload.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/options.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/options.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/protocol.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/protocol.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/reloader.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/reloader.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/startup.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/startup.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/lib/timer.js` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/lib/timer.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/livereload-js/package.json` & `Nikola-8.3.1/npm_assets/node_modules/livereload-js/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/LICENSE.md` & `Nikola-8.3.1/npm_assets/node_modules/luxon/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/README.md` & `Nikola-8.3.1/npm_assets/node_modules/luxon/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/amd/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/amd/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/amd/luxon.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/amd/luxon.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/cjs-browser/luxon.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/es6/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/es6/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/es6/luxon.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/es6/luxon.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.min.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/global/luxon.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/global/luxon.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/node/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/node/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/build/node/luxon.js.map` & `Nikola-8.3.1/npm_assets/node_modules/luxon/build/node/luxon.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/package.json` & `Nikola-8.3.1/npm_assets/node_modules/luxon/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/datetime.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/datetime.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/duration.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/duration.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/errors.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/errors.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/conversions.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/conversions.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/diff.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/diff.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/digits.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/digits.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/english.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/english.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/formats.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/formats.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/formatter.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/formatter.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/locale.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/locale.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/regexParser.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/regexParser.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/tokenParser.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/tokenParser.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/util.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/util.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/impl/zoneUtil.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/impl/zoneUtil.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/info.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/info.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/interval.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/interval.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/luxon.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/luxon.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/settings.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/settings.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/zone.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/zone.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/IANAZone.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/IANAZone.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/fixedOffsetZone.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/fixedOffsetZone.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/invalidZone.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/invalidZone.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/luxon/src/zones/systemZone.js` & `Nikola-8.3.1/npm_assets/node_modules/luxon/src/zones/systemZone.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/LICENSE` & `Nikola-8.3.1/npm_assets/node_modules/merge/LICENSE`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/README.md` & `Nikola-8.3.1/npm_assets/node_modules/merge/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/bower.json` & `Nikola-8.3.1/npm_assets/node_modules/merge/bower.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/merge.js` & `Nikola-8.3.1/npm_assets/node_modules/merge/merge.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/merge.min.js` & `Nikola-8.3.1/npm_assets/node_modules/merge/merge.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/merge/package.json` & `Nikola-8.3.1/npm_assets/node_modules/merge/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/README.md` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper-utils.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/esm/popper.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/esm/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper-utils.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper-utils.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/popper.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper-utils.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js.flow` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js.flow`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.min.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/dist/umd/popper.min.js.map` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/dist/umd/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/index.d.ts` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/index.d.ts`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/index.js.flow` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/index.js.flow`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/package.json` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/package.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/index.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/index.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/defaults.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/defaults.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/destroy.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/destroy.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/placements.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/placements.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/methods/update.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/methods/update.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/applyStyle.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/applyStyle.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/arrow.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/arrow.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/computeStyle.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/computeStyle.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/flip.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/flip.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/hide.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/hide.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/index.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/index.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/inner.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/inner.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/keepTogether.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/keepTogether.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/offset.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/offset.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/preventOverflow.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/preventOverflow.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/modifiers/shift.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/modifiers/shift.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/clockwise.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/clockwise.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/computeAutoPlacement.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/computeAutoPlacement.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/debounce.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/debounce.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/findCommonOffsetParent.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/findCommonOffsetParent.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/findIndex.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/findIndex.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBordersSize.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBordersSize.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBoundaries.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBoundaries.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getBoundingClientRect.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getBoundingClientRect.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getFixedPositionOffsetParent.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getFixedPositionOffsetParent.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetParent.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetParent.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetRect.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetRect.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOffsetRectRelativeToArbitraryNode.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOffsetRectRelativeToArbitraryNode.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getOuterSizes.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getOuterSizes.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getPopperOffsets.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getPopperOffsets.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getReferenceOffsets.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getReferenceOffsets.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getRoundedOffsets.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getRoundedOffsets.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getScroll.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getScroll.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getScrollParent.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getScrollParent.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getSupportedPropertyName.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getSupportedPropertyName.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getViewportOffsetRectRelativeToArtbitraryNode.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getViewportOffsetRectRelativeToArtbitraryNode.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/getWindowSizes.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/getWindowSizes.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/includeScroll.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/includeScroll.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/index.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/index.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isFixed.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isFixed.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/isModifierRequired.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/isModifierRequired.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/removeEventListeners.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/removeEventListeners.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/runModifiers.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/runModifiers.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setAttributes.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setAttributes.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setStyles.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setStyles.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/node_modules/popper.js/src/utils/setupEventListeners.js` & `Nikola-8.3.1/npm_assets/node_modules/popper.js/src/utils/setupEventListeners.js`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/npm_assets/package-lock.json` & `Nikola-8.3.1/npm_assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/baseline.sh` & `Nikola-8.3.1/scripts/baseline.sh`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/capty` & `Nikola-8.3.1/scripts/capty`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/debug_rebuilds/README.md` & `Nikola-8.3.1/scripts/debug_rebuilds/README.md`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/debug_rebuilds/step1_build_and_dumpdb.py` & `Nikola-8.3.1/scripts/debug_rebuilds/step1_build_and_dumpdb.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/debug_rebuilds/step2_analyze_py_files.py` & `Nikola-8.3.1/scripts/debug_rebuilds/step2_analyze_py_files.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/document_path_handlers.py` & `Nikola-8.3.1/scripts/document_path_handlers.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/getpyver.py` & `Nikola-8.3.1/scripts/getpyver.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/github-release.py` & `Nikola-8.3.1/scripts/github-release.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/import_po.py` & `Nikola-8.3.1/scripts/import_po.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/jinjify.py` & `Nikola-8.3.1/scripts/jinjify.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/langmatrix.py` & `Nikola-8.3.1/scripts/langmatrix.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/langstatus.py` & `Nikola-8.3.1/scripts/langstatus.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/release` & `Nikola-8.3.1/scripts/release`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,18 @@
 
 status 'This is the last chance to quit.  Hit ^C now if you want to.'
 read bailout
 
 cleanup
 
 ./setup.py sdist bdist_wheel || exit $?
-gpg --detach-sign -a dist/Nikola-$version.tar.gz.asc dist/Nikola-$version.tar.gz
-gpg --detach-sign -a dist/Nikola-$version*.whl.asc dist/Nikola-$version*.whl
+
+gpg --detach-sign -a dist/Nikola-$version.tar.gz
+gpg --detach-sign -a dist/Nikola-$version*.whl
+
 twine upload dist/Nikola-$version.tar.gz dist/Nikola-$version*.whl || exit $?
 
 cleanup
 
 git add -A --ignore-errors . || exit $?
 
 git commit -S -am "Version $version" || exit $?
```

### Comparing `Nikola-8.3.0/scripts/theme_snapshot` & `Nikola-8.3.1/scripts/theme_snapshot`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/scripts/update-npm-assets.sh` & `Nikola-8.3.1/scripts/update-npm-assets.sh`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/setup.py` & `Nikola-8.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 with open('requirements-tests.txt', 'r') as fh:
     extras['tests'] = [l.strip() for l in fh][1:]
 
 # ########## platform specific stuff #############
 if sys.version_info[0] == 2:
     raise Exception('Python 2 is not supported')
-elif sys.version_info[0] == 3 and sys.version_info[1] < 7:
-    raise Exception('Python 3 version < 3.7 is not supported')
+elif sys.version_info[0] == 3 and sys.version_info[1] < 8:
+    raise Exception('Python 3 version < 3.8 is not supported')
 
 ##################################################
 
 # Provided as an attribute, so you can append to these instead
 # of replicating them:
 standard_exclude = ('*.pyc', '*$py.class', '*~', '.*', '*.bak')
 standard_exclude_directories = ('.*', 'CVS', '_darcs', './build',
@@ -102,15 +102,15 @@
 class nikola_build_py(build_py):
     def run(self):
         expands_symlinks_for_windows()
         build_py.run(self)
 
 
 setup(name='Nikola',
-      version='8.3.0',
+      version='8.3.1',
       description='A modular, fast, simple, static website and blog generator',
       long_description=long_description,
       author='Roberto Alsina and others',
       author_email='ralsina@netmanagers.com.ar',
       url='https://getnikola.com/',
       packages=find_packages(exclude=('tests', 'tests.*')),
       license='MIT',
@@ -124,27 +124,26 @@
                    'Operating System :: MacOS',
                    'Operating System :: MacOS :: MacOS X',
                    'Operating System :: Microsoft :: Windows',
                    'Operating System :: OS Independent',
                    'Operating System :: POSIX',
                    'Operating System :: Unix',
                    'Programming Language :: Python',
-                   'Programming Language :: Python :: 3.7',
                    'Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
                    'Programming Language :: Python :: 3.11',
                    'Programming Language :: Python :: 3.12',
                    'Topic :: Internet',
                    'Topic :: Internet :: WWW/HTTP',
                    'Topic :: Text Processing :: Markup'],
       install_requires=dependencies,
       extras_require=extras,
       include_package_data=True,
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       cmdclass={'install': nikola_install, 'build_py': nikola_build_py},
       data_files=[
               ('share/doc/nikola', [
                'docs/manual.rst',
                'docs/theming.rst',
                'docs/extending.rst']),
               ('share/man/man1', ['docs/man/nikola.1.gz']),
```

### Comparing `Nikola-8.3.0/tests/data/1-nolinks.rst` & `Nikola-8.3.1/tests/data/1-nolinks.rst`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/metadata_extractors/f-ipynb-1-compiler.ipynb` & `Nikola-8.3.1/tests/data/metadata_extractors/f-ipynb-1-compiler.ipynb`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/plugin_manager/broken.py` & `Nikola-8.3.1/tests/data/plugin_manager/broken.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/plugin_manager/one.py` & `Nikola-8.3.1/tests/data/plugin_manager/one.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/plugin_manager/second/two/__init__.py` & `Nikola-8.3.1/tests/data/plugin_manager/second/two/__init__.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/rss-2_0.xsd` & `Nikola-8.3.1/tests/data/rss-2_0.xsd`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/test_config/conf.py` & `Nikola-8.3.1/tests/data/test_config/conf.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/translated_titles/conf.py` & `Nikola-8.3.1/tests/data/translated_titles/conf.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/wordpress_import/wordpress_export_example.xml` & `Nikola-8.3.1/tests/data/wordpress_import/wordpress_export_example.xml`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/wordpress_import/wordpress_qtranslate_item_modernized.xml` & `Nikola-8.3.1/tests/data/wordpress_import/wordpress_qtranslate_item_modernized.xml`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/wordpress_import/wordpress_qtranslate_item_raw_export.xml` & `Nikola-8.3.1/tests/data/wordpress_import/wordpress_qtranslate_item_raw_export.xml`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/data/wordpress_import/wordpress_unicode_export.xml` & `Nikola-8.3.1/tests/data/wordpress_import/wordpress_unicode_export.xml`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/helper.py` & `Nikola-8.3.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/conftest.py` & `Nikola-8.3.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/helper.py` & `Nikola-8.3.1/tests/integration/helper.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_archive_full.py` & `Nikola-8.3.1/tests/integration/test_archive_full.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_archive_per_day.py` & `Nikola-8.3.1/tests/integration/test_archive_per_day.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_archive_per_month.py` & `Nikola-8.3.1/tests/integration/test_archive_per_month.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_building_in_subdir.py` & `Nikola-8.3.1/tests/integration/test_building_in_subdir.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_category_destpath.py` & `Nikola-8.3.1/tests/integration/test_category_destpath.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_check_absolute_subfolder.py` & `Nikola-8.3.1/tests/integration/test_check_absolute_subfolder.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_check_failure.py` & `Nikola-8.3.1/tests/integration/test_check_failure.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_check_full_path_subfolder.py` & `Nikola-8.3.1/tests/integration/test_check_full_path_subfolder.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_demo_build.py` & `Nikola-8.3.1/tests/integration/test_demo_build.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_dev_server.py` & `Nikola-8.3.1/tests/integration/test_dev_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import nikola.plugins.command.auto as auto
 from nikola.utils import get_logger
 import pytest
 import pathlib
 import requests
 import socket
-import sys
 from typing import Optional, Tuple, Any, Dict
 
 from ..helper import FakeSite
 
 SERVER_ADDRESS = "localhost"
 TEST_MAX_DURATION = 10  # Watchdog: Give up the test if it did not succeed during this time span.
 
@@ -34,14 +33,15 @@
         return port
     finally:
         s.close()
 
 
 class MyFakeSite(FakeSite):
     def __init__(self, config: Dict[str, Any], configuration_filename="conf.py"):
+        super(MyFakeSite, self).__init__()
         self.configured = True
         self.debug = True
         self.THEMES = []
         self._plugin_places = []
         self.registered_auto_watched_folders = set()
         self.config = config
         self.configuration_filename = configuration_filename
@@ -56,31 +56,32 @@
     options = {
         "browser": False,
         "ipv6": False,
         "address": SERVER_ADDRESS,
         "port": find_unused_port(),
         "db-file": "/dev/null",
         "backend": "No backend",
-        "no-server": False
+        "no-server": False,
+        "poll": False
     }
 
     # We start an event loop, run the test in an executor,
     # and wait for the event loop to terminate.
     # These variables help to transport the test result to
     # the main thread outside the event loop:
     test_was_successful = False
     test_problem_description = "Async test setup apparently broken"
     test_inner_error: Optional[BaseException] = None
-    loop_for_this_test = None
+    loop = None
 
     async def grab_loop_and_run_test() -> None:
-        nonlocal test_problem_description, loop_for_this_test
+        nonlocal test_problem_description, loop
 
-        loop_for_this_test = asyncio.get_running_loop()
-        watchdog_handle = loop_for_this_test.call_later(TEST_MAX_DURATION, lambda: loop_for_this_test.stop())
+        loop = asyncio.get_running_loop()
+        watchdog_handle = loop.call_later(TEST_MAX_DURATION, loop.stop)
         test_problem_description = f"Test did not complete within {TEST_MAX_DURATION} seconds."
 
         def run_test() -> None:
             nonlocal test_was_successful, test_problem_description, test_inner_error
             try:
                 with requests.Session() as session:
                     server_root_uri = f"http://{options['address']}:{options['port']}"
@@ -109,63 +110,35 @@
                 test_was_successful = False
                 test_problem_description = "(see exception)"
             finally:
                 if test_was_successful:
                     LOGGER.info("Test completed successfully.")
                 else:
                     LOGGER.error("Test failed: %s", test_problem_description)
-                loop_for_this_test.call_soon_threadsafe(lambda: watchdog_handle.cancel())
+                loop.call_soon_threadsafe(watchdog_handle.cancel)
+                # Simulate Ctrl+C:
+                loop.call_soon_threadsafe(lambda: loop.call_later(0.01, loop.stop))
 
-                # We give the outer grab_loop_and_run_test a chance to complete
-                # before burning the bridge:
-                loop_for_this_test.call_soon_threadsafe(lambda: loop_for_this_test.call_later(0.05, lambda: loop_for_this_test.stop()))
-
-        await loop_for_this_test.run_in_executor(None, run_test)
+        await loop.run_in_executor(None, run_test)
 
     # We defeat the nikola site building functionality, so this does not actually get called.
     # But the code setting up site building wants a command list:
     command_auto.nikola_cmd = ["echo"]
 
     # Defeat the site building functionality, and instead insert the test:
     command_auto.run_initial_rebuild = grab_loop_and_run_test
 
-    try:
-        # Start the development server
-        # which under the hood runs our test when trying to build the site:
-        command_auto.execute(options=options)
-
-        # Verify the test succeeded:
-        if test_inner_error is not None:
-            raise test_inner_error
-        assert test_was_successful, test_problem_description
-    finally:
-        # Nikola is written with the assumption that it can
-        # create the event loop at will without ever cleaning it up.
-        # As this tests runs several times in succession,
-        # that assumption becomes a problem.
-        LOGGER.info("Cleaning up loop.")
-        # Loop cleanup:
-        assert loop_for_this_test is not None
-        assert not loop_for_this_test.is_running()
-        loop_for_this_test.close()
-        asyncio.set_event_loop(None)
-        # We would like to leave it at that,
-        # but doing so causes the next test to fail.
-        #
-        # We did not find asyncio - API to reset the loop
-        # to "back to square one, as if just freshly started".
-        #
-        # The following code does not feel right, it's a kludge,
-        # but it apparently works for now:
-        if sys.platform == 'win32':
-            # For this case, the auto module has special code
-            # (at module load time! 😟) which we reluctantly reproduce here:
-            asyncio.set_event_loop(asyncio.ProactorEventLoop())
-        else:
-            asyncio.set_event_loop(asyncio.new_event_loop())
+    # Start the development server
+    # which under the hood runs our test when trying to build the site:
+    command_auto.execute(options=options)
+
+    # Verify the test succeeded:
+    if test_inner_error is not None:
+        raise test_inner_error
+    assert test_was_successful, test_problem_description
 
 
 @pytest.fixture(scope="module",
                 params=["https://example.org",
                         "https://example.org:1234/blog",
                         "https://example.org:3456/blog/",
                         "http://example.org/deep/down/a/rabbit/hole"
@@ -180,15 +153,15 @@
         "FILES_FOLDERS": [],
         "GALLERY_FOLDERS": [],
         "LISTINGS_FOLDERS": [],
         "IMAGE_FOLDERS": [],
         "SITE_URL": request.param,
         "OUTPUT_FOLDER": OUTPUT_FOLDER.as_posix(),
     }
-    return (MyFakeSite(config), auto.base_path_from_siteuri(request.param))
+    return MyFakeSite(config), auto.base_path_from_siteuri(request.param)
 
 
 @pytest.fixture(scope="module")
 def expected_text():
     """Read the index.html file from the fixture folder and return most of it.
 
     For life reload, the server will fiddle with HTML <head>,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Nikola-8.3.0/tests/integration/test_empty_build.py` & `Nikola-8.3.1/tests/integration/test_empty_build.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_future_post.py` & `Nikola-8.3.1/tests/integration/test_future_post.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_page_index_normal_urls.py` & `Nikola-8.3.1/tests/integration/test_page_index_normal_urls.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_page_index_pretty_urls.py` & `Nikola-8.3.1/tests/integration/test_page_index_pretty_urls.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_redirection.py` & `Nikola-8.3.1/tests/integration/test_redirection.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_relative_links.py` & `Nikola-8.3.1/tests/integration/test_relative_links.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_relative_links_with_pages_in_root.py` & `Nikola-8.3.1/tests/integration/test_relative_links_with_pages_in_root.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_repeated_posts_setting.py` & `Nikola-8.3.1/tests/integration/test_repeated_posts_setting.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_translated_content.py` & `Nikola-8.3.1/tests/integration/test_translated_content.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_translated_content_secondary_language.py` & `Nikola-8.3.1/tests/integration/test_translated_content_secondary_language.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_translation_patterns.py` & `Nikola-8.3.1/tests/integration/test_translation_patterns.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/integration/test_wordpress_import.py` & `Nikola-8.3.1/tests/integration/test_wordpress_import.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_command_import_wordpress.py` & `Nikola-8.3.1/tests/test_command_import_wordpress.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,16 @@
     import_command.tag_saniziting_strategy = "first"
     import_command.separate_qtranslate_content = False
     import_command.translations_pattern = "{path}.{lang}.{ext}"
 
     import_command.context = import_command.populate_context(channel)
 
     # Ensuring clean results
-    # assert not import_command.url_map
-    assert not module.links
     import_command.url_map = {}
+    module.links.clear()
 
     write_metadata = mock.MagicMock()
     write_content = mock.MagicMock()
     write_attachments_info = mock.MagicMock()
     download_mock = mock.MagicMock()
 
     with mock.patch(
```

### Comparing `Nikola-8.3.0/tests/test_command_import_wordpress_translation.py` & `Nikola-8.3.1/tests/test_command_import_wordpress_translation.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_command_init.py` & `Nikola-8.3.1/tests/test_command_init.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_compile_markdown.py` & `Nikola-8.3.1/tests/test_compile_markdown.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_config.py` & `Nikola-8.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_locale.py` & `Nikola-8.3.1/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_metadata_extractors.py` & `Nikola-8.3.1/tests/test_metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_path_handlers.py` & `Nikola-8.3.1/tests/test_path_handlers.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_plugin_manager.py` & `Nikola-8.3.1/tests/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_rss_feeds.py` & `Nikola-8.3.1/tests/test_rss_feeds.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_rst_compiler.py` & `Nikola-8.3.1/tests/test_rst_compiler.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_scheduling.py` & `Nikola-8.3.1/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_shortcodes.py` & `Nikola-8.3.1/tests/test_shortcodes.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_slugify.py` & `Nikola-8.3.1/tests/test_slugify.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_task_scale_images.py` & `Nikola-8.3.1/tests/test_task_scale_images.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_template_shortcodes.py` & `Nikola-8.3.1/tests/test_template_shortcodes.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_test_helper.py` & `Nikola-8.3.1/tests/test_test_helper.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/tests/test_utils.py` & `Nikola-8.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/af.po` & `Nikola-8.3.1/translations/nikola.messages/af.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ar.po` & `Nikola-8.3.1/translations/nikola.messages/ar.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/az.po` & `Nikola-8.3.1/translations/nikola.messages/az.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/bg.po` & `Nikola-8.3.1/translations/nikola.messages/bg.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/bn.po` & `Nikola-8.3.1/translations/nikola.messages/bn.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/br.po` & `Nikola-8.3.1/translations/nikola.messages/br.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/bs.po` & `Nikola-8.3.1/translations/nikola.messages/bs.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ca.po` & `Nikola-8.3.1/translations/nikola.messages/ca.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/cs.po` & `Nikola-8.3.1/translations/nikola.messages/cs.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/da.po` & `Nikola-8.3.1/translations/nikola.messages/da.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/de.po` & `Nikola-8.3.1/translations/nikola.messages/de.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/el.po` & `Nikola-8.3.1/translations/nikola.messages/el.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/en.po` & `Nikola-8.3.1/translations/nikola.messages/en.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/eo.po` & `Nikola-8.3.1/translations/nikola.messages/eo.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/es.po` & `Nikola-8.3.1/translations/nikola.messages/es.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/et.po` & `Nikola-8.3.1/translations/nikola.messages/et.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/eu.po` & `Nikola-8.3.1/translations/nikola.messages/eu.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/fa.po` & `Nikola-8.3.1/translations/nikola.messages/fa.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/fi.po` & `Nikola-8.3.1/translations/nikola.messages/fi.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/fr.po` & `Nikola-8.3.1/translations/nikola.messages/fr.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/fur.po` & `Nikola-8.3.1/translations/nikola.messages/fur.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/gl.po` & `Nikola-8.3.1/translations/nikola.messages/gl.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/he.po` & `Nikola-8.3.1/translations/nikola.messages/he.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/hi.po` & `Nikola-8.3.1/translations/nikola.messages/hi.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/hr.po` & `Nikola-8.3.1/translations/nikola.messages/hr.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/hu.po` & `Nikola-8.3.1/translations/nikola.messages/hu.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ia.po` & `Nikola-8.3.1/translations/nikola.messages/ia.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/id.po` & `Nikola-8.3.1/translations/nikola.messages/id.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/it.po` & `Nikola-8.3.1/translations/nikola.messages/it.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ja.po` & `Nikola-8.3.1/translations/nikola.messages/ja.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ko.po` & `Nikola-8.3.1/translations/nikola.messages/ko.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/lt.po` & `Nikola-8.3.1/translations/nikola.messages/lt.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/mi.po` & `Nikola-8.3.1/translations/nikola.messages/mi.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ml.po` & `Nikola-8.3.1/translations/nikola.messages/ml.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/mr.po` & `Nikola-8.3.1/translations/nikola.messages/mr.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/nb.po` & `Nikola-8.3.1/translations/nikola.messages/nb.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/nl.po` & `Nikola-8.3.1/translations/nikola.messages/nl.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/oc.po` & `Nikola-8.3.1/translations/nikola.messages/oc.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/pa.po` & `Nikola-8.3.1/translations/nikola.messages/pa.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/pl.po` & `Nikola-8.3.1/translations/nikola.messages/pl.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/pt.po` & `Nikola-8.3.1/translations/nikola.messages/pt.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/pt_BR.po` & `Nikola-8.3.1/translations/nikola.messages/pt_BR.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ru.po` & `Nikola-8.3.1/translations/nikola.messages/ru.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sk.po` & `Nikola-8.3.1/translations/nikola.messages/sk.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sl.po` & `Nikola-8.3.1/translations/nikola.messages/sl.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sq.po` & `Nikola-8.3.1/translations/nikola.messages/sq.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sr.po` & `Nikola-8.3.1/translations/nikola.messages/sr.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sr@latin.po` & `Nikola-8.3.1/translations/nikola.messages/sr@latin.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/sv.po` & `Nikola-8.3.1/translations/nikola.messages/sv.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ta.po` & `Nikola-8.3.1/translations/nikola.messages/ta.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/te.po` & `Nikola-8.3.1/translations/nikola.messages/te.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/th.po` & `Nikola-8.3.1/translations/nikola.messages/th.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/tr.po` & `Nikola-8.3.1/translations/nikola.messages/tr.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/tzm.po` & `Nikola-8.3.1/translations/nikola.messages/tzm.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/uk.po` & `Nikola-8.3.1/translations/nikola.messages/uk.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/ur.po` & `Nikola-8.3.1/translations/nikola.messages/ur.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/vi.po` & `Nikola-8.3.1/translations/nikola.messages/vi.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/zh_CN.po` & `Nikola-8.3.1/translations/nikola.messages/zh_CN.po`

 * *Files identical despite different names*

### Comparing `Nikola-8.3.0/translations/nikola.messages/zh_TW.po` & `Nikola-8.3.1/translations/nikola.messages/zh_TW.po`

 * *Files identical despite different names*

