# Comparing `tmp/resurfemg-0.2.1-py3-none-any.whl.zip` & `tmp/resurfemg-0.2.2a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,31 @@
-Zip file size: 45281 bytes, number of entries: 26
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/__init__.py
--rw-r--r--  2.0 unx       94 b- defN 24-Jan-18 13:04 resurfemg/__main__.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/cli/__init__.py
--rw-r--r--  2.0 unx     5898 b- defN 24-Jan-18 13:04 resurfemg/cli/cli.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/config/__init__.py
--rw-r--r--  2.0 unx    15003 b- defN 24-Jan-18 13:04 resurfemg/config/config.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/data_connector/__init__.py
--rw-r--r--  2.0 unx     6321 b- defN 24-Jan-18 13:04 resurfemg/data_connector/converter_functions.py
--rw-r--r--  2.0 unx     9456 b- defN 24-Jan-18 13:04 resurfemg/data_connector/tmsisdk_lite.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/helper_functions/__init__.py
--rw-r--r--  2.0 unx    13437 b- defN 24-Jan-18 13:04 resurfemg/helper_functions/helper_functions.py
--rw-r--r--  2.0 unx     2493 b- defN 24-Jan-18 13:04 resurfemg/machine_learning/ml.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/pipelines/__init__.py
--rw-r--r--  2.0 unx    11709 b- defN 24-Jan-18 13:04 resurfemg/pipelines/pipelines.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/postprocessing/__init__.py
--rw-r--r--  2.0 unx    21086 b- defN 24-Jan-18 13:04 resurfemg/postprocessing/features.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/preprocessing/__init__.py
--rw-r--r--  2.0 unx    17468 b- defN 24-Jan-18 13:04 resurfemg/preprocessing/ecg_removal.py
--rw-r--r--  2.0 unx     6250 b- defN 24-Jan-18 13:04 resurfemg/preprocessing/envelope.py
--rw-r--r--  2.0 unx    12737 b- defN 24-Jan-18 13:04 resurfemg/preprocessing/filtering.py
--rw-r--r--  2.0 unx       24 b- defN 24-Jan-18 13:04 resurfemg/visualization/__init__.py
--rw-r--r--  2.0 unx     1411 b- defN 24-Jan-18 13:04 resurfemg/visualization/visualization.py
--rw-r--r--  2.0 unx    19759 b- defN 24-Jan-18 13:05 resurfemg-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-18 13:05 resurfemg-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Jan-18 13:05 resurfemg-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2281 b- defN 24-Jan-18 13:05 resurfemg-0.2.1.dist-info/RECORD
-26 files, 145721 bytes uncompressed, 41543 bytes compressed:  71.5%
+Zip file size: 50481 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/__init__.py
+-rw-r--r--  2.0 unx       94 b- defN 24-Apr-29 10:10 resurfemg/__main__.py
+-rw-r--r--  2.0 unx      413 b- defN 24-Apr-29 10:10 resurfemg/__version__.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/cli/__init__.py
+-rw-r--r--  2.0 unx     5898 b- defN 24-Apr-29 10:10 resurfemg/cli/cli.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/config/__init__.py
+-rw-r--r--  2.0 unx    15003 b- defN 24-Apr-29 10:10 resurfemg/config/config.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/data_connector/__init__.py
+-rw-r--r--  2.0 unx     6321 b- defN 24-Apr-29 10:10 resurfemg/data_connector/converter_functions.py
+-rw-r--r--  2.0 unx     9456 b- defN 24-Apr-29 10:10 resurfemg/data_connector/tmsisdk_lite.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/helper_functions/__init__.py
+-rw-r--r--  2.0 unx    13437 b- defN 24-Apr-29 10:10 resurfemg/helper_functions/helper_functions.py
+-rw-r--r--  2.0 unx     2493 b- defN 24-Apr-29 10:10 resurfemg/machine_learning/ml.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/pipelines/__init__.py
+-rw-r--r--  2.0 unx    11709 b- defN 24-Apr-29 10:10 resurfemg/pipelines/pipelines.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/postprocessing/__init__.py
+-rw-r--r--  2.0 unx     4891 b- defN 24-Apr-29 10:10 resurfemg/postprocessing/baseline.py
+-rw-r--r--  2.0 unx    21086 b- defN 24-Apr-29 10:10 resurfemg/postprocessing/features.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/preprocessing/__init__.py
+-rw-r--r--  2.0 unx    17468 b- defN 24-Apr-29 10:10 resurfemg/preprocessing/ecg_removal.py
+-rw-r--r--  2.0 unx     6250 b- defN 24-Apr-29 10:10 resurfemg/preprocessing/envelope.py
+-rw-r--r--  2.0 unx    12737 b- defN 24-Apr-29 10:10 resurfemg/preprocessing/filtering.py
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-29 10:10 resurfemg/visualization/__init__.py
+-rw-r--r--  2.0 unx     1411 b- defN 24-Apr-29 10:10 resurfemg/visualization/visualization.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-29 10:10 resurfemg-0.2.2a0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17946 b- defN 24-Apr-29 10:10 resurfemg-0.2.2a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 10:10 resurfemg-0.2.2a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-29 10:10 resurfemg-0.2.2a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2555 b- defN 24-Apr-29 10:10 resurfemg-0.2.2a0.dist-info/RECORD
+29 files, 160843 bytes uncompressed, 46309 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: resurfemg/__init__.py
 Comment: 
 
 Filename: resurfemg/__main__.py
 Comment: 
 
