# Comparing `tmp/jupyterlab_sql_explorer-0.1.2.tar.gz` & `tmp/jupyterlab_sql_explorer-0.2.0.tar.gz`

## Comparing `jupyterlab_sql_explorer-0.1.2.tar` & `jupyterlab_sql_explorer-0.2.0.tar`

### file list

```diff
@@ -1,110 +1,156 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/babel.config.js
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/conftest.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jest.config.js
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/package.json
--rw-r--r--   0        0        0   773102 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/preview.gif
--rw-r--r--   0        0        0   138490 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/screenshot.png
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/setup.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   388443 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/yarn.lock
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyter-config/nb-config/jupyterlab-sql-explorer.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyter-config/server-config/jupyterlab-sql-explorer.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/_version.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/comments.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/comments_db.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/const.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/db.py
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/engine.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/handlers.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/serializer.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/task.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/package.json
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/schemas/jupyterlab-sql-explorer/package.json.orig
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/schemas/jupyterlab-sql-explorer/plugin.json
--rw-r--r--   0        0        0    99543 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/107.ee10f805fff4dde9d5ef.js
--rw-r--r--   0        0        0   132863 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/421.29ff64b727e84f4eba9f.js
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/747.a9c2a859ed290bac4c6f.js
--rw-r--r--   0        0        0    24911 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/810.dab59af361bdd56dcaff.js
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/946.4b29558dafd5a7db52a7.js
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/remoteEntry.5d0a100c5f87bad68bb4.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/style.js
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/__init__.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_comments.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_handlers.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_mysql.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_sqlite.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_utils.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/schema/plugin.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/JpServices.ts
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/SqlWidget.tsx
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/cmd_menu.ts
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/handler.ts
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/icons.ts
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/index.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/interfaces.ts
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/model.ts
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/react-window.d.ts
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/resize-observer.d.ts
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/svg.d.ts
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/__tests__/model.spec.ts
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/auto_resizer/AutoSizer.ts
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/auto_resizer/index.ts
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/auto_resizer/types.ts
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/ActionBtn.tsx
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/ask_pass.tsx
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/collist.tsx
--rw-r--r--   0        0        0    17638 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/dblist.tsx
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/loading.tsx
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/new_conn.tsx
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/sqlPanel.tsx
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/components/styles.ts
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/ResultsTable.ts
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/Table.ts
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/console.ts
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/editor.ts
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/index.ts
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/src/sqlConsole/toolbar.tsx
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/index.js
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/column.svg
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/conn-add.svg
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/conn.svg
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/delete.svg
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/error.svg
--rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/hive-1.svg
--rw-r--r--   0        0        0    19243 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/hive-2.svg
--rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/hive.svg
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/mysql.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/oracle.svg
--rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/pgsql-1.svg
--rw-r--r--   0        0        0    12659 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/pgsql-3.svg
--rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/pgsql.svg
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/query.svg
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/root.svg
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/sql.svg
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/sql_script.svg
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/sqlite.svg
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/table-2.svg
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/table-3.svg
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/table.svg
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/view.svg
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/view1.svg
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/view2.svg
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/style/icons/view3.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/ui-tests/tests/jupyterlab-sql-explorer.spec.ts
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/LICENSE
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/README.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/babel.config.js
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/conftest.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/install.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jest.config.js
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/package.json
+-rw-r--r--   0        0        0   773102 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/preview.gif
+-rw-r--r--   0        0        0   138490 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/screenshot.png
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/setup.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/tsconfig.test.json
+-rw-r--r--   0        0        0   379202 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/yarn.lock
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/.copier-answers.yml
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/.gitignore
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/CHANGELOG.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/LICENSE
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/README.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/babel.config.js
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/conftest.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jest.config.js
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/package.json
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/pyproject.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/tsconfig.test.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jupyter-config/server-config/jupyterlab-sql-explorer.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jupyterlab-sql-explorer/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jupyterlab-sql-explorer/handlers.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jupyterlab-sql-explorer/tests/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/jupyterlab-sql-explorer/tests/test_handlers.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/schema/plugin.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/src/handler.ts
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/src/index.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/src/__tests__/jupyterlab-sql-explorer.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/tests/jupyterlab-sql-explorer.spec.ts
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyter-config/nb-config/jupyterlab-sql-explorer.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyter-config/server-config/jupyterlab-sql-explorer.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/_version.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/comments.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/comments_db.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/const.py
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/db.py
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/engine.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/handlers.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/serializer.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/task.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/build_log.json
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/package.json
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/schemas/jupyterlab-sql-explorer/package.json.orig
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/schemas/jupyterlab-sql-explorer/plugin.json
+-rw-r--r--   0        0        0   206809 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/lib_index_js.f775090c89d3b6510a9e.js
+-rw-r--r--   0        0        0   191524 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/lib_index_js.f775090c89d3b6510a9e.js.map
+-rw-r--r--   0        0        0    35828 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/remoteEntry.a6ec51bb86feab5ddc79.js
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/remoteEntry.a6ec51bb86feab5ddc79.js.map
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/style.js
+-rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/style_index_js.d824c71eae6b0e7a7d22.js
+-rw-r--r--   0        0        0    14824 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/style_index_js.d824c71eae6b0e7a7d22.js.map
+-rw-r--r--   0        0        0   407759 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.fc9283ed3b94944ba427.js
+-rw-r--r--   0        0        0   721277 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_lumino_datagrid_dist_index_es6_js.fc9283ed3b94944ba427.js.map
+-rw-r--r--   0        0        0    92074 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_react-window_dist_index_esm_js.16df7828f1198bc71f10.js
+-rw-r--r--   0        0        0   161942 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_react-window_dist_index_esm_js.16df7828f1198bc71f10.js.map
+-rw-r--r--   0        0        0    32665 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_typestyle_lib_es2015_index_js.a39ac557450da534a11c.js
+-rw-r--r--   0        0        0    43622 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/static/vendors-node_modules_typestyle_lib_es2015_index_js.a39ac557450da534a11c.js.map
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/t_mysql.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_comments.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_handlers.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_sqlite.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_utils.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/schema/plugin.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/JpServices.ts
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/SqlWidget.tsx
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/Untitled.ipynb
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/cmd_menu.ts
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/handler.ts
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/icons.ts
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/index.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/interfaces.ts
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/model.ts
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/react-window.d.ts
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/svg.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/__tests__/jupyterlab-sql-explorer.spec.ts
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/__tests__/model.spec.ts
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/auto_resizer/AutoSizer.ts
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/auto_resizer/index.ts
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/auto_resizer/types.ts
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/ActionBtn.tsx
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/ask_pass.tsx
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/collist.tsx
+-rw-r--r--   0        0        0    17638 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/dblist.tsx
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/loading.tsx
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/new_conn.tsx
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/sqlPanel.tsx
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/components/styles.ts
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/ResultsTable.ts
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/Table.ts
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/console.ts
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/editor.ts
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/index.ts
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/src/sqlConsole/toolbar.tsx
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/index.js
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/column.svg
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/conn-add.svg
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/conn.svg
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/delete.svg
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/error.svg
+-rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/hive-1.svg
+-rw-r--r--   0        0        0    19243 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/hive-2.svg
+-rw-r--r--   0        0        0    16307 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/hive.svg
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/mysql.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/oracle.svg
+-rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/pgsql-1.svg
+-rw-r--r--   0        0        0    12659 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/pgsql-3.svg
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/pgsql.svg
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/query.svg
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/root.svg
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/sql.svg
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/sql_script.svg
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/sqlite.svg
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/table-2.svg
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/table-3.svg
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/table.svg
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/view.svg
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/view1.svg
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/view2.svg
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/style/icons/view3.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/ui-tests/tests/jupyterlab-sql-explorer.spec.ts
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9924 2020-02-02 00:00:00.000000 jupyterlab_sql_explorer-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_sql_explorer-0.1.2/package.json` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8982666666666667%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.1.6', '@jupyterlab/coreutils': '^6.1.6', "*

 * *                   "'@jupyterlab/mainmenu': '^4.1.6', '@jupyterlab/services': '^7.1.6', "*

 * *                   "'@jupyterlab/settingregistry': '^4.1.6', '@lumino/datagrid': '^2.3.0-alpha.0', "*

 * *                   "'@lumino/commands': '^2.3.0', '@lumino/widgets': '^2.3.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@jupyterlab/testutils': '^4.0.0', "*

 * *                      "'@types/jest': '^29.2.0', '@ […]*

