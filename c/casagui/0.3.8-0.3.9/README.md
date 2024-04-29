# Comparing `tmp/casagui-0.3.8.tar.gz` & `tmp/casagui-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casagui-0.3.8.tar", last modified: Thu Dec  7 18:49:16 2023, max compression
+gzip compressed data, was "casagui-0.3.9.tar", last modified: Tue Dec 19 17:09:37 2023, max compression
```

## Comparing `casagui-0.3.8.tar` & `casagui-0.3.9.tar`

### file list

```diff
@@ -1,89 +1,90 @@
--rw-r--r--   0        0        0    26526 2023-12-07 18:48:40.933924 casagui-0.3.8/LICENSE
--rw-r--r--   0        0        0    26371 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/LICENSE.rst
--rw-r--r--   0        0        0      604 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/README.rst
--rw-r--r--   0        0        0     3422 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/add-chan.png
--rw-r--r--   0        0        0     2549 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/add-chan.svg
--rw-r--r--   0        0        0    13271 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/add-cube.png
--rw-r--r--   0        0        0     7106 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/add-cube.svg
--rw-r--r--   0        0        0    21946 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/drag.png
--rw-r--r--   0        0        0     3458 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/drag.svg
--rw-r--r--   0        0        0     2674 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/sub-chan.png
--rw-r--r--   0        0        0     2563 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/sub-chan.svg
--rw-r--r--   0        0        0    10011 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/sub-cube.png
--rw-r--r--   0        0        0     6391 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__icons__/sub-cube.svg
--rw-r--r--   0        0        0     1755 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__init__.py
--rw-r--r--   0        0        0    25145 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__js__/casaguijs.min.js
--rw-r--r--   0        0        0    86352 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/__js__/casalib.min.js
--rw-r--r--   0        0        0     1701 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/apps/__init__.py
--rw-r--r--   0        0        0    83296 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/apps/_interactiveclean.py
--rw-r--r--   0        0        0     7340 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/apps/_makemask.py
--rwxr-xr-x   0        0        0    10823 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/apps/_plotants.py
--rw-r--r--   0        0        0      185 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/apps/_plotbandpass.py
--rw-r--r--   0        0        0     1371 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/bokeh/__init__.py
--rw-r--r--   0        0        0     1346 2023-12-07 18:48:40.957924 casagui-0.3.8/casagui/bokeh/components/__init__.py
--rw-r--r--   0        0        0    20579 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/components/_svg_icon.py
--rw-r--r--   0        0        0     1380 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/format/__init__.py
--rw-r--r--   0        0        0     1827 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/format/_wcs_ticks.py
--rw-r--r--   0        0        0       57 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/models/__init__.py
--rw-r--r--   0        0        0     1385 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/models/_tip.py
--rw-r--r--   0        0        0     1577 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/models/_tip_button.py
--rw-r--r--   0        0        0     1525 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/sources/__init__.py
--rw-r--r--   0        0        0    13676 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/sources/_data_pipe.py
--rw-r--r--   0        0        0     3476 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/sources/_image_data_source.py
--rw-r--r--   0        0        0    23324 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/sources/_image_pipe.py
--rw-r--r--   0        0        0     2200 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/sources/_spectra_data_source.py
--rw-r--r--   0        0        0     1628 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/state/__init__.py
--rw-r--r--   0        0        0     5932 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/state/_initialize.py
--rw-r--r--   0        0        0     2407 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/state/_javascript.py
--rw-r--r--   0        0        0     2453 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/state/_palette.py
--rw-r--r--   0        0        0     1761 2023-12-07 18:48:40.961924 casagui-0.3.8/casagui/bokeh/state/_session.py
--rw-r--r--   0        0        0   799179 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/bokeh-2.4.1.min.js
--rw-r--r--   0        0        0   185643 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/bokeh-gl-2.4.1.min.js
--rw-r--r--   0        0        0   292438 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/bokeh-tables-2.4.1.min.js
--rw-r--r--   0        0        0   251390 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/bokeh-widgets-2.4.1.min.js
--rw-r--r--   0        0        0     8432 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.4.0-b2.4.min.js
--rw-r--r--   0        0        0     8587 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.5.0-b2.4.min.js
--rw-r--r--   0        0        0     8981 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.6.0-b2.4.min.js
--rw-r--r--   0        0        0      384 2023-12-07 18:48:40.965924 casagui-0.3.8/casagui/bokeh/state/js/casalib-v0.0.1.min.js
--rw-r--r--   0        0        0     1383 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/bokeh/tools/__init__.py
--rw-r--r--   0        0        0     2208 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/bokeh/tools/_cbreset_tool.py
--rw-r--r--   0        0        0     2845 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/bokeh/tools/_drag_tool.py
--rw-r--r--   0        0        0     1442 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/bokeh/utils/__init__.py
--rw-r--r--   0        0        0     3607 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/bokeh/utils/_axes_labels.py
--rw-r--r--   0        0        0        0 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/private/compatibility/casatasks/private/imagerhelpers/__init__.py
--rw-r--r--   0        0        0    30402 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/private/compatibility/casatasks/private/imagerhelpers/_gclean.py
--rw-r--r--   0        0        0     1349 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/toolbox/__init__.py
--rw-r--r--   0        0        0   170905 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/toolbox/_cube.py
--rw-r--r--   0        0        0     3410 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_ResourceManager.py
--rw-r--r--   0        0        0    22777 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/__init__.py
--rw-r--r--   0        0        0     3262 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_conversion.py
--rw-r--r--   0        0        0      276 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_docenum.py
--rw-r--r--   0        0        0      626 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_image.py
--rw-r--r--   0        0        0     2348 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_logging.py
--rw-r--r--   0        0        0     1669 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_regions.py
--rw-r--r--   0        0        0     2347 2023-12-07 18:48:40.969924 casagui-0.3.8/casagui/utils/_static.py
--rw-r--r--   0        0        0      745 2023-12-07 18:48:41.093923 casagui-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5960 2023-12-07 18:48:41.093923 casagui-0.3.8/readme.rst
--rw-r--r--   0        0        0     7378 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/alma-many-chan/alma-many-chan.py
--rw-r--r--   0        0        0     1761 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/basic-websockets-demo/client.html
--rw-r--r--   0        0        0      251 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/basic-websockets-demo/client.py
--rw-r--r--   0        0        0      437 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/basic-websockets-demo/server.py
--rw-r--r--   0        0        0      940 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra-done-stats.py
--rw-r--r--   0        0        0      878 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra-done.py
--rw-r--r--   0        0        0      649 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra.py
--rw-r--r--   0        0        0      605 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/cubemask-demo/image-slider.py
--rw-r--r--   0        0        0      560 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/cubemask-demo/image.py
--rw-r--r--   0        0        0     3334 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/m100_interactive.py
--rw-r--r--   0        0        0     2427 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/mask0-iclean.py
--rw-r--r--   0        0        0     1043 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/run-gclean.py
--rw-r--r--   0        0        0     2213 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/run-iclean-obj.py
--rw-r--r--   0        0        0     1738 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/run-iclean.py
--rw-r--r--   0        0        0     5852 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-demo/vla-sim-jet-iclean.py
--rw-r--r--   0        0        0     2006 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/iclean-first-look/run-fl.py
--rw-r--r--   0        0        0     2288 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/large-cube/run-largecube.py
--rw-r--r--   0        0        0      956 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/makemask-demo/run-makemask.py
--rw-r--r--   0        0        0      508 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/svg-test.py
--rw-r--r--   0        0        0     2395 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/uranus-demo/uranus-iclean.py
--rw-r--r--   0        0        0     3575 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/websocket-reconnect/client.html
--rw-r--r--   0        0        0      641 2023-12-07 18:48:41.097923 casagui-0.3.8/tests/manual/websocket-reconnect/server.py
--rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 casagui-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-12-19 17:09:06.507243 casagui-0.3.9/LICENSE
+-rw-r--r--   0        0        0    26371 2023-12-19 17:09:06.527243 casagui-0.3.9/casagui/LICENSE.rst
+-rw-r--r--   0        0        0      604 2023-12-19 17:09:06.527243 casagui-0.3.9/casagui/README.rst
+-rw-r--r--   0        0        0     3422 2023-12-19 17:09:06.527243 casagui-0.3.9/casagui/__icons__/add-chan.png
+-rw-r--r--   0        0        0     2549 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/add-chan.svg
+-rw-r--r--   0        0        0    13271 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/add-cube.png
+-rw-r--r--   0        0        0     7106 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/add-cube.svg
+-rw-r--r--   0        0        0    21946 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/drag.png
+-rw-r--r--   0        0        0     3458 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/drag.svg
+-rw-r--r--   0        0        0     2674 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/sub-chan.png
+-rw-r--r--   0        0        0     2563 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/sub-chan.svg
+-rw-r--r--   0        0        0    10011 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/sub-cube.png
+-rw-r--r--   0        0        0     6391 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__icons__/sub-cube.svg
+-rw-r--r--   0        0        0     1755 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__init__.py
+-rw-r--r--   0        0        0    25145 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__js__/casaguijs.min.js
+-rw-r--r--   0        0        0    86352 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/__js__/casalib.min.js
+-rw-r--r--   0        0        0     1701 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/apps/__init__.py
+-rw-r--r--   0        0        0    83749 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/apps/_interactiveclean.py
+-rw-r--r--   0        0        0     7340 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/apps/_makemask.py
+-rwxr-xr-x   0        0        0    10823 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/apps/_plotants.py
+-rw-r--r--   0        0        0      185 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/apps/_plotbandpass.py
+-rw-r--r--   0        0        0     1371 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/__init__.py
+-rw-r--r--   0        0        0     1346 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/components/__init__.py
+-rw-r--r--   0        0        0    20579 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/components/_svg_icon.py
+-rw-r--r--   0        0        0     1380 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/format/__init__.py
+-rw-r--r--   0        0        0     1827 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/format/_wcs_ticks.py
+-rw-r--r--   0        0        0       57 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/models/__init__.py
+-rw-r--r--   0        0        0     1385 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/models/_tip.py
+-rw-r--r--   0        0        0     1577 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/models/_tip_button.py
+-rw-r--r--   0        0        0     1525 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/sources/__init__.py
+-rw-r--r--   0        0        0    13676 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/sources/_data_pipe.py
+-rw-r--r--   0        0        0     3476 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/sources/_image_data_source.py
+-rw-r--r--   0        0        0    23324 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/sources/_image_pipe.py
+-rw-r--r--   0        0        0     2200 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/sources/_spectra_data_source.py
+-rw-r--r--   0        0        0     1628 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/state/__init__.py
+-rw-r--r--   0        0        0     5932 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/state/_initialize.py
+-rw-r--r--   0        0        0     2407 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/state/_javascript.py
+-rw-r--r--   0        0        0     2453 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/state/_palette.py
+-rw-r--r--   0        0        0     1761 2023-12-19 17:09:06.531243 casagui-0.3.9/casagui/bokeh/state/_session.py
+-rw-r--r--   0        0        0   799179 2023-12-19 17:09:06.535243 casagui-0.3.9/casagui/bokeh/state/js/bokeh-2.4.1.min.js
+-rw-r--r--   0        0        0   185643 2023-12-19 17:09:06.535243 casagui-0.3.9/casagui/bokeh/state/js/bokeh-gl-2.4.1.min.js
+-rw-r--r--   0        0        0   292438 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/bokeh-tables-2.4.1.min.js
+-rw-r--r--   0        0        0   251390 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/bokeh-widgets-2.4.1.min.js
+-rw-r--r--   0        0        0     8432 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.4.0-b2.4.min.js
+-rw-r--r--   0        0        0     8587 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.5.0-b2.4.min.js
+-rw-r--r--   0        0        0     8981 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.6.0-b2.4.min.js
+-rw-r--r--   0        0        0      384 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/state/js/casalib-v0.0.1.min.js
+-rw-r--r--   0        0        0     1383 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/tools/__init__.py
+-rw-r--r--   0        0        0     2208 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/tools/_cbreset_tool.py
+-rw-r--r--   0        0        0     2845 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/tools/_drag_tool.py
+-rw-r--r--   0        0        0     1442 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/utils/__init__.py
+-rw-r--r--   0        0        0     3607 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/bokeh/utils/_axes_labels.py
+-rw-r--r--   0        0        0        0 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/private/compatibility/casatasks/private/imagerhelpers/__init__.py
+-rw-r--r--   0        0        0    30402 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/private/compatibility/casatasks/private/imagerhelpers/_gclean.py
+-rw-r--r--   0        0        0     1349 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/toolbox/__init__.py
+-rw-r--r--   0        0        0   170905 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/toolbox/_cube.py
+-rw-r--r--   0        0        0     3410 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_ResourceManager.py
+-rw-r--r--   0        0        0    23129 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/__init__.py
+-rw-r--r--   0        0        0     3262 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_conversion.py
+-rw-r--r--   0        0        0      877 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_docenum.py
+-rw-r--r--   0        0        0     1919 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_image.py
+-rw-r--r--   0        0        0     2348 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_logging.py
+-rw-r--r--   0        0        0     1669 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_regions.py
+-rw-r--r--   0        0        0     2347 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_static.py
+-rw-r--r--   0        0        0     7336 2023-12-19 17:09:06.539243 casagui-0.3.9/casagui/utils/_tiles.py
+-rw-r--r--   0        0        0      745 2023-12-19 17:09:06.667243 casagui-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5960 2023-12-19 17:09:06.667243 casagui-0.3.9/readme.rst
+-rw-r--r--   0        0        0     7374 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/alma-many-chan/alma-many-chan.py
+-rw-r--r--   0        0        0     1761 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/basic-websockets-demo/client.html
+-rw-r--r--   0        0        0      251 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/basic-websockets-demo/client.py
+-rw-r--r--   0        0        0      437 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/basic-websockets-demo/server.py
+-rw-r--r--   0        0        0      940 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra-done-stats.py
+-rw-r--r--   0        0        0      878 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra-done.py
+-rw-r--r--   0        0        0      649 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra.py
+-rw-r--r--   0        0        0      605 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/cubemask-demo/image-slider.py
+-rw-r--r--   0        0        0      560 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/cubemask-demo/image.py
+-rw-r--r--   0        0        0     3334 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/m100_interactive.py
+-rw-r--r--   0        0        0     2427 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/mask0-iclean.py
+-rw-r--r--   0        0        0     1043 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/run-gclean.py
+-rw-r--r--   0        0        0     2213 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/run-iclean-obj.py
+-rw-r--r--   0        0        0     1738 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/run-iclean.py
+-rw-r--r--   0        0        0     5848 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-demo/vla-sim-jet-iclean.py
+-rw-r--r--   0        0        0     2006 2023-12-19 17:09:06.667243 casagui-0.3.9/tests/manual/iclean-first-look/run-fl.py
+-rw-r--r--   0        0        0     2288 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/large-cube/run-largecube.py
+-rw-r--r--   0        0        0      956 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/makemask-demo/run-makemask.py
+-rw-r--r--   0        0        0      508 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/svg-test.py
+-rw-r--r--   0        0        0     2395 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/uranus-demo/uranus-iclean.py
+-rw-r--r--   0        0        0     3575 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/websocket-reconnect/client.html
+-rw-r--r--   0        0        0      641 2023-12-19 17:09:06.671243 casagui-0.3.9/tests/manual/websocket-reconnect/server.py
+-rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 casagui-0.3.9/PKG-INFO
```

### Comparing `casagui-0.3.8/LICENSE` & `casagui-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/LICENSE.rst` & `casagui-0.3.9/casagui/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/README.rst` & `casagui-0.3.9/casagui/README.rst`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/add-chan.png` & `casagui-0.3.9/casagui/__icons__/add-chan.png`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/add-chan.svg` & `casagui-0.3.9/casagui/__icons__/add-chan.svg`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/add-cube.png` & `casagui-0.3.9/casagui/__icons__/add-cube.png`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/add-cube.svg` & `casagui-0.3.9/casagui/__icons__/add-cube.svg`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/drag.png` & `casagui-0.3.9/casagui/__icons__/drag.png`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/drag.svg` & `casagui-0.3.9/casagui/__icons__/drag.svg`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/sub-chan.png` & `casagui-0.3.9/casagui/__icons__/sub-chan.png`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/sub-chan.svg` & `casagui-0.3.9/casagui/__icons__/sub-chan.svg`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/sub-cube.png` & `casagui-0.3.9/casagui/__icons__/sub-cube.png`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__icons__/sub-cube.svg` & `casagui-0.3.9/casagui/__icons__/sub-cube.svg`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__init__.py` & `casagui-0.3.9/casagui/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__js__/casaguijs.min.js` & `casagui-0.3.9/casagui/__js__/casaguijs.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/__js__/casalib.min.js` & `casagui-0.3.9/casagui/__js__/casalib.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/apps/__init__.py` & `casagui-0.3.9/casagui/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/apps/_interactiveclean.py` & `casagui-0.3.9/casagui/apps/_interactiveclean.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from bokeh.plotting import ColumnDataSource, figure, show
 from bokeh.layouts import column, row, Spacer, layout
 from bokeh.io import reset_output as reset_bokeh_output, output_file, output_notebook
 from bokeh.models.dom import HTML
 
 from bokeh.models.ui.tooltips import Tooltip
 from ..bokeh.models import TipButton, Tip
-from ..utils import resource_manager, reset_resource_manager, is_notebook
+from ..utils import resource_manager, reset_resource_manager, is_notebook, is_intstr
 
 try:
     ## gclean version number needed for proper interactive clean behavior
     # pylint: disable=no-name-in-module
     from casatasks.private.imagerhelpers._gclean import _GCV004
     from casatasks.private.imagerhelpers._gclean import gclean as _gclean
     # pylint: enable=no-name-in-module
@@ -221,15 +221,15 @@
     def __init__( self, vis, imagename, usemask='user', mask='', initial_mask_pixel=False, field='', spw='', timerange='', uvrange='', antenna='', scan='', observation='', intent='',
                   datacolumn='corrected', nterms=int(2), imsize=[100], cell=[ ], phasecenter='', stokes='I', startmodel='', specmode='cube', reffreq='',
                   nchan=-1, start='', width='', veltype='radio', restfreq='', outframe='LSRK', interpolation='linear', perchanweightdensity=True, gridder='standard',
                   wprojplanes=int(1), mosweight=True, psterm=False, wbawp=True, usepointing=False, conjbeams=False, pointingoffsetsigdev=[  ], pblimit=0.2,
                   deconvolver='hogbom', niter=0, threshold='0.1Jy', nsigma=0.0, cycleniter=-1, cyclefactor=1.0, scales=[], restoringbeam='',
                   smallscalebias=0.0, pbcor=False, weighting='natural', robust=float(0.5), npixels=0, gain=float(0.1), sidelobethreshold=3.0, noisethreshold=5.0,
                   lownoisethreshold=1.5, negativethreshold=0.0, minbeamfrac=0.3, growiterations=75, dogrowprune=True, minpercentchange=-1.0,
-                  fastnoise=True, savemodel='none', parallel=False, nmajor=1, remote=False):
+                  fastnoise=True, savemodel='none', parallel=False, nmajor=-1, remote=False):
 
         if deconvolver == 'mtmfs':
             raise RuntimeError("deconvolver task does not support 'mtmf' deconvolver")
 
         ###
         ### Whether or not the Interactive Clean session is running remotely
         ###
@@ -308,15 +308,15 @@
                                perchanweightdensity=perchanweightdensity, gridder=gridder, wprojplanes=wprojplanes, mosweight=mosweight, psterm=psterm,
                                wbawp=wbawp, usepointing=usepointing, conjbeams=conjbeams, pointingoffsetsigdev=pointingoffsetsigdev, pblimit=pblimit,
                                deconvolver=deconvolver, smallscalebias=smallscalebias, niter=niter, threshold=threshold, nsigma=nsigma,
                                cycleniter=cycleniter, cyclefactor=cyclefactor, scales=scales, restoringbeam=restoringbeam, pbcor=pbcor,
                                weighting=weighting, robust=robust, npixels=npixels, gain=gain, sidelobethreshold=sidelobethreshold,
                                noisethreshold=noisethreshold, lownoisethreshold=lownoisethreshold, negativethreshold=negativethreshold,
                                minbeamfrac=minbeamfrac, growiterations=growiterations, dogrowprune=dogrowprune,
-                               minpercentchange=minpercentchange, fastnoise=fastnoise, savemodel=savemodel, parallel=parallel, nmajor=1,
+                               minpercentchange=minpercentchange, fastnoise=fastnoise, savemodel=savemodel, parallel=parallel, nmajor=nmajor,
                                usemask=self._usemask, mask=mask
                       )
         ###
         ### self._convergence_data['chan']: accumulated, pre-channel convergence information
         ###                                 used by ColumnDataSource
         ###
         self._status = { }
@@ -428,16 +428,19 @@
                                                //                          }
                                                //                        } )
                                                if ( clean_msg !== undefined && 'iterdone' in clean_msg ) {
                                                  const remaining = parseInt(niter.value) - parseInt(clean_msg['iterdone'])
                                                  niter.value = '' + (remaining < 0 ? 0 : remaining)
                                                }
                                                if ( clean_msg !== undefined && 'majordone' in clean_msg ) {
-                                                 const remaining = parseInt(nmajor.value) - parseInt(clean_msg['majordone'])
-                                                 nmajor.value = '' + (remaining < 0 ? 0 : remaining)
+                                                 const nm = parseInt(nmajor.value)
+                                                 if ( nm != -1 ) {
+                                                     const remaining = nm - parseInt(clean_msg['majordone'])
+                                                     nmajor.value = '' + (remaining < 0 ? 0 : remaining)
+                                                 } else nmajor.value = '' + nm          // nmajor == -1 implies do not consider nmajor in stop decision
                                                }
                                                img_src.refresh( (data) => { if ( 'stats' in data ) cube_obj.update_statistics( data.stats ) } )
 
                                                if ( clean_msg !== undefined && 'convergence' in clean_msg ) {
                                                    // save convergence information and update convergence using saved state
                                                    if ( clean_msg.convergence === null ) {
                                                        delete flux_src._convergence_data
@@ -661,16 +664,18 @@
         ###
         ### Python-side handler for events from the interactive clean control buttons
         ###
         async def clean_handler( msg, self=self ):
             if msg['action'] == 'next' or msg['action'] == 'finish':
 
                 if 'nmajor' in msg['value']:
-                    if msg['value']['nmajor'].isdigit( ):
-                        if int(msg['value']['nmajor']) <= 0:
+                    if is_intstr(msg['value']['nmajor']):
+                        nm = int(msg['value']['nmajor'])
+                        if nm == 0 or nm < -1:
+                            ### nm == -1 means do not consider nmajor as part of the stopping decision
                             return dict( result='no-action', stopcode=1, iterdone=0, majordone=0, status="major cycle limit is zero" )
                     else:
                         return dict( result='error', stopcode=1, iterdone=0, majordone=0, error="major cycle limit is not an integer" )
 
                 if 'mask' in msg['value']:
                     if 'breadcrumbs' in msg['value'] and msg['value']['breadcrumbs'] is not None and msg['value']['breadcrumbs'] != self._last_mask_breadcrumbs:
                         self._last_mask_breadcrumbs = msg['value']['breadcrumbs']
```