+Filename: resurfemg/__version__.py
+Comment: 
+
 Filename: resurfemg/cli/__init__.py
 Comment: 
 
 Filename: resurfemg/cli/cli.py
 Comment: 
 
 Filename: resurfemg/config/__init__.py
@@ -39,14 +42,17 @@
 
 Filename: resurfemg/pipelines/pipelines.py
 Comment: 
 
 Filename: resurfemg/postprocessing/__init__.py
 Comment: 
 
+Filename: resurfemg/postprocessing/baseline.py
+Comment: 
+
 Filename: resurfemg/postprocessing/features.py
 Comment: 
 
 Filename: resurfemg/preprocessing/__init__.py
 Comment: 
 
 Filename: resurfemg/preprocessing/ecg_removal.py
@@ -60,20 +66,23 @@
 
 Filename: resurfemg/visualization/__init__.py
 Comment: 
 
 Filename: resurfemg/visualization/visualization.py
 Comment: 
 
-Filename: resurfemg-0.2.1.dist-info/METADATA
+Filename: resurfemg-0.2.2a0.dist-info/LICENSE
+Comment: 
+
+Filename: resurfemg-0.2.2a0.dist-info/METADATA
 Comment: 
 
-Filename: resurfemg-0.2.1.dist-info/WHEEL
+Filename: resurfemg-0.2.2a0.dist-info/WHEEL
 Comment: 
 
-Filename: resurfemg-0.2.1.dist-info/top_level.txt
+Filename: resurfemg-0.2.2a0.dist-info/top_level.txt
 Comment: 
 
