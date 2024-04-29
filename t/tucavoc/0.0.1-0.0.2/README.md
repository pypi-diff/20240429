# Comparing `tmp/tucavoc-0.0.1.tar.gz` & `tmp/tucavoc-0.0.2.tar.gz`

## Comparing `tucavoc-0.0.1.tar` & `tucavoc-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,80 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tucavoc-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 tucavoc-0.0.1/create_executable.bash
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tucavoc-0.0.1/ovoc-calculations.code-workspace
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 tucavoc-0.0.1/start.bat
--rw-r--r--   0        0        0  1954427 2020-02-02 00:00:00.000000 tucavoc-0.0.1/data/TestData.dat
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tucavoc-0.0.1/data/settings_test.ini
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/make.bat
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/about.rst
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/api.rst
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/exports.rst
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/groups.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/install.rst
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/manual.rst
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/methodology.rst
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/sources.rst
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/equations/calibrationfactor.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/equations/readme.md
--rw-r--r--   0        0        0   194752 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/example_interpolation.png
--rw-r--r--   0        0        0    93129 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/python.png
--rw-r--r--   0        0        0    99853 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/python_next.png
--rw-r--r--   0        0        0   441016 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/stable_diffusion-3.png
--rw-r--r--   0        0        0   606809 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/stable_diffusion_.png
--rw-r--r--   0        0        0   643429 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/stable_diffusion_2.png
--rw-r--r--   0        0        0    55735 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/images/tucavoc_widget.png
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/Calibration.rst
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/Linearity.rst
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/Precision.rst
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/README.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/combined_standard_uncertainty.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/expanded_uncertainty.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/further_instrumental_problems.rst
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/instrument.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/peak_integration.rst
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/sampling_volume_accuracy.rst
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tucavoc-0.0.1/docs/source/uncertainties/volume.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 tucavoc-0.0.1/meteo_files/README.md
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/__main__.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/abstract_uncertainty.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/calculations.py
--rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/equations.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/flags.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/parameters.py
--rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/plots.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/station.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/tex.py
--rw-r--r--   0        0        0    14457 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/uncertainties.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/utils.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/additional_data/__init__.py
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/additional_data/empa.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/additional_data/station.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/additional_data/widget.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/__init__.py
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/ebas_genfile.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/ebas_test.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/empa_qa_tools.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/excel.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/test_exports.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/exports/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/__init__.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/main.spec
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/parameters.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/qsettings_selector.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/station.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/style_sheet.qss
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/substances.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/uncertainties.py
--rw-r--r--   0        0        0    13539 2020-02-02 00:00:00.000000 tucavoc-0.0.1/tucavoc/widgets/utils.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 tucavoc-0.0.1/.gitignore
--rw-r--r--   0        0        0    32759 2020-02-02 00:00:00.000000 tucavoc-0.0.1/LICENSE
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tucavoc-0.0.1/README.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 tucavoc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    38997 2020-02-02 00:00:00.000000 tucavoc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 tucavoc-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tucavoc-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 tucavoc-0.0.2/create_executable.bash
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tucavoc-0.0.2/ovoc-calculations.code-workspace
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tucavoc-0.0.2/start.bat
+-rw-r--r--   0        0        0  1954427 2020-02-02 00:00:00.000000 tucavoc-0.0.2/data/TestData.dat
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tucavoc-0.0.2/data/settings_test.ini
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/about.rst
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/api.rst
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/exports.rst
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/groups.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/install.rst
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/manual.rst
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/methodology.rst
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/sources.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/equations/readme.md
+-rw-r--r--   0        0        0   194752 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/example_interpolation.png
+-rw-r--r--   0        0        0    93129 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/python.png
+-rw-r--r--   0        0        0    99853 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/python_next.png
+-rw-r--r--   0        0        0   441016 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/stable_diffusion-3.png
+-rw-r--r--   0        0        0   606809 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/stable_diffusion_.png
+-rw-r--r--   0        0        0   643429 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/stable_diffusion_2.png
+-rw-r--r--   0        0        0    55735 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/images/tucavoc_widget.png
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/Calibration.rst
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/Linearity.rst
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/Precision.rst
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/Volume.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/combined_standard_uncertainty.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/expanded_uncertainty.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/further_instrumental_problems.rst
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/instrument.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/peak_integration.rst
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tucavoc-0.0.2/docs/source/uncertainties/sampling_volume_accuracy.rst
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tucavoc-0.0.2/examples/simple_calculation_with_uncertainties.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 tucavoc-0.0.2/meteo_files/README.md
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tests/test_calculation.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/__main__.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/abstract_uncertainty.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/calculations.py
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/equations.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/flags.py
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/parameters.py
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/plots.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/settings.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/station.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/tex.py
+-rw-r--r--   0        0        0    14457 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/uncertainties.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/utils.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/additional_data/__init__.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/additional_data/empa.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/additional_data/station.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/additional_data/widget.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/__init__.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/ebas_genfile.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/ebas_test.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/empa_qa_tools.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/excel.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/test_exports.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/exports/utils.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/testing/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/__main__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/parameters.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/qsettings_selector.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/station.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/style_sheet.qss
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/substances.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/uncertainties.py
+-rw-r--r--   0        0        0    13539 2020-02-02 00:00:00.000000 tucavoc-0.0.2/tucavoc/widgets/utils.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 tucavoc-0.0.2/.gitignore
+-rw-r--r--   0        0        0    32759 2020-02-02 00:00:00.000000 tucavoc-0.0.2/LICENSE
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tucavoc-0.0.2/README.md
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tucavoc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    39018 2020-02-02 00:00:00.000000 tucavoc-0.0.2/PKG-INFO
```

### Comparing `tucavoc-0.0.1/ovoc-calculations.code-workspace` & `tucavoc-0.0.2/ovoc-calculations.code-workspace`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,20 @@
 			"path": "..\\..\\AppData\\Local\\Programs\\Python\\Python310\\Lib\\site-packages\\ebas"
 		},
 		{
 			"path": "..\\outdir"
 		},
 		{
 			"path": "H:\\TUCAVOC"
-		},
-		{
-			"path": "../test_tucavoc_anja"
-		},
-		{
-			"path": "../test_volume_ovoc"
 		}
 	],
 	"settings": {
 
 		"[python]": {
-			"editor.wordBasedSuggestions": "off",
+			"editor.wordBasedSuggestions": false,
 			"editor.formatOnSave": true,
 		},
 		"editor.trimAutoWhitespace": true,
 		"python.formatting.provider": "black",
 		"python.formatting.blackArgs": ["-l 79","--experimental-string-processing"],
 		"python.linting.pylintEnabled": false,
 		"python.linting.pylintArgs": [
```