### Comparing `casagui-0.3.8/casagui/apps/_makemask.py` & `casagui-0.3.9/casagui/apps/_makemask.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/apps/_plotants.py` & `casagui-0.3.9/casagui/apps/_plotants.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/__init__.py` & `casagui-0.3.9/casagui/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/components/__init__.py` & `casagui-0.3.9/casagui/bokeh/components/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/components/_svg_icon.py` & `casagui-0.3.9/casagui/bokeh/components/_svg_icon.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/format/__init__.py` & `casagui-0.3.9/casagui/bokeh/format/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/format/_wcs_ticks.py` & `casagui-0.3.9/casagui/bokeh/format/_wcs_ticks.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/models/_tip.py` & `casagui-0.3.9/casagui/bokeh/models/_tip.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/models/_tip_button.py` & `casagui-0.3.9/casagui/bokeh/models/_tip_button.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/sources/__init__.py` & `casagui-0.3.9/casagui/bokeh/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/sources/_data_pipe.py` & `casagui-0.3.9/casagui/bokeh/sources/_data_pipe.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/sources/_image_data_source.py` & `casagui-0.3.9/casagui/bokeh/sources/_image_data_source.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/sources/_image_pipe.py` & `casagui-0.3.9/casagui/bokeh/sources/_image_pipe.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/sources/_spectra_data_source.py` & `casagui-0.3.9/casagui/bokeh/sources/_spectra_data_source.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/__init__.py` & `casagui-0.3.9/casagui/bokeh/state/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/_initialize.py` & `casagui-0.3.9/casagui/bokeh/state/_initialize.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/_javascript.py` & `casagui-0.3.9/casagui/bokeh/state/_javascript.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/_palette.py` & `casagui-0.3.9/casagui/bokeh/state/_palette.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/_session.py` & `casagui-0.3.9/casagui/bokeh/state/_session.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/bokeh-2.4.1.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/bokeh-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/bokeh-gl-2.4.1.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/bokeh-gl-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/bokeh-tables-2.4.1.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/bokeh-tables-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/bokeh-widgets-2.4.1.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/bokeh-widgets-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.4.0-b2.4.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.4.0-b2.4.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.5.0-b2.4.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.5.0-b2.4.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/state/js/casaguijs-v0.0.6.0-b2.4.min.js` & `casagui-0.3.9/casagui/bokeh/state/js/casaguijs-v0.0.6.0-b2.4.min.js`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/tools/__init__.py` & `casagui-0.3.9/casagui/bokeh/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/tools/_cbreset_tool.py` & `casagui-0.3.9/casagui/bokeh/tools/_cbreset_tool.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/tools/_drag_tool.py` & `casagui-0.3.9/casagui/bokeh/tools/_drag_tool.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/utils/__init__.py` & `casagui-0.3.9/casagui/bokeh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/bokeh/utils/_axes_labels.py` & `casagui-0.3.9/casagui/bokeh/utils/_axes_labels.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/private/compatibility/casatasks/private/imagerhelpers/_gclean.py` & `casagui-0.3.9/casagui/private/compatibility/casatasks/private/imagerhelpers/_gclean.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/toolbox/__init__.py` & `casagui-0.3.9/casagui/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/toolbox/_cube.py` & `casagui-0.3.9/casagui/toolbox/_cube.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/utils/_ResourceManager.py` & `casagui-0.3.9/casagui/utils/_ResourceManager.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/utils/__init__.py` & `casagui-0.3.9/casagui/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 logger = get_logger()
 
 from ._conversion import pack_arrays
 from ._conversion import strip_arrays
 from ._conversion import serialize, deserialize
 from ._static import static_vars, static_dir
 from ._image import image_as_mime
