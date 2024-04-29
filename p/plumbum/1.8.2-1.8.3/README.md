# Comparing `tmp/plumbum-1.8.2.tar.gz` & `tmp/plumbum-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 30 10:30:45 2023, max compression
+gzip compressed data, last modified: Mon Apr 29 06:08:30 2024, max compression
```

## Comparing `plumbum-1.8.2.tar` & `plumbum-1.8.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0      118 2023-05-30 10:30:45.000000 plumbum-1.8.2/.editorconfig
--rw-r--r--   0        0        0       35 2023-05-30 10:30:45.000000 plumbum-1.8.2/.gitattributes
--rw-r--r--   0        0        0     1289 2023-05-30 10:30:45.000000 plumbum-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      384 2023-05-30 10:30:45.000000 plumbum-1.8.2/.readthedocs.yml
--rw-r--r--   0        0        0    21952 2023-05-30 10:30:45.000000 plumbum-1.8.2/CHANGELOG.rst
--rw-r--r--   0        0        0      835 2023-05-30 10:30:45.000000 plumbum-1.8.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0      216 2023-05-30 10:30:45.000000 plumbum-1.8.2/MANIFEST.in
--rw-r--r--   0        0        0     1436 2023-05-30 10:30:45.000000 plumbum-1.8.2/noxfile.py
--rw-r--r--   0        0        0      570 2023-05-30 10:30:45.000000 plumbum-1.8.2/setup.cfg
--rwxr-xr-x   0        0        0     1066 2023-05-30 10:30:45.000000 plumbum-1.8.2/translations.py
--rw-r--r--   0        0        0      162 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      654 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2980 2023-05-30 10:30:45.000000 plumbum-1.8.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       67 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/.gitignore
--rw-r--r--   0        0        0      819 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/README.mkd
--rw-r--r--   0        0        0       51 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/bld.bat
--rw-r--r--   0        0        0       38 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/build.sh
--rw-r--r--   0        0        0      904 2023-05-30 10:30:45.000000 plumbum-1.8.2/conda.recipe/meta.yaml
--rw-r--r--   0        0        0        8 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/.gitignore
--rw-r--r--   0        0        0     5632 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/Makefile
--rw-r--r--   0        0        0     5752 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_cheatsheet.rst
--rw-r--r--   0        0        0    22722 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_color_list.html
--rw-r--r--   0        0        0     2762 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_news.rst
--rw-r--r--   0        0        0       53 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/changelog.rst
--rw-r--r--   0        0        0    25762 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/cli.rst
--rw-r--r--   0        0        0    13654 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/colorlib.rst
--rw-r--r--   0        0        0    11770 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/colors.rst
--rw-r--r--   0        0        0     8380 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/conf.py
--rw-r--r--   0        0        0     8041 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/index.rst
--rw-r--r--   0        0        0    13579 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/local_commands.rst
--rw-r--r--   0        0        0     4161 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/local_machine.rst
--rw-r--r--   0        0        0     5130 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/make.bat
--rw-r--r--   0        0        0     4211 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/paths.rst
--rw-r--r--   0        0        0     9886 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/quickref.rst
--rw-r--r--   0        0        0    10216 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/remote.rst
--rw-r--r--   0        0        0     2956 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/typed_env.rst
--rw-r--r--   0        0        0     1728 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/utils.rst
--rw-r--r--   0        0        0     2311 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/fish-text-black.png
--rw-r--r--   0        0        0     2820 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/github-logo.png
--rw-r--r--   0        0        0     9085 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo.png
--rw-r--r--   0        0        0     3413 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo2.png
--rw-r--r--   0        0        0     4527 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo3.png
--rw-r--r--   0        0        0     4147 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo4.png
--rw-r--r--   0        0        0    74592 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo6.png
--rw-r--r--   0        0        0     9700 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo7.png
--rw-r--r--   0        0        0     8599 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/logo8.png
--rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_static/placeholder
--rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/_templates/placeholder
--rw-r--r--   0        0        0      311 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/cli.rst
--rw-r--r--   0        0        0      593 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/colors.rst
--rw-r--r--   0        0        0      373 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/commands.rst
--rw-r--r--   0        0        0      156 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/fs.rst
--rw-r--r--   0        0        0      595 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/machines.rst
--rw-r--r--   0        0        0      348 2023-05-30 10:30:45.000000 plumbum-1.8.2/docs/api/path.rst
--rw-r--r--   0        0        0       75 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/.gitignore
--rw-r--r--   0        0        0    16244 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/PHSP.png
--rw-r--r--   0        0        0      504 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/SimpleColorCLI.py
--rwxr-xr-x   0        0        0      358 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/alignment.py
--rwxr-xr-x   0        0        0      704 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/color.py
--rwxr-xr-x   0        0        0     1064 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/filecopy.py
--rwxr-xr-x   0        0        0      270 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/fullcolor.py
--rwxr-xr-x   0        0        0     3363 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/geet.py
--rwxr-xr-x   0        0        0      768 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/make_figures.py
--rwxr-xr-x   0        0        0     1585 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/simple_cli.py
--rw-r--r--   0        0        0      330 2023-05-30 10:30:45.000000 plumbum-1.8.2/examples/testfigure.tex
--rw-r--r--   0        0        0     5643 2023-05-30 10:30:45.000000 plumbum-1.8.2/experiments/parallel.py
--rw-r--r--   0        0        0     1257 2023-05-30 10:30:45.000000 plumbum-1.8.2/experiments/test_parallel.py
--rw-r--r--   0        0        0     3255 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/__init__.py
--rw-r--r--   0        0        0      651 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/_testtools.py
--rw-r--r--   0        0        0      292 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cmd.py
--rw-r--r--   0        0        0      567 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colors.py
--rw-r--r--   0        0        0     2036 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/lib.py
--rw-r--r--   0        0        0     4935 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/typed_env.py
--rw-r--r--   0        0        0      160 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/version.py
--rw-r--r--   0        0        0      606 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/__init__.py
--rw-r--r--   0        0        0    38071 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/application.py
--rw-r--r--   0        0        0     3200 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/config.py
--rw-r--r--   0        0        0     1647 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n.py
--rw-r--r--   0        0        0     3346 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/image.py
--rw-r--r--   0        0        0     8348 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/progress.py
--rw-r--r--   0        0        0    21058 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/switches.py
--rw-r--r--   0        0        0     7223 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/terminal.py
--rw-r--r--   0        0        0     3109 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/termsize.py
--rw-r--r--   0        0        0     6754 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/de.po
--rw-r--r--   0        0        0     6734 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/fr.po
--rw-r--r--   0        0        0     6727 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/nl.po
--rw-r--r--   0        0        0     8070 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/ru.po
--rw-r--r--   0        0        0     3553 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     3514 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     3510 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     4836 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo
--rw-r--r--   0        0        0     1211 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/__init__.py
--rw-r--r--   0        0        0      165 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/__main__.py
--rw-r--r--   0        0        0      979 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/_ipython_ext.py
--rw-r--r--   0        0        0     6927 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/factories.py
--rw-r--r--   0        0        0     8260 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/names.py
--rw-r--r--   0        0        0    25047 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/colorlib/styles.py
--rw-r--r--   0        0        0      773 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/__init__.py
--rw-r--r--   0        0        0    19546 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/base.py
--rw-r--r--   0        0        0     3543 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/daemons.py
--rw-r--r--   0        0        0    17042 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/modifiers.py
--rw-r--r--   0        0        0    13895 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/commands/processes.py
--rw-r--r--   0        0        0       39 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/atomic.py
--rw-r--r--   0        0        0     1097 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/fs/mounts.py
--rw-r--r--   0        0        0      356 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/__init__.py
--rw-r--r--   0        0        0      727 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/_windows.py
--rw-r--r--   0        0        0     3397 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/base.py
--rw-r--r--   0        0        0     6327 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/env.py
--rw-r--r--   0        0        0    15778 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/local.py
--rw-r--r--   0        0        0    17619 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/paramiko_machine.py
--rw-r--r--   0        0        0    15941 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/remote.py
--rw-r--r--   0        0        0    11809 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/session.py
--rw-r--r--   0        0        0    15149 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/machines/ssh_machine.py
--rw-r--r--   0        0        0      395 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/__init__.py
--rw-r--r--   0        0        0    17362 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/base.py
--rw-r--r--   0        0        0    10610 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/local.py
--rw-r--r--   0        0        0    11309 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/remote.py
--rw-r--r--   0        0        0     3532 2023-05-30 10:30:45.000000 plumbum-1.8.2/plumbum/path/utils.py
--rw-r--r--   0        0        0      307 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/_test_paramiko.py
--rw-r--r--   0        0        0     4145 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/env.py
--rw-r--r--   0        0        0        0 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/file with space.txt
--rwxr-xr-x   0        0        0      145 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/slow_process.bash
--rw-r--r--   0        0        0      736 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_3_cli.py
--rw-r--r--   0        0        0    11564 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_cli.py
--rw-r--r--   0        0        0     2788 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_clicolor.py
--rw-r--r--   0        0        0     2815 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_color.py
--rw-r--r--   0        0        0     2013 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_config.py
--rw-r--r--   0        0        0     2103 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_env.py
--rw-r--r--   0        0        0     6354 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_factories.py
--rw-r--r--   0        0        0    35677 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_local.py
--rw-r--r--   0        0        0     2199 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_nohup.py
--rw-r--r--   0        0        0     1938 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_putty.py
--rw-r--r--   0        0        0    23757 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_remote.py
--rw-r--r--   0        0        0      394 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_sudo.py
--rw-r--r--   0        0        0     5266 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_terminal.py
--rw-r--r--   0        0        0     1544 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_typed_env.py
--rw-r--r--   0        0        0     1706 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_utils.py
--rw-r--r--   0        0        0     2630 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_validate.py
--rw-r--r--   0        0        0     2287 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/test_visual_color.py
--rwxr-xr-x   0        0        0       10 2023-05-30 10:30:45.000000 plumbum-1.8.2/tests/not-in-path/dummy-executable
--rw-r--r--   0        0        0     3191 2023-05-30 10:30:45.000000 plumbum-1.8.2/.gitignore
--rw-r--r--   0        0        0     1080 2023-05-30 10:30:45.000000 plumbum-1.8.2/LICENSE
--rw-r--r--   0        0        0     6920 2023-05-30 10:30:45.000000 plumbum-1.8.2/README.rst
--rw-r--r--   0        0        0     5707 2023-05-30 10:30:45.000000 plumbum-1.8.2/pyproject.toml
--rw-r--r--   0        0        0    10132 2023-05-30 10:30:45.000000 plumbum-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      118 2024-04-29 06:08:30.000000 plumbum-1.8.3/.editorconfig
+-rw-r--r--   0        0        0       35 2024-04-29 06:08:30.000000 plumbum-1.8.3/.gitattributes
+-rw-r--r--   0        0        0     1329 2024-04-29 06:08:30.000000 plumbum-1.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      425 2024-04-29 06:08:30.000000 plumbum-1.8.3/.readthedocs.yml
+-rw-r--r--   0        0        0    22501 2024-04-29 06:08:30.000000 plumbum-1.8.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      835 2024-04-29 06:08:30.000000 plumbum-1.8.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1467 2024-04-29 06:08:30.000000 plumbum-1.8.3/noxfile.py
+-rw-r--r--   0        0        0      294 2024-04-29 06:08:30.000000 plumbum-1.8.3/setup.cfg
+-rwxr-xr-x   0        0        0     1066 2024-04-29 06:08:30.000000 plumbum-1.8.3/translations.py
+-rw-r--r--   0        0        0      224 2024-04-29 06:08:30.000000 plumbum-1.8.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-29 06:08:30.000000 plumbum-1.8.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      654 2024-04-29 06:08:30.000000 plumbum-1.8.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2973 2024-04-29 06:08:30.000000 plumbum-1.8.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       67 2024-04-29 06:08:30.000000 plumbum-1.8.3/conda.recipe/.gitignore
+-rw-r--r--   0        0        0      818 2024-04-29 06:08:30.000000 plumbum-1.8.3/conda.recipe/README.mkd
+-rw-r--r--   0        0        0       51 2024-04-29 06:08:30.000000 plumbum-1.8.3/conda.recipe/bld.bat
+-rw-r--r--   0        0        0       38 2024-04-29 06:08:30.000000 plumbum-1.8.3/conda.recipe/build.sh
+-rw-r--r--   0        0        0      904 2024-04-29 06:08:30.000000 plumbum-1.8.3/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0        8 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/.gitignore
+-rw-r--r--   0        0        0     5632 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/Makefile
+-rw-r--r--   0        0        0     5752 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_cheatsheet.rst
+-rw-r--r--   0        0        0    22722 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_color_list.html
+-rw-r--r--   0        0        0     2876 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_news.rst
+-rw-r--r--   0        0        0       53 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/changelog.rst
+-rw-r--r--   0        0        0    25762 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/cli.rst
+-rw-r--r--   0        0        0    13654 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/colorlib.rst
+-rw-r--r--   0        0        0    11770 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/colors.rst
+-rw-r--r--   0        0        0     8380 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/conf.py
+-rw-r--r--   0        0        0     8031 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/index.rst
+-rw-r--r--   0        0        0    13579 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/local_commands.rst
+-rw-r--r--   0        0        0     4161 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/local_machine.rst
+-rw-r--r--   0        0        0     5130 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/make.bat
+-rw-r--r--   0        0        0     4211 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/paths.rst
+-rw-r--r--   0        0        0     9886 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/quickref.rst
+-rw-r--r--   0        0        0    10216 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/remote.rst
+-rw-r--r--   0        0        0     2956 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/typed_env.rst
+-rw-r--r--   0        0        0     1728 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/utils.rst
+-rw-r--r--   0        0        0     2311 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/fish-text-black.png
+-rw-r--r--   0        0        0     2820 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/github-logo.png
+-rw-r--r--   0        0        0     9085 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo.png
+-rw-r--r--   0        0        0     3413 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo2.png
+-rw-r--r--   0        0        0     4527 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo3.png
+-rw-r--r--   0        0        0     4147 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo4.png
+-rw-r--r--   0        0        0    74592 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo6.png
+-rw-r--r--   0        0        0     9700 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo7.png
+-rw-r--r--   0        0        0     8599 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/logo8.png
+-rw-r--r--   0        0        0        0 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_static/placeholder
+-rw-r--r--   0        0        0        0 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/_templates/placeholder
+-rw-r--r--   0        0        0      311 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/cli.rst
+-rw-r--r--   0        0        0      593 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/colors.rst
+-rw-r--r--   0        0        0      373 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/commands.rst
+-rw-r--r--   0        0        0      156 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/fs.rst
+-rw-r--r--   0        0        0      595 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/machines.rst
+-rw-r--r--   0        0        0      348 2024-04-29 06:08:30.000000 plumbum-1.8.3/docs/api/path.rst
+-rw-r--r--   0        0        0       75 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/.gitignore
+-rw-r--r--   0        0        0    16244 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/PHSP.png
+-rw-r--r--   0        0        0      504 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/SimpleColorCLI.py
+-rwxr-xr-x   0        0        0      358 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/alignment.py
+-rwxr-xr-x   0        0        0      704 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/color.py
+-rwxr-xr-x   0        0        0     1064 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/filecopy.py
+-rwxr-xr-x   0        0        0      270 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/fullcolor.py
+-rwxr-xr-x   0        0        0     3363 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/geet.py
+-rwxr-xr-x   0        0        0      768 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/make_figures.py
+-rwxr-xr-x   0        0        0     1585 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/simple_cli.py
+-rw-r--r--   0        0        0      330 2024-04-29 06:08:30.000000 plumbum-1.8.3/examples/testfigure.tex
+-rw-r--r--   0        0        0     5636 2024-04-29 06:08:30.000000 plumbum-1.8.3/experiments/parallel.py
+-rw-r--r--   0        0        0     1257 2024-04-29 06:08:30.000000 plumbum-1.8.3/experiments/test_parallel.py
+-rw-r--r--   0        0        0     3270 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/_testtools.py
+-rw-r--r--   0        0        0      292 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cmd.py
+-rw-r--r--   0        0        0      566 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colors.py
+-rw-r--r--   0        0        0     2036 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/lib.py
+-rw-r--r--   0        0        0     4913 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/typed_env.py
+-rw-r--r--   0        0        0      411 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/version.py
+-rw-r--r--   0        0        0      606 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/__init__.py
+-rw-r--r--   0        0        0    38055 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/application.py
+-rw-r--r--   0        0        0     3200 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/config.py
+-rw-r--r--   0        0        0     1661 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n.py
+-rw-r--r--   0        0        0     3347 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/image.py
+-rw-r--r--   0        0        0     8348 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/progress.py
+-rw-r--r--   0        0        0    21073 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/switches.py
+-rw-r--r--   0        0        0     7222 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/terminal.py
+-rw-r--r--   0        0        0     3079 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/termsize.py
+-rw-r--r--   0        0        0     6754 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/de.po
+-rw-r--r--   0        0        0     6734 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/fr.po
+-rw-r--r--   0        0        0     6727 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/nl.po
+-rw-r--r--   0        0        0     8070 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/ru.po
+-rw-r--r--   0        0        0     3553 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     3514 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     3510 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     4836 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo
+-rw-r--r--   0        0        0     1211 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/__main__.py
+-rw-r--r--   0        0        0      979 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/_ipython_ext.py
+-rw-r--r--   0        0        0     6926 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/factories.py
+-rw-r--r--   0        0        0     8261 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/names.py
+-rw-r--r--   0        0        0    25046 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/colorlib/styles.py
+-rw-r--r--   0        0        0      773 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/commands/__init__.py
+-rw-r--r--   0        0        0    19464 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/commands/base.py
+-rw-r--r--   0        0        0     3543 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/commands/daemons.py
+-rw-r--r--   0        0        0    17090 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/commands/modifiers.py
+-rw-r--r--   0        0        0    15047 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/commands/processes.py
+-rw-r--r--   0        0        0       39 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/fs/__init__.py
+-rw-r--r--   0        0        0     9425 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/fs/atomic.py
+-rw-r--r--   0        0        0     1097 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/fs/mounts.py
+-rw-r--r--   0        0        0      356 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/_windows.py
+-rw-r--r--   0        0        0     3397 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/base.py
+-rw-r--r--   0        0        0     6327 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/env.py
+-rw-r--r--   0        0        0    15894 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/local.py
+-rw-r--r--   0        0        0    17619 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/paramiko_machine.py
+-rw-r--r--   0        0        0    15941 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/remote.py
+-rw-r--r--   0        0        0    11809 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/session.py
+-rw-r--r--   0        0        0    15149 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/machines/ssh_machine.py
+-rw-r--r--   0        0        0      395 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/path/__init__.py
+-rw-r--r--   0        0        0    17346 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/path/base.py
+-rw-r--r--   0        0        0    10626 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/path/local.py
+-rw-r--r--   0        0        0    11309 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/path/remote.py
+-rw-r--r--   0        0        0     3532 2024-04-29 06:08:30.000000 plumbum-1.8.3/plumbum/path/utils.py
+-rw-r--r--   0        0        0      307 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/_test_paramiko.py
+-rw-r--r--   0        0        0     4145 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/conftest.py
+-rw-r--r--   0        0        0      368 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/env.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/file with space.txt
+-rwxr-xr-x   0        0        0      145 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/slow_process.bash
+-rw-r--r--   0        0        0      736 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_3_cli.py
+-rw-r--r--   0        0        0    11564 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2788 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_clicolor.py
+-rw-r--r--   0        0        0     2815 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_color.py
+-rw-r--r--   0        0        0     2013 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_config.py
+-rw-r--r--   0        0        0     2103 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_env.py
+-rw-r--r--   0        0        0     6354 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_factories.py
+-rw-r--r--   0        0        0    35803 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_local.py
+-rw-r--r--   0        0        0     2199 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_nohup.py
+-rw-r--r--   0        0        0     2524 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_pipelines.py
+-rw-r--r--   0        0        0     1938 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_putty.py
+-rw-r--r--   0        0        0    23705 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_remote.py
+-rw-r--r--   0        0        0      394 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_sudo.py
+-rw-r--r--   0        0        0     5266 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_terminal.py
+-rw-r--r--   0        0        0     1544 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_typed_env.py
+-rw-r--r--   0        0        0     1706 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_utils.py
+-rw-r--r--   0        0        0     2630 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_validate.py
+-rw-r--r--   0        0        0     2287 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/test_visual_color.py
+-rwxr-xr-x   0        0        0       10 2024-04-29 06:08:30.000000 plumbum-1.8.3/tests/not-in-path/dummy-executable
+-rw-r--r--   0        0        0     3191 2024-04-29 06:08:30.000000 plumbum-1.8.3/.gitignore
+-rw-r--r--   0        0        0     1080 2024-04-29 06:08:30.000000 plumbum-1.8.3/LICENSE
+-rw-r--r--   0        0        0     6920 2024-04-29 06:08:30.000000 plumbum-1.8.3/README.rst
+-rw-r--r--   0        0        0     5854 2024-04-29 06:08:30.000000 plumbum-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0    10132 2024-04-29 06:08:30.000000 plumbum-1.8.3/PKG-INFO
```

### Comparing `plumbum-1.8.2/.pre-commit-config.yaml` & `plumbum-1.8.3/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: "v4.4.0"
+  rev: "v4.6.0"
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
     exclude: ^conda.recipe/meta.yaml$
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
-- repo: https://github.com/psf/black
-  rev: "23.3.0"
-  hooks:
-  - id: black
-
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.270"
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: "v0.4.2"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
+    - id: ruff-format
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v1.3.0"
+  rev: "v1.10.0"
   hooks:
   - id: mypy
     files: plumbum
     args: []
