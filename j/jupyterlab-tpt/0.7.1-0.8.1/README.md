# Comparing `tmp/jupyterlab_tpt-0.7.1.tar.gz` & `tmp/jupyterlab_tpt-0.8.1.tar.gz`

## Comparing `jupyterlab_tpt-0.7.1.tar` & `jupyterlab_tpt-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,121 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.eslintrc.js
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.yarnrc.yml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/RELEASE.md
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/install.json
--rw-r--r--   0        0        0   286693 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/package-lock.json
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/package.json
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/package.json.version
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/tsconfig.json
--rw-r--r--   0        0        0   214158 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/yarn.lock
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/examples/hide-input-tools-sample.ipynb
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/examples/other.ipynb
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/_version.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/package.json
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/package.json.orig
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/plugin.json
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/static/212.5290a49a4f1c8e7e24ec.js
--rw-r--r--   0        0        0    13440 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/static/747.4a150ad472d8faa3ea9c.js
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/static/remoteEntry.92eb673846343e76aafe.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/static/style.js
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/schema/plugin.json
--rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/src/index.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/src/typings.d.ts
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/base.css
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/in-and-out.svg
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/index.js
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/noin-noout.svg
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/only-in.svg
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/only-out.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/style/selected_cells.raw.css
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/LICENSE
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/README.md
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.eslintrc.js
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.yarnrc.yml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/RELEASE.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/install.json
+-rw-r--r--   0        0        0   286693 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/package-lock.json
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/package.json
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/package.json.version
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/tsconfig.json
+-rw-r--r--   0        0        0   214158 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/yarn.lock
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/examples/hide-input-tools-sample.ipynb
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/examples/other.ipynb
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/_version.py
+-rw-r--r--   0        0        0    20636 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/build_log.json
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/package.json
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/package.json.orig
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/plugin.json
+-rw-r--r--   0        0        0    20967 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.0009a08f722eea530ae5.js
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.0009a08f722eea530ae5.js.map
+-rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.03aaec581826f0287335.js
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.03aaec581826f0287335.js.map
+-rw-r--r--   0        0        0    22721 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.07236439b2ffe2f690e0.js
+-rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.07236439b2ffe2f690e0.js.map
+-rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.09e47d9ef4a193563383.js
+-rw-r--r--   0        0        0    18812 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.09e47d9ef4a193563383.js.map
+-rw-r--r--   0        0        0    23310 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.1b816c6c8127be1e7392.js
+-rw-r--r--   0        0        0    21564 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.1b816c6c8127be1e7392.js.map
+-rw-r--r--   0        0        0    22671 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.1e47496410d8231287bd.js
+-rw-r--r--   0        0        0    20726 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.1e47496410d8231287bd.js.map
+-rw-r--r--   0        0        0    18457 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.326c3cd8a1379a61b017.js
+-rw-r--r--   0        0        0    16488 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.326c3cd8a1379a61b017.js.map
+-rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.348ff4b0bd4132e48d95.js
+-rw-r--r--   0        0        0    16514 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.348ff4b0bd4132e48d95.js.map
+-rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4bc07777a9b2fca832f2.js
+-rw-r--r--   0        0        0    18799 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4bc07777a9b2fca832f2.js.map
+-rw-r--r--   0        0        0    18457 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4ceee5cc1c43b2ae02fc.js
+-rw-r--r--   0        0        0    22105 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4ceee5cc1c43b2ae02fc.js.map
+-rw-r--r--   0        0        0    21155 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4fd10138bfe2b80c848a.js
+-rw-r--r--   0        0        0    18930 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.4fd10138bfe2b80c848a.js.map
+-rw-r--r--   0        0        0    22661 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5a188703ea7a2e4d852b.js
+-rw-r--r--   0        0        0    20716 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5a188703ea7a2e4d852b.js.map
+-rw-r--r--   0        0        0    21197 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5bbf168543ab9c2d29d8.js
+-rw-r--r--   0        0        0    18978 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5bbf168543ab9c2d29d8.js.map
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5d232dbff97797e29400.js
+-rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.5d232dbff97797e29400.js.map
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.645424d5e78ee7dee6f0.js
+-rw-r--r--   0        0        0    20795 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.645424d5e78ee7dee6f0.js.map
+-rw-r--r--   0        0        0    20980 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.64a3f7c8673440598d2e.js
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.64a3f7c8673440598d2e.js.map
+-rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.939c3ab2832857ac4f8c.js
+-rw-r--r--   0        0        0    20716 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.939c3ab2832857ac4f8c.js.map
+-rw-r--r--   0        0        0    23311 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.9d14caef482b68e7ce93.js
+-rw-r--r--   0        0        0    21565 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.9d14caef482b68e7ce93.js.map
+-rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.9e2ca03f5043f0380753.js
+-rw-r--r--   0        0        0    18877 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.9e2ca03f5043f0380753.js.map
+-rw-r--r--   0        0        0    21001 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.a2abef896db477e58e5b.js
+-rw-r--r--   0        0        0    18829 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.a2abef896db477e58e5b.js.map
+-rw-r--r--   0        0        0    21112 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.af3eab0bef5cb8f6d195.js
+-rw-r--r--   0        0        0    18887 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.af3eab0bef5cb8f6d195.js.map
+-rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.afa52f9a55ced9470ba1.js
+-rw-r--r--   0        0        0    18974 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.afa52f9a55ced9470ba1.js.map
+-rw-r--r--   0        0        0    20988 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.e4f8b6c93109dce2bb8a.js
+-rw-r--r--   0        0        0    18816 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.e4f8b6c93109dce2bb8a.js.map
+-rw-r--r--   0        0        0    22714 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.e9c62e18d8bbf1fde5d3.js
+-rw-r--r--   0        0        0    20775 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.e9c62e18d8bbf1fde5d3.js.map
+-rw-r--r--   0        0        0    22662 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.fb5edbda274d22f4b6ae.js
+-rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/lib_index_js.fb5edbda274d22f4b6ae.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.0f6b1acc529389df0e29.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.117917267e9dc4768c99.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.1d65fb92913d2f305005.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.1fc22ed05d5153107b98.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.36b2fabe644a125e4b89.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.60046f43c5f0ba525fbf.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.62603b5bd5e7078b30b0.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.66c285c2f9fd173b5a2f.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.6c2f160e8e278bfea4b5.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.71dd0bc77ca06bb1d2ae.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.72cbd137b532c53f90d7.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.72f48b0d9dbb0f88982d.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.91b86b7493cab39b31ff.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.9bcfa5ffdbf9b5dec221.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.aff80c9cd025b1bcb9c2.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.b32df1047c15002fd402.js.map
+-rw-r--r--   0        0        0    28648 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.bc695d4e6ba3c0db17ad.js
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.bc695d4e6ba3c0db17ad.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.bdf3274fae45527d415c.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.c868f9947f788d4adb2b.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.de186274bc5935f2c5f7.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.e72cb20f55cca222f096.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.e91daff55aeff9f064ac.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.e97c16e1394219d24cc1.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.edf5d05c90933a7ff22f.js.map
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/remoteEntry.fdb08670a982a4691518.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/style.js
+-rw-r--r--   0        0        0    32024 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/style_index_js.34866469fc6eb683d344.js
+-rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/style_index_js.34866469fc6eb683d344.js.map
+-rw-r--r--   0        0        0    19099 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_apply_on_cells_js-node_modules_jupyterlab-24da5e.240fe473b8815e22d088.js
+-rw-r--r--   0        0        0    18753 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_apply_on_cells_js-node_modules_jupyterlab-24da5e.240fe473b8815e22d088.js.map
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/schema/plugin.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/src/admonitions.ts
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/src/index.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/src/typings.d.ts
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/base.css
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/in-and-out.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/index.js
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/noin-noout.svg
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/only-in.svg
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/only-out.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/style/selected_cells.raw.css
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/README.md
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 jupyterlab_tpt-0.8.1/PKG-INFO
```

### Comparing `jupyterlab_tpt-0.7.1/.eslintrc.js` & `jupyterlab_tpt-0.8.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/RELEASE.md` & `jupyterlab_tpt-0.8.1/RELEASE.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 - Go to the Actions panel
 - Run the "Step 1: Prep Release" workflow
 - Check the draft changelog
 - Run the "Step 2: Publish Release" workflow
 
 ## Publishing to `conda-forge`
 