+from ._tiles import TMSTiles
 
 @static_vars(mgr=None)
 def resource_manager( ):
     if resource_manager.mgr is None:
         resource_manager.mgr = _ResourceManager( )
     return resource_manager.mgr
 
@@ -602,7 +603,23 @@
         else:
             if get_ipython().__class__.__module__ == 'google.colab._shell':
                 return True   # Google Colab
             else:
               return False  # Other type (?)
     except NameError:
         return False
+
+def is_intstr( s ):
+    '''Check to see if a string contains an integer. The standard python checks do not
+    handle things like "-1" or "+45":
+
+    Parameters
+    ----------
+    s: str
+        string to be checked
+    '''
+    try:
+        int(s)
+    except ValueError:
+        return False
+    else:
+        return True
```

### Comparing `casagui-0.3.8/casagui/utils/_conversion.py` & `casagui-0.3.9/casagui/utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/utils/_logging.py` & `casagui-0.3.9/casagui/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/utils/_regions.py` & `casagui-0.3.9/casagui/utils/_regions.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/casagui/utils/_static.py` & `casagui-0.3.9/casagui/utils/_static.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/pyproject.toml` & `casagui-0.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "regions>=0.6",
     "websockets>=10.3",
     "certifi",
     "matplotlib",
 ]
 requires-python = ">=3.8"
 readme = "readme.rst"