-    additional_dependencies: [typed-ast, types-paramiko, types-setuptools]
+    additional_dependencies: [typed-ast, types-paramiko, types-setuptools, pytest]
 
 - repo: https://github.com/abravalheri/validate-pyproject
-  rev: "v0.13"
+  rev: "v0.16"
   hooks:
   - id: validate-pyproject
 
 - repo: https://github.com/codespell-project/codespell
-  rev: "v2.2.4"
+  rev: "v2.2.6"
   hooks:
   - id: codespell
+    args: ["-w"]
+    additional_dependencies: [tomli]
+    exclude: "(^pyproject.toml|.po)$"
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: "v1.10.0"
   hooks:
   - id: rst-backticks
   - id: rst-directive-colons
   - id: rst-inline-touching-normal
```

### Comparing `plumbum-1.8.2/CHANGELOG.rst` & `plumbum-1.8.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+1.8.3
+-----
+
+* Fix StdinDataRedirection's formulate() method by @nebbish in https://github.com/tomerfiliba/plumbum/pull/629
+* Missing non-zero return code from TEE'd pipe by @vient in https://github.com/tomerfiliba/plumbum/pull/661
+* Fix stalling in Pipeline command by @astaric in https://github.com/tomerfiliba/plumbum/pull/632
+* Use high-speed method for C locale too by @henryiii in https://github.com/tomerfiliba/plumbum/pull/681
+* Update index.rst - fix broken link for sh project by @mcint in https://github.com/tomerfiliba/plumbum/pull/658
+
 1.8.2
 -----
 
 * Fix author metadata on PyPI package and add static check (`#648 <https://github.com/tomerfiliba/plumbum/pull/648>`_)
 * Add testing for Python 3.12 beta 1 (`#650 <https://github.com/tomerfiliba/plumbum/pull/650>`_)
 * Use Ruff for linting (`#643 <https://github.com/tomerfiliba/plumbum/pull/643>`_)
 * Paths: Add type hinting for Path (`#646 <https://github.com/tomerfiliba/plumbum/pull/646>`_)
