# Comparing `tmp/body_organ_analysis-0.1.2.tar.gz` & `tmp/body_organ_analysis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "body_organ_analysis-0.1.2.tar", max compression
+gzip compressed data, was "body_organ_analysis-0.1.3.tar", max compression
```

## Comparing `body_organ_analysis-0.1.2.tar` & `body_organ_analysis-0.1.3.tar`

### file list

```diff
@@ -1,360 +1,360 @@
--rw-r--r--   0        0        0    11357 2024-03-21 09:38:21.325338 body_organ_analysis-0.1.2/LICENSE
--rw-r--r--   0        0        0     3249 2024-03-21 09:38:21.325338 body_organ_analysis-0.1.2/README.md
--rw-r--r--   0        0        0      969 2024-03-21 09:38:21.325338 body_organ_analysis-0.1.2/body_organ_analysis/__init__.py
--rw-r--r--   0        0        0       78 2024-03-21 09:38:21.325338 body_organ_analysis-0.1.2/body_organ_analysis/__main__.py
--rw-r--r--   0        0        0      400 2024-03-21 09:38:21.325338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/__init__.py
--rw-r--r--   0        0        0       53 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/__main__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_parts/__init__.py
--rw-r--r--   0        0        0       79 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_parts/definition.py
--rw-r--r--   0        0        0     1581 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_parts/postprocess.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_regions/__init__.py
--rw-r--r--   0        0        0      268 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_regions/definition.py
--rw-r--r--   0        0        0     1523 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_regions/postprocess.py
--rw-r--r--   0        0        0     8494 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/commands.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/infer/__init__.py
--rw-r--r--   0        0        0     3809 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/infer/infer.py
--rw-r--r--   0        0        0     3199 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/io.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/__init__.py
--rw-r--r--   0        0        0    25204 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/builder.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/__init__.py
--rw-r--r--   0        0        0     2509 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/aggregation.py
--rw-r--r--   0        0        0     1299 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/check.py
--rw-r--r--   0        0        0     3864 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/colors.py
--rw-r--r--   0        0        0     3535 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/heatmaps.py
--rw-r--r--   0        0        0     7370 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/overview.py
--rw-r--r--   0        0        0     1327 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/build.py
--rw-r--r--   0        0        0      934 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.html.jinja
--rw-r--r--   0        0        0   351642 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.pdf
--rw-r--r--   0        0        0    45429 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.png
--rw-r--r--   0        0        0     4043 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.css
--rw-r--r--   0        0        0     3919 2024-03-21 09:38:21.329338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.sass
--rw-r--r--   0        0        0   446448 2024-03-21 09:38:21.333338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/boa+ship-ai.svg
--rw-r--r--   0        0        0   224452 2024-03-21 09:38:21.333338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   213168 2024-03-21 09:38:21.333338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-BoldItalic.ttf
--rw-r--r--   0        0        0   212760 2024-03-21 09:38:21.337338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Italic.ttf
--rw-r--r--   0        0        0   222236 2024-03-21 09:38:21.337338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Light.ttf
--rw-r--r--   0        0        0   213024 2024-03-21 09:38:21.337338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-LightItalic.ttf
--rw-r--r--   0        0        0   217276 2024-03-21 09:38:21.337338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0   170760 2024-03-21 09:38:21.341338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   174952 2024-03-21 09:38:21.341338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   173932 2024-03-21 09:38:21.341338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Italic.ttf
--rw-r--r--   0        0        0   170420 2024-03-21 09:38:21.341338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Light.ttf
--rw-r--r--   0        0        0   176616 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   171676 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Regular.ttf
--rw-r--r--   0        0        0      741 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/index.html.jinja
--rw-r--r--   0        0        0     3919 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ship-ai.svg
--rw-r--r--   0        0        0     8224 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ume.svg
--rw-r--r--   0        0        0     1701 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/bmd.html.jinja
--rw-r--r--   0        0        0     1302 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/equidistant_check.html.jinja
--rw-r--r--   0        0        0     3216 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_aggregated.html.jinja
--rw-r--r--   0        0        0     1552 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_total.html.jinja
--rw-r--r--   0        0        0      316 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/other_findings.html.jinja
--rw-r--r--   0        0        0      166 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/summary.html.jinja
--rw-r--r--   0        0        0      414 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/summary_totalsegmentator.html.jinja
--rw-r--r--   0        0        0      944 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/tissue_heatmaps.html.jinja
--rw-r--r--   0        0        0      899 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/report.html.jinja
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/tissue/__init__.py
--rw-r--r--   0        0        0      804 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/tissue/definition.py
--rw-r--r--   0        0        0     2314 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/tissue/subclassification.py
--rw-r--r--   0        0        0     2484 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/__init__.py
--rw-r--r--   0        0        0      274 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/configuration.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/__init__.py
--rw-r--r--   0        0        0     3277 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/add_dummy_task_with_mean_over_all_tasks.py
--rw-r--r--   0        0        0     2069 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/add_mean_dice_to_json.py
--rw-r--r--   0        0        0     2027 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/collect_results_files.py
--rw-r--r--   0        0        0    18123 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/evaluator.py
--rw-r--r--   0        0        0    13883 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/metrics.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/__init__.py
--rw-r--r--   0        0        0     3806 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py
--rw-r--r--   0        0        0     8322 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/ensemble.py
--rw-r--r--   0        0        0    15476 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/figure_out_what_to_submit.py
--rw-r--r--   0        0        0    15186 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates.py
--rw-r--r--   0        0        0     8651 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_StructSeg.py
--rw-r--r--   0        0        0     7989 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_cascade.py
--rw-r--r--   0        0        0    14240 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_in_one_json.py
--rw-r--r--   0        0        0     8132 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_with_plans.py
--rw-r--r--   0        0        0     4048 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/region_based_evaluation.py
--rw-r--r--   0        0        0     2697 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/surface_dice.py
--rw-r--r--   0        0        0    11552 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/DatasetAnalyzer.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/__init__.py
--rw-r--r--   0        0        0     6600 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py
--rw-r--r--   0        0        0     6510 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py
--rw-r--r--   0        0        0     6599 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py
--rw-r--r--   0        0        0     1963 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py
--rw-r--r--   0        0        0     3232 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py
--rw-r--r--   0        0        0     1349 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py
--rw-r--r--   0        0        0     2235 2024-03-21 09:38:21.345338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py
--rw-r--r--   0        0        0     7533 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/__init__.py
--rw-r--r--   0        0        0     1657 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py
--rw-r--r--   0        0        0     2070 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py
--rw-r--r--   0        0        0     1818 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/__init__.py
--rw-r--r--   0        0        0     6800 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py
--rw-r--r--   0        0        0     6088 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/__init__.py
--rw-r--r--   0        0        0     7464 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py
--rw-r--r--   0        0        0     6604 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py
--rw-r--r--   0        0        0      177 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/readme.md
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/__init__.py
--rw-r--r--   0        0        0     3680 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py
--rw-r--r--   0        0        0     1811 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py
--rw-r--r--   0        0        0    12852 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py
--rw-r--r--   0        0        0      515 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/change_batch_size.py
--rw-r--r--   0        0        0    11153 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/common_utils.py
--rw-r--r--   0        0        0     8810 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet.py
--rw-r--r--   0        0        0     5635 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py
--rw-r--r--   0        0        0    27225 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet.py
--rw-r--r--   0        0        0    10208 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py
--rw-r--r--   0        0        0     3562 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_convert_decathlon_task.py
--rw-r--r--   0        0        0     9921 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_plan_and_preprocess.py
--rw-r--r--   0        0        0     4666 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/summarize_plans.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/__init__.py
--rw-r--r--   0        0        0    10595 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py
--rw-r--r--   0        0        0    10162 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/utils.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/__init__.py
--rw-r--r--   0        0        0     2417 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/change_trainer.py
--rw-r--r--   0        0        0     6343 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/ensemble_predictions.py
--rw-r--r--   0        0        0    10201 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/inference_model.py
--rw-r--r--   0        0        0    44053 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/predict.py
--rw-r--r--   0        0        0    13043 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/predict_simple.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/pretrained_models/__init__.py
--rw-r--r--   0        0        0    14494 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/pretrained_models/collect_pretrained_models.py
--rw-r--r--   0        0        0    21688 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/pretrained_models/download_pretrained_model.py
--rw-r--r--   0        0        0    12543 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/segmentation_export.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/__init__.py
--rw-r--r--   0        0        0    13538 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/conv_blocks.py
--rw-r--r--   0        0        0     1547 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/feature_response_normalization.py
--rw-r--r--   0        0        0     1051 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/helperModules.py
--rw-r--r--   0        0        0      731 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/mish.py
--rw-r--r--   0        0        0    23579 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet.py
--rw-r--r--   0        0        0     7089 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet_DP.py
--rw-r--r--   0        0        0    20651 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_UNet.py
--rw-r--r--   0        0        0    28941 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_preact_residual_UNet.py
--rw-r--r--   0        0        0    25562 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_residual_UNet.py
--rw-r--r--   0        0        0     1793 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/initialization.py
--rw-r--r--   0        0        0    47188 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/neural_network.py
--rw-r--r--   0        0        0     3043 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/paths.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/__init__.py
--rw-r--r--   0        0        0    19722 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/connected_components.py
--rw-r--r--   0        0        0     3820 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_all_for_paper.py
--rw-r--r--   0        0        0     4895 2024-03-21 09:38:21.349338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing.py
--rw-r--r--   0        0        0     2734 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing_simple.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/__init__.py
--rw-r--r--   0        0        0     8969 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/cropping.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/__init__.py
--rw-r--r--   0        0        0     3437 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py
--rw-r--r--   0        0        0    50423 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/preprocessing.py
--rw-r--r--   0        0        0    12813 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/sanity_checks.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/__init__.py
--rw-r--r--   0        0        0     3974 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/default_configuration.py
--rw-r--r--   0        0        0     2649 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/load_pretrained_weights.py
--rw-r--r--   0        0        0    11226 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training.py
--rw-r--r--   0        0        0    10915 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training_DDP.py
--rw-r--r--   0        0        0    10756 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training_DP.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/__init__.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/cascade_stuff/__init__.py
--rw-r--r--   0        0        0     6628 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/cascade_stuff/predict_next_stage.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/__init__.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000.py
--rw-r--r--   0        0        0     1896 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py
--rw-r--r--   0        0        0     1896 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/__init__.py
--rw-r--r--   0        0        0     5029 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/custom_transforms.py
--rw-r--r--   0        0        0    12261 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA.py
--rw-r--r--   0        0        0    12409 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA2.py
--rw-r--r--   0        0        0    13631 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_moreDA.py
--rw-r--r--   0        0        0     5215 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_noDA.py
--rw-r--r--   0        0        0    14018 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/default_data_augmentation.py
--rw-r--r--   0        0        0     4335 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/downsampling.py
--rw-r--r--   0        0        0     9535 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/pyramid_augmentations.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/dataloading/__init__.py
--rw-r--r--   0        0        0    35206 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/dataloading/dataset_loading.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/learning_rate/__init__.py
--rw-r--r--   0        0        0      809 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/learning_rate/poly_lr.py
--rw-r--r--   0        0        0     1386 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/TopK_loss.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/__init__.py
--rw-r--r--   0        0        0      440 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/crossentropy.py
--rw-r--r--   0        0        0     1679 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/deep_supervision.py
--rw-r--r--   0        0        0    14272 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/dice_loss.py
--rw-r--r--   0        0        0     8000 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/focal_loss.py
--rw-r--r--   0        0        0     9068 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/model_restore.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/__init__.py
--rw-r--r--   0        0        0    22635 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py
--rw-r--r--   0        0        0    15709 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/__init__.py
--rwxr-xr-x   0        0        0     2764 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/__init__.py
--rw-r--r--   0        0        0      885 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_CascadeFullRes_nomirror.py
--rwxr-xr-x   0        0        0     3126 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_S5_D2_W32_LR_1e4_CropSize_192.py
--rw-r--r--   0        0        0      723 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca.py
--rw-r--r--   0        0        0      723 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca2.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000.py
--rw-r--r--   0        0        0     1896 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000_nomirror.py
--rw-r--r--   0        0        0      661 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250.py
--rw-r--r--   0        0        0     1894 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250_nomirror.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000.py
--rw-r--r--   0        0        0      731 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_AdamW.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_SGD.py
--rw-r--r--   0        0        0     1896 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py
--rw-r--r--   0        0        0      661 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep500.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000.py
--rw-r--r--   0        0        0     1896 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py
--rw-r--r--   0        0        0     1853 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_nomirror.py
--rw-r--r--   0        0        0    33232 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/network_trainer.py
--rw-r--r--   0        0        0    40817 2024-03-21 09:38:21.353338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainer.py
--rw-r--r--   0        0        0    16518 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerCascadeFullRes.py
--rw-r--r--   0        0        0     4816 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerNoDA.py
--rw-r--r--   0        0        0    22343 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2.py
--rw-r--r--   0        0        0    20254 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
--rw-r--r--   0        0        0    35724 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DDP.py
--rw-r--r--   0        0        0    12191 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DP.py
--rw-r--r--   0        0        0     1389 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_fp32.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/__init__.py
--rw-r--r--   0        0        0     2402 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py
--rw-r--r--   0        0        0     2345 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py
--rw-r--r--   0        0        0     2604 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py
--rw-r--r--   0        0        0     2570 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py
--rw-r--r--   0        0        0     2510 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py
--rw-r--r--   0        0        0     2960 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py
--rw-r--r--   0        0        0     2352 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py
--rw-r--r--   0        0        0     2358 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py
--rw-r--r--   0        0        0     2387 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py
--rw-r--r--   0        0        0     1460 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py
--rw-r--r--   0        0        0     2311 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py
--rw-r--r--   0        0        0     2365 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py
--rw-r--r--   0        0        0     2392 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py
--rw-r--r--   0        0        0     5556 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py
--rw-r--r--   0        0        0     5513 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py
--rw-r--r--   0        0        0     2268 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py
--rw-r--r--   0        0        0     1584 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py
--rw-r--r--   0        0        0    20817 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py
--rw-r--r--   0        0        0     2858 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py
--rw-r--r--   0        0        0     2395 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py
--rw-r--r--   0        0        0     2425 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py
--rw-r--r--   0        0        0     9080 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py
--rw-r--r--   0        0        0     6301 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/__init__.py
--rw-r--r--   0        0        0    14605 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py
--rw-r--r--   0        0        0     7166 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/__init__.py
--rw-r--r--   0        0        0     4401 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py
--rw-r--r--   0        0        0     1489 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py
--rw-r--r--   0        0        0     1492 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py
--rw-r--r--   0        0        0     1531 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/__init__.py
--rw-r--r--   0        0        0     3182 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/__init__.py
--rw-r--r--   0        0        0     1181 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py
--rw-r--r--   0        0        0    10263 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py
--rw-r--r--   0        0        0    21366 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py
--rw-r--r--   0        0        0      976 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py
--rw-r--r--   0        0        0     7759 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py
--rw-r--r--   0        0        0     8200 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py
--rw-r--r--   0        0        0     2420 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/__init__.py
--rw-r--r--   0        0        0     1344 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py
--rw-r--r--   0        0        0     1345 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py
--rw-r--r--   0        0        0     1440 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py
--rw-r--r--   0        0        0     1517 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py
--rw-r--r--   0        0        0     2465 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py
--rw-r--r--   0        0        0     1536 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py
--rw-r--r--   0        0        0     1531 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py
--rw-r--r--   0        0        0     2077 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py
--rw-r--r--   0        0        0     1727 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py
--rw-r--r--   0        0        0     2388 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py
--rw-r--r--   0        0        0     1677 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py
--rw-r--r--   0        0        0     1657 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py
--rw-r--r--   0        0        0     2914 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/__init__.py
--rw-r--r--   0        0        0     9948 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py
--rw-r--r--   0        0        0     1447 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py
--rw-r--r--   0        0        0     4816 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/__init__.py
--rw-r--r--   0        0        0     1303 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py
--rw-r--r--   0        0        0     3108 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py
--rw-r--r--   0        0        0     1419 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py
--rw-r--r--   0        0        0     1695 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py
--rw-r--r--   0        0        0     1695 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py
--rw-r--r--   0        0        0     1695 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py
--rw-r--r--   0        0        0     2888 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py
--rw-r--r--   0        0        0     1972 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py
--rw-r--r--   0        0        0     2144 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py
--rw-r--r--   0        0        0     1937 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py
--rw-r--r--   0        0        0     4145 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py
--rw-r--r--   0        0        0     1370 2024-03-21 09:38:21.357338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py
--rw-r--r--   0        0        0     1222 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py
--rw-r--r--   0        0        0     1224 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py
--rw-r--r--   0        0        0     1224 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py
--rw-r--r--   0        0        0     1323 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py
--rw-r--r--   0        0        0     2028 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py
--rw-r--r--   0        0        0     1920 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/__init__.py
--rw-r--r--   0        0        0     3368 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/optimizer/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/optimizer/ranger.py
--rw-r--r--   0        0        0       55 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/__init__.py
--rw-r--r--   0        0        0     3176 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/distributed.py
--rw-r--r--   0        0        0     4631 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/file_conversions.py
--rw-r--r--   0        0        0     1130 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/file_endings.py
--rw-r--r--   0        0        0     1810 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/folder_names.py
--rw-r--r--   0        0        0     4538 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/image_reorientation.py
--rw-r--r--   0        0        0      800 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/nd_softmax.py
--rw-r--r--   0        0        0      990 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/one_hot_encoding.py
--rw-r--r--   0        0        0     8877 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/overlay_plots.py
--rw-r--r--   0        0        0      794 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/random_stuff.py
--rw-r--r--   0        0        0     1548 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/recursive_delete_npz.py
--rw-r--r--   0        0        0     1770 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/recursive_rename_taskXX_to_taskXXX.py
--rw-r--r--   0        0        0     1524 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/set_n_proc_DA.py
--rw-r--r--   0        0        0      908 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/sitk_stuff.py
--rw-r--r--   0        0        0     3599 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/task_name_id_conversion.py
--rw-r--r--   0        0        0     1604 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/tensor_utilities.py
--rw-r--r--   0        0        0     1175 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/to_torch.py
--rw-r--r--   0        0        0    13214 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/TotalSegmentator.py
--rw-r--r--   0        0        0     4809 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/alignment.py
--rw-r--r--   0        0        0     5009 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/cropping.py
--rw-r--r--   0        0        0      262 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/download_pretrained_weights.py
--rw-r--r--   0        0        0    13274 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/libs.py
--rw-r--r--   0        0        0    20934 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/map_to_binary.py
--rw-r--r--   0        0        0     3031 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/nifti_ext_header.py
--rw-r--r--   0        0        0    23039 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/nnunet.py
--rw-r--r--   0        0        0     4032 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/postprocessing.py
--rw-r--r--   0        0        0     8876 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/preview.py
--rw-r--r--   0        0        0     9357 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/resampling.py
--rw-r--r--   0        0        0     4392 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/statistics.py
--rw-r--r--   0        0        0     6959 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/store_models_as_onnx.py
--rw-r--r--   0        0        0     4513 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/task_info.py
--rw-r--r--   0        0        0     6305 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/vtk_utils.py
--rw-r--r--   0        0        0       93 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/_version.py
--rw-r--r--   0        0        0     5559 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/cli.py
--rw-r--r--   0        0        0     7212 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/commands.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/__init__.py
--rw-r--r--   0        0        0     3787 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/bca_metrics.py
--rw-r--r--   0        0        0      755 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/constants.py
--rw-r--r--   0        0        0     2854 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/geometry.py
--rw-r--r--   0        0        0     8438 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/inference.py
--rw-r--r--   0        0        0    11947 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/io.py
--rw-r--r--   0        0        0     8533 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/measurements.py
--rw-r--r--   0        0        0     5224 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/ts_metrics.py
--rw-r--r--   0        0        0     1015 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/compute/util.py
--rw-r--r--   0        0        0     1513 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/body-parts-meta.json
--rw-r--r--   0        0        0     6708 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/body-regions-meta.json
--rw-r--r--   0        0        0     1022 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/cerebral_bleed-meta.json
--rw-r--r--   0        0        0     1008 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/coronary_arteries-meta.json
--rw-r--r--   0        0        0     1011 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/covid-meta.json
--rw-r--r--   0        0        0      996 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/hip_implant-meta.json
--rw-r--r--   0        0        0     1524 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/liver_vessels-meta.json
--rw-r--r--   0        0        0     1534 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/lung_vessels_airways-meta.json
--rw-r--r--   0        0        0     2056 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/pleural_pericard_effusion-meta.json
--rw-r--r--   0        0        0     1025 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/pulmonary_fat-meta.json
--rw-r--r--   0        0        0     4475 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/tissues-meta.json
--rw-r--r--   0        0        0    54236 2024-03-21 09:38:21.361338 body_organ_analysis-0.1.2/body_organ_analysis/templates/total-meta.json
--rw-r--r--   0        0        0     2369 2024-03-21 09:38:21.413338 body_organ_analysis-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 body_organ_analysis-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3249 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/README.md
+-rw-r--r--   0        0        0      969 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/__main__.py
+-rw-r--r--   0        0        0      400 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_parts/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_parts/definition.py
+-rw-r--r--   0        0        0     1581 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_parts/postprocess.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_regions/__init__.py
+-rw-r--r--   0        0        0      268 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_regions/definition.py
+-rw-r--r--   0        0        0     1523 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_regions/postprocess.py
+-rw-r--r--   0        0        0     8494 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/commands.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/infer/__init__.py
+-rw-r--r--   0        0        0     3809 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/infer/infer.py
+-rw-r--r--   0        0        0     3199 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/io.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/__init__.py
+-rw-r--r--   0        0        0    25204 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/builder.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/aggregation.py
+-rw-r--r--   0        0        0     1299 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/check.py
+-rw-r--r--   0        0        0     3864 2024-04-29 13:37:10.396156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/colors.py
+-rw-r--r--   0        0        0     3535 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/heatmaps.py
+-rw-r--r--   0        0        0     7370 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/overview.py
+-rw-r--r--   0        0        0     1327 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/build.py
+-rw-r--r--   0        0        0      934 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.html.jinja
+-rw-r--r--   0        0        0   351642 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.pdf
+-rw-r--r--   0        0        0    45429 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.png
+-rw-r--r--   0        0        0     4043 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.css
+-rw-r--r--   0        0        0     3919 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.sass
+-rw-r--r--   0        0        0   446448 2024-04-29 13:37:10.400156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/boa+ship-ai.svg
+-rw-r--r--   0        0        0   224452 2024-04-29 13:37:10.404156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   213168 2024-04-29 13:37:10.404156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   212760 2024-04-29 13:37:10.404156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Italic.ttf
+-rw-r--r--   0        0        0   222236 2024-04-29 13:37:10.408156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Light.ttf
+-rw-r--r--   0        0        0   213024 2024-04-29 13:37:10.408156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-LightItalic.ttf
+-rw-r--r--   0        0        0   217276 2024-04-29 13:37:10.408156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0   170760 2024-04-29 13:37:10.408156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   174952 2024-04-29 13:37:10.412156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   173932 2024-04-29 13:37:10.412156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   170420 2024-04-29 13:37:10.412156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Light.ttf
+-rw-r--r--   0        0        0   176616 2024-04-29 13:37:10.412156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   171676 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Regular.ttf
+-rw-r--r--   0        0        0      741 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/index.html.jinja
+-rw-r--r--   0        0        0     3919 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ship-ai.svg
+-rw-r--r--   0        0        0     8224 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ume.svg
+-rw-r--r--   0        0        0     1701 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/bmd.html.jinja
+-rw-r--r--   0        0        0     1302 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/equidistant_check.html.jinja
+-rw-r--r--   0        0        0     3216 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_aggregated.html.jinja
+-rw-r--r--   0        0        0     1552 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_total.html.jinja
+-rw-r--r--   0        0        0      316 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/other_findings.html.jinja
+-rw-r--r--   0        0        0      166 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/summary.html.jinja
+-rw-r--r--   0        0        0      414 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/summary_totalsegmentator.html.jinja
+-rw-r--r--   0        0        0      944 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/tissue_heatmaps.html.jinja
+-rw-r--r--   0        0        0      899 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/report.html.jinja
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/tissue/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/tissue/definition.py
+-rw-r--r--   0        0        0     2314 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/tissue/subclassification.py
+-rw-r--r--   0        0        0     2484 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/configuration.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/__init__.py
+-rw-r--r--   0        0        0     3277 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/add_dummy_task_with_mean_over_all_tasks.py
+-rw-r--r--   0        0        0     2069 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/add_mean_dice_to_json.py
+-rw-r--r--   0        0        0     2027 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/collect_results_files.py
+-rw-r--r--   0        0        0    18123 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/evaluator.py
+-rw-r--r--   0        0        0    13883 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/metrics.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/__init__.py
+-rw-r--r--   0        0        0     3806 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py
+-rw-r--r--   0        0        0     8322 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/ensemble.py
+-rw-r--r--   0        0        0    15476 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/figure_out_what_to_submit.py
+-rw-r--r--   0        0        0    15186 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates.py
+-rw-r--r--   0        0        0     8651 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_StructSeg.py
+-rw-r--r--   0        0        0     7989 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_cascade.py
+-rw-r--r--   0        0        0    14240 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_in_one_json.py
+-rw-r--r--   0        0        0     8132 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_with_plans.py
+-rw-r--r--   0        0        0     4048 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/region_based_evaluation.py
+-rw-r--r--   0        0        0     2697 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/surface_dice.py
+-rw-r--r--   0        0        0    11552 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/DatasetAnalyzer.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py
+-rw-r--r--   0        0        0     6510 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py
+-rw-r--r--   0        0        0     6599 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py
+-rw-r--r--   0        0        0     1963 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py
+-rw-r--r--   0        0        0     3232 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py
+-rw-r--r--   0        0        0     1349 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py
+-rw-r--r--   0        0        0     2235 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py
+-rw-r--r--   0        0        0     7533 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py
+-rw-r--r--   0        0        0     2070 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py
+-rw-r--r--   0        0        0     1818 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/__init__.py
+-rw-r--r--   0        0        0     6800 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py
+-rw-r--r--   0        0        0     6088 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/__init__.py
+-rw-r--r--   0        0        0     7464 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py
+-rw-r--r--   0        0        0     6604 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py
+-rw-r--r--   0        0        0      177 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/readme.md
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/__init__.py
+-rw-r--r--   0        0        0     3680 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py
+-rw-r--r--   0        0        0     1811 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py
+-rw-r--r--   0        0        0    12852 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py
+-rw-r--r--   0        0        0      515 2024-04-29 13:37:10.416156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/change_batch_size.py
+-rw-r--r--   0        0        0    11153 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/common_utils.py
+-rw-r--r--   0        0        0     8810 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet.py
+-rw-r--r--   0        0        0     5635 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py
+-rw-r--r--   0        0        0    27225 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet.py
+-rw-r--r--   0        0        0    10208 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py
+-rw-r--r--   0        0        0     3562 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_convert_decathlon_task.py
+-rw-r--r--   0        0        0     9921 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_plan_and_preprocess.py
+-rw-r--r--   0        0        0     4666 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/summarize_plans.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/__init__.py
+-rw-r--r--   0        0        0    10595 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py
+-rw-r--r--   0        0        0    10162 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/utils.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/__init__.py
+-rw-r--r--   0        0        0     2417 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/change_trainer.py
+-rw-r--r--   0        0        0     6343 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/ensemble_predictions.py
+-rw-r--r--   0        0        0    10201 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/inference_model.py
+-rw-r--r--   0        0        0    44053 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/predict.py
+-rw-r--r--   0        0        0    13043 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/predict_simple.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/pretrained_models/__init__.py
+-rw-r--r--   0        0        0    14494 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/pretrained_models/collect_pretrained_models.py
+-rw-r--r--   0        0        0    21688 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/pretrained_models/download_pretrained_model.py
+-rw-r--r--   0        0        0    12543 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/segmentation_export.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/__init__.py
+-rw-r--r--   0        0        0    13538 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/conv_blocks.py
+-rw-r--r--   0        0        0     1547 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/feature_response_normalization.py
+-rw-r--r--   0        0        0     1051 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/helperModules.py
+-rw-r--r--   0        0        0      731 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/mish.py
+-rw-r--r--   0        0        0    23579 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet.py
+-rw-r--r--   0        0        0     7089 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet_DP.py
+-rw-r--r--   0        0        0    20651 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_UNet.py
+-rw-r--r--   0        0        0    28941 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_preact_residual_UNet.py
+-rw-r--r--   0        0        0    25562 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_residual_UNet.py
+-rw-r--r--   0        0        0     1793 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/initialization.py
+-rw-r--r--   0        0        0    47188 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/neural_network.py
+-rw-r--r--   0        0        0     3043 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/paths.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/__init__.py
+-rw-r--r--   0        0        0    19722 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/connected_components.py
+-rw-r--r--   0        0        0     3820 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_all_for_paper.py
+-rw-r--r--   0        0        0     4895 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing.py
+-rw-r--r--   0        0        0     2734 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing_simple.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/__init__.py
+-rw-r--r--   0        0        0     8969 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/cropping.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/__init__.py
+-rw-r--r--   0        0        0     3437 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py
+-rw-r--r--   0        0        0    50423 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/preprocessing.py
+-rw-r--r--   0        0        0    12813 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/sanity_checks.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/__init__.py
+-rw-r--r--   0        0        0     3974 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/default_configuration.py
+-rw-r--r--   0        0        0     2649 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/load_pretrained_weights.py
+-rw-r--r--   0        0        0    11226 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training.py
+-rw-r--r--   0        0        0    10915 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training_DDP.py
+-rw-r--r--   0        0        0    10756 2024-04-29 13:37:10.420156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training_DP.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/cascade_stuff/__init__.py
+-rw-r--r--   0        0        0     6628 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/cascade_stuff/predict_next_stage.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000.py
+-rw-r--r--   0        0        0     1896 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py
+-rw-r--r--   0        0        0     1896 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/__init__.py
+-rw-r--r--   0        0        0     5029 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/custom_transforms.py
+-rw-r--r--   0        0        0    12261 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA.py
+-rw-r--r--   0        0        0    12409 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA2.py
+-rw-r--r--   0        0        0    13631 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_moreDA.py
+-rw-r--r--   0        0        0     5215 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_noDA.py
+-rw-r--r--   0        0        0    14018 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/default_data_augmentation.py
+-rw-r--r--   0        0        0     4335 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/downsampling.py
+-rw-r--r--   0        0        0     9535 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/pyramid_augmentations.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/dataloading/__init__.py
+-rw-r--r--   0        0        0    35206 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/dataloading/dataset_loading.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/learning_rate/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/learning_rate/poly_lr.py
+-rw-r--r--   0        0        0     1386 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/TopK_loss.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/crossentropy.py
+-rw-r--r--   0        0        0     1679 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/deep_supervision.py
+-rw-r--r--   0        0        0    14272 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/dice_loss.py
+-rw-r--r--   0        0        0     8000 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/focal_loss.py
+-rw-r--r--   0        0        0     9068 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/model_restore.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/__init__.py
+-rw-r--r--   0        0        0    22635 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py
+-rw-r--r--   0        0        0    15709 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/__init__.py
+-rwxr-xr-x   0        0        0     2764 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_CascadeFullRes_nomirror.py
+-rwxr-xr-x   0        0        0     3126 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_S5_D2_W32_LR_1e4_CropSize_192.py
+-rw-r--r--   0        0        0      723 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca.py
+-rw-r--r--   0        0        0      723 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca2.py
+-rw-r--r--   0        0        0      663 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000.py
+-rw-r--r--   0        0        0     1896 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000_nomirror.py
+-rw-r--r--   0        0        0      661 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250.py
+-rw-r--r--   0        0        0     1894 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250_nomirror.py
+-rw-r--r--   0        0        0      663 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000.py
+-rw-r--r--   0        0        0      731 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_AdamW.py
+-rw-r--r--   0        0        0      663 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_SGD.py
+-rw-r--r--   0        0        0     1896 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py
+-rw-r--r--   0        0        0      661 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep500.py
+-rw-r--r--   0        0        0      663 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000.py
+-rw-r--r--   0        0        0     1896 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py
+-rw-r--r--   0        0        0     1853 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_nomirror.py
+-rw-r--r--   0        0        0    33232 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/network_trainer.py
+-rw-r--r--   0        0        0    40817 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainer.py
+-rw-r--r--   0        0        0    16518 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerCascadeFullRes.py
+-rw-r--r--   0        0        0     4816 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerNoDA.py
+-rw-r--r--   0        0        0    22343 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2.py
+-rw-r--r--   0        0        0    20254 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
+-rw-r--r--   0        0        0    35724 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DDP.py
+-rw-r--r--   0        0        0    12191 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DP.py
+-rw-r--r--   0        0        0     1389 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_fp32.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/__init__.py
+-rw-r--r--   0        0        0     2402 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py
+-rw-r--r--   0        0        0     2345 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py
+-rw-r--r--   0        0        0     2604 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py
+-rw-r--r--   0        0        0     2570 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py
+-rw-r--r--   0        0        0     2510 2024-04-29 13:37:10.424156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py
+-rw-r--r--   0        0        0     2960 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py
+-rw-r--r--   0        0        0     2352 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py
+-rw-r--r--   0        0        0     2358 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py
+-rw-r--r--   0        0        0     2387 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py
+-rw-r--r--   0        0        0     1460 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py
+-rw-r--r--   0        0        0     2311 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py
+-rw-r--r--   0        0        0     2365 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py
+-rw-r--r--   0        0        0     2392 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py
+-rw-r--r--   0        0        0     5556 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py
+-rw-r--r--   0        0        0     5513 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py
+-rw-r--r--   0        0        0     2268 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py
+-rw-r--r--   0        0        0     1584 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py
+-rw-r--r--   0        0        0    20817 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py
+-rw-r--r--   0        0        0     2858 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py
+-rw-r--r--   0        0        0     2395 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py
+-rw-r--r--   0        0        0     2425 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py
+-rw-r--r--   0        0        0     9080 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py
+-rw-r--r--   0        0        0     6301 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/__init__.py
+-rw-r--r--   0        0        0    14605 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py
+-rw-r--r--   0        0        0     7166 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/__init__.py
+-rw-r--r--   0        0        0     4401 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py
+-rw-r--r--   0        0        0     1489 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py
+-rw-r--r--   0        0        0     1492 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py
+-rw-r--r--   0        0        0     1531 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/__init__.py
+-rw-r--r--   0        0        0     3182 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/__init__.py
+-rw-r--r--   0        0        0     1181 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py
+-rw-r--r--   0        0        0    10263 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py
+-rw-r--r--   0        0        0    21366 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py
+-rw-r--r--   0        0        0      976 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py
+-rw-r--r--   0        0        0     7759 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py
+-rw-r--r--   0        0        0     8200 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py
+-rw-r--r--   0        0        0     2420 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/__init__.py
+-rw-r--r--   0        0        0     1344 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py
+-rw-r--r--   0        0        0     1345 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py
+-rw-r--r--   0        0        0     1440 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py
+-rw-r--r--   0        0        0     1517 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py
+-rw-r--r--   0        0        0     2465 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py
+-rw-r--r--   0        0        0     1536 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py
+-rw-r--r--   0        0        0     1531 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py
+-rw-r--r--   0        0        0     2077 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py
+-rw-r--r--   0        0        0     1727 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py
+-rw-r--r--   0        0        0     2388 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py
+-rw-r--r--   0        0        0     1677 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py
+-rw-r--r--   0        0        0     1657 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py
+-rw-r--r--   0        0        0     2914 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/__init__.py
+-rw-r--r--   0        0        0     9948 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py
+-rw-r--r--   0        0        0     1447 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py
+-rw-r--r--   0        0        0     4816 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py
+-rw-r--r--   0        0        0     3108 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py
+-rw-r--r--   0        0        0     1419 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py
+-rw-r--r--   0        0        0     1695 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py
+-rw-r--r--   0        0        0     1695 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py
+-rw-r--r--   0        0        0     1695 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py
+-rw-r--r--   0        0        0     2888 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py
+-rw-r--r--   0        0        0     1972 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py
+-rw-r--r--   0        0        0     2144 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py
+-rw-r--r--   0        0        0     1937 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py
+-rw-r--r--   0        0        0     4145 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py
+-rw-r--r--   0        0        0     1370 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py
+-rw-r--r--   0        0        0     1222 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py
+-rw-r--r--   0        0        0     1224 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py
+-rw-r--r--   0        0        0     1224 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py
+-rw-r--r--   0        0        0     1323 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py
+-rw-r--r--   0        0        0     2028 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py
+-rw-r--r--   0        0        0     1920 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/__init__.py
+-rw-r--r--   0        0        0     3368 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/optimizer/__init__.py
+-rw-r--r--   0        0        0     6940 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/optimizer/ranger.py
+-rw-r--r--   0        0        0       55 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/__init__.py
+-rw-r--r--   0        0        0     3176 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/distributed.py
+-rw-r--r--   0        0        0     4631 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/file_conversions.py
+-rw-r--r--   0        0        0     1130 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/file_endings.py
+-rw-r--r--   0        0        0     1810 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/folder_names.py
+-rw-r--r--   0        0        0     4538 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/image_reorientation.py
+-rw-r--r--   0        0        0      800 2024-04-29 13:37:10.428156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/nd_softmax.py
+-rw-r--r--   0        0        0      990 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/one_hot_encoding.py
+-rw-r--r--   0        0        0     8877 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/overlay_plots.py
+-rw-r--r--   0        0        0      794 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/random_stuff.py
+-rw-r--r--   0        0        0     1548 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/recursive_delete_npz.py
+-rw-r--r--   0        0        0     1770 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/recursive_rename_taskXX_to_taskXXX.py
+-rw-r--r--   0        0        0     1524 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/set_n_proc_DA.py
+-rw-r--r--   0        0        0      908 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/sitk_stuff.py
+-rw-r--r--   0        0        0     3599 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/task_name_id_conversion.py
+-rw-r--r--   0        0        0     1604 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/tensor_utilities.py
+-rw-r--r--   0        0        0     1175 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/to_torch.py
+-rw-r--r--   0        0        0    13214 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/TotalSegmentator.py
+-rw-r--r--   0        0        0     4809 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/__init__.py
+-rw-r--r--   0        0        0     2558 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/alignment.py
+-rw-r--r--   0        0        0     5009 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/cropping.py
+-rw-r--r--   0        0        0      262 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/download_pretrained_weights.py
+-rw-r--r--   0        0        0    13274 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/libs.py
+-rw-r--r--   0        0        0    20934 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/map_to_binary.py
+-rw-r--r--   0        0        0     3031 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/nifti_ext_header.py
+-rw-r--r--   0        0        0    23039 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/nnunet.py
+-rw-r--r--   0        0        0     4032 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/postprocessing.py
+-rw-r--r--   0        0        0     8876 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/preview.py
+-rw-r--r--   0        0        0     9357 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/resampling.py
+-rw-r--r--   0        0        0     4392 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/statistics.py
+-rw-r--r--   0        0        0     6959 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/store_models_as_onnx.py
+-rw-r--r--   0        0        0     4513 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/task_info.py
+-rw-r--r--   0        0        0     6305 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/vtk_utils.py
+-rw-r--r--   0        0        0       93 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/_version.py
+-rw-r--r--   0        0        0     5559 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/cli.py
+-rw-r--r--   0        0        0     7255 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/commands.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/bca_metrics.py
+-rw-r--r--   0        0        0      755 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/constants.py
+-rw-r--r--   0        0        0     2854 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/geometry.py
+-rw-r--r--   0        0        0     8460 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/inference.py
+-rw-r--r--   0        0        0    11947 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/io.py
+-rw-r--r--   0        0        0     8533 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/measurements.py
+-rw-r--r--   0        0        0     5224 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/ts_metrics.py
+-rw-r--r--   0        0        0     1015 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/compute/util.py
+-rw-r--r--   0        0        0     1513 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/body-parts-meta.json
+-rw-r--r--   0        0        0     6708 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/body-regions-meta.json
+-rw-r--r--   0        0        0     1022 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/cerebral_bleed-meta.json
+-rw-r--r--   0        0        0     1008 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/coronary_arteries-meta.json
+-rw-r--r--   0        0        0     1011 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/covid-meta.json
+-rw-r--r--   0        0        0      996 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/hip_implant-meta.json
+-rw-r--r--   0        0        0     1524 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/liver_vessels-meta.json
+-rw-r--r--   0        0        0     1534 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/lung_vessels_airways-meta.json
+-rw-r--r--   0        0        0     2056 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/pleural_pericard_effusion-meta.json
+-rw-r--r--   0        0        0     1025 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/pulmonary_fat-meta.json
+-rw-r--r--   0        0        0     4475 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/tissues-meta.json
+-rw-r--r--   0        0        0    54236 2024-04-29 13:37:10.432156 body_organ_analysis-0.1.3/body_organ_analysis/templates/total-meta.json
+-rw-r--r--   0        0        0     2369 2024-04-29 13:37:10.484156 body_organ_analysis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 body_organ_analysis-0.1.3/PKG-INFO
```

### Comparing `body_organ_analysis-0.1.2/LICENSE` & `body_organ_analysis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/README.md` & `body_organ_analysis-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/__init__.py` & `body_organ_analysis-0.1.3/body_organ_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_parts/postprocess.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_parts/postprocess.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/body_regions/postprocess.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/body_regions/postprocess.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/commands.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/commands.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/infer/infer.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/infer/infer.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/io.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/io.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/builder.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/builder.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/aggregation.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/aggregation.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/check.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/check.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/colors.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/colors.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/heatmaps.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/heatmaps.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/plots/overview.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/plots/overview.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/build.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/build.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.pdf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.pdf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.png` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/example/report.png`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.css` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.css`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.sass` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/_template_style.sass`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/boa+ship-ai.svg` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/boa+ship-ai.svg`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Bold.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-BoldItalic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Italic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Light.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-LightItalic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Regular.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Bold.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-BoldItalic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Italic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Light.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-LightItalic.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Regular.ttf` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/index.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/index.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ship-ai.svg` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ship-ai.svg`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ume.svg` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/base/template/ume.svg`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/bmd.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/bmd.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/equidistant_check.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/equidistant_check.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_aggregated.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_aggregated.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_total.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/measurements_total.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/tissue_heatmaps.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/blocks/tissue_heatmaps.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/report/template/report.html.jinja` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/report/template/report.html.jinja`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/tissue/definition.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/tissue/definition.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/body_composition_analysis/tissue/subclassification.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/body_composition_analysis/tissue/subclassification.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/__init__.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/add_dummy_task_with_mean_over_all_tasks.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/add_dummy_task_with_mean_over_all_tasks.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/add_mean_dice_to_json.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/add_mean_dice_to_json.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/collect_results_files.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/collect_results_files.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/evaluator.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/metrics.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/ensemble.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/ensemble.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/figure_out_what_to_submit.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/figure_out_what_to_submit.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_StructSeg.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_StructSeg.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_cascade.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/rank_candidates_cascade.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_in_one_json.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_in_one_json.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_with_plans.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/model_selection/summarize_results_with_plans.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/region_based_evaluation.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/region_based_evaluation.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/evaluation/surface_dice.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/evaluation/surface_dice.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/DatasetAnalyzer.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/DatasetAnalyzer.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/change_batch_size.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/change_batch_size.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/common_utils.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/common_utils.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_convert_decathlon_task.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_convert_decathlon_task.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_plan_and_preprocess.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/nnUNet_plan_and_preprocess.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/summarize_plans.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/summarize_plans.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/experiment_planning/utils.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/experiment_planning/utils.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/change_trainer.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/change_trainer.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/ensemble_predictions.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/ensemble_predictions.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/inference_model.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/inference_model.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/predict.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/predict.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/predict_simple.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/predict_simple.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/pretrained_models/collect_pretrained_models.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/pretrained_models/collect_pretrained_models.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/pretrained_models/download_pretrained_model.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/pretrained_models/download_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/inference/segmentation_export.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/inference/segmentation_export.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/conv_blocks.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/feature_response_normalization.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/feature_response_normalization.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/helperModules.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/helperModules.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/mish.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/custom_modules/mish.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet_DP.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_UNet_DP.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_UNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_UNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_preact_residual_UNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_preact_residual_UNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_residual_UNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/generic_modular_residual_UNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/initialization.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/initialization.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/network_architecture/neural_network.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/network_architecture/neural_network.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/paths.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/paths.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/connected_components.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/connected_components.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_all_for_paper.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_all_for_paper.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing_simple.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/postprocessing/consolidate_postprocessing_simple.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/cropping.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/cropping.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/preprocessing.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/preprocessing/sanity_checks.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/preprocessing/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/default_configuration.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/default_configuration.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/load_pretrained_weights.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/load_pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training_DDP.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training_DDP.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/run/run_training_DP.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/run/run_training_DP.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/cascade_stuff/predict_next_stage.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/cascade_stuff/predict_next_stage.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/custom_transforms.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_insaneDA2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_moreDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_moreDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_noDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/data_augmentation_noDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/default_data_augmentation.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/default_data_augmentation.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/downsampling.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/downsampling.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/data_augmentation/pyramid_augmentations.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/data_augmentation/pyramid_augmentations.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/dataloading/dataset_loading.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/dataloading/dataset_loading.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/learning_rate/poly_lr.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/learning_rate/poly_lr.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/TopK_loss.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/TopK_loss.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/deep_supervision.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/dice_loss.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/dice_loss.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/loss_functions/focal_loss.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/loss_functions/focal_loss.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/model_restore.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/model_restore.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_CascadeFullRes_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_CascadeFullRes_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_S5_D2_W32_LR_1e4_CropSize_192.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_S5_D2_W32_LR_1e4_CropSize_192.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_bca2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep2000_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep250_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_AdamW.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_AdamW.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_SGD.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_SGD.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep4000_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep500.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep500.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_ep8000_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_nomirror.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/custom_trainers/nnUNetTrainerV2_nomirror.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/network_trainer.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/network_trainer.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainer.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainer.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerCascadeFullRes.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerCascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerNoDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerNoDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DDP.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DDP.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DP.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_DP.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_fp32.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNetTrainerV2_fp32.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/training/optimizer/ranger.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/training/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/distributed.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/file_conversions.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/file_conversions.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/file_endings.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/file_endings.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/folder_names.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/folder_names.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/image_reorientation.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/image_reorientation.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/nd_softmax.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/nd_softmax.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/one_hot_encoding.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/overlay_plots.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/overlay_plots.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/random_stuff.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/random_stuff.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/recursive_delete_npz.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/recursive_delete_npz.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/recursive_rename_taskXX_to_taskXXX.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/recursive_rename_taskXX_to_taskXXX.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/set_n_proc_DA.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/set_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/sitk_stuff.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/sitk_stuff.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/task_name_id_conversion.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/task_name_id_conversion.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/tensor_utilities.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/tensor_utilities.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/nnunet/utilities/to_torch.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/nnunet/utilities/to_torch.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/TotalSegmentator.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/TotalSegmentator.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/__init__.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/__init__.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/alignment.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/alignment.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/cropping.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/cropping.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/libs.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/libs.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/map_to_binary.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/map_to_binary.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/nifti_ext_header.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/nifti_ext_header.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/nnunet.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/nnunet.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/postprocessing.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/postprocessing.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/preview.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/preview.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/resampling.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/resampling.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/statistics.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/statistics.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/store_models_as_onnx.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/store_models_as_onnx.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/task_info.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/task_info.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/_external/totalsegmentator/vtk_utils.py` & `body_organ_analysis-0.1.3/body_organ_analysis/_external/totalsegmentator/vtk_utils.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/cli.py` & `body_organ_analysis-0.1.3/body_organ_analysis/cli.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/commands.py` & `body_organ_analysis-0.1.3/body_organ_analysis/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     bca_median_filtering: bool = False,
     bca_examined_body_region: str = None,
     bca_pdf: bool = True,
     bca_compute_bmd: bool = False,
     keep_debug_information: bool = False,
     recompute: bool = False,
     nnunet_verbose: bool = False,
+    fast: bool = False,
 ) -> Tuple[Path, Dict]:
     start_total = time()
     ct_info: List[Dict] = []
     if input_folder.is_file() and ".nii" in input_folder.name:
         ct_path = input_folder
     else:
         ct_path, ct_info = get_image_info(
@@ -89,14 +90,15 @@
             median_filtering=bca_median_filtering,
             examined_body_region=bca_examined_body_region,
             save_pdf=bca_pdf,
             compute_bmd=bca_compute_bmd,
         ),
         keep_debug_segmentations=keep_debug_information,
         recompute=recompute,
+        fast=fast,
     )
     logger.info(f"All models computed: DONE in {time() - start:0.5f}s")
 
     stats["inference_time"] = time() - start
     stats.update(ct_stats)
 
     aggr_df, slices_df, slices_no_limbs_df, bmd_df = None, None, None, None
```

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/bca_metrics.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/bca_metrics.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/constants.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/constants.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/geometry.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/geometry.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/inference.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     segmentation_folder: pathlib.Path,
     models_to_compute: List[str],
     force_split_threshold: int = 400,
     totalsegmentator_params: Optional[Dict] = None,
     bca_params: Optional[Dict] = None,
     keep_debug_segmentations: bool = False,
     recompute: bool = True,