-version = "0.3.8"
+version = "0.3.9"
 
 [project.license]
 text = "LGPL"
 
 [tool.pdm.build]
 
 [tool.pdm.version]
```

### Comparing `casagui-0.3.8/readme.rst` & `casagui-0.3.9/readme.rst`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/alma-many-chan/alma-many-chan.py` & `casagui-0.3.9/tests/manual/alma-many-chan/alma-many-chan.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import ssl
 import certifi
 import asyncio
 import urllib
 import tarfile
 
-from casagui.apps import InteractiveClean, MaskMode
+from casagui.apps import InteractiveClean
 
 ##
 ## demo measurement set to use
 ##
 ms_path = [ f'2017.1.00661.S/{ms}' for ms in
             [ 'uid___A002_Xc8d560_X66fa_targets_line.ms',
               'uid___A002_Xc91189_X2368_targets_line.ms',
@@ -97,15 +97,15 @@
                        pbcor=True,
                        weighting='briggsbwtaper',
                        robust=0.5,
                        npixels=0,
                        niter=99999,
                        threshold='0.292Jy',
                        nsigma=0.0,
-                       mask=MaskMode.AUTOMT,
+                       usemask='auto-multithresh',
                        sidelobethreshold=1.25,
                        noisethreshold=5.0,
                        lownoisethreshold=2.0,
                        negativethreshold=0.0,
                        minbeamfrac=0.1,
                        growiterations=75,
                        dogrowprune=True,
```

