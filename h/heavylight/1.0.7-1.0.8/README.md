# Comparing `tmp/heavylight-1.0.7.tar.gz` & `tmp/heavylight-1.0.8.tar.gz`

## Comparing `heavylight-1.0.7.tar` & `heavylight-1.0.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 heavylight-1.0.7/.python-version
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 heavylight-1.0.7/mkdocs.yml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 heavylight-1.0.7/requirements-dev.lock
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 heavylight-1.0.7/requirements.lock
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 heavylight-1.0.7/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 heavylight-1.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 heavylight-1.0.7/developer-setup/environment-notes.md
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/index.md
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/storage_function.md
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/tables.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/custom_css.css
--rw-r--r--   0        0        0   177915 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/dependency-graph-dark.svg
--rw-r--r--   0        0        0   178414 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/dependency-graph-light.svg
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/mathjax.js
--rw-r--r--   0        0        0   176374 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-can-clear-dark.svg
--rw-r--r--   0        0        0   177132 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-can-clear-light.svg
--rw-r--r--   0        0        0   173374 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-last-needed-dark.svg
--rw-r--r--   0        0        0   172658 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-last-needed-light.svg
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/heavylight_Model.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/heavylight_Table.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/lightmodel.md
--rw-r--r--   0        0        0    56497 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/getting_started/heavylight_tables.ipynb
--rw-r--r--   0        0        0   172293 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/getting_started/intro_to_heavylight.ipynb
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/memory_optimization.md
--rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/recursive_life_insurance.ipynb
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/vectorized_models.ipynb
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/basic_cashflow.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/readme.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/readme_example.py
--rw-r--r--   0        0        0    21406 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/memory_optimizations/example.ipynb
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/docs_check_tables_md.ipynb
--rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0    76024 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/safe_string_table_lookup.ipynb
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/string_lookup_investigation.ipynb
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/super_init_example.ipynb
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_bounds_check.ipynb
--rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation.ipynb
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation.md
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/test_tables_v1.0.7.ipynb
--rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/using_dataclasses.ipynb
--rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/vectors.py
--rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
--rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation_files/table_documentation_32_1.png
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/protection_model.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/run_model.py
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/covert_q_x_tables.ipynb
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/q_x_generic.csv
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/qx_generic_raw.csv
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/uk_zero_spot.csv
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/protection_model.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/run_model.py
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/covert_q_x_tables.ipynb
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/q_x_generic.csv
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/qx_generic_raw.csv
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/uk_zero_spot.csv
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/__init__.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/heavylight.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/heavytables.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/make_examples.py
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/memory_optimized_cache.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/memory_optimized_model.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_base.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_mo.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_np.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/readme.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_base.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_mo.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_np.py
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/tables/q_x_generic.csv
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/template/model.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_examples.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_heavylight.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_heavytables.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_lightmodel.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_lightmodel_df.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_memory_savings.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_optimized_cache.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.7/LICENSE
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 heavylight-1.0.7/README.md
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 heavylight-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 heavylight-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 heavylight-1.0.8/.python-version
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 heavylight-1.0.8/mkdocs.yml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 heavylight-1.0.8/requirements-dev.lock
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 heavylight-1.0.8/requirements.lock
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 heavylight-1.0.8/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 heavylight-1.0.8/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 heavylight-1.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 heavylight-1.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 heavylight-1.0.8/developer-setup/environment-notes.md
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/index.md
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/storage_function.md
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/tables.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/custom_css.css
+-rw-r--r--   0        0        0   177915 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/dependency-graph-dark.svg
+-rw-r--r--   0        0        0   178414 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/dependency-graph-light.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/mathjax.js
+-rw-r--r--   0        0        0   176374 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/memopt-can-clear-dark.svg
+-rw-r--r--   0        0        0   177132 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/memopt-can-clear-light.svg
+-rw-r--r--   0        0        0   173374 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/memopt-last-needed-dark.svg
+-rw-r--r--   0        0        0   172658 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/_static/memopt-last-needed-light.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/api/heavylight_Model.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/api/heavylight_Table.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/api/lightmodel.md
+-rw-r--r--   0        0        0    56497 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/getting_started/heavylight_tables.ipynb
+-rw-r--r--   0        0        0   172293 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/getting_started/intro_to_heavylight.ipynb
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/theory/memory_optimization.md
+-rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/theory/recursive_life_insurance.ipynb
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 heavylight-1.0.8/docs/theory/vectorized_models.ipynb
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/basic_cashflow.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/readme.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/readme_example.py
+-rw-r--r--   0        0        0    21406 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/memory_optimizations/example.ipynb
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/docs_check_tables_md.ipynb
+-rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    76024 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/safe_string_table_lookup.ipynb
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/string_lookup_investigation.ipynb
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/super_init_example.ipynb
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/table_bounds_check.ipynb
+-rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/table_documentation.ipynb
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/table_documentation.md
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/test_tables_v1.0.7.ipynb
+-rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/using_dataclasses.ipynb
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/vectors.py
+-rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/notebook/table_documentation_files/table_documentation_32_1.png
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.8/examples/std_model_numpy/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/heavytables.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/make_examples.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/memory_optimized_cache.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/memory_optimized_model.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/protection_model_base.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/protection_model_mo.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/protection_model_np.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/readme.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/run_model_base.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/run_model_mo.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/run_model_np.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/protection/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 heavylight-1.0.8/src/heavylight/examples/template/model.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_examples.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_heavylight.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_heavytables.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_lightmodel.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_lightmodel_df.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_memory_savings.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 heavylight-1.0.8/tests/test_optimized_cache.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.8/LICENSE
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 heavylight-1.0.8/README.md
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 heavylight-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 heavylight-1.0.8/PKG-INFO
```

### Comparing `heavylight-1.0.7/mkdocs.yml` & `heavylight-1.0.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/requirements-dev.lock` & `heavylight-1.0.8/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/.devcontainer/devcontainer.json` & `heavylight-1.0.8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/.github/workflows/docs.yml` & `heavylight-1.0.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/.github/workflows/python-package.yml` & `heavylight-1.0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/developer-setup/environment-notes.md` & `heavylight-1.0.8/developer-setup/environment-notes.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/index.md` & `heavylight-1.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/storage_function.md` & `heavylight-1.0.8/docs/storage_function.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/tables.md` & `heavylight-1.0.8/docs/tables.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/custom_css.css` & `heavylight-1.0.8/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/dependency-graph-dark.svg` & `heavylight-1.0.8/docs/_static/dependency-graph-dark.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/dependency-graph-light.svg` & `heavylight-1.0.8/docs/_static/dependency-graph-light.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/memopt-can-clear-dark.svg` & `heavylight-1.0.8/docs/_static/memopt-can-clear-dark.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/memopt-can-clear-light.svg` & `heavylight-1.0.8/docs/_static/memopt-can-clear-light.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/memopt-last-needed-dark.svg` & `heavylight-1.0.8/docs/_static/memopt-last-needed-dark.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/_static/memopt-last-needed-light.svg` & `heavylight-1.0.8/docs/_static/memopt-last-needed-light.svg`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/getting_started/heavylight_tables.ipynb` & `heavylight-1.0.8/docs/getting_started/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/getting_started/intro_to_heavylight.ipynb` & `heavylight-1.0.8/docs/getting_started/intro_to_heavylight.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/theory/memory_optimization.md` & `heavylight-1.0.8/docs/theory/memory_optimization.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/theory/recursive_life_insurance.ipynb` & `heavylight-1.0.8/docs/theory/recursive_life_insurance.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/docs/theory/vectorized_models.ipynb` & `heavylight-1.0.8/docs/theory/vectorized_models.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/basic_cashflow.py` & `heavylight-1.0.8/examples/basic_cashflow.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/readme_example.py` & `heavylight-1.0.8/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/memory_optimizations/example.ipynb` & `heavylight-1.0.8/examples/memory_optimizations/example.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/docs_check_tables_md.ipynb` & `heavylight-1.0.8/examples/notebook/docs_check_tables_md.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.8/examples/notebook/heavylight_basic.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.8/examples/notebook/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/safe_string_table_lookup.ipynb` & `heavylight-1.0.8/examples/notebook/safe_string_table_lookup.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.8/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/string_lookup_investigation.ipynb` & `heavylight-1.0.8/examples/notebook/string_lookup_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/super_init_example.ipynb` & `heavylight-1.0.8/examples/notebook/super_init_example.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/table_bounds_check.ipynb` & `heavylight-1.0.8/examples/notebook/table_bounds_check.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/table_documentation.ipynb` & `heavylight-1.0.8/examples/notebook/table_documentation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/table_documentation.md` & `heavylight-1.0.8/examples/notebook/table_documentation.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/table_maker.ipynb` & `heavylight-1.0.8/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/test_tables_v1.0.7.ipynb` & `heavylight-1.0.8/examples/notebook/test_tables_v1.0.7.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/using_dataclasses.ipynb` & `heavylight-1.0.8/examples/notebook/using_dataclasses.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/vectors.ipynb` & `heavylight-1.0.8/examples/notebook/vectors.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/vectors.py` & `heavylight-1.0.8/examples/notebook/vectors.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv` & `heavylight-1.0.8/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/notebook/table_documentation_files/table_documentation_32_1.png` & `heavylight-1.0.8/examples/notebook/table_documentation_files/table_documentation_32_1.png`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/protection_model.py` & `heavylight-1.0.8/examples/std_model/protection_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/protection_risk_model_generic.xlsx` & `heavylight-1.0.8/examples/std_model/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/run_model.py` & `heavylight-1.0.8/examples/std_model/run_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/tables/covert_q_x_tables.ipynb` & `heavylight-1.0.8/examples/std_model/tables/covert_q_x_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/tables/forward_rates.csv` & `heavylight-1.0.8/examples/std_model/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/tables/q_x_generic.csv` & `heavylight-1.0.8/examples/std_model/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/tables/qx_generic_raw.csv` & `heavylight-1.0.8/examples/std_model/tables/qx_generic_raw.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model/tables/uk_zero_spot.csv` & `heavylight-1.0.8/examples/std_model/tables/uk_zero_spot.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/protection_model.py` & `heavylight-1.0.8/examples/std_model_numpy/protection_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/protection_risk_model_generic.xlsx` & `heavylight-1.0.8/examples/std_model_numpy/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/run_model.py` & `heavylight-1.0.8/examples/std_model_numpy/run_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/tables/covert_q_x_tables.ipynb` & `heavylight-1.0.8/examples/std_model_numpy/tables/covert_q_x_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/tables/forward_rates.csv` & `heavylight-1.0.8/examples/std_model_numpy/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/tables/q_x_generic.csv` & `heavylight-1.0.8/examples/std_model_numpy/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/tables/qx_generic_raw.csv` & `heavylight-1.0.8/examples/std_model_numpy/tables/qx_generic_raw.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/examples/std_model_numpy/tables/uk_zero_spot.csv` & `heavylight-1.0.8/examples/std_model_numpy/tables/uk_zero_spot.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/heavylight.py` & `heavylight-1.0.8/src/heavylight/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/heavytables.py` & `heavylight-1.0.8/src/heavylight/heavytables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Heavytables
 # Provides a high performance multiple-index -> single index table
 
 import itertools
 import pandas as pd
 import numpy as np