+    fast: bool = True,
 ) -> Dict[str, int]:
     totalsegmentator_params = totalsegmentator_params or {}
     totalsegmentator_params = totalsegmentator_params.copy()
     bca_params = bca_params or {}
     preview_param = totalsegmentator_params.get("preview", False)
     if "preview" in totalsegmentator_params:
         del totalsegmentator_params["preview"]
@@ -101,15 +102,15 @@
         ),
     }
 
     for chosen_task in [m for m in models_to_compute if m != "bca"]:
         logger.info(f"Computing segmentations for task {chosen_task}")
         task_specific_params = get_task_info(
             chosen_task,
-            fast=False,
+            fast=fast,
             multilabel_image=chosen_task not in {"lung_vessels", "body"},
             quiet=True,
         )
         if task_specific_params["multilabel_image"]:
             seg_output = segmentation_folder / f"{chosen_task}.nii.gz"
             if seg_output.exists() and not recompute:
                 logger.info("The segmentation was already computed, skipping...")
```

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/io.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/io.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/measurements.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/measurements.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/ts_metrics.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/ts_metrics.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/compute/util.py` & `body_organ_analysis-0.1.3/body_organ_analysis/compute/util.py`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/body-parts-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/body-parts-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/body-regions-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/body-regions-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/cerebral_bleed-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/cerebral_bleed-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/coronary_arteries-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/coronary_arteries-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/covid-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/covid-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/hip_implant-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/hip_implant-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/liver_vessels-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/liver_vessels-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/lung_vessels_airways-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/lung_vessels_airways-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/pleural_pericard_effusion-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/pleural_pericard_effusion-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/pulmonary_fat-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/pulmonary_fat-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/tissues-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/tissues-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/body_organ_analysis/templates/total-meta.json` & `body_organ_analysis-0.1.3/body_organ_analysis/templates/total-meta.json`

 * *Files identical despite different names*

### Comparing `body_organ_analysis-0.1.2/pyproject.toml` & `body_organ_analysis-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "body-organ-analysis"
-version = "0.1.2"
+version = "0.1.3"
 license = "Apache-2.0"
 description = "BOA is a tool for segmentation of CT scans developed by the SHIP-AI group at the Institute for Artificial Intelligence in Medicine (https://ship-ai.ikim.nrw/). Combining the TotalSegmentator and the Body Composition Analysis, this tool is capable of analyzing medical images and identifying the different structures within the human body, including bones, muscles, organs, and blood vessels."
 authors = ["Giulia Baldini <Giulia.Baldini@uk-essen.de>"]
 readme = "README.md"
 repository = "https://github.com/UMEssen/Body-and-Organ-Analyzer"
 keywords = ["python", "segmentation", "nnunet", "boa", "body composition analysis"]
 packages = [
```

### Comparing `body_organ_analysis-0.1.2/PKG-INFO` & `body_organ_analysis-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: body-organ-analysis
-Version: 0.1.2
+Version: 0.1.3
 Summary: BOA is a tool for segmentation of CT scans developed by the SHIP-AI group at the Institute for Artificial Intelligence in Medicine (https://ship-ai.ikim.nrw/). Combining the TotalSegmentator and the Body Composition Analysis, this tool is capable of analyzing medical images and identifying the different structures within the human body, including bones, muscles, organs, and blood vessels.
 Home-page: https://github.com/UMEssen/Body-and-Organ-Analyzer
 License: Apache-2.0
 Keywords: python,segmentation,nnunet,boa,body composition analysis
 Author: Giulia Baldini
 Author-email: Giulia.Baldini@uk-essen.de
 Requires-Python: >=3.8,<3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: body-organ-analysis Version: 0.1.2 Summary: BOA is
+Metadata-Version: 2.1 Name: body-organ-analysis Version: 0.1.3 Summary: BOA is
 a tool for segmentation of CT scans developed by the SHIP-AI group at the
 Institute for Artificial Intelligence in Medicine (https://ship-ai.ikim.nrw/).
 Combining the TotalSegmentator and the Body Composition Analysis, this tool is
 capable of analyzing medical images and identifying the different structures
 within the human body, including bones, muscles, organs, and blood vessels.
 Home-page: https://github.com/UMEssen/Body-and-Organ-Analyzer License: Apache-
 2.0 Keywords: python,segmentation,nnunet,boa,body composition analysis Author:
```

