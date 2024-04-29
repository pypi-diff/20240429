# Comparing `tmp/julearn-0.3.2.dev24.tar.gz` & `tmp/julearn-0.3.2.dev57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.2.dev24.tar", last modified: Thu Apr  4 14:42:17 2024, max compression
+gzip compressed data, was "julearn-0.3.2.dev57.tar", last modified: Mon Apr 29 10:50:55 2024, max compression
```

## Comparing `julearn-0.3.2.dev24.tar` & `julearn-0.3.2.dev57.tar`

### file list

```diff
@@ -1,284 +1,288 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.452727 julearn-0.3.2.dev24/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.460727 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.460727 julearn-0.3.2.dev24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/check-stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.452727 julearn-0.3.2.dev24/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.464727 julearn-0.3.2.dev24/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.468727 julearn-0.3.2.dev24/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/224.misc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/244.misc
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/249.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/251.misc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/changes/newsfragments/255.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.476727 julearn-0.3.2.dev24/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.480727 julearn-0.3.2.dev24/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.484727 julearn-0.3.2.dev24/julearn/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.488727 julearn-0.3.2.dev24/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    33050 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/pipeline/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16338 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.492727 julearn-0.3.2.dev24/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37962 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.496727 julearn-0.3.2.dev24/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:42:17.500728 julearn-0.3.2.dev24/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 14:42:17.000000 julearn-0.3.2.dev24/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:42:17.504727 julearn-0.3.2.dev24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-04 14:42:12.000000 julearn-0.3.2.dev24/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.080479 julearn-0.3.2.dev57/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.024479 julearn-0.3.2.dev57/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.032479 julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.036480 julearn-0.3.2.dev57/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/check-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-29 10:50:55.080479 julearn-0.3.2.dev57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.036480 julearn-0.3.2.dev57/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.024479 julearn-0.3.2.dev57/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.036480 julearn-0.3.2.dev57/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.040480 julearn-0.3.2.dev57/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.040480 julearn-0.3.2.dev57/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.040480 julearn-0.3.2.dev57/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.040480 julearn-0.3.2.dev57/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.044479 julearn-0.3.2.dev57/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/224.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/244.misc
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/249.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/251.misc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/255.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/260.enh
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/changes/newsfragments/260.misc
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.048479 julearn-0.3.2.dev57/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.048479 julearn-0.3.2.dev57/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.048479 julearn-0.3.2.dev57/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.052480 julearn-0.3.2.dev57/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.052480 julearn-0.3.2.dev57/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.052480 julearn-0.3.2.dev57/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.052480 julearn-0.3.2.dev57/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.052480 julearn-0.3.2.dev57/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.056480 julearn-0.3.2.dev57/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.056480 julearn-0.3.2.dev57/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.056480 julearn-0.3.2.dev57/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.060479 julearn-0.3.2.dev57/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.060479 julearn-0.3.2.dev57/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.060479 julearn-0.3.2.dev57/julearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-29 10:50:54.000000 julearn-0.3.2.dev57/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.060479 julearn-0.3.2.dev57/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.060479 julearn-0.3.2.dev57/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.064479 julearn-0.3.2.dev57/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/tests/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/tests/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/tests/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/pipeline/tests/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16338 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.068480 julearn-0.3.2.dev57/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37962 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.072480 julearn-0.3.2.dev57/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.072480 julearn-0.3.2.dev57/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.072480 julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.072480 julearn-0.3.2.dev57/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:50:55.076480 julearn-0.3.2.dev57/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-29 10:50:54.000000 julearn-0.3.2.dev57/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-29 10:50:55.000000 julearn-0.3.2.dev57/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:50:54.000000 julearn-0.3.2.dev57/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-29 10:50:54.000000 julearn-0.3.2.dev57/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 10:50:54.000000 julearn-0.3.2.dev57/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:50:55.080479 julearn-0.3.2.dev57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 10:50:50.000000 julearn-0.3.2.dev57/tox.ini
```

### Comparing `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.2.dev57/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/ci-docs.yml` & `julearn-0.3.2.dev57/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/ci.yml` & `julearn-0.3.2.dev57/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/docs-preview.yml` & `julearn-0.3.2.dev57/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/docs.yml` & `julearn-0.3.2.dev57/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/lint.yml` & `julearn-0.3.2.dev57/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.github/workflows/pypi.yml` & `julearn-0.3.2.dev57/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.gitignore` & `julearn-0.3.2.dev57/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/.pre-commit-config.yaml` & `julearn-0.3.2.dev57/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/LICENSE.md` & `julearn-0.3.2.dev57/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/PKG-INFO` & `julearn-0.3.2.dev57/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev24
+Version: 0.3.2.dev57
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -36,20 +36,25 @@
 Requires-Dist: seaborn<0.13,>=0.12.2; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15,>=0.13.0; extra == "docs"
 Requires-Dist: furo<2024.0.0,>=2022.9.29; extra == "docs"
 Requires-Dist: sphinx_copybutton<0.6,>=0.5.0; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: towncrier<24; extra == "docs"
+Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "docs"
 Provides-Extra: deslib
 Requires-Dist: deslib<0.4,>=0.3.5; extra == "deslib"
 Provides-Extra: viz
 Requires-Dist: panel>=1.3.0; extra == "viz"
 Requires-Dist: bokeh>=3.0.0; extra == "viz"
 Requires-Dist: param>=2.0.0; extra == "viz"