### Comparing `tucavoc-0.0.1/data/TestData.dat` & `tucavoc-0.0.2/data/TestData.dat`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/Makefile` & `tucavoc-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/make.bat` & `tucavoc-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/about.rst` & `tucavoc-0.0.2/docs/source/about.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/api.rst` & `tucavoc-0.0.2/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/conf.py` & `tucavoc-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/exports.rst` & `tucavoc-0.0.2/docs/source/exports.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/groups.rst` & `tucavoc-0.0.2/docs/source/groups.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/index.rst` & `tucavoc-0.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/install.rst` & `tucavoc-0.0.2/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/manual.rst` & `tucavoc-0.0.2/docs/source/manual.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/methodology.rst` & `tucavoc-0.0.2/docs/source/methodology.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/sources.rst` & `tucavoc-0.0.2/docs/source/sources.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/example_interpolation.png` & `tucavoc-0.0.2/docs/source/images/example_interpolation.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/python.png` & `tucavoc-0.0.2/docs/source/images/python.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/python_next.png` & `tucavoc-0.0.2/docs/source/images/python_next.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/stable_diffusion-3.png` & `tucavoc-0.0.2/docs/source/images/stable_diffusion-3.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/stable_diffusion_.png` & `tucavoc-0.0.2/docs/source/images/stable_diffusion_.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/stable_diffusion_2.png` & `tucavoc-0.0.2/docs/source/images/stable_diffusion_2.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/images/tucavoc_widget.png` & `tucavoc-0.0.2/docs/source/images/tucavoc_widget.png`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/uncertainties/sampling_volume_accuracy.rst` & `tucavoc-0.0.2/docs/source/uncertainties/sampling_volume_accuracy.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/docs/source/uncertainties/volume.rst` & `tucavoc-0.0.2/docs/source/uncertainties/Volume.rst`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/__init__.py` & `tucavoc-0.0.2/tucavoc/__init__.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/abstract_uncertainty.py` & `tucavoc-0.0.2/tucavoc/abstract_uncertainty.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,24 @@
 
     val: bool
     type: Type = bool
     unit: str = "-"
 
 
 @dataclass
+class StrParameter(Parameter):
+    """A parameter that is a string.
+
+    The value is a string.
+    """
+
+    val: str
+    type: Type = str
+
+@dataclass
 class CalculatedVariable(Parameter):
     """A variable that is calculated from other variables.
 
 
     :param val: Value of the variable.
     :param equations: List of equations that are used to calculate the variable.
         (only used for documentation purposes)
```

### Comparing `tucavoc-0.0.1/tucavoc/calculations.py` & `tucavoc-0.0.2/tucavoc/calculations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-from datetime import timedelta
 import logging
-from warnings import warn
-import pandas as pd
+from datetime import timedelta
+from warnings import simplefilter, warn
+
 import numpy as np
-from warnings import simplefilter
-from tucavoc.flags import set_flags, set_group_flags
+import pandas as pd
+from avoca.utils import datetime_for_index
 
+from tucavoc.abstract_uncertainty import Uncertainty
+from tucavoc.flags import set_flags, set_group_flags
 
 from tucavoc.uncertainties import (
     Calibration,
     FurtherInstrumentalProblems,
-    PeakIntegration,
     Linearity,
+    PeakIntegration,
     Precision,
     Sampling,
     Volume,
 )
-from tucavoc.abstract_uncertainty import Uncertainty
-
-from tucavoc.plots import (
-    plot_calibration_areas,
-    plot_calibration_concs,
-    plot_uncertainties,
-    plot_uncertainties_err_bars,
-    plot_uncertainties_parts,
-)
 
 
 def get_groups_dict(df_subs: pd.DataFrame) -> dict[str, list[str]]:
     """Get the substances and their group.
 
     :return groups_dict: A dictionary where keys are group names and
         values are lists of subtances names.