```

### Comparing `plumbum-1.8.2/CONTRIBUTING.rst` & `plumbum-1.8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/noxfile.py` & `plumbum-1.8.3/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 @nox.session
 def pylint(session):
     """
     Run pylint.
     """
 
-    session.install(".", "paramiko", "ipython", "pylint~=2.17.4")
+    session.install(".", "paramiko", "ipython", "pylint~=3.1.0")
     session.run("pylint", "plumbum", *session.posargs)
 
 
 @nox.session(python=ALL_PYTHONS, reuse_venv=True)
 def tests(session):
     """
     Run the unit and regular tests.
     """
     session.install("-e", ".[dev]")
-    session.run("pytest", *session.posargs)
+    session.run("pytest", *session.posargs, env={"PYTHONTRACEMALLOC": "5"})
 
 
 @nox.session(reuse_venv=True)
 def docs(session):
     """
     Build the docs. Pass "serve" to serve.
     """
```

### Comparing `plumbum-1.8.2/translations.py` & `plumbum-1.8.3/translations.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/.github/matchers/pylint.json` & `plumbum-1.8.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/.github/workflows/cd.yml` & `plumbum-1.8.3/.github/workflows/cd.yml`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,29 @@
   FORCE_COLOR: 3
 
 jobs:
   dist:
     name: Dist
     runs-on: ubuntu-22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
-    - uses: hynek/build-and-inspect-python-package@v1
+    - uses: hynek/build-and-inspect-python-package@v2
 
   deploy:
     name: Deploy
     runs-on: ubuntu-22.04
     needs: [dist]
     if: github.event_name == 'release' && github.event.action == 'published'
     environment: pypi
     permissions:
       id-token: write
 
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
         name: Packages
         path: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `plumbum-1.8.2/.github/workflows/ci.yml` & `plumbum-1.8.3/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,56 +16,56 @@
 
 jobs:
 
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: "3.x"
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
     - name: pylint
       run: |
         echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
         pipx run --python python nox -s pylint
 
   tests:
     name: Tests on 🐍 ${{ matrix.python-version }} ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.6", "3.8", "3.11", "3.12-dev"]
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.6", "3.8", "3.11", "3.12"]
+        os: [ubuntu-latest, windows-latest, macos-13]
         include:
         - python-version: 'pypy-3.8'
           os: ubuntu-latest