```diff
@@ -2,47 +2,57 @@
     "author": {
         "name": "groupnotes"
     },
     "bugs": {
         "url": "https://github.com/groupnotes/jupyterlab-sql-explorer/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
-        "@lumino/datagrid": "0.36.7",
+        "@jupyterlab/application": "^4.1.6",
+        "@jupyterlab/coreutils": "^6.1.6",
+        "@jupyterlab/mainmenu": "^4.1.6",
+        "@jupyterlab/services": "^7.1.6",
+        "@jupyterlab/settingregistry": "^4.1.6",
+        "@lumino/commands": "^2.3.0",
+        "@lumino/datagrid": "^2.3.0-alpha.0",
+        "@lumino/widgets": "^2.3.2",
         "react-virtualized-auto-sizer": "^1.0.20",
         "react-window": "^1.8.9"
     },
     "description": "A JupyterLab extension for Database",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
-        "typescript": "~4.1.3"
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "ts-jest": "^29.1.2",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
             "plugin:prettier/recommended"
@@ -102,18 +112,24 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/groupnotes/jupyterlab-sql-explorer",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.a6ec51bb86feab5ddc79.js",
+            "style": "./style"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_sql_explorer"
                 },
                 "managers": [
                     "pip"
@@ -159,28 +175,32 @@
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-explorer",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/groupnotes/jupyterlab-sql-explorer.git"
     },
-    "resolutions": {
-        "@lumino/coreutils": "^1.11.0",
-        "@lumino/widgets": "^1.37.2"
-    },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
@@ -198,30 +218,35 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/preview.gif` & `jupyterlab_sql_explorer-0.2.0/preview.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/screenshot.png` & `jupyterlab_sql_explorer-0.2.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/tsconfig.json` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/tsconfig.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.725%*

 * *Differences: {"'compilerOptions'": "{delete: ['lib', 'types']}", "'include'": "['src/*']"}*