@@ -39,14 +32,16 @@
 
             {
                 '': ['methane', 'isobutane'];
                 'my_group': ['nice_sub', 'other_sub', 'another_one']
             }
 
     """
+    if "group" not in df_subs.columns:
+        return {}
     return {
         group_name: df_subs.loc[df_subs["group"] == group_name].index.to_list()
         for group_name in np.unique(df_subs["group"])
         if group_name
     }
 
 
@@ -79,60 +74,83 @@
         # if all((not df_subs.loc[sub, "in_calib"] for sub in group_members)):
         #    list_of_problems.append(
         #        f"Group '{group_name}' has only substances that are not in "
         #        "the calibration."
         #    )
 
     if any((not df_subs.loc[sub, "in_calib"] for sub in substances)):
-        if not any(
-            (df_subs.loc[sub, "use_for_general_crf"] for sub in substances)
-        ):
+        if not any((df_subs.loc[sub, "use_for_general_crf"] for sub in substances)):
             # If we have some substance not in the calib and we dont have
             # substances for a general crf, we must check that all the non calib
             # substances are in groups
             for group_name, group_members in groups_dict.items():
-                if not any(
-                    (df_subs.loc[sub, "in_calib"] for sub in group_members)
-                ):
+                if not any((df_subs.loc[sub, "in_calib"] for sub in group_members)):
                     list_of_problems.append(
                         "No substance is in the general mean CRF, and"
                         f" '{group_name}' has no calibration substances to"
                         " calculate a group mean CRF."
                     )
 
             # Check that substances not in any group are all in calib
             if any(
                 (not df_subs.loc[sub, "in_calib"] for sub in groups_dict[""])
             ) and all(
-                (
-                    not df_subs.loc[sub, "use_for_general_crf"]
-                    for sub in substances
-                )
+                (not df_subs.loc[sub, "use_for_general_crf"] for sub in substances)
             ):
                 list_of_problems.append(
                     f"No substance is in the General mean CRF, and some"
                     f" substance belonging to no groups need to have a general"
                     f" CRF but no calibration substances were set be used in"
                     f" the General CRF."
                 )
 
+    # Check that the substances will have a proper calibration
+    for sub in substances:
+        if not df_subs.loc[sub, "in_calib"]:
+            # Must have the parameters for the crf calculation
+            if df_subs.loc[sub, "use_for_general_crf"]:
+                list_of_problems.append(
+                    f"{sub} is used for the general CRF but is not in the calibration."
+                )
+            # Check the required fields for the FID method
+            for field in ["carbon_number", "effective_carbon_number_contribution"]:
+                if pd.isna(df_subs.loc[sub, field]):
+                    list_of_problems.append(
+                        f"Substance '{sub}' is not in the calibration and"
+                        f" has no value for '{field}'."
+                    )
+            continue
+        # concnetration can be either set in the df_calc or in the df_subs
+        col = (sub, "conc_calib")
+        if col in df_calc:
+            if df_calc[col].isna().all():
+                list_of_problems.append(
+                    f"Calibration substance '{sub}' has no calibration"
+                    " values in the data (df_calc)."
+                )
+        else:
+            if pd.isna(df_subs.loc[sub, "conc_calib"]):
+                list_of_problems.append(
+                    f"Calibration substance '{sub}' has a none calibration"
+                    " values in the data (df_subs)."
+                )
+
     return list_of_problems
 
 
 def main(
     df_calc: pd.DataFrame,
     df_subs: pd.DataFrame,
     uncertainties: list[Uncertainty] = [],
     blanks_in_df_subs: bool = False,
     calib_type="std",
     blank_type="blank",
     ignore_n_first_blanks: int = 0,
     zero_min: bool = True,
     debug: bool = False,
-    calibration_sustances: list[str] = [],
     interpolate: bool = True,
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
     """Main calculations.
 
     :arg df_calc: The dataframe containing the area of the substances
         for which we want to calculate the concentration.
     :arg df_subs: The dataframe containing information on each substances.
@@ -154,27 +172,64 @@
         in case negative are calculated (clipping).
     :arg debug: Whether to add debug information to the dfs.
     :arg calibration_sustances: The list of substances to use in the calibration
         to calculate the CRF.
         If not given, all substances will be used.
     :arg interpolate: Whether to interpolate the calibration and blank data.
 