-        - python-version: 'pypy-3.9'
+        - python-version: 'pypy-3.10'
           os: ubuntu-latest
         - python-version: '3.6'
           os: ubuntu-20.04
         exclude:
         - python-version: '3.6'
           os: ubuntu-latest
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
-    - uses: actions/cache@v3
+    - uses: actions/cache@v4
       if: runner.os == 'Linux' && startsWith(matrix.python-version, 'pypy')
       with:
         path: ~/.cache/pip
         key: ${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('setup.cfg') }}
         restore-keys: |
           ${{ runner.os }}-${{ matrix.python-version }}-pip-
 
@@ -98,15 +98,15 @@
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         COVERALLS_FLAG_NAME: test-${{ matrix.os }}-${{ matrix.python-version }}
 
   coverage:
     needs: [tests]
     runs-on: ubuntu-22.04
     steps:
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install coveralls
       run: pip install coveralls
     - name: Coveralls Finished
       run: coveralls --service=github --finish
       env:
```

### Comparing `plumbum-1.8.2/conda.recipe/README.mkd` & `plumbum-1.8.3/conda.recipe/README.mkd`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Building instructions
 
 
-Change to the `conda.recipies` directory. Run
+Change to the `conda.recipes` directory. Run
 ```bash
 $ conda install conda-build
 ```
 to acquire the conda build tools. Then you can build with
 ```bash
 conda build --python 3.5 .
 ```
```

### Comparing `plumbum-1.8.2/conda.recipe/meta.yaml` & `plumbum-1.8.3/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/Makefile` & `plumbum-1.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_cheatsheet.rst` & `plumbum-1.8.3/docs/_cheatsheet.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_color_list.html` & `plumbum-1.8.3/docs/_color_list.html`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_news.rst` & `plumbum-1.8.3/docs/_news.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+* **2023.05.30**: Version 1.8.2 released with a PyPI metadata fix, Python 3.12b1 testing, and a bit more typing.
+
 * **2023.01.01**: Version 1.8.1 released with hatchling replacing setuptools for the build system, and support for Path objects in local.
 
 * **2022.10.05**: Version 1.8.0 released with ``NO_COLOR``/``FORCE_COLOR``, ``all_markers`` & future annotations for the CLI, some command enhancements, & Python 3.11 testing.
 
 * **2021.12.23**: Version 1.7.2 released with very minor fixes, final version to support Python 2.7 and 3.5.
 
 * **2021.11.23**: Version 1.7.1 released with a few features like reverse tunnels, color group titles, and a glob path fix. Better Python 3.10 support.
```

### Comparing `plumbum-1.8.2/docs/cli.rst` & `plumbum-1.8.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/colorlib.rst` & `plumbum-1.8.3/docs/colorlib.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/colors.rst` & `plumbum-1.8.3/docs/colors.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/conf.py` & `plumbum-1.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/index.rst` & `plumbum-1.8.3/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 to make it happen. Plumbum was born from the scraps of the ``Path`` class, which I
 wrote for the aforementioned build system, and the ``SshContext`` and ``SshTunnel`` classes
 that I wrote for `RPyC <https://rpyc.readthedocs.io/>`_. When I combined the two with *shell combinators*
 (because shell scripts do have an edge there) the magic happened and here we are.
 
 Credits
 =======
-The project has been inspired by **PBS** (now called `sh <http://amoffat.github.io/sh/>`_)
+The project has been inspired by **PBS** (now called `sh <http://sh.rtfd.org>`_)
 of `Andrew Moffat <https://github.com/amoffat>`_,
 and has borrowed some of his ideas (namely treating programs like functions and the
 nice trick for importing commands). However, I felt there was too much magic going on in PBS,
 and that the syntax wasn't what I had in mind when I came to write shell-like programs.
 I contacted Andrew about these issues, but he wanted to keep PBS this way. Other than that,
 the two libraries go in different directions, where Plumbum attempts to provide a more
 wholesome approach.
```

#### html2text {}

```diff
@@ -76,15 +76,15 @@
 been working on that I decided I've had it with shell scripts and it's time to
 make it happen. Plumbum was born from the scraps of the ``Path`` class, which I
 wrote for the aforementioned build system, and the ``SshContext`` and
 ``SshTunnel`` classes that I wrote for `RPyC
 rpyc.readthedocs.io/>`_. When I combined the two with *shell combinators*
 (because shell scripts do have an edge there) the magic happened and here we
 are. Credits ======= The project has been inspired by **PBS** (now called `sh
-amoffat.github.io/sh/>`_) of `Andrew Moffat
+sh.rtfd.org>`_) of `Andrew Moffat
 github.com/amoffat>`_, and has borrowed some of his ideas (namely treating
 programs like functions and the nice trick for importing commands). However, I
 felt there was too much magic going on in PBS, and that the syntax wasn't what
 I had in mind when I came to write shell-like programs. I contacted Andrew
 about these issues, but he wanted to keep PBS this way. Other than that, the
 two libraries go in different directions, where Plumbum attempts to provide a
 more wholesome approach. Plumbum also pays tribute to `Rotem Yaari
```