-Filename: resurfemg-0.2.1.dist-info/RECORD
+Filename: resurfemg-0.2.2a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `resurfemg-0.2.1.dist-info/METADATA` & `resurfemg-0.2.2a0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 Metadata-Version: 2.1
 Name: resurfemg
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: A package for analysis of respiratory EMG data
-Home-page: https://github.com/ReSurfEMG/ReSurfEMG
-Author: A team including the NLeSC and the U. of Twente
-Author-email: c.moore@esciencecenter.nl
-License: Apache v2
-Platform: UNKNOWN
+Maintainer-email: Eline Mos-Oppersma <e.oppersma@utwente.nl>, Rob Warnaar <r.s.p.warnaar@utwente.nl>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/ReSurfEMG
+Project-URL: Documentation, https://resurfemg.github.io/ReSurfEMG/
+Project-URL: Repository, https://github.com/ReSurfEMG/ReSurfEMG
+Project-URL: Issues, https://github.com/ReSurfEMG/ReSurfEMG/issues
+Project-URL: Changelog, https://github.com/ReSurfEMG/ReSurfEMG/blob/main/CHANGELOG.md
+Keywords: electromyography,EMG,respiratory,Python,surface EMG
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pyxdf
 Requires-Dist: mne ==0.23.4
 Requires-Dist: textdistance
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: h5py
-Requires-Dist: scikit-learn ==1.1.1
+Requires-Dist: numpy ==1.24.4
+Requires-Dist: scikit-learn ==1.3.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
-Requires-Dist: codestyle ; extra == 'dev'
+Requires-Dist: pytest-cov ; extra == 'dev'
+Requires-Dist: pycodestyle ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: wheel ; extra == 'dev'
 Requires-Dist: jupyter ; extra == 'dev'
 Requires-Dist: ipympl ; extra == 'dev'
+Requires-Dist: sphinx ; extra == 'dev'
+Requires-Dist: twine ; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: wheel ; extra == 'docs'
+Requires-Dist: sphinx ; extra == 'docs'
+Provides-Extra: tests
+Requires-Dist: pytest ; extra == 'tests'
+Requires-Dist: pytest-cov ; extra == 'tests'
+Requires-Dist: pycodestyle ; extra == 'tests'
+Requires-Dist: isort ; extra == 'tests'
+Requires-Dist: wheel ; extra == 'tests'
 
 <p align="center">
     <img style="width: 35%; height: 35%" src="https://github.com/resurfemg/resurfemg/blob/main/Logo_rond_tekst.svg">
 </p>
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6811554.svg)](https://doi.org/10.5281/zenodo.6811554)
 [![PyPI](https://img.shields.io/pypi/v/resurfemg.svg)](https://pypi.python.org/pypi/resurfemg/)
-[![Anaconda-Server Badge](https://anaconda.org/resurfemg/resurfemg/badges/version.svg)](https://anaconda.org/resurfemg/resurfemg)
 [![Sanity](https://github.com/resurfemg/resurfemg/actions/workflows/on-commit.yml/badge.svg)](https://github.com/resurfemg/resurfemg/actions/workflows/on-commit.yml)
 [![Sanity](https://github.com/resurfemg/resurfemg/actions/workflows/on-tag.yml/badge.svg)](https://github.com/resurfemg/resurfemg/actions/workflows/on-tag.yml)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6487/badge)](https://bestpractices.coreinfrastructure.org/projects/6487)
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
 [![status](https://joss.theoj.org/papers/5f08d1f2bb717b7d05762296e37ded3d/status.svg)](https://joss.theoj.org/papers/5f08d1f2bb717b7d05762296e37ded3d)
 
@@ -95,15 +116,15 @@
 
 ### Data sets
 
 The notebooks are configured to run on various datasets.  Contact
 Dr. Eline Mos-Oppersma( 📫 e.mos-oppersma@utwente.nl) to discuss any
 questions on data configuration for your datasets.
 
-If you want to use a standardized dataset for any purpose we reccomend
+If you want to use a standardized dataset for any purpose we recommend
 the data in the ReSurfEMG/synthetic_data repository
 
 [![DOI](https://zenodo.org/badge/635680008.svg)](https://zenodo.org/badge/latestdoi/635680008)
 
 Data there can be used with any respiratory EMG algorithms in any program. Thus that data can function as a benchmarking set to compare algorithms across different programs.
 
 
@@ -156,16 +177,16 @@
 ```
 
 ### Supported Platforms
 
 ReSurfEMG is a pure Python package. Below is the list of
 platforms that should work. Other platforms may work, but have had less extensive testing.
 Please note that where
-python.org Python or Anaconda Python stated as supported, it means
-that versions 3.8 or 3.9 (depending on the release) are supported.
+python.org Python stated as supported, it means
+that versions 3.9 are supported.
 
 #### AMD64 (x86)
 
 |                             | Linux     | Win       | OSX       |
 |:---------------------------:|:---------:|:---------:|:---------:|
 | ![p](etc/python-logo.png)   | Supported | Unknown   | Unknown   |
 | ![a](etc/anaconda-logo.png) | Supported | Supported | Supported |
@@ -177,15 +198,15 @@
 If you wish to install with pip:
 
 1. Create and activate a virtual environment (see developer setup section for more details) 
 2. Install ResurfEMG package by running `pip install resurfemg`.
 
 
 ## Getting Started