+    :return df_calc: The dataframe with the calculated concentrations.
+    :return df_calib: The dataframe with the calibration values.
     """
+    logger = logging.getLogger(__name__)
     # Ignore these warnings
     simplefilter(action="ignore", category=pd.errors.PerformanceWarning)
     substances = list(df_subs.index.values)
 
     # Find which substrances are used for the calibraiton
-    calib_substances = calibration_sustances or substances
-    substances_not_in_calib = [
-        sub for sub in substances if sub not in calib_substances
-    ]
+    calib_substances = df_subs.loc[df_subs["in_calib"]].index.to_list()
+    substances_not_in_calib = [sub for sub in substances if sub not in calib_substances]
+    logger.info(f"Calibration substances: {calib_substances}")
+    logger.info(f"Substances not in the calibration: {substances_not_in_calib}")
     # Find how groups are constituted
     groups_dict = get_groups_dict(df_subs)
 
+    # Copy the main dataframe
+    df_calc = df_calc.copy()
+    # Make sure we have datetime consistency
+    # Check the index is not date time
+    if isinstance(df_calc.index, pd.DatetimeIndex):
+        # Set it to a datetime column
+        if ("-", "datetime") not in df_calc.columns:
+            df_calc[("-", "datetime")] = df_calc.index
+        else:
+            # Check that they are the same
+            if not df_calc[("-", "datetime")].equals(df_calc.index):
+                raise ValueError("The datetime column is not the same as the index.")
+
+    if ("-", "datetime") not in df_calc.columns:
+        raise ValueError("The datetime column is not given.")
+    # Set the index to a simple integer indexP
+    df_calc = df_calc.reset_index(drop=True)
+
+    # Setup some data
+    for sub in calib_substances:
+        col = (sub, "conc_calib")
+        if col not in df_calc.columns:
+            df_calc[col] = df_subs.loc[sub, "conc_calib"]
+        else:
+            # There is a column in the df_calc, we will use it
+            # but we need to remove the nan values
+            if interpolate:
+                with datetime_for_index(df_calc):
+                    df_calc[col] = df_calc[col].interpolate(
+                        method="time", limit_direction="both"
+                    )
+            else:
+                df_calc[col] = df_calc[col].ffill()
+
     # 1. find the calibrations values
     # This will add
     df_calib = make_calibration(
         df_calc,
         calib_substances,
         calib_type=calib_type,
         debug=debug,
@@ -195,15 +250,15 @@
                 # Do now for calib substances, as FID substances are handled later
                 # Retreive the area using the BLANK_AREA_FROM_CONC equation
                 df_calc[(sub, "area_blank")] = (
                     df_calc[(sub, "area_calib")]
                     * df_subs.loc[sub, "blank_conc_preset"]
                     / (
                         df_subs.loc[sub, "blank_conc_preset"]
-                        + df_subs.loc[sub, "conc_calib"]
+                        + df_calc[(sub, "conc_calib")]
                         * df_subs.loc[sub, "volume_calib"]
                         / df_subs.loc[sub, "volume_sample"]
                     )
                 )
     else:
         # All substance must be read from the data
         subs_blank_from_data = substances
@@ -223,15 +278,15 @@
         )
 
     # 3. calculate the calibration factor
     # ml * pmol/mol / area = ml * pmol/mol / area
     for sub in calib_substances:
         df_calc[(sub, "calib_factor")] = (
             df_subs.loc[sub, "volume_calib"]
-            * df_subs.loc[sub, "conc_calib"]
+            * df_calc[(sub, "conc_calib")]
             / (df_calc[(sub, "area_calib")] - df_calc[(sub, "area_blank")])
         )
         # Also calucalte the calibraiton error
         df_calc[(sub, "rel_std_area_cal_series")] = (
             df_calc[(sub, "area_std_calib")] / df_calc[(sub, "area_calib")]
         )
 
@@ -251,31 +306,26 @@
                 df_calc[(sub, "calib_factor")]
                 * df_subs.loc[sub, "carbon_number"]
                 * df_subs.loc[sub, "effective_carbon_number_contribution"]
             )
 
         # Get substances used to compute the general mean crf
         general_crf_substances = [
-            sub
-            for sub in calib_substances
-            if df_subs.loc[sub, "use_for_general_crf"]
+            sub for sub in calib_substances if df_subs.loc[sub, "use_for_general_crf"]
         ]
 
         # Calculate a general mean CRF
         df_calc[("-", "general_mean_carbon_response_factor")] = df_calc[
             [(sub, "carbon_response_factor") for sub in general_crf_substances]
         ].mean(axis=1)
 
         # The general error on the calibration
         df_calc[("-", "general_rel_std_area_cal_series")] = (
             df_calc[
-                [
-                    (sub, "rel_std_area_cal_series")
-                    for sub in general_crf_substances
-                ]
+                [(sub, "rel_std_area_cal_series") for sub in general_crf_substances]
             ]
             .pow(2)
             .sum(axis=1)
             .pow(0.5)
             .divide(len(general_crf_substances))
         )
         # Calculate the mean carbon response factor of each group
@@ -284,18 +334,15 @@
             group_calib_substances = [
                 sub for sub in group_members if sub in calib_substances
             ]
             # If the group has some substance and the group is not the default
             if group_calib_substances and group_name != "":
                 # Mean CRF of the group
                 df_calc[(group_name, "mean_carbon_response_factor")] = df_calc[
-                    [
-                        (sub, "carbon_response_factor")
-                        for sub in group_calib_substances
-                    ]
+                    [(sub, "carbon_response_factor") for sub in group_calib_substances]
                 ].mean(axis=1)
                 # Error on the calibration of the group uses the std of the
                 # calibration substances in the group
                 # (same one used for the crf calculation)
                 df_calc[(group_name, "rel_std_area_cal_series")] = (
                     df_calc[
                         [
@@ -368,31 +415,33 @@
                         df_calc[(sub, "conc")],
                         df_calc[(sub, "rel_std_area_cal_series")],
                         df_subs.loc[(sub, "detection_limit")],
                     )
                 case Calibration():
                     df_calc[(sub, f"u_{u.name}")] = u.calculate(
                         df_calc[(sub, "conc")],
-                        df_subs.loc[sub, "conc_calib"],
+                        (
+                            df_calc[(sub, "conc_calib")]
+                            if sub in calib_substances
+                            else 0.0
+                        ),
                         df_subs.loc[sub, "abs_u_cal"],
                     )
                     # TODO: remove this temporary correction
                     # It is dued to CRF, not having their uncertainty
                     # formula calculated yet
                     mask_inf = df_calc[(sub, f"u_{u.name}")] == np.inf
                     mask_conc_0 = df_calc[(sub, "conc")] == 0.0
-                    df_calc.loc[
-                        mask_inf | mask_conc_0, (sub, f"u_{u.name}")
-                    ] = 0.0
+                    df_calc.loc[mask_inf | mask_conc_0, (sub, f"u_{u.name}")] = 0.0
                 case PeakIntegration():
                     if sub in calib_substances:
                         df_calc[(sub, f"u_{u.name}")] = u.calculate(
                             df_calc[(sub, "calib_factor")],
                             df_subs.loc[sub, "volume_calib"],
-                            df_subs.loc[sub, "conc_calib"],
+                            df_calc[(sub, "conc_calib")],
                             df_calc[(sub, "area_calib")],
                             df_calc[(sub, "area")],
                             df_subs.loc[sub, "volume_sample"],
                             df_subs.loc[sub, "u_peak_area_integ_sample"],
                             df_subs.loc[sub, "u_peak_area_integ_calib"],
                         )
                     else:
@@ -416,17 +465,15 @@
                     )
                 case Linearity():
                     df_calc[(sub, f"u_{u.name}")] = u.calculate(
                         df_subs.loc[sub, "uncertainty_due_to_linearity"],
                     )
                 case Sampling():
                     df_calc[(sub, f"u_{u.name}")] = u.calculate(
-                        df_subs.loc[
-                            sub, "uncertainty_sampling_volume_accuracy"
-                        ],
+                        df_subs.loc[sub, "uncertainty_sampling_volume_accuracy"],
                     )
 
                 case _:
                     raise NotImplementedError(u)
 
     # 7. calculate the concentration and uncertainties of the groups
     for group_name, group_members in groups_dict.items():
@@ -544,14 +591,18 @@
     :arg ignore_n_first: The number of first runs that should be ignored during
         the calibration.
     :arg interpolate: Whether to interpolate the values between the calibrations
         If not, the previous calibration value will be used.
 
     """
 
+    logger = logging.getLogger(__name__)
+
+    logger.debug(f"Making calibration for {df_calc.head()=}")
+
     if calib_name in ["std"]:
         raise ValueError(f"Cannot use {calib_name=}")
 
     mask_calib = df_calc[("-", "type")] == calib_type
     # Add a column that retrives this info
     df_calc[f"is_{calib_name}"] = False
 
@@ -574,68 +625,65 @@
             f" '{calib_name=}'."
         )
 
     # Create all the columns for the calibration and the df
     subs_areas = [(sub, "area") for sub in substances]
     subs_area_std = [(sub, "area_std") for sub in substances]
     df_calib = pd.DataFrame(
-        columns=["datetime"] + subs_areas + subs_area_std,
+        columns=[("-", "datetime")] + subs_areas + subs_area_std,
     )
 
+    logger.debug(f"{indexes_calib_batches_start=}")
+    logger.debug(f"{indexes_calib_batches_end=}")
+    number_of_calibrations = len(indexes_calib_batches_start)
+
+    if number_of_calibrations == 0:
+        raise ValueError(f"No calibration found for {calib_type=}, {calib_name=}")
+
+    logger.debug(f"{subs_areas=}")
+
     # Iterate over the std battches to compute the means and std