### Comparing `plumbum-1.8.2/docs/local_commands.rst` & `plumbum-1.8.3/docs/local_commands.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/local_machine.rst` & `plumbum-1.8.3/docs/local_machine.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/make.bat` & `plumbum-1.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/paths.rst` & `plumbum-1.8.3/docs/paths.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/quickref.rst` & `plumbum-1.8.3/docs/quickref.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/remote.rst` & `plumbum-1.8.3/docs/remote.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/typed_env.rst` & `plumbum-1.8.3/docs/typed_env.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/utils.rst` & `plumbum-1.8.3/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/fish-text-black.png` & `plumbum-1.8.3/docs/_static/fish-text-black.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/github-logo.png` & `plumbum-1.8.3/docs/_static/github-logo.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo.png` & `plumbum-1.8.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo2.png` & `plumbum-1.8.3/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo3.png` & `plumbum-1.8.3/docs/_static/logo3.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo4.png` & `plumbum-1.8.3/docs/_static/logo4.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo6.png` & `plumbum-1.8.3/docs/_static/logo6.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo7.png` & `plumbum-1.8.3/docs/_static/logo7.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/_static/logo8.png` & `plumbum-1.8.3/docs/_static/logo8.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/api/colors.rst` & `plumbum-1.8.3/docs/api/colors.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/docs/api/machines.rst` & `plumbum-1.8.3/docs/api/machines.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/PHSP.png` & `plumbum-1.8.3/examples/PHSP.png`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/color.py` & `plumbum-1.8.3/examples/color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/filecopy.py` & `plumbum-1.8.3/examples/filecopy.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/geet.py` & `plumbum-1.8.3/examples/geet.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/make_figures.py` & `plumbum-1.8.3/examples/make_figures.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/examples/simple_cli.py` & `plumbum-1.8.3/examples/simple_cli.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/experiments/parallel.py` & `plumbum-1.8.3/experiments/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,15 @@
 
     def path(self, *parts):
         return [mach.path(*parts) for mach in self]
 
     def __getitem__(self, progname):
         if not isinstance(progname, str):
             raise TypeError(
-                "progname must be a string, not %r"
-                % (
+                "progname must be a string, not {!r}".format(
                     type(
                         progname,
                     )
                 )
             )
         return ConcurrentCommand(*(mach[progname] for mach in self))
 
@@ -162,15 +161,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, t, v, tb):
         self.close()
 
     def __del__(self):
-        try:  # noqa: 167
+        try:  # noqa: SIM105
             self.close()
         except Exception:
             pass
 
     def alive(self):
         """Returns ``True`` if the underlying shells are all alive, ``False`` otherwise"""
         return all(session.alive for session in self)
```

### Comparing `plumbum-1.8.2/experiments/test_parallel.py` & `plumbum-1.8.3/experiments/test_parallel.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/__init__.py` & `plumbum-1.8.3/plumbum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 # ===================================================================================================
 # Module hack: ``from plumbum.cmd import ls``
 # Can be replaced by a real module with __getattr__ after Python 3.6 is dropped
 # ===================================================================================================
 
 
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 7):  # noqa: UP036
     from types import ModuleType
     from typing import List
 
     class LocalModule(ModuleType):
         """The module-hack that allows us to use ``from plumbum.cmd import some_program``"""
 
         __all__ = ()  # to make help() happy
```

### Comparing `plumbum-1.8.2/plumbum/_testtools.py` & `plumbum-1.8.3/plumbum/_testtools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import platform
 import sys
 
-import pytest  # type: ignore[import]
+import pytest
 
 skip_without_chown = pytest.mark.skipif(
     not hasattr(os, "chown"), reason="os.chown not supported"
 )
 
 skip_without_tty = pytest.mark.skipif(not sys.stdin.isatty(), reason="Not a TTY")
```

### Comparing `plumbum-1.8.2/plumbum/colors.py` & `plumbum-1.8.3/plumbum/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 This module imitates a real module, providing standard syntax
 like from `plumbum.colors` and from `plumbum.colors.bg` to work alongside
 all the standard syntax for colors.
 """
 
-
 import atexit
 import sys
 
 from plumbum.colorlib import ansicolors, main
 
 _reset = ansicolors.reset.now
 if __name__ == "__main__":
```

### Comparing `plumbum-1.8.2/plumbum/lib.py` & `plumbum-1.8.3/plumbum/lib.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/typed_env.py` & `plumbum-1.8.3/plumbum/typed_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,15 @@
 
     class CSV(_BaseVar):
         """
         Comma-separated-strings get split using the ``separator`` (',' by default) into
         a list of objects of type ``type`` (``str`` by default).
         """
 
-        def __init__(
-            self, name, default=NO_DEFAULT, type=str, separator=","
-        ):  # pylint:disable=redefined-builtin
+        def __init__(self, name, default=NO_DEFAULT, type=str, separator=","):  # pylint:disable=redefined-builtin
             super().__init__(name, default=default)
             self.type = type
             self.separator = separator
 
         def __set__(self, instance, value):
             instance[self.name] = self.separator.join(map(str, value))
```

### Comparing `plumbum-1.8.2/plumbum/cli/__init__.py` & `plumbum-1.8.3/plumbum/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/application.py` & `plumbum-1.8.3/plumbum/cli/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
             for item in m.annotations:
                 annotation = (
                     sig.parameters[item].annotation
                     if item != "return"
                     else sig.return_annotation
                 )
                 if sys.version_info < (3, 10) and isinstance(annotation, str):
-                    annotation = eval(annotation)  # noqa: PGH001
+                    annotation = eval(annotation)
                 if item == m.varargs:
                     varargs = annotation
                 elif item != "return":
                     positional[args_names.index(item)] = annotation
 
             tailargs = self._positional_validate(
                 tailargs, positional, varargs, m.args[1:], m.varargs
```

### Comparing `plumbum-1.8.2/plumbum/cli/config.py` & `plumbum-1.8.3/plumbum/cli/config.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n.py` & `plumbum-1.8.3/plumbum/cli/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import locale
 
 # High performance method for English (no translation needed)
 loc = locale.getlocale()[0]
-if loc is None or loc.startswith("en"):
+if loc is None or loc.startswith("en") or loc == "C":
 
     class NullTranslation:
         def gettext(self, str1: str) -> str:  # pylint: disable=no-self-use
             return str1
 
         def ngettext(self, str1, strN, n):  # pylint: disable=no-self-use
             if n == 1:
```

### Comparing `plumbum-1.8.2/plumbum/cli/image.py` & `plumbum-1.8.3/plumbum/cli/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             sys.stdout.write(colors.reset + " \n")
         sys.stdout.write(colors.reset + "\n")
         sys.stdout.flush()
 
 
 class ShowImageApp(cli.Application):
     "Display an image on the terminal"
+
     double = cli.Flag(
         ["-d", "--double"], help="Double resolution (looks good only with some fonts)"
     )
 
     @cli.switch(["-c", "--colors"], cli.Range(1, 4), help="Level of color, 1-4")
     def colors_set(self, n):  # pylint: disable=no-self-use
         colors.use_color = n
```

### Comparing `plumbum-1.8.2/plumbum/cli/progress.py` & `plumbum-1.8.3/plumbum/cli/progress.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/switches.py` & `plumbum-1.8.3/plumbum/cli/switches.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,16 @@
         names,
         argtype=str,
         default=None,
         list=False,  # pylint: disable=redefined-builtin
         argname=VALUE,
         **kwargs,
     ):
-        self.__doc__ = "Sets an attribute"  # to prevent the help message from showing SwitchAttr's docstring
+        # Setting to prevent the help message from showing SwitchAttr's docstring
+        self.__doc__ = "Sets an attribute"
         if default and argtype is not None:
             defaultmsg = _("; the default is {0}").format(default)
             if "help" in kwargs:
                 kwargs["help"] += defaultmsg
             else:
                 kwargs["help"] = defaultmsg.lstrip("; ")
```

### Comparing `plumbum-1.8.2/plumbum/cli/terminal.py` & `plumbum-1.8.3/plumbum/cli/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Terminal-related utilities
 --------------------------
 """
 