-#### with the reccomended Conda setup
+#### with the recommended Conda setup
 
 How to get the notebooks running?  Assuming the raw data set and
 metadata is available. Note for non-conda installations see next sections.
 
 0. Assuming you are using conda for package management:    
   * Make sure you are in no environment:
 
@@ -219,15 +240,15 @@
    * The command for Windows/Anaconda users can be something like:
 
      ```sh
      conda env create -f environment.yml
      ```
 
    * Linux users can create their own environment by hand (use
-     install_dev as in setup).
+     .[dev] as in setup).
     
   Make sure to enter your newly created environment.
 
 Option C: In theory if you want to work, but never develop (i.e. add code), as a conda user
    with a stable (released) version create an empty environment, and install
    there: 
 
@@ -262,16 +283,16 @@
 simply want to use our library need to install the packaged version
 from one of the package indexes to which we publish released versions
 (eg. PyPI).  This section of the readme is for advanced developers who want to
 modify the library code (and possibly contribute their changes back or eventually publish thier own modified fork). NB: you can accomplish modifications of the code, submit PRs and soforth without 
 a 'developer's setup' but we feel this setup will make advanced contributions easier.
 
 We have transitioned to a fully Python 3.9 environment.  The
-instructions below are for our newer versions above 0.1.0:
-(For older instructions with `venv` please see versions below 0.1.0, and
+instructions below are for our newer versions above 3.0.0:
+(For older instructions with `venv` please see versions below 0.2.0, and
 adapt them if using Windows and/or a different Python version than
 Python.org Python e.g. you may need to use `.venv/Scripts/activate` in
 place of `.venv/bin/activate`.  This will create a distributable
 package from the source code, then install it in the currently active
 environment.  This will also install development tools we use
 s.a. `pytest` and `codestyle` and will also install tools we use for
 working with the library, s.a. `jupyter`.)
@@ -283,182 +304,122 @@
 
 
 1. Using Anaconda Python
 
    ```sh
    conda create -n resurfemg python=3.9
    conda activate resurfemg
-   python setup.py anaconda_gen_meta
-   python setup.py install_dev
+   pip install -e .[dev]
    ```
 
-   Note, you will need to run `anaconda_gen_meta`.  This generates
-   `meta.yaml` which is necessary to create `conda` package.  In the
-   future this will probably be called automatically by `install_dev`.
-
 2. Using PyPI Python
 
    ```sh
    python3.9 -m venv .venv3.9
    # On Linux:
    . .venv3.9/bin/activate
    # On Windows:
    .venv3.9/Scripts/activate
-   python setup.py install_dev
+   pip install -e .[dev]
    ```
 
 Now you should have everything necessary to start working on the
-source code.  Whenever you make any changes, re-run `install_dev` to
-see them applied in your environment.  It's possible to find a
-shortcut sometimes to running the entire cycle (`install_dev` takes a
-long time to run).  Look at the source of `bdist_conda` and
-`sdist_conda` commands in `setup.py` for more info.
-
+source code.  Whenever you make any changes, re-run `pip install -e .[dev]` to
+see them applied in your environment.
 
 ## Generating documentation
 
 Online documentation can be found at
 https://resurfemg.github.io/ReSurfEMG/
 or on https://readthedocs.org/ by searching for ReSurfEMG.
 Up to date documentation can be generated in command-line as follows
 (in bash terminal):
 
 ``` sh
 python3 -m venv .venv
-. ./.venv/bin/activate
-pip install wheel sphinx
-./setup.py install
-./setup.py apidoc
-./setup.py build_sphinx
+source ./.venv/bin/activate
+pip install -e .[docs]
+python setup.py apidoc
+python setup.py build_sphinx
 ```
 
 If you are working in a VScode command line interface (terminal cmd)
 should be more or less something like the following:
 
 This is given with `cmd.exe` in mind:
 
 ``` sh
 python3 -m venv .venv
 .venv/bin/activate
-pip install wheel sphinx
-python setup.py install
+pip install -e .[docs]
 python setup.py apidoc
 python setup.py build_sphinx
 ```
 
 
 ## Automation
 
 The project comes with several modifications to the typical
 default `setup.py`.
 
 At the moment, the support for Anaconda Python is lacking.  The
 instructions and the commands listed below will work in Anaconda
 installation but due to the difference in management of installed
 packages, the project will be installed into base environment
-regardless of the currently active one.  We are planning to integrate
-with Anaconda in near future.
+regardless of the currently active one.
 
 The project has a sub-project of a related dashboard.  Dashboard is a GUI that
 exposes some of the project's functionality. In the past we kept a a legacy dashboard
 in the same repository with ReSurfEMG code but we have deleted it. The
 current version of the dashboard into it's own repository:
 https://github.com/ReSurfEMG/ReSurfEMG-dashboard
 
 
 ### New commands
 
-Commands that perform repeating tasks have a `--fast` option.  Use
-this if you ran `setup.py install_dev`, and you are sure the
-dependencies are up to date.  Otherwise, these commands will create a
-new virtual environment and install necessary dependencies there
-before execution.  This is primarily intended for use in CI to create
-controlled environment.
-
 Please note that documentation is built using `sphinx` command
 for `setuptools`: `setup.py build_sphinx`, but `sphinx` is not
 installed as part of development dependencies, rather it is declared
 as a dependency of `setup.py` itself.  There are cases when `setup.py`
 will not install its own dependencies.  You are advised to install
 them manually.
 
-* `setup.py lint` checks that the source code is formatted according to
-  PEP-8 recommendations.
 * `setup.py isort` checks that the imports are properly formatted and
   sorted.
 * `setup.py apidoc` generates RST outlines necessary to generate
   documentation.
-* `setup.py install_dev` installs dependencies necessary for
-  development.
-  
-### Modified commands
-
-* `setup.py test` the original command is overloaded with a new one.
-  Similarly to most of the new commands, this command takes `--fast`
-  as an option with the same meaning.  Unlike its predecessor, this
-  command will create a clean environment and install all necessary
-  dependencies before running the test (the original did install
-  dependencies, but ran the test in the source directory, this made it
-  impossible to test code that relied on being installed).
-  
-  
-### Installing from source
-
-The traditional way to install from source is to run `setup.py
-install` or `setup.py develop`.  Both of these will
-work... sort of.  This is because of the default behavior inherited from
-`setuptools`.  The problem here is that instead of creating a
-distributable package and installing that, `setuptools` does it
-in the other order: it installs the package in order to create a distributable
-one.
-
-As was already mentioned earlier, Anaconda Python will need better
-support, at which point, `setup.py install` will have to change to
-enable that.
-
-We are not planning on patching `setup.py develop` as we don't believe
-it is a good practice to use this command.  It is not removed,
-however, and should work in the same way it would work with a typical
-`setuptools` project.  
-
-Note that `pip install -e .` and `pip install -e '.[dev]'` are
-discouraged by association (since that is just a wrapper around
-`setup.py develop`.)  Similarly to `setup.py develop` they might work,
-but you have to be careful with interpreting the results.  If those
-don't work, it's on you.
-
 
 ### Testing
 
 The project doesn't include testing data.  It was packaged into a Docker
 image which can be found at `crabbone/resurfemg-poly5-test-files:latest`.
 This test data was created by taking a signal from equipment, not a human,
 and certainly not a patient.
 
 It is possible to run tests in container created from this image.
 Alternatively, you may download the image and extract directory
 `/ReSurfEMG/tests/not_pushed` into `not_pushed` in the root of the
 project and run:
 
 ``` sh
-python setup.py test
+pytest
 ```
 
 Below is a snippet that may help you to run the tests in a container:
 
 ``` sh
 docker run --rm -v $(pwd):/ci \
     --cap-add=SYS_ADMIN \
     --privileged=true \
     crabbone/resurfemg-poly5-test-files \
     sh -c 'set -xe
         cd /ci
         mkdir -p ./not_pushed/
         mount --bind /ReSurfEMG/tests/not_pushed/ ./not_pushed/
-        python setup.py test'
+        pytest'
 ```
 
 
 
 ## Command-Line Interface
 
 You will be able to preprocess, train and use models using command-line interface.
@@ -487,16 +448,14 @@
             --model  ml_models/finalized_lr_model_in_111.sav \
 
 You can also make synthetic data. To explore this start with
     `python -m resurfemg synth --help`
 You can also make from horizontally formated csv files 
 that can be read by the dashboard. To explore this start with
     `python -m resurfemg save_np --help`
-The help commandis also available for ml and acquire.
+The help command is also available for ml and acquire.
 
 All long options have short aliases.
 
 
 ✨Copyright 2022 Netherlands eScience Center and U. Twente
 Licensed under the Apache License, version 2.0. See LICENSE for details.✨
-
-
```

## Comparing `resurfemg-0.2.1.dist-info/RECORD` & `resurfemg-0.2.2a0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 resurfemg/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/__main__.py,sha256=0EiYudOep65jOuzzaev-yuTYrevgwNOLQLbsPNlQr4E,94
+resurfemg/__version__.py,sha256=P1AWJN7ghBRZ2aSCCCnZihradDcYVrrrkBt_1aqYaO8,413
 resurfemg/cli/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/cli/cli.py,sha256=XLKnrxoFmj2-Li5GOqJreb3jk8tYenn696jQIrIDVp4,5898
 resurfemg/config/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/config/config.py,sha256=-CJHSW6_LJqAQCumOdDhruggOGTmad9XLSCEAfEfJeM,15003
 resurfemg/data_connector/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/data_connector/converter_functions.py,sha256=NJZFP7ULcFMPV6ClClwntZS9L-vWzjU-4pkbxRlb2Nk,6321
 resurfemg/data_connector/tmsisdk_lite.py,sha256=J12cMVXu7OOFuN3XG_aNlkQImacPVMdV_8lQi5wu9uE,9456
 resurfemg/helper_functions/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/helper_functions/helper_functions.py,sha256=i6TKgYNX9ECS3ei2pkF3cdbkPKOiS1-bIIrClfLfmr8,13437
 resurfemg/machine_learning/ml.py,sha256=iApO8hnoAOdE_LE1h_texCi6RNXuzS18m1AMLmVeJdE,2493
 resurfemg/pipelines/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/pipelines/pipelines.py,sha256=A4ho9kzgpodbGrOZvo77Ij1nqkGSkVyN1_9f2PMyJK4,11709
 resurfemg/postprocessing/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
+resurfemg/postprocessing/baseline.py,sha256=D7tP4tLpB8MsxakQacVYmtSffkoY2wc9gcs8wfwQ14w,4891
 resurfemg/postprocessing/features.py,sha256=_KMg1H3BcpHk2MMLcRq40MkqYz4BWwA0-m-pWKfGFfI,21086
 resurfemg/preprocessing/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/preprocessing/ecg_removal.py,sha256=6anmZbqlVNUyTH_Dp-czEthkX7jzly58dphY-Nofkn8,17468
 resurfemg/preprocessing/envelope.py,sha256=2JECtSLgl53AkZJpot1zFpuTgBVykVZTiU4RS0VdO_A,6250
 resurfemg/preprocessing/filtering.py,sha256=F6ysn7C4wT1GYajxuKylv-xx6TR_vg3Q23dqwsDSu_M,12737
 resurfemg/visualization/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/visualization/visualization.py,sha256=HsZyTicyD9Zf6pHWjXZCRAhxpeYwwl5MannCOw_9UlQ,1411
-resurfemg-0.2.1.dist-info/METADATA,sha256=0vRe1Svn3wZi0UHHMqLTQ7wB9lS8IQ3hC-9nAGWz7DE,19759
-resurfemg-0.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-resurfemg-0.2.1.dist-info/top_level.txt,sha256=u30hNTZIkHnbFMEMG0n9CswHMS6bEFL6iqbq1RX6jwU,10
-resurfemg-0.2.1.dist-info/RECORD,,
+resurfemg-0.2.2a0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+resurfemg-0.2.2a0.dist-info/METADATA,sha256=JCIR13pdX9s2HghsCoJNXX1yuUFxhkjB4DEXb7hgdU8,17946
+resurfemg-0.2.2a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+resurfemg-0.2.2a0.dist-info/top_level.txt,sha256=u30hNTZIkHnbFMEMG0n9CswHMS6bEFL6iqbq1RX6jwU,10
+resurfemg-0.2.2a0.dist-info/RECORD,,
```