-    for start, end in zip(
-        indexes_calib_batches_start, indexes_calib_batches_end
-    ):
+    for start, end in zip(indexes_calib_batches_start, indexes_calib_batches_end):
         df_calc.loc[start:end, f"is_{calib_name}"] = True
         df_this_calib = df_calc.loc[start:end, subs_areas]
 
         # Calculate mean and std
         mean_values = df_this_calib.mean(axis="index")
-        std_values = df_this_calib.std(axis="index").rename(
-            {"area": "area_std"}
-        )
-        df_calib.loc[start] = mean_values
-        df_calib.loc[end] = mean_values
+        std_values = df_this_calib.std(axis="index").rename({"area": "area_std"})
+
+        df_calib.loc[start, subs_areas] = mean_values
+        df_calib.loc[end, subs_areas] = mean_values
         df_calib.loc[start, subs_area_std] = std_values
         df_calib.loc[end, subs_area_std] = std_values
 
     # Finds out the indexes where the calibration occured
     indexes_calib = np.sort(
-        np.concatenate(
-            [indexes_calib_batches_start, indexes_calib_batches_end]
-        )
+        np.concatenate([indexes_calib_batches_start, indexes_calib_batches_end])
     )
-    # Add datetime info
-    df_calib.loc[indexes_calib, "datetime"] = df_calc.loc[
-        indexes_calib, "datetime"
-    ]
 
+    logger.debug(f"{indexes_calib=}")
     # Add calib info
     df_calc[f"previous_{calib_name}"] = indexes_calib[
         np.maximum(
             np.searchsorted(indexes_calib, df_calc.index, side="right") - 1,
             0,
         )
     ]
     df_calc[f"next_{calib_name}"] = indexes_calib[
         np.minimum(
             np.searchsorted(indexes_calib, df_calc.index, side="left"),
             len(indexes_calib) - 1,
         )
     ]
 
-    sample_dt = df_calc["datetime"].to_numpy()
-    previous_calib_time = sample_dt[
-        df_calc[f"previous_{calib_name}"].to_numpy()
-    ]
+    sample_dt = df_calc[("-", "datetime")].to_numpy()
+    previous_calib_time = sample_dt[df_calc[f"previous_{calib_name}"].to_numpy()]
     next_calib_time = sample_dt[df_calc[f"next_{calib_name}"].to_numpy()]
     # Find the timedeltas to the other calibrations
-    previous_td = np.maximum(
-        sample_dt - previous_calib_time, np.timedelta64(0)
-    )
+    previous_td = np.maximum(sample_dt - previous_calib_time, np.timedelta64(0))
     next_td = np.maximum(next_calib_time - sample_dt, np.timedelta64(0))
 
     # Find the weigths
     # Remove 0 values
     mask_0 = previous_td == next_td
     next_td[mask_0] = np.timedelta64(timedelta(seconds=1))
     total = previous_td + next_td
@@ -648,131 +696,42 @@
         df_calc[f"next_{calib_name}_time"] = next_calib_time
         df_calc["previous_td"] = previous_td
         df_calc["next_td"] = next_td
         df_calc["previous_w"] = previous_w
         df_calc["next_w"] = next_w
 
     # Set the calibration values in the df
-
-    #    for sub in substances:
-    #        df_calc[(sub, f"{calib_name}_area")] = df_calib[(sub, "area")]
-    #        df_calc[(sub, f"{calib_name}_area_std2")] = (
-    #            df_calib[(sub, "area_std")] ** 2
-    #        )
-
-    df_calc[[(sub, f"area_{calib_name}") for sub in substances]] = df_calib[
-        [(sub, "area") for sub in substances]
-    ]
-    df_calc[[(sub, f"area_std2_{calib_name}") for sub in substances]] = (
-        df_calib[[(sub, "area_std") for sub in substances]] ** 2
-    )
-
-    df_calc["row_index"] = df_calc.index
-
-    df_calc.set_index("datetime", inplace=True)
     for sub in substances:
-        if not interpolate:
-            # Use the previous value as calibration value
-            df_calc[(sub, f"area_{calib_name}")].interpolate(
-                method="pad", inplace=True, limit_direction="forward"
-            )
-            df_calc[(sub, f"area_std2_{calib_name}")].interpolate(
-                method="pad", inplace=True, limit_direction="forward"
-            )
-            # The first values will be have the first calibration value
-            # From the intepolation below
-
-        # Interpolate the values according to the time weights
-        df_calc[(sub, f"area_{calib_name}")].interpolate(
-            method="time", inplace=True, limit_direction="both"
-        )
-        df_calc[(sub, f"area_std2_{calib_name}")].interpolate(
-            method="time", inplace=True, limit_direction="both"
-        )
-
-        df_calc[(sub, f"area_std_{calib_name}")] = np.sqrt(
-            df_calc[(sub, f"area_std2_{calib_name}")]
+        df_calc[(sub, f"area_{calib_name}")] = df_calib[(sub, "area")].astype(float)
+        col_std = (sub, "area_std")
+        df_calib[col_std] = (
+            # Remove the inf values
+            df_calib[col_std]
+            .astype(float)
+            .replace([np.inf, -np.inf], np.nan)
         )
-    df_calc["datetime"] = df_calc.index
-    df_calc.set_index("row_index", inplace=True)
-
-    return df_calib
+        df_calc[(sub, f"area_std2_{calib_name}")] = df_calib[col_std] ** 2
 
+    cols_to_interpolate = [f"area_{calib_name}", f"area_std2_{calib_name}"]
 
-# %%
-if __name__ == "__main__":
-    from tucavoc import read_gcwerks
-
-    df_calc = read_gcwerks(
-        r"C:\Users\coli\Documents\ovoc-calculations\data\TestData.dat"
-    )
-
-    substances = [
-        sub
-        for sub, _ in df_calc.columns
-        if sub not in ["-", "datetime", "datetime_start", "datetime_end"]
-    ]
-
-    df_subs = pd.DataFrame(
-        columns=["volume_calib", "conc_calib"], index=substances
-    )
+    with datetime_for_index(df_calc):
+        for sub in substances:
+            for col in cols_to_interpolate:
 
-    df_subs["volume_calib"] = 600
-    df_subs["volume_sample"] = 600
-    df_subs["detection_limit"] = 10
-    df_subs["volume_uncertainty_sample"] = 20
-    df_subs["volume_uncertainty_calib"] = 20
-    df_subs["error_systematic_instrument"] = 1.0
-    df_subs["uncertainty_due_to_linearity"] = 0.0
-    df_subs["uncertainty_sampling_volume_accuracy"] = 0.0
-    df_subs["u_peak_area_integ_sample"] = 2.0
-    df_subs["u_peak_area_integ_calib"] = 2.0
-    df_subs["conc_calib"] = 4000
-    df_subs["abs_u_cal"] = 1.0
-    df_subs["carbon_number"] = 2.0
-    df_subs["effective_carbon_number_contribution"] = 1.0
-    df_subs["use_for_general_crf"] = True
-    df_subs["blank_conc_preset"] = 0.0
-
-    df_subs["group"] = ""
-
-    uncs = [
-        Precision(),
-        Calibration(),
-        PeakIntegration(),
-        Volume(),
-        FurtherInstrumentalProblems(),
-        Linearity(),
-        Sampling(),
-    ]
-    main(
-        df_calc,
-        df_subs,
-        uncertainties=uncs,
-        debug=True,
-        blanks_in_df_subs=True,
-        calibration_sustances=substances[1:3],
-        interpolate=False,
-    )
-    # print(df_calc.loc[505:520])
-    # print(df_calc.loc[1285:1295])
-    # print(df_calc.loc[2624:2632])
-    # print(df_calc.columns)
-
-    import matplotlib.pyplot as plt
-
-    fig, axes = plt.subplots(3, 1, sharex=True)
-
-    name = "ethane"
-    # name = "methane"
-    plot_calibration_areas(axes[0], name, df_calc, df_subs)
-    plot_uncertainties(
-        axes[1], name, uncs, df_calc[~df_calc["is_calib"]], df_subs
-    )
-    plot_uncertainties_parts(
-        axes[2], name, uncs, df_calc[~df_calc["is_calib"]], df_subs
-    )
-    # plot_uncertainties_err_bars(axes[1], name, uncs, df_calc, df_subs)
+                if not interpolate:
+                    # Use the previous value as calibration value
+                    df_calc[(sub, col)] = df_calc[(sub, col)].ffill()
+                # The first values will be have the first calibration value
+                # From the intepolation below
+
+                # Interpolate the values according to the time weights
+                df_calc[(sub, col)] = df_calc[(sub, col)].interpolate(
+                    method="time", limit_direction="both"
+                )
+            # Calculate the std from the root of the std2
+            logger.debug(df_calc[(sub, f"area_std2_{calib_name}")])
+            df_calc[(sub, f"area_std_{calib_name}")] = (
+                df_calc[(sub, f"area_std2_{calib_name}")].astype(float).apply(np.sqrt)
+            )
 
-    plt.show()
+    return df_calib
 
-# %%
```

### Comparing `tucavoc-0.0.1/tucavoc/equations.py` & `tucavoc-0.0.2/tucavoc/equations.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/flags.py` & `tucavoc-0.0.2/tucavoc/flags.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/parameters.py` & `tucavoc-0.0.2/tucavoc/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from tucavoc import tex
 from tucavoc.abstract_uncertainty import (
     CalculatedVariable,
     DataVariable,
     OptionalDataVariable,
     OptionalFloatParameter,
     FloatParamter,
+    StrParameter,
     OptionalDataVariableOrCalculated,
     Selection,
     BoolParameter,
 )
 
 
 SAMPLE_AREA = DataVariable(
@@ -368,7 +369,15 @@
 
 
 FLAG = CalculatedVariable(
     "flag",
     full_name="A Flag value",
     explanation="The flag value attributed. See :ref:`flagging`.",
 )
+
+
+GROUP = StrParameter(
+    name="group",
+    val="", 
+    full_name="Group name",
+    explanation="The name of the group to which a compound belongs.",
+)
```

### Comparing `tucavoc-0.0.1/tucavoc/plots.py` & `tucavoc-0.0.2/tucavoc/plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,77 +22,78 @@
 ):
     """Plot the calibration."""
     # Plot tanks in a different color
     if ("-", "type") in df_calc:
         mask_tank = df_calc[("-", "type")] == "tank"
         if any(mask_tank):
             ax.scatter(
-                df_calc.loc[mask_tank, "datetime"],
+                df_calc.loc[mask_tank, ("-", "datetime")],
                 df_calc.loc[mask_tank, (sub, "area")],
                 label="tank_area",
                 color=Colors.TANK,
             )
         # Simply plot the area of everything
         ax.plot(
-            df_calc.loc[~mask_tank, "datetime"],
+            df_calc.loc[~mask_tank, ("-", "datetime")],
             df_calc.loc[~mask_tank, (sub, "area")],
             label="measured_area",
             color=Colors.SAMPLE,
         )
     else:
         # Simply plot the area of everything
         ax.plot(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             df_calc[(sub, "area")],
             label="measured_area",
             color=Colors.SAMPLE,
         )
     if (sub, "area_calib") in df_calc:
         ax.plot(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             df_calc[(sub, "area_calib")],
             label="area_calib",
             color=Colors.CALIBRATION,
         )
     if (sub, "area_blank") in df_calc:
         # Check has blank
         ax.plot(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             df_calc[(sub, "area_blank")],
             label="area_blank",
             color=Colors.BLANK,
         )
         mask_blank = df_calc["is_blank"]
         ax.scatter(
-            df_calc.loc[mask_blank, "datetime"],
+            df_calc.loc[mask_blank, ("-", "datetime")],
             df_calc.loc[mask_blank, (sub, "area")],
             color=Colors.BLANK,
         )
     if (sub, "area_calib") in df_calc:
         ax.fill_between(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             df_calc[(sub, "area_calib")] - df_calc[(sub, "area_std_calib")],
             df_calc[(sub, "area_calib")] + df_calc[(sub, "area_std_calib")],
             color=Colors.CALIBRATION,
             alpha=0.6,
         )
     mask_calib = df_calc["is_calib"]
     ax.scatter(
-        df_calc.loc[mask_calib, "datetime"],
+        df_calc.loc[mask_calib,("-", "datetime")],
         df_calc.loc[mask_calib, (sub, "area")],
         color=Colors.CALIBRATION,
     )
     ax2 = ax.twinx()
     if (sub, "calib_factor") in df_calc:
-        ax2.plot(
-            df_calc["datetime"],
-            df_calc[(sub, "calib_factor")],
-            color="grey",
-            label="calibration factor",
-        )
+        if not df_calc[(sub, "calib_factor")].isna().all():
+            ax2.plot(
+                df_calc[("-", "datetime")],
+                df_calc[(sub, "calib_factor")],
+                color="grey",
+                label="calibration factor",
+            )
         ax2.set_ylabel(parameters.CALIB_FACTOR.unit)
         # Just to show the legend with the others
         ax.plot(
             [],
             color="grey",
             label=f"{parameters.CALIB_FACTOR.name} (scale right)",
         )
@@ -101,15 +102,15 @@
 
         mean_crf = (
             df_calc[(group, "mean_carbon_response_factor")]
             if group
             else df_calc[("-", "general_mean_carbon_response_factor")]
         )
         ax2.plot(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             mean_crf,
             color="grey",
             label=parameters.MEAN_CRF.full_name,
         )
         ax2.set_ylabel(parameters.MEAN_CRF.unit)
         # Just to show the legend with the others
         ax.plot(
@@ -123,25 +124,35 @@
     ax.set_title(f"Areas for {sub}")
 
 
 def plot_calibration_concs(
     ax: Axes, sub: str, df_calc: pd.DataFrame, df_subs: pd.DataFrame
 ):
     """Plot the concentration of the calibration."""
-    ax.plot(
-        df_calc["datetime"],
-        df_calc[(sub, "conc")],
-        label="Calculated Concentration",
-        color=Colors.SAMPLE,
-    )
+    if not df_calc[(sub, "conc")].isna().all():
+        ax.plot(
+            df_calc[("-", "datetime")],
+            df_calc[(sub, "conc")],
+            label="Calculated Concentration",
+            color=Colors.SAMPLE,
+        )
     mask_calibration = df_calc[("-", "type")] == "std"
+
+    conc_calib = (
+        df_calc[(sub, "conc_calib")]
+        if (sub, "conc_calib") in df_calc
+        else pd.Series(df_subs.loc["conc_calib", sub], index=df_calc.index)
+    )
+    mask_not_nan = ~conc_calib.isna()
+    mask = mask_calibration & mask_not_nan
+
+
     ax.scatter(
-        df_calc.loc[mask_calibration, "datetime"],
-        # Full array for every calibration point
-        np.full(np.sum(mask_calibration), df_subs.loc["conc_calib", sub]),
+        df_calc.loc[mask, ("-", "datetime")],
+        conc_calib.loc[mask],
         label="Calibration Concentration",
         color=Colors.CALIBRATION,
     )
     ax.set_ylabel("[pmol/mol]")
     ax.legend()
 
 
@@ -150,88 +161,88 @@
     sub: str,
     uncertainties: list[Uncertainty],
     df_calc: pd.DataFrame,
     df_subs: pd.DataFrame,
 ):
     """Plot the uncertainties."""
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")],
         label="Calculated Concentration",
         color=Colors.SAMPLE,
     )
     top_line = df_calc[(sub, "conc")].to_numpy()
     bot_line = df_calc[(sub, "conc")].to_numpy()
     for u in uncertainties:
         std = df_calc[(sub, f"u_{u.name}")]
         new_top_line = top_line + std
         new_bot_line = bot_line - std
         ax.fill_between(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             top_line,
             new_top_line,
             label=f"Uncertainty {u.name}",
             color=u.color,
         )
         ax.fill_between(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             bot_line,
             new_bot_line,
             color=u.color,
         )
         # Update where the lines are
         top_line = new_top_line
         bot_line = new_bot_line
 
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")] + df_calc[(sub, "u_combined")],
         label="Combined Uncertainty",
         color=Colors.COMBINED_U,
         linestyle="--",
     )
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")] - df_calc[(sub, "u_combined")],
         color=Colors.COMBINED_U,
         linestyle="--",
     )
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")] + df_calc[(sub, "u_expanded")],
         label="Expanded Uncertainty",
         color=Colors.EXPANDED_U,
         linestyle="--",
     )
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")] - df_calc[(sub, "u_expanded")],
         color=Colors.EXPANDED_U,
         linestyle="--",
     )
 
     ax.set_ylabel("[pmol/mol]")
 
     ax2 = ax.twinx()
     ax2.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "u_rel_combined")] * 100,
         label="Relative Combined Uncertainty",
         color=Colors.COMBINED_REL_U,
         linestyle="--",
     )
     # Just to show the legend with the others
     ax.plot(
         [],
         label="Relative Combined Uncertainty  (scale right)",
         color=Colors.COMBINED_REL_U,
         linestyle="--",
     )
     ax2.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "u_rel_expanded")] * 100,
         label="Relative Expanded Uncertainty",
         color=Colors.EXPANDED_REL_U,
         linestyle="--",
     )
     # Just to show the legend with the others
     ax.plot(
@@ -250,61 +261,61 @@
     sub: str,
     uncertainties: list[Uncertainty],
     df_calc: pd.DataFrame,
     df_subs: pd.DataFrame,
 ):
     """Plot the uncertainties using error bars instead of surface errors."""
     ax.scatter(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")],
         label="Calculated Concentration",
         color=Colors.SAMPLE,
     )
     top_line = df_calc[(sub, "conc")].to_numpy()
     bot_line = df_calc[(sub, "conc")].to_numpy()
 
     cap_size = 5
     for u in uncertainties:
         std = df_calc[(sub, f"u_{u.name}")]
         new_top_line = top_line + std
         new_bot_line = bot_line - std
         ax.errorbar(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             top_line,
             std,
             lolims=True,
             label=f"Uncertainty {u.name}",
             linestyle="None",
             color=u.color,
             capsize=cap_size,
         )
         ax.errorbar(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             bot_line,
             std,
             uplims=True,
             linestyle="None",
             color=u.color,
             capsize=cap_size,
         )
         # Update where the lines are
         top_line = new_top_line
         bot_line = new_bot_line
 
     ax.errorbar(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")],
         df_calc[(sub, "u_combined")],
         label="Combined Uncertainty",
         color=Colors.COMBINED_U,
         linestyle="None",
         capsize=3 * cap_size,
     )
     ax.errorbar(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(sub, "conc")],
         df_calc[(sub, "u_expanded")],
         label="Expanded Uncertainty",
         color=Colors.EXPANDED_U,
         linestyle="None",
         capsize=3 * cap_size,
     )
