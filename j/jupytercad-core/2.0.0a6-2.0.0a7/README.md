# Comparing `tmp/jupytercad_core-2.0.0a6.tar.gz` & `tmp/jupytercad_core-2.0.0a7.tar.gz`

## Comparing `jupytercad_core-2.0.0a6.tar` & `jupytercad_core-2.0.0a7.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/extension.webpack.config.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/install.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/setup.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/tsconfig.json
--rw-r--r--   0        0        0   101190 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupyter-config/server-config/jupytercad_core.json
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/_version.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/handlers.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/jcad_ydoc.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/step_ydoc.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/stl_ydoc.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/package.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js
--rw-r--r--   0        0        0   237762 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js
--rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js.LICENSE.txt
--rw-r--r--   0        0        0   113742 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/32.249c6bd27daaea51e991.js
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js
--rw-r--r--   0        0        0   183516 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js
--rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/413.e3edef5e15636d5f7630.js
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js
--rw-r--r--   0        0        0   103210 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js
--rw-r--r--   0        0        0  1120083 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js.LICENSE.txt
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/794.55a891e10ed7a9b7a805.js
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/813.013761880a7e5d30e958.js
--rw-r--r--   0        0        0  8606972 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0    10430 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/remoteEntry.42b7768c40743ee87403.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/style.js
--rw-r--r--   0        0        0    64526 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/externalcommand.d.ts
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/externalcommand.js
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/factory.d.ts
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/factory.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/index.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/index.js
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/plugin.d.ts
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/plugin.js
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/schemaregistry.d.ts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/schemaregistry.js
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/workerregistry.d.ts
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/workerregistry.js
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.d.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.js
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/model.d.ts
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/model.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/plugins.d.ts
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/plugins.js
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/model.d.ts
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/model.js
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.js
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/plugins.d.ts
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/plugins.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/webpack -> ../../../../node_modules/webpack/bin/webpack.js
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/scripts/bump-version.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/externalcommand.ts
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/factory.ts
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/index.ts
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/plugin.ts
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/schemaregistry.ts
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/workerregistry.ts
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/model.ts
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/modelfactory.ts
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/plugins.ts
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/model.ts
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/modelfactory.ts
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/plugins.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/index.js
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/README.md
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/extension.webpack.config.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/install.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/setup.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/tsconfig.json
+-rw-r--r--   0        0        0   101336 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupyter-config/server-config/jupytercad_core.json
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/_version.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/handlers.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/jcad_ydoc.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/step_ydoc.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/stl_ydoc.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/package.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js
+-rw-r--r--   0        0        0   238208 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/201.0c67a92e1b3da08ee0d5.js
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js
+-rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js.LICENSE.txt
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js
+-rw-r--r--   0        0        0   183516 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js
+-rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/413.378697570d8f23193ff4.js
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js
+-rw-r--r--   0        0        0   114475 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/54.82242ec748b90c3c68dc.js
+-rw-r--r--   0        0        0   103210 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js
+-rw-r--r--   0        0        0  1120079 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/702.f302218e05c5eeadd41a.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/702.f302218e05c5eeadd41a.js.LICENSE.txt
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/794.65d4da338c815b694314.js
+-rw-r--r--   0        0        0    22897 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/813.b937fc9b357ed86a0372.js
+-rw-r--r--   0        0        0  8606972 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/remoteEntry.0e4fbdda31fcefbd6536.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/style.js
+-rw-r--r--   0        0        0    64526 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/externalcommand.d.ts
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/externalcommand.js
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/factory.d.ts
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/factory.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/index.d.ts
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/index.js
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/plugin.d.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/plugin.js
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/schemaregistry.d.ts
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/schemaregistry.js
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/workerregistry.d.ts
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/workerregistry.js
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/jcadplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/jcadplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/jcadplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/jcadplugin/plugins.js
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/model.d.ts
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/model.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/plugins.d.ts
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stepplugin/plugins.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/model.d.ts
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/model.js
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/modelfactory.js
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/plugins.d.ts
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/lib/stlplugin/plugins.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/node_modules/.bin/webpack -> ../../../../node_modules/webpack/bin/webpack.js
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/scripts/bump-version.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/externalcommand.ts
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/factory.ts
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/index.ts
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/plugin.ts
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/schemaregistry.ts
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/workerregistry.ts
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stepplugin/model.ts
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stepplugin/modelfactory.ts
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stepplugin/plugins.ts
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stlplugin/model.ts
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stlplugin/modelfactory.ts
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/src/stlplugin/plugins.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/style/index.js
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/README.md
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a7/PKG-INFO
```

### Comparing `jupytercad_core-2.0.0a6/extension.webpack.config.js` & `jupytercad_core-2.0.0a7/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/package.json` & `jupytercad_core-2.0.0a7/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724999999999999%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.7', '@jupytercad/occ-worker': "*

 * *                   "'^2.0.0-alpha.7', '@jupytercad/schema': '^2.0.0-alpha.7'}",*

 * * "'version'": "'2.0.0-alpha.7'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.6",
-        "@jupytercad/occ-worker": "^2.0.0-alpha.6",
-        "@jupytercad/schema": "^2.0.0-alpha.6",
+        "@jupytercad/base": "^2.0.0-alpha.7",
+        "@jupytercad/occ-worker": "^2.0.0-alpha.7",
+        "@jupytercad/schema": "^2.0.0-alpha.7",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
@@ -116,9 +116,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.6"
+    "version": "2.0.0-alpha.7"
 }
```

### Comparing `jupytercad_core-2.0.0a6/tsconfig.tsbuildinfo` & `jupytercad_core-2.0.0a7/tsconfig.tsbuildinfo`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9634507842197939%*

 * *Differences: {"'program'": "{'fileNames': {insert: [(302, "*

 * *              "'../../node_modules/@types/react/jsx-runtime.d.ts')]}, 'fileInfos': {134: "*

 * *              "{'version': '8ca4709dbd22a34bcc1ebf93e1877645bdb02ebd3f3d9a211a299a8db2ee4ba1'}, "*

 * *              "insert: [(84, 'eb7375e005b02971567356809faeeecf14becb300aa9ca483fcd6c9f8aa80d8c'), "*

 * *              "(87, '219657f1d170f05d7c1640dd36299a7e9d2554330adc500f4e11e875a2d9bc94'), (94, "*

 * *              "'7097daf64b1ff790a73ff0ab39b4f23c1a75404d903714338dbcae9b47ba347c […]*

```diff
@@ -1,36 +1,36 @@
 {
     "program": {
         "exportedModulesMap": [
             [
-                371,
+                372,
                 1
             ],
             [
-                425,
+                426,
                 2
             ],
             [
-                453,
+                454,
                 3
             ],
             [
-                456,
+                457,
                 4
             ],
             [
-                452,
+                453,
                 5
             ],
             [
-                454,
+                455,
                 6
             ],
             [
-                455,
+                456,
                 7
             ],
             [
                 76,
                 8
             ],
             [
@@ -62,191 +62,191 @@
                 15
             ],
             [
                 126,
                 16
             ],
             [
-                406,
+                407,
                 17
             ],
             [
-                404,
+                405,
                 18
             ],
             [
-                415,
+                416,
                 19
             ],
             [
-                410,
+                411,
                 20
             ],
             [
-                407,
+                408,
                 21
             ],
             [
-                411,
+                412,
                 22
             ],
             [
-                412,
+                413,
                 23
             ],
             [
-                408,
+                409,
                 24
             ],
             [
-                409,
+                410,
                 25
             ],
             [
-                405,
+                406,
                 26
             ],
             [
-                413,
+                414,
                 27
             ],
             [
-                414,
+                415,
                 28
             ],
             [
-                353,
+                354,
                 27
             ],
             [
-                354,
+                355,
                 29
             ],
             [
-                355,
+                356,
                 30
             ],
             [
-                357,
+                358,
                 31
             ],
             [
-                358,
+                359,
                 1
             ],
             [
-                370,
+                371,
                 32
             ],
             [
-                359,
+                360,
                 33
             ],
             [
-                360,
+                361,
                 34
             ],
             [
-                362,
+                363,
                 35
             ],
             [
-                363,
+                364,
                 36
             ],
             [
-                364,
+                365,
                 37
             ],
             [
-                361,
+                362,
                 38
             ],
             [
-                365,
+                366,
                 39
             ],
             [
-                366,
+                367,
                 40
             ],
             [
-                367,
+                368,
                 38
             ],
             [
-                347,
+                348,
                 41
             ],
             [
-                368,
+                369,
                 42
             ],
             [
-                348,
+                349,
                 43
             ],
             [
-                349,
+                350,
                 44
             ],
             [
-                352,
+                353,
                 45
             ],
             [
-                350,
+                351,
                 46
             ],
             [
-                351,
+                352,
                 47
             ],
             [
-                356,
+                357,
                 48
             ],
             [
-                369,
+                370,
                 49
             ],
             [
-                372,
+                373,
                 50
             ],
             [
-                373,
+                374,
                 51
             ],
             [
-                380,
+                381,
                 52
             ],
             [
-                374,
+                375,
                 53
             ],
             [
-                375,
+                376,
                 54
             ],
             [
-                376,
+                377,
                 55
             ],
             [
-                377,
+                378,
                 56
             ],
             [
-                378,
+                379,
                 57
             ],
             [
-                379,
+                380,
                 58
             ],
             [
                 189,
                 59
             ],
             [
@@ -286,235 +286,235 @@
                 1
             ],
             [
                 198,
                 27
             ],
             [
-                457,
+                458,
                 62
             ],
             [
-                464,
+                465,
                 63
             ],
             [
-                460,
+                461,
                 64
             ],
             [
-                461,
+                462,
                 65
             ],
             [
-                462,
+                463,
                 66
             ],
             [
-                463,
+                464,
                 67
             ],
             [
-                458,
+                459,
                 68
             ],
             [
-                459,
+                460,
                 69
             ],
             [
-                395,
+                396,
                 70
             ],
             [
-                382,
+                383,
                 71
             ],
             [
-                383,
+                384,
                 72
             ],
             [
-                396,
+                397,
                 73
             ],
             [
-                394,
+                395,
                 74
             ],
             [
-                381,
+                382,
                 75
             ],
             [
-                469,
+                470,
                 76
             ],
             [
-                466,
+                467,
                 77
             ],
             [
-                474,
+                475,
                 78
             ],
             [
-                468,
+                469,
                 79
             ],
             [
-                465,
+                466,
                 80
             ],
             [
-                470,
+                471,
                 81
             ],
             [
-                471,
+                472,
                 82
             ],
             [
-                472,
+                473,
                 83
             ],
             [
-                473,
+                474,
                 84
             ],
             [
-                477,
+                478,
                 85
             ],
             [
-                475,
+                476,
                 86
             ],
             [
-                476,
+                477,
                 87
             ],
             [
-                486,
+                487,
                 88
             ],
             [
-                487,
+                488,
                 88
             ],
             [
-                488,
+                489,
                 88
             ],
             [
-                496,
+                497,
                 89
             ],
             [
-                489,
+                490,
                 88
             ],
             [
-                495,
+                496,
                 90
             ],
             [
-                490,
+                491,
                 88
             ],
             [
-                491,
+                492,
                 91
             ],
             [
-                492,
+                493,
                 91
             ],
             [
-                494,
+                495,
                 92
             ],
             [
-                493,
+                494,
                 88
             ],
             [
                 73,
                 27
             ],
             [
-                339,
+                340,
                 93
             ],
             [
-                338,
+                339,
                 94
             ],
             [
-                334,
+                335,
                 95
             ],
             [
-                336,
+                337,
                 59
             ],
             [
-                333,
+                334,
                 96
             ],
             [
-                335,
+                336,
                 96
             ],
             [
-                337,
+                338,
                 97
             ],
             [
                 168,
                 98
             ],
             [
-                384,
+                385,
                 99
             ],
             [
-                385,
+                386,
                 40
             ],
             [
-                393,
+                394,
                 100
             ],
             [
-                386,
+                387,
                 1
             ],
             [
-                387,
+                388,
                 101
             ],
             [
-                388,
+                389,
                 99
             ],
             [
-                390,
+                391,
                 102
             ],
             [
-                391,
+                392,
                 103
             ],
             [
-                389,
+                390,
                 104
             ],
             [
-                392,
+                393,
                 105
             ],
             [
                 183,
                 106
             ],
             [
@@ -690,163 +690,163 @@
                 145
             ],
             [
                 297,
                 146
             ],
             [
-                345,
+                346,
                 147
             ],
             [
                 136,
                 148
             ],
             [
                 167,
                 149
             ],
             [
-                307,
+                308,
                 150
             ],
             [
-                320,
+                321,
                 151
             ],
             [
-                321,
+                322,
                 38
             ],
             [
-                341,
+                342,
                 152
             ],
             [
-                322,
+                323,
                 153
             ],
             [
-                319,
+                320,
                 1
             ],
             [
-                323,
+                324,
                 154
             ],
             [
-                326,
+                327,
                 155
             ],
             [
-                327,
+                328,
                 156
             ],
             [
-                328,
+                329,
                 157
             ],
             [
-                329,
+                330,
                 30
             ],
             [
-                330,
+                331,
                 1
             ],
             [
-                331,
+                332,
                 158
             ],
             [
-                332,
+                333,
                 148
             ],
             [
-                325,
+                326,
                 159
             ],
             [
-                324,
+                325,
                 160
             ],
             [
-                340,
+                341,
                 161
             ],
             [
-                342,
+                343,
                 1
             ],
             [
-                313,
+                314,
                 162
             ],
             [
-                318,
+                319,
                 163
             ],
             [
-                312,
+                313,
                 164
             ],
             [
-                314,
+                315,
                 165
             ],
             [
-                317,
+                318,
                 166
             ],
             [
-                315,
+                316,
                 167
             ],
             [
-                316,
+                317,
                 168
             ],
             [
-                346,
+                347,
                 169
             ],
             [
-                310,
+                311,
                 170
             ],
             [
-                311,
+                312,
                 171
             ],
             [
-                343,
+                344,
                 172
             ],
             [
-                344,
+                345,
                 1
             ],
             [
-                303,
+                304,
                 173
             ],
             [
-                305,
+                306,
                 174
             ],
             [
-                306,
+                307,
                 175
             ],
             [
-                304,
+                305,
                 176
             ],
             [
-                403,
+                404,
                 177
             ],
             [
                 151,
                 178
             ],
             [
@@ -886,15 +886,15 @@
                 1
             ],
             [
                 75,
                 61
             ],
             [
-                467,
+                468,
                 182
             ],
             [
                 137,
                 1
             ],
             [
@@ -1322,227 +1322,227 @@
                 210
             ],
             [
                 210,
                 1
             ],
             [
-                508,
+                509,
                 218
             ],
             [
-                509,
+                510,
                 218
             ],
             [
-                544,
+                545,
                 219
             ],
             [
-                545,
+                546,
                 220
             ],
             [
-                546,
+                547,
                 221
             ],
             [
-                547,
+                548,
                 222
             ],
             [
-                548,
+                549,
                 223
             ],
             [
-                549,
+                550,
                 224
             ],
             [
-                550,
+                551,
                 225
             ],
             [
-                551,
+                552,
                 226
             ],
             [
-                552,
+                553,
                 227
             ],
             [
-                553,
+                554,
                 228
             ],
             [
-                554,
+                555,
                 228
             ],
             [
-                556,
+                557,
                 229
             ],
             [
-                555,
+                556,
                 230
             ],
             [
-                557,
+                558,
                 231
             ],
             [
-                558,
+                559,
                 232
             ],
             [
-                559,
+                560,
                 233
             ],
             [
-                543,
+                544,
                 234
             ],
             [
-                593,
+                594,
                 1
             ],
             [
-                560,
+                561,
                 235
             ],
             [
-                561,
+                562,
                 236
             ],
             [
-                562,
+                563,
                 237
             ],
             [
-                594,
+                595,
                 238
             ],
             [
-                563,
+                564,
                 239
             ],
             [
-                564,
+                565,
                 240
             ],
             [
-                565,
+                566,
                 241
             ],
             [
-                566,
+                567,
                 242
             ],
             [
-                567,
+                568,
                 243
             ],
             [
-                568,
+                569,
                 244
             ],
             [
-                569,
+                570,
                 245
             ],
             [
-                570,
+                571,
                 246
             ],
             [
-                571,
+                572,
                 247
             ],
             [
-                572,
+                573,
                 248
             ],
             [
-                573,
+                574,
                 248
             ],
             [
-                574,
+                575,
                 249
             ],
             [
-                575,
+                576,
                 250
             ],
             [
-                577,
+                578,
                 251
             ],
             [
-                576,
+                577,
                 252
             ],
             [
-                578,
+                579,
                 253
             ],
             [
-                579,
+                580,
                 254
             ],
             [
-                580,
+                581,
                 255
             ],
             [
-                581,
+                582,
                 256
             ],
             [
-                582,
+                583,
                 257
             ],
             [
-                583,
+                584,
                 258
             ],
             [
-                584,
+                585,
                 259
             ],
             [
-                585,
+                586,
                 260
             ],
             [
-                586,
+                587,
                 261
             ],
             [
-                587,
+                588,
                 262
             ],
             [
-                588,
+                589,
                 263
             ],
             [
-                589,
+                590,
                 264
             ],
             [
-                590,
+                591,
                 265
             ],
             [
-                591,
+                592,
                 266
             ],
             [
-                592,
+                593,
                 267
             ],
             [
                 134,
                 1
             ],
             [
@@ -1550,23 +1550,27 @@
                 1
             ],
             [
                 135,
                 268
             ],
             [
+                303,
+                148
+            ],
+            [
                 133,
                 1
             ],
             [
-                510,
+                511,
                 1
             ],
             [
-                308,
+                309,
                 1
             ],
             [
                 80,
                 1
             ],
             [
@@ -1766,151 +1770,151 @@
                 1
             ],
             [
                 9,
                 1
             ],
             [
-                309,
+                310,
                 269
             ],
             [
-                526,
+                527,
                 270
             ],
             [
-                533,
+                534,
                 271
             ],
             [
-                525,
+                526,
                 270
             ],
             [
-                540,
+                541,
                 272
             ],
             [
-                517,
+                518,
                 273
             ],
             [
-                516,
+                517,
                 274
             ],
             [
-                539,
+                540,
                 275
             ],
             [
-                534,
+                535,
                 276
             ],
             [
-                537,
+                538,
                 277
             ],
             [
-                519,
+                520,
                 278
             ],
             [
-                518,
+                519,
                 279
             ],
             [
-                514,
+                515,
                 280
             ],
             [
-                513,
+                514,
                 281
             ],
             [
-                536,
+                537,
                 282
             ],
             [
-                515,
+                516,
                 283
             ],
             [
-                520,
+                521,
                 284
             ],
             [
-                521,
+                522,
                 1
             ],
             [
-                524,
+                525,
                 284
             ],
             [
-                511,
+                512,
                 1
             ],
             [
-                542,
+                543,
                 285
             ],
             [
-                541,
+                542,
                 284
             ],
             [
-                528,
+                529,
                 286
             ],
             [
-                529,
+                530,
                 287
             ],
             [
-                531,
+                532,
                 288
             ],
             [
-                527,
+                528,
                 289
             ],
             [
-                530,
+                531,
                 290
             ],
             [
-                535,
+                536,
                 275
             ],
             [
-                522,
+                523,
                 291
             ],
             [
-                523,
+                524,
                 292
             ],
             [
-                532,
+                533,
                 293
             ],
             [
-                512,
+                513,
                 294
             ],
             [
-                538,
+                539,
                 295
             ],
             [
                 124,
                 296
             ],
             [
-                451,
+                452,
                 297
             ],
             [
                 122,
                 298
             ],
             [
@@ -2074,167 +2078,167 @@
                 329
             ],
             [
                 111,
                 330
             ],
             [
-                422,
+                423,
                 331
             ],
             [
-                421,
+                422,
                 332
             ],
             [
-                420,
+                421,
                 333
             ],
             [
-                448,
+                449,
                 334
             ],
             [
-                447,
+                448,
                 335
             ],
             [
-                445,
+                446,
                 336
             ],
             [
-                446,
+                447,
                 337
             ],
             [
-                418,
+                419,
                 338
             ],
             [
-                419,
+                420,
                 339
             ],
             [
-                449,
+                450,
                 340
             ],
             [
-                424,
+                425,
                 341
             ],
             [
-                427,
+                428,
                 342
             ],
             [
-                428,
+                429,
                 38
             ],
             [
-                434,
+                435,
                 343
             ],
             [
-                429,
+                430,
                 344
             ],
             [
-                430,
+                431,
                 345
             ],
             [
-                431,
+                432,
                 346
             ],
             [
-                432,
+                433,
                 347
             ],
             [
-                433,
+                434,
                 344
             ],
             [
-                436,
+                437,
                 348
             ],
             [
-                441,
+                442,
                 349
             ],
             [
-                437,
+                438,
                 350
             ],
             [
-                438,
+                439,
                 351
             ],
             [
-                439,
+                440,
                 352
             ],
             [
-                440,
+                441,
                 348
             ],
             [
-                435,
+                436,
                 353
             ],
             [
-                444,
+                445,
                 354
             ],
             [
-                442,
+                443,
                 337
             ],
             [
-                443,
+                444,
                 355
             ],
             [
-                423,
+                424,
                 91
             ],
             [
-                416,
+                417,
                 356
             ],
             [
-                417,
+                418,
                 357
             ],
             [
-                426,
+                427,
                 2
             ],
             [
-                502,
+                503,
                 358
             ],
             [
-                500,
+                501,
                 359
             ],
             [
-                501,
+                502,
                 360
             ],
             [
-                499,
+                500,
                 361
             ],
             [
-                498,
+                499,
                 362
             ],
             [
-                497,
+                498,
                 1
             ],
             [
                 48,
                 1
             ],
             [
@@ -2262,15 +2266,15 @@
                 1
             ],
             [
                 51,
                 1
             ],
             [
-                504,
+                505,
                 1
             ],
             [
                 56,
                 1
             ],
             [
@@ -2298,362 +2302,361 @@
                 1
             ],
             [
                 62,
                 1
             ],
             [
-                399,
+                400,
                 363
             ],
             [
-                397,
+                398,
                 364
             ],
             [
-                398,
+                399,
                 365
             ],
             [
-                400,
+                401,
                 366
             ],
             [
-                401,
+                402,
                 367
             ],
             [
-                402,
+                403,
                 378
             ],
             [
-                450,
+                451,
                 379
             ],
             [
-                507,
+                508,
                 380
             ],
             [
-                478,
+                479,
                 381
             ],
             [
-                479,
+                480,
                 382
             ],
             [
-                506,
+                507,
                 383
             ],
             [
-                505,
+                506,
                 378
             ],
             [
-                481,
+                482,
                 384
             ],
             [
-                480,
+                481,
                 381
             ],
             [
-                482,
+                483,
                 382
             ],
             [
-                484,
+                485,
                 384
             ],
             [
-                483,
+                484,
                 381
             ],
             [
-                485,
+                486,
                 382
             ],
             [
-                503,
+                504,
                 378
             ]
         ],
         "fileIdsList": [
             [
-                425,
-                426
+                426,
+                427
             ],
             [
                 135,
                 210,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 131,
                 296,
-                425,
                 426,
-                451,
-                452
+                427,
+                452,
+                453
             ],
             [
-                425,
                 426,
-                452,
+                427,
                 453,
                 454,
-                455
+                455,
+                456
             ],
             [
                 72,
                 74,
                 131,
                 296,
-                425,
                 426,
-                453
+                427,
+                454
             ],
             [
                 296,
                 302,
-                425,
                 426,
-                452
+                427,
+                453
             ],
             [
                 75,
                 131,
                 296,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
                 74,
                 75,
-                425,
-                426
+                426,
+                427
             ],
             [
                 124,
-                425,
-                426
+                426,
+                427
             ],
             [
                 76,
                 123,
                 125,
                 126,
                 127,
                 128,
                 129,
                 130,
-                425,
-                426
+                426,
+                427
             ],
             [
                 76,
                 122,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
                 74,
                 76,
                 122,
                 124,
                 126,
                 130,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 76,
                 122,
                 124,
-                425,
-                426
+                426,
+                427
             ],
             [
                 76,
                 122,
                 126,
                 127,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
                 74,
                 76,
                 122,
                 127,
                 129,
-                425,
-                426
+                426,
+                427
             ],
             [
                 76,
                 122,
                 124,
-                425,
-                426
+                426,
+                427
             ],
             [
-                405,
-                425,
-                426
+                406,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 166,
                 296,
-                346,
-                370,
-                396,
-                403,
-                425,
-                426
+                347,
+                371,
+                397,
+                404,
+                426,
+                427
             ],
             [
-                404,
                 405,
                 406,
                 407,
                 408,
-                410,
+                409,
                 411,
                 412,
                 413,
                 414,
-                425,
-                426
+                415,
+                426,
+                427
             ],
             [
                 72,
                 168,
-                404,
-                408,
+                405,
                 409,
-                425,
-                426
+                410,
+                426,
+                427
             ],
             [
                 72,
                 151,
                 166,
                 209,
-                370,
-                408,
-                425,
-                426
+                371,
+                409,
+                426,
+                427
             ],
             [
                 72,
                 168,
-                370,
-                396,
-                415,
-                425,
-                426
+                371,
+                397,
+                416,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 151,
-                405,
-                425,
-                426
+                406,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 137,
                 166,
                 302,
-                396,
-                404,
-                407,
-                425,
-                426
+                397,
+                405,
+                408,
+                426,
+                427
             ],
             [
                 74,
                 75,
-                404,
                 405,
-                425,
-                426
+                406,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 151,
                 296,
                 302,
-                404,
-                425,
-                426
+                405,
+                426,
+                427
             ],
             [
                 72,
-                425,
-                426
+                426,
+                427
             ],
             [
                 151,
                 302,
-                370,
-                404,
-                425,
-                426
+                371,
+                405,
+                426,
+                427
             ],
             [
                 72,
                 75,
                 138,
                 151,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 135,
                 137,
                 166,
                 302,
-                356,
-                425,
-                426
+                357,
+                426,
+                427
             ],
             [
                 166,
-                346,
                 347,
                 348,
-                352,
+                349,
                 353,
                 354,
                 355,
                 356,
                 357,
                 358,
                 359,
@@ -2663,702 +2666,703 @@
                 363,
                 364,
                 365,
                 366,
                 367,
                 368,
                 369,
-                425,
-                426
+                370,
+                426,
+                427
             ],
             [
-                357,
-                425,
-                426
+                358,
+                426,
+                427
             ],
             [
                 302,
-                346,
                 347,
-                425,
-                426
+                348,
+                426,
+                427
             ],
             [
                 137,
                 166,
                 302,
-                346,
-                361,
-                425,
-                426
+                347,
+                362,
+                426,
+                427
             ],
             [
                 166,
                 287,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
-                425,
-                426
+                426,
+                427
             ],
             [
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 296,
                 302,
-                346,
-                425,
-                426
+                347,
+                426,
+                427
             ],
             [
                 168,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 199,
                 296,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 166,
                 199,
                 287,
                 302,
-                348,
-                425,
-                426
+                349,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 166,
                 168,
                 199,
                 287,
-                347,
-                425,
-                426
+                348,
+                426,
+                427
             ],
             [
                 166,
                 287,
                 302,
-                339,
-                346,
-                348,
-                425,
-                426
+                340,
+                347,
+                349,
+                426,
+                427
             ],
             [
-                349,
                 350,
                 351,
-                425,
-                426
+                352,
+                426,
+                427
             ],
             [
                 74,
                 151,
                 166,
-                348,
-                425,
-                426
+                349,
+                426,
+                427
             ],
             [
                 166,
                 302,
-                347,
-                425,
-                426
+                348,
+                426,
+                427
             ],
             [
                 74,
                 75,
                 166,
                 209,
-                425,
-                426
+                426,
+                427
             ],
             [
-                348,
-                425,
-                426
+                349,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 131,
                 199,
                 302,
-                339,
-                371,
-                425,
-                426
+                340,
+                372,
+                426,
+                427
             ],
             [
-                372,
-                425,
-                426
+                373,
+                426,
+                427
             ],
             [
-                372,
                 373,
                 374,
                 375,
                 376,
                 377,
                 378,
                 379,
-                425,
-                426
+                380,
+                426,
+                427
             ],
             [
                 137,
                 166,
                 302,
-                339,
-                372,
-                425,
-                426
+                340,
+                373,
+                426,
+                427
             ],
             [
                 135,
                 302,
-                346,
-                372,
-                425,
-                426
+                347,
+                373,
+                426,
+                427
             ],
             [
                 73,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 166,
-                372,
                 373,
-                376,
-                425,
-                426
+                374,
+                377,
+                426,
+                427
             ],
             [
                 166,
-                372,
-                425,
-                426
+                373,
+                426,
+                427
             ],
             [
                 137,
                 166,
-                380,
-                425,
-                426
+                381,
+                426,
+                427
             ],
             [
                 74,
                 75,
-                425,
-                426
+                426,
+                427
             ],
             [
                 189,
                 190,
                 191,
                 192,
                 193,
                 194,
                 195,
                 196,
                 197,
                 198,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 296,
                 302,
-                396,
-                425,
+                397,
                 426,
-                464
+                427,
+                465
             ],
             [
-                425,
                 426,
-                457,
+                427,
                 458,
                 459,
                 460,
                 461,
                 462,
-                463
+                463,
+                464
             ],
             [
                 74,
                 75,
                 166,
                 199,
                 296,
                 302,
-                370,
-                396,
-                425,
+                371,
+                397,
                 426,
-                458,
-                459
+                427,
+                459,
+                460
             ],
             [
                 166,
-                346,
-                425,
+                347,
                 426,
-                458
+                427,
+                459
             ],
             [
                 75,
-                396,
-                425,
-                426
+                397,
+                426,
+                427
             ],
             [
                 166,
                 302,
-                346,
-                396,
-                425,
+                347,
+                397,
                 426,
-                458
+                427,
+                459
             ],
             [
                 72,
                 74,
                 75,
                 166,
                 199,
                 296,
-                396,
-                425,
-                426
+                397,
+                426,
+                427
             ],
             [
                 74,
                 75,
                 137,
                 166,
                 199,
                 302,
-                396,
-                425,
-                426
+                397,
+                426,
+                427
             ],
             [
                 166,
                 302,
-                396,
-                425,
-                426
+                397,
+                426,
+                427
             ],
             [
                 74,
                 75,
                 166,
                 168,
                 296,
                 302,
-                370,
-                381,
-                425,
-                426
+                371,
+                382,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 131,
                 166,
                 168,
                 199,
                 296,
                 302,
-                370,
-                380,
-                396,
-                425,
-                426
+                371,
+                381,
+                397,
+                426,
+                427
             ],
             [
-                381,
                 382,
                 383,
-                394,
+                384,
                 395,
-                425,
-                426
+                396,
+                426,
+                427
             ],
             [
                 137,
                 166,
                 302,
-                370,
-                381,
-                383,
-                393,
-                425,
-                426
+                371,
+                382,
+                384,
+                394,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 131,
                 166,
                 168,
                 199,
                 296,
                 302,
-                339,
-                346,
-                370,
-                380,
-                425,
-                426
+                340,
+                347,
+                371,
+                381,
+                426,
+                427
             ],
             [
                 166,
                 296,
                 302,
-                346,
-                425,
+                347,
                 426,
-                465,
+                427,
                 466,
-                468
+                467,
+                469
             ],
             [
                 137,
                 166,
                 302,
-                425,
                 426,
-                465
+                427,
+                466
             ],
             [
-                425,
                 426,
-                465,
+                427,
                 466,
-                468,
+                467,
                 469,
                 470,
                 471,
                 472,
-                473
+                473,
+                474
             ],
             [
                 74,
                 137,
                 166,
                 296,
                 302,
-                396,
-                425,
+                397,
                 426,
-                465,
-                467
+                427,
+                466,
+                468
             ],
             [
                 74,
                 75,
                 174,
                 199,
                 209,
                 296,
                 302,
-                346,
-                425,
+                347,
                 426,
-                464
+                427,
+                465
             ],
             [
                 296,
                 302,
-                346,
-                370,
-                425,
+                347,
+                371,
                 426,
-                464
+                427,
+                465
             ],
             [
                 72,
                 209,
-                370,
-                425,
+                371,
                 426,
-                469
+                427,
+                470
             ],
             [
                 302,
-                346,
-                425,
+                347,
                 426,
-                465
+                427,
+                466
             ],
             [
                 302,
-                346,
-                370,
-                425,
+                347,
+                371,
                 426,
-                474
+                427,
+                475
             ],
             [
-                425,
                 426,
-                475,
-                476
+                427,
+                476,
+                477
             ],
             [
                 72,
                 75,
                 151,
                 166,
                 302,
-                346,
-                425,
-                426
+                347,
+                426,
+                427
             ],
             [
                 75,
                 135,
                 302,
-                346,
-                425,
+                347,
                 426,
-                475
+                427,
+                476
             ],
             [
-                346,
-                370,
-                425,
-                426
+                347,
+                371,
+                426,
+                427
             ],
             [
-                425,
                 426,
-                486,
+                427,
                 487,
                 488,
                 489,
                 490,
                 491,
                 492,
                 493,
                 494,
-                495
+                495,
+                496
             ],
             [
                 151,
                 166,
                 302,
-                346,
-                425,
+                347,
                 426,
-                486,
+                427,
                 487,
                 488,
                 489,
                 490,
                 491,
                 492,
                 493,
-                494
+                494,
+                495
             ],
             [
-                346,
-                425,
-                426
+                347,
+                426,
+                427
             ],
             [
                 72,
                 166,
-                370,
-                425,
+                371,
                 426,
-                486,
+                427,
                 487,
                 488,
                 489,
                 490,
                 491,
                 492,
-                493
+                493,
+                494
             ],
             [
-                333,
                 334,
                 335,
                 336,
                 337,
                 338,
-                425,
-                426
+                339,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
-                333,
                 334,
                 335,
-                337,
-                425,
-                426
+                336,
+                338,
+                426,
+                427
             ],
             [
                 72,
                 137,
-                333,
-                425,
-                426
+                334,
+                426,
+                427
             ],
             [
                 74,
                 75,
-                338,
-                425,
-                426
+                339,
+                426,
+                427
             ],
             [
                 72,
-                336,
-                425,
-                426
+                337,
+                426,
+                427
             ],
             [
                 72,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
                 74,
                 168,
-                425,
-                426
+                426,
+                427
             ],
             [
                 168,
-                384,
                 385,
                 386,
                 387,
                 388,
                 389,
                 390,
                 391,
                 392,
-                425,
-                426
+                393,
+                426,
+                427
             ],
             [
                 72,
                 168,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 168,
                 296,
                 302,
-                387,
-                389,
-                425,
-                426
+                388,
+                390,
+                426,
+                427
             ],
             [
                 168,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 168,
                 302,
-                387,
-                425,
-                426
+                388,
+                426,
+                427
             ],
             [
                 137,
                 166,
                 168,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 182,
-                425,
-                426
+                426,
+                427
             ],
             [
                 182,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 131,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 182,
-                425,
-                426
+                426,
+                427
             ],
             [
                 176,
                 181,
                 182,
                 183,
                 184,
@@ -3368,93 +3372,93 @@
                 188,
                 203,
                 288,
                 292,
                 293,
                 294,
                 295,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 169,
                 176,
                 178,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 169,
                 177,
                 178,
                 179,
                 180,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 169,
                 176,
                 177,
                 183,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 174,
                 177,
                 178,
                 183,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
-                425,
-                426
+                426,
+                427
             ],
             [
                 170,
                 171,
                 175,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 170,
                 183,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 170,
                 171,
                 174,
                 182,
                 183,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 182,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 174,
                 176,
                 181,
@@ -3464,568 +3468,569 @@
                 187,
                 188,
                 203,
                 288,
                 292,
                 293,
                 294,
-                425,
-                426
+                426,
+                427
             ],
             [
                 181,
-                425,
-                426
+                426,
+                427
             ],
             [
                 200,
                 201,
                 202,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 174,
                 181,
                 182,
                 183,
                 200,
-                425,
-                426
+                426,
+                427
             ],
             [
                 182,
                 203,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 181,
                 199,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 182,
                 209,
                 287,
-                425,
-                426
+                426,
+                427
             ],
             [
                 289,
                 290,
                 291,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 174,
                 183,
                 290,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 183,
                 289,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 174,
                 182,
                 183,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 182,
                 209,
-                425,
-                426
+                426,
+                427
             ],
             [
                 285,
                 286,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 209,
                 285,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 73,
                 74,
                 75,
                 209,
                 284,
                 286,
-                425,
-                426
+                426,
+                427
             ],
             [
                 204,
-                425,
-                426
+                426,
+                427
             ],
             [
                 204,
                 205,
                 206,
                 207,
                 208,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 151,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 204,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 204,
                 207,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 204,
-                425,
-                426
+                426,
+                427
             ],
             [
                 297,
-                425,
-                426
+                426,
+                427
             ],
             [
                 297,
                 298,
                 299,
                 300,
                 301,
-                425,
-                426
+                426,
+                427
             ],
             [
                 296,
                 297,
-                425,
-                426
+                426,
+                427
             ],
             [
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 168,
                 209,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
-                343,
-                425,
-                426
+                344,
+                426,
+                427
             ],
             [
                 135,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 135,
                 284,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
                 135,
-                318,
                 319,
-                425,
-                426
+                320,
+                426,
+                427
             ],
             [
                 136,
                 167,
-                307,
-                319,
+                308,
                 320,
                 321,
                 322,
                 323,
                 324,
                 325,
                 326,
                 327,
                 328,
                 329,
                 330,
                 331,
                 332,
-                340,
-                425,
-                426
+                333,
+                341,
+                426,
+                427
             ],
             [
                 135,
-                318,
-                425,
-                426
+                319,
+                426,
+                427
             ],
             [
                 75,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 166,
-                325,
-                425,
-                426
+                326,
+                426,
+                427
             ],
             [
                 135,
-                324,
-                425,
-                426
+                325,
+                426,
+                427
             ],
             [
                 166,
                 302,
-                325,
-                425,
-                426
+                326,
+                426,
+                427
             ],
             [
                 74,
                 166,
                 199,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 137,
                 151,
                 166,
                 302,
-                318,
-                324,
-                425,
-                426
+                319,
+                325,
+                426,
+                427
             ],
             [
                 74,
                 75,
                 135,
                 137,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 137,
                 166,
                 199,
-                339,
-                425,
-                426
+                340,
+                426,
+                427
             ],
             [
-                312,
-                425,
-                426
+                313,
+                426,
+                427
             ],
             [
-                312,
                 313,
-                317,
-                425,
-                426
+                314,
+                318,
+                426,
+                427
             ],
             [
                 74,
                 135,
                 138,
                 168,
-                311,
-                425,
-                426
+                312,
+                426,
+                427
             ],
             [
                 138,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
-                314,
                 315,
                 316,
-                425,
-                426
+                317,
+                426,
+                427
             ],
             [
                 74,
                 75,
                 138,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 138,
                 166,
                 302,
-                425,
-                426
+                426,
+                427
             ],
             [
-                318,
-                341,
+                319,
                 342,
                 343,
                 344,
                 345,
-                425,
-                426
+                346,
+                426,
+                427
             ],
             [
-                309,
-                425,
-                426
+                310,
+                426,
+                427
             ],
             [
-                310,
-                425,
-                426
+                311,
+                426,
+                427
             ],
             [
                 72,
                 284,
-                425,
-                426
+                426,
+                427
             ],
             [
                 135,
                 284,
-                425,
-                426
+                303,
+                426,
+                427
             ],
             [
                 284,
-                425,
-                426
+                426,
+                427
             ],
             [
-                303,
                 304,
                 305,
-                425,
-                426
+                306,
+                426,
+                427
             ],
             [
                 135,
                 284,
-                303,
-                425,
-                426
+                304,
+                426,
+                427
             ],
             [
                 72,
                 151,
                 166,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
                 138,
-                425,
-                426
+                426,
+                427
             ],
             [
                 64,
                 65,
                 66,
                 67,
-                425,
-                426
+                426,
+                427
             ],
             [
                 68,
                 70,
                 71,
-                425,
-                426
+                426,
+                427
             ],
             [
                 69,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 75,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 172,
                 173,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 174,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 172,
                 174,
-                425,
-                426
+                426,
+                427
             ],
             [
                 139,
                 140,
                 143,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 139,
                 140,
                 143,
                 144,
                 146,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 140,
                 142,
-                425,
-                426
+                426,
+                427
             ],
             [
                 140,
                 145,
                 149,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 137,
                 138,
                 140,
                 151,
-                425,
-                426
+                426,
+                427
             ],
             [
                 75,
                 151,
                 153,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 140,
                 141,
                 155,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 140,
                 155,
                 156,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 140,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 140,
                 141,
-                425,
-                426
+                426,
+                427
             ],
             [
                 139,
                 140,
                 141,
                 142,
                 143,
@@ -4046,129 +4051,129 @@
                 159,
                 160,
                 161,
                 162,
                 163,
                 164,
                 165,
-                425,
-                426
+                426,
+                427
             ],
             [
                 75,
                 137,
                 140,
-                425,
-                426
+                426,
+                427
             ],
             [
                 72,
                 74,
                 137,
                 138,
                 140,
                 151,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 138,
                 139,
                 140,
                 153,
-                425,
-                426
+                426,
+                427
             ],
             [
                 140,
                 142,
-                425,
-                426
+                426,
+                427
             ],
             [
                 140,
                 141,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 140,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 140,
                 143,
                 145,
-                425,
-                426
+                426,
+                427
             ],
             [
                 137,
                 140,
                 141,
                 142,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 140,
                 145,
                 163,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 137,
                 138,
                 139,
                 140,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 140,
                 155,
                 164,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 138,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 75,
                 137,
                 139,
                 141,
-                425,
-                426
+                426,
+                427
             ],
             [
                 212,
-                425,
-                426
+                426,
+                427
             ],
             [
                 211,
-                425,
-                426
+                426,
+                427
             ],
             [
                 211,
                 212,
                 213,
                 214,
                 215,
@@ -4221,28 +4226,28 @@
                 262,
                 263,
                 264,
                 265,
                 266,
                 269,
                 283,
-                425,
-                426
+                426,
+                427
             ],
             [
                 267,
                 268,
-                425,
-                426
+                426,
+                427
             ],
             [
                 212,
                 267,
-                425,
-                426
+                426,
+                427
             ],
             [
                 270,
                 271,
                 272,
                 273,
                 274,
@@ -4250,185 +4255,184 @@
                 276,
                 277,
                 278,
                 279,
                 280,
                 281,
                 282,
-                425,
-                426
+                426,
+                427
             ],
             [
                 210,
                 212,
-                425,
-                426
+                426,
+                427
             ],
             [
                 135,
                 210,
                 211,
-                425,
-                426
-            ],
-            [
-                425,
                 426,
-                508
+                427
             ],
             [
-                425,
                 426,
-                544
+                427,
+                509
             ],
             [
-                425,
                 426,
-                545,
-                550,
-                578
+                427,
+                545
             ],
             [
-                425,
                 426,
+                427,
                 546,
-                557,
-                558,
-                565,
-                575,
-                586
+                551,
+                579
             ],
             [
-                425,
                 426,
-                546,
+                427,
                 547,
-                557,
-                565
+                558,
+                559,
+                566,
+                576,
+                587
             ],
             [
-                425,
                 426,
+                427,
+                547,
                 548,
-                587
+                558,
+                566
             ],
             [
-                425,
                 426,
+                427,
                 549,
-                550,
-                558,
-                566
+                588
             ],
             [
-                425,
                 426,
+                427,
                 550,
-                575,
-                583
+                551,
+                559,
+                567
             ],
             [
-                425,
                 426,
+                427,
                 551,
-                553,
-                557,
-                565
+                576,
+                584
             ],
             [
-                425,
                 426,
-                544,
-                552
+                427,
+                552,
+                554,
+                558,
+                566
             ],
             [
-                425,
                 426,
-                553,
-                554
+                427,
+                545,
+                553
             ],
             [
-                425,
                 426,
-                557
+                427,
+                554,
+                555
             ],
             [
-                425,
                 426,
-                555,
-                557
+                427,
+                558
             ],
             [
-                425,
                 426,
-                544,
-                557
+                427,
+                556,
+                558
             ],
             [
-                425,
                 426,
-                557,
+                427,
+                545,
+                558
+            ],
+            [
+                426,
+                427,
                 558,
                 559,
-                575,
-                586
+                560,
+                576,
+                587
             ],
             [
-                425,
                 426,
-                557,
+                427,
                 558,
                 559,
-                572,
-                575,
-                578
+                560,
+                573,
+                576,
+                579
             ],
             [
-                425,
                 426,
-                542,
-                591
+                427,
+                543,
+                592
             ],
             [
-                425,
                 426,
-                553,
-                557,
-                560,
-                565,
-                575,
-                586
+                427,
+                554,
+                558,
+                561,
+                566,
+                576,
+                587
             ],
             [
-                425,
                 426,
-                557,
+                427,
                 558,
-                560,
+                559,
                 561,
-                565,
-                575,
-                583,
-                586
+                562,
+                566,
+                576,
+                584,
+                587
             ],
             [
-                425,
                 426,
-                560,
-                562,
-                575,
-                583,
-                586
+                427,
+                561,
+                563,
+                576,
+                584,
+                587
             ],
             [
-                425,
                 426,
-                508,
+                427,
                 509,
-                543,
+                510,
                 544,
                 545,
                 546,
                 547,
                 548,
                 549,
                 550,
@@ -4470,447 +4474,448 @@
                 586,
                 587,
                 588,
                 589,
                 590,
                 591,
                 592,
-                593
-            ],
-            [
-                425,
-                426,
-                557,
-                563
+                593,
+                594
             ],
             [
-                425,
                 426,
-                564,
-                586,
-                591
+                427,
+                558,
+                564
             ],
             [
-                425,
                 426,
-                553,
-                557,
+                427,
                 565,
-                575
+                587,
+                592
             ],
             [
-                425,
                 426,
-                566
+                427,
+                554,
+                558,
+                566,
+                576
             ],
             [
-                425,
                 426,
+                427,
                 567
             ],
             [
-                425,
                 426,
-                544,
+                427,
                 568
             ],
             [
-                425,
                 426,
-                569,
-                585,
-                591
+                427,
+                545,
+                569
             ],
             [
-                425,
                 426,
-                570
+                427,
+                570,
+                586,
+                592
             ],
             [
-                425,
                 426,
+                427,
                 571
             ],
             [
-                425,
                 426,
-                557,
-                572,
-                573
+                427,
+                572
             ],
             [
-                425,
                 426,
-                572,
-                574,
-                587,
-                589
+                427,
+                558,
+                573,
+                574
             ],
             [
-                425,
                 426,
-                545,
-                557,
+                427,
+                573,
                 575,
-                576,
-                577,
-                578
+                588,
+                590
             ],
             [
-                425,
                 426,
-                545,
-                575,
-                577
+                427,
+                546,
+                558,
+                576,
+                577,
+                578,
+                579
             ],
             [
-                425,
                 426,
-                575,
-                576
+                427,
+                546,
+                576,
+                578
             ],
             [
-                425,
                 426,
-                578
+                427,
+                576,
+                577
             ],
             [
-                425,
                 426,
+                427,
                 579
             ],
             [
-                425,
                 426,
-                544,
-                575
+                427,
+                580
             ],
             [
-                425,
                 426,
-                557,
-                581,
-                582
+                427,
+                545,
+                576
             ],
             [
-                425,
                 426,
-                581,
-                582
+                427,
+                558,
+                582,
+                583
             ],
             [
-                425,
                 426,
-                550,
-                565,
-                575,
+                427,
+                582,
                 583
             ],
             [
-                425,
                 426,
+                427,
+                551,
+                566,
+                576,
                 584
             ],
             [
-                425,
                 426,
-                565,
+                427,
                 585
             ],
             [
-                425,
                 426,
-                545,
-                560,
-                571,
+                427,
+                566,
                 586
             ],
             [
-                425,
                 426,
-                550,
+                427,
+                546,
+                561,
+                572,
                 587
             ],
             [
-                425,
                 426,
-                575,
+                427,
+                551,
                 588
             ],
             [
-                425,
                 426,
-                564,
+                427,
+                576,
                 589
             ],
             [
-                425,
                 426,
+                427,
+                565,
                 590
             ],
             [
-                425,
                 426,
-                545,
-                550,
-                557,
-                559,
-                568,
-                575,
-                586,
-                589,
+                427,
                 591
             ],
             [
-                425,
                 426,
-                575,
+                427,
+                546,
+                551,
+                558,
+                560,
+                569,
+                576,
+                587,
+                590,
                 592
             ],
             [
+                426,
+                427,
+                576,
+                593
+            ],
+            [
                 132,
                 133,
                 134,
-                425,
-                426
+                426,
+                427
             ],
             [
-                308,
-                425,
-                426
+                309,
+                426,
+                427
             ],
             [
-                425,
                 426,
-                519,
-                523,
-                586
+                427,
+                520,
+                524,
+                587
             ],
             [
-                425,
                 426,
-                519,
-                575,
-                586
+                427,
+                520,
+                576,
+                587
             ],
             [
-                425,
                 426,
-                514
+                427,
+                515
             ],
             [
-                425,
                 426,
-                516,
-                519,
-                583,
-                586
+                427,
+                517,
+                520,
+                584,
+                587
             ],
             [
-                425,
                 426,
-                565,
-                583
+                427,
+                566,
+                584
             ],
             [
-                425,
                 426,
-                594
+                427,
+                595
             ],
             [
-                425,
                 426,
-                514,
-                594
+                427,
+                515,
+                595
             ],
             [
-                425,
                 426,
-                516,
-                519,
-                565,
-                586
+                427,
+                517,
+                520,
+                566,
+                587
             ],
             [
-                425,
                 426,
-                511,
+                427,
                 512,
-                515,
-                518,
-                545,
-                557,
-                575,
-                586
+                513,
+                516,
+                519,
+                546,
+                558,
+                576,
+                587
             ],
             [
-                425,
                 426,
-                511,
-                517
+                427,
+                512,
+                518
             ],
             [
-                425,
                 426,
-                515,
-                519,
-                545,
-                578,
-                586,
-                594
+                427,
+                516,
+                520,
+                546,
+                579,
+                587,
+                595
             ],
             [
-                425,
                 426,
-                545,
-                594
+                427,
+                546,
+                595
             ],
             [
-                425,
                 426,
-                535,
-                545,
-                594
+                427,
+                536,
+                546,
+                595
             ],
             [
-                425,
                 426,
-                513,
+                427,
                 514,
-                594
+                515,
+                595
             ],
             [
-                425,
                 426,
-                519
+                427,
+                520
             ],
             [
-                425,
                 426,
-                513,
+                427,
                 514,
                 515,
                 516,
                 517,
                 518,
                 519,
                 520,
                 521,
-                523,
+                522,
                 524,
                 525,
                 526,
                 527,
                 528,
                 529,
                 530,
                 531,
                 532,
                 533,
                 534,
-                536,
+                535,
                 537,
                 538,
                 539,
                 540,
-                541
-            ],
-            [
-                425,
-                426,
-                519,
-                526,
-                527
+                541,
+                542
             ],
             [
-                425,
                 426,
-                517,
-                519,
+                427,
+                520,
                 527,
                 528
             ],
             [
-                425,
                 426,
-                518
+                427,
+                518,
+                520,
+                528,
+                529
             ],
             [
-                425,
                 426,
-                511,
-                514,
+                427,
                 519
             ],
             [
-                425,
                 426,
-                519,
-                523,
-                527,
-                528
+                427,
+                512,
+                515,
+                520
             ],
             [
-                425,
                 426,
-                523
+                427,
+                520,
+                524,
+                528,
+                529
             ],
             [
-                425,
                 426,
-                517,
-                519,
-                522,
-                586
+                427,
+                524
             ],
             [
-                425,
                 426,
-                511,
-                516,
-                517,
-                519,
+                427,
+                518,
+                520,
                 523,
-                526
+                587
             ],
             [
-                425,
                 426,
-                545,
-                575
+                427,
+                512,
+                517,
+                518,
+                520,
+                524,
+                527
             ],
             [
-                425,
                 426,
-                514,
-                519,
-                535,
-                545,
-                591,
-                594
+                427,
+                546,
+                576
+            ],
+            [
+                426,
+                427,
+                515,
+                520,
+                536,
+                546,
+                592,
+                595
             ],
             [
                 77,
                 122,
-                425,
-                426
+                426,
+                427
             ],
             [
                 77,
                 79,
                 80,
                 122,
                 124,
-                425,
-                426
+                426,
+                427
             ],
             [
                 121,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 83,
                 84,
                 85,
@@ -4945,573 +4950,573 @@
                 114,
                 115,
                 116,
                 117,
                 118,
                 119,
                 120,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 85,
                 89,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 85,
                 92,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 85,
                 92,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 85,
                 88,
                 92,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 85,
                 90,
                 92,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 83,
                 85,
                 88,
                 89,
                 90,
                 92,
                 93,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 84,
                 85,
                 86,
                 87,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 84,
                 85,
                 88,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 84,
                 85,
                 87,
                 88,
                 89,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 87,
                 88,
                 98,
                 101,
-                425,
-                426
+                426,
+                427
             ],
             [
                 84,
                 85,
                 98,
                 101,
                 102,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 88,
                 94,
                 98,
                 99,
                 100,
                 102,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 97,
-                425,
-                426
+                426,
+                427
             ],
             [
                 82,
                 96,
                 102,
-                425,
-                426
+                426,
+                427
             ],
             [
                 77,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 85,
                 89,
                 91,
                 92,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 77,
                 78,
                 84,
                 85,
                 88,
                 92,
                 94,
                 95,
                 96,
                 97,
                 101,
                 102,
-                425,
-                426
+                426,
+                427
             ],
             [
                 79,
                 80,
                 88,
-                425,
-                426
+                426,
+                427
             ],
             [
                 83,
                 85,
                 89,
                 97,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 79,
                 80,
                 88,
                 89,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 83,
                 85,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 85,
                 89,
                 91,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 83,
                 84,
                 88,
                 89,
                 90,
                 92,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 77,
                 83,
                 84,
                 85,
                 88,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 80,
                 89,
-                425,
-                426
+                426,
+                427
             ],
             [
                 79,
                 89,
-                425,
-                426
+                426,
+                427
             ],
             [
                 85,
                 88,
                 90,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 80,
                 81,
                 82,
                 85,
                 91,
                 92,
                 94,
                 103,
-                425,
-                426
+                426,
+                427
             ],
             [
                 88,
                 94,
-                425,
-                426
+                426,
+                427
             ],
             [
                 88,
-                425,
-                426
+                426,
+                427
             ],
             [
                 81,
                 82,
                 83,
                 91,
                 94,
                 110,
-                425,
-                426
+                426,
+                427
             ],
             [
-                421,
-                425,
-                426
+                422,
+                426,
+                427
             ],
             [
                 135,
                 296,
-                401,
-                420,
-                425,
-                426
+                402,
+                421,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 75,
-                339,
-                401,
-                425,
-                426
+                340,
+                402,
+                426,
+                427
             ],
             [
-                425,
                 426,
-                445,
+                427,
                 446,
-                447
+                447,
+                448
             ],
             [
                 135,
                 296,
-                425,
-                426
+                426,
+                427
             ],
             [
                 74,
                 296,
-                396,
-                401,
-                425,
-                426
+                397,
+                402,
+                426,
+                427
             ],
             [
                 135,
-                401,
-                425,
-                426
+                402,
+                426,
+                427
             ],
             [
                 302,
-                370,
-                401,
-                415,
-                417,
-                425,
-                426
+                371,
+                402,
+                416,
+                418,
+                426,
+                427
             ],
             [
-                370,
-                396,
-                401,
-                425,
-                426
+                371,
+                397,
+                402,
+                426,
+                427
             ],
             [
-                416,
                 417,
                 418,
                 419,
-                422,
+                420,
                 423,
-                425,
+                424,
                 426,
-                434,
-                441,
-                444,
-                448
+                427,
+                435,
+                442,
+                445,
+                449
             ],
             [
                 135,
-                346,
-                401,
-                425,
-                426
+                347,
+                402,
+                426,
+                427
             ],
             [
                 135,
-                416,
-                425,
-                426
+                417,
+                426,
+                427
             ],
             [
-                424,
                 425,
                 426,
                 427,
                 428,
                 429,
                 430,
                 431,
                 432,
-                433
+                433,
+                434
             ],
             [
-                346,
-                401,
-                416,
-                425,
-                426
+                347,
+                402,
+                417,
+                426,
+                427
             ],
             [
                 74,
-                401,
-                416,
-                425,
-                426
+                402,
+                417,
+                426,
+                427
             ],
             [
                 166,
-                346,
-                401,
-                416,
-                425,
-                426
+                347,
+                402,
+                417,
+                426,
+                427
             ],
             [
                 166,
-                346,
-                416,
-                425,
-                426
+                347,
+                417,
+                426,
+                427
             ],
             [
                 135,
-                425,
                 426,
-                435
+                427,
+                436
             ],
             [
-                425,
                 426,
-                435,
+                427,
                 436,
                 437,
                 438,
                 439,
-                440
+                440,
+                441
             ],
             [
-                425,
                 426,
-                435
+                427,
+                436
             ],
             [
-                370,
-                401,
-                425,
-                426
+                371,
+                402,
+                426,
+                427
             ],
             [
-                401,
-                425,
+                402,
                 426,
-                435
+                427,
+                436
             ],
             [
-                416,
-                425,
-                426
+                417,
+                426,
+                427
             ],
             [
-                425,
                 426,
-                442,
-                443
+                427,
+                443,
+                444
             ],
             [
                 151,
                 166,
-                346,
-                401,
-                425,
-                426
+                347,
+                402,
+                426,
+                427
             ],
             [
                 74,
-                401,
-                425,
-                426
+                402,
+                426,
+                427
             ],
             [
                 72,
                 74,
                 135,
-                339,
-                370,
-                396,
-                401,
-                416,
-                425,
-                426
+                340,
+                371,
+                397,
+                402,
+                417,
+                426,
+                427
             ],
             [
-                425,
                 426,
-                499,
+                427,
                 500,
-                501
+                501,
+                502
             ],
             [
-                401,
-                425,
+                402,
                 426,
-                499
+                427,
+                500
             ],
             [
-                401,
-                425,
-                426
+                402,
+                426,
+                427
             ],
             [
-                401,
-                425,
+                402,
                 426,
-                498
+                427,
+                499
             ],
             [
-                425,
                 426,
-                497
+                427,
+                498
             ],
             [
                 58,
                 72,
                 74,
                 131,
-                397,
-                425,
-                426
+                398,
+                426,
+                427
             ],
             [
                 58,
                 72,
                 74,
                 131,
                 199,
                 296,
-                346,
-                370,
-                396,
-                425,
-                426
+                347,
+                371,
+                397,
+                426,
+                427
             ],
             [
                 58,
                 72,
                 74,
                 131,
                 199,
-                396,
                 397,
-                425,
-                426
+                398,
+                426,
+                427
             ],
             [
                 72,
-                397,
-                425,
-                426
+                398,
+                426,
+                427
             ],
             [
                 48,
                 49,
                 50,
                 51,
                 52,
@@ -5522,144 +5527,144 @@
                 57,
                 58,
                 59,
                 60,
                 61,
                 62,
                 63,
-                397,
                 398,
                 399,
                 400,
-                425,
-                426
+                401,
+                426,
+                427
             ],
             [
                 151,
-                396,
-                401,
-                425,
+                397,
+                402,
                 426,
-                449
+                427,
+                450
             ],
             [
-                425,
                 426,
-                450,
-                479,
-                482,
-                485,
-                503,
-                506
+                427,
+                451,
+                480,
+                483,
+                486,
+                504,
+                507
             ],
             [
                 296,
-                396,
-                401,
-                425,
-                426
+                397,
+                402,
+                426,
+                427
             ],
             [
-                346,
-                370,
-                401,
-                415,
-                425,
+                347,
+                371,
+                402,
+                416,
                 426,
-                450,
-                456,
-                474,
-                477,
-                478
+                427,
+                451,
+                457,
+                475,
+                478,
+                479
             ],
             [
                 302,
-                370,
-                401,
+                371,
                 402,
-                415,
-                425,
+                403,
+                416,
                 426,
-                449,
-                496,
-                503,
-                505
+                427,
+                450,
+                497,
+                504,
+                506
             ],
             [
-                401,
-                425,
+                402,
                 426,
-                504
+                427,
+                505
             ],
             [
                 72,
                 74,
                 122,
-                401,
-                425,
-                426
+                402,
+                426,
+                427
             ],
             [
-                370,
-                401,
-                415,
-                425,
+                371,
+                402,
+                416,
                 426,
-                450,
-                456,
-                480,
-                481
+                427,
+                451,
+                457,
+                481,
+                482
             ],
             [
-                370,
-                401,
-                415,
-                425,
+                371,
+                402,
+                416,
                 426,
-                450,
-                456,
-                483,
-                484
+                427,
+                451,
+                457,
+                484,
+                485
             ],
             [
-                401,
-                425,
+                402,
                 426,
-                502
+                427,
+                503
             ],
             [
-                401
+                402
             ],
             [
                 151,
-                396,
-                401,
-                449
+                397,
+                402,
+                450
             ],
             [
-                401,
-                415,
-                450,
-                503
+                402,
+                416,
+                451,
+                504
             ],
             [
                 296,
-                396,
-                401
+                397,
+                402
             ],
             [
-                415
+                416
             ],
             [
-                401,
-                415
+                402,
+                416
             ],
             [
                 74,
-                401
+                402
             ]
         ],
         "fileInfos": [
             {
                 "affectsGlobalScope": true,
                 "version": "824cb491a40f7e8fdeb56f1df5edf91b23f3e3ee6b4cde84d4a99be32338faee"
             },
@@ -5862,39 +5867,39 @@
             "0f3ab64d7d7c82028025a8b1a9a0af7900f5746f4abd861882ec57d93dad394e",
             "980e589df7fa1e5c5faa5e98bd716e16f4cd544d50f8fa1837f67e80bcb29e69",
             "443278cb0834bee339cbdee9eb8303b5bfcdfd02d9b32ac1a237b6c7df437eaf",
             "02e8d6b9f3c89e7ad07c65a486c8387cf862a4c4e7c4d3cb7f51598c7ec057a6",
             "f3745a58f2bd7ed2c210e882e95b67d0707f97b9ed7b2431f68e5cccec0e20ba",
             "2435893282189602e1c3c5ae3f08a0129508c4ab3db3895c436525bd238ef2b6",
             "9ff7cb447d63e95594b2732f048834e458d0332014b39117123a6d8dda83e246",
-            "c86fb5bff522697115b31087201de6359c0d8828041e24ee980d4657d096c727",
+            "eb7375e005b02971567356809faeeecf14becb300aa9ca483fcd6c9f8aa80d8c",
             "e7c738913fab4ba4b00fcf1d1eb1ddf8989b64355da34250407340f4894a2384",
             "c871756fb890365824f416826bb7bb363b06c4aa48f1a99263c4fb75ab690b2d",
-            "4cc80e749273f8c64b9b574c76e6f4483f03faf1227e86a458deab754d9a4482",
+            "219657f1d170f05d7c1640dd36299a7e9d2554330adc500f4e11e875a2d9bc94",
             "431eef47c55a88198c1cc62ea7c9c7537c3219c3fd652c554d3d5bb7a63658a1",
             "ee5af755629403e296dcc1bb67c3d405ba2996eb2111ce0d6af5cf39df258e73",
             "16b311651dbd580d429938c993c41e1c610ef0b1e83c38229f3ad4d81a35cd39",
             "a45c8c0c99d344b9bdbdf836f3d8fb8a90a2b0adc6ecba2592593d7bcb28ec5f",
             "c39c1eb3c9ee9f208c595683a383ffee7b424848b6d662e79c08b4e6e74c79d6",
             "064733c01462ae496e7b62ffce6a3cb21facb351c0375b151ed66da38de60d69",
-            "302301b6291dc914d9eaa4defd4e8036d8430ff40650308b0ca20c5b2fd9d037",
-            "5164b9597b0d547779e0b5d59d9c64c1a97a5688199ea73c558ddcc7dec98cc0",
-            "08f1ca6a55e44fd247c3b84a9cd35f2d03fe92a087728221287533ff92f52a49",
-            "f5492cf939012c336f4ab84a2496e9e63bb56b42218664d08e3282220f400b2a",
-            "72c9b0f8c9ee268fe755eeab915e5b0897772244aa0ef11f59e15c50a6a55121",
+            "7097daf64b1ff790a73ff0ab39b4f23c1a75404d903714338dbcae9b47ba347c",
+            "bd8dc03b548c7081497d76abc21c97fadf0d768ccbb5860424406ca8d22433c6",
+            "4f1d88b42e347f1868a0bd8db7563bc54017c5112a6edb01d5617c342995fdc7",
+            "f1add31820a8e538ced1fa56092ad68adb998e0e48cecbf4e69b0638391fe5c5",
+            "a11c0481bbb4d82204954b2d83865b29878713af71d71e72bfb28e5c2138bcaa",
             "9577fb6c932b23da87716c2c48e7062346d169f5b5d47aed592328bb6a414aae",
-            "deb5dcff37bc6791471dfcfef1d164916029baf60c58f28f0f7ce73d402c7eeb",
-            "eedc5fb164c9d9107aa786a8f1b09220382323c7dca620dda2ec9b003c6bb656",
-            "ee32a122fe108f3fdc220cfbc0e7a2c6038f2ff0786e79a9dd7fa53cc845a87f",
+            "d980757560074d9746471db513531d87e7b756eb2263dd2c8bd187860bffa3b6",
+            "75c4e0aa4e6dd5efaeb4471455cd730c1c21baacdc60bb6d13ae87fd40a55625",
+            "186fb8b8765fecb459e5aeada1fa861170cb7689f89f46384ea0c3882b529c2d",
             "8249670da9c5c37d7cdd03576170536f4c3c9cdcfe8cf21df0bbb07a45e5f748",
             "d9b96d27372967e8f53b3f7b7cb6e875b8d128080abc4fa204a13f0d3f2b6506",
             "d41b65a0fb48a14a7b52eaa45d9b65988af076e63704cba1dd1f72e961e0e2f5",
             "92b40a9393f937e4bd7eed4b0161ad03296607bfdf26b0bb323cde18c51e0687",
             "fdcbabde604d3123e01b2dc359fe3a0d64e6c1563b8c6a27ec0d626f528f7670",
-            "7215a5c611e92a934a4280874c9844cd6b8dba4fd4523badc27203a60303c8ca",
+            "0b7a411df6f8e1e4eb3537abe3ff7df590300b1af856bdb6e167a54a4a54ca8a",
             "59217222f06b2b24784160c8e2eaf0de94906912505101576a1dd744fd90cdcf",
             "c60e185eaab239d465baec8e4a8c2f76fdff641431cb57d12c4e233d61be5474",
             "d8b6dc94bc2761afdcff7a1e29359a383472bd8af2ce03485a2792026f15f458",
             "1955442a305cd1622782ce89c898be431c66c39c36a253abb0543052f4917613",
             "2251d1a89b3d8aac866bc79839c28681886d289d117404276ecf1d4fd5f5c19c",
             "2a55511100028e4af650f52bdd7826fb187b9eee380b7ce9249a69f0713503fa",
             "8bdf3edd4e55c0167be8af39a89763628fba6d8670777f720957f080c2ce9a50",
@@ -5917,15 +5922,15 @@
                 "affectsGlobalScope": true,
                 "version": "55461596dc873b866911ef4e640fae4c39da7ac1fbc7ef5e649cb2f2fb42c349"
             },
             "8a8eb4ebffd85e589a1cc7c178e291626c359543403d58c9cd22b81fab5b1fb9",
             "247a952efd811d780e5630f8cfd76f495196f5fa74f6f0fee39ac8ba4a3c9800",
             {
                 "affectsGlobalScope": true,
-                "version": "8117d2726c78497306ceef07b4ccd08a863a9bd6e1fd7ff9ed6332f0e49bbb1a"
+                "version": "8ca4709dbd22a34bcc1ebf93e1877645bdb02ebd3f3d9a211a299a8db2ee4ba1"
             },
             "70134f200796978a596026e8113c4114815c2dfad8de968d4b92522076458a97",
             "2db1598bb162fbd038338fd92e405681c300d93e016e465e55249503e096ed5f",
             "55a8b93f44a188af9f50623245baecd09cb8dd84f4450f772718cfbf3d74dc6e",
             "1f7f96ce3335beab9ab0ffa1cee5f29a07d03f6438a638f7833e20c875cb1f17",
             "cb8c899eceb8657773a0c22aa08445db31229fa1c0d801b25f1d0d740178edc7",
             "d1566bbd806610bb864c414ee85043155e6be9409d5cb7af54d5f334a97740a3",
@@ -6086,15 +6091,16 @@
             "11fc68bda6e4b7d30fc377346f1cbd0ffb9d637fd9adbf3e190f65f82679940f",
             "a56cd8e25d118a1518e05fcad9e391427ef504078403ea0dd6d44fb7d1013023",
             "6df7d57b493d75ff66e426f15a53e428d4d77c60fbded8591cd13ffef8efd40b",
             "52e936849e598306fe1f929bde30881b9b92cf3a0caaf70963f69978d0089bbe",
             "643900082d10e2ea2309a88d5cc3db02583e822e9e0cd3525ad1ff77c9d88433",
             "e2bfb86488150c78cea78c2b726a3bd81c9a2053a5d56916beed898d4dc7f5b5",
             "c2d417bfcfb62ed2101db6175ea83f91b2656ada1397d4abaf8c7681c42fb534",
-            "ab85206fe068194d70b200f8e7571990187ee0e7df8d71a9cb34efc475014517",
+            "42c169fb8c2d42f4f668c624a9a11e719d5d07dacbebb63cbcf7ef365b0a75b3",
+            "cb14e0ba947dced2842507d6457a6b7e08c888beaf0702f08af107b1a76fad84",
             "13dc13295d9c20a110f85403e9129e263f7ca08a576aad19fa26344d451d5f0f",
             "ceb76f8a9524b92d1a09d17239734eabb73274a7cebe48136f71e70aae65f5d1",
             "2bf405f8a5b25539b485e40e6b9db1c130f8e0750acb98d8563e4ced0e656f5a",
             "2d4484c320e5df4d0d6b1d3e49db9bccc4fe11c5d8decec874d15525e1acba41",
             "381899b8d1d4c1be716f18cb5242ba39f66f4b1e31d45af62a32a99f8edcb39d",
             "07e05f7848cbab3cd06298fd5ec3e2c2ac106c6c76b2233d667bd04b49109ed1",
             "a91d1b1373de9d8a1f498b496fe1a41f07cd3e5a0a28b1d920a14284404acb91",
@@ -6180,15 +6186,15 @@
             "1b162dfbafe3d183e089c97e1105ec93f9f102517977d0ef2322c32fb1ae69b3",
             "25fdcfcf217efc4a1ce16b1b87ba4b9de850706512f038a286cd00da9aee0c9b",
             "e087fcd41297b51f643ec14daed135350edd42517292c172837d3bb0f445a001",
             "4ed051e63cb4e713c8629ddb425b61b4acaac453183994a78187346f86f5c635",
             "1d24d23d670fbc3763013f9341a7a376499e8a4f2a35f24b008535d133101cd6",
             "15301c8c565b8581e9fd2b5524f4562ac204ad3e939125a850a8ba98aa151be0",
             "dc63de5eb376f0d81b06149ccb2da01a3a5a21cc3eca641ff5319ca6c048672e",
-            "e87bf3a17f2ba157837dfdd8f2a8ab67be222ea362c9e87447b1cf07b686bb37",
+            "f4ee3318129f694f6e6892e14a6b35b82e9cc3efc5c54a184f37192900cfc6e2",
             "e44a13a7be4eed59adc9bd3a26167425df44e45cd3a7cef0ad18b9d9d3d4bf87",
             "fe6c594baff933c3d6f1cb80d0db05bab273b61ce8cf39e03d9d87ced00efb1b",
             "81d2576b03c68c38c81c7d2a1cd5c8ad3b1683298bfb703a8c4dd2b31fa0e1e2",
             "3daafd119d681097f0172dd4defb4e46fc687a0b3f9ad8840b632f55421e06f1",
             {
                 "signature": "78504a274642f4915a309c3108811f9ec837e4bdfe5e3411322555b30d1a1e19",
                 "version": "f75682cd4e31159bf78af61c388a7149a394d131bd1b0742f0e7ee198f013bcb"
@@ -6206,16 +6212,16 @@
             "becb1ba9752bab39612cd77eaf3140cca067ff0a1e651dc2b1242caf007e08b0",
             "9c554facd42b92c91cba6e487e9b9f6d012a1ea61a6d64096748e38f0946e7a7",
             "c9258d5692cbee696190eb474b532ac5069011d13f7be2ffa9af1f72f20afb5a",
             "cf3cbaee880ea25a8440feb8c49554e4d656ec003e2a7d82799a811c91bc920d",
             "9b09f3820a22f432dd59a447574b6e29aa27b24efc817024f40404c315300c4d",
             "86fbc20c92f731d0493b083291601491a93e73a3fdff9e4d25ade2458572c21e",
             "9f021433d0dcf255a95c0ccd312a6b7ea32458365dbc30d2390257cfad374630",
-            "14c1ba615330caba1a7f24bc8ed4ddbcfbe05a8750ee3691a99505b18b7605ca",
-            "967b1bfbb1eaa1d394465232c542bae781dcbd1aa9865a9da753c3c0ca51f032",
+            "c68f00de76bf6ae3fc56a91b8339752ee56e38156e86ad7a7f83bf28c8a042f6",
+            "0c5fb1444f03120ac052b31ed702b34caa9fdc3f894cbe62edc4dfccbb484a3e",
             "f0c4d7cd3054bf45245ab53a73336311100707472665c5b7fc90e5df7c7e795f",
             "aff801ef4268090333d6907db4fb1e1d286fbf8467283d4ee58f78d3f805c3b3",
             "43e7862403a3a325288bd4108fcb1d76d42c57fefb2a660eb46d1c1df356dbb4",
             "a81498798cca946eeaec5844059412baaca219eee731de4bb054b02faa26b8f5",
             "64a8c63ee138480e609ef6c9579c010dc0a902b61085a40f77a78b3f316cac78",
             "15afdb5ca062ea5473867906de2944f3ed87a8621e428ca60ea3a19075903cf9",
             "0d61c1d4612557df3c9d438d2614fb9286e1cf748c726321a2998b483426ac23",
@@ -6313,22 +6319,22 @@
             "ee0760073f06433deaaa0d6f99b16cfe02dc76f948af1dd3e3131ba96ecc0239",
             "a929551e028e45fc1767413db1a01b084a492089e61d04a4c2a5982f207053ee",
             "1b2b9d78e7ce48b7f04ffee25104b79377eb7ccf264f3e1faf0185c8ff3dc2ee",
             "f3c17ff965e9a69df7d433482ff29449cbec9437f5d745ab352b5888298a6473",
             "f6be97b35d86c8b32bce65be01928b595d5dd019d04ebb7df71533a4aa3b1203",
             "c06e01a405cdc998d2870e2fd0cf16c176a57c691aa8e37b6d93cb1c6be64c28",
             "87c0b22add5a37e232c2597eff729947967d90a10bc44c460e6c5bd8421f2689",
-            "e3643474c1823585fb7b0ab772a17c668faa6bb6ad1e18254956d6d3e1a615c3",
+            "affd504cffb5d74447a889f6a25c2c72c2142c32849cd174fe5f33d69888f485",
             "3fdee1fdcbf954cdc5c4e84928f10f8d65c8cbde9db953e1cb0538bddf2f2331",
             "28cd8d1f6bb01be3681b2e82b03dfc9b0d796117762f9af7a9a0e17f21cd9cce",
             {
                 "signature": "ff98c70b5486ea9a33e433a36353094b70abcc1394cd59751e5fc48cb07c8362",
                 "version": "1ee7b1bf627087baa464397169e9f45d6a07e797164444e2ca2016bab1e24695"
             },
-            "2b9acc85b8a75a1720300c969831f4fc6be44c4edbeba81286168ee262584512",
+            "cfb84aaaa90bb4229e569a3f075ce83deaabd0a35a76bbc570f78b31fa26becd",
             {
                 "signature": "94f153dc366146b0b048372c38272a6189b5b18aee07ca6bba98f6f67ad28514",
                 "version": "09e72ffbe0d4f37f8aeaef3cceb166fed8598f8bd1217d93fb789d8f1721db4f"
             },
             {
                 "signature": "05c6dd04dae483ac84b2505ec19ea5ca902d31472f34c6e0f048ad3ccee6e7a4",
                 "version": "d2e394b11d5d2680edec1c830cf1d7279f3a5d1dff79f5e1e3b7091f2fe5fbe2"
@@ -6766,14 +6772,15 @@
             "../../node_modules/@jupyterlab/services/lib/index.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/tokens.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/base.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/gettext.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/manager.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/server.d.ts",
             "../../node_modules/@jupyterlab/translation/lib/index.d.ts",
+            "../../node_modules/@types/react/jsx-runtime.d.ts",
             "../../node_modules/@jupyterlab/ui-components/node_modules/@rjsf/core/lib/components/Form.d.ts",
             "../../node_modules/@jupyterlab/ui-components/node_modules/@rjsf/core/lib/withTheme.d.ts",
             "../../node_modules/@jupyterlab/ui-components/node_modules/@rjsf/core/lib/getDefaultRegistry.d.ts",
             "../../node_modules/@jupyterlab/ui-components/node_modules/@rjsf/core/lib/index.d.ts",
             "../../node_modules/@jupyterlab/ui-components/lib/components/form.d.ts",
             "../../node_modules/csstype/index.d.ts",
             "../../node_modules/typestyle/lib/types.d.ts",
@@ -7080,39 +7087,39 @@
             "strict": true,
             "strictNullChecks": true,
             "strictPropertyInitialization": false,
             "target": 4
         },
         "referencedMap": [
             [
-                371,
+                372,
                 1
             ],
             [
-                425,
+                426,
                 2
             ],
             [
-                453,
+                454,
                 3
             ],
             [
-                456,
+                457,
                 4
             ],
             [
-                452,
+                453,
                 5
             ],
             [
-                454,
+                455,
                 6
             ],
             [
-                455,
+                456,
                 7
             ],
             [
                 76,
                 8
             ],
             [
@@ -7144,191 +7151,191 @@
                 15
             ],
             [
                 126,
                 16
             ],
             [
-                406,
+                407,
                 17
             ],
             [
-                404,
+                405,
                 18
             ],
             [
-                415,
+                416,
                 19
             ],
             [
-                410,
+                411,
                 20
             ],
             [
-                407,
+                408,
                 21
             ],
             [
-                411,
+                412,
                 22
             ],
             [
-                412,
+                413,
                 23
             ],
             [
-                408,
+                409,
                 24
             ],
             [
-                409,
+                410,
                 25
             ],
             [
-                405,
+                406,
                 26
             ],
             [
-                413,
+                414,
                 27
             ],
             [
-                414,
+                415,
                 28
             ],
             [
-                353,
+                354,
                 27
             ],
             [
-                354,
+                355,
                 29
             ],
             [
-                355,
+                356,
                 30
             ],
             [
-                357,
+                358,
                 31
             ],
             [
-                358,
+                359,
                 1
             ],
             [
-                370,
+                371,
                 32
             ],
             [
-                359,
+                360,
                 33
             ],
             [
-                360,
+                361,
                 34
             ],
             [
-                362,
+                363,
                 35
             ],
             [
-                363,
+                364,
                 36
             ],
             [
-                364,
+                365,
                 37
             ],
             [
-                361,
+                362,
                 38
             ],
             [
-                365,
+                366,
                 39
             ],
             [
-                366,
+                367,
                 40
             ],
             [
-                367,
+                368,
                 38
             ],
             [
-                347,
+                348,
                 41
             ],
             [
-                368,
+                369,
                 42
             ],
             [
-                348,
+                349,
                 43
             ],
             [
-                349,
+                350,
                 44
             ],
             [
-                352,
+                353,
                 45
             ],
             [
-                350,
+                351,
                 46
             ],
             [
-                351,
+                352,
                 47
             ],
             [
-                356,
+                357,
                 48
             ],
             [
-                369,
+                370,
                 49
             ],
             [
-                372,
+                373,
                 50
             ],
             [
-                373,
+                374,
                 51
             ],
             [
-                380,
+                381,
                 52
             ],
             [
-                374,
+                375,
                 53
             ],
             [
-                375,
+                376,
                 54
             ],
             [
-                376,
+                377,
                 55
             ],
             [
-                377,
+                378,
                 56
             ],
             [
-                378,
+                379,
                 57
             ],
             [
-                379,
+                380,
                 58
             ],
             [
                 189,
                 59
             ],
             [
@@ -7368,235 +7375,235 @@
                 1
             ],
             [
                 198,
                 27
             ],
             [
-                457,
+                458,
                 62
             ],
             [
-                464,
+                465,
                 63
             ],
             [
-                460,
+                461,
                 64
             ],
             [
-                461,
+                462,
                 65
             ],
             [
-                462,
+                463,
                 66
             ],
             [
-                463,
+                464,
                 67
             ],
             [
-                458,
+                459,
                 68
             ],
             [
-                459,
+                460,
                 69
             ],
             [
-                395,
+                396,
                 70
             ],
             [
-                382,
+                383,
                 71
             ],
             [
-                383,
+                384,
                 72
             ],
             [
-                396,
+                397,
                 73
             ],
             [
-                394,
+                395,
                 74
             ],
             [
-                381,
+                382,
                 75
             ],
             [
-                469,
+                470,
                 76
             ],
             [
-                466,
+                467,
                 77
             ],
             [
-                474,
+                475,
                 78
             ],
             [
-                468,
+                469,
                 79
             ],
             [
-                465,
+                466,
                 80
             ],
             [
-                470,
+                471,
                 81
             ],
             [
-                471,
+                472,
                 82
             ],
             [
-                472,
+                473,
                 83
             ],
             [
-                473,
+                474,
                 84
             ],
             [
-                477,
+                478,
                 85
             ],
             [
-                475,
+                476,
                 86
             ],
             [
-                476,
+                477,
                 87
             ],
             [
-                486,
+                487,
                 88
             ],
             [
-                487,
+                488,
                 88
             ],
             [
-                488,
+                489,
                 88
             ],
             [
-                496,
+                497,
                 89
             ],
             [
-                489,
+                490,
                 88
             ],
             [
-                495,
+                496,
                 90
             ],
             [
-                490,
+                491,
                 88
             ],
             [
-                491,
+                492,
                 91
             ],
             [
-                492,
+                493,
                 91
             ],
             [
-                494,
+                495,
                 92
             ],
             [
-                493,
+                494,
                 88
             ],
             [
                 73,
                 27
             ],
             [
-                339,
+                340,
                 93
             ],
             [
-                338,
+                339,
                 94
             ],
             [
-                334,
+                335,
                 95
             ],
             [
-                336,
+                337,
                 59
             ],
             [
-                333,
+                334,
                 96
             ],
             [
-                335,
+                336,
                 96
             ],
             [
-                337,
+                338,
                 97
             ],
             [
                 168,
                 98
             ],
             [
-                384,
+                385,
                 99
             ],
             [
-                385,
+                386,
                 40
             ],
             [
-                393,
+                394,
                 100
             ],
             [
-                386,
+                387,
                 1
             ],
             [
-                387,
+                388,
                 101
             ],
             [
-                388,
+                389,
                 99
             ],
             [
-                390,
+                391,
                 102
             ],
             [
-                391,
+                392,
                 103
             ],
             [
-                389,
+                390,
                 104
             ],
             [
-                392,
+                393,
                 105
             ],
             [
                 183,
                 106
             ],
             [
@@ -7772,163 +7779,163 @@
                 145
             ],
             [
                 297,
                 146
             ],
             [
-                345,
+                346,
                 147
             ],
             [
                 136,
                 148
             ],
             [
                 167,
                 149
             ],
             [
-                307,
+                308,
                 150
             ],
             [
-                320,
+                321,
                 151
             ],
             [
-                321,
+                322,
                 38
             ],
             [
-                341,
+                342,
                 152
             ],
             [
-                322,
+                323,
                 153
             ],
             [
-                319,
+                320,
                 1
             ],
             [
-                323,
+                324,
                 154
             ],
             [
-                326,
+                327,
                 155
             ],
             [
-                327,
+                328,
                 156
             ],
             [
-                328,
+                329,
                 157
             ],
             [
-                329,
+                330,
                 30
             ],
             [
-                330,
+                331,
                 1
             ],
             [
-                331,
+                332,
                 158
             ],
             [
-                332,
+                333,
                 148
             ],
             [
-                325,
+                326,
                 159
             ],
             [
-                324,
+                325,
                 160
             ],
             [
-                340,
+                341,
                 161
             ],
             [
-                342,
+                343,
                 1
             ],
             [
-                313,
+                314,
                 162
             ],
             [
-                318,
+                319,
                 163
             ],
             [
-                312,
+                313,
                 164
             ],
             [
-                314,
+                315,
                 165
             ],
             [
-                317,
+                318,
                 166
             ],
             [
-                315,
+                316,
                 167
             ],
             [
-                316,
+                317,
                 168
             ],
             [
-                346,
+                347,
                 169
             ],
             [
-                310,
+                311,
                 170
             ],
             [
-                311,
+                312,
                 171
             ],
             [
-                343,
+                344,
                 172
             ],
             [
-                344,
+                345,
                 1
             ],
             [
-                303,
+                304,
                 173
             ],
             [
-                305,
+                306,
                 174
             ],
             [
-                306,
+                307,
                 175
             ],
             [
-                304,
+                305,
                 176
             ],
             [
-                403,
+                404,
                 177
             ],
             [
                 151,
                 178
             ],
             [
@@ -7968,15 +7975,15 @@
                 1
             ],
             [
                 75,
                 61
             ],
             [
-                467,
+                468,
                 182
             ],
             [
                 137,
                 1
             ],
             [
@@ -8404,227 +8411,227 @@
                 210
             ],
             [
                 210,
                 1
             ],
             [
-                508,
+                509,
                 218
             ],
             [
-                509,
+                510,
                 218
             ],
             [
-                544,
+                545,
                 219
             ],
             [
-                545,
+                546,
                 220
             ],
             [
-                546,
+                547,
                 221
             ],
             [
-                547,
+                548,
                 222
             ],
             [
-                548,
+                549,
                 223
             ],
             [
-                549,
+                550,
                 224
             ],
             [
-                550,
+                551,
                 225
             ],
             [
-                551,
+                552,
                 226
             ],
             [
-                552,
+                553,
                 227
             ],
             [
-                553,
+                554,
                 228
             ],
             [
-                554,
+                555,
                 228
             ],
             [
-                556,
+                557,
                 229
             ],
             [
-                555,
+                556,
                 230
             ],
             [
-                557,
+                558,
                 231
             ],
             [
-                558,
+                559,
                 232
             ],
             [
-                559,
+                560,
                 233
             ],
             [
-                543,
+                544,
                 234
             ],
             [
-                593,
+                594,
                 1
             ],
             [
-                560,
+                561,
                 235
             ],
             [
-                561,
+                562,
                 236
             ],
             [
-                562,
+                563,
                 237
             ],
             [
-                594,
+                595,
                 238
             ],
             [
-                563,
+                564,
                 239
             ],
             [
-                564,
+                565,
                 240
             ],
             [
-                565,
+                566,
                 241
             ],
             [
-                566,
+                567,
                 242
             ],
             [
-                567,
+                568,
                 243
             ],
             [
-                568,
+                569,
                 244
             ],
             [
-                569,
+                570,
                 245
             ],
             [
-                570,
+                571,
                 246
             ],
             [
-                571,
+                572,
                 247
             ],
             [
-                572,
+                573,
                 248
             ],
             [
-                573,
+                574,
                 248
             ],
             [
-                574,
+                575,
                 249
             ],
             [
-                575,
+                576,
                 250
             ],
             [
-                577,
+                578,
                 251
             ],
             [
-                576,
+                577,
                 252
             ],
             [
-                578,
+                579,
                 253
             ],
             [
-                579,
+                580,
                 254
             ],
             [
-                580,
+                581,
                 255
             ],
             [
-                581,
+                582,
                 256
             ],
             [
-                582,
+                583,
                 257
             ],
             [
-                583,
+                584,
                 258
             ],
             [
-                584,
+                585,
                 259
             ],
             [
-                585,
+                586,
                 260
             ],
             [
-                586,
+                587,
                 261
             ],
             [
-                587,
+                588,
                 262
             ],
             [
-                588,
+                589,
                 263
             ],
             [
-                589,
+                590,
                 264
             ],
             [
-                590,
+                591,
                 265
             ],
             [
-                591,
+                592,
                 266
             ],
             [
-                592,
+                593,
                 267
             ],
             [
                 134,
                 1
             ],
             [
@@ -8632,23 +8639,27 @@
                 1
             ],
             [
                 135,
                 268
             ],
             [
+                303,
+                148
+            ],
+            [
                 133,
                 1
             ],
             [
-                510,
+                511,
                 1
             ],
             [
-                308,
+                309,
                 1
             ],
             [
                 80,
                 1
             ],
             [
@@ -8848,151 +8859,151 @@
                 1
             ],
             [
                 9,
                 1
             ],
             [
-                309,
+                310,
                 269
             ],
             [
-                526,
+                527,
                 270
             ],
             [
-                533,
+                534,
                 271
             ],
             [
-                525,
+                526,
                 270
             ],
             [
-                540,
+                541,
                 272
             ],
             [
-                517,
+                518,
                 273
             ],
             [
-                516,
+                517,
                 274
             ],
             [
-                539,
+                540,
                 275
             ],
             [
-                534,
+                535,
                 276
             ],
             [
-                537,
+                538,
                 277
             ],
             [
-                519,
+                520,
                 278
             ],
             [
-                518,
+                519,
                 279
             ],
             [
-                514,
+                515,
                 280
             ],
             [
-                513,
+                514,
                 281
             ],
             [
-                536,
+                537,
                 282
             ],
             [
-                515,
+                516,
                 283
             ],
             [
-                520,
+                521,
                 284
             ],
             [
-                521,
+                522,
                 1
             ],
             [
-                524,
+                525,
                 284
             ],
             [
-                511,
+                512,
                 1
             ],
             [
-                542,
+                543,
                 285
             ],
             [
-                541,
+                542,
                 284
             ],
             [
-                528,
+                529,
                 286
             ],
             [
-                529,
+                530,
                 287
             ],
             [
-                531,
+                532,
                 288
             ],
             [
-                527,
+                528,
                 289
             ],
             [
-                530,
+                531,
                 290
             ],
             [
-                535,
+                536,
                 275
             ],
             [
-                522,
+                523,
                 291
             ],
             [
-                523,
+                524,
                 292
             ],
             [
-                532,
+                533,
                 293
             ],
             [
-                512,
+                513,
                 294
             ],
             [
-                538,
+                539,
                 295
             ],
             [
                 124,
                 296
             ],
             [
-                451,
+                452,
                 297
             ],
             [
                 122,
                 298
             ],
             [
@@ -9156,167 +9167,167 @@
                 329
             ],
             [
                 111,
                 330
             ],
             [
-                422,
+                423,
                 331
             ],
             [
-                421,
+                422,
                 332
             ],
             [
-                420,
+                421,
                 333
             ],
             [
-                448,
+                449,
                 334
             ],
             [
-                447,
+                448,
                 335
             ],
             [
-                445,
+                446,
                 336
             ],
             [
-                446,
+                447,
                 337
             ],
             [
-                418,
+                419,
                 338
             ],
             [
-                419,
+                420,
                 339
             ],
             [
-                449,
+                450,
                 340
             ],
             [
-                424,
+                425,
                 341
             ],
             [
-                427,
+                428,
                 342
             ],
             [
-                428,
+                429,
                 38
             ],
             [
-                434,
+                435,
                 343
             ],
             [
-                429,
+                430,
                 344
             ],
             [
-                430,
+                431,
                 345
             ],
             [
-                431,
+                432,
                 346
             ],
             [
-                432,
+                433,
                 347
             ],
             [
-                433,
+                434,
                 344
             ],
             [
-                436,
+                437,
                 348
             ],
             [
-                441,
+                442,
                 349
             ],
             [
-                437,
+                438,
                 350
             ],
             [
-                438,
+                439,
                 351
             ],
             [
-                439,
+                440,
                 352
             ],
             [
-                440,
+                441,
                 348
             ],
             [
-                435,
+                436,
                 353
             ],
             [
-                444,
+                445,
                 354
             ],
             [
-                442,
+                443,
                 337
             ],
             [
-                443,
+                444,
                 355
             ],
             [
-                423,
+                424,
                 91
             ],
             [
-                416,
+                417,
                 356
             ],
             [
-                417,
+                418,
                 357
             ],
             [
-                426,
+                427,
                 2
             ],
             [
-                502,
+                503,
                 358
             ],
             [
-                500,
+                501,
                 359
             ],
             [
-                501,
+                502,
                 360
             ],
             [
-                499,
+                500,
                 361
             ],
             [
-                498,
+                499,
                 362
             ],
             [
-                497,
+                498,
                 1
             ],
             [
                 48,
                 1
             ],
             [
@@ -9344,15 +9355,15 @@
                 1
             ],
             [
                 51,
                 1
             ],
             [
-                504,
+                505,
                 1
             ],
             [
                 56,
                 1
             ],
             [
@@ -9380,232 +9391,232 @@
                 1
             ],
             [
                 62,
                 1
             ],
             [
-                399,
+                400,
                 363
             ],
             [
-                397,
+                398,
                 364
             ],
             [
-                398,
+                399,
                 365
             ],
             [
-                400,
+                401,
                 366
             ],
             [
-                401,
+                402,
                 367
             ],
             [
-                402,
+                403,
                 360
             ],
             [
-                450,
+                451,
                 368
             ],
             [
-                507,
+                508,
                 369
             ],
             [
-                478,
+                479,
                 370
             ],
             [
-                479,
+                480,
                 371
             ],
             [
-                506,
+                507,
                 372
             ],
             [
-                505,
+                506,
                 373
             ],
             [
-                481,
+                482,
                 374
             ],
             [
-                480,
+                481,
                 370
             ],
             [
-                482,
+                483,
                 375
             ],
             [
-                484,
+                485,
                 374
             ],
             [
-                483,
+                484,
                 370
             ],
             [
-                485,
+                486,
                 376
             ],
             [
-                503,
+                504,
                 377
             ]
         ],
         "root": [
-            402,
-            450,
+            403,
+            451,
             [
-                478,
-                485
+                479,
+                486
             ],
-            503,
+            504,
             [
-                505,
-                507
+                506,
+                508
             ]
         ],
         "semanticDiagnosticsPerFile": [
-            371,
-            425,
-            453,
-            456,
-            452,
+            372,
+            426,
             454,
+            457,
+            453,
             455,
+            456,
             76,
             125,
             131,
             123,
             129,
             127,
             128,
             130,
             126,
-            406,
-            404,
-            415,
-            410,
             407,
+            405,
+            416,
             411,
-            412,
             408,
-            409,
-            405,
+            412,
             413,
+            409,
+            410,
+            406,
             414,
-            353,
+            415,
             354,
             355,
-            357,
+            356,
             358,
-            370,
             359,
+            371,
             360,
-            362,
+            361,
             363,
             364,
-            361,
             365,
+            362,
             366,
             367,
-            347,
             368,
             348,
+            369,
             349,
-            352,
             350,
+            353,
             351,
-            356,
-            369,
-            372,
+            352,
+            357,
+            370,
             373,
-            380,
             374,
+            381,
             375,
             376,
             377,
             378,
             379,
+            380,
             189,
             199,
             190,
             191,
             192,
             193,
             194,
             195,
             196,
             197,
             198,
-            457,
-            464,
-            460,
+            458,
+            465,
             461,
             462,
             463,
-            458,
+            464,
             459,
+            460,
+            396,
+            383,
+            384,
+            397,
             395,
             382,
-            383,
-            396,
-            394,
-            381,
+            470,
+            467,
+            475,
             469,
             466,
-            474,
-            468,
-            465,
-            470,
             471,
             472,
             473,
-            477,
-            475,
+            474,
+            478,
             476,
-            486,
+            477,
             487,
             488,
-            496,
             489,
-            495,
+            497,
             490,
+            496,
             491,
             492,
-            494,
             493,
+            495,
+            494,
             73,
+            340,
             339,
-            338,
-            334,
-            336,
-            333,
             335,
             337,
+            334,
+            336,
+            338,
             168,
-            384,
             385,
-            393,
             386,
+            394,
             387,
             388,
-            390,
-            391,
             389,
+            391,
             392,
+            390,
+            393,
             183,
             187,
             184,
             185,
             186,
             296,
             179,
@@ -9643,64 +9654,64 @@
             207,
             298,
             299,
             302,
             300,
             301,
             297,
-            345,
+            346,
             136,
             167,
-            307,
-            320,
+            308,
             321,
-            341,
             322,
-            319,
+            342,
             323,
-            326,
+            320,
+            324,
             327,
             328,
             329,
             330,
             331,
             332,
+            333,
+            326,
             325,
-            324,
-            340,
-            342,
-            313,
-            318,
-            312,
+            341,
+            343,
             314,
-            317,
+            319,
+            313,
             315,
+            318,
             316,
-            346,
-            310,
+            317,
+            347,
             311,
-            343,
+            312,
             344,
-            303,
-            305,
-            306,
+            345,
             304,
-            403,
+            306,
+            307,
+            305,
+            404,
             151,
             68,
             72,
             64,
             65,
             66,
             70,
             69,
             67,
             71,
             75,
-            467,
+            468,
             137,
             174,
             172,
             173,
             74,
             138,
             144,
@@ -9801,74 +9812,75 @@
             260,
             212,
             261,
             262,
             263,
             264,
             210,
-            508,
             509,
-            544,
+            510,
             545,
             546,
             547,
             548,
             549,
             550,
             551,
             552,
             553,
             554,
-            556,
             555,
             557,
+            556,
             558,
             559,
-            543,
-            593,
             560,
+            544,
+            594,
             561,
             562,
-            594,
             563,
+            595,
             564,
             565,
             566,
             567,
             568,
             569,
             570,
             571,
             572,
             573,
             574,
             575,
-            577,
             576,
             578,
+            577,
             579,
             580,
             581,
             582,
             583,
             584,
             585,
             586,
             587,
             588,
             589,
             590,
             591,
             592,
+            593,
             134,
             132,
             135,
+            303,
             133,
-            510,
-            308,
+            511,
+            309,
             80,
             79,
             77,
             78,
             46,
             47,
             8,
@@ -9912,49 +9924,49 @@
             39,
             40,
             41,
             42,
             1,
             45,
             9,
-            309,
+            310,
+            527,
+            534,
             526,
-            533,
-            525,
-            540,
+            541,
+            518,
             517,
-            516,
-            539,
-            534,
-            537,
+            540,
+            535,
+            538,
+            520,
             519,
-            518,
-            514,
-            513,
-            536,
             515,
-            520,
+            514,
+            537,
+            516,
             521,
-            524,
-            511,
+            522,
+            525,
+            512,
+            543,
             542,
-            541,
-            528,
             529,
-            531,
-            527,
             530,
-            535,
-            522,
-            523,
             532,
-            512,
-            538,
+            528,
+            531,
+            536,
+            523,
+            524,
+            533,
+            513,
+            539,
             124,
-            451,
+            452,
             122,
             121,
             90,
             118,
             112,
             113,
             114,
@@ -9989,86 +10001,86 @@
             82,
             81,
             84,
             105,
             106,
             107,
             111,
+            423,
             422,
             421,
-            420,
+            449,
             448,
-            447,
-            445,
             446,
-            418,
+            447,
             419,
-            449,
-            424,
-            427,
+            420,
+            450,
+            425,
             428,
-            434,
             429,
+            435,
             430,
             431,
             432,
             433,
-            436,
-            441,
+            434,
             437,
+            442,
             438,
             439,
             440,
-            435,
-            444,
-            442,
+            441,
+            436,
+            445,
             443,
-            423,
-            416,
+            444,
+            424,
             417,
-            426,
+            418,
+            427,
+            503,
+            501,
             502,
             500,
-            501,
             499,
             498,
-            497,
             48,
             49,
             50,
             52,
             53,
             54,
             55,
             51,
-            504,
+            505,
             56,
             57,
             58,
             59,
             63,
             60,
             61,
             62,
-            399,
-            397,
-            398,
             400,
+            398,
+            399,
             401,
             402,
-            450,
-            507,
-            478,
+            403,
+            451,
+            508,
             479,
-            506,
-            505,
-            481,
             480,
+            507,
+            506,
             482,
-            484,
+            481,
             483,
             485,
-            503
+            484,
+            486,
+            504
         ]
     },
     "version": "5.4.5"
 }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/__init__.py` & `jupytercad_core-2.0.0a7/jupytercad_core/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/handlers.py` & `jupytercad_core-2.0.0a7/jupytercad_core/handlers.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/jcad_ydoc.py` & `jupytercad_core-2.0.0a7/jupytercad_core/jcad_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/step_ydoc.py` & `jupytercad_core-2.0.0a7/jupytercad_core/step_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/stl_ydoc.py` & `jupytercad_core-2.0.0a7/jupytercad_core/stl_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/package.json` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9721527777777779%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.7', '@jupytercad/occ-worker': "*

 * *                   "'^2.0.0-alpha.7', '@jupytercad/schema': '^2.0.0-alpha.7'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0e4fbdda31fcefbd6536.js'}}",*

 * * "'version'": "'2.0.0-alpha.7'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.6",
-        "@jupytercad/occ-worker": "^2.0.0-alpha.6",
-        "@jupytercad/schema": "^2.0.0-alpha.6",
+        "@jupytercad/base": "^2.0.0-alpha.7",
+        "@jupytercad/occ-worker": "^2.0.0-alpha.7",
+        "@jupytercad/schema": "^2.0.0-alpha.7",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
@@ -40,15 +40,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupytercad/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.42b7768c40743ee87403.js",
+            "load": "static/remoteEntry.0e4fbdda31fcefbd6536.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupytercad_core"
                 },
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.6"
+    "version": "2.0.0-alpha.7"
 }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/201.0c67a92e1b3da08ee0d5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -517,15 +517,15 @@
                                     }) {
                                         return `${this.lhs} = ${this.rhs};` + e
                                     }
                                     optimizeNames(e, t) {
                                         if (!(this.lhs instanceof n.Name) || e[this.lhs.str] || this.sideEffects) return this.rhs = O(this.rhs, e, t), this
                                     }
                                     get names() {
-                                        return x(this.lhs instanceof n.Name ? {} : {
+                                        return A(this.lhs instanceof n.Name ? {} : {
                                             ...this.lhs.names
                                         }, this.rhs)
                                     }
                                 }
                                 class l extends u {
                                     constructor(e, t, r, n) {
                                         super(e, r, n), this.op = t
@@ -614,15 +614,15 @@
                                         for (; n--;) {
                                             const o = r[n];
                                             o.optimizeNames(e, t) || (N(e, o.names), r.splice(n, 1))
                                         }
                                         return r.length > 0 ? this : void 0
                                     }
                                     get names() {
-                                        return this.nodes.reduce(((e, t) => A(e, t.names)), {})
+                                        return this.nodes.reduce(((e, t) => x(e, t.names)), {})
                                     }
                                 }
                                 class y extends m {
                                     render(e) {
                                         return "{" + e._n + super.render(e) + "}" + e._n
                                     }
                                 }
@@ -650,15 +650,15 @@
                                     }
                                     optimizeNames(e, t) {
                                         var r;
                                         if (this.else = null === (r = this.else) || void 0 === r ? void 0 : r.optimizeNames(e, t), super.optimizeNames(e, t) || this.else) return this.condition = O(this.condition, e, t), this
                                     }
                                     get names() {
                                         const e = super.names;
-                                        return x(e, this.condition), this.else && A(e, this.else.names), e
+                                        return A(e, this.condition), this.else && x(e, this.else.names), e
                                     }
                                 }
                                 w.kind = "if";
                                 class _ extends y {}
                                 _.kind = "for";
                                 class b extends _ {
                                     constructor(e) {
@@ -667,15 +667,15 @@
                                     render(e) {
                                         return `for(${this.iteration})` + super.render(e)
                                     }
                                     optimizeNames(e, t) {
                                         if (super.optimizeNames(e, t)) return this.iteration = O(this.iteration, e, t), this
                                     }
                                     get names() {
-                                        return A(super.names, this.iteration.names)
+                                        return x(super.names, this.iteration.names)
                                     }
                                 }
                                 class E extends _ {
                                     constructor(e, t, r, n) {
                                         super(), this.varKind = e, this.name = t, this.from = r, this.to = n
                                     }
                                     render(e) {
@@ -684,30 +684,30 @@
                                                 name: r,
                                                 from: n,
                                                 to: a
                                             } = this;
                                         return `for(${t} ${r}=${n}; ${r}<${a}; ${r}++)` + super.render(e)
                                     }
                                     get names() {
-                                        const e = x(super.names, this.from);
-                                        return x(e, this.to)
+                                        const e = A(super.names, this.from);
+                                        return A(e, this.to)
                                     }
                                 }
                                 class $ extends _ {
                                     constructor(e, t, r, n) {
                                         super(), this.loop = e, this.varKind = t, this.name = r, this.iterable = n
                                     }
                                     render(e) {
                                         return `for(${this.varKind} ${this.name} ${this.loop} ${this.iterable})` + super.render(e)
                                     }
                                     optimizeNames(e, t) {
                                         if (super.optimizeNames(e, t)) return this.iterable = O(this.iterable, e, t), this
                                     }
                                     get names() {
-                                        return A(super.names, this.iterable.names)
+                                        return x(super.names, this.iterable.names)
                                     }
                                 }
                                 class S extends y {
                                     constructor(e, t, r) {
                                         super(), this.name = e, this.args = t, this.async = r
                                     }
                                     render(e) {
@@ -732,15 +732,15 @@
                                     }
                                     optimizeNames(e, t) {
                                         var r, n;
                                         return super.optimizeNames(e, t), null === (r = this.catch) || void 0 === r || r.optimizeNames(e, t), null === (n = this.finally) || void 0 === n || n.optimizeNames(e, t), this
                                     }
                                     get names() {
                                         const e = super.names;
-                                        return this.catch && A(e, this.catch.names), this.finally && A(e, this.finally.names), e
+                                        return this.catch && x(e, this.catch.names), this.finally && x(e, this.finally.names), e
                                     }
                                 }
                                 class k extends y {
                                     constructor(e) {
                                         super(), this.error = e
                                     }
                                     render(e) {
@@ -750,21 +750,21 @@
                                 k.kind = "catch";
                                 class C extends y {
                                     render(e) {
                                         return "finally" + super.render(e)
                                     }
                                 }
 
-                                function A(e, t) {
+                                function x(e, t) {
                                     for (const r in t) e[r] = (e[r] || 0) + (t[r] || 0);
                                     return e
                                 }
 
-                                function x(e, t) {
-                                    return t instanceof n._CodeOrName ? A(e, t.names) : e
+                                function A(e, t) {
+                                    return t instanceof n._CodeOrName ? x(e, t.names) : e
                                 }
 
                                 function O(e, t, r) {
                                     return e instanceof n.Name ? a(e) : (o = e) instanceof n._Code && o._items.some((e => e instanceof n.Name && 1 === t[e.str] && void 0 !== r[e.str])) ? new n._Code(e._items.reduce(((e, t) => (t instanceof n.Name && (t = a(t)), t instanceof n._Code ? e.push(...t._items) : e.push(t), e)), [])) : e;
                                     var o;
 
                                     function a(e) {
@@ -2183,15 +2183,15 @@
                                                     }(e), t.return(l._`${d.default.errors} === 0`))
                                                 }(e)
                                         }))
                                     }(e) : m(e, (() => (0, n.topBoolOrEmptySchema)(e)))
                                 };
                                 class T {
                                     constructor(e, t, r) {
-                                        if ((0, c.validateKeywordUsage)(e, t, r), this.gen = e.gen, this.allErrors = e.allErrors, this.keyword = r, this.data = e.data, this.schema = e.schema[r], this.$data = t.$data && e.opts.$data && this.schema && this.schema.$data, this.schemaValue = (0, h.schemaRefOrVal)(e, this.schema, r, this.$data), this.schemaType = t.schemaType, this.parentSchema = e.schema, this.params = {}, this.it = e, this.def = t, this.$data) this.schemaCode = e.gen.const("vSchema", x(this.$data, e));
+                                        if ((0, c.validateKeywordUsage)(e, t, r), this.gen = e.gen, this.allErrors = e.allErrors, this.keyword = r, this.data = e.data, this.schema = e.schema[r], this.$data = t.$data && e.opts.$data && this.schema && this.schema.$data, this.schemaValue = (0, h.schemaRefOrVal)(e, this.schema, r, this.$data), this.schemaType = t.schemaType, this.parentSchema = e.schema, this.params = {}, this.it = e, this.def = t, this.$data) this.schemaCode = e.gen.const("vSchema", A(this.$data, e));
                                         else if (this.schemaCode = this.schemaValue, !(0, c.validSchemaType)(this.schema, t.schemaType, t.allowUndefined)) throw new Error(`${r} value must be ${JSON.stringify(t.schemaType)}`);
                                         ("code" in t ? t.trackErrors : !1 !== t.errors) && (this.errsCount = e.gen.const("_errs", d.default.errors))
                                     }
                                     result(e, t, r) {
                                         this.failResult((0, l.not)(e), t, r)
                                     }
                                     failResult(e, t, r) {
@@ -2318,28 +2318,28 @@
 
                                 function k(e, t, r, n) {
                                     const o = new T(e, r, t);
                                     "code" in r ? r.code(o, n) : o.$data && r.validate ? (0, c.funcKeywordCode)(o, r) : "macro" in r ? (0, c.macroKeywordCode)(o, r) : (r.compile || r.validate) && (0, c.funcKeywordCode)(o, r)
                                 }
                                 t.KeywordCxt = T;
                                 const C = /^\/(?:[^~]|~0|~1)*$/,
-                                    A = /^([0-9]+)(#|\/(?:[^~]|~0|~1)*)?$/;
+                                    x = /^([0-9]+)(#|\/(?:[^~]|~0|~1)*)?$/;
 
-                                function x(e, {
+                                function A(e, {
                                     dataLevel: t,
                                     dataNames: r,
                                     dataPathArr: n
                                 }) {
                                     let o, a;
                                     if ("" === e) return d.default.rootData;
                                     if ("/" === e[0]) {
                                         if (!C.test(e)) throw new Error(`Invalid JSON-pointer: ${e}`);
                                         o = e, a = d.default.rootData
                                     } else {
-                                        const s = A.exec(e);
+                                        const s = x.exec(e);
                                         if (!s) throw new Error(`Invalid JSON-pointer: ${e}`);
                                         const i = +s[1];
                                         if (o = s[2], "#" === o) {
                                             if (i >= t) throw new Error(c("property/index", i));
                                             return n[t - i]
                                         }
                                         if (i > t) throw new Error(c("data", i));
@@ -2350,15 +2350,15 @@
                                     for (const e of i) e && (a = l._`${a}${(0,l.getProperty)((0,h.unescapeJsonPointer)(e))}`, s = l._`${s} && ${a}`);
                                     return s;
 
                                     function c(e, r) {
                                         return `Cannot access ${e} ${r} levels up, current level is ${t}`
                                     }
                                 }
-                                t.getData = x
+                                t.getData = A
                             },
                             5277: (e, t, r) => {
                                 "use strict";
                                 Object.defineProperty(t, "__esModule", {
                                     value: !0
                                 }), t.validateKeywordUsage = t.validSchemaType = t.funcKeywordCode = t.macroKeywordCode = void 0;
                                 const n = r(5265),
@@ -2620,30 +2620,30 @@
                                         jsPropertySyntax: "",
                                         unicode: '"minLength"/"maxLength" account for unicode characters by default.'
                                     };
 
                                 function _(e) {
                                     var t, r, n, o, a, s, i, c, u, l, d, f, h, y, v, g, w, _, b, E, $, S, P, T, k;
                                     const C = e.strict,
-                                        A = null === (t = e.code) || void 0 === t ? void 0 : t.optimize,
-                                        x = !0 === A || void 0 === A ? 1 : A || 0,
+                                        x = null === (t = e.code) || void 0 === t ? void 0 : t.optimize,
+                                        A = !0 === x || void 0 === x ? 1 : x || 0,
                                         O = null !== (n = null === (r = e.code) || void 0 === r ? void 0 : r.regExp) && void 0 !== n ? n : m,
                                         N = null !== (o = e.uriResolver) && void 0 !== o ? o : p.default;
                                     return {
                                         strictSchema: null === (s = null !== (a = e.strictSchema) && void 0 !== a ? a : C) || void 0 === s || s,
                                         strictNumbers: null === (c = null !== (i = e.strictNumbers) && void 0 !== i ? i : C) || void 0 === c || c,
                                         strictTypes: null !== (l = null !== (u = e.strictTypes) && void 0 !== u ? u : C) && void 0 !== l ? l : "log",
                                         strictTuples: null !== (f = null !== (d = e.strictTuples) && void 0 !== d ? d : C) && void 0 !== f ? f : "log",
                                         strictRequired: null !== (y = null !== (h = e.strictRequired) && void 0 !== h ? h : C) && void 0 !== y && y,
                                         code: e.code ? {
                                             ...e.code,
-                                            optimize: x,
+                                            optimize: A,
                                             regExp: O
                                         } : {
-                                            optimize: x,
+                                            optimize: A,
                                             regExp: O
                                         },
                                         loopRequired: null !== (v = e.loopRequired) && void 0 !== v ? v : 200,
                                         loopEnum: null !== (g = e.loopEnum) && void 0 !== g ? g : 200,
                                         meta: null === (w = e.meta) || void 0 === w || w,
                                         messages: null === (_ = e.messages) || void 0 === _ || _,
                                         inlineRefs: null === (b = e.inlineRefs) || void 0 === b || b,
@@ -2830,15 +2830,15 @@
                                     addKeyword(e, t) {
                                         let r;
                                         if ("string" == typeof e) r = e, "object" == typeof t && (this.logger.warn("these parameters are deprecated, see docs for addKeyword"), t.keyword = r);
                                         else {
                                             if ("object" != typeof e || void 0 !== t) throw new Error("invalid addKeywords parameters");
                                             if (r = (t = e).keyword, Array.isArray(r) && !r.length) throw new Error("addKeywords: keyword must be string or non-empty array")
                                         }
-                                        if (x.call(this, r, t), !t) return (0, f.eachItem)(r, (e => O.call(this, e))), this;
+                                        if (A.call(this, r, t), !t) return (0, f.eachItem)(r, (e => O.call(this, e))), this;
                                         j.call(this, t);
                                         const n = {
                                             ...t,
                                             type: (0, d.getJSONTypes)(t.type),
                                             schemaType: (0, d.getJSONTypes)(t.schemaType)
                                         };
                                         return (0, f.eachItem)(r, 0 === n.type.length ? e => O.call(this, e, n) : e => n.type.forEach((t => O.call(this, e, n, t)))), this
@@ -2977,23 +2977,23 @@
                                 }
                                 t.default = b, b.ValidationError = a.default, b.MissingRefError = s.default;
                                 const C = {
                                         log() {},
                                         warn() {},
                                         error() {}
                                     },
-                                    A = /^[a-z_$][a-z0-9_$:-]*$/i;
+                                    x = /^[a-z_$][a-z0-9_$:-]*$/i;
 
-                                function x(e, t) {
+                                function A(e, t) {
                                     const {
                                         RULES: r
                                     } = this;
                                     if ((0, f.eachItem)(e, (e => {
                                             if (r.keywords[e]) throw new Error(`Keyword ${e} is already defined`);
-                                            if (!A.test(e)) throw new Error(`Keyword ${e} has invalid name`)
+                                            if (!x.test(e)) throw new Error(`Keyword ${e} has invalid name`)
                                         })), t && t.$data && !("code" in t) && !("validate" in t)) throw new Error('$data keyword must have "code" or "validate" function')
                                 }
 
                                 function O(e, t, r) {
                                     var n;
                                     const o = null == t ? void 0 : t.post;
                                     if (r && o) throw new Error('keyword with "post" flag cannot have "type"');
@@ -4990,36 +4990,36 @@
                                             E = r(r(r(m + "\\:") + "{0,3}" + m) + "?\\:\\:" + m + "\\:" + y),
                                             $ = r(r(r(m + "\\:") + "{0,4}" + m) + "?\\:\\:" + y),
                                             S = r(r(r(m + "\\:") + "{0,5}" + m) + "?\\:\\:" + m),
                                             P = r(r(r(m + "\\:") + "{0,6}" + m) + "?\\:\\:"),
                                             T = r([v, g, w, _, b, E, $, S, P].join("|")),
                                             k = r(r(l + "|" + s) + "+"),
                                             C = (r(T + "\\%25" + k), r(T + r("\\%25|\\%(?!" + a + "{2})") + k)),
-                                            A = r("[vV]" + a + "+\\." + t(l, i, "[\\:]") + "+"),
-                                            x = r("\\[" + r(C + "|" + T + "|" + A) + "\\]"),
+                                            x = r("[vV]" + a + "+\\." + t(l, i, "[\\:]") + "+"),
+                                            A = r("\\[" + r(C + "|" + T + "|" + x) + "\\]"),
                                             O = r(r(s + "|" + t(l, i)) + "*"),
-                                            N = r(x + "|" + p + "(?!" + O + ")|" + O),
+                                            N = r(A + "|" + p + "(?!" + O + ")|" + O),
                                             j = r(o + "*"),
                                             D = r(r(f + "@") + "?" + N + r("\\:" + j) + "?"),
                                             R = r(s + "|" + t(l, i, "[\\:\\@]")),
                                             M = r(R + "*"),
                                             I = r(R + "+"),
                                             F = r(r(s + "|" + t(l, i, "[\\@]")) + "+"),
                                             V = r(r("\\/" + M) + "*"),
                                             L = r("\\/" + r(I + V) + "?"),
                                             B = r(F + V),
                                             U = r(I + V),
                                             z = "(?!" + R + ")",
-                                            H = (r(V + "|" + L + "|" + B + "|" + U + "|" + z), r(r(R + "|" + t("[\\/\\?]", u)) + "*")),
-                                            q = r(r(R + "|[\\/\\?]") + "*"),
+                                            q = (r(V + "|" + L + "|" + B + "|" + U + "|" + z), r(r(R + "|" + t("[\\/\\?]", u)) + "*")),
+                                            H = r(r(R + "|[\\/\\?]") + "*"),
                                             W = r(r("\\/\\/" + D + V) + "|" + L + "|" + U + "|" + z),
-                                            G = r(d + "\\:" + W + r("\\?" + H) + "?" + r("\\#" + q) + "?"),
+                                            G = r(d + "\\:" + W + r("\\?" + q) + "?" + r("\\#" + H) + "?"),
                                             K = r(r("\\/\\/" + D + V) + "|" + L + "|" + B + "|" + z),
-                                            Y = r(K + r("\\?" + H) + "?" + r("\\#" + q) + "?");
-                                        return r(G + "|" + Y), r(d + "\\:" + W + r("\\?" + H) + "?"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + U + "|" + z + ")"), r("\\?(" + H + ")"), r("\\#(" + q + ")"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + B + "|" + z + ")"), r("\\?(" + H + ")"), r("\\#(" + q + ")"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + U + "|" + z + ")"), r("\\?(" + H + ")"), r("\\#(" + q + ")"), r("(" + f + ")@"), r("\\:(" + j + ")"), {
+                                            Y = r(K + r("\\?" + q) + "?" + r("\\#" + H) + "?");
+                                        return r(G + "|" + Y), r(d + "\\:" + W + r("\\?" + q) + "?"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + U + "|" + z + ")"), r("\\?(" + q + ")"), r("\\#(" + H + ")"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + B + "|" + z + ")"), r("\\?(" + q + ")"), r("\\#(" + H + ")"), r(r("\\/\\/(" + r("(" + f + ")@") + "?(" + N + ")" + r("\\:(" + j + ")") + "?)") + "?(" + V + "|" + L + "|" + U + "|" + z + ")"), r("\\?(" + q + ")"), r("\\#(" + H + ")"), r("(" + f + ")@"), r("\\:(" + j + ")"), {
                                             NOT_SCHEME: new RegExp(t("[^]", n, o, "[\\+\\-\\.]"), "g"),
                                             NOT_USERINFO: new RegExp(t("[^\\%\\:]", l, i), "g"),
                                             NOT_HOST: new RegExp(t("[^\\%\\[\\]\\:]", l, i), "g"),
                                             NOT_PATH: new RegExp(t("[^\\%\\/\\:\\@]", l, i), "g"),
                                             NOT_PATH_NOSCHEME: new RegExp(t("[^\\%\\/\\@]", l, i), "g"),
                                             NOT_QUERY: new RegExp(t("[^\\%]", l, i, "[\\:\\@\\/\\?]", u), "g"),
                                             NOT_FRAGMENT: new RegExp(t("[^\\%]", l, i, "[\\:\\@\\/\\?]"), "g"),
@@ -5163,38 +5163,38 @@
                                                 } finally {
                                                     try {
                                                         !$ && k.return && k.return()
                                                     } finally {
                                                         if (S) throw P
                                                     }
                                                 }
-                                                var A = g + 1;
-                                                E - n > m((u - o) / A) && v("overflow"), o += (E - n) * A, n = E;
-                                                var x = !0,
+                                                var x = g + 1;
+                                                E - n > m((u - o) / x) && v("overflow"), o += (E - n) * x, n = E;
+                                                var A = !0,
                                                     O = !1,
                                                     N = void 0;
                                                 try {
-                                                    for (var j, D = e[Symbol.iterator](); !(x = (j = D.next()).done); x = !0) {
+                                                    for (var j, D = e[Symbol.iterator](); !(A = (j = D.next()).done); A = !0) {
                                                         var R = j.value;
                                                         if (R < n && ++o > u && v("overflow"), R == n) {
                                                             for (var M = o, I = l;; I += l) {
                                                                 var F = I <= a ? 1 : I >= a + 26 ? 26 : I - a;
                                                                 if (M < F) break;
                                                                 var V = M - F,
                                                                     L = l - F;
                                                                 t.push(y(_(F + V % L, 0))), M = m(V / L)
                                                             }
-                                                            t.push(y(_(M, 0))), a = b(o, A, g == p), o = 0, ++g
+                                                            t.push(y(_(M, 0))), a = b(o, x, g == p), o = 0, ++g
                                                         }
                                                     }
                                                 } catch (e) {
                                                     O = !0, N = e
                                                 } finally {
                                                     try {
-                                                        !x && D.return && D.return()
+                                                        !A && D.return && D.return()
                                                     } finally {
                                                         if (O) throw N
                                                     }
                                                 }++o, ++n
                                             }
                                             return t.join("")
                                         },
@@ -5258,32 +5258,32 @@
                                         function r(e) {
                                             var r = k(e);
                                             return r.match(t.UNRESERVED) ? r : e
                                         }
                                         return e.scheme && (e.scheme = String(e.scheme).replace(t.PCT_ENCODED, r).toLowerCase().replace(t.NOT_SCHEME, "")), void 0 !== e.userinfo && (e.userinfo = String(e.userinfo).replace(t.PCT_ENCODED, r).replace(t.NOT_USERINFO, T).replace(t.PCT_ENCODED, o)), void 0 !== e.host && (e.host = String(e.host).replace(t.PCT_ENCODED, r).toLowerCase().replace(t.NOT_HOST, T).replace(t.PCT_ENCODED, o)), void 0 !== e.path && (e.path = String(e.path).replace(t.PCT_ENCODED, r).replace(e.scheme ? t.NOT_PATH : t.NOT_PATH_NOSCHEME, T).replace(t.PCT_ENCODED, o)), void 0 !== e.query && (e.query = String(e.query).replace(t.PCT_ENCODED, r).replace(t.NOT_QUERY, T).replace(t.PCT_ENCODED, o)), void 0 !== e.fragment && (e.fragment = String(e.fragment).replace(t.PCT_ENCODED, r).replace(t.NOT_FRAGMENT, T).replace(t.PCT_ENCODED, o)), e
                                     }
 
-                                    function A(e) {
+                                    function x(e) {
                                         return e.replace(/^0*(.*)/, "$1") || "0"
                                     }
 
-                                    function x(e, t) {
+                                    function A(e, t) {
                                         var r = e.match(t.IPV4ADDRESS) || [],
                                             n = c(r, 2)[1];
-                                        return n ? n.split(".").map(A).join(".") : e
+                                        return n ? n.split(".").map(x).join(".") : e
                                     }
 
                                     function O(e, t) {
                                         var r = e.match(t.IPV6ADDRESS) || [],
                                             n = c(r, 3),
                                             o = n[1],
                                             a = n[2];
                                         if (o) {
-                                            for (var s = o.toLowerCase().split("::").reverse(), i = c(s, 2), u = i[0], l = i[1], d = l ? l.split(":").map(A) : [], f = u.split(":").map(A), h = t.IPV4ADDRESS.test(f[f.length - 1]), p = h ? 7 : 8, m = f.length - p, y = Array(p), v = 0; v < p; ++v) y[v] = d[v] || f[m + v] || "";
-                                            h && (y[p - 1] = x(y[p - 1], t));
+                                            for (var s = o.toLowerCase().split("::").reverse(), i = c(s, 2), u = i[0], l = i[1], d = l ? l.split(":").map(x) : [], f = u.split(":").map(x), h = t.IPV4ADDRESS.test(f[f.length - 1]), p = h ? 7 : 8, m = f.length - p, y = Array(p), v = 0; v < p; ++v) y[v] = d[v] || f[m + v] || "";
+                                            h && (y[p - 1] = A(y[p - 1], t));
                                             var g = y.reduce((function(e, t, r) {
                                                     if (!t || "0" === t) {
                                                         var n = e[e.length - 1];
                                                         n && n.index + n.length === r ? n.length++ : e.push({
                                                             index: r,
                                                             length: 1
                                                         })
@@ -5308,15 +5308,15 @@
                                     function D(e) {
                                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                                             r = {},
                                             n = !1 !== t.iri ? i : s;
                                         "suffix" === t.reference && (e = (t.scheme ? t.scheme + ":" : "") + "//" + e);
                                         var o = e.match(N);
                                         if (o) {
-                                            j ? (r.scheme = o[1], r.userinfo = o[3], r.host = o[4], r.port = parseInt(o[5], 10), r.path = o[6] || "", r.query = o[7], r.fragment = o[8], isNaN(r.port) && (r.port = o[5])) : (r.scheme = o[1] || void 0, r.userinfo = -1 !== e.indexOf("@") ? o[3] : void 0, r.host = -1 !== e.indexOf("//") ? o[4] : void 0, r.port = parseInt(o[5], 10), r.path = o[6] || "", r.query = -1 !== e.indexOf("?") ? o[7] : void 0, r.fragment = -1 !== e.indexOf("#") ? o[8] : void 0, isNaN(r.port) && (r.port = e.match(/\/\/(?:.|\n)*\:(?:\/|\?|\#|$)/) ? o[4] : void 0)), r.host && (r.host = O(x(r.host, n), n)), void 0 !== r.scheme || void 0 !== r.userinfo || void 0 !== r.host || void 0 !== r.port || r.path || void 0 !== r.query ? void 0 === r.scheme ? r.reference = "relative" : void 0 === r.fragment ? r.reference = "absolute" : r.reference = "uri" : r.reference = "same-document", t.reference && "suffix" !== t.reference && t.reference !== r.reference && (r.error = r.error || "URI is not a " + t.reference + " reference.");
+                                            j ? (r.scheme = o[1], r.userinfo = o[3], r.host = o[4], r.port = parseInt(o[5], 10), r.path = o[6] || "", r.query = o[7], r.fragment = o[8], isNaN(r.port) && (r.port = o[5])) : (r.scheme = o[1] || void 0, r.userinfo = -1 !== e.indexOf("@") ? o[3] : void 0, r.host = -1 !== e.indexOf("//") ? o[4] : void 0, r.port = parseInt(o[5], 10), r.path = o[6] || "", r.query = -1 !== e.indexOf("?") ? o[7] : void 0, r.fragment = -1 !== e.indexOf("#") ? o[8] : void 0, isNaN(r.port) && (r.port = e.match(/\/\/(?:.|\n)*\:(?:\/|\?|\#|$)/) ? o[4] : void 0)), r.host && (r.host = O(A(r.host, n), n)), void 0 !== r.scheme || void 0 !== r.userinfo || void 0 !== r.host || void 0 !== r.port || r.path || void 0 !== r.query ? void 0 === r.scheme ? r.reference = "relative" : void 0 === r.fragment ? r.reference = "absolute" : r.reference = "uri" : r.reference = "same-document", t.reference && "suffix" !== t.reference && t.reference !== r.reference && (r.error = r.error || "URI is not a " + t.reference + " reference.");
                                             var a = P[(t.scheme || r.scheme || "").toLowerCase()];
                                             if (t.unicodeSupport || a && a.unicodeSupport) C(r, n);
                                             else {
                                                 if (r.host && (t.domainHost || a && a.domainHost)) try {
                                                     r.host = S.toASCII(r.host.replace(n.PCT_ENCODED, k).toLowerCase())
                                                 } catch (e) {
                                                     r.error = r.error || "Host's domain name can not be converted to ASCII via punycode: " + e
@@ -5359,15 +5359,15 @@
                                         } catch (r) {
                                             e.error = e.error || "Host's domain name can not be converted to " + (t.iri ? "Unicode" : "ASCII") + " via punycode: " + r
                                         }
                                         C(e, r), "suffix" !== t.reference && e.scheme && (n.push(e.scheme), n.push(":"));
                                         var a = function(e, t) {
                                             var r = !1 !== t.iri ? i : s,
                                                 n = [];
-                                            return void 0 !== e.userinfo && (n.push(e.userinfo), n.push("@")), void 0 !== e.host && n.push(O(x(String(e.host), r), r).replace(r.IPV6ADDRESS, (function(e, t, r) {
+                                            return void 0 !== e.userinfo && (n.push(e.userinfo), n.push("@")), void 0 !== e.host && n.push(O(A(String(e.host), r), r).replace(r.IPV6ADDRESS, (function(e, t, r) {
                                                 return "[" + t + (r ? "%25" + r : "") + "]"
                                             }))), "number" != typeof e.port && "string" != typeof e.port || (n.push(":"), n.push(String(e.port))), n.length ? n.join("") : void 0
                                         }(e, t);
                                         if (void 0 !== a && ("suffix" !== t.reference && n.push("//"), n.push(a), e.path && "/" !== e.path.charAt(0) && n.push("/")), void 0 !== e.path) {
                                             var c = e.path;
                                             t.absolutePath || o && o.absolutePath || (c = V(c)), void 0 === a && (c = c.replace(/^\/\//, "/%2F")), n.push(c)
                                         }
@@ -5390,33 +5390,33 @@
                                                 return e.host || (e.error = e.error || "HTTP URIs must have a host."), e
                                             },
                                             serialize: function(e, t) {
                                                 var r = "https" === String(e.scheme).toLowerCase();
                                                 return e.port !== (r ? 443 : 80) && "" !== e.port || (e.port = void 0), e.path || (e.path = "/"), e
                                             }
                                         },
-                                        H = {
+                                        q = {
                                             scheme: "https",
                                             domainHost: z.domainHost,
                                             parse: z.parse,
                                             serialize: z.serialize
                                         };
 
-                                    function q(e) {
+                                    function H(e) {
                                         return "boolean" == typeof e.secure ? e.secure : "wss" === String(e.scheme).toLowerCase()
                                     }
                                     var W = {
                                             scheme: "ws",
                                             domainHost: !0,
                                             parse: function(e, t) {
                                                 var r = e;
-                                                return r.secure = q(r), r.resourceName = (r.path || "/") + (r.query ? "?" + r.query : ""), r.path = void 0, r.query = void 0, r
+                                                return r.secure = H(r), r.resourceName = (r.path || "/") + (r.query ? "?" + r.query : ""), r.path = void 0, r.query = void 0, r
                                             },
                                             serialize: function(e, t) {
-                                                if (e.port !== (q(e) ? 443 : 80) && "" !== e.port || (e.port = void 0), "boolean" == typeof e.secure && (e.scheme = e.secure ? "wss" : "ws", e.secure = void 0), e.resourceName) {
+                                                if (e.port !== (H(e) ? 443 : 80) && "" !== e.port || (e.port = void 0), "boolean" == typeof e.secure && (e.scheme = e.secure ? "wss" : "ws", e.secure = void 0), e.resourceName) {
                                                     var r = e.resourceName.split("?"),
                                                         n = c(r, 2),
                                                         o = n[0],
                                                         a = n[1];
                                                     e.path = o && "/" !== o ? o : void 0, e.query = a, e.resourceName = void 0
                                                 }
                                                 return e.fragment = void 0, e
@@ -5540,15 +5540,15 @@
                                                 return r.uuid = r.nss, r.nss = void 0, t.tolerant || r.uuid && r.uuid.match(ce) || (r.error = r.error || "UUID is not valid."), r
                                             },
                                             serialize: function(e, t) {
                                                 var r = e;
                                                 return r.nss = (e.uuid || "").toLowerCase(), r
                                             }
                                         };
-                                    P[z.scheme] = z, P[H.scheme] = H, P[W.scheme] = W, P[G.scheme] = G, P[ae.scheme] = ae, P[ie.scheme] = ie, P[ue.scheme] = ue, e.SCHEMES = P, e.pctEncChar = T, e.pctDecChars = k, e.parse = D, e.removeDotSegments = V, e.serialize = L, e.resolveComponents = B, e.resolve = function(e, t, r) {
+                                    P[z.scheme] = z, P[q.scheme] = q, P[W.scheme] = W, P[G.scheme] = G, P[ae.scheme] = ae, P[ie.scheme] = ie, P[ue.scheme] = ue, e.SCHEMES = P, e.pctEncChar = T, e.pctDecChars = k, e.parse = D, e.removeDotSegments = V, e.serialize = L, e.resolveComponents = B, e.resolve = function(e, t, r) {
                                         var n = function(e, t) {
                                             var r = {
                                                 scheme: "null"
                                             };
                                             if (t)
                                                 for (var n in t) r[n] = t[n];
                                             return r
@@ -5698,15 +5698,15 @@
                             function $(e) {
                                 for (var t = 0, r = 0; r < e.length; ++r) {
                                     var n = e.charCodeAt(r);
                                     n >= 55296 && n <= 57343 && (n = 65536 + ((1023 & n) << 10) | 1023 & e.charCodeAt(++r)), n <= 127 ? ++t : t += n <= 2047 ? 2 : n <= 65535 ? 3 : 4
                                 }
                                 return t
                             }
-                            var S, P, T, k, C, A, x, O, N, j = "undefined" != typeof TextDecoder ? new TextDecoder("utf-16le") : void 0;
+                            var S, P, T, k, C, x, A, O, N, j = "undefined" != typeof TextDecoder ? new TextDecoder("utf-16le") : void 0;
 
                             function D(e, t) {
                                 for (var r = e, n = r >> 1, o = n + t / 2; !(n >= o) && C[n >>> 0];) ++n;
                                 if ((r = n << 1) - e > 32 && j) return j.decode(T.subarray(e >>> 0, r >>> 0));
                                 for (var a = "", s = 0; !(s >= t / 2); ++s) {
                                     var i = k[e + 2 * s >>> 1];
                                     if (0 == i) break;
@@ -5726,52 +5726,52 @@
 
                             function M(e) {
                                 return 2 * e.length
                             }
 
                             function I(e, t) {
                                 for (var r = 0, n = ""; !(r >= t / 4);) {
-                                    var o = A[e + 4 * r >>> 2];
+                                    var o = x[e + 4 * r >>> 2];
                                     if (0 == o) break;
                                     if (++r, o >= 65536) {
                                         var a = o - 65536;
                                         n += String.fromCharCode(55296 | a >> 10, 56320 | 1023 & a)
                                     } else n += String.fromCharCode(o)
                                 }
                                 return n
                             }
 
                             function F(e, t, r) {
                                 if (void 0 === r && (r = 2147483647), r < 4) return 0;
                                 for (var n = t >>>= 0, o = n + r - 4, a = 0; a < e.length; ++a) {
                                     var s = e.charCodeAt(a);
-                                    if (s >= 55296 && s <= 57343 && (s = 65536 + ((1023 & s) << 10) | 1023 & e.charCodeAt(++a)), A[t >>> 2] = s, (t += 4) + 4 > o) break
+                                    if (s >= 55296 && s <= 57343 && (s = 65536 + ((1023 & s) << 10) | 1023 & e.charCodeAt(++a)), x[t >>> 2] = s, (t += 4) + 4 > o) break
                                 }
-                                return A[t >>> 2] = 0, t - n
+                                return x[t >>> 2] = 0, t - n
                             }
 
                             function V(e) {
                                 for (var t = 0, r = 0; r < e.length; ++r) {
                                     var n = e.charCodeAt(r);
                                     n >= 55296 && n <= 57343 && ++r, t += 4
                                 }
                                 return t
                             }
 
                             function L(e) {
                                 var t = $(e) + 1,
-                                    r = Ht(t);
+                                    r = qt(t);
                                 return r && b(e, P, r, t), r
                             }
 
                             function B(e) {
-                                S = e, t.HEAP8 = P = new Int8Array(e), t.HEAP16 = k = new Int16Array(e), t.HEAP32 = A = new Int32Array(e), t.HEAPU8 = T = new Uint8Array(e), t.HEAPU16 = C = new Uint16Array(e), t.HEAPU32 = x = new Uint32Array(e), t.HEAPF32 = O = new Float32Array(e), t.HEAPF64 = N = new Float64Array(e)
+                                S = e, t.HEAP8 = P = new Int8Array(e), t.HEAP16 = k = new Int16Array(e), t.HEAP32 = x = new Int32Array(e), t.HEAPU8 = T = new Uint8Array(e), t.HEAPU16 = C = new Uint16Array(e), t.HEAPU32 = A = new Uint32Array(e), t.HEAPF32 = O = new Float32Array(e), t.HEAPF64 = N = new Float64Array(e)
                             }
                             t.INITIAL_MEMORY;
-                            var U, z, H, q, W, G = [],
+                            var U, z, q, H, W, G = [],
                                 K = [],
                                 Y = [],
                                 J = 0,
                                 X = null,
                                 Z = null;
 
                             function Q(e) {
@@ -5809,55 +5809,55 @@
                                     var r = e.shift();
                                     if ("function" != typeof r) {
                                         var n = r.func;
                                         "number" == typeof n ? void 0 === r.arg ? se(n)() : se(n)(r.arg) : n(void 0 === r.arg ? null : r.arg)
                                     } else r(t)
                                 }
                             }
-                            re(z = "jupytercad.opencascade.wasm") || (H = z, z = t.locateFile ? t.locateFile(H, l) : l + H);
+                            re(z = "jupytercad.opencascade.wasm") || (q = z, z = t.locateFile ? t.locateFile(q, l) : l + q);
                             var ae = [];
 
                             function se(e) {
                                 var t = ae[e];
                                 return t || (e >= ae.length && (ae.length = e + 1), ae[e] = t = U.get(e)), t
                             }
 
                             function ie(e) {
                                 this.excPtr = e, this.ptr = e - 24, this.set_type = function(e) {
-                                    x[this.ptr + 4 >>> 2] = e
+                                    A[this.ptr + 4 >>> 2] = e
                                 }, this.get_type = function() {
-                                    return x[this.ptr + 4 >>> 2]
+                                    return A[this.ptr + 4 >>> 2]
                                 }, this.set_destructor = function(e) {
-                                    x[this.ptr + 8 >>> 2] = e
+                                    A[this.ptr + 8 >>> 2] = e
                                 }, this.get_destructor = function() {
-                                    return x[this.ptr + 8 >>> 2]
+                                    return A[this.ptr + 8 >>> 2]
                                 }, this.set_refcount = function(e) {
-                                    A[this.ptr >>> 2] = e
+                                    x[this.ptr >>> 2] = e
                                 }, this.set_caught = function(e) {
                                     e = e ? 1 : 0, P[this.ptr + 12 >>> 0] = e
                                 }, this.get_caught = function() {
                                     return 0 != P[this.ptr + 12 >>> 0]
                                 }, this.set_rethrown = function(e) {
                                     e = e ? 1 : 0, P[this.ptr + 13 >>> 0] = e
                                 }, this.get_rethrown = function() {
                                     return 0 != P[this.ptr + 13 >>> 0]
                                 }, this.init = function(e, t) {
                                     this.set_adjusted_ptr(0), this.set_type(e), this.set_destructor(t), this.set_refcount(0), this.set_caught(!1), this.set_rethrown(!1)
                                 }, this.add_ref = function() {
-                                    var e = A[this.ptr >>> 2];
-                                    A[this.ptr >>> 2] = e + 1
+                                    var e = x[this.ptr >>> 2];
+                                    x[this.ptr >>> 2] = e + 1
                                 }, this.release_ref = function() {
-                                    var e = A[this.ptr >>> 2];
-                                    return A[this.ptr >>> 2] = e - 1, 1 === e
+                                    var e = x[this.ptr >>> 2];
+                                    return x[this.ptr >>> 2] = e - 1, 1 === e
                                 }, this.set_adjusted_ptr = function(e) {
-                                    x[this.ptr + 16 >>> 2] = e
+                                    A[this.ptr + 16 >>> 2] = e
                                 }, this.get_adjusted_ptr = function() {
-                                    return x[this.ptr + 16 >>> 2]
+                                    return A[this.ptr + 16 >>> 2]
                                 }, this.get_exception_ptr = function() {
-                                    if (Jt(this.get_type())) return x[this.excPtr >>> 2];
+                                    if (Jt(this.get_type())) return A[this.excPtr >>> 2];
                                     var e = this.get_adjusted_ptr();
                                     return 0 !== e ? e : this.excPtr
                                 }
                             }
                             var ce = {
                                     isAbs: e => "/" === e.charAt(0),
                                     splitPath: e => /^(\/?|)([\s\S]*?)((?:\.{1,2}|[^\/]+?|)(\.[^.\/]*|))(?:[\/]*)$/.exec(e).slice(1),
@@ -7138,23 +7138,23 @@
                                     doStat: function(e, t, r) {
                                         try {
                                             var n = e(t)
                                         } catch (e) {
                                             if (e && e.node && ce.normalize(t) !== ce.normalize(he.getPath(e.node))) return -54;
                                             throw e
                                         }
-                                        return A[r >>> 2] = n.dev, A[r + 4 >>> 2] = 0, A[r + 8 >>> 2] = n.ino, A[r + 12 >>> 2] = n.mode, A[r + 16 >>> 2] = n.nlink, A[r + 20 >>> 2] = n.uid, A[r + 24 >>> 2] = n.gid, A[r + 28 >>> 2] = n.rdev, A[r + 32 >>> 2] = 0, W = [n.size >>> 0, (q = n.size, +Math.abs(q) >= 1 ? q > 0 ? (0 | Math.min(+Math.floor(q / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((q - +(~~q >>> 0)) / 4294967296) >>> 0 : 0)], A[r + 40 >>> 2] = W[0], A[r + 44 >>> 2] = W[1], A[r + 48 >>> 2] = 4096, A[r + 52 >>> 2] = n.blocks, A[r + 56 >>> 2] = n.atime.getTime() / 1e3 | 0, A[r + 60 >>> 2] = 0, A[r + 64 >>> 2] = n.mtime.getTime() / 1e3 | 0, A[r + 68 >>> 2] = 0, A[r + 72 >>> 2] = n.ctime.getTime() / 1e3 | 0, A[r + 76 >>> 2] = 0, W = [n.ino >>> 0, (q = n.ino, +Math.abs(q) >= 1 ? q > 0 ? (0 | Math.min(+Math.floor(q / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((q - +(~~q >>> 0)) / 4294967296) >>> 0 : 0)], A[r + 80 >>> 2] = W[0], A[r + 84 >>> 2] = W[1], 0
+                                        return x[r >>> 2] = n.dev, x[r + 4 >>> 2] = 0, x[r + 8 >>> 2] = n.ino, x[r + 12 >>> 2] = n.mode, x[r + 16 >>> 2] = n.nlink, x[r + 20 >>> 2] = n.uid, x[r + 24 >>> 2] = n.gid, x[r + 28 >>> 2] = n.rdev, x[r + 32 >>> 2] = 0, W = [n.size >>> 0, (H = n.size, +Math.abs(H) >= 1 ? H > 0 ? (0 | Math.min(+Math.floor(H / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((H - +(~~H >>> 0)) / 4294967296) >>> 0 : 0)], x[r + 40 >>> 2] = W[0], x[r + 44 >>> 2] = W[1], x[r + 48 >>> 2] = 4096, x[r + 52 >>> 2] = n.blocks, x[r + 56 >>> 2] = n.atime.getTime() / 1e3 | 0, x[r + 60 >>> 2] = 0, x[r + 64 >>> 2] = n.mtime.getTime() / 1e3 | 0, x[r + 68 >>> 2] = 0, x[r + 72 >>> 2] = n.ctime.getTime() / 1e3 | 0, x[r + 76 >>> 2] = 0, W = [n.ino >>> 0, (H = n.ino, +Math.abs(H) >= 1 ? H > 0 ? (0 | Math.min(+Math.floor(H / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((H - +(~~H >>> 0)) / 4294967296) >>> 0 : 0)], x[r + 80 >>> 2] = W[0], x[r + 84 >>> 2] = W[1], 0
                                     },
                                     doMsync: function(e, t, r, n, o) {
                                         var a = T.slice(e, e + r);
                                         he.msync(t, a, o, r, n)
                                     },
                                     varargs: void 0,
                                     get: function() {
-                                        return pe.varargs += 4, A[pe.varargs - 4 >>> 2]
+                                        return pe.varargs += 4, x[pe.varargs - 4 >>> 2]
                                     },
                                     getStr: function(e) {
                                         return _(e)
                                     },
                                     getStreamFromFD: function(e) {
                                         var t = he.getStream(e);
                                         if (!t) throw new he.ErrnoError(8);
@@ -7211,22 +7211,22 @@
                             var Te = void 0;
 
                             function ke(e) {
                                 throw new Te(e)
                             }
                             var Ce = void 0;
 
-                            function Ae(e) {
+                            function xe(e) {
                                 throw new Ce(e)
                             }
 
-                            function xe(e, t, r) {
+                            function Ae(e, t, r) {
                                 function n(t) {
                                     var n = r(t);
-                                    n.length !== e.length && Ae("Mismatched type converter count");
+                                    n.length !== e.length && xe("Mismatched type converter count");
                                     for (var o = 0; o < e.length; ++o) Oe(e[o], n[o])
                                 }
                                 e.forEach((function(e) {
                                     _e[e] = t
                                 }));
                                 var o = new Array(t.length),
                                     a = [],
@@ -7279,15 +7279,15 @@
                                     e.$$.deleteScheduled = !1, e.delete()
                                 }
                             }
                             var Le = void 0,
                                 Be = {};
 
                             function Ue(e, t) {
-                                return t.ptrType && t.ptr || Ae("makeClassHandle requires ptr and ptrType"), !!t.smartPtrType != !!t.smartPtr && Ae("Both smartPtrType and smartPtr must be specified"), t.count = {
+                                return t.ptrType && t.ptr || xe("makeClassHandle requires ptr and ptrType"), !!t.smartPtrType != !!t.smartPtr && xe("Both smartPtrType and smartPtr must be specified"), t.count = {
                                     value: 1
                                 }, ze(Object.create(e, {
                                     $$: {
                                         value: t
                                     }
                                 }))
                             }
@@ -7303,27 +7303,27 @@
                                         };
                                         je.register(e, r, e)
                                     }
                                     return e
                                 }, De = e => je.unregister(e), ze(e))
                             }
 
-                            function He() {}
+                            function qe() {}
 
-                            function qe(e, t, r) {
+                            function He(e, t, r) {
                                 if (void 0 === e[t].overloadTable) {
                                     var n = e[t];
                                     e[t] = function() {
                                         return e[t].overloadTable.hasOwnProperty(arguments.length) || ke("Function '" + r + "' called with an invalid number of arguments (" + arguments.length + ") - expects one of (" + e[t].overloadTable + ")!"), e[t].overloadTable[arguments.length].apply(this, arguments)
                                     }, e[t].overloadTable = [], e[t].overloadTable[n.argCount] = n
                                 }
                             }
 
                             function We(e, r, n) {
-                                t.hasOwnProperty(e) ? ((void 0 === n || void 0 !== t[e].overloadTable && void 0 !== t[e].overloadTable[n]) && ke("Cannot register public name '" + e + "' twice"), qe(t, e, e), t.hasOwnProperty(n) && ke("Cannot register multiple overloads of a function with the same number of arguments (" + n + ")!"), t[e].overloadTable[n] = r) : (t[e] = r, void 0 !== n && (t[e].numArguments = n))
+                                t.hasOwnProperty(e) ? ((void 0 === n || void 0 !== t[e].overloadTable && void 0 !== t[e].overloadTable[n]) && ke("Cannot register public name '" + e + "' twice"), He(t, e, e), t.hasOwnProperty(n) && ke("Cannot register multiple overloads of a function with the same number of arguments (" + n + ")!"), t[e].overloadTable[n] = r) : (t[e] = r, void 0 !== n && (t[e].numArguments = n))
                             }
 
                             function Ge(e, t, r, n, o, a, s, i) {
                                 this.name = e, this.constructor = t, this.instancePrototype = r, this.rawDestructor = n, this.baseClass = o, this.getActualType = a, this.upcast = s, this.downcast = i, this.pureVirtualFunctions = []
                             }
 
                             function Ke(e, t, r) {
@@ -7369,15 +7369,15 @@
                                 if (null === t) return this.isReference && ke("null is not a valid " + this.name), 0;
                                 t.$$ || ke('Cannot pass "' + pt(t) + '" as a ' + this.name), t.$$.ptr || ke("Cannot pass deleted object as a pointer of type " + this.name), t.$$.ptrType.isConst && ke("Cannot convert argument of type " + t.$$.ptrType.name + " to parameter type " + this.name);
                                 var r = t.$$.ptrType.registeredClass;
                                 return Ke(t.$$.ptr, r, this.registeredClass)
                             }
 
                             function Ze(e) {
-                                return this.fromWireType(x[e >>> 2])
+                                return this.fromWireType(A[e >>> 2])
                             }
 
                             function Qe(e, t, r, n, o, a, s, i, c, u, l) {
                                 this.name = e, this.registeredClass = t, this.isReference = r, this.isConst = n, this.isSmartPointer = o, this.pointeeType = a, this.sharingPolicy = s, this.rawGetPointee = i, this.rawConstructor = c, this.rawShare = u, this.rawDestructor = l, o || void 0 !== t.baseClass ? this.toWireType = Je : n ? (this.toWireType = Ye, this.destructorFunction = null) : (this.toWireType = Xe, this.destructorFunction = null)
                             }
 
                             function et(e, r) {
@@ -7393,15 +7393,15 @@
                                 return "function" != typeof s && ke("unknown function pointer with signature " + e + ": " + r), s
                             }
                             var tt = void 0;
 
                             function rt(e) {
                                 var t = Gt(e),
                                     r = ve(t);
-                                return qt(t), r
+                                return Ht(t), r
                             }
 
                             function nt(e, t) {
                                 var r = [],
                                     n = {};
                                 throw t.forEach((function e(t) {
                                     n[t] || we[t] || (_e[t] ? _e[t].forEach(e) : (r.push(t), n[t] = !0))
@@ -7447,15 +7447,15 @@
                                         var y = 1 === c ? "thisWired" : "arg" + (c - 2) + "Wired";
                                         null !== t[c].destructorFunction && (f += y + "_dtor(" + y + "); // " + t[c].name + "\n", p.push(y + "_dtor"), m.push(t[c].destructorFunction))
                                     }
                                 return u && (f += "var ret = retType.fromWireType(rv);\nreturn ret;\n"), f += "}\n", p.push(f), ot(Function, p).apply(null, m)
                             }
 
                             function it(e, t) {
-                                for (var r = [], n = 0; n < e; n++) r.push(A[(t >> 2) + n >>> 0]);
+                                for (var r = [], n = 0; n < e; n++) r.push(x[(t >> 2) + n >>> 0]);
                                 return r
                             }
                             var ct = [],
                                 ut = [{}, {
                                     value: void 0
                                 }, {
                                     value: null
@@ -7500,15 +7500,15 @@
                                     case 1:
                                         return function(e) {
                                             var t = r ? k : C;
                                             return this.fromWireType(t[e >>> 1])
                                         };
                                     case 2:
                                         return function(e) {
-                                            var t = r ? A : x;
+                                            var t = r ? x : A;
                                             return this.fromWireType(t[e >>> 2])
                                         };
                                     default:
                                         throw new TypeError("Unknown integer type: " + e)
                                 }
                             }
 
@@ -7550,17 +7550,17 @@
                                         return r ? function(e) {
                                             return k[e >>> 1]
                                         } : function(e) {
                                             return C[e >>> 1]
                                         };
                                     case 2:
                                         return r ? function(e) {
-                                            return A[e >>> 2]
-                                        } : function(e) {
                                             return x[e >>> 2]
+                                        } : function(e) {
+                                            return A[e >>> 2]
                                         };
                                     default:
                                         throw new TypeError("Unknown integer type: " + e)
                                 }
                             }
                             var vt = {};
 
@@ -7665,16 +7665,16 @@
                                     },
                                     getNewId: function(e) {
                                         for (var t = Ct.counter++, r = e.length; r < t; r++) e[r] = null;
                                         return t
                                     },
                                     getSource: function(e, t, r, n) {
                                         for (var o = "", a = 0; a < t; ++a) {
-                                            var s = n ? A[n + 4 * a >>> 2] : -1;
-                                            o += _(A[r + 4 * a >>> 2], s < 0 ? void 0 : s)
+                                            var s = n ? x[n + 4 * a >>> 2] : -1;
+                                            o += _(x[r + 4 * a >>> 2], s < 0 ? void 0 : s)
                                         }
                                         return o
                                     },
                                     createContext: function(e, t) {
                                         if (!e.getContextSafariWebGL2Fixed) {
                                             function n(t, r) {
                                                 var n = e.getContextSafariWebGL2Fixed(t, r);
@@ -7738,19 +7738,19 @@
                                             }(r), r.disjointTimerQueryExt = r.getExtension("EXT_disjoint_timer_query"), (t = r).multiDrawWebgl = t.getExtension("WEBGL_multi_draw"), (r.getSupportedExtensions() || []).forEach((function(e) {
                                                 e.includes("lose_context") || e.includes("debug") || r.getExtension(e)
                                             }))
                                         }
                                     }
                                 };
 
-                            function At(e) {
+                            function xt(e) {
                                 return "]" == e.slice(-1) && e.lastIndexOf("[")
                             }
 
-                            function xt(e) {
+                            function At(e) {
                                 var t = Dt.currentProgram;
                                 if (t) {
                                     var r = t.uniformLocsById[e];
                                     return "number" == typeof r && (t.uniformLocsById[e] = r = Dt.getUniformLocation(t, t.uniformArrayNamesById[e] + (r > 0 ? "[" + r + "]" : ""))), r
                                 }
                                 Ct.recordError(1282)
                             }
@@ -7792,21 +7792,21 @@
                                             return he.isChrdev(this.mode)
                                         }
                                     }
                                 }), he.FSNode = It, he.staticInit(),
                                 function() {
                                     for (var e = new Array(256), t = 0; t < 256; ++t) e[t] = String.fromCharCode(t);
                                     ye = e
-                                }(), Te = t.BindingError = Pe(Error, "BindingError"), Ce = t.InternalError = Pe(Error, "InternalError"), He.prototype.isAliasOf = function(e) {
-                                    if (!(this instanceof He)) return !1;
-                                    if (!(e instanceof He)) return !1;
+                                }(), Te = t.BindingError = Pe(Error, "BindingError"), Ce = t.InternalError = Pe(Error, "InternalError"), qe.prototype.isAliasOf = function(e) {
+                                    if (!(this instanceof qe)) return !1;
+                                    if (!(e instanceof qe)) return !1;
                                     for (var t = this.$$.ptrType.registeredClass, r = this.$$.ptr, n = e.$$.ptrType.registeredClass, o = e.$$.ptr; t.baseClass;) r = t.upcast(r), t = t.baseClass;
                                     for (; n.baseClass;) o = n.upcast(o), n = n.baseClass;
                                     return t === n && r === o
-                                }, He.prototype.clone = function() {
+                                }, qe.prototype.clone = function() {
                                     if (this.$$.ptr || Ne(this), this.$$.preservePointerOnDelete) return this.$$.count.value += 1, this;
                                     var e, t = ze(Object.create(Object.getPrototypeOf(this), {
                                         $$: {
                                             value: (e = this.$$, {
                                                 count: e.count,
                                                 deleteScheduled: e.deleteScheduled,
                                                 preservePointerOnDelete: e.preservePointerOnDelete,
@@ -7814,19 +7814,19 @@
                                                 ptrType: e.ptrType,
                                                 smartPtr: e.smartPtr,
                                                 smartPtrType: e.smartPtrType
                                             })
                                         }
                                     }));
                                     return t.$$.count.value += 1, t.$$.deleteScheduled = !1, t
-                                }, He.prototype.delete = function() {
+                                }, qe.prototype.delete = function() {
                                     this.$$.ptr || Ne(this), this.$$.deleteScheduled && !this.$$.preservePointerOnDelete && ke("Object already scheduled for deletion"), De(this), Re(this.$$), this.$$.preservePointerOnDelete || (this.$$.smartPtr = void 0, this.$$.ptr = void 0)
-                                }, He.prototype.isDeleted = function() {
+                                }, qe.prototype.isDeleted = function() {
                                     return !this.$$.ptr
-                                }, He.prototype.deleteLater = function() {
+                                }, qe.prototype.deleteLater = function() {
                                     return this.$$.ptr || Ne(this), this.$$.deleteScheduled && !this.$$.preservePointerOnDelete && ke("Object already scheduled for deletion"), Fe.push(this), 1 === Fe.length && Le && Le(Ve), this.$$.deleteScheduled = !0, this
                                 }, t.getInheritedInstanceCount = function() {
                                     return Object.keys(Be).length
                                 }, t.getLiveInheritedInstances = function() {
                                     var e = [];
                                     for (var t in Be) Be.hasOwnProperty(t) && e.push(Be[t]);
                                     return e
@@ -7900,15 +7900,15 @@
                                     fa: function() {
                                         return t.HEAP8.length
                                     },
                                     i: function(e, t, r, n) {
                                         te("Assertion failed: " + _(e) + ", at: " + [t ? _(t) : "unknown filename", r, n ? _(n) : "unknown function"])
                                     },
                                     a: function(e) {
-                                        return Ht(e + 24) + 24
+                                        return qt(e + 24) + 24
                                     },
                                     b: function(e, t, r) {
                                         throw new ie(e).init(t, r), e
                                     },
                                     P: function(e, t) {
                                         try {
                                             return e = pe.getStr(e), he.chmod(e, t), 0
@@ -7951,15 +7951,15 @@
                                                 case 5:
                                                     return o = pe.get(), k[o + 0 >>> 1] = 2, 0;
                                                 case 16:
                                                 case 8:
                                                 default:
                                                     return -28;
                                                 case 9:
-                                                    return A[Wt() >>> 2] = 28, -1
+                                                    return x[Wt() >>> 2] = 28, -1
                                             }
                                         } catch (e) {
                                             if (void 0 === he || !(e instanceof he.ErrnoError)) throw e;
                                             return -e.errno
                                         }
                                     },
                                     J: function(e, t) {
@@ -7986,15 +7986,15 @@
                                                 case 21508:
                                                 case 21523:
                                                 case 21524:
                                                     return n.tty ? 0 : -59;
                                                 case 21519:
                                                     if (!n.tty) return -59;
                                                     var o = pe.get();
-                                                    return A[o >>> 2] = 0, 0;
+                                                    return x[o >>> 2] = 0, 0;
                                                 case 21520:
                                                     return n.tty ? -28 : -59;
                                                 case 21531:
                                                     return o = pe.get(), he.ioctl(n, t, o);
                                                 default:
                                                     te("bad ioctl syscall " + t)
                                             }
@@ -8055,29 +8055,29 @@
                                             argPackAdvance: 8,
                                             readValueFromPointer: function(e) {
                                                 var n;
                                                 if (1 === r) n = P;
                                                 else if (2 === r) n = k;
                                                 else {
                                                     if (4 !== r) throw new TypeError("Unknown boolean type size: " + t);
-                                                    n = A
+                                                    n = x
                                                 }
                                                 return this.fromWireType(n[e >>> a])
                                             },
                                             destructorFunction: null
                                         })
                                     },
                                     d: function(e, r, n, o, a, s, i, c, u, l, d, f, h) {
                                         d = ve(d), s = et(a, s), c && (c = et(i, c)), l && (l = et(u, l)), h = et(f, h);
                                         var p = $e(d);
                                         We(p, (function() {
                                             nt("Cannot construct " + d + " due to unbound types", [o])
-                                        })), xe([e, r, n], o ? [o] : [], (function(r) {
+                                        })), Ae([e, r, n], o ? [o] : [], (function(r) {
                                             var n, a;
-                                            r = r[0], a = o ? (n = r.registeredClass).instancePrototype : He.prototype;
+                                            r = r[0], a = o ? (n = r.registeredClass).instancePrototype : qe.prototype;
                                             var i = Se(p, (function() {
                                                     if (Object.getPrototypeOf(this) !== u) throw new Te("Use 'new' to construct " + d);
                                                     if (void 0 === f.constructor_body) throw new Te(d + " has no accessible constructor");
                                                     var e = f.constructor_body[arguments.length];
                                                     if (void 0 === e) throw new Te("Tried to invoke ctor of " + d + " with invalid number of parameters (" + arguments.length + ") - expected (" + Object.keys(f.constructor_body).toString() + ") parameters instead!");
                                                     return e.apply(this, arguments)
                                                 })),
@@ -8092,60 +8092,60 @@
                                                 y = new Qe(d + "*", f, !1, !1, !1),
                                                 v = new Qe(d + " const*", f, !1, !0, !1);
                                             return Ie[e] = {
                                                     pointerType: y,
                                                     constPointerType: v
                                                 },
                                                 function(e, r, n) {
-                                                    t.hasOwnProperty(e) || Ae("Replacing nonexistant public symbol"), t[e].overloadTable, t[e] = r, t[e].argCount = void 0
+                                                    t.hasOwnProperty(e) || xe("Replacing nonexistant public symbol"), t[e].overloadTable, t[e] = r, t[e].argCount = void 0
                                                 }(p, i), [m, y, v]
                                         }))
                                     },
                                     f: function(e, t, r, n, o, a, s) {
                                         var i = it(r, n);
-                                        t = ve(t), a = et(o, a), xe([], [e], (function(e) {
+                                        t = ve(t), a = et(o, a), Ae([], [e], (function(e) {
                                             var n = (e = e[0]).name + "." + t;
 
                                             function o() {
                                                 nt("Cannot call " + n + " due to unbound types", i)
                                             }
                                             t.startsWith("@@") && (t = Symbol[t.substring(2)]);
                                             var c = e.registeredClass.constructor;
-                                            return void 0 === c[t] ? (o.argCount = r - 1, c[t] = o) : (qe(c, t, n), c[t].overloadTable[r - 1] = o), xe([], i, (function(e) {
+                                            return void 0 === c[t] ? (o.argCount = r - 1, c[t] = o) : (He(c, t, n), c[t].overloadTable[r - 1] = o), Ae([], i, (function(e) {
                                                 var o = [e[0], null].concat(e.slice(1)),
                                                     i = st(n, o, null, a, s);
                                                 return void 0 === c[t].overloadTable ? (i.argCount = r - 1, c[t] = i) : c[t].overloadTable[r - 1] = i, []
                                             })), []
                                         }))
                                     },
                                     e: function(e, t, r, n, o, a) {
                                         v(t > 0);
                                         var s = it(t, r);
-                                        o = et(n, o), xe([], [e], (function(e) {
+                                        o = et(n, o), Ae([], [e], (function(e) {
                                             var r = "constructor " + (e = e[0]).name;
                                             if (void 0 === e.registeredClass.constructor_body && (e.registeredClass.constructor_body = []), void 0 !== e.registeredClass.constructor_body[t - 1]) throw new Te("Cannot register multiple constructors with identical number of parameters (" + (t - 1) + ") for class '" + e.name + "'! Overload resolution is currently only performed using the parameter count, not actual type info!");
                                             return e.registeredClass.constructor_body[t - 1] = () => {
                                                 nt("Cannot construct " + e.name + " due to unbound types", s)
-                                            }, xe([], s, (function(n) {
+                                            }, Ae([], s, (function(n) {
                                                 return n.splice(1, 0, null), e.registeredClass.constructor_body[t - 1] = st(r, n, null, o, a), []
                                             })), []
                                         }))
                                     },
                                     c: function(e, t, r, n, o, a, s, i) {
                                         var c = it(r, n);
-                                        t = ve(t), a = et(o, a), xe([], [e], (function(e) {
+                                        t = ve(t), a = et(o, a), Ae([], [e], (function(e) {
                                             var n = (e = e[0]).name + "." + t;
 
                                             function o() {
                                                 nt("Cannot call " + n + " due to unbound types", c)
                                             }
                                             t.startsWith("@@") && (t = Symbol[t.substring(2)]), i && e.registeredClass.pureVirtualFunctions.push(t);
                                             var u = e.registeredClass.instancePrototype,
                                                 l = u[t];
-                                            return void 0 === l || void 0 === l.overloadTable && l.className !== e.name && l.argCount === r - 2 ? (o.argCount = r - 2, o.className = e.name, u[t] = o) : (qe(u, t, n), u[t].overloadTable[r - 2] = o), xe([], c, (function(o) {
+                                            return void 0 === l || void 0 === l.overloadTable && l.className !== e.name && l.argCount === r - 2 ? (o.argCount = r - 2, o.className = e.name, u[t] = o) : (He(u, t, n), u[t].overloadTable[r - 2] = o), Ae([], c, (function(o) {
                                                 var i = st(n, o, e, a, s);
                                                 return void 0 === u[t].overloadTable ? (i.argCount = r - 2, u[t] = i) : u[t].overloadTable[r - 2] = i, []
                                             })), []
                                         }))
                                     },
                                     U: function(e, t) {
                                         Oe(e, {
@@ -8231,15 +8231,15 @@
                                             destructorFunction: null
                                         })
                                     },
                                     g: function(e, t, r) {
                                         var n = [Int8Array, Uint8Array, Int16Array, Uint16Array, Int32Array, Uint32Array, Float32Array, Float64Array][t];
 
                                         function o(e) {
-                                            var t = x,
+                                            var t = A,
                                                 r = t[(e >>= 2) >>> 0],
                                                 o = t[e + 1 >>> 0];
                                             return new n(S, o, r)
                                         }
                                         Oe(e, {
                                             name: r = ve(r),
                                             fromWireType: o,
@@ -8250,75 +8250,75 @@
                                         })
                                     },
                                     w: function(e, t) {
                                         var r = "std::string" === (t = ve(t));
                                         Oe(e, {
                                             name: t,
                                             fromWireType: function(e) {
-                                                var t, n = x[e >>> 2];
+                                                var t, n = A[e >>> 2];
                                                 if (r)
                                                     for (var o = e + 4, a = 0; a <= n; ++a) {
                                                         var s = e + 4 + a;
                                                         if (a == n || 0 == T[s >>> 0]) {
                                                             var i = _(o, s - o);
                                                             void 0 === t ? t = i : (t += String.fromCharCode(0), t += i), o = s + 1
                                                         }
                                                     } else {
                                                         var c = new Array(n);
                                                         for (a = 0; a < n; ++a) c[a] = String.fromCharCode(T[e + 4 + a >>> 0]);
                                                         t = c.join("")
                                                     }
-                                                return qt(e), t
+                                                return Ht(e), t
                                             },
                                             toWireType: function(e, t) {
                                                 t instanceof ArrayBuffer && (t = new Uint8Array(t));
                                                 var n = "string" == typeof t;
                                                 n || t instanceof Uint8Array || t instanceof Uint8ClampedArray || t instanceof Int8Array || ke("Cannot pass non-string to std::string");
                                                 var o = (r && n ? () => $(t) : () => t.length)(),
-                                                    a = Ht(4 + o + 1);
-                                                if (x[(a >>>= 0) >>> 2] = o, r && n) E(t, a + 4, o + 1);
+                                                    a = qt(4 + o + 1);
+                                                if (A[(a >>>= 0) >>> 2] = o, r && n) E(t, a + 4, o + 1);
                                                 else if (n)
                                                     for (var s = 0; s < o; ++s) {
                                                         var i = t.charCodeAt(s);
-                                                        i > 255 && (qt(a), ke("String has UTF-16 code units that do not fit in 8 bits")), T[a + 4 + s >>> 0] = i
+                                                        i > 255 && (Ht(a), ke("String has UTF-16 code units that do not fit in 8 bits")), T[a + 4 + s >>> 0] = i
                                                     } else
                                                         for (s = 0; s < o; ++s) T[a + 4 + s >>> 0] = t[s];
-                                                return null !== e && e.push(qt, a), a
+                                                return null !== e && e.push(Ht, a), a
                                             },
                                             argPackAdvance: 8,
                                             readValueFromPointer: Ze,
                                             destructorFunction: function(e) {
-                                                qt(e)
+                                                Ht(e)
                                             }
                                         })
                                     },
                                     r: function(e, t, r) {
                                         var n, o, a, s, i;
-                                        r = ve(r), 2 === t ? (n = D, o = R, s = M, a = () => C, i = 1) : 4 === t && (n = I, o = F, s = V, a = () => x, i = 2), Oe(e, {
+                                        r = ve(r), 2 === t ? (n = D, o = R, s = M, a = () => C, i = 1) : 4 === t && (n = I, o = F, s = V, a = () => A, i = 2), Oe(e, {
                                             name: r,
                                             fromWireType: function(e) {
-                                                for (var r, o = x[e >>> 2], s = a(), c = e + 4, u = 0; u <= o; ++u) {
+                                                for (var r, o = A[e >>> 2], s = a(), c = e + 4, u = 0; u <= o; ++u) {
                                                     var l = e + 4 + u * t;
                                                     if (u == o || 0 == s[l >>> i]) {
                                                         var d = n(c, l - c);
                                                         void 0 === r ? r = d : (r += String.fromCharCode(0), r += d), c = l + t
                                                     }
                                                 }
-                                                return qt(e), r
+                                                return Ht(e), r
                                             },
                                             toWireType: function(e, n) {
                                                 "string" != typeof n && ke("Cannot pass non-string to C++ string type " + r);
                                                 var a = s(n),
-                                                    c = Ht(4 + a + t);
-                                                return x[(c >>>= 0) >>> 2] = a >> i, o(n, c + 4, a + t), null !== e && e.push(qt, c), c
+                                                    c = qt(4 + a + t);
+                                                return A[(c >>>= 0) >>> 2] = a >> i, o(n, c + 4, a + t), null !== e && e.push(Ht, c), c
                                             },
                                             argPackAdvance: 8,
                                             readValueFromPointer: Ze,
                                             destructorFunction: function(e) {
-                                                qt(e)
+                                                Ht(e)
                                             }
                                         })
                                     },
                                     W: function(e, t) {
                                         Oe(e, {
                                             isVoid: !0,
                                             name: t = ve(t),
@@ -8333,29 +8333,29 @@
                                     L: function() {
                                         return !0
                                     },
                                     m: function(e, t, r) {
                                         e = dt.toValue(e), t = ht(t, "emval::as");
                                         var n = [],
                                             o = dt.toHandle(n);
-                                        return A[r >>> 2] = o, t.toWireType(n, e)
+                                        return x[r >>> 2] = o, t.toWireType(n, e)
                                     },
                                     ka: function(e, t, r, n, o) {
                                         return (e = wt[e])(t = dt.toValue(t), r = gt(r), function(e) {
                                             var t = [];
-                                            return A[e >>> 2] = dt.toHandle(t), t
+                                            return x[e >>> 2] = dt.toHandle(t), t
                                         }(n), o)
                                     },
                                     x: lt,
                                     la: function(e) {
                                         return 0 === e ? dt.toHandle(_t()) : (e = gt(e), dt.toHandle(_t()[e]))
                                     },
                                     ja: function(e, t) {
                                         var r = function(e, t) {
-                                                for (var r = new Array(e), n = 0; n < e; ++n) r[n] = ht(x[t + 4 * n >>> 2], "parameter " + n);
+                                                for (var r = new Array(e), n = 0; n < e; ++n) r[n] = ht(A[t + 4 * n >>> 2], "parameter " + n);
                                                 return r
                                             }(e, t),
                                             n = r[0],
                                             o = n.name + "_$" + r.slice(1).map((function(e) {
                                                 return e.name
                                             })).join("_") + "$",
                                             a = bt[o];
@@ -8386,23 +8386,23 @@
                                         var r = (e = ht(e, "_emval_take_value")).readValueFromPointer(t);
                                         return dt.toHandle(r)
                                     },
                                     ma: function(e) {
                                         return e = dt.toValue(e), dt.toHandle(typeof e)
                                     },
                                     N: function(e, t) {
-                                        var r = new Date(1e3 * A[e >>> 2]);
-                                        A[t >>> 2] = r.getSeconds(), A[t + 4 >>> 2] = r.getMinutes(), A[t + 8 >>> 2] = r.getHours(), A[t + 12 >>> 2] = r.getDate(), A[t + 16 >>> 2] = r.getMonth(), A[t + 20 >>> 2] = r.getFullYear() - 1900, A[t + 24 >>> 2] = r.getDay();
+                                        var r = new Date(1e3 * x[e >>> 2]);
+                                        x[t >>> 2] = r.getSeconds(), x[t + 4 >>> 2] = r.getMinutes(), x[t + 8 >>> 2] = r.getHours(), x[t + 12 >>> 2] = r.getDate(), x[t + 16 >>> 2] = r.getMonth(), x[t + 20 >>> 2] = r.getFullYear() - 1900, x[t + 24 >>> 2] = r.getDay();
                                         var n = new Date(r.getFullYear(), 0, 1),
                                             o = (r.getTime() - n.getTime()) / 864e5 | 0;
-                                        A[t + 28 >>> 2] = o, A[t + 36 >>> 2] = -60 * r.getTimezoneOffset();
+                                        x[t + 28 >>> 2] = o, x[t + 36 >>> 2] = -60 * r.getTimezoneOffset();
                                         var a = new Date(r.getFullYear(), 6, 1).getTimezoneOffset(),
                                             s = n.getTimezoneOffset(),
                                             i = 0 | (a != s && r.getTimezoneOffset() == Math.min(s, a));
-                                        A[t + 32 >>> 2] = i
+                                        x[t + 32 >>> 2] = i
                                     },
                                     D: function(e, t, r, n, o, a) {
                                         try {
                                             e >>>= 0;
                                             var s = he.getStream(o);
                                             s && (2 & r && pe.doMsync(e, s, t, n, a), he.munmap(s))
                                         } catch (e) {
@@ -8419,20 +8419,20 @@
                                                 i = a.getTimezoneOffset(),
                                                 c = Math.max(s, i);
 
                                             function u(e) {
                                                 var t = e.toTimeString().match(/\(([A-Za-z ]+)\)$/);
                                                 return t ? t[1] : "GMT"
                                             }
-                                            A[e >>> 2] = 60 * c, A[t >>> 2] = Number(s != i);
+                                            x[e >>> 2] = 60 * c, x[t >>> 2] = Number(s != i);
                                             var l = u(o),
                                                 d = u(a),
                                                 f = L(l),
                                                 h = L(d);
-                                            i < s ? (x[r >>> 2] = f, x[r + 4 >>> 2] = h) : (x[r >>> 2] = h, x[r + 4 >>> 2] = f)
+                                            i < s ? (A[r >>> 2] = f, A[r + 4 >>> 2] = h) : (A[r >>> 2] = h, A[r + 4 >>> 2] = f)
                                         }(t, r, n))
                                     },
                                     t: function() {
                                         te("")
                                     },
                                     C: function() {
                                         return 4294901760
@@ -8450,28 +8450,28 @@
                                         }
                                         return !1
                                     },
                                     E: function(e, t) {
                                         var r = 0;
                                         return St().forEach((function(n, o) {
                                             var a = t + r;
-                                            x[e + 4 * o >>> 2] = a,
+                                            A[e + 4 * o >>> 2] = a,
                                                 function(e, t, r) {
                                                     for (var n = 0; n < e.length; ++n) P[t++ >>> 0] = e.charCodeAt(n);
                                                     P[t >>> 0] = 0
                                                 }(n, a), r += n.length + 1
                                         })), 0
                                     },
                                     F: function(e, t) {
                                         var r = St();
-                                        x[e >>> 2] = r.length;
+                                        A[e >>> 2] = r.length;
                                         var n = 0;
                                         return r.forEach((function(e) {
                                             n += e.length + 1
-                                        })), x[t >>> 2] = n, 0
+                                        })), A[t >>> 2] = n, 0
                                     },
                                     ha: function(e) {
                                         ! function(e, r) {
                                             var n;
                                             n = e, m || (t.onExit && t.onExit(n), y = !0), u(n, new Xt(n))
                                         }(e)
                                     },
@@ -8484,160 +8484,160 @@
                                             return e.errno
                                         }
                                     },
                                     S: function(e, t, r, n) {
                                         try {
                                             var o = function(e, t, r, n) {
                                                 for (var o = 0, a = 0; a < r; a++) {
-                                                    var s = x[t >>> 2],
-                                                        i = x[t + 4 >>> 2];
+                                                    var s = A[t >>> 2],
+                                                        i = A[t + 4 >>> 2];
                                                     t += 8;
                                                     var c = he.read(e, P, s, i, void 0);
                                                     if (c < 0) return -1;
                                                     if (o += c, c < i) break
                                                 }
                                                 return o
                                             }(pe.getStreamFromFD(e), t, r);
-                                            return A[n >>> 2] = o, 0
+                                            return x[n >>> 2] = o, 0
                                         } catch (e) {
                                             if (void 0 === he || !(e instanceof he.ErrnoError)) throw e;
                                             return e.errno
                                         }
                                     },
                                     y: function(e, t, r, n, o) {
                                         try {
                                             var a = (c = r) + 2097152 >>> 0 < 4194305 - !!(i = t) ? (i >>> 0) + 4294967296 * c : NaN;
                                             if (isNaN(a)) return 61;
                                             var s = pe.getStreamFromFD(e);
-                                            return he.llseek(s, a, n), W = [s.position >>> 0, (q = s.position, +Math.abs(q) >= 1 ? q > 0 ? (0 | Math.min(+Math.floor(q / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((q - +(~~q >>> 0)) / 4294967296) >>> 0 : 0)], A[o >>> 2] = W[0], A[o + 4 >>> 2] = W[1], s.getdents && 0 === a && 0 === n && (s.getdents = null), 0
+                                            return he.llseek(s, a, n), W = [s.position >>> 0, (H = s.position, +Math.abs(H) >= 1 ? H > 0 ? (0 | Math.min(+Math.floor(H / 4294967296), 4294967295)) >>> 0 : ~~+Math.ceil((H - +(~~H >>> 0)) / 4294967296) >>> 0 : 0)], x[o >>> 2] = W[0], x[o + 4 >>> 2] = W[1], s.getdents && 0 === a && 0 === n && (s.getdents = null), 0
                                         } catch (e) {
                                             if (void 0 === he || !(e instanceof he.ErrnoError)) throw e;
                                             return e.errno
                                         }
                                         var i, c
                                     },
                                     R: function(e, t, r, n) {
                                         try {
                                             var o = function(e, t, r, n) {
                                                 for (var o = 0, a = 0; a < r; a++) {
-                                                    var s = x[t >>> 2],
-                                                        i = x[t + 4 >>> 2];
+                                                    var s = A[t >>> 2],
+                                                        i = A[t + 4 >>> 2];
                                                     t += 8;
                                                     var c = he.write(e, P, s, i, void 0);
                                                     if (c < 0) return -1;
                                                     o += c
                                                 }
                                                 return o
                                             }(pe.getStreamFromFD(e), t, r);
-                                            return x[n >>> 2] = o, 0
+                                            return A[n >>> 2] = o, 0
                                         } catch (e) {
                                             if (void 0 === he || !(e instanceof he.ErrnoError)) throw e;
                                             return e.errno
                                         }
                                     },
                                     ga: function(e) {
                                         return function(e) {
-                                            var t = Ht(20),
-                                                r = Ht(e.length + 1);
-                                            E(e, r, e.length + 1), x[t >>> 2] = r;
-                                            var n = Ht(4);
-                                            x[n >>> 2] = 0, x[t + 4 >>> 2] = n, A[t + 8 >>> 2] = 2, A[t + 12 >>> 2] = 4;
-                                            var o = Ht(12);
-                                            return x[o >>> 2] = o + 8, x[o + 4 >>> 2] = 0, A[o + 8 >>> 2] = Pt(kt.lookup_name(e)), x[t + 16 >>> 2] = o, t
+                                            var t = qt(20),
+                                                r = qt(e.length + 1);
+                                            E(e, r, e.length + 1), A[t >>> 2] = r;
+                                            var n = qt(4);
+                                            A[n >>> 2] = 0, A[t + 4 >>> 2] = n, x[t + 8 >>> 2] = 2, x[t + 12 >>> 2] = 4;
+                                            var o = qt(12);
+                                            return A[o >>> 2] = o + 8, A[o + 4 >>> 2] = 0, x[o + 8 >>> 2] = Pt(kt.lookup_name(e)), A[t + 16 >>> 2] = o, t
                                         }(_(e))
                                     },
                                     ea: function(e, t) {
                                         if (t = _(t), e = Ct.programs[e]) {
                                             ! function(e) {
                                                 var t, r, n = e.uniformLocsById,
                                                     o = e.uniformSizeAndIdsByName;
                                                 if (!n)
                                                     for (e.uniformLocsById = n = {}, e.uniformArrayNamesById = {}, t = 0; t < Dt.getProgramParameter(e, 35718); ++t) {
                                                         var a = Dt.getActiveUniform(e, t),
                                                             s = a.name,
                                                             i = a.size,
-                                                            c = At(s),
+                                                            c = xt(s),
                                                             u = c > 0 ? s.slice(0, c) : s,
                                                             l = e.uniformIdCounter;
                                                         for (e.uniformIdCounter += i, o[u] = [i, l], r = 0; r < i; ++r) n[l] = r, e.uniformArrayNamesById[l++] = u
                                                     }
                                             }(e);
                                             var r = e.uniformLocsById,
                                                 n = 0,
                                                 o = t,
-                                                a = At(t);
+                                                a = xt(t);
                                             a > 0 && (n = Tt(t.slice(a + 1)) >>> 0, o = t.slice(0, a));
                                             var s = e.uniformSizeAndIdsByName[o];
                                             if (s && n < s[0] && (r[n += s[1]] = r[n] || Dt.getUniformLocation(e, t))) return n
                                         } else Ct.recordError(1281);
                                         return -1
                                     },
                                     ca: function(e, t) {
-                                        Dt.uniform1f(xt(e), t)
+                                        Dt.uniform1f(At(e), t)
                                     },
                                     da: function(e, t) {
-                                        Dt.uniform1i(xt(e), t)
+                                        Dt.uniform1i(At(e), t)
                                     },
                                     Z: function(e, t, r) {
                                         if (t <= 144)
                                             for (var n = Ot[2 * t - 1], o = 0; o < 2 * t; o += 2) n[o] = O[r + 4 * o >>> 2], n[o + 1] = O[r + (4 * o + 4) >>> 2];
                                         else n = O.subarray(r >>> 2, r + 8 * t >>> 2);
-                                        Dt.uniform2fv(xt(e), n)
+                                        Dt.uniform2fv(At(e), n)
                                     },
                                     ba: function(e, t, r) {
                                         if (t <= 144)
-                                            for (var n = Nt[2 * t - 1], o = 0; o < 2 * t; o += 2) n[o] = A[r + 4 * o >>> 2], n[o + 1] = A[r + (4 * o + 4) >>> 2];
-                                        else n = A.subarray(r >>> 2, r + 8 * t >>> 2);
-                                        Dt.uniform2iv(xt(e), n)
+                                            for (var n = Nt[2 * t - 1], o = 0; o < 2 * t; o += 2) n[o] = x[r + 4 * o >>> 2], n[o + 1] = x[r + (4 * o + 4) >>> 2];
+                                        else n = x.subarray(r >>> 2, r + 8 * t >>> 2);
+                                        Dt.uniform2iv(At(e), n)
                                     },
                                     Y: function(e, t, r) {
                                         if (t <= 96)
                                             for (var n = Ot[3 * t - 1], o = 0; o < 3 * t; o += 3) n[o] = O[r + 4 * o >>> 2], n[o + 1] = O[r + (4 * o + 4) >>> 2], n[o + 2] = O[r + (4 * o + 8) >>> 2];
                                         else n = O.subarray(r >>> 2, r + 12 * t >>> 2);
-                                        Dt.uniform3fv(xt(e), n)
+                                        Dt.uniform3fv(At(e), n)
                                     },
                                     aa: function(e, t, r) {
                                         if (t <= 96)
-                                            for (var n = Nt[3 * t - 1], o = 0; o < 3 * t; o += 3) n[o] = A[r + 4 * o >>> 2], n[o + 1] = A[r + (4 * o + 4) >>> 2], n[o + 2] = A[r + (4 * o + 8) >>> 2];
-                                        else n = A.subarray(r >>> 2, r + 12 * t >>> 2);
-                                        Dt.uniform3iv(xt(e), n)
+                                            for (var n = Nt[3 * t - 1], o = 0; o < 3 * t; o += 3) n[o] = x[r + 4 * o >>> 2], n[o + 1] = x[r + (4 * o + 4) >>> 2], n[o + 2] = x[r + (4 * o + 8) >>> 2];
+                                        else n = x.subarray(r >>> 2, r + 12 * t >>> 2);
+                                        Dt.uniform3iv(At(e), n)
                                     },
                                     X: function(e, t, r) {
                                         if (t <= 72) {
                                             var n = Ot[4 * t - 1],
                                                 o = O;
                                             r >>= 2;
                                             for (var a = 0; a < 4 * t; a += 4) {
                                                 var s = r + a;
                                                 n[a] = o[s >>> 0], n[a + 1] = o[s + 1 >>> 0], n[a + 2] = o[s + 2 >>> 0], n[a + 3] = o[s + 3 >>> 0]
                                             }
                                         } else n = O.subarray(r >>> 2, r + 16 * t >>> 2);
-                                        Dt.uniform4fv(xt(e), n)
+                                        Dt.uniform4fv(At(e), n)
                                     },
                                     $: function(e, t, r) {
                                         if (t <= 72)
-                                            for (var n = Nt[4 * t - 1], o = 0; o < 4 * t; o += 4) n[o] = A[r + 4 * o >>> 2], n[o + 1] = A[r + (4 * o + 4) >>> 2], n[o + 2] = A[r + (4 * o + 8) >>> 2], n[o + 3] = A[r + (4 * o + 12) >>> 2];
-                                        else n = A.subarray(r >>> 2, r + 16 * t >>> 2);
-                                        Dt.uniform4iv(xt(e), n)
+                                            for (var n = Nt[4 * t - 1], o = 0; o < 4 * t; o += 4) n[o] = x[r + 4 * o >>> 2], n[o + 1] = x[r + (4 * o + 4) >>> 2], n[o + 2] = x[r + (4 * o + 8) >>> 2], n[o + 3] = x[r + (4 * o + 12) >>> 2];
+                                        else n = x.subarray(r >>> 2, r + 16 * t >>> 2);
+                                        Dt.uniform4iv(At(e), n)
                                     },
                                     A: function(e) {},
                                     B: function(e, t, r, n) {
                                         return function(e, t, r, n) {
-                                            var o = A[n + 40 >>> 2],
+                                            var o = x[n + 40 >>> 2],
                                                 a = {
-                                                    tm_sec: A[n >>> 2],
-                                                    tm_min: A[n + 4 >>> 2],
-                                                    tm_hour: A[n + 8 >>> 2],
-                                                    tm_mday: A[n + 12 >>> 2],
-                                                    tm_mon: A[n + 16 >>> 2],
-                                                    tm_year: A[n + 20 >>> 2],
-                                                    tm_wday: A[n + 24 >>> 2],
-                                                    tm_yday: A[n + 28 >>> 2],
-                                                    tm_isdst: A[n + 32 >>> 2],
-                                                    tm_gmtoff: A[n + 36 >>> 2],
+                                                    tm_sec: x[n >>> 2],
+                                                    tm_min: x[n + 4 >>> 2],
+                                                    tm_hour: x[n + 8 >>> 2],
+                                                    tm_mday: x[n + 12 >>> 2],
+                                                    tm_mon: x[n + 16 >>> 2],
+                                                    tm_year: x[n + 20 >>> 2],
+                                                    tm_wday: x[n + 24 >>> 2],
+                                                    tm_yday: x[n + 28 >>> 2],
+                                                    tm_isdst: x[n + 32 >>> 2],
+                                                    tm_gmtoff: x[n + 36 >>> 2],
                                                     tm_zone: o ? _(o) : ""
                                                 },
                                                 s = _(r),
                                                 i = {
                                                     "%c": "%a %b %d %H:%M:%S %Y",
                                                     "%D": "%m/%d/%y",
                                                     "%F": "%Y-%m-%d",
@@ -8833,15 +8833,15 @@
                                             var v = Bt(s = s.replace(/\0\0/g, "%"), !1);
                                             return v.length > t ? 0 : (function(e, t) {
                                                 P.set(e, t >>> 0)
                                             }(v, e), v.length - 1)
                                         }(e, t, r, n)
                                     }
                                 },
-                                Ht = (function() {
+                                qt = (function() {
                                     var e = {
                                         a: zt
                                     };
 
                                     function r(e, r) {
                                         var n, o = e.exports;
                                         t.asm = o, B((p = t.asm.oa).buffer), U = t.asm.va, n = t.asm.pa, K.unshift(n), ee()
@@ -8879,18 +8879,18 @@
                                         return WebAssembly.instantiateStreaming(t, e).then(o, (function(e) {
                                             return h("wasm streaming compile failed: " + e), h("falling back to ArrayBuffer instantiation"), a(o)
                                         }))
                                     }))).catch(n)
                                 }(), t.___wasm_call_ctors = function() {
                                     return (t.___wasm_call_ctors = t.asm.pa).apply(null, arguments)
                                 }, t._malloc = function() {
-                                    return (Ht = t._malloc = t.asm.qa).apply(null, arguments)
+                                    return (qt = t._malloc = t.asm.qa).apply(null, arguments)
                                 }),
-                                qt = t._free = function() {
-                                    return (qt = t._free = t.asm.ra).apply(null, arguments)
+                                Ht = t._free = function() {
+                                    return (Ht = t._free = t.asm.ra).apply(null, arguments)
                                 },
                                 Wt = t.___errno_location = function() {
                                     return (Wt = t.___errno_location = t.asm.sa).apply(null, arguments)
                                 },
                                 Gt = t.___getTypeName = function() {
                                     return (Gt = t.___getTypeName = t.asm.ta).apply(null, arguments)
                                 },
@@ -9348,22 +9348,22 @@
                                     return this.map.get(e)
                                 }
                             },
                             C = !0;
                         try {
                             "undefined" != typeof localStorage && localStorage && (k = localStorage, C = !1)
                         } catch (e) {}
-                        const A = k,
-                            x = void 0 !== o && o.release && /node|io\.js/.test(o.release.name) && "[object process]" === Object.prototype.toString.call(void 0 !== o ? o : 0);
+                        const x = k,
+                            A = void 0 !== o && o.release && /node|io\.js/.test(o.release.name) && "[object process]" === Object.prototype.toString.call(void 0 !== o ? o : 0);
                         let O;
                         "undefined" != typeof navigator && /Mac/.test(navigator.platform);
                         const N = [],
                             j = e => (() => {
                                 if (void 0 === O)
-                                    if (x) {
+                                    if (A) {
                                         O = w();
                                         const e = o.argv;
                                         let t = null;
                                         for (let r = 0; r < e.length; r++) {
                                             const n = e[r];
                                             "-" === n[0] ? (null !== t && O.set(t, ""), t = n) : null !== t ? (O.set(t, n), t = null) : N.push(n)
                                         }
@@ -9373,21 +9373,21 @@
                                             const [t, r] = e.split("=");
                                             O.set(`--${$(t,"-")}`, r), O.set(`-${$(t,"-")}`, r)
                                         }
                                     }))) : O = w();
                                 return O
                             })().has(e),
                             D = e => {
-                                return void 0 === (t = x ? o.env[e.toUpperCase().replaceAll("-", "_")] : A.getItem(e)) ? null : t;
+                                return void 0 === (t = A ? o.env[e.toUpperCase().replaceAll("-", "_")] : x.getItem(e)) ? null : t;
                                 var t
                             };
                         j("--production") || D("production");
-                        const R = x && (M = o.env.FORCE_COLOR, ["true", "1", "2"].includes(M));
+                        const R = A && (M = o.env.FORCE_COLOR, ["true", "1", "2"].includes(M));
                         var M;
-                        !j("no-colors") && (!x || o.stdout.isTTY || R) && (!x || j("color") || R || null !== D("COLORTERM") || (D("TERM") || "").includes("color"));
+                        !j("no-colors") && (!A || o.stdout.isTTY || R) && (!A || j("color") || R || null !== D("COLORTERM") || (D("TERM") || "").includes("color"));
                         class I {
                             constructor(e, t) {
                                 this.left = e, this.right = t
                             }
                         }
                         const F = (e, t) => new I(e, t),
                             V = "undefined" != typeof document ? document : {},
@@ -9399,19 +9399,19 @@
                             }
                         }, U = new Map, new class {
                             constructor(e, t) {
                                 this.ds = e, this.sv = t
                             }
                         }(B, U), Symbol.iterator, Symbol.iterator, Symbol.iterator;
                         const z = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : void 0 !== r.g ? r.g : {},
-                            H = "__ $YJS$ __";
-                        let q;
+                            q = "__ $YJS$ __";
+                        let H;
 
                         function W() {
-                            return q || (q = self.occ), q
+                            return H || (H = self.occ), H
                         }
 
                         function G(e) {
                             return Math.PI * e / 180
                         }
 
                         function K(e, t) {
@@ -9419,15 +9419,15 @@
                             const r = W(),
                                 n = new r.gp_Trsf_1,
                                 o = new r.gp_Ax1_2(new r.gp_Pnt_3(0, 0, 0), new r.gp_Dir_4(t.Axis[0], t.Axis[1], t.Axis[2])),
                                 a = G(t.Angle);
                             n.SetRotation_1(o, a), n.SetTranslationPart(new r.gp_Vec_4(t.Position[0], t.Position[1], t.Position[2]));
                             const s = new r.TopLoc_Location_2(n);
                             return e.Location_2(s, !0), e
-                        }!0 === z[H] && console.error("Yjs was already imported. This breaks constructor checks and will lead to issues! - https://github.com/yjs/yjs/issues/438"), z[H] = !0, new y.Token("jupyterCadDocTracker"), new y.Token("jupytercadAnnotationModel"), new y.Token("jupytercadWorkerRegistry"), new y.Token("jupytercadFormSchemaRegistry"), new y.Token("jupytercadExternalCommandRegistry");
+                        }!0 === z[q] && console.error("Yjs was already imported. This breaks constructor checks and will lead to issues! - https://github.com/yjs/yjs/issues/438"), z[q] = !0, new y.Token("jupyterCadDocTracker"), new y.Token("jupytercadAnnotationModel"), new y.Token("jupytercadWorkerRegistry"), new y.Token("jupytercadFormSchemaRegistry"), new y.Token("jupytercadExternalCommandRegistry");
                         const Y = {
                             "Part::Any": void 0,
                             "Part::Box": void 0,
                             "Part::Cylinder": void 0,
                             "Part::Sphere": void 0,
                             "Part::Cone": void 0,
                             "Part::Torus": void 0,
@@ -9468,16 +9468,60 @@
                                     r = (re[e[t + 0]] + re[e[t + 1]] + re[e[t + 2]] + re[e[t + 3]] + "-" + re[e[t + 4]] + re[e[t + 5]] + "-" + re[e[t + 6]] + re[e[t + 7]] + "-" + re[e[t + 8]] + re[e[t + 9]] + "-" + re[e[t + 10]] + re[e[t + 11]] + re[e[t + 12]] + re[e[t + 13]] + re[e[t + 14]] + re[e[t + 15]]).toLowerCase();
                                 if (! function(e) {
                                         return "string" == typeof e && te.test(e)
                                     }(r)) throw TypeError("Stringified UUID is invalid");
                                 return r
                             }(n)
                         };
+                        class ae {
+                            constructor(e, t) {
+                                this._Idx1 = e, this._Idx2 = t
+                            }
+                            get Idx1() {
+                                return this._Idx1
+                            }
+                            get Idx2() {
+                                return this._Idx2
+                            }
+                            get hashStr() {
+                                return `${this.Idx1}@${this.Idx2}`
+                            }
+                            equal(e) {
+                                return this.hashStr === e.hashStr
+                            }
+                        }
+                        class se {
+                            constructor() {
+                                this._internalMap = new Map, this._currentIdx = 0
+                            }
+                            add(e, t) {
+                                const r = this._hash(e),
+                                    n = this._internalMap.get(r);
+                                return n ? n.index : (this._currentIdx += 1, this._internalMap.set(r, {
+                                    index: this._currentIdx,
+                                    value: t
+                                }), this._currentIdx)
+                            }
+                            findFromKey(e) {
+                                var t;
+                                const r = this._hash(e);
+                                return null === (t = this._internalMap.get(r)) || void 0 === t ? void 0 : t.value
+                            }
+                            contains(e) {
+                                const t = this._hash(e);
+                                return this._internalMap.has(t)
+                            }
+                            _hash(e) {
+                                if (e.hashStr) return e.hashStr;
+                                if ("number" == typeof e || "string" == typeof e) return e + "";
+                                throw new Error("Key type is not supported")
+                            }
+                        }
 
-                        function ae(e) {
+                        function ie(e) {
                             switch (e.type.toLowerCase()) {
                                 case "brep":
                                     return function(e) {
                                         const t = W(),
                                             r = `${oe()}.brep`;
                                         t.FS.createDataFile("/", r, e, !0, !0, !0);
                                         const n = new t.TopoDS_Shape,
@@ -9507,138 +9551,135 @@
                                                 if (e.IsNull()) return;
                                                 const t = e.get();
                                                 if (0 === t.NbNodes() || 0 === t.NbTriangles()) return;
                                                 const r = 1e-9,
                                                     n = W(),
                                                     o = t.NbNodes(),
                                                     a = t.NbTriangles(),
-                                                    s = new Map;
-                                                for (let e = 1; e <= o; e++) {
+                                                    s = new se;
+                                                for (let e = 1; e <= o; ++e) {
                                                     const r = t.Node(e),
                                                         o = new n.BRepBuilderAPI_MakeVertex(r);
-                                                    s.set(e, o.Vertex())
+                                                    s.add(e, o.Vertex())
                                                 }
-                                                const i = new Map;
-                                                for (let e = 1; e <= a; e++) {
+                                                const i = new se;
+                                                for (let e = 1; e <= a; ++e) {
                                                     const o = t.Triangle(e),
                                                         a = [o.Value(1), o.Value(2), o.Value(3)];
                                                     if (a[0] === a[1] || a[0] === a[2] || a[1] === a[2]) continue;
                                                     const c = t.Node(a[0]),
                                                         u = t.Node(a[1]),
                                                         l = t.Node(a[2]),
                                                         d = c.SquareDistance(u),
                                                         f = c.SquareDistance(l),
                                                         h = u.SquareDistance(l);
                                                     if (d < r || f < r || h < r) continue;
-                                                    const p = s.get(a[0]),
-                                                        m = s.get(a[1]),
-                                                        y = s.get(a[2]);
+                                                    const p = s.findFromKey(a[0]),
+                                                        m = s.findFromKey(a[1]),
+                                                        y = s.findFromKey(a[2]);
                                                     if (!p || !m || !y) return;
-                                                    const v = [Math.min(a[0], a[1]), Math.max(a[0], a[1])],
-                                                        g = [Math.min(a[1], a[2]), Math.max(a[1], a[2])],
-                                                        w = [Math.min(a[2], a[0]), Math.max(a[2], a[0])],
+                                                    const v = new ae(a[0], a[1]),
+                                                        g = new ae(a[1], a[2]),
+                                                        w = new ae(a[2], a[0]),
                                                         _ = new n.BRepBuilderAPI_MakeEdge_2(p, m).Edge();
                                                     a[1] < a[0] && _.Reverse();
                                                     const b = new n.BRepBuilderAPI_MakeEdge_2(m, y).Edge();
                                                     a[2] < a[1] && b.Reverse();
                                                     const E = new n.BRepBuilderAPI_MakeEdge_2(y, p).Edge();
-                                                    a[0] < a[2] && E.Reverse(), i.set(`${v[0]}:${v[1]}`, _), i.set(`${g[0]}:${g[1]}`, b), i.set(`${w[0]}:${w[1]}`, E)
+                                                    a[0] < a[2] && E.Reverse(), i.add(v, _), i.add(g, b), i.add(w, E)
                                                 }
                                                 const c = new n.TopoDS_Compound,
                                                     u = new n.BRep_Builder;
                                                 u.MakeCompound(c);
                                                 for (let e = 1; e <= a; e++) {
                                                     const o = t.Triangle(e),
                                                         a = [o.Value(1), o.Value(2), o.Value(3)],
-                                                        s = [Math.min(a[0], a[1]), Math.max(a[0], a[1])],
-                                                        l = [Math.min(a[1], a[2]), Math.max(a[1], a[2])],
-                                                        d = [Math.min(a[2], a[0]), Math.max(a[2], a[0])],
+                                                        s = new ae(a[0], a[1]),
+                                                        l = new ae(a[1], a[2]),
+                                                        d = new ae(a[2], a[0]),
                                                         f = a[1] < a[0],
                                                         h = a[2] < a[1],
-                                                        p = a[0] < a[2],
-                                                        m = `${s[0]}:${s[1]}`,
-                                                        y = `${l[0]}:${l[1]}`,
-                                                        v = `${d[0]}:${d[1]}`;
-                                                    if (!(i.has(m) && i.has(y) && i.has(v))) continue;
-                                                    const g = i.get(m),
-                                                        w = i.get(y),
-                                                        _ = i.get(v);
-                                                    if (!g || !w || !_) continue;
-                                                    f && g.Reverse(), h && w.Reverse(), p && _.Reverse();
-                                                    const b = new n.BRepBuilderAPI_MakeWire_1;
-                                                    b.Add_1(g), b.Add_1(w), b.Add_1(_);
-                                                    const E = b.Wire(),
-                                                        $ = new n.BRepAdaptor_Curve_2(g),
-                                                        S = new n.BRepAdaptor_Curve_2(w),
-                                                        P = $.Line().Direction(),
-                                                        T = S.Line().Direction(),
-                                                        k = P.XYZ().Crossed(T.XYZ());
-                                                    if (k.SquareModulus() < r) continue;
-                                                    g.Orientation_1() === n.TopAbs_Orientation.TopAbs_REVERSED && k.Reverse(), w.Orientation_1() === n.TopAbs_Orientation.TopAbs_REVERSED && k.Reverse();
-                                                    const C = new n.gp_Dir_3(k),
-                                                        A = new n.gp_Pln_3(t.Node(a[0]), C),
-                                                        x = new n.BRepBuilderAPI_MakeFace_16(A, E, !0).Face();
-                                                    u.Add(c, x)
+                                                        p = a[0] < a[2];
+                                                    if (!(i.contains(s) && i.contains(l) && i.contains(d))) continue;
+                                                    const m = i.findFromKey(s),
+                                                        y = i.findFromKey(l),
+                                                        v = i.findFromKey(d);
+                                                    if (!m || !y || !v) continue;
+                                                    f && m.Reverse(), h && y.Reverse(), p && v.Reverse();
+                                                    const g = new n.BRepBuilderAPI_MakeWire_1;
+                                                    g.Add_1(m), g.Add_1(y), g.Add_1(v);
+                                                    const w = g.Wire(),
+                                                        _ = new n.BRepAdaptor_Curve_2(m),
+                                                        b = new n.BRepAdaptor_Curve_2(y),
+                                                        E = _.Line().Direction(),
+                                                        $ = b.Line().Direction(),
+                                                        S = E.XYZ().Crossed($.XYZ());
+                                                    if (S.SquareModulus() < r) continue;
+                                                    m.Orientation_1() === n.TopAbs_Orientation.TopAbs_REVERSED && S.Reverse(), y.Orientation_1() === n.TopAbs_Orientation.TopAbs_REVERSED && S.Reverse();
+                                                    const P = new n.gp_Dir_3(S),
+                                                        T = new n.gp_Pln_3(t.Node(a[0]), P),
+                                                        k = new n.BRepBuilderAPI_MakeFace_16(T, w, !0).Face();
+                                                    u.Add(c, k)
                                                 }
                                                 return c
                                             }(t.RWStl.ReadFile_2(r, new t.Message_ProgressRange_1)) || void console.error("Something in OCCT went wrong trying to read")
                                     }(e.content);
                                 default:
                                     throw `${e.type} file not supported`
                             }
                         }
-                        const se = new Map,
-                            ie = ["Part::Box", "Part::Cylinder", "Part::Sphere", "Part::Cone", "Part::Torus"],
-                            ce = ["Part::Cut", "Part::MultiFuse", "Part::Extrusion", "Part::MultiCommon", "Part::Chamfer", "Part::Fillet"],
-                            ue = ["ObjectFile", "Sketcher::SketchObject", "Part::Any"];
+                        const ce = new Map,
+                            ue = ["Part::Box", "Part::Cylinder", "Part::Sphere", "Part::Cone", "Part::Torus"],
+                            le = ["Part::Cut", "Part::MultiFuse", "Part::Extrusion", "Part::MultiCommon", "Part::Chamfer", "Part::Fillet"],
+                            de = ["ObjectFile", "Sketcher::SketchObject", "Part::Any"];
 
-                        function le(e, t, r) {
+                        function fe(e, t, r) {
                             const n = {};
-                            if (ie.includes(e)) n[e] = t;
-                            else if (ce.includes(e)) switch (e) {
+                            if (ue.includes(e)) n[e] = t;
+                            else if (le.includes(e)) switch (e) {
                                 case "Part::Cut": {
                                     const o = JSON.parse(JSON.stringify(t)),
                                         {
                                             Base: a,
                                             Tool: s
                                         } = o,
                                         i = r.objects.filter((e => e.name === a)),
                                         c = r.objects.filter((e => e.name === s));
-                                    i.length > 0 && (o.Base = le(i[0].shape, i[0].parameters, r)), c.length > 0 && (o.Tool = le(c[0].shape, c[0].parameters, r)), n[e] = o;
+                                    i.length > 0 && (o.Base = fe(i[0].shape, i[0].parameters, r)), c.length > 0 && (o.Tool = fe(c[0].shape, c[0].parameters, r)), n[e] = o;
                                     break
                                 }
                                 case "Part::Extrusion":
                                 case "Part::Fillet":
                                 case "Part::Chamfer": {
                                     const o = JSON.parse(JSON.stringify(t)),
                                         {
                                             Base: a
                                         } = o,
                                         s = r.objects.filter((e => e.name === a));
-                                    s.length > 0 && (o.Base = le(s[0].shape, s[0].parameters, r)), n[e] = o;
+                                    s.length > 0 && (o.Base = fe(s[0].shape, s[0].parameters, r)), n[e] = o;
                                     break
                                 }
                                 case "Part::MultiCommon":
                                 case "Part::MultiFuse": {
                                     const o = JSON.parse(JSON.stringify(t)),
                                         {
                                             Shapes: a
                                         } = o,
                                         s = [];
                                     a.forEach((e => {
                                         const t = r.objects.filter((t => t.name === e));
-                                        t.length > 0 && s.push(le(t[0].shape, t[0].parameters, r))
+                                        t.length > 0 && s.push(fe(t[0].shape, t[0].parameters, r))
                                     })), o.Shapes = s, n[e] = o;
                                     break
                                 }
-                            } else ue.includes(e), n[e] = t;
+                            } else de.includes(e), n[e] = t;
                             return n
                         }
 
-                        function de(e) {
+                        function he(e) {
                             const t = W(),
                                 r = new t.GProp_GProps_1;
                             t.BRepGProp.VolumeProperties_1(e, r, !1, !1, !1);
                             const n = r.Mass(),
                                 o = r.CentreOfMass(),
                                 a = r.MatrixOfInertia();
                             return {
@@ -9648,33 +9689,33 @@
                                     [a.Row(0).X(), a.Row(0).Y(), a.Row(0).Z()],
                                     [a.Row(1).X(), a.Row(1).Y(), a.Row(1).Z()],
                                     [a.Row(2).X(), a.Row(2).Y(), a.Row(2).Z()]
                                 ]
                             }
                         }
 
-                        function fe(e, t) {
+                        function pe(e, t) {
                             return (r, n) => {
-                                const o = le(e, r, n),
+                                const o = fe(e, r, n),
                                     a = `${function(e){let t=0;for(let r=0;r<e.length;r++)t=(t<<5)-t+e.charCodeAt(r),t|=0;return t}(JSON.stringify(o))}`;
-                                if (se.has(a)) return se.get(a);
+                                if (ce.has(a)) return ce.get(a);
                                 {
                                     const e = t(r, n);
                                     if (e) {
                                         const t = {
                                             occShape: e,
-                                            metadata: de(e)
+                                            metadata: he(e)
                                         };
-                                        return se.set(a, t), t
+                                        return ce.set(a, t), t
                                     }
                                 }
                             }
                         }
 
-                        function he(e, t) {
+                        function me(e, t) {
                             var r;
                             const n = t.objects.filter((t => t.name === e.Object));
                             if (0 === n.length) return {
                                 postShape: ""
                             };
                             const o = J(),
                                 a = n[0].shape;
@@ -9697,108 +9738,108 @@
                                 }
                             }
                             return {
                                 postShape: ""
                             }
                         }
 
-                        function pe(e) {
+                        function ye(e) {
                             const t = W(),
                                 r = new t.gp_Pnt_3(e.CenterX, e.CenterY, e.CenterZ),
                                 n = new t.gp_Dir_4(e.NormalX, e.NormalY, e.NormalZ),
                                 o = e.Radius,
                                 a = new t.GC_MakeCircle_6(r, n, o).Value(),
                                 s = new t.BRepBuilderAPI_MakeEdge_8(a.get().Circ()).Edge();
                             return new t.BRepBuilderAPI_MakeWire_2(s).Wire()
                         }
 
-                        function me(e) {
+                        function ve(e) {
                             const t = W(),
                                 r = new t.gp_Pnt_3(e.StartX, e.StartY, e.StartZ),
                                 n = new t.gp_Pnt_3(e.EndX, e.EndY, e.EndZ),
                                 o = new t.BRepBuilderAPI_MakeEdge_3(r, n).Edge();
                             return new t.BRepBuilderAPI_MakeWire_2(o).Wire()
                         }
-                        const ye = fe("Part::Any", (function(e, t) {
+                        const ge = pe("Part::Any", (function(e, t) {
                                 const {
                                     Content: r,
                                     Type: n,
                                     Placement: o
-                                } = e, a = ae({
+                                } = e, a = ie({
                                     content: r,
                                     type: n
                                 });
                                 if (a) return K(a, o)
                             })),
-                            ve = fe("Part::Box", (function(e, t) {
+                            we = pe("Part::Box", (function(e, t) {
                                 const {
                                     Length: r,
                                     Width: n,
                                     Height: o,
                                     Placement: a
                                 } = e;
                                 return K(new(W().BRepPrimAPI_MakeBox_2)(r, n, o).Shape(), a)
                             })),
-                            ge = fe("Part::Cylinder", (function(e, t) {
+                            _e = pe("Part::Cylinder", (function(e, t) {
                                 const {
                                     Radius: r,
                                     Height: n,
                                     Angle: o,
                                     Placement: a
                                 } = e;
                                 return K(new(W().BRepPrimAPI_MakeCylinder_2)(r, n, G(o)).Shape(), a)
                             })),
-                            we = fe("Part::Sphere", (function(e, t) {
+                            be = pe("Part::Sphere", (function(e, t) {
                                 const {
                                     Radius: r,
                                     Angle1: n,
                                     Angle2: o,
                                     Angle3: a,
                                     Placement: s
                                 } = e;
                                 return K(new(W().BRepPrimAPI_MakeSphere_4)(r, G(n), G(o), G(a)).Shape(), s)
                             })),
-                            _e = fe("Part::Cone", (function(e, t) {
+                            Ee = pe("Part::Cone", (function(e, t) {
                                 const {
                                     Radius1: r,
                                     Radius2: n,
                                     Height: o,
                                     Angle: a,
                                     Placement: s
                                 } = e;
                                 return K(new(W().BRepPrimAPI_MakeCone_2)(r, n, o, G(a)).Shape(), s)
                             })),
-                            be = fe("Part::Torus", (function(e, t) {
+                            $e = pe("Part::Torus", (function(e, t) {
                                 const {
                                     Radius1: r,
                                     Radius2: n,
                                     Angle1: o,
                                     Angle2: a,
                                     Angle3: s,
                                     Placement: i
                                 } = e;
                                 return K(new(W().BRepPrimAPI_MakeTorus_4)(r, n, G(o), G(a), G(s)).Shape(), i)
                             })),
-                            Ee = fe("Sketcher::SketchObject", (function(e, t) {
+                            Se = pe("Sketcher::SketchObject", (function(e, t) {
                                 const r = W(),
                                     n = new r.BRep_Builder,
                                     o = new r.TopoDS_Compound;
                                 if (0 !== e.Geometry.length) {
                                     n.MakeCompound(o);
                                     for (const t of e.Geometry) switch (t.TypeId) {
                                         case "Part::GeomCircle":
-                                            n.Add(o, pe(t));
+                                            n.Add(o, ye(t));
                                             break;
                                         case "Part::GeomLineSegment":
-                                            n.Add(o, me(t))
+                                            n.Add(o, ve(t))
                                     }
                                     return o
                                 }
                             })),
-                            $e = fe("Part::Cut", (function(e, t) {
+                            Pe = pe("Part::Cut", (function(e, t) {
                                 var r, n;
                                 const {
                                     Placement: o,
                                     Base: a,
                                     Tool: s
                                 } = e, i = W(), c = t.objects.filter((e => e.name === a)), u = t.objects.filter((e => e.name === s));
                                 if (0 === c.length || 0 === u.length) return;
@@ -9811,15 +9852,15 @@
                                     if (e && a && e.occShape && a.occShape) {
                                         c[0].visible = !1, u[0].visible = !1;
                                         const t = new i.BRepAlgoAPI_Cut_3(e.occShape, a.occShape, new i.Message_ProgressRange_1);
                                         if (t.IsDone()) return K(t.Shape(), o)
                                     }
                                 }
                             })),
-                            Se = fe("Part::MultiFuse", (function(e, t) {
+                            Te = pe("Part::MultiFuse", (function(e, t) {
                                 const r = W(),
                                     {
                                         Shapes: n,
                                         Placement: o
                                     } = e,
                                     a = [];
                                 n.forEach((e => {
@@ -9832,15 +9873,15 @@
                                         const e = null === (r = o[s]) || void 0 === r ? void 0 : r.call(o, n[0].parameters, t);
                                         e && e.occShape && (a.push(e.occShape), n[0].visible = !1)
                                     }
                                 }));
                                 const s = new r.BRepAlgoAPI_Fuse_3(a[0], a[1], new r.Message_ProgressRange_1);
                                 if (s.IsDone()) return K(s.Shape(), o)
                             })),
-                            Pe = fe("Part::MultiCommon", (function(e, t) {
+                            ke = pe("Part::MultiCommon", (function(e, t) {
                                 const r = W(),
                                     {
                                         Shapes: n,
                                         Placement: o
                                     } = e,
                                     a = [];
                                 n.forEach((e => {
@@ -9853,15 +9894,15 @@
                                         const e = null === (r = o[s]) || void 0 === r ? void 0 : r.call(o, n[0].parameters, t);
                                         e && e.occShape && (a.push(e.occShape), n[0].visible = !1)
                                     }
                                 }));
                                 const s = new r.BRepAlgoAPI_Common_3(a[0], a[1], new r.Message_ProgressRange_1);
                                 if (s.IsDone()) return K(s.Shape(), o)
                             })),
-                            Te = fe("Part::Extrusion", (function(e, t) {
+                            Ce = pe("Part::Extrusion", (function(e, t) {
                                 var r;
                                 const {
                                     Base: n,
                                     Dir: o,
                                     LengthFwd: a,
                                     LengthRev: s,
                                     Placement: i,
@@ -9892,15 +9933,15 @@
                                                 t.Add_1(r), e.Next()
                                             }
                                             const r = t.Wire();
                                             p = new u.BRepBuilderAPI_MakeFace_15(r, !1).Face()
                                         } return K(new u.BRepPrimAPI_MakePrism_1(p, h, !1, !0).Shape(), i)
                                 }
                             })),
-                            ke = fe("Part::Chamfer", (function(e, t) {
+                            xe = pe("Part::Chamfer", (function(e, t) {
                                 var r;
                                 const {
                                     Base: n,
                                     Edge: o,
                                     Dist: a,
                                     Placement: s
                                 } = e, i = W(), c = t.objects.filter((e => e.name === n));
@@ -9914,15 +9955,15 @@
                                     i.TopExp.MapShapes_1(e.occShape, i.TopAbs_ShapeEnum.TopAbs_EDGE, n);
                                     const d = i.TopoDS.Edge_1(n.FindKey(o + 1)),
                                         f = new i.BRepFilletAPI_MakeChamfer(e.occShape);
                                     if (f.Add_2(a, d), f.Build(new i.Message_ProgressRange_1), f.IsDone()) return K(f.Shape(), s);
                                     console.error("Failed to create chamfer")
                                 }
                             })),
-                            Ce = fe("Part::Fillet", (function(e, t) {
+                            Ae = pe("Part::Fillet", (function(e, t) {
                                 var r;
                                 const {
                                     Base: n,
                                     Edge: o,
                                     Radius: a,
                                     Placement: s
                                 } = e, i = W(), c = t.objects.filter((e => e.name === n));
@@ -9936,18 +9977,18 @@
                                     i.TopExp.MapShapes_1(e.occShape, i.TopAbs_ShapeEnum.TopAbs_EDGE, n);
                                     const d = i.TopoDS.Edge_1(n.FindKey(o + 1)),
                                         f = new i.BRepFilletAPI_MakeFillet(e.occShape, i.ChFi3d_FilletShape);
                                     if (f.Add_2(a, d), f.Build(new i.Message_ProgressRange_1), f.IsDone()) return K(f.Shape(), s);
                                     console.error("Failed to create fillet")
                                 }
                             })),
-                            Ae = fe("ObjectFile", ae);
-                        class xe {
+                            Oe = pe("ObjectFile", ie);
+                        class Ne {
                             constructor(e) {
-                                this._occ = self.occ, this._showEdge = !0, this._shapeList = e
+                                this._occ = self.occ, this._shapeList = e
                             }
                             execute() {
                                 const e = {};
                                 return this._shapeList.forEach((t => {
                                     const {
                                         shapeData: r,
                                         jcObject: n
@@ -9955,24 +9996,31 @@
                                         occShape: o,
                                         metadata: a
                                     } = r;
                                     if (!o) return;
                                     new this._occ.BRepMesh_IncrementalMesh_2(o, .1, !1, .5, !0);
                                     const s = this._build_face_mesh(o);
                                     let i = [];
-                                    this._showEdge && (i = this._build_edge_mesh(o));
-                                    const c = this._build_wire_mesh(o, .1);
-                                    e[n.name] = {
+                                    this._shouldComputeEdge(n) && (i = this._build_edge_mesh(o));
+                                    let c = [];
+                                    this._shouldComputeWire(n) && (c = this._build_wire_mesh(o, .1)), e[n.name] = {
                                         jcObject: n,
                                         faceList: s,
                                         edgeList: [...i, ...c],
                                         meta: a
                                     }
                                 })), e
                             }
+                            _shouldComputeEdge(e) {
+                                var t;
+                                return "Part::Any" !== e.shape || "STL" !== (null === (t = e.parameters) || void 0 === t ? void 0 : t.Type)
+                            }
+                            _shouldComputeWire(e) {
+                                return "Sketcher::SketchObject" === e.shape
+                            }
                             _build_wire_mesh(e, t) {
                                 const r = [],
                                     n = this._occ,
                                     o = new n.TopExp_Explorer_2(e, n.TopAbs_ShapeEnum.TopAbs_EDGE, n.TopAbs_ShapeEnum.TopAbs_SHAPE);
                                 for (o.Init(e, n.TopAbs_ShapeEnum.TopAbs_EDGE, n.TopAbs_ShapeEnum.TopAbs_SHAPE); o.More();) {
                                     const e = n.TopoDS.Edge_1(o.Current()),
                                         a = new n.TopLoc_Location_1,
@@ -10001,48 +10049,40 @@
                                         s = n.BRep_Tool.Triangulation(e, a, 0);
                                     if (s.IsNull()) {
                                         console.error("Encountered Null Face!"), o.Next();
                                         continue
                                     }
                                     const i = {
                                             vertexCoord: [],
-                                            normalCoord: [],
                                             triIndexes: [],
                                             numberOfTriangles: 0
                                         },
-                                        c = new n.Poly_Connect_2(s),
-                                        u = s.get(),
-                                        l = u.NbNodes();
-                                    i.vertexCoord = new Array(3 * l);
-                                    for (let e = 0; e < l; e++) {
-                                        const t = u.Node(e + 1).Transformed(a.Transformation());
+                                        c = s.get(),
+                                        u = c.NbNodes();
+                                    i.vertexCoord = new Array(3 * u);
+                                    for (let e = 0; e < u; e++) {
+                                        const t = c.Node(e + 1).Transformed(a.Transformation());
                                         i.vertexCoord[3 * e + 0] = t.X(), i.vertexCoord[3 * e + 1] = t.Y(), i.vertexCoord[3 * e + 2] = t.Z()
                                     }
-                                    const d = e.Orientation_1(),
-                                        f = new n.TColgp_Array1OfDir_2(1, l);
-                                    n.StdPrs_ToolTriangulatedShape.Normal(e, c, f), i.normalCoord = new Array(3 * f.Length());
-                                    for (let e = 0; e < f.Length(); e++) {
-                                        const t = f.Value(e + 1).Transformed(a.Transformation());
-                                        i.normalCoord[3 * e + 0] = t.X(), i.normalCoord[3 * e + 1] = t.Y(), i.normalCoord[3 * e + 2] = t.Z()
-                                    }
-                                    const h = u.NbTriangles();
-                                    i.triIndexes = new Array(3 * h);
-                                    let p = 0;
+                                    const l = e.Orientation_1(),
+                                        d = c.NbTriangles();
+                                    i.triIndexes = new Array(3 * d);
+                                    let f = 0;
                                     for (let e = 1; e <= s.get().NbTriangles(); e++) {
-                                        const t = u.Triangle(e);
+                                        const t = c.Triangle(e);
                                         let r = t.Value(1),
                                             o = t.Value(2);
                                         const a = t.Value(3);
-                                        if (d !== n.TopAbs_Orientation.TopAbs_FORWARD) {
+                                        if (l !== n.TopAbs_Orientation.TopAbs_FORWARD) {
                                             const e = r;
                                             r = o, o = e
                                         }
-                                        i.triIndexes[3 * p + 0] = r - 1, i.triIndexes[3 * p + 1] = o - 1, i.triIndexes[3 * p + 2] = a - 1, p++
+                                        i.triIndexes[3 * f + 0] = r - 1, i.triIndexes[3 * f + 1] = o - 1, i.triIndexes[3 * f + 2] = a - 1, f++
                                     }
-                                    i.numberOfTriangles = p, t.push(i), r.push(s), o.Next()
+                                    i.numberOfTriangles = f, t.push(i), r.push(s), o.Next()
                                 }
                                 return t
                             }
                             _build_edge_mesh(e) {
                                 const t = this._occ,
                                     r = [],
                                     n = new t.TopTools_IndexedMapOfShape_1;
@@ -10084,16 +10124,16 @@
                                         }
                                     }
                                     r.push(u)
                                 }
                                 return r
                             }
                         }
-                        const Oe = {};
-                        Oe[c.LOAD_FILE] = function(e) {
+                        const je = {};
+                        je[c.LOAD_FILE] = function(e) {
                             const {
                                 content: t
                             } = e, r = function(e) {
                                 const t = [],
                                     {
                                         objects: r
                                     } = e;
@@ -10106,15 +10146,15 @@
                                     } = r;
                                     if (!i || !c) return;
                                     const d = J();
                                     let f;
                                     if (d[i]) f = null === (n = d[i]) || void 0 === n ? void 0 : n.call(d, c, e);
                                     else if (c.Shape) {
                                         const t = null !== (o = c.Type) && void 0 !== o ? o : "brep";
-                                        f = Ae({
+                                        f = Oe({
                                             content: c.Shape,
                                             type: t
                                         }, e)
                                     } else if (i.startsWith("Post::") && u) switch (null !== (a = u.shapeFormat) && void 0 !== a ? a : l.BREP) {
                                         case l.BREP:
                                             f = null === (s = d["Post::Operator"]) || void 0 === s ? void 0 : s.call(d, c, e);
                                             break;
@@ -10124,29 +10164,29 @@
                                             }
                                     }
                                     f && t.push({
                                         shapeData: f,
                                         jcObject: r
                                     })
                                 })), t
-                            }(t), n = new xe(r).execute(), o = {};
+                            }(t), n = new Ne(r).execute(), o = {};
                             return r.forEach((e => {
                                 var t;
                                 (null === (t = e.jcObject.shape) || void 0 === t ? void 0 : t.startsWith("Post::")) && (o[e.jcObject.name] = {
                                     jcObject: e.jcObject,
                                     postShape: e.shapeData.postShape
                                 })
                             })), {
                                 result: n,
                                 postResult: o
                             }
                         };
-                        const Ne = Oe;
-                        let je;
-                        const De = {};
+                        const De = je;
+                        let Re;
+                        const Me = {};
                         console.log("Initializing OCC..."), async function() {
                             return e = {
                                 mainJS: s,
                                 mainWasm: i
                             }, new Promise(((t, r) => {
                                 const {
                                     mainJS: n,
@@ -10165,42 +10205,42 @@
                                         allowUndefined: !1
                                     });
                                     t(e)
                                 }))
                             }));
                             var e
                         }().then((e => {
-                            console.log("Done!"), je = e, self.occ = je, X("Part::Any", ye), X("Part::Box", ve), X("Part::Cylinder", ge), X("Part::Sphere", we), X("Part::Cone", _e), X("Part::Torus", be), X("Part::Cut", $e), X("Part::MultiFuse", Se), X("Part::Extrusion", Te), X("Part::MultiCommon", Pe), X("Part::Chamfer", ke), X("Part::Fillet", Ce), X("Sketcher::SketchObject", Ee), X("Post::Operator", he);
-                            for (const e of Object.keys(De)) Re({
+                            console.log("Done!"), Re = e, self.occ = Re, X("Part::Any", ge), X("Part::Box", we), X("Part::Cylinder", _e), X("Part::Sphere", be), X("Part::Cone", Ee), X("Part::Torus", $e), X("Part::Cut", Pe), X("Part::MultiFuse", Te), X("Part::Extrusion", Ce), X("Part::MultiCommon", ke), X("Part::Chamfer", xe), X("Part::Fillet", Ae), X("Sketcher::SketchObject", Se), X("Post::Operator", me);
+                            for (const e of Object.keys(Me)) Ie({
                                 action: u.INITIALIZED,
                                 payload: !1
                             }, e)
                         }));
-                        const Re = (e, t) => {
-                            t in De && De[t].postMessage(e)
+                        const Ie = (e, t) => {
+                            t in Me && Me[t].postMessage(e)
                         };
                         self.onmessage = async e => {
                             const t = e.data,
                                 {
                                     id: r
                                 } = t;
                             switch (t.action) {
                                 case c.REGISTER: {
                                     const t = e.ports[0];
                                     await (async (e, t) => {
-                                        De[e] = t, je && Re({
+                                        Me[e] = t, Re && Ie({
                                             action: u.INITIALIZED,
                                             payload: !1
                                         }, e)
                                     })(r, t);
                                     break
                                 }
                                 case c.LOAD_FILE: {
-                                    const e = Ne[t.action](t.payload);
-                                    Re({
+                                    const e = De[t.action](t.payload);
+                                    Ie({
                                         action: u.DISPLAY_SHAPE,
                                         payload: e
                                     }, r);
                                     break
                                 }
                             }
                         }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/32.249c6bd27daaea51e991.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/54.82242ec748b90c3c68dc.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,77 +1,77 @@
 "use strict";
 (self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || []).push([
-    [32], {
+    [54], {
         2070: (e, t, n) => {
             n.r(t), n.d(t, {
                 Annotation: () => Ce,
                 AnnotationModel: () => ht,
                 Annotations: () => qe,
                 CommandIDs: () => ue,
                 ControlPanelHeader: () => $e,
                 ControlPanelModel: () => it,
                 FloatingAnnotation: () => je,
                 FormDialog: () => V,
-                JupyterCadPanel: () => Ze,
+                JupyterCadPanel: () => He,
                 JupyterCadWidget: () => Ue,
                 LeftPanelWidget: () => nt,
                 LuminoSchemaForm: () => d,
                 MainView: () => We,
                 Message: () => xe,
                 ObjectProperties: () => st,
                 ObjectPropertiesForm: () => c,
                 ObjectTree: () => et,
                 PanZoom: () => Q,
-                ReactAnnotations: () => He,
+                ReactAnnotations: () => Ze,
                 RightPanelWidget: () => at,
                 Separator: () => dt,
                 SketcherDialog: () => ee,
                 SketcherModel: () => X,
                 SketcherReactWidget: () => K,
                 TOOLBAR_SEPARATOR_CLASS: () => lt,
                 ToolbarSwitch: () => Y,
                 ToolbarWidget: () => ct,
                 UsersItem: () => rt,
                 addCommands: () => me,
                 axesIcon: () => S,
                 boxIcon: () => _,
-                chamferIcon: () => O,
-                clippingIcon: () => E,
+                chamferIcon: () => E,
+                clippingIcon: () => O,
                 coneIcon: () => b,
                 createHeader: () => Ye,
                 cutIcon: () => x,
                 cylinderIcon: () => y,
                 debounce: () => I,
                 distance: () => J,
                 drawCircle: () => $,
                 drawLine: () => q,
-                drawPoint: () => H,
+                drawPoint: () => Z,
                 explodedViewIcon: () => P,
                 extrusionIcon: () => M,
                 filletIcon: () => A,
                 focusInputField: () => k,
                 getCSSVariableColor: () => W,
-                getElementFromProperty: () => N,
+                getElementFromProperty: () => B,
                 intersectionIcon: () => j,
                 isLightTheme: () => z,
                 itemFromName: () => L,
                 jcLightIcon: () => g,
                 minimizeIcon: () => v,
                 nearest: () => D,
                 newName: () => ne,
-                removeStyleFromProperty: () => B,
+                removeStyleFromProperty: () => N,
                 requestAPI: () => R,
                 setVisible: () => ie,
                 sphereIcon: () => w,
                 throttle: () => T,
                 torusIcon: () => f,
                 unionIcon: () => C
             });
-            var i = n(7638),
-                s = n(7664),
+            var i = n(8440),
+                s = n(2126),
                 o = n(3345),
                 a = n(2858),
                 r = n(6230),
                 l = n(5256);
             const d = e => {
                 const t = o.useRef(null),
                     {
@@ -207,16 +207,16 @@
                         }, o.createElement("div", {
                             className: "jp-Dialog-buttonLabel"
                         }, "Submit"))))
                     }
                     return o.createElement("div", null, this.buildForm())
                 }
             }
-            var h = n(6597),
-                p = n(2486),
+            var h = n(7655),
+                p = n(8824),
                 m = n(8996);
             const u = '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px"><g class="jp-icon3" fill="#616161"><g><path d="M2,6c0.55,0,1-0.45,1-1V4c0-0.55,0.45-1,1-1h1c0.55,0,1-0.45,1-1S5.55,1,5,1H4C2.34,1,1,2.34,1,4v1C1,5.55,1.45,6,2,6z"/><path d="M5,21H4c-0.55,0-1-0.45-1-1v-1c0-0.55-0.45-1-1-1c-0.55,0-1,0.45-1,1v1c0,1.66,1.34,3,3,3h1c0.55,0,1-0.45,1-1 S5.55,21,5,21z"/><path d="M20,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c0.55,0,1,0.45,1,1v1c0,0.55,0.45,1,1,1c0.55,0,1-0.45,1-1V4 C23,2.34,21.66,1,20,1z"/><path d="M22,18c-0.55,0-1,0.45-1,1v1c0,0.55-0.45,1-1,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c1.66,0,3-1.34,3-3v-1 C23,18.45,22.55,18,22,18z"/><path d="M19,14.87V9.13c0-0.72-0.38-1.38-1-1.73l-5-2.88c-0.31-0.18-0.65-0.27-1-0.27s-0.69,0.09-1,0.27L6,7.39 C5.38,7.75,5,8.41,5,9.13v5.74c0,0.72,0.38,1.38,1,1.73l5,2.88c0.31,0.18,0.65,0.27,1,0.27s0.69-0.09,1-0.27l5-2.88 C18.62,16.25,19,15.59,19,14.87z M11,17.17l-4-2.3v-4.63l4,2.33V17.17z M12,10.84L8.04,8.53L12,6.25l3.96,2.28L12,10.84z M17,14.87l-4,2.3v-4.6l4-2.33V14.87z"/></g></g></svg>\n',
                 g = new s.LabIcon({
                     name: "jupytercad:control-light",
                     svgstr: u
                 }),
                 v = new s.LabIcon({
@@ -263,19 +263,19 @@
                     name: "jupytercad:axes-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg width="14.3" viewBox="0 0 21.45 14.3" version="1.1" height="14.3" xmlns="http://www.w3.org/2000/svg">\n   <g class="jp-icon3" fill="#616161">\n      <path\n         d="m 10.785156,8.0390625 a 0.97509752,0.97509752 0 0 0 -0.40039,0.083984 L 3.5761719,11.185547 A 0.97500002,0.97500002 0 0 0 3.0859375,12.474609 0.97500002,0.97500002 0 0 0 4.375,12.964844 l 6.619141,-2.9765627 h 8.791015 a 0.97500002,0.97500002 0 0 0 0.97461,-0.9746094 0.97500002,0.97500002 0 0 0 -0.97461,-0.9746094 z" />\n      <path\n         d="M 10.785156,-0.9609375 A 0.97500002,0.97500002 0 0 0 9.8105469,0.01367188 V 9.0136719 a 0.97500002,0.97500002 0 0 0 0.9746091,0.9746094 0.97500002,0.97500002 0 0 0 0.97461,-0.9746094 V 0.01367188 a 0.97500002,0.97500002 0 0 0 -0.97461,-0.97460938 z" />\n      <path\n         d="m 10.095703,-0.67578125 -1.4999999,1.5 a 0.97500002,0.97500002 0 0 0 0,1.37890625 0.97500002,0.97500002 0 0 0 1.3789063,0 L 10.785156,1.3925781 11.595703,2.203125 a 0.97500002,0.97500002 0 0 0 1.378906,0 0.97500002,0.97500002 0 0 0 0,-1.37890625 l -1.5,-1.5 a 0.97509752,0.97509752 0 0 0 -1.378906,0 z" />\n      <path\n         d="m 3.0019531,10.109375 a 0.97500002,0.97500002 0 0 0 -1.1933594,0.689453 l -0.5507812,2.048828 a 0.97509752,0.97509752 0 0 0 0.6894531,1.19336 l 2.0507813,0.548828 A 0.97500002,0.97500002 0 0 0 5.1914062,13.900391 0.97500002,0.97500002 0 0 0 4.5019531,12.707031 L 3.3945313,12.410156 3.6914063,11.302734 A 0.97500002,0.97500002 0 0 0 3.0019531,10.109375 Z " />\n      <path d=" m 17.595703,6.8242187 a 0.97500002,0.97500002 0 0 0 0,1.3789063 l 0.810547,0.8105469 -0.810547,0.8105469 a\n         0.97500002,0.97500002 0 0 0 0,1.3789062 0.97500002,0.97500002 0 0 0 1.378906,0 l 1.5,-1.5 a\n         0.97509752,0.97509752 0 0 0 0,-1.3789062 l -1.5,-1.5000001 a 0.97500002,0.97500002 0 0 0 -1.378906,0 z" />\n   </g>\n</svg>\n'
                 }),
                 P = new s.LabIcon({
                     name: "jupytercad:explodedView-icon",
                     svgstr: u
                 }),
-                E = new s.LabIcon({
+                O = new s.LabIcon({
                     name: "jupytercad:clipping-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg height="24px" viewBox="0 0 24 24" width="24px" version="1.1" id="svg6" xmlns="http://www.w3.org/2000/svg">\n   <defs id="defs6" />\n\n   <g class="jp-icon3" fill="#616161" id="g6">\n      <g id="g5">\n         <path\n            d="M2,6c0.55,0,1-0.45,1-1V4c0-0.55,0.45-1,1-1h1c0.55,0,1-0.45,1-1S5.55,1,5,1H4C2.34,1,1,2.34,1,4v1C1,5.55,1.45,6,2,6z"\n            id="path1" />\n         <path\n            d="M5,21H4c-0.55,0-1-0.45-1-1v-1c0-0.55-0.45-1-1-1c-0.55,0-1,0.45-1,1v1c0,1.66,1.34,3,3,3h1c0.55,0,1-0.45,1-1 S5.55,21,5,21z"\n            id="path2" />\n         <path\n            d="M20,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c0.55,0,1,0.45,1,1v1c0,0.55,0.45,1,1,1c0.55,0,1-0.45,1-1V4 C23,2.34,21.66,1,20,1z"\n            id="path3" />\n         <path\n            d="M22,18c-0.55,0-1,0.45-1,1v1c0,0.55-0.45,1-1,1h-1c-0.55,0-1,0.45-1,1s0.45,1,1,1h1c1.66,0,3-1.34,3-3v-1 C23,18.45,22.55,18,22,18z"\n            id="path4" />\n         <path\n            d="M 19,14.87 V 9.13 C 19,8.41 18.62,7.75 18,7.4 L 13,4.52 C 12.69,4.34 12.35,4.25 12,4.25 c -0.35,0 -0.69,0.09 -1,0.27 L 6,7.39 C 5.38,7.75 5,8.41 5,9.13 v 5.74 c 0,0.72 0.38,1.38 1,1.73 l 5,2.88 c 0.31,0.18 0.65,0.27 1,0.27 0.35,0 0.69,-0.09 1,-0.27 l 5,-2.88 c 0.62,-0.35 1,-1.01 1,-1.73 z m -8,2.3 -4,-2.3 v -4.63 l 4,2.33 z M 12,10.84 8.04,8.53 12,6.25 15.96,8.53 Z"\n            id="path5" />\n      </g>\n   </g>\n</svg>\n'
                 }),
-                O = new s.LabIcon({
+                E = new s.LabIcon({
                     name: "jupytercad:chamfer-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   width="14.3"\n   viewBox="0 0 21.45 14.3"\n   version="1.1"\n   height="14.3"\n   xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n      <path\n         d="M 1.7695312,0.25 A 0.97509752,0.97509752 0 0 0 0.79101562,1.2207031 L 0.74414062,16.126953 A 0.97509752,0.97509752 0 0 0 1.71875,17.105469 l 15.074219,0.02734 a 0.97509752,0.97509752 0 0 0 0.976562,-0.978515 l -0.0332,-7.0566407 A 0.97509752,0.97509752 0 0 0 17.455078,8.4179688 L 9.7226563,0.55859375 A 0.97509752,0.97509752 0 0 0 9.0292969,0.26757813 Z m 0.9687501,1.9511719 5.8789062,0.015625 7.1699215,7.2851562 0.02734,5.6796879 -13.1152342,-0.02539 z"\n         />\n      <path\n         d="m 4.9628906,-2.8339844 a 0.97500002,0.97500002 0 0 0 -0.9804687,0.96875 0.97500002,0.97500002 0 0 0 0.96875,0.9824219 l 7.0117191,0.0429687 6.789062,6.78515625 -0.05078,6.9570315 -2.478516,2.511719 a 0.97500002,0.97500002 0 0 0 0.0078,1.378906 0.97500002,0.97500002 0 0 0 1.378906,-0.0098 l 2.757812,-2.792969 a 0.97509752,0.97509752 0 0 0 0.28125,-0.677734 l 0.05664,-7.7617188 A 0.97509752,0.97509752 0 0 0 20.419922,4.8554687 L 13.058594,-2.5019531 A 0.97509752,0.97509752 0 0 0 12.375,-2.7871094 Z"\n         />\n      <path\n         d="M 4.2441406,-2.5371094 1.125,0.4921875 a 0.97500002,0.97500002 0 0 0 -0.019531,1.3789062 0.97500002,0.97500002 0 0 0 1.3769532,0.019531 l 3.1191406,-3.0292969 a 0.97500002,0.97500002 0 0 0 0.021484,-1.3789062 0.97500002,0.97500002 0 0 0 -1.3789063,-0.019531 z"\n         />\n      <path\n         d="m 12.277344,-2.7636719 a 0.97500002,0.97500002 0 0 0 -0.69336,0.2753906 L 8.4648438,0.54101562 a 0.97500002,0.97500002 0 0 0 -0.019531,1.37890628 0.97500002,0.97500002 0 0 0 1.3789063,0.021484 l 3.1191402,-3.0312499 a 0.97500002,0.97500002 0 0 0 0.01953,-1.3789063 0.97500002,0.97500002 0 0 0 -0.685547,-0.2949219 z"\n         />\n      <path\n         d="m 19.671875,4.9160156 a 0.97500002,0.97500002 0 0 0 -0.693359,0.2773438 l -3.119141,3.0292969 a 0.97500002,0.97500002 0 0 0 -0.01953,1.3789062 0.97500002,0.97500002 0 0 0 1.378906,0.019531 l 3.119141,-3.0292969 a 0.97500002,0.97500002 0 0 0 0.01953,-1.3789063 0.97500002,0.97500002 0 0 0 -0.685547,-0.296875 z"\n         />\n   </g>\n</svg>\n'
                 }),
                 A = new s.LabIcon({
                     name: "jupytercad:fillet-icon",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   width="14.3"\n   viewBox="0 0 21.45 14.3"\n   version="1.1"\n   height="14.3"\n   xmlns="http://www.w3.org/2000/svg">\n  <g class="jp-icon3" fill="#616161">\n   <path\n      d="m 5.1523437,0.31640625 c -0.00131,0.001298 -0.00261,0.0026 -0.00391,0.003906 h -3.43359 C 1.1766933,0.32058161 0.74050356,0.75677152 0.74023437,1.2949219 V 16.210937 c 2.6899e-4,0.538151 0.43645883,0.974341 0.97460933,0.97461 H 16.574219 c 0.53815,-2.7e-4 0.97434,-0.43646 0.974609,-0.97461 v -3.527343 c -0.03739,-0.267121 -0.183757,-0.506823 -0.404297,-0.66211 l 0.394531,0.611329 c -0.156559,-3.3353437 -1.57375,-6.5223534 -3.871093,-8.8144536 -6.66e-4,-6.51e-4 -0.0013,-0.0013 -0.002,-0.00195 C 11.381408,1.5548042 8.3211488,0.27858118 5.1738281,0.3203125 c -6.485e-4,8.6e-6 -0.0013,-8.71e-6 -0.00195,0 -0.00674,9.047e-5 -0.012795,-0.004009 -0.019531,-0.003906 z M 5.1816406,2.265625 v 0.00195 c 2.6074513,-0.039706 5.1795204,1.0231917 7.1113284,2.9355469 1.936348,1.9335244 3.16369,4.6841259 3.296875,7.5214841 0.0064,0.564684 0.0065,0.369792 0.0098,0.554688 v 1.957031 H 2.6894531 V 2.2695313 h 2.484375 c 0.00261,-0.00129 0.00521,-0.0026 0.00781,-0.00391 z"\n      />\n   <path\n      d="m 4.8828125,-2.8847656 a 0.97509752,0.97509752 0 0 0 -0.9414062,1.2539062 l 0.00586,0.021484 a 0.97500002,0.97500002 0 0 0 0.9570313,0.62695312 l -0.035156,0.046875 3.4863282,0.0273438 a 0.97509752,0.97509752 0 0 0 0.025391,-0.009766 l -0.00391,0.009766 c 2.6127999,-0.0397866 5.1423829,0.99157809 7.0742189,2.90234373 1.937891,1.9334685 3.173428,4.6957347 3.30664,7.5332032 a 0.97509752,0.97509752 0 0 0 0.002,0.00195 v 3.4746091 a 0.97500002,0.97500002 0 0 0 0.976562,0.976563 0.97500002,0.97500002 0 0 0 0.974609,-0.976563 V 9.4765625 a 0.97509752,0.97509752 0 0 0 -0.03711,-0.050781 l 0.0332,0.00977 C 20.550382,6.0988535 19.127635,2.9055945 16.830078,0.61328125 a 0.97509752,0.97509752 0 0 0 -0.0039,-0.001953 C 14.542021,-1.6498218 11.509562,-2.8972038 8.3691406,-2.8554688 l 0.00195,-0.00195 h -0.013672 c -0.00338,4.85e-5 -0.00639,-0.002 -0.00977,-0.00195 a 0.97509752,0.97509752 0 0 0 -0.00195,0.00195 z"\n      />\n   <path\n      d="m 4.7871094,-2.875 a 0.97500002,0.97500002 0 0 0 -0.6855469,0.296875 l -3.0820313,3.1875 a 0.97500002,0.97500002 0 0 0 0.021484,1.3789062 0.97500002,0.97500002 0 0 0 1.3789063,-0.023437 L 5.5039062,-1.2226562 A 0.97500002,0.97500002 0 0 0 5.4804687,-2.6015625 0.97500002,0.97500002 0 0 0 4.7871094,-2.875 Z"\n      />\n   <path\n      d="m 10.542969,-2.5097656 a 0.97500002,0.97500002 0 0 0 -1.3789065,0.021484 L 6.0820312,0.69921875 A 0.97500002,0.97500002 0 0 0 6.1054687,2.078125 0.97500002,0.97500002 0 0 0 7.4824219,2.0566406 l 3.0839841,-3.1875 a 0.97500002,0.97500002 0 0 0 -0.02344,-1.3789062 z"\n      />\n   <path\n      d="m 19.576172,7.2675781 a 0.97500002,0.97500002 0 0 0 -0.685547,0.296875 l -3.082031,3.1894529 a 0.97500002,0.97500002 0 0 0 0.02344,1.376953 0.97500002,0.97500002 0 0 0 1.376953,-0.02148 l 3.083985,-3.1875 A 0.97500002,0.97500002 0 0 0 20.269531,7.5429687 0.97500002,0.97500002 0 0 0 19.576172,7.2675781 Z"\n      />\n   <path\n      d="m 20.40625,12.310547 a 0.97500002,0.97500002 0 0 0 -1.378906,0.02148 l -3.082031,3.1875 a 0.97500002,0.97500002 0 0 0 0.02344,1.378906 0.97500002,0.97500002 0 0 0 1.376953,-0.02148 l 3.083984,-3.1875 a 0.97500002,0.97500002 0 0 0 -0.02344,-1.378906 z"\n      />\n   </g>\n</svg>\n'
                 }),
@@ -305,37 +305,37 @@
 
             function k(e, t, n, i, s) {
                 var o;
                 const a = ["border-color", "box-shadow"];
                 let r;
                 if (t) {
                     if (t !== s) {
-                        B(e, s, a);
-                        const n = N(e, t);
+                        N(e, s, a);
+                        const n = B(e, t);
                         n && (n.style.borderColor = null != i ? i : "red", n.style.boxShadow = `inset 0 0 4px ${null!=i?i:"red"}`), r = t
                     }
                 } else if (s) {
-                    if (B(e, s, a), n) {
-                        const t = N(e, s);
+                    if (N(e, s, a), n) {
+                        const t = B(e, s);
                         "input" === (null === (o = null == t ? void 0 : t.tagName) || void 0 === o ? void 0 : o.toLowerCase()) && (t.value = n)
                     }
                     r = void 0
                 }
                 return r
             }
 
-            function N(e, t) {
+            function B(e, t) {
                 if (!e || !t) return;
                 const n = document.querySelector(`[data-path="${e}"]`);
                 return n ? n.querySelector(`[id$=${t}]`) : void 0
             }
 
-            function B(e, t, n) {
+            function N(e, t, n) {
                 if (!e || !t || 0 === n.length) return;
-                const i = N(e, t);
+                const i = B(e, t);
                 i && n.forEach((e => i.style.removeProperty(e)))
             }
 
             function D(e, t) {
                 const n = Math.round(e);
                 return Math.abs(n - e) < t ? n : e
             }
@@ -392,15 +392,15 @@
                         var i, o, a, l, d;
                         const c = null === (i = null == s ? void 0 : s.localState) || void 0 === i ? void 0 : i.remoteUser;
                         if (c) {
                             const e = t.get(c),
                                 i = null === (o = null == e ? void 0 : e.selectedPropField) || void 0 === o ? void 0 : o.id,
                                 s = null === (a = null == e ? void 0 : e.selectedPropField) || void 0 === a ? void 0 : a.value;
                             "dialog" === (null === (l = null == e ? void 0 : e.selectedPropField) || void 0 === l ? void 0 : l.parentType) && (r = k(`${n}::dialog`, i, s, null === (d = null == e ? void 0 : e.user) || void 0 === d ? void 0 : d.color, r))
-                        } else r && (B(`${n}::dialog`, r, ["border-color", "box-shadow"]), r = void 0)
+                        } else r && (N(`${n}::dialog`, r, ["border-color", "box-shadow"]), r = void 0)
                     })), super({
                         title: e.title,
                         body: a,
                         buttons: [i.Dialog.cancelButton()]
                     }), this.addClass("jpcad-property-FormDialog")
                 }
             }
@@ -432,15 +432,15 @@
                         end: {
                             x: this.end.x / e,
                             y: this.end.y / e
                         }
                     }
                 }
             }
-            class Z {
+            class H {
                 constructor(e, t, n) {
                     this.option = n, this._x = e, this._y = t
                 }
                 get position() {
                     return {
                         x: this._x,
                         y: this._y
@@ -450,15 +450,15 @@
                     return {
                         x: this._x / e,
                         y: this._y / e
                     }
                 }
             }
 
-            function H(e, t, n = "blue", i = 6) {
+            function Z(e, t, n = "blue", i = 6) {
                 e.save(), e.fillStyle = n, e.fillRect(t.x - i / 2, t.y - i / 2, i, i), e.restore()
             }
 
             function q(e, t, n, i, s = .5) {
                 e.save(), e.lineWidth = s, e.strokeStyle = i, e.beginPath(), e.moveTo(t.x, t.y), e.lineTo(n.x, n.y), e.setTransform(1, 0, 0, 1, 0, 0), e.stroke(), e.closePath(), e.restore()
             }
 
@@ -521,15 +521,15 @@
                     }
                     this._editing.type = null, this._editing.content = null
                 }
                 addPoint(e, t) {
                     const n = this.getPointByPosition(e);
                     if (n) return n;
                     const i = (0, F.A)();
-                    return this._points.set(i, new Z(e.x, e.y, t)), i
+                    return this._points.set(i, new H(e.x, e.y, t)), i
                 }
                 removePoint(e) {
                     this._points.delete(e)
                 }
                 getPointByPosition(e) {
                     for (const [t, n] of this._points.entries())
                         if (J(n.position, e) < .05 * this._gridSize) return t
@@ -816,26 +816,26 @@
                         const n = this._panZoom,
                             i = this._canvasRef.current,
                             s = i.getContext("2d"),
                             o = this.screenToWorldPos({
                                 x: e,
                                 y: t
                             });
-                        n.apply(), s.lineWidth = .5, s.strokeStyle = "#000", s.beginPath(), s.moveTo(o.x - 2 / n.scale * i.width, o.y), s.lineTo(o.x + 2 / n.scale * i.width, o.y), s.moveTo(o.x, o.y - 2 / n.scale * i.height), s.lineTo(o.x, o.y + 2 / n.scale * i.height), s.setTransform(1, 0, 0, 1, 0, 0), s.stroke(), s.closePath(), H(s, n.toScreen(o), "crimson")
+                        n.apply(), s.lineWidth = .5, s.strokeStyle = "#000", s.beginPath(), s.moveTo(o.x - 2 / n.scale * i.width, o.y), s.lineTo(o.x + 2 / n.scale * i.width, o.y), s.moveTo(o.x, o.y - 2 / n.scale * i.height), s.lineTo(o.x, o.y + 2 / n.scale * i.height), s.setTransform(1, 0, 0, 1, 0, 0), s.stroke(), s.closePath(), Z(s, n.toScreen(o), "crimson")
                     }, this.draw = () => {
                         const e = this.ctx;
                         if (!e) return;
                         const {
                             model: t
                         } = this.props, n = this._panZoom;
                         t.points.forEach(((t, i) => {
                             var s;
                             const o = n.toScreen(t.position),
                                 a = null === (s = t.option) || void 0 === s ? void 0 : s.color;
-                            H(e, o, a)
+                            Z(e, o, a)
                         })), t.lines.forEach((t => {
                             const i = n.toScreen(t.start),
                                 s = n.toScreen(t.end);
                             q(e, i, s, "blue", 1)
                         })), t.circles.forEach((t => {
                             const {
                                 center: i
@@ -1578,15 +1578,15 @@
                     label: o.__("Intersection"),
                     isEnabled: () => !!t.currentWidget && t.currentWidget.context.model.sharedModel.editable,
                     icon: j,
                     execute: ge.executeOperator("intersection", t)
                 }), a.addCommand(ue.chamfer, {
                     label: o.__("Make chamfer"),
                     isEnabled: () => !!t.currentWidget && t.currentWidget.context.model.sharedModel.editable,
-                    icon: O,
+                    icon: E,
                     execute: ge.executeOperator("chamfer", t)
                 }), a.addCommand(ue.fillet, {
                     label: o.__("Make fillet"),
                     isEnabled: () => !!t.currentWidget && t.currentWidget.context.model.sharedModel.editable,
                     icon: A,
                     execute: ge.executeOperator("fillet", t)
                 }), a.addCommand(ue.updateAxes, {
@@ -1639,15 +1639,15 @@
                             cancelButton: !0
                         });
                         await n.launch()
                     }
                 }), a.addCommand(ue.updateClipView, {
                     label: o.__("Clipping"),
                     isEnabled: () => Boolean(t.currentWidget),
-                    icon: E,
+                    icon: O,
                     execute: async () => {
                         const e = t.currentWidget;
                         if (!e) return;
                         const n = new V({
                             context: e.context,
                             title: he.title,
                             schema: he.schema,
@@ -1899,25 +1899,25 @@
                         right: 3,
                         background: e.remoteUser.color
                     }
                 }, `Following ${e.remoteUser.display_name}`) : null
             }
             var Se = n(9047),
                 Pe = n(8307),
-                Ee = n(4790),
-                Oe = n(919);
+                Oe = n(4790),
+                Ee = n(919);
             _e.LoY.prototype.computeBoundsTree = Se.LO, _e.LoY.prototype.disposeBoundsTree = Se.je, _e.eaF.prototype.raycast = Se.zQ;
             const Ae = "--jp-inverse-layout-color4",
                 Ie = "--jp-inverse-layout-color2",
                 Te = "--jp-brand-color0",
                 Le = new _e.Q1f(W(Ae)),
                 ke = new _e.Q1f(W(Ie)),
-                Ne = new _e.Q1f(W(Te));
+                Be = new _e.Q1f(W(Te));
 
-            function Be(e) {
+            function Ne(e) {
                 var t;
                 const {
                     mesh: n,
                     boundingGroup: i,
                     factor: s
                 } = e, o = new _e.Pq0;
                 i.getCenter(o);
@@ -1948,15 +1948,15 @@
                     super(e), this.addContextMenu = () => {
                         const e = new ve.CommandRegistry;
                         e.addCommand("add-annotation", {
                             execute: () => {
                                 if (!this._pointer3D) return;
                                 const e = (new _e.Pq0).copy(this._pointer3D.mesh.position);
                                 if (this._explodedView.enabled) {
-                                    const t = Be({
+                                    const t = Ne({
                                         mesh: this._pointer3D.mesh,
                                         boundingGroup: this._boundingGroup,
                                         factor: this._explodedView.factor
                                     });
                                     e.add(t.vector.multiplyScalar(-t.distance))
                                 }
                                 this._mainViewModel.addAnnotation({
@@ -1973,15 +1973,15 @@
                         }), this._contextMenu.addItem({
                             command: "add-annotation",
                             selector: "canvas",
                             rank: 1
                         })
                     }, this.sceneSetup = () => {
                         if (null !== this.divRef.current) {
-                            Le.set(W(Ae)), ke.set(W(Ie)), Ne.set(W(Te)), this._camera = new _e.ubm(90, 2, .1, 1e3), this._camera.position.set(8, 8, 8), this._camera.up.set(0, 0, 1), this._scene = new _e.Z58, this._scene.add(new _e.$p8(16777215, .5)), this._cameraLight = new _e.HiM(16777215, 1), this._camera.add(this._cameraLight), this._scene.add(this._camera), this._renderer = new _e.JeP({
+                            Le.set(W(Ae)), ke.set(W(Ie)), Be.set(W(Te)), this._camera = new _e.ubm(90, 2, .1, 1e3), this._camera.position.set(8, 8, 8), this._camera.up.set(0, 0, 1), this._scene = new _e.Z58, this._scene.add(new _e.$p8(16777215, .5)), this._cameraLight = new _e.HiM(16777215, 1), this._camera.add(this._cameraLight), this._scene.add(this._camera), this._renderer = new _e.JeP({
                                 alpha: !0,
                                 antialias: !0
                             }), this._renderer.setClearColor(0, 0), this._renderer.setSize(500, 500, !1), this.divRef.current.appendChild(this._renderer.domElement), this._syncPointer = T(((e, t) => {
                                 e && t ? this._model.syncPointer({
                                     parent: t,
                                     x: e.x,
                                     y: e.y,
@@ -2024,15 +2024,15 @@
                         null !== this._clippingPlaneMesh && (this._clippingPlane.coplanarPoint(this._clippingPlaneMesh.position), this._clippingPlaneMesh.lookAt(this._clippingPlaneMesh.position.x - this._clippingPlane.normal.x, this._clippingPlaneMesh.position.y - this._clippingPlane.normal.y, this._clippingPlaneMesh.position.z - this._clippingPlane.normal.z)), this._controls.update(), this._renderer.setRenderTarget(null), this._renderer.clearDepth(), this._renderer.render(this._scene, this._camera)
                     }, this.resizeCanvasToDisplaySize = () => {
                         null !== this.divRef.current && (this._renderer.setSize(this.divRef.current.clientWidth, this.divRef.current.clientHeight, !1), "PerspectiveCamera" === this._camera.type ? this._camera.aspect = this.divRef.current.clientWidth / this.divRef.current.clientHeight : (this._camera.left = this.divRef.current.clientWidth / -2, this._camera.right = this.divRef.current.clientWidth / 2, this._camera.top = this.divRef.current.clientHeight / 2, this._camera.bottom = this.divRef.current.clientHeight / -2), this._camera.updateProjectionMatrix())
                     }, this.generateScene = () => {
                         this.sceneSetup(), this.animate(), this.resizeCanvasToDisplaySize()
                     }, this._shapeToMesh = e => {
                         var t;
-                        null !== this._meshGroup && this._scene.remove(this._meshGroup), null !== this._explodedViewLinesHelperGroup && this._scene.remove(this._explodedViewLinesHelperGroup);
+                        null !== this._meshGroup && this._scene.remove(this._meshGroup), null !== this._explodedViewLinesHelperGroup && this._scene.remove(this._explodedViewLinesHelperGroup), null !== this._clippingPlaneMesh && this._scene.remove(this._clippingPlaneMesh);
                         const n = this._model.sharedModel.getOption("guidata"),
                             i = this._selectedMeshes.map((e => e.name));
                         this._selectedMeshes = [], this._boundingGroup = new _e.NRn, this._edgeMaterials = [], this._meshGroup = new _e.YJl, Object.entries(e).forEach((([e, t]) => {
                             var s;
                             const o = i.includes(e),
                                 a = function(e) {
                                     const {
@@ -2041,81 +2041,83 @@
                                         guidata: i,
                                         clippingPlanes: s,
                                         selected: o
                                     } = e, {
                                         faceList: a,
                                         edgeList: r,
                                         jcObject: l
-                                    } = n, d = [], c = [], h = [];
-                                    let p = 0;
+                                    } = n, d = [], c = [];
+                                    let h = 0;
                                     if (0 === a.length && 0 === r.length) return null;
-                                    a.forEach((e => {
-                                        d.push(...e.vertexCoord), c.push(...e.normalCoord);
-                                        for (let t = 0; t < e.triIndexes.length; t += 3) h.push(e.triIndexes[t + 0] + p, e.triIndexes[t + 1] + p, e.triIndexes[t + 2] + p);
-                                        p += e.vertexCoord.length / 3
-                                    }));
-                                    let m = Le,
-                                        u = l.visible;
+                                    for (const e of a) {
+                                        const t = e.vertexCoord.length;
+                                        for (let n = 0; n < t; n++) d.push(e.vertexCoord[n]);
+                                        const n = e.triIndexes.length;
+                                        for (let t = 0; t < n; t += 3) c.push(e.triIndexes[t + 0] + h, e.triIndexes[t + 1] + h, e.triIndexes[t + 2] + h);
+                                        h += t / 3
+                                    }
+                                    let p = Le,
+                                        m = l.visible;
                                     if (i && i[t]) {
                                         const e = i[t];
                                         if (Object.prototype.hasOwnProperty.call(e, "color")) {
                                             const t = e.color;
-                                            m = new _e.Q1f(t[0], t[1], t[2])
+                                            p = new _e.Q1f(t[0], t[1], t[2])
                                         }
-                                        Object.prototype.hasOwnProperty.call(e, "visibility") && (u = i[t].visibility)
+                                        Object.prototype.hasOwnProperty.call(e, "visibility") && (m = i[t].visibility)
                                     }
-                                    const g = new _e.tXL({
-                                            color: m,
-                                            side: _e.$EB,
+                                    const u = new _e.tXL({
+                                            color: p,
                                             wireframe: !1,
                                             flatShading: !1,
                                             clippingPlanes: s,
                                             shininess: 0
                                         }),
-                                        v = new _e.LoY;
-                                    v.setIndex(h), v.setAttribute("position", new _e.qtW(d, 3)), v.setAttribute("normal", new _e.qtW(c, 3)), v.computeBoundingBox(), d.length > 0 && v.computeBoundsTree();
-                                    const _ = new _e.YJl;
-                                    _.name = `${t}-group`, _.visible = u;
-                                    const b = new _e.V9B;
-                                    b.depthWrite = !1, b.depthTest = !1, b.colorWrite = !1, b.stencilWrite = !0, b.stencilFunc = _e.sKt;
-                                    const w = b.clone();
-                                    w.side = _e.hsX, w.clippingPlanes = s, w.stencilFail = _e.Ru$, w.stencilZFail = _e.Ru$, w.stencilZPass = _e.Ru$;
-                                    const y = new _e.eaF(v, w);
-                                    y.name = `${t}-back`, _.add(y);
-                                    const f = b.clone();
-                                    f.side = _e.hB5, f.clippingPlanes = s, f.stencilFail = _e.fJr, f.stencilZFail = _e.fJr, f.stencilZPass = _e.fJr;
-                                    const x = new _e.eaF(v, f);
-                                    x.name = `${t}-front`, _.add(x);
-                                    const C = new _e.eaF(v, g);
-                                    C.name = t, C.userData = {
+                                        g = new _e.LoY;
+                                    g.setIndex(c), g.setAttribute("position", new _e.qtW(d, 3)), g.computeVertexNormals(), g.computeBoundingBox(), d.length > 0 && g.computeBoundsTree();
+                                    const v = new _e.YJl;
+                                    v.name = `${t}-group`, v.visible = m;
+                                    const _ = new _e.V9B;
+                                    _.depthWrite = !1, _.depthTest = !1, _.colorWrite = !1, _.stencilWrite = !0, _.stencilFunc = _e.sKt;
+                                    const b = _.clone();
+                                    b.side = _e.hsX, b.clippingPlanes = s, b.stencilFail = _e.Ru$, b.stencilZFail = _e.Ru$, b.stencilZPass = _e.Ru$;
+                                    const w = new _e.eaF(g, b);
+                                    w.name = `${t}-back`, v.add(w);
+                                    const y = _.clone();
+                                    y.side = _e.hB5, y.clippingPlanes = s, y.stencilFail = _e.fJr, y.stencilZFail = _e.fJr, y.stencilZPass = _e.fJr;
+                                    const f = new _e.eaF(g, y);
+                                    f.name = `${t}-front`, v.add(f);
+                                    const x = new _e.eaF(g, u);
+                                    x.name = t, x.userData = {
                                         type: "shape"
-                                    }, o && (C.material.color = Ne);
-                                    let j = 0;
-                                    const M = [];
-                                    return r.forEach((e => {
-                                        const n = new Ee.G({
-                                                linewidth: 4,
+                                    }, o && (x.material.color = Be);
+                                    let C = 0;
+                                    const j = [];
+                                    for (const e of r) {
+                                        const n = new Oe.G({
+                                                linewidth: 2,
                                                 color: ke,
                                                 clippingPlanes: s,
                                                 polygonOffset: !0,
                                                 polygonOffsetFactor: -5,
                                                 polygonOffsetUnits: -5
                                             }),
                                             i = new Pe.v;
                                         i.setPositions(e.vertexCoord);
-                                        const o = new Oe.b(i, n);
-                                        o.name = `edge-${t}-${j}`, o.userData = {
+                                        const o = new Ee.b(i, n);
+                                        o.name = `edge-${t}-${C}`, o.userData = {
                                             type: "edge",
-                                            edgeIndex: j,
+                                            edgeIndex: C,
                                             parent: t
-                                        }, M.push(o), j++
-                                    })), _.add(...M), _.add(C), {
-                                        meshGroup: _,
-                                        mainMesh: C,
-                                        edgesMeshes: M
+                                        }, j.push(o), v.add(o), C++
+                                    }
+                                    return v.add(x), {
+                                        meshGroup: v,
+                                        mainMesh: x,
+                                        edgesMeshes: j
                                     }
                                 }({
                                     objName: e,
                                     data: t,
                                     clippingPlanes: this._clippingPlanes,
                                     selected: o,
                                     guidata: n
@@ -2123,15 +2125,15 @@
                             if (a) {
                                 const {
                                     meshGroup: e,
                                     mainMesh: t,
                                     edgesMeshes: n
                                 } = a;
                                 e.visible && this._boundingGroup.expandByObject(t), o && this._selectedMeshes.push(t), n.forEach((e => {
-                                    this._edgeMaterials.push(e.material), i.includes(e.name) && (this._selectedMeshes.push(e), e.material.color = Ne, e.material.linewidth = 12)
+                                    this._edgeMaterials.push(e.material), i.includes(e.name) && (this._selectedMeshes.push(e), e.material.color = Be, e.material.linewidth = 6)
                                 })), null === (s = this._meshGroup) || void 0 === s || s.add(e)
                             }
                         })), n && (null === (t = this._model.sharedModel) || void 0 === t || t.setOption("guidata", n)), this._updateRefLength(), this._setupExplodedView();
                         const s = new _e.bdM(10 * this._refLength, 10 * this._refLength),
                             o = new _e.tXL({
                                 color: ke,
                                 stencilWrite: !0,
@@ -2140,15 +2142,15 @@
                                 stencilFail: _e.kG0,
                                 stencilZFail: _e.kG0,
                                 stencilZPass: _e.kG0,
                                 side: _e.$EB
                             });
                         this._clippingPlaneMesh = new _e.eaF(s, o), this._clippingPlaneMesh.onAfterRender = e => {
                             e.clearStencil()
-                        }, this._scene.add(this._clippingPlaneMesh), this._scene.add(this._meshGroup), this.setState((e => Object.assign(Object.assign({}, e), {
+                        }, this._scene.add(this._clippingPlaneMesh), this._scene.add(this._meshGroup), this._loadingTimeout && (clearTimeout(this._loadingTimeout), this._loadingTimeout = null), this.setState((e => Object.assign(Object.assign({}, e), {
                             loading: !1
                         })))
                     }, this._onSharedMetadataChanged = (e, t) => {
                         const n = Object.assign({}, this.state.annotations);
                         t.forEach(((e, t) => {
                             if (!t.startsWith("annotation")) return;
                             const i = this._model.sharedModel.getMetadata(t);
@@ -2207,56 +2209,56 @@
                                     const i = this._createPointer(e.user);
                                     o = this._collaboratorPointers[t] = {
                                         mesh: i,
                                         parent: n
                                     }, this._scene.add(i)
                                 }
                                 if (o.mesh.visible = !0, this._explodedView.enabled) {
-                                    const e = Be({
+                                    const e = Ne({
                                             mesh: n,
                                             boundingGroup: this._boundingGroup,
                                             factor: this._explodedView.factor
                                         }),
                                         t = e.vector.multiplyScalar(e.distance);
                                     o.mesh.position.copy(new _e.Pq0(s.x + t.x, s.y + t.y, s.z + t.z))
                                 } else o.mesh.position.copy(new _e.Pq0(s.x, s.y, s.z));
                                 o.parent = n
                             } else this._collaboratorPointers[t] && (this._collaboratorPointers[t].mesh.visible = !1)
                         }))
                     }, this._handleThemeChange = () => {
                         const e = z();
-                        Le.set(W(Ae)), ke.set(W(Ie)), Ne.set(W(Te)), this.setState((t => Object.assign(Object.assign({}, t), {
+                        Le.set(W(Ae)), ke.set(W(Ie)), Be.set(W(Te)), this.setState((t => Object.assign(Object.assign({}, t), {
                             lightTheme: e
                         })))
                     }, this._handleWindowResize = () => {
                         this.resizeCanvasToDisplaySize(), this._updateAnnotation()
                     }, this.divRef = o.createRef(), this._selectedMeshes = [], this._meshGroup = null, this._boundingGroup = new _e.NRn, this._explodedView = {
                         enabled: !1,
                         factor: 0
                     }, this._explodedViewLinesHelperGroup = null, this._cameraSettings = {
                         type: "Perspective"
                     }, this._clipSettings = {
                         enabled: !1,
                         showClipPlane: !0
-                    }, this._clippingPlaneMesh = null, this._clippingPlane = new _e.Zcv(new _e.Pq0(-1, 0, 0), 0), this._clippingPlanes = [this._clippingPlane], this._edgeMaterials = [], this._raycaster = new _e.tBo, this._requestID = null, this._refLength = null, this._pointer3D = null, this._geometry = new _e.LoY, this._geometry.setDrawRange(0, 3e4), this._mainViewModel = this.props.viewModel, this._mainViewModel.viewSettingChanged.connect(this._onViewChanged, this), this._model = this._mainViewModel.jcadModel, this._pointer = new _e.I9Y, this._collaboratorPointers = {}, this._model.themeChanged.connect(this._handleThemeChange, this), this._mainViewModel.jcadModel.sharedOptionsChanged.connect(this._onSharedOptionsChanged, this), this._mainViewModel.jcadModel.clientStateChanged.connect(this._onClientSharedStateChanged, this), this._mainViewModel.jcadModel.sharedMetadataChanged.connect(this._onSharedMetadataChanged, this), this._mainViewModel.renderSignal.connect(this._requestRender, this), this._raycaster.params.Line2 = {}, this._raycaster.params.Line2.threshold = 50, this.state = {
+                    }, this._clippingPlaneMesh = null, this._clippingPlane = new _e.Zcv(new _e.Pq0(-1, 0, 0), 0), this._clippingPlanes = [this._clippingPlane], this._edgeMaterials = [], this._raycaster = new _e.tBo, this._requestID = null, this._refLength = null, this._pointer3D = null, this._geometry = new _e.LoY, this._geometry.setDrawRange(0, 3e4), this._mainViewModel = this.props.viewModel, this._mainViewModel.viewSettingChanged.connect(this._onViewChanged, this), this._model = this._mainViewModel.jcadModel, this._pointer = new _e.I9Y, this._collaboratorPointers = {}, this._model.themeChanged.connect(this._handleThemeChange, this), this._mainViewModel.jcadModel.sharedOptionsChanged.connect(this._onSharedOptionsChanged, this), this._mainViewModel.jcadModel.clientStateChanged.connect(this._onClientSharedStateChanged, this), this._mainViewModel.jcadModel.sharedMetadataChanged.connect(this._onSharedMetadataChanged, this), this._mainViewModel.renderSignal.connect(this._requestRender, this), this._mainViewModel.workerBusy.connect(this._workerBusyHandler, this), this._raycaster.params.Line2 = {}, this._raycaster.params.Line2.threshold = 50, this.state = {
                         id: this._mainViewModel.id,
                         lightTheme: z(),
                         loading: !0,
                         annotations: {},
                         firstLoad: !0
                     }
                 }
                 componentDidMount() {
                     window.addEventListener("resize", this._handleWindowResize), this.generateScene(), this.addContextMenu(), this._mainViewModel.initWorker(), this._mainViewModel.initSignal()
                 }
                 componentDidUpdate(e, t) {
                     this.resizeCanvasToDisplaySize()
                 }
                 componentWillUnmount() {
-                    window.cancelAnimationFrame(this._requestID), window.removeEventListener("resize", this._handleWindowResize), this._mainViewModel.viewSettingChanged.disconnect(this._onViewChanged, this), this._controls.dispose(), this._model.themeChanged.disconnect(this._handleThemeChange, this), this._model.sharedOptionsChanged.disconnect(this._onSharedOptionsChanged, this), this._mainViewModel.jcadModel.clientStateChanged.disconnect(this._onClientSharedStateChanged, this), this._mainViewModel.jcadModel.sharedMetadataChanged.disconnect(this._onSharedMetadataChanged, this), this._mainViewModel.renderSignal.disconnect(this._requestRender, this), this._mainViewModel.dispose()
+                    window.cancelAnimationFrame(this._requestID), window.removeEventListener("resize", this._handleWindowResize), this._mainViewModel.viewSettingChanged.disconnect(this._onViewChanged, this), this._controls.dispose(), this._model.themeChanged.disconnect(this._handleThemeChange, this), this._model.sharedOptionsChanged.disconnect(this._onSharedOptionsChanged, this), this._mainViewModel.jcadModel.clientStateChanged.disconnect(this._onClientSharedStateChanged, this), this._mainViewModel.jcadModel.sharedMetadataChanged.disconnect(this._onSharedMetadataChanged, this), this._mainViewModel.renderSignal.disconnect(this._requestRender, this), this._mainViewModel.workerBusy.disconnect(this._workerBusyHandler, this), this._mainViewModel.dispose()
                 }
                 _updateAnnotation() {
                     Object.keys(this.state.annotations).forEach((e => {
                         var t;
                         const n = document.getElementById(e);
                         if (n) {
                             const i = null === (t = this._model.annotationModel) || void 0 === t ? void 0 : t.getAnnotation(e);
@@ -2271,15 +2273,15 @@
                     const n = this._pick();
                     if (!this._pointer3D && this._model.localState && n && (this._pointer3D = {
                             parent: n.mesh,
                             mesh: this._createPointer(this._model.localState.user)
                         }, this._scene.add(this._pointer3D.mesh)), n) {
                         if (!this._pointer3D) return void this._syncPointer(void 0, void 0);
                         if (this._pointer3D.mesh.visible = !0, this._pointer3D.mesh.position.copy(n.position), this._pointer3D.parent = n.mesh, this._explodedView.enabled) {
-                            const e = Be({
+                            const e = Ne({
                                 mesh: this._pointer3D.parent,
                                 boundingGroup: this._boundingGroup,
                                 factor: this._explodedView.factor
                             });
                             n.position.add(e.vector.multiplyScalar(-e.distance))
                         }
                         this._syncPointer(n.position, n.mesh.name)
@@ -2355,22 +2357,31 @@
                         d = new _e.XJ7(l.geometry),
                         c = new _e.mrM({
                             color: "black"
                         }),
                         h = new _e.DXC(d, c);
                     l.add(h), l.name = e, l.visible = !0, this._meshGroup && (this._meshGroup.add(l), null === (n = this._boundingGroup) || void 0 === n || n.expandByObject(l)), this._updateRefLength(!0)
                 }
+                _workerBusyHandler(e, t) {
+                    this._loadingTimeout && clearTimeout(this._loadingTimeout), t ? this._loadingTimeout = setTimeout((() => {
+                        this.setState((e => Object.assign(Object.assign({}, e), {
+                            loading: !0
+                        })))
+                    }), 250) : this.setState((e => Object.assign(Object.assign({}, e), {
+                        loading: !1
+                    })))
+                }
                 async _requestRender(e, t) {
                     const {
                         shapes: n,
                         postShapes: i,
                         postResult: s
                     } = t;
                     if (null != n) {
-                        this._shapeToMesh(t.shapes);
+                        this._shapeToMesh(n);
                         const e = {
                             binary: !0,
                             onlyVisible: !1
                         };
                         if (s && this._meshGroup) {
                             const t = new ye.r,
                                 n = [];
@@ -2405,25 +2416,25 @@
                         color: i ? new _e.Q1f(i.r / 255, i.g / 255, i.b / 255) : "black"
                     });
                     return new _e.eaF(this._pointerGeometry, s)
                 }
                 _updateSelected(e) {
                     var t, n, i, s, o;
                     for (const e of this._selectedMeshes) {
-                        let i = Le;
+                        let i = e.name.startsWith("edge-") ? ke : Le;
                         const s = this._model.sharedModel.getOption("guidata");
                         if (s && s[e.name] && s[e.name].color) {
                             const t = s[e.name].color;
                             i = new _e.Q1f(t[0], t[1], t[2])
-                        }(null === (t = e.material) || void 0 === t ? void 0 : t.color) && (e.material.color = i), (null === (n = e.material) || void 0 === n ? void 0 : n.linewidth) && (e.material.linewidth = 4)
+                        }(null === (t = e.material) || void 0 === t ? void 0 : t.color) && (e.material.color = i), (null === (n = e.material) || void 0 === n ? void 0 : n.linewidth) && (e.material.linewidth = 2)
                     }
                     this._selectedMeshes = [];
                     for (const t in e) {
                         const e = null === (i = this._meshGroup) || void 0 === i ? void 0 : i.getObjectByName(t);
-                        e && (this._selectedMeshes.push(e), (null === (s = null == e ? void 0 : e.material) || void 0 === s ? void 0 : s.color) && (e.material.color = Ne), (null === (o = null == e ? void 0 : e.material) || void 0 === o ? void 0 : o.linewidth) && (e.material.linewidth = 12))
+                        e && (this._selectedMeshes.push(e), (null === (s = null == e ? void 0 : e.material) || void 0 === s ? void 0 : s.color) && (e.material.color = Be), (null === (o = null == e ? void 0 : e.material) || void 0 === o ? void 0 : o.linewidth) && (e.material.linewidth = 6))
                     }
                 }
                 _onSharedOptionsChanged(e, t) {
                     var n, i;
                     const s = e.getOption("guidata");
                     if (s)
                         for (const e in s) {
@@ -2465,23 +2476,23 @@
                 }
                 _setupExplodedView() {
                     var e, t, n, i;
                     if (this._explodedView.enabled) {
                         const n = new _e.Pq0;
                         this._boundingGroup.getCenter(n), null === (e = this._explodedViewLinesHelperGroup) || void 0 === e || e.removeFromParent(), this._explodedViewLinesHelperGroup = new _e.YJl;
                         for (const e of null === (t = this._meshGroup) || void 0 === t ? void 0 : t.children) {
-                            const t = Be({
+                            const t = Ne({
                                 mesh: e.getObjectByName(e.name.replace("-group", "")),
                                 boundingGroup: this._boundingGroup,
                                 factor: this._explodedView.factor
                             });
                             e.position.set(0, 0, 0), e.translateOnAxis(t.vector, t.distance);
                             const n = new _e.mrM({
                                     color: ke,
-                                    linewidth: 4
+                                    linewidth: 2
                                 }),
                                 i = (new _e.LoY).setFromPoints([t.oldGeometryCenter, t.newGeometryCenter]),
                                 s = new _e.N1A(i, n);
                             s.name = e.name, s.visible = e.visible, this._explodedViewLinesHelperGroup.add(s)
                         }
                         this._scene.add(this._explodedViewLinesHelperGroup)
                     } else {
@@ -2505,15 +2516,15 @@
                     this._clipSettings.enabled ? (this._renderer.localClippingEnabled = !0, this._transformControls.enabled = !0, this._transformControls.visible = !0, this._clippingPlaneMeshControl.visible = this._clipSettings.showClipPlane) : (this._renderer.localClippingEnabled = !1, this._transformControls.enabled = !1, this._transformControls.visible = !1, this._clippingPlaneMeshControl.visible = !1)
                 }
                 _computeAnnotationPosition(e) {
                     var t;
                     const n = null === (t = this._meshGroup) || void 0 === t ? void 0 : t.getObjectByName(e.parent),
                         i = new _e.Pq0(e.position[0], e.position[1], e.position[2]);
                     if (this._explodedView.enabled && n) {
-                        const e = Be({
+                        const e = Ne({
                                 mesh: n,
                                 boundingGroup: this._boundingGroup,
                                 factor: this._explodedView.factor
                             }),
                             t = e.vector.multiplyScalar(e.distance);
                         i.add(t)
                     }
@@ -2564,18 +2575,18 @@
                         style: {
                             width: "100%",
                             height: "calc(100%)"
                         }
                     }))
                 }
             }
-            var Re = n(8859),
-                ze = n(8265),
+            var Re = n(921),
+                ze = n(4123),
                 Ve = n(4602),
-                Fe = n(3342);
+                Fe = n(3283);
             class Ge {
                 constructor(e) {
                     this.messageHandler = e => {
                         switch (e.action) {
                             case Fe.MainAction.DISPLAY_SHAPE: {
                                 const {
                                     result: t,
@@ -2593,20 +2604,21 @@
                                         postResult: s
                                     }), this._firstRender = !1
                                 } else this._renderSignal.emit({
                                     shapes: t,
                                     postShapes: null,
                                     postResult: s
                                 }), this.sendRawGeometryToWorker(i);
+                                this._workerBusy.emit(!1);
                                 break
                             }
                             case Fe.MainAction.INITIALIZED: {
                                 if (!this._jcadModel) return;
                                 const e = this._jcadModel.getContent();
-                                this._postMessage({
+                                this._workerBusy.emit(!0), this._postMessage({
                                     action: Fe.WorkerAction.LOAD_FILE,
                                     payload: {
                                         content: e
                                     }
                                 })
                             }
                         }
@@ -2634,25 +2646,28 @@
                             });
                             this._worker.postMessage(t)
                         }
                     }, this._saveMeta = e => {
                         this._jcadModel && Object.entries(e).forEach((([e, t]) => {
                             this._jcadModel.sharedModel.setShapeMeta(e, t.meta)
                         }))
-                    }, this._postWorkerId = new Map, this._firstRender = !0, this._renderSignal = new Ve.Signal(this), this._isDisposed = !1, this._jcadModel = e.jcadModel, this._viewSetting = e.viewSetting, this._workerRegistry = e.workerRegistry
+                    }, this._postWorkerId = new Map, this._firstRender = !0, this._renderSignal = new Ve.Signal(this), this._workerBusy = new Ve.Signal(this), this._isDisposed = !1, this._jcadModel = e.jcadModel, this._viewSetting = e.viewSetting, this._workerRegistry = e.workerRegistry
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get id() {
                     return this._id
                 }
                 get renderSignal() {
                     return this._renderSignal
                 }
+                get workerBusy() {
+                    return this._workerBusy
+                }
                 get jcadModel() {
                     return this._jcadModel
                 }
                 get viewSettingChanged() {
                     return this._viewSetting.changed
                 }
                 dispose() {
@@ -2689,33 +2704,37 @@
                     }))
                 }
                 addAnnotation(e) {
                     var t;
                     null === (t = this._jcadModel.annotationModel) || void 0 === t || t.addAnnotation((0, F.A)(), e)
                 }
                 async _onSharedObjectsChanged(e, t) {
-                    t.objectChange && (await this._worker.ready, this._postMessage({
-                        action: Fe.WorkerAction.LOAD_FILE,
-                        payload: {
-                            content: this._jcadModel.getContent()
-                        }
-                    }))
+                    if (t.objectChange) {
+                        await this._worker.ready;
+                        const e = this._jcadModel.getContent();
+                        this._workerBusy.emit(!0), this._postMessage({
+                            action: Fe.WorkerAction.LOAD_FILE,
+                            payload: {
+                                content: e
+                            }
+                        })
+                    }
                 }
             }
             class Ue extends Re.DocumentWidget {
                 constructor(e) {
                     super(e), this.onResize = e => {
                         window.dispatchEvent(new Event("resize"))
                     }
                 }
                 dispose() {
                     this.content.dispose(), super.dispose()
                 }
             }
-            class Ze extends i.ReactWidget {
+            class He extends i.ReactWidget {
                 constructor(e) {
                     super(), this.addClass("jp-jupytercad-panel"), this._view = new ze.ObservableMap, this._mainViewModel = new Ge({
                         jcadModel: e.model,
                         workerRegistry: e.workerRegistry,
                         viewSetting: this._view
                     })
                 }
@@ -2754,15 +2773,15 @@
                 }
                 render() {
                     return o.createElement(We, {
                         viewModel: this._mainViewModel
                     })
                 }
             }
-            class He extends o.Component {
+            class Ze extends o.Component {
                 constructor(e) {
                     super(e);
                     const t = () => {
                         this.forceUpdate()
                     };
                     this._model = e.model, this._model.contextChanged.connect((async () => {
                         var n, i, s, o, a, r, l, d;
@@ -2780,15 +2799,15 @@
                         className: "jpcad-Annotations-Separator"
                     }))));
                     return o.createElement("div", null, n)
                 }
             }
             class qe extends s.PanelWithToolbar {
                 constructor(e) {
-                    super({}), this.title.label = "Annotations", this.addClass("jpcad-Annotations"), this._model = e.model, this._widget = s.ReactWidget.create(o.createElement(He, {
+                    super({}), this.title.label = "Annotations", this.addClass("jpcad-Annotations"), this._model = e.model, this._widget = s.ReactWidget.create(o.createElement(Ze, {
                         model: this._model
                     })), this.addWidget(this._widget)
                 }
             }
             class $e extends l.Widget {
                 constructor() {
                     super({
@@ -3129,15 +3148,15 @@
                         if (h) {
                             m = t.get(h);
                             const e = null === (s = null == m ? void 0 : m.selectedPropField) || void 0 === s ? void 0 : s.id,
                                 n = null === (o = null == m ? void 0 : m.selectedPropField) || void 0 === o ? void 0 : o.value;
                             "panel" === (null === (a = null == m ? void 0 : m.selectedPropField) || void 0 === a ? void 0 : a.parentType) && (this._lastSelectedPropFieldId = k(`${this.state.filePath}::panel`, e, n, null === (r = null == m ? void 0 : m.user) || void 0 === r ? void 0 : r.color, this._lastSelectedPropFieldId))
                         } else {
                             const e = p ? t.get(p) : null;
-                            this._lastSelectedPropFieldId && (B(`${this.state.filePath}::panel`, this._lastSelectedPropFieldId, ["border-color", "box-shadow"]), this._lastSelectedPropFieldId = void 0), e && (null === (l = e.selected) || void 0 === l ? void 0 : l.emitter) && e.selected.emitter !== this.state.id && (null === (d = e.selected) || void 0 === d ? void 0 : d.value) && (m = e)
+                            this._lastSelectedPropFieldId && (N(`${this.state.filePath}::panel`, this._lastSelectedPropFieldId, ["border-color", "box-shadow"]), this._lastSelectedPropFieldId = void 0), e && (null === (l = e.selected) || void 0 === l ? void 0 : l.emitter) && e.selected.emitter !== this.state.id && (null === (d = e.selected) || void 0 === d ? void 0 : d.value) && (m = e)
                         }
                         if (m) {
                             const e = m.selected.value,
                                 t = Object.keys(e || {});
                             if (void 0 === e || 1 !== t.length || "shape" !== e[t[0]].type) return void this.setState((e => Object.assign(Object.assign({}, e), {
                                 schema: void 0,
                                 selectedObject: "",
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/413.e3edef5e15636d5f7630.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/413.378697570d8f23193ff4.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,210 +1,209 @@
 "use strict";
 (self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || []).push([
     [413, 794], {
-        9794: (e, o, r) => {
-            r.r(o), r.d(o, {
-                OccParser: () => t,
+        9794: (e, o, t) => {
+            t.r(o), t.d(o, {
+                OccParser: () => r,
                 OccWorker: () => h
             });
-            class t {
+            class r {
                 constructor(e) {
-                    this._occ = self.occ, this._showEdge = !0, this._shapeList = e
+                    this._occ = self.occ, this._shapeList = e
                 }
                 execute() {
                     const e = {};
                     return this._shapeList.forEach((o => {
                         const {
-                            shapeData: r,
-                            jcObject: t
+                            shapeData: t,
+                            jcObject: r
                         } = o, {
                             occShape: n,
                             metadata: s
-                        } = r;
+                        } = t;
                         if (!n) return;
                         new this._occ.BRepMesh_IncrementalMesh_2(n, .1, !1, .5, !0);
                         const a = this._build_face_mesh(n);
                         let i = [];
-                        this._showEdge && (i = this._build_edge_mesh(n));
-                        const p = this._build_wire_mesh(n, .1);
-                        e[t.name] = {
-                            jcObject: t,
+                        this._shouldComputeEdge(r) && (i = this._build_edge_mesh(n));
+                        let p = [];
+                        this._shouldComputeWire(r) && (p = this._build_wire_mesh(n, .1)), e[r.name] = {
+                            jcObject: r,
                             faceList: a,
                             edgeList: [...i, ...p],
                             meta: s
                         }
                     })), e
                 }
+                _shouldComputeEdge(e) {
+                    var o;
+                    return "Part::Any" !== e.shape || "STL" !== (null === (o = e.parameters) || void 0 === o ? void 0 : o.Type)
+                }
+                _shouldComputeWire(e) {
+                    return "Sketcher::SketchObject" === e.shape
+                }
                 _build_wire_mesh(e, o) {
-                    const r = [],
-                        t = this._occ,
-                        n = new t.TopExp_Explorer_2(e, t.TopAbs_ShapeEnum.TopAbs_EDGE, t.TopAbs_ShapeEnum.TopAbs_SHAPE);
-                    for (n.Init(e, t.TopAbs_ShapeEnum.TopAbs_EDGE, t.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
-                        const e = t.TopoDS.Edge_1(n.Current()),
-                            s = new t.TopLoc_Location_1,
-                            a = new t.BRepAdaptor_Curve_2(e),
-                            i = new t.GCPnts_TangentialDeflection_2(a, o, .1, 2, 1e-9, 1e-7),
+                    const t = [],
+                        r = this._occ,
+                        n = new r.TopExp_Explorer_2(e, r.TopAbs_ShapeEnum.TopAbs_EDGE, r.TopAbs_ShapeEnum.TopAbs_SHAPE);
+                    for (n.Init(e, r.TopAbs_ShapeEnum.TopAbs_EDGE, r.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
+                        const e = r.TopoDS.Edge_1(n.Current()),
+                            s = new r.TopLoc_Location_1,
+                            a = new r.BRepAdaptor_Curve_2(e),
+                            i = new r.GCPnts_TangentialDeflection_2(a, o, .1, 2, 1e-9, 1e-7),
                             p = new Array(3 * i.NbPoints());
                         for (let e = 0; e < i.NbPoints(); e++) {
                             const o = i.Value(e + 1).Transformed(s.Transformation());
                             p[3 * e + 0] = o.X(), p[3 * e + 1] = o.Y(), p[3 * e + 2] = o.Z()
                         }
-                        r.push({
+                        t.push({
                             vertexCoord: p,
                             numberOfCoords: 3 * i.NbPoints()
                         }), n.Next()
                     }
-                    return r
+                    return t
                 }
                 _build_face_mesh(e) {
                     const o = [],
-                        r = [],
-                        t = this._occ,
-                        n = new t.TopExp_Explorer_2(e, t.TopAbs_ShapeEnum.TopAbs_FACE, t.TopAbs_ShapeEnum.TopAbs_SHAPE);
-                    for (n.Init(e, t.TopAbs_ShapeEnum.TopAbs_FACE, t.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
-                        const e = t.TopoDS.Face_1(n.Current()),
-                            s = new t.TopLoc_Location_1,
-                            a = t.BRep_Tool.Triangulation(e, s, 0);
+                        t = [],
+                        r = this._occ,
+                        n = new r.TopExp_Explorer_2(e, r.TopAbs_ShapeEnum.TopAbs_FACE, r.TopAbs_ShapeEnum.TopAbs_SHAPE);
+                    for (n.Init(e, r.TopAbs_ShapeEnum.TopAbs_FACE, r.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
+                        const e = r.TopoDS.Face_1(n.Current()),
+                            s = new r.TopLoc_Location_1,
+                            a = r.BRep_Tool.Triangulation(e, s, 0);
                         if (a.IsNull()) {
                             console.error("Encountered Null Face!"), n.Next();
                             continue
                         }
                         const i = {
                                 vertexCoord: [],
-                                normalCoord: [],
                                 triIndexes: [],
                                 numberOfTriangles: 0
                             },
-                            p = new t.Poly_Connect_2(a),
-                            c = a.get(),
-                            d = c.NbNodes();
-                        i.vertexCoord = new Array(3 * d);
-                        for (let e = 0; e < d; e++) {
-                            const o = c.Node(e + 1).Transformed(s.Transformation());
+                            p = a.get(),
+                            c = p.NbNodes();
+                        i.vertexCoord = new Array(3 * c);
+                        for (let e = 0; e < c; e++) {
+                            const o = p.Node(e + 1).Transformed(s.Transformation());
                             i.vertexCoord[3 * e + 0] = o.X(), i.vertexCoord[3 * e + 1] = o.Y(), i.vertexCoord[3 * e + 2] = o.Z()
                         }
-                        const _ = e.Orientation_1(),
-                            u = new t.TColgp_Array1OfDir_2(1, d);
-                        t.StdPrs_ToolTriangulatedShape.Normal(e, p, u), i.normalCoord = new Array(3 * u.Length());
-                        for (let e = 0; e < u.Length(); e++) {
-                            const o = u.Value(e + 1).Transformed(s.Transformation());
-                            i.normalCoord[3 * e + 0] = o.X(), i.normalCoord[3 * e + 1] = o.Y(), i.normalCoord[3 * e + 2] = o.Z()
-                        }
-                        const l = c.NbTriangles();
-                        i.triIndexes = new Array(3 * l);
-                        let h = 0;
+                        const d = e.Orientation_1(),
+                            u = p.NbTriangles();
+                        i.triIndexes = new Array(3 * u);
+                        let _ = 0;
                         for (let e = 1; e <= a.get().NbTriangles(); e++) {
-                            const o = c.Triangle(e);
-                            let r = o.Value(1),
+                            const o = p.Triangle(e);
+                            let t = o.Value(1),
                                 n = o.Value(2);
                             const s = o.Value(3);
-                            if (_ !== t.TopAbs_Orientation.TopAbs_FORWARD) {
-                                const e = r;
-                                r = n, n = e
+                            if (d !== r.TopAbs_Orientation.TopAbs_FORWARD) {
+                                const e = t;
+                                t = n, n = e
                             }
-                            i.triIndexes[3 * h + 0] = r - 1, i.triIndexes[3 * h + 1] = n - 1, i.triIndexes[3 * h + 2] = s - 1, h++
+                            i.triIndexes[3 * _ + 0] = t - 1, i.triIndexes[3 * _ + 1] = n - 1, i.triIndexes[3 * _ + 2] = s - 1, _++
                         }
-                        i.numberOfTriangles = h, o.push(i), r.push(a), n.Next()
+                        i.numberOfTriangles = _, o.push(i), t.push(a), n.Next()
                     }
                     return o
                 }
                 _build_edge_mesh(e) {
                     const o = this._occ,
-                        r = [],
-                        t = new o.TopTools_IndexedMapOfShape_1;
-                    o.TopExp.MapShapes_1(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, t);
+                        t = [],
+                        r = new o.TopTools_IndexedMapOfShape_1;
+                    o.TopExp.MapShapes_1(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, r);
                     const n = new o.TopTools_IndexedDataMapOfShapeListOfShape_1;
                     o.TopExp.MapShapesAndAncestors(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, o.TopAbs_ShapeEnum.TopAbs_FACE, n);
                     for (let e = 1; e <= n.Extent(); e++) {
                         if (0 === n.FindFromIndex(e).Extent()) continue;
-                        const s = o.TopoDS.Edge_1(t.FindKey(e));
+                        const s = o.TopoDS.Edge_1(r.FindKey(e));
                         let a = new o.gp_Trsf_1;
                         const i = new o.TopLoc_Location_1,
                             p = o.BRep_Tool.Polygon3D(s, i),
                             c = {
                                 vertexCoord: [],
                                 numberOfCoords: 0
                             };
                         let d;
                         if (p.IsNull()) {
-                            const r = o.TopoDS.Face_1(n.FindFromIndex(e).First_1()),
-                                t = o.BRep_Tool.Triangulation(r, i, 0);
+                            const t = o.TopoDS.Face_1(n.FindFromIndex(e).First_1()),
+                                r = o.BRep_Tool.Triangulation(t, i, 0);
                             i.IsIdentity() || (a = i.Transformation());
-                            const p = o.BRep_Tool.PolygonOnTriangulation_1(s, t, i);
+                            const p = o.BRep_Tool.PolygonOnTriangulation_1(s, r, i);
                             if (p.IsNull()) continue;
                             d = p.get().NbNodes(), c.numberOfCoords = d, c.vertexCoord = new Array(3 * d);
-                            const _ = p.get().Nodes(),
-                                u = t.get();
-                            for (let e = _.Lower(); e <= _.Upper(); e++) {
-                                const o = u.Node(_.Value(e));
+                            const u = p.get().Nodes(),
+                                _ = r.get();
+                            for (let e = u.Lower(); e <= u.Upper(); e++) {
+                                const o = _.Node(u.Value(e));
                                 o.Transform(a);
-                                const r = e - 1;
-                                c.vertexCoord[3 * r + 0] = o.X(), c.vertexCoord[3 * r + 1] = o.Y(), c.vertexCoord[3 * r + 2] = o.Z()
+                                const t = e - 1;
+                                c.vertexCoord[3 * t + 0] = o.X(), c.vertexCoord[3 * t + 1] = o.Y(), c.vertexCoord[3 * t + 2] = o.Z()
                             }
                         } else {
                             i.IsIdentity() || (a = i.Transformation()), d = p.get().NbNodes(), c.numberOfCoords = d, c.vertexCoord = new Array(3 * d);
                             const e = p.get().Nodes();
                             for (let o = 0; o < d; o++) {
-                                const r = e.Value(o + 1);
-                                r.Transform(a), c.vertexCoord[3 * o + 0] = r.X(), c.vertexCoord[3 * o + 1] = r.Y(), c.vertexCoord[3 * o + 2] = r.Z()
+                                const t = e.Value(o + 1);
+                                t.Transform(a), c.vertexCoord[3 * o + 0] = t.X(), c.vertexCoord[3 * o + 1] = t.Y(), c.vertexCoord[3 * o + 2] = t.Z()
                             }
                         }
-                        r.push(c)
+                        t.push(c)
                     }
-                    return r
+                    return t
                 }
             }
-            var n, s = r(3342),
-                a = r(7262),
+            var n, s = t(3283),
+                a = t(7262),
                 i = new Uint8Array(16);
 
             function p() {
                 if (!n && !(n = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || "undefined" != typeof msCrypto && "function" == typeof msCrypto.getRandomValues && msCrypto.getRandomValues.bind(msCrypto))) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
                 return n(i)
             }
             const c = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
-            for (var d = [], _ = 0; _ < 256; ++_) d.push((_ + 256).toString(16).substr(1));
-            const u = function(e) {
+            for (var d = [], u = 0; u < 256; ++u) d.push((u + 256).toString(16).substr(1));
+            const _ = function(e) {
                     var o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
-                        r = (d[e[o + 0]] + d[e[o + 1]] + d[e[o + 2]] + d[e[o + 3]] + "-" + d[e[o + 4]] + d[e[o + 5]] + "-" + d[e[o + 6]] + d[e[o + 7]] + "-" + d[e[o + 8]] + d[e[o + 9]] + "-" + d[e[o + 10]] + d[e[o + 11]] + d[e[o + 12]] + d[e[o + 13]] + d[e[o + 14]] + d[e[o + 15]]).toLowerCase();
+                        t = (d[e[o + 0]] + d[e[o + 1]] + d[e[o + 2]] + d[e[o + 3]] + "-" + d[e[o + 4]] + d[e[o + 5]] + "-" + d[e[o + 6]] + d[e[o + 7]] + "-" + d[e[o + 8]] + d[e[o + 9]] + "-" + d[e[o + 10]] + d[e[o + 11]] + d[e[o + 12]] + d[e[o + 13]] + d[e[o + 14]] + d[e[o + 15]]).toLowerCase();
                     if (! function(e) {
                             return "string" == typeof e && c.test(e)
-                        }(r)) throw TypeError("Stringified UUID is invalid");
-                    return r
+                        }(t)) throw TypeError("Stringified UUID is invalid");
+                    return t
                 },
-                l = function(e, o, r) {
-                    var t = (e = e || {}).random || (e.rng || p)();
-                    if (t[6] = 15 & t[6] | 64, t[8] = 63 & t[8] | 128, o) {
-                        r = r || 0;
-                        for (var n = 0; n < 16; ++n) o[r + n] = t[n];
+                l = function(e, o, t) {
+                    var r = (e = e || {}).random || (e.rng || p)();
+                    if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, o) {
+                        t = t || 0;
+                        for (var n = 0; n < 16; ++n) o[t + n] = r[n];
                         return o
                     }
-                    return u(t)
+                    return _(r)
                 };
             class h {
                 constructor(e) {
                     this._ready = new a.PromiseDelegate, this._messageChannels = new Map, this._nativeWorker = e.worker
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 register(e) {
                     const {
                         messageHandler: o,
-                        thisArg: r
-                    } = e, t = l(), n = new MessageChannel;
-                    r && o.bind(r), n.port1.onmessage = this._handlerFactory(o), this._messageChannels.set(t, n);
+                        thisArg: t
+                    } = e, r = l(), n = new MessageChannel;
+                    t && o.bind(t), n.port1.onmessage = this._handlerFactory(o), this._messageChannels.set(r, n);
                     const a = {
-                        id: t,
+                        id: r,
                         action: s.WorkerAction.REGISTER,
                         payload: {
-                            id: t
+                            id: r
                         }
                     };
-                    return this._nativeWorker.postMessage(a, [n.port2]), t
+                    return this._nativeWorker.postMessage(a, [n.port2]), r
                 }
                 unregister(e) {
                     this._messageChannels.delete(e)
                 }
                 postMessage(e) {
                     this._nativeWorker.postMessage(e)
                 }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/702.f302218e05c5eeadd41a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 702.ec2cae811960a903c14a.js.LICENSE.txt */
+/*! For license information please see 702.f302218e05c5eeadd41a.js.LICENSE.txt */
 (self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || []).push([
     [702], {
         2858: (e, t, n) => {
             "use strict";
             n.d(t, {
                 q: () => se
             });
@@ -35,18 +35,18 @@
                 }
             }((async () => {
                 const {
                     withTheme: e
                 } = await Promise.resolve().then(n.bind(n, 2192));
                 return e((await n.e(366).then(n.bind(n, 8366))).default)
             }));
-            var a = n(7638),
-                s = n(6901),
-                l = n(6597),
-                c = n(7714),
+            var a = n(8440),
+                s = n(7623),
+                l = n(7655),
+                c = n(2844),
                 u = n(4053),
                 h = n(9452),
                 d = n.n(h);
             let p = {
                 async: !1,
                 baseUrl: null,
                 breaks: !1,
@@ -14971,15 +14971,15 @@
             "use strict";
             var r = n(1372);
             e.exports = r
         },
         5023: (e, t, n) => {
             "use strict";
             var r = n(2490),
-                i = n(5283),
+                i = n(7664),
                 o = TypeError;
             e.exports = function(e) {
                 if (r(e)) return e;
                 throw new o(i(e) + " is not a function")
             }
         },
         780: e => {
@@ -15559,15 +15559,15 @@
             var r = n(7836),
                 i = n(8730);
             e.exports = function(e) {
                 var t = r(e, "string");
                 return i(t) ? t : t + ""
             }
         },
-        5283: e => {
+        7664: e => {
             "use strict";
             var t = String;
             e.exports = function(e) {
                 try {
                     return t(e)
                 } catch (e) {
                     return "Object"
@@ -16789,15 +16789,15 @@
                 for (var r = -1, i = null == e ? 0 : e.length; ++r < i;)
                     if (n(t, e[r])) return !0;
                 return !1
             }
         },
         358: (e, t, n) => {
             var r = n(6137),
-                i = n(3283),
+                i = n(5664),
                 o = n(3142),
                 a = n(5853),
                 s = n(9632),
                 l = n(8666),
                 c = Object.prototype.hasOwnProperty;
             e.exports = function(e, t) {
                 var n = o(e),
@@ -17307,15 +17307,15 @@
         },
         6885: (e, t, n) => {
             var r = n(4810),
                 i = n(7099),
                 o = n(2264),
                 a = n(4354),
                 s = n(5964),
-                l = n(3283),
+                l = n(5664),
                 c = n(3142),
                 u = n(5406),
                 h = n(5853),
                 d = n(3655),
                 p = n(1580),
                 f = n(8360),
                 m = n(8666),
@@ -17378,15 +17378,15 @@
                 return r(e, t, (function(t, n) {
                     return i(e, n)
                 }))
             }
         },
         5031: (e, t, n) => {
             var r = n(7923),
-                i = n(7655),
+                i = n(36),
                 o = n(3526);
             e.exports = function(e, t, n) {
                 for (var a = -1, s = t.length, l = {}; ++a < s;) {
                     var c = t[a],
                         u = r(e, c);
                     n(u, c) && i(l, o(c, e), u)
                 }
@@ -17430,15 +17430,15 @@
             var r = n(2053),
                 i = n(5234),
                 o = n(796);
             e.exports = function(e, t) {
                 return o(i(e, t, r), e + "")
             }
         },
-        7655: (e, t, n) => {
+        36: (e, t, n) => {
             var r = n(3422),
                 i = n(3526),
                 o = n(9632),
                 a = n(1580),
                 s = n(6040);
             e.exports = function(e, t, n, l) {
                 if (!a(e)) return e;
@@ -18001,15 +18001,15 @@
         155: e => {
             e.exports = function(e, t) {
                 return null == e ? void 0 : e[t]
             }
         },
         5899: (e, t, n) => {
             var r = n(3526),
-                i = n(3283),
+                i = n(5664),
                 o = n(3142),
                 a = n(9632),
                 s = n(5387),
                 l = n(6040);
             e.exports = function(e, t, n) {
                 for (var c = -1, u = (t = r(t, e)).length, h = !1; ++c < u;) {
                     var d = l(t[c]);
@@ -18111,15 +18111,15 @@
                 o = n(4882);
             e.exports = function(e) {
                 return "function" != typeof e.constructor || o(e) ? {} : r(i(e))
             }
         },
         714: (e, t, n) => {
             var r = n(5650),
-                i = n(3283),
+                i = n(5664),
                 o = n(3142),
                 a = r ? r.isConcatSpreadable : void 0;
             e.exports = function(e) {
                 return o(e) || i(e) || !!(a && e && e[a])
             }
         },
         9632: e => {
@@ -18572,15 +18572,15 @@
                 l = o((function(e) {
                     var t = s(e),
                         n = r(e, a);
                     return (t = "function" == typeof t ? t : void 0) && n.pop(), n.length && n[0] === e[0] ? i(n, void 0, t) : []
                 }));
             e.exports = l
         },
-        3283: (e, t, n) => {
+        5664: (e, t, n) => {
             var r = n(6027),
                 i = n(547),
                 o = Object.prototype,
                 a = o.hasOwnProperty,
                 s = o.propertyIsEnumerable,
                 l = r(function() {
                     return arguments
@@ -18623,15 +18623,15 @@
                 s = a && a.exports === o ? r.Buffer : void 0,
                 l = (s ? s.isBuffer : void 0) || i;
             e.exports = l
         },
         3514: (e, t, n) => {
             var r = n(195),
                 i = n(8486),
-                o = n(3283),
+                o = n(5664),
                 a = n(3142),
                 s = n(6529),
                 l = n(5853),
                 c = n(4882),
                 u = n(8666),
                 h = Object.prototype.hasOwnProperty;
             e.exports = function(e) {
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/794.55a891e10ed7a9b7a805.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/794.65d4da338c815b694314.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,210 +1,209 @@
 "use strict";
 (self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || []).push([
     [794, 413], {
-        9794: (e, o, r) => {
-            r.r(o), r.d(o, {
-                OccParser: () => t,
+        9794: (e, o, t) => {
+            t.r(o), t.d(o, {
+                OccParser: () => r,
                 OccWorker: () => h
             });
-            class t {
+            class r {
                 constructor(e) {
-                    this._occ = self.occ, this._showEdge = !0, this._shapeList = e
+                    this._occ = self.occ, this._shapeList = e
                 }
                 execute() {
                     const e = {};
                     return this._shapeList.forEach((o => {
                         const {
-                            shapeData: r,
-                            jcObject: t
+                            shapeData: t,
+                            jcObject: r
                         } = o, {
                             occShape: n,
                             metadata: s
-                        } = r;
+                        } = t;
                         if (!n) return;
                         new this._occ.BRepMesh_IncrementalMesh_2(n, .1, !1, .5, !0);
                         const a = this._build_face_mesh(n);
                         let i = [];
-                        this._showEdge && (i = this._build_edge_mesh(n));
-                        const p = this._build_wire_mesh(n, .1);
-                        e[t.name] = {
-                            jcObject: t,
+                        this._shouldComputeEdge(r) && (i = this._build_edge_mesh(n));
+                        let p = [];
+                        this._shouldComputeWire(r) && (p = this._build_wire_mesh(n, .1)), e[r.name] = {
+                            jcObject: r,
                             faceList: a,
                             edgeList: [...i, ...p],
                             meta: s
                         }
                     })), e
                 }
+                _shouldComputeEdge(e) {
+                    var o;
+                    return "Part::Any" !== e.shape || "STL" !== (null === (o = e.parameters) || void 0 === o ? void 0 : o.Type)
+                }
+                _shouldComputeWire(e) {
+                    return "Sketcher::SketchObject" === e.shape
+                }
                 _build_wire_mesh(e, o) {
-                    const r = [],
-                        t = this._occ,
-                        n = new t.TopExp_Explorer_2(e, t.TopAbs_ShapeEnum.TopAbs_EDGE, t.TopAbs_ShapeEnum.TopAbs_SHAPE);
-                    for (n.Init(e, t.TopAbs_ShapeEnum.TopAbs_EDGE, t.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
-                        const e = t.TopoDS.Edge_1(n.Current()),
-                            s = new t.TopLoc_Location_1,
-                            a = new t.BRepAdaptor_Curve_2(e),
-                            i = new t.GCPnts_TangentialDeflection_2(a, o, .1, 2, 1e-9, 1e-7),
+                    const t = [],
+                        r = this._occ,
+                        n = new r.TopExp_Explorer_2(e, r.TopAbs_ShapeEnum.TopAbs_EDGE, r.TopAbs_ShapeEnum.TopAbs_SHAPE);
+                    for (n.Init(e, r.TopAbs_ShapeEnum.TopAbs_EDGE, r.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
+                        const e = r.TopoDS.Edge_1(n.Current()),
+                            s = new r.TopLoc_Location_1,
+                            a = new r.BRepAdaptor_Curve_2(e),
+                            i = new r.GCPnts_TangentialDeflection_2(a, o, .1, 2, 1e-9, 1e-7),
                             p = new Array(3 * i.NbPoints());
                         for (let e = 0; e < i.NbPoints(); e++) {
                             const o = i.Value(e + 1).Transformed(s.Transformation());
                             p[3 * e + 0] = o.X(), p[3 * e + 1] = o.Y(), p[3 * e + 2] = o.Z()
                         }
-                        r.push({
+                        t.push({
                             vertexCoord: p,
                             numberOfCoords: 3 * i.NbPoints()
                         }), n.Next()
                     }
-                    return r
+                    return t
                 }
                 _build_face_mesh(e) {
                     const o = [],
-                        r = [],
-                        t = this._occ,
-                        n = new t.TopExp_Explorer_2(e, t.TopAbs_ShapeEnum.TopAbs_FACE, t.TopAbs_ShapeEnum.TopAbs_SHAPE);
-                    for (n.Init(e, t.TopAbs_ShapeEnum.TopAbs_FACE, t.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
-                        const e = t.TopoDS.Face_1(n.Current()),
-                            s = new t.TopLoc_Location_1,
-                            a = t.BRep_Tool.Triangulation(e, s, 0);
+                        t = [],
+                        r = this._occ,
+                        n = new r.TopExp_Explorer_2(e, r.TopAbs_ShapeEnum.TopAbs_FACE, r.TopAbs_ShapeEnum.TopAbs_SHAPE);
+                    for (n.Init(e, r.TopAbs_ShapeEnum.TopAbs_FACE, r.TopAbs_ShapeEnum.TopAbs_SHAPE); n.More();) {
+                        const e = r.TopoDS.Face_1(n.Current()),
+                            s = new r.TopLoc_Location_1,
+                            a = r.BRep_Tool.Triangulation(e, s, 0);
                         if (a.IsNull()) {
                             console.error("Encountered Null Face!"), n.Next();
                             continue
                         }
                         const i = {
                                 vertexCoord: [],
-                                normalCoord: [],
                                 triIndexes: [],
                                 numberOfTriangles: 0
                             },
-                            p = new t.Poly_Connect_2(a),
-                            c = a.get(),
-                            d = c.NbNodes();
-                        i.vertexCoord = new Array(3 * d);
-                        for (let e = 0; e < d; e++) {
-                            const o = c.Node(e + 1).Transformed(s.Transformation());
+                            p = a.get(),
+                            c = p.NbNodes();
+                        i.vertexCoord = new Array(3 * c);
+                        for (let e = 0; e < c; e++) {
+                            const o = p.Node(e + 1).Transformed(s.Transformation());
                             i.vertexCoord[3 * e + 0] = o.X(), i.vertexCoord[3 * e + 1] = o.Y(), i.vertexCoord[3 * e + 2] = o.Z()
                         }
-                        const _ = e.Orientation_1(),
-                            u = new t.TColgp_Array1OfDir_2(1, d);
-                        t.StdPrs_ToolTriangulatedShape.Normal(e, p, u), i.normalCoord = new Array(3 * u.Length());
-                        for (let e = 0; e < u.Length(); e++) {
-                            const o = u.Value(e + 1).Transformed(s.Transformation());
-                            i.normalCoord[3 * e + 0] = o.X(), i.normalCoord[3 * e + 1] = o.Y(), i.normalCoord[3 * e + 2] = o.Z()
-                        }
-                        const l = c.NbTriangles();
-                        i.triIndexes = new Array(3 * l);
-                        let h = 0;
+                        const d = e.Orientation_1(),
+                            u = p.NbTriangles();
+                        i.triIndexes = new Array(3 * u);
+                        let _ = 0;
                         for (let e = 1; e <= a.get().NbTriangles(); e++) {
-                            const o = c.Triangle(e);
-                            let r = o.Value(1),
+                            const o = p.Triangle(e);
+                            let t = o.Value(1),
                                 n = o.Value(2);
                             const s = o.Value(3);
-                            if (_ !== t.TopAbs_Orientation.TopAbs_FORWARD) {
-                                const e = r;
-                                r = n, n = e
+                            if (d !== r.TopAbs_Orientation.TopAbs_FORWARD) {
+                                const e = t;
+                                t = n, n = e
                             }
-                            i.triIndexes[3 * h + 0] = r - 1, i.triIndexes[3 * h + 1] = n - 1, i.triIndexes[3 * h + 2] = s - 1, h++
+                            i.triIndexes[3 * _ + 0] = t - 1, i.triIndexes[3 * _ + 1] = n - 1, i.triIndexes[3 * _ + 2] = s - 1, _++
                         }
-                        i.numberOfTriangles = h, o.push(i), r.push(a), n.Next()
+                        i.numberOfTriangles = _, o.push(i), t.push(a), n.Next()
                     }
                     return o
                 }
                 _build_edge_mesh(e) {
                     const o = this._occ,
-                        r = [],
-                        t = new o.TopTools_IndexedMapOfShape_1;
-                    o.TopExp.MapShapes_1(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, t);
+                        t = [],
+                        r = new o.TopTools_IndexedMapOfShape_1;
+                    o.TopExp.MapShapes_1(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, r);
                     const n = new o.TopTools_IndexedDataMapOfShapeListOfShape_1;
                     o.TopExp.MapShapesAndAncestors(e, o.TopAbs_ShapeEnum.TopAbs_EDGE, o.TopAbs_ShapeEnum.TopAbs_FACE, n);
                     for (let e = 1; e <= n.Extent(); e++) {
                         if (0 === n.FindFromIndex(e).Extent()) continue;
-                        const s = o.TopoDS.Edge_1(t.FindKey(e));
+                        const s = o.TopoDS.Edge_1(r.FindKey(e));
                         let a = new o.gp_Trsf_1;
                         const i = new o.TopLoc_Location_1,
                             p = o.BRep_Tool.Polygon3D(s, i),
                             c = {
                                 vertexCoord: [],
                                 numberOfCoords: 0
                             };
                         let d;
                         if (p.IsNull()) {
-                            const r = o.TopoDS.Face_1(n.FindFromIndex(e).First_1()),
-                                t = o.BRep_Tool.Triangulation(r, i, 0);
+                            const t = o.TopoDS.Face_1(n.FindFromIndex(e).First_1()),
+                                r = o.BRep_Tool.Triangulation(t, i, 0);
                             i.IsIdentity() || (a = i.Transformation());
-                            const p = o.BRep_Tool.PolygonOnTriangulation_1(s, t, i);
+                            const p = o.BRep_Tool.PolygonOnTriangulation_1(s, r, i);
                             if (p.IsNull()) continue;
                             d = p.get().NbNodes(), c.numberOfCoords = d, c.vertexCoord = new Array(3 * d);
-                            const _ = p.get().Nodes(),
-                                u = t.get();
-                            for (let e = _.Lower(); e <= _.Upper(); e++) {
-                                const o = u.Node(_.Value(e));
+                            const u = p.get().Nodes(),
+                                _ = r.get();
+                            for (let e = u.Lower(); e <= u.Upper(); e++) {
+                                const o = _.Node(u.Value(e));
                                 o.Transform(a);
-                                const r = e - 1;
-                                c.vertexCoord[3 * r + 0] = o.X(), c.vertexCoord[3 * r + 1] = o.Y(), c.vertexCoord[3 * r + 2] = o.Z()
+                                const t = e - 1;
+                                c.vertexCoord[3 * t + 0] = o.X(), c.vertexCoord[3 * t + 1] = o.Y(), c.vertexCoord[3 * t + 2] = o.Z()
                             }
                         } else {
                             i.IsIdentity() || (a = i.Transformation()), d = p.get().NbNodes(), c.numberOfCoords = d, c.vertexCoord = new Array(3 * d);
                             const e = p.get().Nodes();
                             for (let o = 0; o < d; o++) {
-                                const r = e.Value(o + 1);
-                                r.Transform(a), c.vertexCoord[3 * o + 0] = r.X(), c.vertexCoord[3 * o + 1] = r.Y(), c.vertexCoord[3 * o + 2] = r.Z()
+                                const t = e.Value(o + 1);
+                                t.Transform(a), c.vertexCoord[3 * o + 0] = t.X(), c.vertexCoord[3 * o + 1] = t.Y(), c.vertexCoord[3 * o + 2] = t.Z()
                             }
                         }
-                        r.push(c)
+                        t.push(c)
                     }
-                    return r
+                    return t
                 }
             }
-            var n, s = r(3342),
-                a = r(7262),
+            var n, s = t(3283),
+                a = t(7262),
                 i = new Uint8Array(16);
 
             function p() {
                 if (!n && !(n = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || "undefined" != typeof msCrypto && "function" == typeof msCrypto.getRandomValues && msCrypto.getRandomValues.bind(msCrypto))) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
                 return n(i)
             }
             const c = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
-            for (var d = [], _ = 0; _ < 256; ++_) d.push((_ + 256).toString(16).substr(1));
-            const u = function(e) {
+            for (var d = [], u = 0; u < 256; ++u) d.push((u + 256).toString(16).substr(1));
+            const _ = function(e) {
                     var o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
-                        r = (d[e[o + 0]] + d[e[o + 1]] + d[e[o + 2]] + d[e[o + 3]] + "-" + d[e[o + 4]] + d[e[o + 5]] + "-" + d[e[o + 6]] + d[e[o + 7]] + "-" + d[e[o + 8]] + d[e[o + 9]] + "-" + d[e[o + 10]] + d[e[o + 11]] + d[e[o + 12]] + d[e[o + 13]] + d[e[o + 14]] + d[e[o + 15]]).toLowerCase();
+                        t = (d[e[o + 0]] + d[e[o + 1]] + d[e[o + 2]] + d[e[o + 3]] + "-" + d[e[o + 4]] + d[e[o + 5]] + "-" + d[e[o + 6]] + d[e[o + 7]] + "-" + d[e[o + 8]] + d[e[o + 9]] + "-" + d[e[o + 10]] + d[e[o + 11]] + d[e[o + 12]] + d[e[o + 13]] + d[e[o + 14]] + d[e[o + 15]]).toLowerCase();
                     if (! function(e) {
                             return "string" == typeof e && c.test(e)
-                        }(r)) throw TypeError("Stringified UUID is invalid");
-                    return r
+                        }(t)) throw TypeError("Stringified UUID is invalid");
+                    return t
                 },
-                l = function(e, o, r) {
-                    var t = (e = e || {}).random || (e.rng || p)();
-                    if (t[6] = 15 & t[6] | 64, t[8] = 63 & t[8] | 128, o) {
-                        r = r || 0;
-                        for (var n = 0; n < 16; ++n) o[r + n] = t[n];
+                l = function(e, o, t) {
+                    var r = (e = e || {}).random || (e.rng || p)();
+                    if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, o) {
+                        t = t || 0;
+                        for (var n = 0; n < 16; ++n) o[t + n] = r[n];
                         return o
                     }
-                    return u(t)
+                    return _(r)
                 };
             class h {
                 constructor(e) {
                     this._ready = new a.PromiseDelegate, this._messageChannels = new Map, this._nativeWorker = e.worker
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 register(e) {
                     const {
                         messageHandler: o,
-                        thisArg: r
-                    } = e, t = l(), n = new MessageChannel;
-                    r && o.bind(r), n.port1.onmessage = this._handlerFactory(o), this._messageChannels.set(t, n);
+                        thisArg: t
+                    } = e, r = l(), n = new MessageChannel;
+                    t && o.bind(t), n.port1.onmessage = this._handlerFactory(o), this._messageChannels.set(r, n);
                     const a = {
-                        id: t,
+                        id: r,
                         action: s.WorkerAction.REGISTER,
                         payload: {
-                            id: t
+                            id: r
                         }
                     };
-                    return this._nativeWorker.postMessage(a, [n.port2]), t
+                    return this._nativeWorker.postMessage(a, [n.port2]), r
                 }
                 unregister(e) {
                     this._messageChannels.delete(e)
                 }
                 postMessage(e) {
                     this._nativeWorker.postMessage(e)
                 }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/813.013761880a7e5d30e958.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/813.b937fc9b357ed86a0372.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,21 +4,21 @@
         2813: (e, t, r) => {
             r.r(t), r.d(t, {
                 JupyterCadWidgetFactory: () => l,
                 JupyterCadWorkerRegistry: () => S,
                 default: () => I
             });
             var i = r(4796),
-                n = r(3342),
-                o = r(7638),
-                a = r(9221),
-                s = r(1595),
-                c = r(7664),
-                d = r(8859),
-                p = r(8626);
+                n = r(3283),
+                o = r(8440),
+                a = r(9943),
+                s = r(9265),
+                c = r(2126),
+                d = r(921),
+                p = r(207);
             class l extends d.ABCWidgetFactory {
                 constructor(e) {
                     const {
                         backendCheck: t,
                         externalCommandRegistry: r
                     } = e;
                     super(function(e, t) {
@@ -353,17 +353,17 @@
                     o && o.sharedModelFactory.registerDocumentFactory("stl", (() => new j)), a.widgetCreated.connect(((i, n) => {
                         n.context.pathChanged.connect((() => {
                             t.save(n)
                         })), r.themeChanged.connect(((e, t) => n.context.model.themeChanged.emit(t))), t.add(n), e.shell.activateById("jupytercad::leftControlPanel"), e.shell.activateById("jupytercad::rightControlPanel")
                     }))
                 }
             };
-            var T = r(1381),
-                k = r(7714),
-                w = r(492);
+            var T = r(8215),
+                k = r(2844),
+                w = r(9169);
             class S {
                 constructor() {
                     this._registry = new Map;
                     const e = new Worker(new URL(r.p + r.u(201), r.b));
                     this._defaultWorker = new w.OccWorker({
                         worker: e
                     })
@@ -380,15 +380,15 @@
                 getWorker(e) {
                     return this._registry.get(e)
                 }
                 getAllWorkers() {
                     return [...this._registry.values()]
                 }
             }
-            const R = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the object":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Post::Operator":{"type":"object","required":["Object"],"additionalProperties":true,"properties":{"Object":{"type":"string","description":"The name of input object"}}},"Part::Any":{"type":"object","required":["Content","Type"],"additionalProperties":false,"properties":{"Content":{"type":"string","description":"The string content of the object"},"Type":{"type":"string","enum":["brep","step","stl"]},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Chamfer":{"type":"object","required":["Base","Edge","Dist","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Dist":{"type":"number","description":"The distance of the symmetric chamfer"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Fillet":{"type":"object","required":["Base","Edge","Radius","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Radius":{"type":"number","description":"The radius for the fillet"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const R = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the object":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Post::Operator":{"type":"object","required":["Object"],"additionalProperties":true,"properties":{"Object":{"type":"string","description":"The name of input object"}}},"Part::Any":{"type":"object","required":["Content","Type"],"additionalProperties":false,"properties":{"Content":{"type":"string","description":"The string content of the object"},"Type":{"type":"string","enum":["brep","step","stl"]},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Chamfer":{"type":"object","required":["Base","Edge","Dist","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Dist":{"type":"number","description":"The distance of the symmetric chamfer"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Fillet":{"type":"object","required":["Base","Edge","Radius","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Radius":{"type":"number","description":"The radius for the fillet"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             class v {
                 constructor() {
                     this._registry = new Map(Object.entries(R))
                 }
                 registerSchema(e, t) {
                     this._registry.has(e) ? console.error("Worker is already registered!") : this._registry.set(e, t)
                 }
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/jupytercad.opencascade.wasm` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/remoteEntry.42b7768c40743ee87403.js` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/remoteEntry.0e4fbdda31fcefbd6536.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, d, f, l, u, i, c, s, p, b, h, v, m, y, g, j, w, P, S, k, E = {
+    var e, r, t, a, o, n, f, d, l, u, i, c, s, p, b, h, v, m, y, g, j, w, P, S, k, E = {
             2401: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(262), t.e(602), t.e(342), t.e(644), t.e(813)]).then((() => () => t(2813))),
-                        "./extension": () => Promise.all([t.e(262), t.e(602), t.e(342), t.e(644), t.e(813)]).then((() => () => t(2813))),
+                        "./index": () => Promise.all([t.e(262), t.e(602), t.e(283), t.e(820), t.e(813)]).then((() => () => t(2813))),
+                        "./extension": () => Promise.all([t.e(262), t.e(602), t.e(283), t.e(820), t.e(813)]).then((() => () => t(2813))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -44,85 +44,85 @@
         }), r
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        32: "249c6bd27daaea51e991",
         36: "699cdc9ecc81734b4ed2",
+        54: "82242ec748b90c3c68dc",
         197: "93f84c7921605ea391a1",
-        201: "7c726c3797b41065333d",
+        201: "0c67a92e1b3da08ee0d5",
         226: "9d3aa6c870e5597b7470",
-        262: "a4099c9aa3c3452ec3d3",
+        262: "a762b41f970a9a2e0576",
         279: "04093e206c0c74048dd7",
+        283: "dfd5d50de209e2314105",
         341: "dc0a046959cb1d02b85c",
-        342: "c1128ed25dbde3d0f9fd",
         366: "f05a9a2d265b69bc39df",
-        413: "e3edef5e15636d5f7630",
+        413: "378697570d8f23193ff4",
         432: "95862c204ad10cbf88b7",
         509: "74b2abfe3e59889c4fb9",
         601: "cf6a431ba637c1b317f2",
-        602: "4c95dde683ea2cdb62eb",
-        644: "42ff2779d9e633efa2b0",
-        702: "ec2cae811960a903c14a",
+        602: "b711147bf1f1eea3595b",
+        702: "f302218e05c5eeadd41a",
         733: "56e708a06e7632c214b0",
-        794: "55a891e10ed7a9b7a805",
-        813: "013761880a7e5d30e958"
+        794: "65d4da338c815b694314",
+        813: "b937fc9b357ed86a0372",
+        820: "d4b61627f6aef0e2c8ab"
     } [e] + ".js?v=" + {
-        32: "249c6bd27daaea51e991",
         36: "699cdc9ecc81734b4ed2",
+        54: "82242ec748b90c3c68dc",
         197: "93f84c7921605ea391a1",
-        201: "7c726c3797b41065333d",
+        201: "0c67a92e1b3da08ee0d5",
         226: "9d3aa6c870e5597b7470",
-        262: "a4099c9aa3c3452ec3d3",
+        262: "a762b41f970a9a2e0576",
         279: "04093e206c0c74048dd7",
+        283: "dfd5d50de209e2314105",
         341: "dc0a046959cb1d02b85c",
-        342: "c1128ed25dbde3d0f9fd",
         366: "f05a9a2d265b69bc39df",
-        413: "e3edef5e15636d5f7630",
+        413: "378697570d8f23193ff4",
         432: "95862c204ad10cbf88b7",
         509: "74b2abfe3e59889c4fb9",
         601: "cf6a431ba637c1b317f2",
-        602: "4c95dde683ea2cdb62eb",
-        644: "42ff2779d9e633efa2b0",
-        702: "ec2cae811960a903c14a",
+        602: "b711147bf1f1eea3595b",
+        702: "f302218e05c5eeadd41a",
         733: "56e708a06e7632c214b0",
-        794: "55a891e10ed7a9b7a805",
-        813: "013761880a7e5d30e958"
+        794: "65d4da338c815b694314",
+        813: "b937fc9b357ed86a0372",
+        820: "d4b61627f6aef0e2c8ab"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupytercad/jupytercad-core:", x.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var d, f;
+            var f, d;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
                     var i = l[u];
                     if (i.getAttribute("src") == t || i.getAttribute("data-webpack") == r + o) {
-                        d = i;
+                        f = i;
                         break
                     }
                 }
-            d || (f = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, x.nc && d.setAttribute("nonce", x.nc), d.setAttribute("data-webpack", r + o), d.src = t), e[t] = [a];
+            f || (d = !0, (f = document.createElement("script")).charset = "utf-8", f.timeout = 120, x.nc && f.setAttribute("nonce", x.nc), f.setAttribute("data-webpack", r + o), f.src = t), e[t] = [a];
             var c = (r, a) => {
-                    d.onerror = d.onload = null, clearTimeout(s);
+                    f.onerror = f.onload = null, clearTimeout(s);
                     var o = e[t];
-                    if (delete e[t], d.parentNode && d.parentNode.removeChild(d), o && o.forEach((e => e(a))), r) return r(a)
+                    if (delete e[t], f.parentNode && f.parentNode.removeChild(f), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
-                    target: d
+                    target: f
                 }), 12e4);
-            d.onerror = c.bind(null, d.onerror), d.onload = c.bind(null, d.onload), f && document.head.appendChild(d)
+            f.onerror = c.bind(null, f.onerror), f.onload = c.bind(null, f.onload), d && document.head.appendChild(f)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -133,26 +133,26 @@
         x.I = (t, a) => {
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 x.o(x.S, t) || (x.S[t] = {});
                 var n = x.S[t],
-                    d = "@jupytercad/jupytercad-core",
-                    f = (e, r, t, a) => {
+                    f = "@jupytercad/jupytercad-core",
+                    d = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            f = o[r];
-                        (!f || !f.loaded && (!a != !f.eager ? a : d > f.from)) && (o[r] = {
+                            d = o[r];
+                        (!d || !d.loaded && (!a != !d.eager ? a : f > d.from)) && (o[r] = {
                             get: t,
-                            from: d,
+                            from: f,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (f("@jupytercad/base", "2.0.0-alpha.6", (() => Promise.all([x.e(279), x.e(702), x.e(602), x.e(342), x.e(32), x.e(644)]).then((() => () => x(2070))))), f("@jupytercad/jupytercad-core", "2.0.0-alpha.6", (() => Promise.all([x.e(262), x.e(602), x.e(342), x.e(644), x.e(813)]).then((() => () => x(2813))))), f("@jupytercad/occ-worker", "2.0.0-alpha.6", (() => Promise.all([x.e(262), x.e(342), x.e(794)]).then((() => () => x(9794))))), f("@jupytercad/schema", "2.0.0-alpha.6", (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupytercad/base", "2.0.0-alpha.7", (() => Promise.all([x.e(279), x.e(702), x.e(602), x.e(283), x.e(54), x.e(820)]).then((() => () => x(2070))))), d("@jupytercad/jupytercad-core", "2.0.0-alpha.7", (() => Promise.all([x.e(262), x.e(602), x.e(283), x.e(820), x.e(813)]).then((() => () => x(2813))))), d("@jupytercad/occ-worker", "2.0.0-alpha.7", (() => Promise.all([x.e(262), x.e(283), x.e(794)]).then((() => () => x(9794))))), d("@jupytercad/schema", "2.0.0-alpha.7", (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -170,79 +170,79 @@
     }, a = (e, r) => {
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
-            var d = r[a],
-                f = (typeof d)[0];
-            if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
-            if ("o" != n && "u" != n && o != d) return o < d;
+            var f = r[a],
+                d = (typeof f)[0];
+            if (n != d) return "o" == n && "n" == d || "s" == d || "u" == n;
+            if ("o" != n && "u" != n && o != f) return o < f;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(f = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(d = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
-        var d = [];
+        var f = [];
         for (n = 1; n < e.length; n++) {
-            var f = e[n];
-            d.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? d.pop() + " " + d.pop() : o(f))
+            var d = e[n];
+            f.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? f.pop() + " " + f.pop() : o(d))
         }
         return l();
 
         function l() {
-            return d.pop().replace(/^\((.+)\)$/, "$1")
+            return f.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var d = 0, f = 1, l = !0;; f++, d++) {
-                var u, i, c = f < e.length ? (typeof e[f])[0] : "";
-                if (d >= r.length || "o" == (i = (typeof(u = r[d]))[0])) return !l || ("u" == c ? f > a && !o : "" == c != o);
+            for (var f = 0, d = 1, l = !0;; d++, f++) {
+                var u, i, c = d < e.length ? (typeof e[d])[0] : "";
+                if (f >= r.length || "o" == (i = (typeof(u = r[f]))[0])) return !l || ("u" == c ? d > a && !o : "" == c != o);
                 if ("u" == i) {
                     if (!l || "u" != c) return !1
                 } else if (l)
                     if (c == i)
-                        if (f <= a) {
-                            if (u != e[f]) return !1
+                        if (d <= a) {
+                            if (u != e[d]) return !1
                         } else {
-                            if (o ? u > e[f] : u < e[f]) return !1;
-                            u != e[f] && (l = !1)
+                            if (o ? u > e[d] : u < e[d]) return !1;
+                            u != e[d] && (l = !1)
                         }
                 else if ("s" != c && "n" != c) {
-                    if (o || f <= a) return !1;
-                    l = !1, f--
+                    if (o || d <= a) return !1;
+                    l = !1, d--
                 } else {
-                    if (f <= a || i < c != o) return !1;
+                    if (d <= a || i < c != o) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, f--)
+                } else "s" != c && "n" != c && (l = !1, d--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
-        for (d = 1; d < e.length; d++) {
-            var b = e[d];
+        for (f = 1; f < e.length; f++) {
+            var b = e[f];
             s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
         }
         return !!p()
-    }, d = (e, r) => {
+    }, f = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, f = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", i = (e, r, t, a) => {
         var o = l(e, t);
@@ -256,50 +256,50 @@
     }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, b = (e, r, t, a) => {
         p(s(e, r, t, a))
     }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, a, o) {
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
-    })(((e, r, t, a) => (d(e, t), h(c(r, t, a) || b(r, e, t, a) || f(r, t))))), y = v(((e, r, t, a) => (d(e, t), i(r, 0, t, a)))), g = v(((e, r, t, a, o) => r && x.o(r, t) ? i(r, 0, t, a) : o())), j = v(((e, r, t, a, o) => {
+    })(((e, r, t, a) => (f(e, t), h(c(r, t, a) || b(r, e, t, a) || d(r, t))))), y = v(((e, r, t, a) => (f(e, t), i(r, 0, t, a)))), g = v(((e, r, t, a, o) => r && x.o(r, t) ? i(r, 0, t, a) : o())), j = v(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && c(r, t, a);
         return n ? h(n) : o()
     })), w = {}, P = {
         7262: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4602: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
-        3342: () => g("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 6], (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341))))),
-        7638: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        7664: () => y("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        7714: () => y("default", "@jupyterlab/translation", [1, 4, 1, 6]),
-        8859: () => m("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
-        492: () => j("default", "@jupytercad/occ-worker", [1, 2, 0, 0, , "alpha", 6], (() => x.e(413).then((() => () => x(9794))))),
-        1381: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
-        1595: () => y("default", "@jupyterlab/launcher", [1, 4, 1, 6]),
+        3283: () => g("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 7], (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341))))),
+        921: () => m("default", "@jupyterlab/docregistry", [1, 4, 1, 8]),
+        2126: () => y("default", "@jupyterlab/ui-components", [1, 4, 1, 8]),
+        2844: () => y("default", "@jupyterlab/translation", [1, 4, 1, 8]),
+        8440: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        207: () => g("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 7], (() => Promise.all([x.e(279), x.e(702), x.e(54)]).then((() => () => x(2070))))),
         4796: () => y("default", "@jupyter/docprovider", [1, 2, 0, 0]),
-        8626: () => g("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 6], (() => Promise.all([x.e(279), x.e(702), x.e(32)]).then((() => () => x(2070))))),
-        9221: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
-        2486: () => y("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        8215: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
+        9169: () => j("default", "@jupytercad/occ-worker", [1, 2, 0, 0, , "alpha", 7], (() => x.e(413).then((() => () => x(9794))))),
+        9265: () => y("default", "@jupyterlab/launcher", [1, 4, 1, 8]),
+        9943: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
         3345: () => y("default", "react", [1, 18, 2, 0]),
         4053: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        4123: () => m("default", "@jupyterlab/observables", [1, 5, 1, 8]),
         5256: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         6167: () => y("default", "@lumino/commands", [1, 2, 0, 1]),
         6230: () => y("default", "@lumino/messaging", [1, 2, 0, 0]),
-        6597: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
-        6901: () => y("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
-        8265: () => m("default", "@jupyterlab/observables", [1, 5, 1, 6]),
+        7623: () => y("default", "@jupyterlab/codemirror", [1, 4, 1, 8]),
+        7655: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
+        8824: () => y("default", "@jupyterlab/services", [1, 7, 1, 8]),
         667: () => y("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         2206: () => y("default", "yjs", [1, 13, 5, 40])
     }, S = {
-        32: [2486, 3345, 4053, 5256, 6167, 6230, 6597, 6901, 8265],
+        54: [3345, 4053, 4123, 5256, 6167, 6230, 7623, 7655, 8824],
         262: [7262],
+        283: [3283],
         341: [667, 2206],
-        342: [3342],
         602: [4602],
-        644: [7638, 7664, 7714, 8859],
-        813: [492, 1381, 1595, 4796, 8626, 9221]
+        813: [207, 4796, 8215, 9169, 9265, 9943],
+        820: [921, 2126, 2844, 8440]
     }, k = {}, x.f.consumes = (e, r) => {
         x.o(S, e) && S[e].forEach((e => {
             if (x.o(w, e)) return r.push(w[e]);
             if (!k[e]) {
                 var t = r => {
                     w[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
@@ -324,35 +324,35 @@
         var e = {
             490: 0
         };
         x.f.j = (r, t) => {
             var a = x.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^((26|34|60)2|644)$/.test(r)) e[r] = 0;
+                else if (/^(262|283|602|820)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = x.p + x.u(r),
-                    d = new Error;
+                    f = new Error;
                 x.l(n, (t => {
                     if (x.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             n = t && t.target && t.target.src;
-                        d.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", d.name = "ChunkLoadError", d.type = o, d.request = n, a[1](d)
+                        f.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", f.name = "ChunkLoadError", f.type = o, f.request = n, a[1](f)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, d, f] = t,
+                var a, o, [n, f, d] = t,
                     l = 0;
                 if (n.some((r => 0 !== e[r]))) {
-                    for (a in d) x.o(d, a) && (x.m[a] = d[a]);
-                    f && f(x)
+                    for (a in f) x.o(f, a) && (x.m[a] = f[a]);
+                    d && d(x)
                 }
                 for (r && r(t); l < n.length; l++) o = n[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
     var T = x(2401);
```

### Comparing `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/third-party-licenses.json` & `jupytercad_core-2.0.0a7/jupytercad_core/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959239130434783%*

 * *Differences: {"'packages'": "{5: {'versionInfo': '2.0.0-alpha.7'}, 6: {'versionInfo': '2.0.0-alpha.7'}, 7: "*

 * *               "{'versionInfo': '2.0.0-alpha.7'}}"}*

```diff
@@ -30,27 +30,27 @@
             "name": "@emotion/unitless",
             "versionInfo": "0.7.5"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/base",
-            "versionInfo": "2.0.0-alpha.6"
+            "versionInfo": "2.0.0-alpha.7"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/occ-worker",
-            "versionInfo": "2.0.0-alpha.6"
+            "versionInfo": "2.0.0-alpha.7"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/schema",
-            "versionInfo": "2.0.0-alpha.6"
+            "versionInfo": "2.0.0-alpha.7"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/rendermime",
             "versionInfo": "3.6.7"
         },
```

### Comparing `jupytercad_core-2.0.0a6/lib/factory.d.ts` & `jupytercad_core-2.0.0a7/lib/factory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/factory.js` & `jupytercad_core-2.0.0a7/lib/factory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/index.d.ts` & `jupytercad_core-2.0.0a7/lib/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/index.js` & `jupytercad_core-2.0.0a7/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/plugin.d.ts` & `jupytercad_core-2.0.0a7/lib/plugin.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/plugin.js` & `jupytercad_core-2.0.0a7/lib/plugin.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/schemaregistry.js` & `jupytercad_core-2.0.0a7/lib/schemaregistry.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/workerregistry.js` & `jupytercad_core-2.0.0a7/lib/workerregistry.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a7/lib/jcadplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.js` & `jupytercad_core-2.0.0a7/lib/jcadplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.js` & `jupytercad_core-2.0.0a7/lib/jcadplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stepplugin/model.d.ts` & `jupytercad_core-2.0.0a7/lib/stepplugin/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stepplugin/model.js` & `jupytercad_core-2.0.0a7/lib/stepplugin/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a7/lib/stepplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.js` & `jupytercad_core-2.0.0a7/lib/stepplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stepplugin/plugins.js` & `jupytercad_core-2.0.0a7/lib/stepplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stlplugin/model.js` & `jupytercad_core-2.0.0a7/lib/stlplugin/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a7/lib/stlplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.js` & `jupytercad_core-2.0.0a7/lib/stlplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/lib/stlplugin/plugins.js` & `jupytercad_core-2.0.0a7/lib/stlplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/factory.ts` & `jupytercad_core-2.0.0a7/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/index.ts` & `jupytercad_core-2.0.0a7/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/plugin.ts` & `jupytercad_core-2.0.0a7/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/schemaregistry.ts` & `jupytercad_core-2.0.0a7/src/schemaregistry.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/workerregistry.ts` & `jupytercad_core-2.0.0a7/src/workerregistry.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/jcadplugin/modelfactory.ts` & `jupytercad_core-2.0.0a7/src/jcadplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/jcadplugin/plugins.ts` & `jupytercad_core-2.0.0a7/src/jcadplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stepplugin/model.ts` & `jupytercad_core-2.0.0a7/src/stepplugin/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stepplugin/modelfactory.ts` & `jupytercad_core-2.0.0a7/src/stepplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stepplugin/plugins.ts` & `jupytercad_core-2.0.0a7/src/stepplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stlplugin/model.ts` & `jupytercad_core-2.0.0a7/src/stlplugin/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stlplugin/modelfactory.ts` & `jupytercad_core-2.0.0a7/src/stlplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/src/stlplugin/plugins.ts` & `jupytercad_core-2.0.0a7/src/stlplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/LICENSE` & `jupytercad_core-2.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/pyproject.toml` & `jupytercad_core-2.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a6/PKG-INFO` & `jupytercad_core-2.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupytercad_core
-Version: 2.0.0a6
+Version: 2.0.0a7
 Dynamic: Keywords
 Summary: JupyterCad core extension
 Project-URL: Homepage, https://github.com/jupytercad/jupytercad
 Project-URL: Bug Tracker, https://github.com/jupytercad/jupytercad/issues
 Project-URL: Repository, https://github.com/jupytercad/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
```