-
 import contextlib
 import os
 import sys
 from typing import List, Optional
 
 from plumbum import local
```

### Comparing `plumbum-1.8.2/plumbum/cli/termsize.py` & `plumbum-1.8.3/plumbum/cli/termsize.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 def _ioctl_GWINSZ(fd: int) -> Optional[Tuple[int, int]]:
     yx = Struct("hh")
     try:
         import fcntl
         import termios
 
         # TODO: Clean this up. Problems could be hidden by the broad except.
-        return yx.unpack(fcntl.ioctl(fd, termios.TIOCGWINSZ, b"1234"))  # type: ignore[return-value]
+        return yx.unpack(fcntl.ioctl(fd, termios.TIOCGWINSZ, b"1234"))
     except Exception:
         return None
 
 
 def _get_terminal_size_linux() -> Optional[Tuple[int, int]]:
     cr = _ioctl_GWINSZ(0) or _ioctl_GWINSZ(1) or _ioctl_GWINSZ(2)
     if not cr:
```

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/de.po` & `plumbum-1.8.3/plumbum/cli/i18n/de.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/fr.po` & `plumbum-1.8.3/plumbum/cli/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/nl.po` & `plumbum-1.8.3/plumbum/cli/i18n/nl.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/ru.po` & `plumbum-1.8.3/plumbum/cli/i18n/ru.po`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.3/plumbum/cli/i18n/de/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.3/plumbum/cli/i18n/fr/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.3/plumbum/cli/i18n/nl/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo` & `plumbum-1.8.3/plumbum/cli/i18n/ru/LC_MESSAGES/plumbum.cli.mo`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/colorlib/__init__.py` & `plumbum-1.8.3/plumbum/colorlib/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/colorlib/_ipython_ext.py` & `plumbum-1.8.3/plumbum/colorlib/_ipython_ext.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/colorlib/factories.py` & `plumbum-1.8.3/plumbum/colorlib/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Color-related factories. They produce Styles.
 """
 
-
 import functools
 import operator
 import sys
 from typing import Any
 
 from .names import color_names, default_styles
 from .styles import ColorNotFound
```

### Comparing `plumbum-1.8.2/plumbum/colorlib/names.py` & `plumbum-1.8.3/plumbum/colorlib/names.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Names for the standard and extended color set.
 Extended set is similar to `vim wiki <http://vim.wikia.com/wiki/Xterm256_color_names_for_console_Vim>`_, `colored <https://pypi.python.org/pypi/colored>`_, etc. Colors based on `wikipedia <https://en.wikipedia.org/wiki/ANSI_escape_code#Colors>`_.
 
 You can access the index of the colors with names.index(name). You can access the
 rgb values with ``r=int(html[n][1:3],16)``, etc.
 """
+
 from typing import Tuple
 
 color_names = """\
 black
 red
 green
 yellow
```

### Comparing `plumbum-1.8.2/plumbum/colorlib/styles.py` & `plumbum-1.8.3/plumbum/colorlib/styles.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 ``Color`` is rarely used directly,
 but merely provides the workhorse for finding and manipulating colors.
 
 With the ``Style`` class, any color can be directly called or given to a with statement.
 """
 
-
 import contextlib
 import os
 import platform
 import re
 import sys
 from abc import ABCMeta, abstractmethod
 from copy import copy
```

### Comparing `plumbum-1.8.2/plumbum/commands/__init__.py` & `plumbum-1.8.3/plumbum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/commands/base.py` & `plumbum-1.8.3/plumbum/commands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,16 +394,14 @@
             src_kwargs["stdin"] = kwargs["stdin"]
 
         srcproc = self.srccmd.popen(args, **src_kwargs)
         kwargs["stdin"] = srcproc.stdout
         dstproc = self.dstcmd.popen(**kwargs)
         # allow p1 to receive a SIGPIPE if p2 exits
         srcproc.stdout.close()
-        if srcproc.stderr is not None:
-            dstproc.stderr = srcproc.stderr
         if srcproc.stdin and src_kwargs.get("stdin") != PIPE:
             srcproc.stdin.close()
         dstproc.srcproc = srcproc
 
         # monkey-patch .wait() to wait on srcproc as well (it's expected to die when dstproc dies)
         dstproc_wait = dstproc.wait
 
@@ -532,15 +530,15 @@
     def _get_encoding(self):
         return self.cmd._get_encoding()
 
     def formulate(self, level=0, args=()):
         return [
             f"echo {shquote(self.data)}",
             "|",
-            self.cmd.formulate(level + 1, args),
+            *self.cmd.formulate(level + 1, args),
         ]
 
     @property
     def machine(self):
         return self.cmd.machine
 
     def popen(self, args=(), **kwargs):
```

### Comparing `plumbum-1.8.2/plumbum/commands/daemons.py` & `plumbum-1.8.3/plumbum/commands/daemons.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/commands/modifiers.py` & `plumbum-1.8.3/plumbum/commands/modifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 
                         # And then "unbuffered" is just flushing after each write
                         if not self.buffered:
                             tee_to[fd].flush()
 
                         buf.append(data)
 
+            p.wait()  # To get return code in p
             stdout = "".join([x.decode("utf-8") for x in outbuf])
             stderr = "".join([x.decode("utf-8") for x in errbuf])
             return p.returncode, stdout, stderr
 
 
 class _TF(ExecutionModifier):
     """
```

### Comparing `plumbum-1.8.2/plumbum/commands/processes.py` & `plumbum-1.8.3/plumbum/commands/processes.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,22 +14,52 @@
 # utility functions
 # ===================================================================================================
 def _check_process(proc, retcode, timeout, stdout, stderr):
     proc.verify(retcode, timeout, stdout, stderr)
     return proc.returncode, stdout, stderr
 
 
+def _get_piped_streams(proc):
+    """Get a list of all valid standard streams for proc that were opened with PIPE option.
+
+    If proc was started from a Pipeline command, this function assumes it will have a
+    "srcproc" member pointing to the previous command in the pipeline. That link will
+    be used to traverse all started processes started from the pipeline, the list will
+    include stdout/stderr streams opened as PIPE for all commands in the pipeline.
+    If that was not the case, some processes could write to pipes no one reads from
+    which would result in process stalling after the pipe's buffer is filled.
+
+    Streams that were closed (because they were redirected to the input of a subsequent command)
+    are not included in the result
+    """
+    streams = []
+
+    def add_stream(type_, stream):
+        if stream is None or stream.closed:
+            return
+        streams.append((type_, stream))
+
+    while proc:
+        add_stream(1, proc.stderr)
+        add_stream(0, proc.stdout)
+        proc = getattr(proc, "srcproc", None)
+
+    return streams
+
+
 def _iter_lines_posix(proc, decode, linesize, line_timeout=None):
     from selectors import EVENT_READ, DefaultSelector
 
+    streams = _get_piped_streams(proc)
+
     # Python 3.4+ implementation
     def selector():
         sel = DefaultSelector()