```diff
@@ -2,31 +2,24 @@
     "compilerOptions": {
         "allowSyntheticDefaultImports": true,
         "composite": true,
         "declaration": true,
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
-        "lib": [
-            "DOM",
-            "ESnext"
-        ],
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "ES2018",
-        "types": [
-            "jest"
-        ]
+        "target": "ES2018"
     },
     "include": [
-        "src/**/*"
+        "src/*"
     ]
 }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/__init__.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/comments.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/comments.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/comments_db.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/comments_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import create_engine, Column, Integer, String, Index, text, Sequence
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker, declarative_base
+#from sqlalchemy.ext.declarative import declarative_base
 
 C_CONN = 1
 C_SCHEMA = 2
 C_TABLE = 3
 C_COLUMN = 4
 
 _conn_str=None
@@ -16,108 +16,113 @@
 class Comments(Base):
     __tablename__ = 'comments'
 
     id = Column(Integer, comments_sequence, primary_key=True)
     type = Column(Integer)
     dbid = Column(String(20))
     schema = Column(String(100))
-    table = Column(String(100))
-    column = Column(String(100))
-    comment = Column(String(500))
+    tabname = Column(String(100))
+    colname = Column(String(100))
+    memo = Column(String(500))
 
-    index_name = Index('idx', type, dbid, schema, column)
+    index_name = Index('idx', type, dbid, schema, tabname, colname)
 
 def init(conn_str: str):
     global _conn_str
     _conn_str= conn_str
     engine = create_engine(conn_str)
     Base.metadata.create_all(engine)
 
 def get_conn_comments():
     try:
         engine = create_engine(_conn_str)
-        result = engine.execute(text('''
-        SELECT `dbid`, `comment` FROM comments 
-        WHERE id in ( SELECT max(id) as id FROM comments
-                    WHERE `type` = :type
-                    GROUP BY `dbid` )
-        '''), type=str(C_CONN))
-        data={}
-        for r in result.fetchall():
-            data[r[0]]=r[1]
-        return data
+        with engine.connect() as conn:
+            result = conn.execute(text('''
+            SELECT dbid, memo FROM comments 
+            WHERE id in ( SELECT max(id) as id FROM comments
+                    WHERE type = :type
+                    GROUP BY dbid )
+            '''), {"type":str(C_CONN)})
+            data={}
+            for r in result.fetchall():
+                data[r[0]]=r[1]
+            return data
     except Exception:
         return {}
 
 def get_schema_comments(dbid: str):
     try:
         engine = create_engine(_conn_str)
-        result = engine.execute(text('''
-        SELECT `schema`, `comment` FROM comments
-        WHERE id in ( SELECT max(id) as id FROM comments
-                    WHERE `type` = :type and `dbid` = :dbid
-                    GROUP BY `schema` )
-        '''), type=str(C_SCHEMA), dbid=dbid)
-        data={}
-        for r in result.fetchall():
-            data[r[0]]=r[1]
-        return data
+        with engine.connect() as conn:
+            result = conn.execute(text('''
+            SELECT schema, memo FROM comments
+            WHERE id in ( SELECT max(id) as id FROM comments
+                        WHERE type = :type and dbid = :dbid
+                        GROUP BY schema )
+            '''), {'type':str(C_SCHEMA), 'dbid':dbid})
+            data={}
+            for r in result.fetchall():
+                data[r[0]]=r[1]
+            return data
     except Exception:
         return {}
 
 def get_table_comments(dbid: str, schema: str):
     try:
-        engine = create_engine(_conn_str)
-        result = engine.execute(text('''
-        SELECT `table`, `comment` FROM comments 
-        WHERE id in ( SELECT max(id) as id FROM comments
-                    WHERE `type` = :type and `dbid` = :dbid and `schema` = :schema 
-                    GROUP BY `table` )
-        '''), type=str(C_TABLE), dbid=dbid, schema=schema)
+        engine = create_engine(_conn_str)       
         data={}
-        for r in result.fetchall():
-            data[r[0]]=r[1]
+        with engine.connect() as conn:
+            result = conn.execute(text('''
+            SELECT tabname, memo FROM comments
+            WHERE id in ( SELECT max(id) as id FROM comments
+                        WHERE type = :type and dbid = :dbid and schema = :schema
+                        GROUP BY tabname )
+            '''), {'type':str(C_TABLE), 'dbid':dbid, 'schema':schema})
+            
+            for r in result.fetchall():
+                data[r[0]]=r[1]
         return data
     except Exception:
         return {}
 
 def get_column_comments(dbid: str, schema: str, table: str):
     try:
         engine = create_engine(_conn_str)
-        result = engine.execute(text('''
-        SELECT `column`, `comment` FROM comments 
-        WHERE id in ( SELECT max(id) as id FROM comments
-                    WHERE `type` = :type and `dbid` = :dbid and `schema` = :schema and `table` = :table
-                    GROUP BY `column` )
-        '''), type=str(C_COLUMN), dbid=dbid, schema=schema, table=table)
-        data={}
-        for r in result.fetchall():
-            data[r[0]]=r[1]
-        return data
+        with engine.connect() as conn:
+            result = conn.execute(text('''
+            SELECT colname, memo FROM comments
+            WHERE id in ( SELECT max(id) as id FROM comments
+                        WHERE type = :type and dbid = :dbid and schema = :schema and tabname = :table
+                        GROUP BY colname )
+            '''), {'type':str(C_COLUMN), 'dbid':dbid, 'schema':schema, 'table':table})
+            data={}
+            for r in result.fetchall():
+                data[r[0]]=r[1]
+            return data
     except Exception:
         return {}
 
 def set_comments(**args):
 
     param={
         'type': args['type'],
-        'comment': args['comment'],
+        'memo': args['comment'],
         'dbid': args['dbid']
     }
 
     type = int(args['type'])
 
     if type==C_CONN:
         pass
     elif type==C_SCHEMA:
         param.update({'schema': args['schema']})
     elif type==C_TABLE:
-        param.update({'schema': args['schema'], 'table': args['table']})
+        param.update({'schema': args['schema'], 'tabname': args['table']})
     elif type==C_COLUMN:
-        param.update({'schema': args['schema'], 'table': args['table'], 'column': args['column']})
+        param.update({'schema': args['schema'], 'tabname': args['table'], 'colname': args['column']})
     else:
         raise Exception('arg error')
 
     engine = create_engine(_conn_str)
     Session = sessionmaker(bind=engine)
     session = Session()
     c = Comments(**param)
```

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/db.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     '''
     usedb=None
     if 'db' in kwargs:
         usedb=kwargs['db']
     eng = engine.getEngine(dbid, usedb)
     if eng:
         conn = eng.connect()
-        result = conn.execute(sql)
+        result = conn.exec_driver_sql(sql)
         data = result.fetchall()
         conn.close()
         return data
 
     return []
 
 def set_limit(sql: str, def_lim: int = 200, max_lim: int = 10000) -> (bool, str):
@@ -75,15 +75,19 @@
         raise Exception(sql)
 
     usedb=None
     if 'db' in kwargs:
         usedb=kwargs['db']
     eng = engine.getEngine(dbid, usedb)
     if eng:
-        result = eng.execute(sql)
+        conn = eng.connect()
+        transaction=conn.begin()
+        result = conn.exec_driver_sql(sql)
+        transaction.commit()
+        conn.close()
         if result.returns_rows:
             data = [make_row_serializable(row) for row in result]
             columns = list(result.keys())
             return {'columns': columns, 'data': data}
     return {}
 
 def get_column_info(dbid, db, tbl):
```

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/engine.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/engine.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/handlers.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/serializer.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/serializer.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/task.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/task.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/package.json` & `jupyterlab_sql_explorer-0.2.0/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8982666666666667%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.1.6', '@jupyterlab/coreutils': '^6.1.6', "*

 * *                   "'@jupyterlab/mainmenu': '^4.1.6', '@jupyterlab/services': '^7.1.6', "*

 * *                   "'@jupyterlab/settingregistry': '^4.1.6', '@lumino/datagrid': '^2.3.0-alpha.0', "*

 * *                   "'@lumino/commands': '^2.3.0', '@lumino/widgets': '^2.3.2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@jupyterlab/testutils': '^4.0.0', "*

 * *                      "'@types/jest': '^29.2.0', '@ […]*

```diff
@@ -2,47 +2,57 @@
     "author": {
         "name": "groupnotes"
     },
     "bugs": {
         "url": "https://github.com/groupnotes/jupyterlab-sql-explorer/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
-        "@lumino/datagrid": "0.36.7",
+        "@jupyterlab/application": "^4.1.6",
+        "@jupyterlab/coreutils": "^6.1.6",
+        "@jupyterlab/mainmenu": "^4.1.6",
+        "@jupyterlab/services": "^7.1.6",
+        "@jupyterlab/settingregistry": "^4.1.6",
+        "@lumino/commands": "^2.3.0",
+        "@lumino/datagrid": "^2.3.0-alpha.0",
+        "@lumino/widgets": "^2.3.2",
         "react-virtualized-auto-sizer": "^1.0.20",
         "react-window": "^1.8.9"
     },
     "description": "A JupyterLab extension for Database",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
         "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
-        "typescript": "~4.1.3"
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "ts-jest": "^29.1.2",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
             "plugin:prettier/recommended"
@@ -102,23 +112,19 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "schema/*.json",
+        "style/index.js"
     ],
     "homepage": "https://github.com/groupnotes/jupyterlab-sql-explorer",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.5d0a100c5f87bad68bb4.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_sql_explorer"
                 },
                 "managers": [
                     "pip"
@@ -164,28 +170,32 @@
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-explorer",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/groupnotes/jupyterlab-sql-explorer.git"
     },
-    "resolutions": {
-        "@lumino/coreutils": "^1.11.0",
-        "@lumino/widgets": "^1.37.2"
-    },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
@@ -203,30 +213,35 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/labextension/schemas/jupyterlab-sql-explorer/package.json.orig` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8194083333333333%*

 * *Differences: {"'author'": "'groupnotes'",*

 * * "'bugs'": "{'url': 'https://github.com/groupnotes/jupyterlab-sql-explorer.git/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/coreutils': '^6.0.0', "*

 * *                   "'@jupyterlab/services': '^7.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/mainmenu', '@lumino/datagrid', "*

 * *                   "'react-virtualized-auto-sizer', 'react-window']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0' […]*

```diff
@@ -1,48 +1,46 @@
 {
-    "author": {
-        "name": "groupnotes"
-    },
+    "author": "groupnotes",
     "bugs": {
-        "url": "https://github.com/groupnotes/jupyterlab-sql-explorer/issues"
+        "url": "https://github.com/groupnotes/jupyterlab-sql-explorer.git/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
-        "@lumino/datagrid": "0.36.7",
-        "react-virtualized-auto-sizer": "^1.0.20",
-        "react-window": "^1.8.9"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "A JupyterLab extension for Database",
     "devDependencies": {
-        "@babel/core": "^7.0.0",
-        "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
-        "@types/jest": "^26.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "jest": "^29.2.0",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
-        "typescript": "~4.1.3"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
             "plugin:prettier/recommended"
@@ -102,95 +100,72 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
-    "homepage": "https://github.com/groupnotes/jupyterlab-sql-explorer",
+    "homepage": "https://github.com/groupnotes/jupyterlab-sql-explorer.git",
     "jupyterlab": {
         "discovery": {
             "server": {
                 "base": {
-                    "name": "jupyterlab_sql_explorer"
+                    "name": "jupyterlab-sql-explorer"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
-        "outputDir": "jupyterlab_sql_explorer/labextension",
-        "schemaDir": "schema",
-        "sharedPackages": {
-            "@jupyterlab/application": {
-                "bundled": false,
-                "singleton": true
-            },
-            "@lumino/datagrid": {
-                "bundled": true,
-                "singleton": true
-            },
-            "codemirror": {
-                "bundled": false,
-                "singleton": true
-            },
-            "react": {
-                "bundled": false,
-                "singleton": true
-            },
-            "react-dom": {
-                "bundled": false,
-                "singleton": true
-            }
-        }
+        "outputDir": "jupyterlab-sql-explorer/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
-        "jupyterlab-extension",
-        "sql",
-        "database",
-        "hive",
-        "mysql",
-        "postgresql",
-        "sqlite"
+        "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab-sql-explorer",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/groupnotes/jupyterlab-sql-explorer.git"
-    },
-    "resolutions": {
-        "@lumino/coreutils": "^1.11.0",
-        "@lumino/widgets": "^1.37.2"
+        "url": "https://github.com/groupnotes/jupyterlab-sql-explorer.git.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_sql_explorer/labextension jupyterlab_sql_explorer/_version.py",
+        "clean:labextension": "rimraf jupyterlab-sql-explorer/labextension jupyterlab-sql-explorer/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -198,30 +173,35 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.0"
 }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_comments.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_handlers.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_mysql.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/t_mysql.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_sqlite.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/jupyterlab_sql_explorer/tests/test_utils.py` & `jupyterlab_sql_explorer-0.2.0/jupyterlab_sql_explorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/SqlWidget.tsx` & `jupyterlab_sql_explorer-0.2.0/src/SqlWidget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  */
 export class SqlWidget extends ReactWidget {
   constructor(
     model: SqlModel,
     jp_services: IJpServices,
     options?: Widget.IOptions
   ) {
-    super(options);
+    super();
     this._model = model;
     this._jp_services = jp_services;
     this.node.id = 'SqlSession-root';
     this.addClass(sqlWidgetStyle);
   }
 
   /**
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/cmd_menu.ts` & `jupyterlab_sql_explorer-0.2.0/src/cmd_menu.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/handler.ts` & `jupyterlab_sql_explorer-0.2.0/src/handler.ts`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'jupyterlab-sql-explorer', // API Namespace
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
-  } catch (error) {
+  } catch (error: any) {
     // when user about, return { error }
     // FIXME: Because the ServerConnection does not handle AbortError, we have to use a hack to deal with user abort
     if (error.message === 'The user aborted a request.') {
       return { status: 'ERR', message: error.message as string } as any as T;
     }
     throw new ServerConnection.NetworkError(error);
   }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/icons.ts` & `jupyterlab_sql_explorer-0.2.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/index.ts` & `jupyterlab_sql_explorer-0.2.0/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
   });
 
   addCommands(app, model, trans);
 
   // Add a menu for the plugin
   if (mainMenu && app.version.split('.').slice(0, 2).join('.') < '3.7') {
     // Support JLab 3.0
-    mainMenu.addMenu(createMenu(app.commands, trans), { rank: 60 });
+    mainMenu.addMenu(createMenu(app.commands, trans));
   }
 
   // Create the Sql widget sidebar
   const sqlPlugin = new SqlWidget(model, jp_services);
   sqlPlugin.id = 'jp-sql-sessions';
   sqlPlugin.title.icon = sqlIcon;
   sqlPlugin.title.caption = 'SQL explorer';
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/interfaces.ts` & `jupyterlab_sql_explorer-0.2.0/src/interfaces.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/model.ts` & `jupyterlab_sql_explorer-0.2.0/src/model.ts`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
       }
       if (!find) {
         return [];
       }
     }
     return cur_list.map(
       ({ name, desc, type, subtype, fix }) =>
-        ({ name, desc, type, subtype, fix } as IDbItem)
+        ({ name, desc, type, subtype, fix }) as IDbItem
     );
   }
 
   add_conn = async (conn: IDBConn): Promise<void> => {
     const rc = await edit_conn(conn);
     if (rc.status === 'OK') {
       const { name, db_id } = conn;
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/__tests__/model.spec.ts` & `jupyterlab_sql_explorer-0.2.0/src/__tests__/model.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/auto_resizer/AutoSizer.ts` & `jupyterlab_sql_explorer-0.2.0/src/auto_resizer/AutoSizer.ts`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     width: (this.props as HeightAndWidthProps).defaultWidth || 0
   };
 
   _autoSizer: HTMLElement | null = null;
   //_detectElementResize: DetectElementResize | null = null;
   _parentNode: HTMLElement | null = null;
   _resizeObserver: ResizeObserver | null = null;
-  _timeoutId: number | null = null;
+  _timeoutId: ReturnType<typeof setTimeout> | null = null;
 
   componentDidMount(): void {
     //const { nonce } = this.props;
 
     if (
       this._autoSizer &&
       this._autoSizer.parentNode &&
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/auto_resizer/types.ts` & `jupyterlab_sql_explorer-0.2.0/src/auto_resizer/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/ActionBtn.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/ActionBtn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/ask_pass.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/ask_pass.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/collist.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/collist.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/dblist.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/dblist.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/new_conn.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/new_conn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/sqlPanel.tsx` & `jupyterlab_sql_explorer-0.2.0/src/components/sqlPanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/components/styles.ts` & `jupyterlab_sql_explorer-0.2.0/src/components/styles.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/sqlConsole/ResultsTable.ts` & `jupyterlab_sql_explorer-0.2.0/src/sqlConsole/ResultsTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/sqlConsole/Table.ts` & `jupyterlab_sql_explorer-0.2.0/src/sqlConsole/Table.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/src/sqlConsole/console.ts` & `jupyterlab_sql_explorer-0.2.0/src/sqlConsole/console.ts`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     if (this._context) {
       await this._context.save();
       return;
     }
 
     if (this._context2) {
-      this._context2.model.value.text = this.editor.value;
+      this._context2.model.sharedModel.setSource(this.editor.value);
       await this._context2.save();
       return;
     }
 
     const result = await InputDialog.getText({
       title: trans.__('Please input sql file name'),
       text: 'work/untitled.sql'
@@ -123,15 +123,16 @@
       //const m=await docManager.newUntitled({type:'file', ext:'.sql'})
       const context = new Context({
         manager: docManager.services,
         factory: textModelFactory,
         path: fp
       });
       await context.initialize(true);
-      context.model.value.text = this.editor.value;
+      // for 3.6.x context.model.value.text = this.editor.value;
+      context.model.sharedModel.setSource(this.editor.value);
       await context.save();
 
       this._context2 = context;
     }
   };
 
   stop = (): void => {
@@ -310,15 +311,17 @@
       const sql = `;\n\n${init_sql}\n`;
       (
         (widget as MainAreaWidget).content as SqlConsoleWidget
       ).editor.appendText(sql);
     }
   } else {
     const sql = `-- conn: ${qmodel.dbid}\n\n${init_sql}\n`;
-    const model = new CodeEditor.Model({ value: sql });
+    // for 3.6.x const model = new CodeEditor.Model({ value: sql });
+    const model = new CodeEditor.Model();
+    model.sharedModel.setSource(sql);
     const content = new SqlConsoleWidget(qmodel, undefined, model, jp_services);
     content.theme = get_theme(themeManager);
     widget = new MainAreaWidget({ content });
     setToolbar(widget, toolbarFactory);
     widget.id = id;
     widget.title.icon = queryIcon;
     widget.title.label = qmodel.isConnReadOnly
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/sqlConsole/editor.ts` & `jupyterlab_sql_explorer-0.2.0/src/sqlConsole/editor.ts`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   readonly updateConn: (conn: string) => void;
 }
 
 export class Editor implements IEditor, IDisposable {
   constructor(model: CodeEditor.IModel, editorFactory: IEditorFactoryService) {
     this._model = model;
     this._widget = new EditorWidget(model, editorFactory);
-    this._model.value.changed.connect(() => {
+    this._model.sharedModel.changed.connect(() => {
       this._valueChanged.emit(this.value);
     }, this);
     this._model.mimeType = 'text/x-sql';
     this._widget.executeCurrent.connect(() => {
       this._execute.emit(this.value);
     }, this);
   }
@@ -53,29 +53,29 @@
     const line0 = lines[0];
     const match = line0?.match(/^--\s*conn:\s*(.*?)\s*$/);
     if (match) {
       lines[0] = newline;
     } else {
       lines.unshift(newline + '\n');
     }
-    this.widget.model.value.text = lines.join('\n');
+    this.widget.model.sharedModel.setSource(lines.join('\n'));
   }
 
   get value(): string {
-    return this._model.value.text;
+    return this._model.sharedModel.getSource();
   }
 
   get sql(): string {
     // Get the current SQL statement separated by semicolons
     // or the selected text as sql
     const editor = this.widget.editor;
     const selection = editor.getSelection();
     const start: number = editor.getOffsetAt(selection.start);
     const end: number = editor.getOffsetAt(selection.end);
-    let text = this._model.value.text;
+    let text = this._model.sharedModel.getSource();
     if (start !== end) {
       if (start > end) {
         text = text.slice(end, start);
       } else {
         text = text.slice(start, end);
       }
     }
@@ -135,20 +135,20 @@
 
 export class EditorWidget extends CodeEditorWrapper {
   constructor(model: CodeEditor.IModel, editorFactory: IEditorFactoryService) {
     super({
       model,
       factory: editorFactory.newInlineEditor
     });
-    this.editor.addKeydownHandler(this._onKeydown);
+    //this.editor.addKeydownHandler(this._onKeydown);
     this.addClass('jp-sql-explorer-ed');
   }
 
   dispose = (): void => {
-    this.editor.addKeydownHandler(this._onKeydown);
+    //this.editor.addKeydownHandler(this._onKeydown);
     //this.editor.removeKeydownHandler(this._onKeydown)
     super.dispose();
   };
 
   get executeCurrent(): ISignal<this, void> {
     return this._executeCurrent;
   }
```

### Comparing `jupyterlab_sql_explorer-0.1.2/src/sqlConsole/toolbar.tsx` & `jupyterlab_sql_explorer-0.2.0/src/sqlConsole/toolbar.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
   private _showDetail = () => {
     const { errmsg } = this.state;
     const { trans } = this.props;
     showErrorMessage(trans.__('ERROR'), errmsg);
   };
 
-  private _timer_id!: number | null;
+  private _timer_id!: ReturnType<typeof setTimeout> | null;
 }
 
 export class RunStatus extends ReactWidget {
   constructor(options: IRunStatusOptions) {
     super();
     this._queryModel = options.model;
     this._trans = options.trans;
```

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/column.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/column.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/conn-add.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/conn-add.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/conn.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/conn.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/delete.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/error.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/error.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/hive-1.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/hive-1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/hive-2.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/hive-2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/hive.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/hive.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/mysql.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/mysql.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/oracle.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/oracle.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/pgsql-1.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/pgsql-1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/pgsql-3.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/pgsql-3.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/pgsql.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/pgsql.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/query.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/query.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/root.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/root.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/sql.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/sql.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/sql_script.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/sql_script.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/sqlite.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/sqlite.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/table-2.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/table-2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/table-3.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/table-3.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/table.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/table.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/view.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/view.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/view1.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/view1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/view2.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/view2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/style/icons/view3.svg` & `jupyterlab_sql_explorer-0.2.0/style/icons/view3.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/ui-tests/README.md` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Integration Testing
 
 This folder contains the integration tests of the extension.
 
 They are defined using [Playwright](https://playwright.dev/docs/intro) test runner
-and [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) helper.
+and [Galata](https://github.com/jupyterlab/jupyterlab/tree/main/galata) helper.
 
 The Playwright configuration is defined in [playwright.config.js](./playwright.config.js).
 
 The JupyterLab server configuration to use for the integration test is defined
 in [jupyter_server_test_config.py](./jupyter_server_test_config.py).
 
 The default configuration will produce video for failing tests and an HTML report.
 
+> There is a new experimental UI mode that you may fall in love with; see [that video](https://www.youtube.com/watch?v=jF0yA-JLQW0).
+
 ## Run the tests
 
 > All commands are assumed to be executed from the root directory
 
 To run the tests, you need to:
 
 1. Compile the extension:
@@ -105,15 +107,22 @@
 ```sh
 cd ./ui-tests
 jlpm install
 jlpm playwright install
 cd ..
 ```
 
-3. Execute the [Playwright code generator](https://playwright.dev/docs/codegen):
+3. Start the server:
+
+```sh
+cd ./ui-tests
+jlpm start
+```
+
+4. Execute the [Playwright code generator](https://playwright.dev/docs/codegen) in **another terminal**:
 
 ```sh
 cd ./ui-tests
 jlpm playwright codegen localhost:8888
 ```
 
 ## Debug tests
@@ -140,9 +149,19 @@
 cd ..
 ```
 
 3. Execute the Playwright tests in [debug mode](https://playwright.dev/docs/debug):
 
 ```sh
 cd ./ui-tests
-PWDEBUG=1 jlpm playwright test
+jlpm playwright test --debug
+```
+
+## Upgrade Playwright and the browsers
+
+To update the web browser versions, you must update the package `@playwright/test`:
+
+```sh
+cd ./ui-tests
+jlpm up "@playwright/test"
+jlpm playwright install
 ```
```

### Comparing `jupyterlab_sql_explorer-0.1.2/ui-tests/tests/jupyterlab-sql-explorer.spec.ts` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/ui-tests/tests/jupyterlab-sql-explorer.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/.gitignore` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 node_modules/
 *.log
 .eslintcache
 .stylelintcache
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
-jupyterlab_sql_explorer/labextension
+jupyterlab-sql-explorer/labextension
 # Version file is handled by hatchling
-jupyterlab_sql_explorer/_version.py
+jupyterlab-sql-explorer/_version.py
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
@@ -116,7 +116,10 @@
 # Pyre type checker
 .pyre/
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
+
+# Yarn cache
+.yarn/
```

### Comparing `jupyterlab_sql_explorer-0.1.2/LICENSE` & `jupyterlab_sql_explorer-0.2.0/_temp_extension/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, esc
+Copyright (c) 2024, groupnotes
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_sql_explorer-0.1.2/README.md` & `jupyterlab_sql_explorer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_explorer-0.1.2/pyproject.toml` & `jupyterlab_sql_explorer-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
-requires = ["hatchling>=1.4.0", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab-sql-explorer"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
-    "Framework :: Jupyter :: JupyterLab :: 3",
+    "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
+
 dependencies = [
-    "jupyter_server>=1.21,<3",
-    "sqlalchemy>=1.4,<2",
-    "sqlparse>=0.4.1"
+    "jupyter_server>=2.0.1,<3",
+    "sqlalchemy>=1.3",
+    "sqlparse>=0.4.1",
 ]
+
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
@@ -79,12 +81,16 @@
 source_dir = "src"
 build_dir = "jupyterlab_sql_explorer/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
-before-build-npm = ["python -m pip install jupyterlab~=3.1", "jlpm", "jlpm build:prod"]
+before-build-npm = [
+    "python -m pip install 'jupyterlab>=4.0.0,<5'",
+    "jlpm",
+    "jlpm build:prod"
+]
 before-build-python = ["jlpm clean:all"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `jupyterlab_sql_explorer-0.1.2/PKG-INFO` & `jupyterlab_sql_explorer-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab-sql-explorer
-Version: 0.1.2
+Version: 0.2.0
+Dynamic: Keywords
 Summary: A JupyterLab extension for Database
 Project-URL: Homepage, https://github.com/groupnotes/jupyterlab-sql-explorer
 Project-URL: Bug Tracker, https://github.com/groupnotes/jupyterlab-sql-explorer/issues
 Project-URL: Repository, https://github.com/groupnotes/jupyterlab-sql-explorer.git
 Author: groupnotes
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, esc
+        Copyright (c) 2024, groupnotes
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -34,28 +35,28 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: jupyter-server<3,>=1.21
-Requires-Dist: sqlalchemy<2,>=1.4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
+Requires-Dist: sqlalchemy>=1.3
 Requires-Dist: sqlparse>=0.4.1
 Provides-Extra: hive
 Requires-Dist: pyhive[hive]>=0.6.5; extra == 'hive'
 Provides-Extra: mysql
 Requires-Dist: pymysql; extra == 'mysql'
 Provides-Extra: pgsql
 Requires-Dist: psycopg2; extra == 'pgsql'
```