@@ -321,15 +332,15 @@
     df_subs: pd.DataFrame,
 ):
     """Plot the part of uncertainties in the total uncertainties."""
     for u in uncertainties:
         part_of_u = df_calc[(sub, f"ratio_u_{u.name}_in_u_combined")]
 
         ax.plot(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             part_of_u,
             label=f"Uncertainty {u.name}",
             color=u.color,
         )
 
     ax.set_ylabel("[%]")
     ax.legend()
@@ -339,25 +350,25 @@
     ax: Axes,
     group: str,
     df_calc: pd.DataFrame,
     df_subs: pd.DataFrame,
 ):
     """Plot the uncertainties."""
     ax.plot(
-        df_calc["datetime"],
+        df_calc[("-", "datetime")],
         df_calc[(group, "conc")],
         label="Calculated Concentration",
         color=Colors.SAMPLE,
     )
     top_line = np.zeros(len(df_calc))
     for member in df_subs["group"].loc[df_subs["group"] == group].index:
         conc = df_calc[(member, "conc")]
         new_top_line = top_line + conc
         ax.fill_between(
-            df_calc["datetime"],
+            df_calc[("-", "datetime")],
             top_line,
             new_top_line,
             label=member,
         )
 
         # Update where the line is
         top_line = new_top_line