+Provides-Extra: skopt
+Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "skopt"
+Provides-Extra: all
+Requires-Dist: julearn[skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
```

### Comparing `julearn-0.3.2.dev24/README.md` & `julearn-0.3.2.dev57/README.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/codecov.yml` & `julearn-0.3.2.dev57/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/Makefile` & `julearn-0.3.2.dev57/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/_templates/class.rst` & `julearn-0.3.2.dev57/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/_templates/function_warning.rst` & `julearn-0.3.2.dev57/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/_templates/versions.html` & `julearn-0.3.2.dev57/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/base.rst` & `julearn-0.3.2.dev57/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/model_selection.rst` & `julearn-0.3.2.dev57/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/models.rst` & `julearn-0.3.2.dev57/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/scoring.rst` & `julearn-0.3.2.dev57/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/transformers.rst` & `julearn-0.3.2.dev57/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/utils.rst` & `julearn-0.3.2.dev57/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/api/viz.rst` & `julearn-0.3.2.dev57/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/available_pipeline_steps.rst` & `julearn-0.3.2.dev57/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/conf.py` & `julearn-0.3.2.dev57/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     "nilearn": ("https://nilearn.github.io/stable/", None),
     "nibabel": ("https://nipy.org/nibabel/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/dev", None),
     # "sqlalchemy": ("https://docs.sqlalchemy.org/en/20/", None),
     "joblib": ("https://joblib.readthedocs.io/en/latest/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
+    "skopt": ("https://scikit-optimize.readthedocs.io/en/latest", None),
 }
 
 
 # -- numpydoc configuration --------------------------------------------------
 
 numpydoc_show_class_members = False
 numpydoc_xref_param_type = False
```

### Comparing `julearn-0.3.2.dev24/docs/configuration.rst` & `julearn-0.3.2.dev57/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/contributing.rst` & `julearn-0.3.2.dev57/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/examples.rst` & `julearn-0.3.2.dev57/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/faq.rst` & `julearn-0.3.2.dev57/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/getting_started.rst` & `julearn-0.3.2.dev57/docs/getting_started.rst`

 * *Files 4% similar despite different names*

```diff
@@ -82,8 +82,12 @@
 
     pip install -U julearn[viz]
 
 The following optional dependencies are available:
 
 * ``viz``: Visualization tools for ``julearn``. This includes the
   :mod:`.viz` module.
-* ``deslib``: The :mod:`.dynamic` module requires the `deslib`_ package.
+* ``deslib``: The :mod:`.dynamic` module requires the `deslib`_ package. This
+  module is not compatible with newer Python versions and it is unmaintained.
+* ``skopt``: Using the ``"bayes"`` searcher (:class:`~skopt.BayesSearchCV`)
+  requires the `scikit-optimize`_ package.
+* ``all``: Install all optional functional dependencies (except ``deslib``).
```

### Comparing `julearn-0.3.2.dev24/docs/images/corrected_ttest.png` & `julearn-0.3.2.dev57/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/final_estimator.png` & `julearn-0.3.2.dev57/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/iris_X.png` & `julearn-0.3.2.dev57/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/iris_df.png` & `julearn-0.3.2.dev57/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/iris_y.png` & `julearn-0.3.2.dev57/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_calm.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_confbias.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_cv.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_generalization.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_it.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_ml.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/julearn_logo_mlit.png` & `julearn-0.3.2.dev57/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.2.dev57/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/plot_scores.png` & `julearn-0.3.2.dev57/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/scores_run_cv.png` & `julearn-0.3.2.dev57/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.2.dev57/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/images/scores_run_cv_train.png` & `julearn-0.3.2.dev57/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/index.rst` & `julearn-0.3.2.dev57/docs/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/links.inc` & `julearn-0.3.2.dev57/docs/links.inc`

 * *Files 4% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 .. _`setuptools_scm`: https://github.com/pypa/setuptools_scm/
 
 .. _`sphinx gallery`: https://sphinx-gallery.github.io/stable/index.html
 .. _`sphinx RST reference`: https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup
 
 
 .. _`DESlib`: https://github.com/scikit-learn-contrib/DESlib
+.. _`scikit-optimize`: https://scikit-optimize.readthedocs.io/en/stable/
```

### Comparing `julearn-0.3.2.dev24/docs/maintaining.rst` & `julearn-0.3.2.dev57/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.2.dev57/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.2.dev57/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/what_really_need_know/index.rst` & `julearn-0.3.2.dev57/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/docs/whats_new.rst` & `julearn-0.3.2.dev57/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.2.dev57/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/plot_example_regression.py` & `julearn-0.3.2.dev57/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.2.dev57/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.2.dev57/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.2.dev57/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.2.dev57/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.2.dev57/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.2.dev57/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.2.dev57/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.2.dev57/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.2.dev57/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.2.dev57/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.2.dev57/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.2.dev57/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.2.dev57/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.2.dev57/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.2.dev57/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.2.dev57/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.2.dev57/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_data_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_hyperparameters_docs.py`

 * *Files 15% similar despite different names*

```diff
@@ -239,30 +239,140 @@
 #
 # ``julearn`` uses the same concept as `scikit-learn`_ to tune hyperparameters:
 # it uses a *searcher* to find the best hyperparameter set. A searcher is an
 # object that receives a set of hyperparameters and their values, and then
 # tries to find the best combination of values for the hyperparameters using
 # cross-validation.
 #
-# By default, ``julearn`` uses a :class:`~sklearn.model_selection.GridSearchCV`.
-# This searcher is very simple. First, it construct the "grid" of
-# hyperparameters to try. As we see above, we have 3 hyperparameters to tune.
-# So it constructs a 3-dimentional grid with all the possible combinations of
-# the hyperparameters values. The second step is to perform cross-validation
-# on each of the possible combinations of hyperparameters values.
-#
-# Another searcher that ``julearn`` provides is the
-# :class:`~sklearn.model_selection.RandomizedSearchCV`. This searcher is
-# similar to the :class:`~sklearn.model_selection.GridSearchCV`, but instead
-# of trying all the possible combinations of hyperparameters values, it tries
+# By default, ``julearn`` uses a
+# :class:`~sklearn.model_selection.GridSearchCV`.
+# This searcher, specified as ``"grid"`` is very simple. First, it constructs
+# the _grid_ of hyperparameters to try. As we see above, we have 3
+# hyperparameters to tune. So it constructs a 3-dimentional grid with all the
+# possible combinations of the hyperparameters values. The second step is to
+# perform cross-validation on each of the possible combinations of
+# hyperparameters values.
+#
+# Other searchers that ``julearn`` provides are the
+# :class:`~sklearn.model_selection.RandomizedSearchCV` and
+# :class:`~skopt.BayesSearchCV`.
+#
+# The randomized searcher
+# (:class:`~sklearn.model_selection.RandomizedSearchCV`) is similar to the
+# :class:`~sklearn.model_selection.GridSearchCV`, but instead
+# of trying all the possible combinations of hyperparameter values, it tries
 # a random subset of them. This is useful when we have a lot of hyperparameters
-# to tune, since it can be very time consuming to try all the possible, as well
-# as continuous parameters that can be sampled out of a distribution. For
-# more information, see the
+# to tune, since it can be very time consuming to try all the possible
+# combinations, as well as continuous parameters that can be sampled out of a
+# distribution. For more information, see the
 # :class:`~sklearn.model_selection.RandomizedSearchCV` documentation.
+#
+# The Bayesian searcher (:class:`~skopt.BayesSearchCV`) is a bit more
+# complex. It uses Bayesian optimization to find the best hyperparameter set.
+# As with the randomized search, it is useful when we have many
+# hyperparameters to tune, and we don't want to try all the possible
+# combinations due to computational constraints. For more information, see the
+# :class:`~skopt.BayesSearchCV` documentation, including how to specify
+# the prior distributions of the hyperparameters.
+#
+# We can specify the kind of searcher and its parametrization, by setting the
+# ``search_params`` parameter in the :func:`.run_cross_validation` function.
+# For example, we can use the
+# :class:`~sklearn.model_selection.RandomizedSearchCV` searcher with
+# 10 iterations of random search.
+
+search_params = {
+    "kind": "random",
+    "n_iter": 10,
+}
+
+scores_tuned, model_tuned = run_cross_validation(
+    X=X,
+    y=y,
+    data=df,
+    X_types=X_types,
+    model=creator,
+    return_estimator="all",
+    search_params=search_params,
+)
+
+print(
+    "Scores with best hyperparameter using 10 iterations of "
+    f"randomized search: {scores_tuned['test_score'].mean()}"
+)
+pprint(model_tuned.best_params_)
+
+###############################################################################
+# We can now see that the best hyperparameter might be different from the grid
+# search. This is because it tried only 10 combinations and not the whole grid.
+# Furthermore, the  :class:`~sklearn.model_selection.RandomizedSearchCV`
+# searcher can sample hyperparameters from distributions, which can be useful
+# when we have continuous hyperparameters.
+# Let's set both ``C`` and ``gamma`` to be sampled from log-uniform
+# distributions. We can do this by setting the hyperparameter values as a
+# tuple with the following format: ``(low, high, distribution)``. The
+# distribution can be either ``"log-uniform"`` or ``"uniform"``.
+
+creator = PipelineCreator(problem_type="classification")
+creator.add("zscore")
+creator.add("select_k", k=[2, 3, 4])
+creator.add(
+    "svm",
+    C=(0.01, 10, "log-uniform"),
+    gamma=(1e-3, 1e-1, "log-uniform"),
+)
+
+print(creator)
+
+scores_tuned, model_tuned = run_cross_validation(
+    X=X,
+    y=y,
+    data=df,
+    X_types=X_types,
+    model=creator,
+    return_estimator="all",
+    search_params=search_params,
+)
+
+print(
+    "Scores with best hyperparameter using 10 iterations of "
+    f"randomized search: {scores_tuned['test_score'].mean()}"
+)
+pprint(model_tuned.best_params_)
+
+
+###############################################################################
+# We can also control the number of cross-validation folds used by the searcher
+# by setting the ``cv`` parameter in the ``search_params`` dictionary. For
+# example, we can use a bayesian search with 3 folds. Fortunately, the
+# :class:`~skopt.BayesSearchCV` searcher also accepts distributions for the
+# hyperparameters.
+
+search_params = {
+    "kind": "bayes",
+    "n_iter": 10,
+    "cv": 3,
+}
+
+scores_tuned, model_tuned = run_cross_validation(
+    X=X,
+    y=y,
+    data=df,
+    X_types=X_types,
+    model=creator,
+    return_estimator="all",
+    search_params=search_params,
+)
+
+print(
+    "Scores with best hyperparameter using 10 iterations of "
+    f"bayesian search and 3-fold CV: {scores_tuned['test_score'].mean()}"
+)
+pprint(model_tuned.best_params_)
+
 
 ###############################################################################
 #
 # Tuning more than one *grid*
 # ---------------------------
 #
 # Following our tuning of the :class:`~sklearn.svm.SVC` hyperparameters, we
```

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.2.dev57/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.2.dev57/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.2.dev57/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/api.py` & `julearn-0.3.2.dev57/julearn/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """API for julearn."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 
-from typing import Dict, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
-from sklearn.model_selection import check_cv, cross_validate
+from sklearn.model_selection import (
+    BaseCrossValidator,
+    check_cv,
+    cross_validate,
+)
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.pipeline import Pipeline
 
 from .inspect import Inspector
 from .pipeline import PipelineCreator
 from .pipeline.merger import merge_pipelines
 from .prepare import check_consistency, prepare_input_data
@@ -21,22 +25,22 @@
 from .utils import _compute_cvmdsum, logger, raise_error
 
 
 def run_cross_validation(  # noqa: C901
     X: List[str],  # noqa: N803
     y: str,
     model: Union[str, PipelineCreator, BaseEstimator, List[PipelineCreator]],
+    data: pd.DataFrame,
     X_types: Optional[Dict] = None,  # noqa: N803
-    data: Optional[pd.DataFrame] = None,
     problem_type: Optional[str] = None,
     preprocess: Union[None, str, List[str]] = None,
     return_estimator: Optional[str] = None,
     return_inspector: bool = False,
     return_train_score: bool = False,
-    cv: Optional[int] = None,
+    cv: Optional[Union[int, BaseCrossValidator, Iterable]] = None,
     groups: Optional[str] = None,
     scoring: Union[str, List[str], None] = None,
     pos_labels: Union[str, List[str], None] = None,
     model_params: Optional[Dict] = None,
     search_params: Optional[Dict] = None,
     seed: Optional[int] = None,
     n_jobs: Optional[int] = None,
@@ -50,20 +54,19 @@
         The features to use.
         See :ref:`data_usage` for details.
     y : str
         The targets to predict.
         See :ref:`data_usage` for details.
     model : str or scikit-learn compatible model.
         If string, it will use one of the available models.
+    data : pandas.DataFrame
+        DataFrame with the data. See :ref:`data_usage` for details.
     X_types : dict[str, list of str]
         A dictionary containing keys with column type as a str and the
         columns of this column type as a list of str.
-    data : pandas.DataFrame | None
-        DataFrame with the data (optional).
-        See :ref:`data_usage` for details.
     problem_type : str
         The kind of problem to model.
 
         Options are:
 
         * "classification": Perform a classification
           in which the target (y) has categorical classes (default).
@@ -128,16 +131,16 @@
           performed.
 
     search_params : dict | None
         Additional parameters in case Hyperparameter Tuning is performed, with
         the following keys:
 
         * 'kind': The kind of search algorithm to use, e.g.:
-            'grid' or 'random'. Can be any valid julearn searcher name or
-            scikit-learn compatible searcher.
+            'grid', 'random' or 'bayes'. Can be any valid julearn searcher name
+            or scikit-learn compatible searcher.
         * 'cv': If a searcher is going to be used, the cross-validation
             splitting strategy to use. Defaults to same CV as for the model
             evaluation.
         * 'scoring': If a searcher is going to be used, the scoring metric to
             evaluate the performance.
 
         See :ref:`hp_tuning` for details.
@@ -192,15 +195,15 @@
     if seed is not None:
         # If a seed is passed, use it, otherwise do not do anything. User
         # might have set the seed outside of the library
         logger.info(f"Setting random seed to {seed}")
         np.random.seed(seed)
 
     # Interpret the input data and prepare it to be used with the library
-    df_X, y, df_groups, X_types = prepare_input_data(
+    df_X, df_y, df_groups, X_types = prepare_input_data(
         X=X,
         y=y,
         df=data,
         pos_labels=pos_labels,
         groups=groups,
         X_types=X_types,
     )
@@ -263,15 +266,15 @@
                 *all_pipelines, search_params=search_params
             )
         else:
             pipeline = all_pipelines[0]
 
         if has_target_transformer:
             if isinstance(pipeline, BaseSearchCV):
-                last_step = pipeline.estimator[-1]
+                last_step = pipeline.estimator[-1]  # type: ignore
             else:
                 last_step = pipeline[-1]
             if not last_step.can_inverse_transform():
                 wrap_score = True
         problem_type = model[0].problem_type
 
     elif not isinstance(model, (str, BaseEstimator)):
@@ -309,15 +312,15 @@
         else:
             model_name = model.__class__.__name__.lower()
             if any(x.startswith(f"{model_name}__") for x in model_params):
                 raise_error(
                     "Cannot use model_params with a model object. Use either "
                     "a string or a PipelineCreator"
                 )
-        pipeline_creator.add(step=model, **t_params)
+        pipeline_creator.add(step=model, **t_params)  # type: ignore
 
         # Check for extra model_params that are not used
         unused_params = []
         for t_param in model_params:
             used = False
             for step in pipeline_creator.steps:
                 if t_param.startswith(f"{step.name}__"):
@@ -342,74 +345,80 @@
     logger.info(f"\tProblem type: {problem_type}")
     logger.info(f"\tNumber of samples: {len(df_X)}")
     logger.info(f"\tNumber of features: {len(df_X.columns)}")
     logger.info("====================")
     logger.info("")
 
     if problem_type == "classification":
-        logger.info(f"\tNumber of classes: {len(np.unique(y))}")
-        logger.info(f"\tTarget type: {y.dtype}")
-        logger.info(f"\tClass distributions: {y.value_counts()}")
+        logger.info(f"\tNumber of classes: {len(np.unique(df_y))}")
+        logger.info(f"\tTarget type: {df_y.dtype}")
+        logger.info(f"\tClass distributions: {df_y.value_counts()}")
     elif problem_type == "regression":
-        logger.info(f"\tTarget type: {y.dtype}")
+        logger.info(f"\tTarget type: {df_y.dtype}")
 
     # Prepare cross validation
-    cv_outer = check_cv(cv, classifier=problem_type == "classification")
+    cv_outer = check_cv(
+        cv, classifier=problem_type == "classification"  # type: ignore
+    )
     logger.info(f"Using outer CV scheme {cv_outer}")
 
-    check_consistency(y, cv, groups, problem_type)
+    check_consistency(df_y, cv, groups, problem_type)  # type: ignore
 
     cv_return_estimator = return_estimator in ["cv", "all"]
     scoring = check_scoring(pipeline, scoring, wrap_score=wrap_score)
 
     cv_mdsum = _compute_cvmdsum(cv_outer)
     fit_params = {}
     if df_groups is not None:
         if isinstance(pipeline, BaseSearchCV):
             fit_params["groups"] = df_groups.values
     scores = cross_validate(
         pipeline,
         df_X,
-        y,
+        df_y,
         cv=cv_outer,
         scoring=scoring,
         groups=df_groups,
         return_estimator=cv_return_estimator,
         n_jobs=n_jobs,
         return_train_score=return_train_score,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore
         fit_params=fit_params,
     )
 
     n_repeats = getattr(cv_outer, "n_repeats", 1)
     n_folds = len(scores["fit_time"]) // n_repeats
 
     repeats = np.repeat(np.arange(n_repeats), n_folds)
     folds = np.tile(np.arange(n_folds), n_repeats)
 
     fold_sizes = np.array(
-        [list(map(len, x)) for x in cv_outer.split(df_X, y, groups=df_groups)]
+        [
+            list(map(len, x))
+            for x in cv_outer.split(df_X, df_y, groups=df_groups)
+        ]
     )
     scores["n_train"] = fold_sizes[:, 0]
     scores["n_test"] = fold_sizes[:, 1]
     scores["repeat"] = repeats
     scores["fold"] = folds
     scores["cv_mdsum"] = cv_mdsum
 
     scores_df = pd.DataFrame(scores)
     out = scores_df
     if return_estimator in ["final", "all"]:
-        pipeline.fit(df_X, y, **fit_params)
+        logger.info("Fitting final model")
+        pipeline.fit(df_X, df_y, **fit_params)
         out = scores_df, pipeline
 
     if return_inspector:
         inspector = Inspector(
             scores=scores_df,
             model=pipeline,
             X=df_X,
-            y=y,
+            y=df_y,
             groups=df_groups,
             cv=cv_outer,
         )
         out = scores_df, pipeline, inspector
 
     return out
```

### Comparing `julearn-0.3.2.dev24/julearn/base/column_types.py` & `julearn-0.3.2.dev57/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/base/estimators.py` & `julearn-0.3.2.dev57/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.2.dev57/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/base/tests/test_column_types.py` & `julearn-0.3.2.dev57/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/config.py` & `julearn-0.3.2.dev57/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/conftest.py` & `julearn-0.3.2.dev57/julearn/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,85 @@
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 import typing
 from copy import copy
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
-from pytest import FixtureRequest, fixture
+import pytest
+from pytest import FixtureRequest, fixture, mark
 from seaborn import load_dataset
 
 
+_filter_keys = {
+    "nodeps": "Test that runs without conditional dependencies only",
+}
+
+
+def pytest_configure(config: pytest.Config) -> None:
+    """Add a new marker to pytest.
+
+    Parameters
+    ----------
+    config : pytest.Config
+        The pytest configuration object.
+
+    """
+    # register your new marker to avoid warnings
+    for k, v in _filter_keys.items():
+        config.addinivalue_line("markers", f"{k}: {v}")
+
+
+def pytest_addoption(parser: pytest.Parser) -> None:
+    """Add a new filter option to pytest.
+
+    Parameters
+    ----------
+    parser : pytest.Parser
+        The pytest parser object.
+
+    """
+    # add your new filter option (you can name it whatever you want)
+    parser.addoption(
+        "--filter",
+        action="store",
+        help="Select tests based on markers.",
+    )
+
+
+def pytest_collection_modifyitems(
+    config: pytest.Config, items: List[pytest.Item]
+) -> None:
+    """Filter tests based on the key marker.
+
+    Parameters
+    ----------
+    config : pytest.Config
+        The pytest configuration object.
+    items : list
+        The list of items.
+
+    """
+    filter = config.getoption("--filter", None)  # type: ignore
+    if filter is None:
+        for k in _filter_keys.keys():
+            skip_keys = mark.skip(
+                reason=f"Filter not specified for this test: {k}"
+            )
+            for item in items:
+                if k in item.keywords:
+                    item.add_marker(skip_keys)  # skip the test
+    else:
+        new_items = []
+        for item in items:
+            if filter in item.keywords:
+                new_items.append(item)
+        items[:] = new_items
+
+
 @fixture(scope="function")
 def df_typed_iris() -> pd.DataFrame:
     """Return a typed iris dataset.
 
     Returns
     -------
     df : pd.DataFrame
@@ -187,14 +254,40 @@
 
     Returns
     -------
     dict or None
         A dictionary with the search_params argument.
 
     """
+
+    return request.param
+
+
+@fixture(
+    params=[
+        {"kind": "bayes", "n_iter": 2, "cv": 3},
+        {"kind": "bayes", "n_iter": 2},
+    ],
+    scope="function",
+)
+def bayes_search_params(request: FixtureRequest) -> Optional[Dict]:
+    """Return different  search_params argument for BayesSearchCV.
+
+    Parameters
+    ----------
+    request : pytest.FixtureRequest
+        The request object.
+
+    Returns
+    -------
+    dict or None
+        A dictionary with the search_params argument.
+
+    """
+
     return request.param
 
 
 _tuning_params = {
     "zscore": {"with_mean": [True, False]},
     "pca": {"n_components": [0.2, 0.7]},
     "select_univariate": {"mode": ["k_best", "percentile"]},
@@ -230,14 +323,54 @@
 
         """
         return copy(_tuning_params.get(step, {}))
 
     return get
 
 
+_tuning_distributions = {
+    "zscore": {"with_mean": [True, False]},
+    "pca": {"n_components": (0.2, 0.7, "uniform")},
+    "select_univariate": {"mode": ["k_best", "percentile"]},
+    "rf": {"n_estimators": [2, 5]},
+    "svm": {"C": (1, 10, "log-uniform")},
+    "ridge": {"alpha": (1, 3, "uniform")},
+}
+
+
+@fixture(scope="function")
+def get_tuning_distributions() -> Callable:
+    """Return a function that returns the distributions to tune.
+
+    Returns
+    -------
+    get : callable
+        A function that returns the distributions to tune for a given step.
+
+    """
+
+    def get(step: str) -> Dict:
+        """Return the distributions to tune for a given step.
+
+        Parameters
+        ----------
+        step : str
+            The name of the step.
+
+        Returns
+        -------
+        dict
+            The distributions to tune for the given step.
+
+        """
+        return copy(_tuning_distributions.get(step, {}))
+
+    return get
+
+
 @fixture(
     params=[
         "zscore",
         ["zscore"],
         ["pca"],
         ["select_univariate"],
         ["zscore", "pca"],
```

### Comparing `julearn-0.3.2.dev24/julearn/inspect/_cv.py` & `julearn-0.3.2.dev57/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/inspect/_pipeline.py` & `julearn-0.3.2.dev57/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/inspect/_preprocess.py` & `julearn-0.3.2.dev57/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/inspect/inspector.py` & `julearn-0.3.2.dev57/julearn/inspect/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
+import pandas as pd
+from sklearn.model_selection import BaseCrossValidator
+
 from ..utils.logging import raise_error
 from ._cv import FoldsInspector
 from ._pipeline import PipelineInspector
 
 
 if TYPE_CHECKING:
-    import pandas as pd
+
     from sklearn.base import BaseEstimator
 
     from ..pipeline.pipeline_creator import PipelineCreator
 
 
 class Inspector:
     """Base class for inspector.
@@ -44,18 +47,18 @@
         model: Union[
             str,
             "PipelineCreator",
             List["PipelineCreator"],
             "BaseEstimator",
             None,
         ] = None,
-        X: Optional[List[str]] = None,  # noqa: N803
-        y: Optional[str] = None,
-        groups: Optional[str] = None,
-        cv: Optional[int] = None,
+        X: Optional[pd.DataFrame] = None,  # noqa: N803
+        y: Optional[pd.Series] = None,
+        groups: Optional[pd.Series] = None,
+        cv: Optional[Union[int, BaseCrossValidator]] = None,
     ) -> None:
         self._scores = scores
         self._model = model
         self._X = X
         self._y = y
         self._groups = groups
         self._cv = cv
```

### Comparing `julearn-0.3.2.dev24/julearn/inspect/tests/test_cv.py` & `julearn-0.3.2.dev57/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.2.dev57/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.2.dev57/julearn/inspect/tests/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from julearn.transformers import JuColumnTransformer
 
 
 if TYPE_CHECKING:
     import pandas as pd
 
 
-class TestEst(BaseEstimator):
+class MockTestEst(BaseEstimator):
     """Class for estimator tests.
 
     Parameters
     ----------
     hype_0 : int
         First hyperparameter.
     hype_1 : int
@@ -38,29 +38,29 @@
         self.hype_1 = hype_1
 
     def fit(
         self,
         X: List[str],  # noqa: N803
         y: Optional[str] = None,
         **fit_params: Any,
-    ) -> "TestEst":
+    ) -> "MockTestEst":
         """Fit the estimator.
 
         Parameters
         ----------
         X : list of str
             The features to use.
         y : str, optional
             The target to use (default None).
         **fit_params : dict
             Parameters for fitting the estimator.
 
         Returns
         -------
-        TestEst
+        MockTestEst
             The fitted estimator.
 
         """
         self.param_0_ = 0
         self.param_1_ = 1
         return self
 
@@ -151,17 +151,17 @@
         step_est = inspector.get_step(name=steps[i], as_estimator=as_estimator)
         assert isinstance(step_est, returns[i].__class__)
 
 
 @pytest.mark.parametrize(
     "est,fitted_params",
     [
-        [TestEst(), {"param_0_": 0, "param_1_": 1}],
+        [MockTestEst(), {"param_0_": 0, "param_1_": 1}],
         [
-            JuColumnTransformer("test", TestEst(), "continuous"),
+            JuColumnTransformer("test", MockTestEst(), "continuous"),
             {"param_0_": 0, "param_1_": 1},
         ],
     ],
 )
 def test_inspect_estimator(
     est: Type, fitted_params: Dict[str, int], df_iris: "pd.DataFrame"
 ) -> None:
@@ -197,15 +197,15 @@
     expected_fitted_params = {
         "jucolumntransformer__param_0_": 0,
         "jucolumntransformer__param_1_": 1,
     }
 
     pipe = (
         PipelineCreator(problem_type="classification")
-        .add(JuColumnTransformer("test", TestEst(), "continuous"))
+        .add(JuColumnTransformer("test", MockTestEst(), "continuous"))
         .add(SVC())
         .to_pipeline()
     )
     pipe.fit(df_iris.iloc[:, :-1], df_iris.species)
     inspector = PipelineInspector(pipe)
     inspect_params = inspector.get_fitted_params()
     inspect_params.pop("jucolumntransformer__column_transformer_", None)
@@ -226,15 +226,15 @@
     ----------
     df_iris : pd.DataFrame
         The iris dataset.
 
     """
     pipe = (
         PipelineCreator(problem_type="classification")
-        .add(JuColumnTransformer("test", TestEst(), "continuous"))
+        .add(JuColumnTransformer("test", MockTestEst(), "continuous"))
         .add(SVC())
         .to_pipeline()
     )
     pipe.fit(df_iris.iloc[:, :-1], df_iris.species)
     inspector = PipelineInspector(pipe)
     svc = inspector.get_step("svc").estimator
     assert isinstance(svc, SVC)
```

### Comparing `julearn-0.3.2.dev24/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.2.dev57/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.2.dev57/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.2.dev57/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.2.dev57/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.2.dev57/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/models/available_models.py` & `julearn-0.3.2.dev57/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/models/dynamic.py` & `julearn-0.3.2.dev57/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/models/tests/test_available_models.py` & `julearn-0.3.2.dev57/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/models/tests/test_dynamic.py` & `julearn-0.3.2.dev57/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/models/tests/test_models.py` & `julearn-0.3.2.dev57/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.2.dev57/julearn/pipeline/pipeline_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
-from sklearn.model_selection import check_cv
+from scipy import stats
+from sklearn.model_selection import RandomizedSearchCV, check_cv
 from sklearn.pipeline import Pipeline
 
 from ..base import ColumnTypes, ColumnTypesLike, JuTransformer, WrapModel
 from ..model_selection.available_searchers import get_searcher, list_searchers
 from ..models import get_model, list_models
 from ..prepare import prepare_search_params
 from ..transformers import (
@@ -247,14 +248,18 @@
             ):
                 if len(vals) > 1:
                     logger.info(f"Tuning hyperparameter {param} = {vals}")
                     params_to_tune[param] = vals
                 else:
                     logger.info(f"Setting hyperparameter {param} = {vals[0]}")
                     params_to_set[param] = vals[0]
+            elif hasattr(vals, "rvs"):
+                # If it is a distribution, we will tune it.
+                logger.info(f"Tuning hyperparameter {param} = {vals}")
+                params_to_tune[param] = vals
             else:
                 logger.info(f"Setting hyperparameter {param} = {vals}")
                 params_to_set[param] = vals
 
         # Build the estimator for this step
         if isinstance(step, str):
             step = self._get_estimator_from(
@@ -697,15 +702,16 @@
                 self._added_target_transformer = True
         elif self._is_model_step(step):
             self._added_model = True
         else:
             raise_error(f"Cannot add a {step}. I don't know what it is.")
 
     def _check_X_types(
-        self, X_types: Optional[Dict] = None  # noqa: N803
+        self,
+        X_types: Optional[Dict] = None,  # noqa: N803
     ) -> Dict[str, List[str]]:
         """Check the X_types against the pipeline creator settings.
 
         Parameters
         ----------
         X_types : dict, optional
             The types of the columns in the data.
@@ -781,15 +787,17 @@
         return False
 
     @staticmethod
     def _is_model_step(step: Union[EstimatorLike, str]) -> bool:
         """Check if a step is a model."""
         if step in list_models():
             return True
-        if hasattr(step, "fit") and hasattr(step, "predict"):
+        if hasattr(step, "fit") and (
+            hasattr(step, "predict") or hasattr(step, "score")
+        ):
             return True
         return False
 
     @staticmethod
     def _wrap_step(
         name, step, column_types, row_select_col_type, row_select_vals
     ) -> JuColumnTransformer:
@@ -851,14 +859,49 @@
             return get_model(name, problem_type, **kwargs)
         raise_error(
             f"{name} is neither a registered transformer"
             "nor a registered model."
         )
 
 
+def _prepare_hyperparameters_distributions(
+    params_to_tune: Dict[str, Any],
+) -> Dict[str, Any]:
+    """Prepare hyperparameters distributions for RandomizedSearchCV.
+
+    This method replaces tuples with distributions for RandomizedSearchCV
+    following the skopt convention. That is, if a parameter is a tuple
+    with 3 elements, the first two elements are the bounds of the
+    distribution and the third element is the type of distribution.
+
+    Parameters
+    ----------
+    params_to_tune : dict
+        The parameters to tune.
+
+    Returns
+    -------
+    dict
+        The modified parameters to tune.
+
+    """
+    mod_params_to_tune = {}
+    for k, v in params_to_tune.items():
+        if isinstance(v, tuple) and len(v) == 3:
+            if v[2] == "uniform":
+                mod_params_to_tune[k] = stats.uniform(v[0], v[1])
+            elif v[2] in ("loguniform", "log-uniform"):
+                mod_params_to_tune[k] = stats.loguniform(v[0], v[1])
+            else:
+                mod_params_to_tune[k] = v
+        else:
+            mod_params_to_tune[k] = v
+    return mod_params_to_tune
+
+
 def _prepare_hyperparameter_tuning(
     params_to_tune: Union[Dict[str, Any], List[Dict[str, Any]]],
     search_params: Optional[Dict[str, Any]],
     pipeline: Pipeline,
 ):
     """Prepare hyperparameter tuning in the pipeline.
 
@@ -872,15 +915,16 @@
         the 'svm' step. The value of the parameter must be a list of
         values to test.
 
     search_params : dict
         The parameters for the search. The following keys are accepted:
 
         * 'kind': The kind of search algorithm to use e.g.:
-            'grid' or 'random'. All valid julearn searchers can be entered.
+            'grid', 'random' or 'bayes'. All valid julearn searchers can be
+            entered.
         * 'cv': If search is going to be used, the cross-validation
             splitting strategy to use. Defaults to same CV as for the model
             evaluation.
         * 'scoring': If search is going to be used, the scoring metric to
             evaluate the performance.
 
     pipeline : sklearn.pipeline.Pipeline
@@ -925,14 +969,28 @@
         else:
             logger.info("Hyperparameters list:")
             for i_list, t_params in enumerate(params_to_tune):
                 logger.info(f"\tSet {i_list}")
                 for k, v in t_params.items():
                     logger.info(f"\t\t{k}: {v}")
 
+        if search == RandomizedSearchCV:
+            # If we are using RandomizedSearchCV, we can adopt the
+            # skopt convention of using a 3-element tuple to define
+            # the distributions.
+            if isinstance(params_to_tune, dict):
+                params_to_tune = _prepare_hyperparameters_distributions(
+                    params_to_tune
+                )
+            else:
+                params_to_tune = [
+                    _prepare_hyperparameters_distributions(p)
+                    for p in params_to_tune
+                ]
+
         cv_inner = check_cv(cv_inner)  # type: ignore
         logger.info(f"Using inner CV scheme {cv_inner}")
         search_params["cv"] = cv_inner
         logger.info("Search Parameters:")
         for k, v in search_params.items():
             logger.info(f"\t{k}: {v}")
```

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/target_pipeline.py` & `julearn-0.3.2.dev57/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.2.dev57/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/test/test_merger.py` & `julearn-0.3.2.dev57/julearn/pipeline/tests/test_merger.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,24 +70,24 @@
     with pytest.raises(ValueError, match="Only pipelines and searchers"):
         merge_pipelines(pipe1, SVC(), search_params=None)
 
     search_params = {"kind": "random"}
 
     with pytest.raises(
         ValueError,
-        match="At least one of the pipelines to merge is a GridSearchCV",
+        match="One of the pipelines to merge is a GridSearchCV",
     ):
         merge_pipelines(pipe1, pipe2, search_params=search_params)
 
     search_params = {"kind": "grid"}
     pipe2 = creator2.to_pipeline(search_params={"kind": "random"})
 
     with pytest.raises(
         ValueError,
-        match="one of the pipelines to merge is a RandomizedSearchCV",
+        match="One of the pipelines to merge is a RandomizedSearchCV",
     ):
         merge_pipelines(pipe1, pipe2, search_params=search_params)
 
     pipe3 = GridSearchCV(SVC(), param_grid={"C": [1, 10]})
     with pytest.raises(
         ValueError,
         match="All searchers must use a pipeline.",
@@ -100,7 +100,16 @@
     creator4.add("rf", n_estimators=[10, 100])
     pipe4 = creator4.to_pipeline(search_params={"kind": "grid"})
     with pytest.raises(
         ValueError,
         match="must have the same named steps.",
     ):
         merge_pipelines(pipe1, pipe4, search_params=None)
+
+    search_params = {"kind": "grid"}
+    pipe5 = creator2.to_pipeline(search_params={"kind": "bayes"})
+
+    with pytest.raises(
+        ValueError,
+        match="One of the pipelines to merge is a BayesSearchCV",
+    ):
+        merge_pipelines(pipe1, pipe5, search_params=search_params)
```

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/test/test_pipeline_creator.py` & `julearn-0.3.2.dev57/julearn/pipeline/tests/test_pipeline_creator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provides tests for the pipeline creator module."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 # License: AGPL
 
 import warnings
-from typing import Callable, Dict, List, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Tuple, Union
 
 import pandas as pd
 import pytest
 from sklearn.dummy import DummyClassifier
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
 from sklearn.preprocessing import RobustScaler, StandardScaler
@@ -18,14 +18,18 @@
 from julearn.base import ColumnTypesLike, WrapModel
 from julearn.models import get_model
 from julearn.pipeline import PipelineCreator, TargetPipelineCreator
 from julearn.pipeline.pipeline_creator import JuColumnTransformer
 from julearn.transformers import get_transformer
 
 
+if TYPE_CHECKING:
+    from sklearn.pipeline import Pipeline
+
+
 def test_construction_working(
     model: str, preprocess: Union[str, List[str]], problem_type: str
 ) -> None:
     """Test that the pipeline constructions works as expected.
 
     Parameters
     ----------
@@ -96,22 +100,22 @@
     )
     creator.add(model)
     pipeline = creator.to_pipeline({})
     pipeline.fit(X_iris, y_iris)
     pipeline[:-1].transform(X_iris)
 
 
-def test_hyperparameter_tuning(
+def _hyperparam_tuning_base_test(
     X_types_iris: Dict[str, List[str]],  # noqa: N803
     model: str,
     preprocess: Union[str, List[str]],
     problem_type: str,
     get_tuning_params: Callable,
     search_params: Dict[str, List],
-) -> None:
+) -> Tuple["Pipeline", Dict]:
     """Test that the pipeline hyperparameter tuning works as expected.
 
     Parameters
     ----------
     X_types_iris : dict
         The iris dataset features types.
     model : str
@@ -121,14 +125,22 @@
     problem_type : str
         The problem type to test.
     get_tuning_params : Callable
         A function that returns the tuning hyperparameters for a given step.
     search_params : dict of str and list
         The parameters for the search.
 
+    Returns
+    -------
+    pipeline : Pipeline
+        The pipeline created.
+    param_grid : dict
+        The parameter grid for the search, using scikit-learn's
+        convention.
+
     """
     if isinstance(preprocess, str):
         preprocess = [preprocess]
 
     creator = PipelineCreator(problem_type=problem_type)
     param_grid = {}
 
@@ -151,23 +163,226 @@
     param_grid.update(
         {f"{model}__{param}": val for param, val in model_params.items()}
     )
     pipeline = creator.to_pipeline(
         X_types=X_types_iris, search_params=search_params
     )
 
+    return pipeline, param_grid
+
+
+def test_hyperparameter_tuning(
+    X_types_iris: Dict[str, List[str]],  # noqa: N803
+    model: str,
+    preprocess: Union[str, List[str]],
+    problem_type: str,
+    get_tuning_params: Callable,
+    search_params: Dict[str, List],
+) -> None:
+    """Test that the pipeline hyperparameter tuning works as expected.
+
+    Parameters
+    ----------
+    X_types_iris : dict
+        The iris dataset features types.
+    model : str
+        The model to test.
+    preprocess : str or list of str
+        The preprocessing steps to test.
+    problem_type : str
+        The problem type to test.
+    get_tuning_params : Callable
+        A function that returns the tuning hyperparameters for a given step.
+    search_params : dict of str and list
+        The parameters for the search.
+
+
+    """
+
+    pipeline, param_grid = _hyperparam_tuning_base_test(
+        X_types_iris,
+        model,
+        preprocess,
+        problem_type,
+        get_tuning_params,
+        search_params,
+    )
     kind = "grid"
     if search_params is not None:
         kind = search_params.get("kind", "grid")
+
     if kind == "grid":
         assert isinstance(pipeline, GridSearchCV)
-        assert pipeline.param_grid == param_grid
+        assert pipeline.param_grid == param_grid  # type: ignore
     else:
+        assert kind == "random"
         assert isinstance(pipeline, RandomizedSearchCV)
-        assert pipeline.param_distributions == param_grid
+        assert pipeline.param_distributions == param_grid  # type: ignore
+
+
+def test_hyperparameter_tuning_bayes(
+    X_types_iris: Dict[str, List[str]],  # noqa: N803
+    model: str,
+    preprocess: Union[str, List[str]],
+    problem_type: str,
+    get_tuning_params: Callable,
+    bayes_search_params: Dict[str, List],
+) -> None:
+    """Test that the pipeline hyperparameter tuning works as expected.
+
+    Parameters
+    ----------
+    X_types_iris : dict
+        The iris dataset features types.
+    model : str
+        The model to test.
+    preprocess : str or list of str
+        The preprocessing steps to test.
+    problem_type : str
+        The problem type to test.
+    get_tuning_params : Callable
+        A function that returns the tuning hyperparameters for a given step.
+    bayes_search_params : dict of str and list
+        The parameters for the search.
+
+    """
+    BayesSearchCV = pytest.importorskip("skopt.BayesSearchCV")
+
+    pipeline, param_grid = _hyperparam_tuning_base_test(
+        X_types_iris,
+        model,
+        preprocess,
+        problem_type,
+        get_tuning_params,
+        bayes_search_params,
+    )
+    assert isinstance(pipeline, BayesSearchCV)
+    assert pipeline.search_spaces == param_grid  # type: ignore
+
+
+def _compare_param_grids(a: Dict, b: Dict) -> None:
+    """Compare two param grids.
+
+    Parameters
+    ----------
+    a : dict
+        The first param grid (processed).
+    b : dict
+        The second param grid (raw).
+
+    Raises
+    ------
+    AssertionError
+        If the param grids are not equal.
+
+    """
+    for key, val in a.items():
+        assert key in b
+        if hasattr(val, "rvs"):
+            assert val.args[0] == b[key][0]
+            assert val.args[1] == b[key][1]
+            if b[key][2] in ["log-uniform", "loguniform"]:
+                assert val.dist.name == "loguniform"
+            elif b[key][2] == "uniform":
+                assert val.dist.name == "uniform"
+            else:
+                pytest.fail(
+                    f"Unknown distributions {val.dist.name} or {b[key][2]}"
+                )
+        else:
+            assert val == b[key]
+
+
+def test_hyperparameter_tuning_distributions(
+    X_types_iris: Dict[str, List[str]],  # noqa: N803
+    model: str,
+    preprocess: Union[str, List[str]],
+    problem_type: str,
+    get_tuning_distributions: Callable,
+    search_params: Dict[str, List],
+) -> None:
+    """Test hyperparameter tuning using distributions.
+
+    Parameters
+    ----------
+    X_types_iris : dict
+        The iris dataset features types.
+    model : str
+        The model to test.
+    preprocess : str or list of str
+        The preprocessing steps to test.
+    problem_type : str
+        The problem type to test.
+    get_tuning_distributions : Callable
+        A function that returns the tuning hyperparameters for a given step.
+    search_params : dict of str and list
+        The parameters for the search.
+
+    """
+    kind = "grid"
+    if search_params is not None:
+        kind = search_params.get("kind", "grid")
+    if kind != "random":
+        return  # No sense to test distributions for other than gridsearch
+
+    pipeline, param_grid = _hyperparam_tuning_base_test(
+        X_types_iris,
+        model,
+        preprocess,
+        problem_type,
+        get_tuning_distributions,
+        search_params,
+    )
+
+    assert isinstance(pipeline, RandomizedSearchCV)
+    _compare_param_grids(
+        pipeline.param_distributions,  # type: ignore
+        param_grid,
+    )
+
+
+def test_hyperparameter_tuning_distributions_bayes(
+    X_types_iris: Dict[str, List[str]],  # noqa: N803
+    model: str,
+    preprocess: Union[str, List[str]],
+    problem_type: str,
+    get_tuning_distributions: Callable,
+    bayes_search_params: Dict[str, List],
+) -> None:
+    """Test BayesSearchCV hyperparameter tuning using distributions.
+
+    Parameters
+    ----------
+    X_types_iris : dict
+        The iris dataset features types.
+    model : str
+        The model to test.
+    preprocess : str or list of str
+        The preprocessing steps to test.
+    problem_type : str
+        The problem type to test.
+    get_tuning_distributions : Callable
+        A function that returns the tuning hyperparameters for a given step.
+    bayes_search_params : dict of str and list
+        The parameters for the search.
+
+    """
+    BayesSearchCV = pytest.importorskip("skopt.BayesSearchCV")
+
+    pipeline, param_grid = _hyperparam_tuning_base_test(
+        X_types_iris,
+        model,
+        preprocess,
+        problem_type,
+        get_tuning_distributions,
+        bayes_search_params,
+    )
+
+    assert isinstance(pipeline, BayesSearchCV)
+    _compare_param_grids(pipeline.search_spaces, param_grid)
 
 
 @pytest.mark.parametrize(
     "X_types,apply_to,warns",
     [
         ({"duck": "B"}, ["duck", "chicken"], True),
         ({"duck": "B"}, ["duck"], False),
@@ -293,15 +508,16 @@
     assert pipeline_creator._added_target_transformer
     assert pipeline_creator._added_model is False
     pipeline_creator.add("rf")
     assert pipeline_creator._added_model
 
 
 def test_stacking(
-    X_iris: pd.DataFrame, y_iris: pd.Series  # noqa: N803
+    X_iris: pd.DataFrame,  # noqa: N803
+    y_iris: pd.Series,
 ) -> None:
     """Test that the stacking model works correctly."""
     # Define our feature types
     X_types = {
         "sepal": ["sepal_length", "sepal_width"],
         "petal": ["petal_length", "petal_width"],
     }
@@ -574,19 +790,26 @@
     creator1.add("dummy", strategy="uniform", name="dummy")
 
     model1 = creator1.to_pipeline()
 
     assert model1.steps[-1][1].get_params()["strategy"] == "uniform"
 
     creator2 = PipelineCreator(problem_type="classification", apply_to="*")
-    creator2.add(DummyClassifier(strategy="uniform"), name="dummy")
+    creator2.add(
+        DummyClassifier(strategy="uniform"),  # type: ignore
+        name="dummy",
+    )
 
     model2 = creator2.to_pipeline()
 
     assert model2.steps[-1][1].get_params()["strategy"] == "uniform"
 
     creator3 = PipelineCreator(problem_type="classification", apply_to="*")
-    creator3.add(DummyClassifier(), strategy="uniform", name="dummy")
+    creator3.add(
+        DummyClassifier(),  # type: ignore
+        strategy="uniform",
+        name="dummy",
+    )
 
     model3 = creator3.to_pipeline()
 
     assert model3.steps[-1][1].get_params()["strategy"] == "uniform"
```

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline.py` & `julearn-0.3.2.dev57/julearn/pipeline/tests/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/pipeline/test/test_target_pipeline_creator.py` & `julearn-0.3.2.dev57/julearn/pipeline/tests/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/prepare.py` & `julearn-0.3.2.dev57/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/scoring/available_scorers.py` & `julearn-0.3.2.dev57/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/scoring/metrics.py` & `julearn-0.3.2.dev57/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.2.dev57/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.2.dev57/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/stats/corrected_ttest.py` & `julearn-0.3.2.dev57/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.2.dev57/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/tests/test_api.py` & `julearn-0.3.2.dev57/julearn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/tests/test_config.py` & `julearn-0.3.2.dev57/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/tests/test_prepare.py` & `julearn-0.3.2.dev57/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/__init__.py` & `julearn-0.3.2.dev57/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/available_transformers.py` & `julearn-0.3.2.dev57/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/cbpm.py` & `julearn-0.3.2.dev57/julearn/transformers/cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/confound_remover.py` & `julearn-0.3.2.dev57/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.2.dev57/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.2.dev57/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/__init__.py` & `julearn-0.3.2.dev57/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.2.dev57/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.2.dev57/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.2.dev57/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.2.dev57/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.2.dev57/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.2.dev57/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.2.dev57/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.2.dev57/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.2.dev57/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.2.dev57/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.2.dev57/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/_cv.py` & `julearn-0.3.2.dev57/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/checks.py` & `julearn-0.3.2.dev57/julearn/utils/checks.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/logging.py` & `julearn-0.3.2.dev57/julearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/testing.py` & `julearn-0.3.2.dev57/julearn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/tests/test_logging.py` & `julearn-0.3.2.dev57/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/tests/test_version.py` & `julearn-0.3.2.dev57/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/typing.py` & `julearn-0.3.2.dev57/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/utils/versions.py` & `julearn-0.3.2.dev57/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/viz/_scores.py` & `julearn-0.3.2.dev57/julearn/viz/_scores.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.2.dev57/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev24/julearn.egg-info/PKG-INFO` & `julearn-0.3.2.dev57/julearn.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev24
+Version: 0.3.2.dev57
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -36,20 +36,25 @@
 Requires-Dist: seaborn<0.13,>=0.12.2; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15,>=0.13.0; extra == "docs"
 Requires-Dist: furo<2024.0.0,>=2022.9.29; extra == "docs"
 Requires-Dist: sphinx_copybutton<0.6,>=0.5.0; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: towncrier<24; extra == "docs"
+Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "docs"
 Provides-Extra: deslib
 Requires-Dist: deslib<0.4,>=0.3.5; extra == "deslib"
 Provides-Extra: viz
 Requires-Dist: panel>=1.3.0; extra == "viz"
 Requires-Dist: bokeh>=3.0.0; extra == "viz"
 Requires-Dist: param>=2.0.0; extra == "viz"
+Provides-Extra: skopt
+Requires-Dist: scikit-optimize<0.11,>=0.10.0; extra == "skopt"
+Provides-Extra: all
+Requires-Dist: julearn[skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
```

### Comparing `julearn-0.3.2.dev24/julearn.egg-info/SOURCES.txt` & `julearn-0.3.2.dev57/julearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 docs/changes/contributors.inc
 docs/changes/newsfragments/.gitignore
 docs/changes/newsfragments/224.misc
 docs/changes/newsfragments/244.misc
 docs/changes/newsfragments/249.bugfix
 docs/changes/newsfragments/251.misc
 docs/changes/newsfragments/255.bugfix
+docs/changes/newsfragments/260.enh
+docs/changes/newsfragments/260.misc
 docs/images/corrected_ttest.png
 docs/images/final_estimator.png
 docs/images/iris_X.png
 docs/images/iris_df.png
 docs/images/iris_y.png
 docs/images/julearn_logo.png
 docs/images/julearn_logo_calm.png
@@ -107,14 +109,15 @@
 examples/02_inspection/plot_preprocess.py
 examples/02_inspection/run_binary_inspect_folds.py
 examples/03_complex_models/README.rst
 examples/03_complex_models/run_apply_to_target.py
 examples/03_complex_models/run_example_pca_featsets.py
 examples/03_complex_models/run_hyperparameter_multiple_grids.py
 examples/03_complex_models/run_hyperparameter_tuning.py
+examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
 examples/03_complex_models/run_stacked_models.py
 examples/04_confounds/README.rst
 examples/04_confounds/plot_confound_removal_classification.py
 examples/04_confounds/run_return_confounds.py
 examples/05_customization/README.rst
 examples/05_customization/run_custom_scorers_regression.py
 examples/99_docs/README.rst
@@ -153,14 +156,15 @@
 julearn/inspect/_preprocess.py
 julearn/inspect/inspector.py
 julearn/inspect/tests/test_cv.py
 julearn/inspect/tests/test_inspector.py
 julearn/inspect/tests/test_pipeline.py
 julearn/inspect/tests/test_preprocess.py
 julearn/model_selection/__init__.py
+julearn/model_selection/_skopt_searcher.py
 julearn/model_selection/available_searchers.py
 julearn/model_selection/continuous_stratified_kfold.py
 julearn/model_selection/stratified_bootstrap.py
 julearn/model_selection/tests/test_available_searchers.py
 julearn/model_selection/tests/test_continous_stratified_kfold.py
 julearn/model_selection/tests/test_stratified_bootstrap.py
 julearn/models/__init__.py
@@ -170,18 +174,18 @@
 julearn/models/tests/test_dynamic.py
 julearn/models/tests/test_models.py
 julearn/pipeline/__init__.py
 julearn/pipeline/merger.py
 julearn/pipeline/pipeline_creator.py
 julearn/pipeline/target_pipeline.py
 julearn/pipeline/target_pipeline_creator.py
-julearn/pipeline/test/test_merger.py
-julearn/pipeline/test/test_pipeline_creator.py
-julearn/pipeline/test/test_target_pipeline.py
-julearn/pipeline/test/test_target_pipeline_creator.py
+julearn/pipeline/tests/test_merger.py
+julearn/pipeline/tests/test_pipeline_creator.py
+julearn/pipeline/tests/test_target_pipeline.py
+julearn/pipeline/tests/test_target_pipeline_creator.py
 julearn/scoring/__init__.py
 julearn/scoring/available_scorers.py
 julearn/scoring/metrics.py
 julearn/scoring/tests/test_available_scorers.py
 julearn/scoring/tests/test_metrics.py
 julearn/stats/__init__.py
 julearn/stats/corrected_ttest.py
```

### Comparing `julearn-0.3.2.dev24/pyproject.toml` & `julearn-0.3.2.dev57/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -55,22 +55,29 @@
     "seaborn>=0.12.2,<0.13",
     "sphinx>=5.3.0,<7.3",
     "sphinx-gallery>=0.13.0,<0.15",
     "furo>=2022.9.29,<2024.0.0",
     "sphinx_copybutton>=0.5.0,<0.6",
     "numpydoc>=1.5.0,<1.6",
     "towncrier<24",
+    "scikit-optimize>=0.10.0,<0.11",
 ]
 deslib = ["deslib>=0.3.5,<0.4"]
 viz = [
     "panel>=1.3.0",
     "bokeh>=3.0.0",
     "param>=2.0.0",
 ]
 
+skopt = ["scikit-optimize>=0.10.0,<0.11"]
+
+# Add all optional functional dependencies (skip deslib until its fixed)
+# This does not include dev/docs building dependencies
+all = ["julearn[viz,skopt]"]
+
 ################
 # Tool configs #
 ################
 
 [tool.setuptools]
 packages = ["julearn"]
 
@@ -208,7 +215,11 @@
 name = "Enhancements"
 showcontent = true
 
 # Add custom towncrier fragment for API changes
 [tool.towncrier.fragment.change]
 name = "API Changes"
 showcontent = true
+
+## Configure pyright to ignore assigment types until scikit-learn stubs are updated
+[tool.pyright]
+reportAssignmentType = "none"
```

### Comparing `julearn-0.3.2.dev24/tox.ini` & `julearn-0.3.2.dev57/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tox]
-envlist = ruff, black, test, coverage, codespell, py3{8,9,10,11}
+envlist = ruff, black, test, coverage, codespell, py3{8,9,10,11}, nodeps
 isolated_build = true
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: coverage
-    3.11: py311
+    3.11: py311, nodeps
 
 [testenv]
 skip_install = false
 deps =
     pytest
     seaborn
+    scikit-optimize>=0.10.0,<0.11
 commands =
-    pytest
+    pytest {toxinidir}/julearn
 
 [testenv:ruff]
 skip_install = true
 deps =
     ruff
 commands =
     ruff check {toxinidir}
@@ -36,27 +37,37 @@
 deps =
     pytest
     seaborn
     deslib
     panel>=1.0.0b1
     bokeh>=3.0.0
     param
+    scikit-optimize>=0.10.0,<0.11
+commands =
+    pytest -vv {toxinidir}/julearn
+
+[testenv:nodeps]
+skip_install = false
+deps =
+    pytest
+    seaborn
 commands =
-    pytest -vv
+    pytest -vv --filter=nodeps {toxinidir}/julearn
 
 [testenv:coverage]
 skip_install = false
 deps =
     pytest
     pytest-cov
     seaborn
     deslib
     panel>=1.0.0b1
     bokeh>=3.0.0
     param
+    scikit-optimize>=0.10.0,<0.11
 commands =
     pytest --cov={envsitepackagesdir}/julearn --cov=./julearn --cov-report=xml --cov-report=term -vv
 
 [testenv:codespell]
 skip_install = true
 deps =
     codespell
```