-        sel.register(proc.stdout, EVENT_READ, 0)
-        sel.register(proc.stderr, EVENT_READ, 1)
+        for stream_type, stream in streams:
+            sel.register(stream, EVENT_READ, stream_type)
         while True:
             ready = sel.select(line_timeout)
             if not ready and line_timeout:
                 raise ProcessLineTimedOut(
                     "popen line timeout expired",
                     getattr(proc, "argv", None),
                     getattr(proc, "machine", None),
@@ -37,18 +67,17 @@
             for key, _mask in ready:
                 yield key.data, decode(key.fileobj.readline(linesize))
 
     for ret in selector():
         yield ret
         if proc.poll() is not None:
             break
-    for line in proc.stdout:
-        yield 0, decode(line)
-    for line in proc.stderr:
-        yield 1, decode(line)
+    for stream_type, stream in streams:
+        for line in stream:
+            yield stream_type, decode(line)
 
 
 def _iter_lines_win32(proc, decode, linesize, line_timeout=None):
     class Piper(Thread):
         def __init__(self, fd, pipe):
             super().__init__(name=f"PlumbumPiper{fd}Thread")
             self.pipe = pipe
@@ -110,15 +139,15 @@
     match the expected result, this exception is raised by :func:`run_proc
     <plumbum.commands.run_proc>`. It contains the process' return code, stdout, and stderr, as
     well as the command line used to create the process (``argv``)
     """
 
     def __init__(self, argv, retcode, stdout, stderr, message=None, *, host=None):
         # we can't use 'super' here since OSError only keeps the first 2 args,
-        # which leads to failuring in loading this object from a pickle.dumps.
+        # which leads to failing in loading this object from a pickle.dumps.
         # pylint: disable-next=non-parent-init-called
         Exception.__init__(self, argv, retcode, stdout, stderr)
 
         self.message = message
         self.host = host
         self.argv = argv
         self.retcode = retcode
@@ -337,28 +366,28 @@
 
     :param line_timeout: The maximal amount of time (in seconds) to allow between consecutive lines in either stream.
                     Raise an :class:`ProcessLineTimedOut <plumbum.commands.ProcessLineTimedOut>` if the timeout has
                     been reached. ``None`` means no timeout is imposed.
 
     :param buffer_size: Maximum number of lines to keep in the stdout/stderr buffers, in case of a ProcessExecutionError.
                     Default is ``None``, which defaults to DEFAULT_BUFFER_SIZE (which is infinite by default).
-                    ``0`` will disable bufferring completely.
+                    ``0`` will disable buffering completely.
 
     :param mode: Controls what the generator yields. Defaults to DEFAULT_ITER_LINES_MODE (which is BY_POSITION by default)
                 - BY_POSITION (default): yields ``(out, err)`` line tuples, where either item may be ``None``
                 - BY_TYPE: yields ``(fd, line)`` tuples, where ``fd`` is 1 (stdout) or 2 (stderr)
 
     :returns: An iterator of (out, err) line tuples.
     """
     if mode is None:
         mode = DEFAULT_ITER_LINES_MODE
 
     if buffer_size is None:
         buffer_size = DEFAULT_BUFFER_SIZE
-    buffer_size: int
+    buffer_size: int  # type: ignore[annotation-unchecked]
 
     assert mode in (BY_POSITION, BY_TYPE)
 
     encoding = getattr(proc, "custom_encoding", None) or "utf-8"
     decode = lambda s: s.decode(encoding, errors="replace").rstrip()  # noqa: E731
 
     _register_proc_timeout(proc, timeout)
```

### Comparing `plumbum-1.8.2/plumbum/fs/atomic.py` & `plumbum-1.8.3/plumbum/fs/atomic.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/fs/mounts.py` & `plumbum-1.8.3/plumbum/fs/mounts.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/_windows.py` & `plumbum-1.8.3/plumbum/machines/_windows.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/base.py` & `plumbum-1.8.3/plumbum/machines/base.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/env.py` & `plumbum-1.8.3/plumbum/machines/env.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/local.py` & `plumbum-1.8.3/plumbum/machines/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,16 +255,18 @@
         new_session=False,
         **kwargs,
     ):
         if new_session:
             kwargs["start_new_session"] = True
 
         if IS_WIN32 and "startupinfo" not in kwargs and stdin not in (sys.stdin, None):
+            # pylint: disable-next=used-before-assignment
             subsystem = get_pe_subsystem(str(executable))
 