-If the package is not on conda forge yet, check the documentation to learn how to add it: https://conda-forge.org/docs/maintainer/adding_pkgs.html
+If the package is not on conda forge yet, check the documentation to learn how to add it: <https://conda-forge.org/docs/maintainer/adding_pkgs.html>
 
 Otherwise a bot should pick up the new version publish to PyPI, and open a new PR on the feedstock repository automatically.
```

### Comparing `jupyterlab_tpt-0.7.1/package-lock.json` & `jupyterlab_tpt-0.8.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/package.json` & `jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/package.json.version` & `jupyterlab_tpt-0.8.1/package.json.version`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/tsconfig.json` & `jupyterlab_tpt-0.8.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/yarn.lock` & `jupyterlab_tpt-0.8.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/examples/hide-input-tools-sample.ipynb` & `jupyterlab_tpt-0.8.1/examples/hide-input-tools-sample.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/examples/other.ipynb` & `jupyterlab_tpt-0.8.1/examples/other.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9296875%*

 * *Differences: {"'cells'": "{0: {'source': ['````{error}\\n', '\\n', '````']}, insert: [(1, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'96389af6-d3ba-4b9d-ae8d-2abe6c17e62b'), ('metadata', OrderedDict()), ('source', "*

 * *            "['some text \\n', '### solution\\n', '\\n', '````{admonition} ouvrez-moi\\n', "*

 * *            "':class: dropdown\\n', '\\n', '```{literalinclude} xxx.py\\n', '```\\n', '\\n', "*

 * *            "'````\\n', 'already'])]))]}"}*

```diff
@@ -6,15 +6,37 @@
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
-            "source": []
+            "source": [
+                "````{error}\n",
+                "\n",
+                "````"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "96389af6-d3ba-4b9d-ae8d-2abe6c17e62b",
+            "metadata": {},
+            "source": [
+                "some text \n",
+                "### solution\n",
+                "\n",
+                "````{admonition} ouvrez-moi\n",
+                ":class: dropdown\n",
+                "\n",
+                "```{literalinclude} xxx.py\n",
+                "```\n",
+                "\n",
+                "````\n",
+                "already"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/package.json` & `jupyterlab_tpt-0.8.1/jupyterlab_tpt/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.bc695d4e6ba3c0db17ad.js'}}",*

 * * "'version'": "'0.7.1'"}*

```diff
@@ -46,15 +46,15 @@
         "style/index.js",
         "schema/*.json"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-tpt",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.92eb673846343e76aafe.js",
+            "load": "static/remoteEntry.bc695d4e6ba3c0db17ad.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_tpt/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.7.1"
 }
```

### Comparing `jupyterlab_tpt-0.7.1/jupyterlab_tpt/labextension/schemas/jupyterlab-tpt/package.json.orig` & `jupyterlab_tpt-0.8.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.8.1'"}*

```diff
@@ -96,9 +96,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.8.1"
 }
```

### Comparing `jupyterlab_tpt-0.7.1/src/index.ts` & `jupyterlab_tpt-0.8.1/src/index.ts`

 * *Files 18% similar despite different names*

```diff
@@ -16,28 +16,56 @@
 } from '@jupyterlab/notebook'
 
 import { CodeCell, MarkdownCell, Cell } from '@jupyterlab/cells'
 
 // md_clean may be broken
 import {
   md_get,
+  md_unset,
   md_insert,
-  md_remove
+  md_remove,
 } from 'jupyterlab-celltagsclasses'
+
 import { ISettingRegistry } from '@jupyterlab/settingregistry'
 
 import { Scope, apply_on_cells } from 'jupyterlab-celltagsclasses'
 
 import selectedCellsCss from '../style/selected_cells.raw.css'
 
+import { toggle_admonition, insert_solution } from './admonitions'
+
 const PLUGIN_ID = 'jupyterlab-tpt:plugin'
 
-// regarding hide-input, forget about the nbclassic behaviour
-// we will just run once hideinput-to-hidecell
-// and be done with it
+// metadata
+// md_clean may be broken
+// import { md_set, , md_insert, md_remove } from 'jupyterlab-celltagsclasses'
+
+const clean_cell_metadata = (cell: Cell) => {
+  console.log('Cleaning metadata for cell', cell)
+  const editable = cell.model.getMetadata('editable')
+  if (editable === true) {
+    md_unset(cell, 'editable')
+  }
+  const tags = cell.model.getMetadata('tags')
+  if (tags?.length === 0) {
+    md_unset(cell, 'tags')
+  }
+  const slide_type = md_get(cell, 'slideshow.slide_type')
+  if (slide_type === '') {
+    md_unset(cell, 'slideshow.slide_type')
+  }
+  const slideshow = md_get(cell, 'slideshow')
+  if (slideshow !== undefined && JSON.stringify(slideshow) === '{}') {
+    md_unset(cell, 'slideshow')
+  }
+  const user_expressions = md_get(cell, 'user_expressions')
+  if (user_expressions?.length === 0) {
+    md_unset(cell, 'user_expressions')
+  }
+}
 
 // cells that have this in their code
 const NEEDLE = 'tools.sample_from'
 
 const set_remove_input_needle = (cell: Cell, hidden: boolean) => {
   // ignore text cells
   if (cell instanceof CodeCell) {
@@ -82,14 +110,15 @@
 const toggle_tag = (cell: Cell, tag: string) => {
   if (md_get(cell, 'tags', tag)) {
     md_remove(cell, 'tags', tag)
   } else {
     md_insert(cell, 'tags', tag)
   }
 }
+
 /**
  * Initialization data for the jupyterlab-tpt extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab-tpt:plugin',
   autoStart: true,
   requires: [ICommandPalette, INotebookTracker, ISettingRegistry],
@@ -116,14 +145,40 @@
     // Cmd modifier is ignored on non-Mac platforms.
     // Alt is option on mac
 
     let [outline_selected_cells] = [false]
 
     let command
 
+    command = 'metadata:clean-selected'
+    app.commands.addCommand(command, {
+      label: 'clean metadata for all selected cells',
+      execute: () =>
+        apply_on_cells(notebookTracker, Scope.Multiple, clean_cell_metadata)
+    })
+    palette.addItem({ command, category: 'metadata' })
+    app.commands.addKeyBinding({
+      command,
+      keys: ['Alt Cmd 7'],
+      selector: '.jp-Notebook'
+    })
+
+    command = 'metadata:clean-all'
+    app.commands.addCommand(command, {
+      label: 'clean metadata for all cells',
+      execute: () =>
+        apply_on_cells(notebookTracker, Scope.All, clean_cell_metadata)
+    })
+    palette.addItem({ command, category: 'metadata' })
+    app.commands.addKeyBinding({
+      command,
+      keys: ['Ctrl Alt 7'],
+      selector: '.jp-Notebook'
+    })
+
     // Option-Command-9 = toggle (hide-input) on all selected cells
     // Ctrl-Alt-9 = show (wrt hide-input) on all selected cells
     command = 'convenience:show-settings'
     app.commands.addCommand(command, {
       label: 'show settings',
       execute: () =>
         console.log(
@@ -186,15 +241,15 @@
 
     // render-all-cells - unrender-all-cells (markdown actually)
 
     const unrender_markdown = (cell: Cell) => {
       if (cell.model.type !== 'markdown') {
         return
       }
-      ;(cell as MarkdownCell).rendered = false
+      (cell as MarkdownCell).rendered = false
     }
     command = 'notebook:unrender-all-markdown'
     app.commands.addCommand(command, {
       label: 'unrender all markdown cells',
       execute: () =>
         apply_on_cells(notebookTracker, Scope.All, unrender_markdown)
     })
@@ -276,14 +331,77 @@
         }
         inject_css(selectedCellsCss, id)
       } else {
         console.log('removing css for outlining selection')
         present?.remove()
       }
     }
+
+    // admonitions
+    for (const [name, key] of [
+      ['admonition', 'Ctrl A'],
+      ['tip', 'Ctrl T'],
+      ['note', 'Ctrl N'],
+      ['attention', null],
+      ['caution', null],
+      ['danger', null],
+      ['error', null],
+      ['hint', null],
+      ['important', null],
+      ['seealso', null],
+      ['warning', null]
+    ]) {
+      // need to cast because name is typed as string | null ?!?
+      const admonition = name as string
+      command = 'admonition:toggle'
+      let label = 'toggle admonition'
+      if (admonition !== 'admonition') {
+        command += `-${admonition}`
+        label += ` ${admonition}`
+      }
+      app.commands.addCommand(command, {
+        label,
+        execute: () => {
+          const notebook = notebookTracker.currentWidget?.content
+          if (notebook === undefined) {
+            return
+          }
+          toggle_admonition(notebook, admonition)
+        }
+      })
+      palette.addItem({ command, category: 'admonition' })
+      if (key !== null) {
+        app.commands.addKeyBinding({
+          command,
+          keys: ['Ctrl \\', key],
+          selector: '.jp-Notebook'
+        })
+      }
+    }
+
+    // solution
+    command = 'admonition:insert-solution'
+    app.commands.addCommand(command, {
+      label: 'insert a solution block at cursor location',
+      execute: () => {
+        const notebook = notebookTracker.currentWidget?.content
+        if (notebook === undefined) {
+          return
+        }
+        insert_solution(notebook, 'ouvrez-moi', 'xxx.py')
+      }
+    })
+    palette.addItem({ command, category: 'convenience' })
+    app.commands.addKeyBinding({
+      command,
+      keys: ['Ctrl \\', 'Ctrl S'],
+      selector: '.jp-Notebook'
+    })
+
+
     function loadSetting(setting: ISettingRegistry.ISettings): void {
       // Read the settings and convert to the correct type
       outline_selected_cells = setting.get('outline_selected_cells')
         .composite as boolean
 
       console.log(
         `tpt extension, outline_selected is read as ${outline_selected_cells}`
```

### Comparing `jupyterlab_tpt-0.7.1/style/base.css` & `jupyterlab_tpt-0.8.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/style/in-and-out.svg` & `jupyterlab_tpt-0.8.1/style/in-and-out.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/style/noin-noout.svg` & `jupyterlab_tpt-0.8.1/style/noin-noout.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/style/only-in.svg` & `jupyterlab_tpt-0.8.1/style/only-in.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/style/only-out.svg` & `jupyterlab_tpt-0.8.1/style/only-out.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/.gitignore` & `jupyterlab_tpt-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/LICENSE` & `jupyterlab_tpt-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/pyproject.toml` & `jupyterlab_tpt-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_tpt-0.7.1/PKG-INFO` & `jupyterlab_tpt-0.8.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_tpt
-Version: 0.7.1
+Version: 0.8.1
+Dynamic: Keywords
 Summary: My custom tweaks for using JLAB
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-tpt
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-tpt/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-tpt.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
         
@@ -53,15 +54,16 @@
 Requires-Dist: jupyterlab-gridwidth
 Requires-Dist: jupyterlab-hidecell
 Description-Content-Type: text/markdown
 
 # jupyterlab_tpt
 
 [![Github Actions Status](https://github.com/parmentelat/jupyterlab-tpt/workflows/Build/badge.svg)](https://github.com/parmentelat/jupyterlab-tpt/actions/workflows/build.yml)
-My custom tweaks for using JLAB
+
+My custom tweaks for using JLAB; something that would have gone into a `custom.js` in nb classic...
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 - jupyterlab-myst
 
 ## Install
@@ -80,14 +82,30 @@
 pip uninstall jupyterlab_tpt
 ```
 
 ## misc commands and keystrokes
 
 search for `convenience` in the command palette to see the list of commands and associated keystrokes
 
+as well as for adding/removing an admonition around a cell
+
+|                command                |   keybinding    |
+| :-----------------------------------: | :-------------: |
+| `admonition:toggle`                   | `Ctrl-\ Ctrl-A` |
+| `admonition:toggle-tip`               | `Ctrl-\ Ctrl-T` |
+| `admonition:toggle-note`              | `Ctrl-\ Ctrl-N` |
+| `admonition:toggle-attention`         |                 |
+| `admonition:toggle-caution`           |                 |
+| `admonition:toggle-danger`            |                 |
+| `admonition:toggle-error`             |                 |
+| `admonition:toggle-hint`              |                 |
+| `admonition:toggle-important`         |                 |
+| `admonition:toggle-seealso`           |                 |
+| `admonition:toggle-warning`           |                 |
+
 ## Development
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
@@ -132,23 +150,24 @@
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab-tpt` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
 
-# My notes
+## My notes
 
 - on using signals
   <https://github.com/jupyterlab/extension-examples/tree/master/signals>
 
 - a very useful example of arming callbacks on changes
-  // https://discourse.jupyter.org/t/how-to-get-output-model-for-a-given-cell-in-a-jupyterlab-extension/11342/6
+  <https://discourse.jupyter.org/t/how-to-get-output-model-for-a-given-cell-in-a-jupyterlab-extension/11342/6>
 
 - waiting for a notebook context to be ready
+
   ```js
   notebookContext: DocumentRegistry.IContext<INotebookModel>
   notebookContext.ready.then(() => {
     /*
      * The order of operations here is key. First, create a model that contains a log of
      * executed cells and the state of the gather UI.
      */
```