+from typing import Callable, Dict, List, Union, Any
 
 # Lookup classes
 # Each key column requires an input class which maps from the source datatype to an integer
 
 class IntegerLookup:
     """An integer lookup - unsafe as doesn't check bounds"""
     def get(self, values):
@@ -121,28 +122,29 @@
         return self.get_value(*keys)
     
 class Table:
     """Table provides multi-key compatible high performance table lookup.
     """
     col_types = "int", "int_bound", "str", "band", "float"
 
-    def __init__(self, df:pd.DataFrame, rectify=False, safe=True):
+    def __init__(self, df:pd.DataFrame, rectify: Union[bool, None]=False, safe: Union[bool, None]=True):
         """Initialise a table from a dataframe.
         
         parameters:
-         - `rectify`: force table to be rectangular (default False)
-         - `safe`: validates that integers are between bounds (default True)
+          df: the pandas dataframe used to initialise the table
+          rectify: force table to be rectangular (default False)
+          safe: validates that integers are between bounds (default True)
 
         Tables should be in long format:
          - the final column containing the values to look up
          - all other columns contain keys to lookup
          - tables should be contingous, i.e. no gaps in integer keys.
          - tables should be complete if viewed as square matrixes (i.e. all combinations of keys are input).  If not, you should fill any gaps with np.nan or a suitable value.
 
-        The type of key is determined by the suffix on the column name:
+        The type of key is determined by the suffix on the dataframe `df` column names:
         `|int`: integers (...0, 1, 2, 3...), can start and end anywhere, but must be consecutive
         `|int_bound`: as `|int` but any values are constrained to the lowest and highest values.
         `|str': keys are interpreted as strings, e.g. 'M' and 'F'
         `|band`: key is numeric and treated as the upper bound on a lookup.
         `|float`: not currently available due to floating point equality, use int or band depending on use case.
         """
         if rectify:
@@ -169,15 +171,15 @@
                 lower = df[col].min()
                 upper = df[col].max()
                 self.mappers.append(BoundIntLookup(lower=lower, upper=upper))
             elif col_type == "str":
                 cols = df[col].unique()
                 string_mapper = StringLookup(cols)
                 self.mappers.append(string_mapper)
-                df_int_keys[col] = string_mapper.get(df_int_keys[col])
+                df_int_keys[col] = string_mapper.get(df_int_keys[col].values)
 
             elif col_type in ["str_unsafe", "band"]:
                 df_col = pd.DataFrame(df[col].unique(), columns=["band_name"]).reset_index().sort_values("band_name")
 
                 # add a nan on the end so we get errors if the lookup fails
                 # as by default the BandLookup will return last item if no earlier matches
                 # commented out as it converts the datatype - we need these to be integers
```

### Comparing `heavylight-1.0.7/src/heavylight/make_examples.py` & `heavylight-1.0.8/src/heavylight/make_examples.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/memory_optimized_cache.py` & `heavylight-1.0.8/src/heavylight/memory_optimized_cache.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/memory_optimized_model.py` & `heavylight-1.0.8/src/heavylight/memory_optimized_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/protection_model_base.py` & `heavylight-1.0.8/src/heavylight/examples/protection/protection_model_base.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/protection_model_mo.py` & `heavylight-1.0.8/src/heavylight/examples/protection/protection_model_mo.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/protection_model_np.py` & `heavylight-1.0.8/src/heavylight/examples/protection/protection_model_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/protection_risk_model_generic.xlsx` & `heavylight-1.0.8/src/heavylight/examples/protection/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/run_model_base.py` & `heavylight-1.0.8/src/heavylight/examples/protection/run_model_base.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/run_model_mo.py` & `heavylight-1.0.8/src/heavylight/examples/protection/run_model_mo.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/run_model_np.py` & `heavylight-1.0.8/src/heavylight/examples/protection/run_model_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/tables/forward_rates.csv` & `heavylight-1.0.8/src/heavylight/examples/protection/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/protection/tables/q_x_generic.csv` & `heavylight-1.0.8/src/heavylight/examples/protection/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/src/heavylight/examples/template/model.py` & `heavylight-1.0.8/src/heavylight/examples/template/model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_heavylight.py` & `heavylight-1.0.8/tests/test_heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_heavytables.py` & `heavylight-1.0.8/tests/test_heavytables.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_lightmodel.py` & `heavylight-1.0.8/tests/test_lightmodel.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_lightmodel_df.py` & `heavylight-1.0.8/tests/test_lightmodel_df.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_memory_savings.py` & `heavylight-1.0.8/tests/test_memory_savings.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/tests/test_optimized_cache.py` & `heavylight-1.0.8/tests/test_optimized_cache.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/.gitignore` & `heavylight-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/LICENSE` & `heavylight-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/README.md` & `heavylight-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.7/pyproject.toml` & `heavylight-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ] }
 
 [tool.hatch.build.targets.wheel]
 src-dir = "src"
 
 [project]
 name = "heavylight"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
   { name="Matthew Caseres", email="matthewcaseres@outlook.com"}
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `heavylight-1.0.7/PKG-INFO` & `heavylight-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: heavylight
-Version: 1.0.7
+Version: 1.0.8
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
 Project-URL: Documentation, https://lewisfogden.github.io/heavylight/
 Author-email: Lewis Fogden <lewisfogden@gmail.com>, Matthew Caseres <matthewcaseres@outlook.com>
 License-File: LICENSE
 Requires-Python: >=3.8
```