+            # pylint: disable-next=used-before-assignment
             if subsystem == IMAGE_SUBSYSTEM_WINDOWS_CUI:
                 # don't open a new console
                 sui = subprocess.STARTUPINFO()
                 kwargs["startupinfo"] = sui
                 if hasattr(subprocess, "_subprocess"):
                     sui.dwFlags |= (
                         subprocess._subprocess.STARTF_USESHOWWINDOW
```

### Comparing `plumbum-1.8.2/plumbum/machines/paramiko_machine.py` & `plumbum-1.8.3/plumbum/machines/paramiko_machine.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/remote.py` & `plumbum-1.8.3/plumbum/machines/remote.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/session.py` & `plumbum-1.8.3/plumbum/machines/session.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/machines/ssh_machine.py` & `plumbum-1.8.3/plumbum/machines/ssh_machine.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/path/base.py` & `plumbum-1.8.3/plumbum/path/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return f"<{self.__class__.__name__} {self}>"
 
     def __truediv__(self: _PathImpl, other: typing.Any) -> _PathImpl:
         """Joins two paths"""
         return self.join(other)
 
     def __getitem__(self, key):
-        if type(key) == str or isinstance(key, Path):
+        if type(key) == str or isinstance(key, Path):  # noqa: E721
             return self / key
         return str(self)[key]
 
     def __floordiv__(self, expr):
         """Returns a (possibly empty) list of paths that matched the glob-pattern under this path"""
         return self.glob(expr)
 
@@ -415,18 +415,16 @@
 
     @staticmethod
     def _glob(pattern, fn):
         """Applies a glob string or list/tuple/iterable to the current path, using ``fn``"""
         if isinstance(pattern, str):
             return fn(pattern)
 
-        results = []
-        for single_pattern in pattern:
-            results.extend(fn(single_pattern))
-        return sorted(list(set(results)))
+        results = {value for single_pattern in pattern for value in fn(single_pattern)}
+        return sorted(results)
 
     def resolve(self, strict=False):  # noqa: ARG002
         """Added to allow pathlib like syntax. Does nothing since
         Plumbum paths are always absolute. Does not (currently) resolve
         symlinks."""
         # TODO: Resolve symlinks here
         return self
```

### Comparing `plumbum-1.8.2/plumbum/path/local.py` & `plumbum-1.8.3/plumbum/path/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                     os.mkdir(str(self), mode)
             except OSError as ex:  # pragma: no cover
                 # directory might already exist (a race with other threads/processes)
                 if ex.errno != errno.EEXIST or not exist_ok:
                     raise
 
     def open(self, mode="r", encoding=None):
-        return open(
+        return open(  # noqa: SIM115
             str(self),
             mode,
             encoding=encoding,
         )
 
     def read(self, encoding=None, mode="r"):
         if encoding and "b" not in mode:
```

### Comparing `plumbum-1.8.2/plumbum/path/remote.py` & `plumbum-1.8.3/plumbum/path/remote.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/plumbum/path/utils.py` & `plumbum-1.8.3/plumbum/path/utils.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/conftest.py` & `plumbum-1.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_3_cli.py` & `plumbum-1.8.3/tests/test_3_cli.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_cli.py` & `plumbum-1.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_clicolor.py` & `plumbum-1.8.3/tests/test_clicolor.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_color.py` & `plumbum-1.8.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_config.py` & `plumbum-1.8.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_env.py` & `plumbum-1.8.3/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_factories.py` & `plumbum-1.8.3/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_local.py` & `plumbum-1.8.3/tests/test_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -603,27 +603,33 @@
             for i, (out, err) in enumerate(cmd.popen().iter_lines(line_timeout=0.2)):
                 print(i, "out:", out)
                 print(i, "err:", err)
         assert i == 1
 
     @skip_on_windows
     def test_modifiers(self):
-        from plumbum.cmd import grep, ls
+        from plumbum.cmd import cat, grep, ls
 
         f = (ls["-a"] | grep["\\.py"]) & BG
         f.wait()
         assert "test_local.py" in f.stdout.splitlines()
 
         command = ls["-a"] | grep["local"]
         command_false = ls["-a"] | grep["not_a_file_here"]
+        command_false_2 = command_false | cat
         command & FG
         assert command & TF
         assert not (command_false & TF)
+        assert not (command_false_2 & TF)
         assert command & RETCODE == 0
         assert command_false & RETCODE == 1
+        assert command_false_2 & RETCODE == 1
+        assert (command & TEE)[0] == 0
+        assert (command_false & TEE(retcode=None))[0] == 1
+        assert (command_false_2 & TEE(retcode=None))[0] == 1
 
     @skip_on_windows
     def test_tee_modifier(self, capfd):
         from plumbum.cmd import echo
 
         result = echo["This is fun"] & TEE
         assert result[1] == "This is fun\n"
@@ -898,24 +904,22 @@
 
     @skip_on_windows
     def test_atomic_counter(self):
         local.path("counter").delete()
         num_of_procs = 20
         num_of_increments = 20
 
-        code = """from plumbum.fs.atomic import AtomicCounterFile
+        code = f"""from plumbum.fs.atomic import AtomicCounterFile
 import time
 time.sleep(0.2)
 afc = AtomicCounterFile.open("counter")
-for _ in range({}):
+for _ in range({num_of_increments}):
     print(afc.next())
     time.sleep(0.1)
-""".format(
-            num_of_increments,
-        )
+"""
 
         procs = []
         for _ in range(num_of_procs):
             procs.append(local.python["-c", code].popen())
         results = []
         for p in procs:
             out, _ = p.communicate()
@@ -1044,18 +1048,14 @@
 
 class TestLocalEncoding:
     try:
         richstr = unichr(40960)
     except NameError:
         richstr = chr(40960)
 
-    @pytest.mark.xfail(
-        IS_WIN32,
-        reason="Unicode output on Windows does not work (Python 3.6+ was supposed to work)",
-    )
     def test_inout_rich(self):
         from plumbum.cmd import echo
 
         out = echo(self.richstr)
         assert self.richstr in out
 
     @pytest.mark.usefixtures("cleandir")
```

### Comparing `plumbum-1.8.2/tests/test_nohup.py` & `plumbum-1.8.3/tests/test_nohup.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_putty.py` & `plumbum-1.8.3/tests/test_putty.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_remote.py` & `plumbum-1.8.3/tests/test_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,22 +524,20 @@
                 assert tun.lport == lport
                 if not dynamic_dport:
                     assert tun.dport == remote_socket
                 else:
                     assert_is_port(tun.dport)
                 assert tun.reverse
 
-                remote_send_af_inet = """import socket
+                remote_send_af_inet = f"""import socket
 s = socket.socket()
-s.connect(("localhost", {}))
-s.send("{}".encode("ascii"))
+s.connect(("localhost", {tun.dport}))
+s.send("{message}".encode("ascii"))
 s.close()
-""".format(
-                    tun.dport, message
-                )
+"""
                 (rem.python["-u"] << remote_send_af_inet).popen()
                 tunnel_server.join(timeout=1)
                 assert queue.get() == message
 
     def test_get(self):
         with self._connect() as rem:
             assert str(rem["ls"]) == str(rem.get("ls"))
@@ -634,19 +632,19 @@
                 pytest.fail("Should not pipe")
 
     @pytest.mark.xfail(message="Not working yet")
     def test_encoding(self):
         with self._connect() as rem:
             unicode_half = b"\xc2\xbd".decode("utf8")
 
-            ret = rem["bash"]("-c", 'echo -e "\xC2\xBD"')
-            assert ret == "%s\n" % unicode_half
+            ret = rem["bash"]("-c", 'echo -e "\xc2\xbd"')
+            assert ret == f"{unicode_half}\n"
 
-            ret = list(rem["bash"]["-c", 'echo -e "\xC2\xBD"'].popen())
-            assert ret == [["%s\n" % unicode_half, None]]
+            ret = list(rem["bash"]["-c", 'echo -e "\xc2\xbd"'].popen())
+            assert ret == [[f"{unicode_half}\n", None]]
 
     def test_path_open_remote_write_local_read(self):
         with self._connect() as rem:
             with rem.tempdir() as remote_tmpdir, local.tempdir() as tmpdir:
                 assert remote_tmpdir.is_dir()
                 assert tmpdir.is_dir()
                 data = b"hello world"
```

### Comparing `plumbum-1.8.2/tests/test_terminal.py` & `plumbum-1.8.3/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_typed_env.py` & `plumbum-1.8.3/tests/test_typed_env.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_utils.py` & `plumbum-1.8.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_validate.py` & `plumbum-1.8.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/tests/test_visual_color.py` & `plumbum-1.8.3/tests/test_visual_color.py`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/.gitignore` & `plumbum-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/LICENSE` & `plumbum-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/README.rst` & `plumbum-1.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `plumbum-1.8.2/pyproject.toml` & `plumbum-1.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "plumbum/version.py"
 
 
 [tool.mypy]
 files = ["plumbum"]
-python_version = "3.6"
+python_version = "3.8"
 warn_unused_configs = true
 warn_unused_ignores = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "truthy-bool"]
 disallow_any_generics = false
 disallow_subclassing_any = false
 disallow_untyped_calls = false
@@ -100,21 +100,23 @@
 
 [[tool.mypy.overrides]]
 module = ["IPython.*", "pywintypes.*", "win32con.*", "win32file.*", "PIL.*", "plumbum.cmd.*", "ipywidgets.*", "traitlets.*", "plumbum.version"]
 ignore_missing_imports = true
 
 
 [tool.pytest.ini_options]
+testpaths = ["tests"]
 minversion = "6.0"
-addopts = ["-ra", "--cov-config=setup.cfg", "--strict-markers", "--strict-config"]
+addopts = ["-ra", "--showlocals", "--cov-config=setup.cfg", "--strict-markers", "--strict-config"]
 norecursedirs = ["examples", "experiments"]
 filterwarnings = [
   "always"
 ]
 log_cli_level = "info"
+xfail_strict = true
 required_plugins = ["pytest-timeout", "pytest-mock"]
 timeout = 300
 optional_tests = """
   ssh: requires self ssh access to run
   sudo: requires sudo access to run
 """
 
@@ -163,17 +165,20 @@
   "eval-used",  # Needed for Python <3.10 annotations
   "unused-argument", # Covered by ruff
   "global-statement", # Covered by ruff
   "pointless-statement", # Covered by ruff
 ]
 
 [tool.ruff]
-select = [
-  "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
+target-version = "py37"
+exclude = ["docs/conf.py"]
+
+[tool.ruff.lint]
+extend-select = [
+  "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
   "PIE",         # flake8-pie
@@ -181,28 +186,29 @@
   "PT",          # flake8-pytest-style
   "RET",         # flake8-return
   "RUF",         # Ruff-specific
   "SIM",         # flake8-simplify
   "T20",         # flake8-print
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
-
 ]
-extend-ignore = [
+ignore = [
   "E501",
   "PLR",
   "PT004",
   "PT011",  # TODO: add match parameter
-  "PLC1901", # Simplify == "", might be risky
+  "RUF012",  # ClassVar required if mutable
+  "ISC001",  # conflicts with formatter
 ]
-target-version = "py37"
-exclude = ["docs/conf.py"]
-mccabe.max-complexity = 50
 flake8-unused-arguments.ignore-variadic-names = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "examples/*" = ["T20"]
 "experiments/*" = ["T20"]
 "tests/*" = ["T20"]
 "plumbum/cli/application.py" = ["T20"]
 "plumbum/commands/base.py" = ["SIM115"]
 "plumbum/commands/daemons.py" = ["SIM115"]
+
+[tool.codespell]
+ignore-words-list = "ans,switchs,hart,ot,twoo,fo"
+skip = "*.po"
```

### Comparing `plumbum-1.8.2/PKG-INFO` & `plumbum-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: plumbum
-Version: 1.8.2
+Version: 1.8.3
 Summary: Plumbum: shell combinators library
 Project-URL: Homepage, https://github.com/tomerfiliba/plumbum
 Project-URL: Documentation, https://plumbum.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/tomerfiliba/plumbum/issues
 Project-URL: Changelog, https://plumbum.readthedocs.io/en/latest/changelog.html
 Project-URL: Cheatsheet, https://plumbum.readthedocs.io/en/latest/quickref.html
 Author-email: Tomer Filiba <tomerfiliba@gmail.com>
```