### Comparing `casagui-0.3.8/tests/manual/basic-websockets-demo/client.html` & `casagui-0.3.9/tests/manual/basic-websockets-demo/client.html`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra-done-stats.py` & `casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra-done-stats.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra-done.py` & `casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra-done.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/cubemask-demo/image-slider-spectra.py` & `casagui-0.3.9/tests/manual/cubemask-demo/image-slider-spectra.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/cubemask-demo/image-slider.py` & `casagui-0.3.9/tests/manual/cubemask-demo/image-slider.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/cubemask-demo/image.py` & `casagui-0.3.9/tests/manual/cubemask-demo/image.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/m100_interactive.py` & `casagui-0.3.9/tests/manual/iclean-demo/m100_interactive.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/mask0-iclean.py` & `casagui-0.3.9/tests/manual/iclean-demo/mask0-iclean.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/run-gclean.py` & `casagui-0.3.9/tests/manual/iclean-demo/run-gclean.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/run-iclean-obj.py` & `casagui-0.3.9/tests/manual/iclean-demo/run-iclean-obj.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/run-iclean.py` & `casagui-0.3.9/tests/manual/iclean-demo/run-iclean.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/iclean-demo/vla-sim-jet-iclean.py` & `casagui-0.3.9/tests/manual/iclean-demo/vla-sim-jet-iclean.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 import ssl
 import certifi
 import asyncio
 import urllib
 import tarfile
 