```

### Comparing `tucavoc-0.0.1/tucavoc/station.py` & `tucavoc-0.0.2/tucavoc/station.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/tex.py` & `tucavoc-0.0.2/tucavoc/tex.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/uncertainties.py` & `tucavoc-0.0.2/tucavoc/uncertainties.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/additional_data/__init__.py` & `tucavoc-0.0.2/tucavoc/additional_data/__init__.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/additional_data/empa.py` & `tucavoc-0.0.2/tucavoc/additional_data/empa.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/additional_data/station.py` & `tucavoc-0.0.2/tucavoc/additional_data/station.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/additional_data/widget.py` & `tucavoc-0.0.2/tucavoc/additional_data/widget.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/__init__.py` & `tucavoc-0.0.2/tucavoc/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/ebas_genfile.py` & `tucavoc-0.0.2/tucavoc/exports/ebas_genfile.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/ebas_test.py` & `tucavoc-0.0.2/tucavoc/exports/ebas_test.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/empa_qa_tools.py` & `tucavoc-0.0.2/tucavoc/exports/empa_qa_tools.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/excel.py` & `tucavoc-0.0.2/tucavoc/exports/excel.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/exports/test_exports.py` & `tucavoc-0.0.2/tucavoc/exports/test_exports.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/parameters.py` & `tucavoc-0.0.2/tucavoc/widgets/parameters.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/qsettings_selector.py` & `tucavoc-0.0.2/tucavoc/widgets/qsettings_selector.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/station.py` & `tucavoc-0.0.2/tucavoc/widgets/station.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/substances.py` & `tucavoc-0.0.2/tucavoc/widgets/substances.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/uncertainties.py` & `tucavoc-0.0.2/tucavoc/widgets/uncertainties.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/tucavoc/widgets/utils.py` & `tucavoc-0.0.2/tucavoc/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/.gitignore` & `tucavoc-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 calculations/*
 meteo_files/Bero*
 original_ebas/
 exports/ebas_test.py
 settings.ini
 
 build/
+dist/
 
 tucavoc.egg-info/
 docs/build/
 # This is generated at doc build time
 docs/source/uncertainties/uncertainties.rst
 docs/source/parameters_glossary.rst
 docs/source/equations_glossary.rst
```

### Comparing `tucavoc-0.0.1/LICENSE` & `tucavoc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tucavoc-0.0.1/pyproject.toml` & `tucavoc-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tucavoc"
-version = "0.0.1"
+version = "0.0.2"
 description = "Application to calculate concentration and uncertainties of OVOC chromatography measurements"
 authors = [
     {name = "Lionel Constantin", email="lionel.constantin@empa.ch"},
     {name = "Stefan Reimann", email="Stefan.Reimann@empa.ch"},
 ]
 dependencies = [
     "numpy",
     "PySide6",
     "pandas",
     "tzdata",
     "openpyxl",
     "matplotlib",
+    "avoca",
     #"ebas-io @ https://git.nilu.no/ebas/ebas-io/-/raw/master/dist/ebas_io-4.2.0-py3-none-any.whl",
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["one", "two"]
 classifiers = [
@@ -38,7 +39,15 @@
 doc = [
     "sphinx",
     "furo",
     "enum_tools",
     "sphinx_toolbox",
 ]
 dev = ["black"]
+
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = [
+    "tests",
+]
```

### Comparing `tucavoc-0.0.1/PKG-INFO` & `tucavoc-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tucavoc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application to calculate concentration and uncertainties of OVOC chromatography measurements
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>, Stefan Reimann <Stefan.Reimann@empa.ch>
 License: 
         tucavoc
         
         Copyright (C) 2022  abt503 / Climate Gases / EMPA
         
@@ -649,14 +649,15 @@
                            END OF TERMS AND CONDITIONS
         
          
 License-File: LICENSE
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: avoca
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pyside6
 Requires-Dist: tzdata
 Provides-Extra: dev
```