-from casagui.apps import InteractiveClean, MaskMode
+from casagui.apps import InteractiveClean
 
 ##
 ## demo measurement set to use
 ##
 ms_path = 'sim_data_VLA_jet.ms'
 ##
 ## where to fetch the demo measurement set
@@ -76,15 +76,15 @@
                        nchan=5,
                        start='1.0GHz',
                        width='0.2GHz',
                        pblimit=-1e-05,
                        deconvolver='hogbom',
                        niter=10000,
                        gain=0.2,
-                       mask=MaskMode.AUTOMT )
+                       usemask='auto-multithresh' )
 
 if True:
     print( "Result: %s" % ic( ) )
     print( " Masks: %s" % repr(ic.masks( )) )
 else:
     try:
         asyncio.get_event_loop().run_until_complete(ic.show( ))
```

### Comparing `casagui-0.3.8/tests/manual/iclean-first-look/run-fl.py` & `casagui-0.3.9/tests/manual/iclean-first-look/run-fl.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/large-cube/run-largecube.py` & `casagui-0.3.9/tests/manual/large-cube/run-largecube.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/makemask-demo/run-makemask.py` & `casagui-0.3.9/tests/manual/makemask-demo/run-makemask.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/uranus-demo/uranus-iclean.py` & `casagui-0.3.9/tests/manual/uranus-demo/uranus-iclean.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/websocket-reconnect/client.html` & `casagui-0.3.9/tests/manual/websocket-reconnect/client.html`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/tests/manual/websocket-reconnect/server.py` & `casagui-0.3.9/tests/manual/websocket-reconnect/server.py`

 * *Files identical despite different names*

### Comparing `casagui-0.3.8/PKG-INFO` & `casagui-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casagui
-Version: 0.3.8
+Version: 0.3.9
 Summary: visualization toolkit and apps for casa
 License: LGPL
 Author-email: Darrell Schiebel <darrell@schiebel.us>,Joshua Hoskins <jhoskins@nrao.edu>,Pam Harris <pharris@nrao.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 casagui - visualization tools and applications for CASA
```

