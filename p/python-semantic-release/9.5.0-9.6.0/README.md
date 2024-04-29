# Comparing `tmp/python_semantic_release-9.5.0.tar.gz` & `tmp/python_semantic_release-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_semantic_release-9.5.0.tar", last modified: Tue Apr 23 02:38:39 2024, max compression
+gzip compressed data, was "python_semantic_release-9.6.0.tar", last modified: Mon Apr 29 04:29:51 2024, max compression
```

## Comparing `python_semantic_release-9.5.0.tar` & `python_semantic_release-9.6.0.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/
--rw-r--r--   0 root         (0) root         (0)      230 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.131866 python_semantic_release-9.5.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.131866 python_semantic_release-9.5.0/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    15332 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    13289 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    28291 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3501 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8866 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9146 2024-04-23 02:38:33.000000 python_semantic_release-9.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5538 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.135866 python_semantic_release-9.5.0/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-04-23 02:38:33.000000 python_semantic_release-9.5.0/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.135866 python_semantic_release-9.5.0/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4087 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1703 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    23015 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    17574 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2609 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4393 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5777 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.123866 python_semantic_release-9.5.0/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5232 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)    11004 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    11450 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    19965 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     7409 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11360 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    28853 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     8953 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13292 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)     4494 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6222 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.155866 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5840 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.155866 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5952 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    10521 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    27246 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    35951 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    15576 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     5551 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.993059 python_semantic_release-9.6.0/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-29 04:29:50.993059 python_semantic_release-9.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.965059 python_semantic_release-9.6.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.969059 python_semantic_release-9.6.0/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    17609 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    16256 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    28291 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8869 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9146 2024-04-29 04:29:45.000000 python_semantic_release-9.6.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.993059 python_semantic_release-9.6.0/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 04:29:50.000000 python_semantic_release-9.6.0/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.969059 python_semantic_release-9.6.0/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-29 04:29:45.000000 python_semantic_release-9.6.0/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.969059 python_semantic_release-9.6.0/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.973059 python_semantic_release-9.6.0/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.973059 python_semantic_release-9.6.0/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    24488 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    20389 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.977059 python_semantic_release-9.6.0/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.957059 python_semantic_release-9.6.0/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.977059 python_semantic_release-9.6.0/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.977059 python_semantic_release-9.6.0/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11152 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    18287 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/remote_hvcs_base.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.977059 python_semantic_release-9.6.0/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 04:29:50.997059 python_semantic_release-9.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.981059 python_semantic_release-9.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.981059 python_semantic_release-9.6.0/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    30551 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.981059 python_semantic_release-9.6.0/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    12976 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.981059 python_semantic_release-9.6.0/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.981059 python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.985059 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.989059 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.989059 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.989059 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27795 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    36478 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:29:50.993059 python_semantic_release-9.6.0/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-04-29 04:28:31.000000 python_semantic_release-9.6.0/tests/util.py
```

### Comparing `python_semantic_release-9.5.0/LICENSE` & `python_semantic_release-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/PKG-INFO` & `python_semantic_release-9.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.5.0
+Version: 9.6.0
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
```

### Comparing `python_semantic_release-9.5.0/README.rst` & `python_semantic_release-9.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/Makefile` & `python_semantic_release-9.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/algorithm.rst` & `python_semantic_release-9.6.0/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.6.0/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.6.0/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/automatic-releases/index.rst` & `python_semantic_release-9.6.0/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/automatic-releases/travis.rst` & `python_semantic_release-9.6.0/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/changelog_templates.rst` & `python_semantic_release-9.6.0/docs/changelog_templates.rst`

 * *Files 10% similar despite different names*

```diff
@@ -140,39 +140,77 @@
 You may wish to leverage this behaviour to modularise your changelog template, to
 define macros in a separate file, or to reference static data which you would like
 to avoid duplicating between your template environment and the remainder of your
 project.
 
 .. _changelog-templates-template-rendering-template-context:
 
-Template Context:
-^^^^^^^^^^^^^^^^^
+Template Context
+^^^^^^^^^^^^^^^^
 
 Alongside the rendering of a directory tree, Python Semantic Release makes information
 about the history of the project available within the templating environment in order
 for it to be used to generate Changelogs and other such documents.
 
 The history of the project is made available via the global variable ``context``. In
 Python terms, ``context`` is a `dataclass`_ with the following attributes:
 
 * ``repo_name: str``: the name of the current repository parsed from the Git url.
 * ``repo_owner: str``: the owner of the current repository parsed from the Git url.
+* ``hvcs_type: str``: the name of the VCS server type currently configured.
 * ``history: ReleaseHistory``: a :py:class:`semantic_release.changelog.ReleaseHistory` instance.
   (See :ref:`changelog-templates-template-rendering-template-context-release-history`)
 * ``filters: Tuple[Callable[..., Any], ...]``: a tuple of filters for the template environment.
   These are added to the environment's ``filters``, and therefore there should be no need to
   access these from the ``context`` object inside the template.
 
-Currently, two filters are defined:
+The filters provided vary based on the VCS configured and available features:
+
+* ``create_server_url: Callable[[str, str | None, str | None, str | None], str]``: when given
+  a path, prepend the configured vcs server host and url scheme.  Optionally you can provide,
+  a auth string, a query string or a url fragment to be normalized into the resulting url.
+  Parameter order is as described above respectively.
+
+* ``create_repo_url: Callable[[str, str | None, str | None], str]``: when given a repository
+  path, prepend the configured vcs server host, and repo namespace.  Optionally you can provide,
+  an additional query string and/or a url fragment to also put in the url. Parameter order is
+  as described above respectively. This is similar to ``create_server_url`` but includes the repo
+  namespace and owner automatically.
 
-* ``pull_request_url: Callable[[str], str]``: given a pull request number, return a URL
-  to the pull request in the remote.
 * ``commit_hash_url: Callable[[str], str]``: given a commit hash, return a URL to the
   commit in the remote.
 
+* ``compare_url: Callable[[str, str], str]``: given a starting git reference and a ending git
+  reference create a comparison url between the two references that can be opened on the remote
+
+* ``issue_url: Callable[[str | int], str]``: given an issue number, return a URL to the issue
+  on the remote vcs.
+
+* ``merge_request_url: Callable[[str | int], str]``: given a merge request number, return a URL
+  to the merge request in the remote. This is an alias to the ``pull_request_url`` but only
+  available for the VCS that uses the merge request terminology.
+
+* ``pull_request_url: Callable[[str | int], str]``: given a pull request number, return a URL
+  to the pull request in the remote. For remote vcs' that use merge request terminology, this
+  filter is an alias to the ``merge_request_url`` filter function.
+
+Availability of the documented filters can be found in the table below:
+
+======================  =========  =====  ======  ======
+**filter - hvcs_type**  bitbucket  gitea  github  gitlab
+======================  =========  =====  ======  ======
+create_server_url          ✅       ✅      ✅      ✅
+create_repo_url            ✅       ✅      ✅      ✅
+commit_hash_url            ✅       ✅      ✅      ✅
+compare_url                ✅       ❌      ✅      ✅
+issue_url                  ❌       ✅      ✅      ✅
+merge_request_url          ❌       ❌      ❌      ✅
+pull_request_url           ✅       ✅      ✅      ✅
+======================  =========  =====  ======  ======
+
 .. seealso::
    * `Filters <https://jinja.palletsprojects.com/en/3.1.x/templates/#filters>`_
 
 .. _changelog-templates-template-rendering-template-context-release-history:
 
 ``ReleaseHistory``
 """"""""""""""""""
```

### Comparing `python_semantic_release-9.5.0/docs/commands.rst` & `python_semantic_release-9.6.0/docs/commands.rst`

 * *Files 11% similar despite different names*

```diff
@@ -169,47 +169,118 @@
 
 Same as the :ref:`cmd-version-option-print-last-released` flag but prints the
 complete tag name (ex. ``v1.0.0`` or ``py-v1.0.0``) instead of the raw version
 number (``1.0.0``).
 
 .. _cmd-version-option-force-level:
 
-``--major/--minor/--patch``
-***************************
+``--major/--minor/--patch/--prerelease``
+****************************************
 
-Force the next version to increment the major, minor or patch digit, respectively.
-These flags are optional but mutually exclusive, so only one may be supplied, or none at all.
-Using these flags overrides the usual calculation for the next version; this can be useful, say,
-when a project wants to release its initial 1.0.0 version.
+Force the next version to increment the major, minor or patch digits, or the prerelease revision,
+respectively. These flags are optional but mutually exclusive, so only one may be supplied, or
+none at all. Using these flags overrides the usual calculation for the next version; this can
+be useful, say, when a project wants to release its initial 1.0.0 version.
 
 .. warning::
-    Using these flags will override the value of prerelease, **regardless of your configuration or the
-    current version**. To produce a prerelease with the appropriate digit incremented you should also
-    supply the :ref:`cmd-version-option-prerelease` flag. If you do not, using these flags will force
+
+    Using these flags will override the configured value of ``prerelease`` (configured
+    in your :ref:`Release Group<multibranch-releases-configuring>`),
+    **regardless of your configuration or the current version**.
+
+    To produce a prerelease with the appropriate digit incremented you should also
+    supply the :ref:`cmd-version-option-as-prerelease` flag. If you do not, using these flags will force
     a full (non-prerelease) version to be created.
 
+For example, suppose your project's current version is ``0.2.1-rc.1``. The following
+shows how these options can be combined with ``--as-prerelease`` to force different
+versions:
+
+.. code-block:: bash
+
+   semantic-release version --prerelease --print
+   # 0.2.1-rc.2
+
+   semantic-release version --patch --print
+   # 0.2.2
+
+   semantic-release version --minor --print
+   # 0.3.0
+
+   semantic-release version --major --print
+   # 1.0.0
+
+   semantic-release version --minor --as-prerelease --print
+   # 0.3.0-rc.1
+
+   semantic-release version --prerelease --as-prerelease --print
+   # 0.2.1-rc.2
+
 These options are forceful overrides, but there is no action required for subsequent releases
 performed using the usual calculation algorithm.
 
+Supplying ``--prerelease`` will cause Python Semantic Release to scan your project history
+for any previous prereleases with the same major, minor and patch versions as the latest
+version and the same :ref:`prerelease token<cmd-version-option-prerelease-token>` as the
+one passed by command-line or configuration. If one is not found, ``--prerelease`` will
+produce the next version according to the following format:
+
+.. code-block:: python
+
+    f"{latest_version.major}.{latest_version.minor}.{latest_version.patch}-{prerelease_token}.1"
+
+However, if Python Semantic Release identifies a previous *prerelease* version with the same
+major, minor and patch digits as the latest version, *and* the same prerelease token as the
+one supplied by command-line or configuration, then Python Semantic Release will increment
+the revision found on that previous prerelease version in its new version.
+
+For example, if ``"0.2.1-rc.1"`` and already exists as a previous version, and the latest version
+is ``"0.2.1"``, invoking the following command will produce ``"0.2.1-rc.2"``:
+
+.. code-block:: bash
+
+   semantic-release version --prerelease --prerelease-token "rc" --print
+
+.. warning::
+
+   This is true irrespective of the branch from which ``"0.2.1-rc.1"`` was released from.
+   The check for previous prereleases "leading up to" this normal version is intended to
+   help prevent collisions in git tags to an extent, but isn't foolproof. As the example
+   shows it is possible to release a prerelease for a normal version that's already been
+   released when using this flag, which would in turn be ignored by tools selecting
+   versions by `SemVer precedence rules`_.
+
+
+.. _SemVer precedence rules: https://semver.org/#spec-item-11
+
+
 .. seealso::
     - :ref:`configuration`
     - :ref:`config-branches`
 
-.. _cmd-version-option-prerelease:
+.. _cmd-version-option-as-prerelease:
 
-``--prerelease``
-****************
+``--as-prerelease``
+*******************
 
-Force the next version to be a prerelease. As with :ref:`cmd-version-option-force-level`, this option
+After performing the normal calculation of the next version, convert the resulting next version
+to a prerelease before applying it. As with :ref:`cmd-version-option-force-level`, this option
 is a forceful override, but no action is required to resume calculating versions as normal on the
-subsequent releases.
+subsequent releases. The main distinction between ``--prerelease`` and ``--as-prerelease`` is that
+the latter will not *force* a new version if one would not have been released without supplying
+the flag.
+
+This can be useful when making a single prerelease on a branch that would typically release
+normal versions.
 
 If not specified in :ref:`cmd-version-option-prerelease-token`, the prerelease token is idenitified using the
 :ref:`Multibranch Release Configuration <multibranch-releases-configuring>`
 
+See the examples alongside :ref:`cmd-version-option-force-level` for how to use this flag.
+
 .. _cmd-version-option-prerelease-token:
 
 ``--prerelease-token [VALUE]``
 ******************************
 
 Force the next version to use the value as the prerelease token. This overrides the configured value if one is
 present. If not used during a release producing a prerelease version, this option has no effect.
```

### Comparing `python_semantic_release-9.5.0/docs/commit-parsing.rst` & `python_semantic_release-9.6.0/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/conf.py` & `python_semantic_release-9.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/configuration.rst` & `python_semantic_release-9.6.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/github-action.rst` & `python_semantic_release-9.6.0/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/index.rst` & `python_semantic_release-9.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/make.bat` & `python_semantic_release-9.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/migrating_from_v7.rst` & `python_semantic_release-9.6.0/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/multibranch_releases.rst` & `python_semantic_release-9.6.0/docs/multibranch_releases.rst`

 * *Files 1% similar despite different names*

```diff
@@ -159,9 +159,9 @@
    semantic-release version \
       --build-metadata "$(git branch --show-current).$(date +%Y%m%d)"
 
 This would lead to versions such as ``1.1.1+main.20221127`` or ``2.0.0-rc.4+2.x.x.20221201``.
 
 .. note::
    Remember that is always possible to override the release rules configured by using
-   the :ref:`cmd-version-option-force-level` and :ref:`cmd-version-option-prerelease`
+   the :ref:`cmd-version-option-force-level` and :ref:`cmd-version-option-as-prerelease`
    flags.
```

### Comparing `python_semantic_release-9.5.0/docs/strict_mode.rst` & `python_semantic_release-9.6.0/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/docs/troubleshooting.rst` & `python_semantic_release-9.6.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/pyproject.toml` & `python_semantic_release-9.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.5.0"
+version = "9.6.0"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
```

### Comparing `python_semantic_release-9.5.0/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.6.0/python_semantic_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.5.0
+Version: 9.6.0
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
```

### Comparing `python_semantic_release-9.5.0/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.6.0/python_semantic_release.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 semantic_release/data/templates/release_notes.md.j2
 semantic_release/hvcs/__init__.py
 semantic_release/hvcs/_base.py
 semantic_release/hvcs/bitbucket.py
 semantic_release/hvcs/gitea.py
 semantic_release/hvcs/github.py
 semantic_release/hvcs/gitlab.py
+semantic_release/hvcs/remote_hvcs_base.py
 semantic_release/hvcs/token_auth.py
 semantic_release/hvcs/util.py
 semantic_release/version/__init__.py
 semantic_release/version/algorithm.py
 semantic_release/version/declaration.py
 semantic_release/version/translator.py
 semantic_release/version/version.py
@@ -109,30 +110,30 @@
 tests/scenario/test_next_version.py
 tests/scenario/test_release_history.py
 tests/scenario/test_template_render.py
 tests/unit/__init__.py
 tests/unit/semantic_release/__init__.py
 tests/unit/semantic_release/test_helpers.py
 tests/unit/semantic_release/changelog/__init__.py
+tests/unit/semantic_release/changelog/test_changelog_context.py
 tests/unit/semantic_release/changelog/test_default_changelog.py
 tests/unit/semantic_release/changelog/test_release_notes.py
 tests/unit/semantic_release/changelog/test_template.py
 tests/unit/semantic_release/cli/__init__.py
 tests/unit/semantic_release/cli/test_config.py
 tests/unit/semantic_release/cli/test_github_actions_output.py
 tests/unit/semantic_release/cli/test_masking_filter.py
 tests/unit/semantic_release/cli/test_util.py
 tests/unit/semantic_release/cli/test_version.py
 tests/unit/semantic_release/commit_parser/__init__.py
-tests/unit/semantic_release/commit_parser/helper.py
 tests/unit/semantic_release/commit_parser/test_angular.py
 tests/unit/semantic_release/commit_parser/test_emoji.py
+tests/unit/semantic_release/commit_parser/test_parsed_commit.py
 tests/unit/semantic_release/commit_parser/test_scipy.py
 tests/unit/semantic_release/commit_parser/test_tag.py
-tests/unit/semantic_release/commit_parser/test_token.py
 tests/unit/semantic_release/commit_parser/test_util.py
 tests/unit/semantic_release/hvcs/__init__.py
 tests/unit/semantic_release/hvcs/test__base.py
 tests/unit/semantic_release/hvcs/test_bitbucket.py
 tests/unit/semantic_release/hvcs/test_gitea.py
 tests/unit/semantic_release/hvcs/test_github.py
 tests/unit/semantic_release/hvcs/test_gitlab.py
```

### Comparing `python_semantic_release-9.5.0/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.6.0/python_semantic_release.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/__init__.py` & `python_semantic_release-9.6.0/semantic_release/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.5.0"
+__version__ = "9.6.0"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python_semantic_release-9.5.0/semantic_release/changelog/context.py` & `python_semantic_release-9.6.0/semantic_release/changelog/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from semantic_release.hvcs._base import HvcsBase
 
 
 @dataclass
 class ChangelogContext:
     repo_name: str
     repo_owner: str
+    hvcs_type: str
     history: ReleaseHistory
     filters: tuple[Callable[..., Any], ...] = ()
 
     def bind_to_environment(self, env: Environment) -> Environment:
         env.globals["context"] = self
         for f in self.filters:
             env.filters[f.__name__] = f
@@ -27,9 +28,10 @@
 def make_changelog_context(
     hvcs_client: HvcsBase, release_history: ReleaseHistory
 ) -> ChangelogContext:
     return ChangelogContext(
         repo_name=hvcs_client.repo_name,
         repo_owner=hvcs_client.owner,
         history=release_history,
-        filters=(hvcs_client.pull_request_url, hvcs_client.commit_hash_url),
+        hvcs_type=hvcs_client.__class__.__name__.lower(),
+        filters=(*hvcs_client.get_changelog_context_filters(),),
     )
```

### Comparing `python_semantic_release-9.5.0/semantic_release/changelog/release_history.py` & `python_semantic_release-9.6.0/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/changelog/template.py` & `python_semantic_release-9.6.0/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/changelog.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from semantic_release.changelog.context import make_changelog_context
 from semantic_release.cli.common import (
     get_release_notes_template,
     render_default_changelog_file,
     render_release_notes,
 )
 from semantic_release.cli.util import noop_report
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 
 if TYPE_CHECKING:
     from semantic_release.cli.commands.cli_context import CliContextObj
     from semantic_release.version import Version
 
 log = logging.getLogger(__name__)
 
@@ -75,15 +76,15 @@
             noop_report(
                 f"would have recursively rendered the template directory "
                 f"{template_dir!r} relative to {repo.working_dir!r}"
             )
         else:
             recursive_render(template_dir, environment=env, _root_dir=repo.working_dir)
 
-    if release_tag:
+    if release_tag and isinstance(hvcs_client, RemoteHvcsBase):
         if runtime.global_cli_options.noop:
             noop_report(
                 f"would have posted changelog to the release for tag {release_tag}"
             )
 
         # note: the following check ensures 'version is not None', but mypy can't follow
         version: Version = translator.from_tag(release_tag)  # type: ignore[assignment]
```

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/main.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import TYPE_CHECKING
 
 import click
 
 from semantic_release.cli.util import noop_report
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 from semantic_release.version import tags_and_versions
 
 if TYPE_CHECKING:
     from semantic_release.cli.commands.cli_context import CliContextObj
 
 
 log = logging.getLogger(__name__)
@@ -41,14 +42,21 @@
         try:
             tag = str(tags_and_versions(repo.tags, translator)[0][0])
         except IndexError:
             ctx.fail(
                 f"No tags found with format {translator.tag_format!r}, couldn't "
                 "identify latest version"
             )
+
+    if not isinstance(hvcs_client, RemoteHvcsBase):
+        log.info(
+            "Remote does not support artifact upload. Exiting with no action taken..."
+        )
+        ctx.exit(0)
+
     if runtime.global_cli_options.noop:
         noop_report(
             "would have uploaded files matching any of the globs "
             + ", ".join(repr(g) for g in dist_glob_patterns)
             + " to a remote VCS release, if supported"
         )
         ctx.exit(0)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/commands/version.py` & `python_semantic_release-9.6.0/semantic_release/cli/commands/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     render_release_notes,
 )
 from semantic_release.cli.github_actions_output import VersionGitHubActionsOutput
 from semantic_release.cli.util import indented, noop_report, rprint
 from semantic_release.const import DEFAULT_SHELL, DEFAULT_VERSION
 from semantic_release.enums import LevelBump
 from semantic_release.errors import UnexpectedResponse
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 from semantic_release.version import Version, next_version, tags_and_versions
 
 log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import ContextManager, Iterable
 
@@ -37,45 +38,79 @@
 
     from semantic_release.cli.commands.cli_context import CliContextObj
     from semantic_release.version import VersionTranslator
     from semantic_release.version.declaration import VersionDeclarationABC
 
 
 def is_forced_prerelease(
-    force_prerelease: bool, force_level: str | None, prerelease: bool
+    as_prerelease: bool, forced_level_bump: LevelBump | None, prerelease: bool
 ) -> bool:
     """
     Determine if this release is forced to have prerelease on/off.
     If ``force_prerelease`` is set then yes.
     Otherwise if we are forcing a specific level bump without force_prerelease,
     it's False.
     Otherwise (``force_level is None``) use the value of ``prerelease``
     """
-    log.debug(", ".join(f"{k} = {v}" for k, v in locals().items()))
-    return force_prerelease or ((force_level is None) and prerelease)
+    local_vars = list(locals().items())
+    log.debug(
+        "%s: %s",
+        is_forced_prerelease.__name__,
+        ", ".join(f"{k} = {v}" for k, v in local_vars),
+    )
+    return (
+        as_prerelease
+        or forced_level_bump is LevelBump.PRERELEASE_REVISION
+        or ((forced_level_bump is None) and prerelease)
+    )
 
 
 def last_released(
     repo: Repo, translator: VersionTranslator
 ) -> tuple[Tag, Version] | None:
     ts_and_vs = tags_and_versions(repo.tags, translator)
     return ts_and_vs[0] if ts_and_vs else None
 
 
 def version_from_forced_level(
-    repo: Repo, level_bump: LevelBump, translator: VersionTranslator
+    repo: Repo, forced_level_bump: LevelBump, translator: VersionTranslator
 ) -> Version:
     ts_and_vs = tags_and_versions(repo.tags, translator)
 
     # If we have no tags, return the default version
     if not ts_and_vs:
-        return Version.parse(DEFAULT_VERSION).bump(level_bump)
+        return Version.parse(DEFAULT_VERSION).bump(forced_level_bump)
 
     _, latest_version = ts_and_vs[0]
-    return latest_version.bump(level_bump)
+    if forced_level_bump is not LevelBump.PRERELEASE_REVISION:
+        return latest_version.bump(forced_level_bump)
+
+    # We need to find the latest version with the prerelease token
+    # we're looking for, and return that version + an increment to
+    # the prerelease revision.
+
+    # NOTE this can probably be cleaned up.
+    # ts_and_vs are in order, so check if we're looking at prereleases
+    # for the same (major, minor, patch) as the latest version.
+    # If we are, we can increment the revision and we're done. If
+    # we don't find a prerelease targeting this version with the same
+    # token as the one we're looking to prerelease, we can use revision 1.
+    for _, version in ts_and_vs:
+        if not (
+            version.major == latest_version.major
+            and version.minor == latest_version.minor
+            and version.patch == latest_version.patch
+        ):
+            break
+        if (
+            version.is_prerelease
+            and version.prerelease_token == translator.prerelease_token
+        ):
+            return version.bump(LevelBump.PRERELEASE_REVISION)
+    return latest_version.to_prerelease(token=translator.prerelease_token, revision=1)
 
 
 def apply_version_to_source_files(
     repo: Repo,
     version_declarations: Iterable[VersionDeclarationABC],
     version: Version,
     noop: bool = False,
@@ -141,42 +176,48 @@
 )
 @optgroup.option(
     "--print-last-released-tag",
     is_flag=True,
     help="Print the last released version tag and exit",
 )
 @click.option(
-    "--prerelease",
-    "force_prerelease",
+    "--as-prerelease",
+    "as_prerelease",
     is_flag=True,
-    help="Force the next version to be a prerelease",
+    help="Ensure the next version to be released is a prerelease version",
 )
 @click.option(
     "--prerelease-token",
     "prerelease_token",
     default=None,
     help="Force the next version to use this prerelease token, if it is a prerelease",
 )
 @click.option(
     "--major",
     "force_level",
     flag_value="major",
-    help="force the next version to be a major release",
+    help="Force the next version to be a major release",
 )
 @click.option(
     "--minor",
     "force_level",
     flag_value="minor",
-    help="force the next version to be a minor release",
+    help="Force the next version to be a minor release",
 )
 @click.option(
     "--patch",
     "force_level",
     flag_value="patch",
-    help="force the next version to be a patch release",
+    help="Force the next version to be a patch release",
+)
+@click.option(
+    "--prerelease",
+    "force_level",
+    flag_value="prerelease_revision",
+    help="Force the next version to be a prerelease",
 )
 @click.option(
     "--commit/--no-commit",
     "commit_changes",
     default=True,
     help="Whether or not to commit changes locally",
 )
@@ -220,15 +261,15 @@
 @click.pass_obj
 def version(  # noqa: C901
     cli_ctx: CliContextObj,
     print_only: bool = False,
     print_only_tag: bool = False,
     print_last_released: bool = False,
     print_last_released_tag: bool = False,
-    force_prerelease: bool = False,
+    as_prerelease: bool = False,
     prerelease_token: str | None = None,
     force_level: str | None = None,
     commit_changes: bool = True,
     create_tag: bool = True,
     update_changelog: bool = True,
     push_changes: bool = True,
     make_vcs_release: bool = True,
@@ -267,17 +308,18 @@
             if print_last_released_tag:
                 click.echo(last_release[0])
         else:
             log.warning("No release tags found.")
         ctx.exit(0)
 
     parser = runtime.commit_parser
+    forced_level_bump = None if not force_level else LevelBump.from_string(force_level)
     prerelease = is_forced_prerelease(
-        force_prerelease=force_prerelease,
-        force_level=force_level,
+        as_prerelease=as_prerelease,
+        forced_level_bump=forced_level_bump,
         prerelease=runtime.prerelease,
     )
     hvcs_client = runtime.hvcs_client
     changelog_file = runtime.changelog_file
     changelog_excluded_commit_patterns = runtime.changelog_excluded_commit_patterns
     env = runtime.template_environment
     template_dir = runtime.template_dir
@@ -302,31 +344,27 @@
         log.info("new tag will not be pushed because --no-tag disables pushing")
         push_changes &= create_tag
     # Only make a release if we're pushing the changes
     if make_vcs_release and not push_changes:
         log.info("No vcs release will be created because pushing changes is disabled")
         make_vcs_release &= push_changes
 
-    if force_prerelease:
-        log.warning("Forcing prerelease due to '--prerelease' command-line flag")
-    elif force_level:
+    if forced_level_bump:
         log.warning(
-            "Forcing prerelease=False due to '--%s' command-line flag and no "
-            "'--prerelease' flag",
+            "Forcing a '%s' release due to '--%s' command-line flag",
             force_level,
-        )
-
-    if force_level:
-        level_bump = LevelBump.from_string(force_level)
-        log.warning(
-            "Forcing a %s level bump due to '--force' command-line option", force_level
+            (
+                force_level
+                if forced_level_bump is not LevelBump.PRERELEASE_REVISION
+                else "prerelease"
+            ),
         )
 
         new_version = version_from_forced_level(
-            repo=repo, level_bump=level_bump, translator=translator
+            repo=repo, forced_level_bump=forced_level_bump, translator=translator
         )
 
         # We only turn the forced version into a prerelease if the user has specified
         # that that is what they want on the command-line; otherwise we assume they are
         # forcing a full release
         new_version = (
             new_version.to_prerelease(token=translator.prerelease_token)
@@ -343,14 +381,25 @@
             major_on_zero=major_on_zero,
             allow_zero_version=runtime.allow_zero_version,
         )
 
     if build_metadata:
         new_version.build_metadata = build_metadata
 
+    if as_prerelease:
+        before_conversion, new_version = (
+            new_version,
+            new_version.to_prerelease(token=translator.prerelease_token),
+        )
+        log.info(
+            "Converting %s to %s due to '--as-prerelease' command-line option",
+            before_conversion,
+            new_version,
+        )
+
     gha_output.released = False
     gha_output.version = new_version
     ctx.call_on_close(gha_output.write_if_possible)
 
     # Print the new version so that command-line output capture will work
     if print_only_tag:
         click.echo(translator.str_to_tag(str(new_version)))
@@ -597,15 +646,15 @@
             # Resolves issue #803 where a tag that already existed was pushed and caused
             # a failure. Its not clear why there was an incorrect tag (likely user error change)
             # but we will avoid possibly pushing an separate tag that we didn't create.
             repo.git.push(remote_url, "tag", new_version.as_tag())
 
     gha_output.released = True
 
-    if make_vcs_release:
+    if make_vcs_release and isinstance(hvcs_client, RemoteHvcsBase):
         if opts.noop:
             noop_report(
                 f"would have created a release for the tag {new_version.as_tag()!r}"
             )
 
         release = rh.released[new_version]
         # Use a new, non-configurable environment for release notes -
@@ -626,18 +675,19 @@
         if opts.noop:
             noop_report(
                 "would have created the following release notes: \n" + release_notes
             )
             noop_report(f"would have uploaded the following assets: {runtime.assets}")
         else:
             try:
-                release_id = hvcs_client.create_or_update_release(
+                hvcs_client.create_release(
                     tag=new_version.as_tag(),
                     release_notes=release_notes,
                     prerelease=new_version.is_prerelease,
+                    assets=assets,
                 )
             except HTTPError as err:
                 log.exception(err)
                 ctx.fail(str.join("\n", [str(err), "Failed to create release!"]))
             except UnexpectedResponse as err:
                 log.exception(err)
                 ctx.fail(
@@ -650,19 +700,8 @@
                         ],
                     )
                 )
             except Exception as e:
                 log.exception(e)
                 ctx.fail(str(e))
 
-            for asset in assets:
-                log.info("Uploading asset %s", asset)
-                try:
-                    hvcs_client.upload_asset(release_id, asset)
-                except HTTPError as err:
-                    log.exception(err)
-                    ctx.fail(str.join("\n", [str(err), "Failed to upload asset!"]))
-                except Exception as e:
-                    log.exception(e)
-                    ctx.fail(str(e))
-
     return str(new_version)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/common.py` & `python_semantic_release-9.6.0/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/config.py` & `python_semantic_release-9.6.0/semantic_release/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,21 @@
     EmojiCommitParser,
     ParseResult,
     ParserOptions,
     ScipyCommitParser,
     TagCommitParser,
 )
 from semantic_release.const import COMMIT_MESSAGE, DEFAULT_COMMIT_AUTHOR, SEMVER_REGEX
-from semantic_release.errors import InvalidConfiguration, NotAReleaseBranch
+from semantic_release.errors import (
+    InvalidConfiguration,
+    NotAReleaseBranch,
+    ParserLoadError,
+)
 from semantic_release.helpers import dynamic_import
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 from semantic_release.version import VersionTranslator
 from semantic_release.version.declaration import (
     PatternVersionDeclaration,
     TomlVersionDeclaration,
     VersionDeclarationABC,
 )
 
@@ -137,21 +142,30 @@
         )
         return ret_val or None
 
     @model_validator(mode="after")
     def set_default_token(self) -> Self:
         # Set the default token name for the given VCS when no user input is given
         if not self.token and self.type in _known_hvcs:
-            default_token_name = _known_hvcs[self.type].DEFAULT_ENV_TOKEN_NAME
-            if default_token_name:
-                env_token = EnvConfigVar(env=default_token_name).getvalue()
-                if env_token:
-                    self.token = env_token
+            if env_token := self._get_default_token():
+                self.token = env_token
         return self
 
+    def _get_default_token(self) -> str | None:
+        hvcs_client_class = _known_hvcs[self.type]
+        default_hvcs_instance = hvcs_client_class("git@example.com:owner/project.git")
+        if not isinstance(default_hvcs_instance, RemoteHvcsBase):
+            return None
+
+        default_token_name = default_hvcs_instance.DEFAULT_ENV_TOKEN_NAME
+        if not default_token_name:
+            return None
+
+        return EnvConfigVar(env=default_token_name).getvalue()
+
     @model_validator(mode="after")
     def check_url_scheme(self) -> Self:
         if self.url and isinstance(self.url, str):
             self.check_insecure_flag(self.url, "url")
 
         if self.domain and isinstance(self.domain, str):
             self.check_insecure_flag(self.domain, "domain")
@@ -218,26 +232,58 @@
     @model_validator(mode="after")
     def set_default_opts(self) -> Self:
         # Set the default parser options for the given commit parser when no user input is given
         if not self.commit_parser_options and self.commit_parser:
             parser_opts_type = None
             # If the commit parser is a known one, pull the default options object from it
             if self.commit_parser in _known_commit_parsers:
+                # TODO: BREAKING CHANGE v10
+                # parser_opts_type = (
+                #     _known_commit_parsers[self.commit_parser]
+                #     .get_default_options()
+                #     .__class__
+                # )
                 parser_opts_type = _known_commit_parsers[
                     self.commit_parser
                 ].parser_options
             else:
-                # if its a custom parser, try to import it and pull the default options object type
-                custom_class = dynamic_import(self.commit_parser)
-                if hasattr(custom_class, "parser_options"):
-                    parser_opts_type = custom_class.parser_options
+                try:
+                    # if its a custom parser, try to import it and pull the default options object type
+                    custom_class = dynamic_import(self.commit_parser)
+                    # TODO: BREAKING CHANGE v10
+                    # parser_opts_type = custom_class.get_default_options().__class__
+                    if hasattr(custom_class, "parser_options"):
+                        parser_opts_type = custom_class.parser_options
+
+                except ModuleNotFoundError as err:
+                    raise ParserLoadError(
+                        str.join(
+                            "\n",
+                            [
+                                str(err),
+                                "Unable to import your custom parser! Check your configuration!",
+                            ],
+                        )
+                    ) from err
+
+                except AttributeError as err:
+                    raise ParserLoadError(
+                        str.join(
+                            "\n",
+                            [
+                                str(err),
+                                "Unable to find your custom parser class inside the given module.",
+                                "Check your configuration!",
+                            ],
+                        )
+                    ) from err
 
             # from either the custom opts class or the known parser opts class, create an instance
             if callable(parser_opts_type):
-                opts_obj = parser_opts_type()
+                opts_obj: Any = parser_opts_type()
                 # if the opts object is a dataclass, wrap it in a RootModel so it can be transformed to a Mapping
                 opts_obj = (
                     opts_obj if not is_dataclass(opts_obj) else RootModel(opts_obj)
                 )
                 # Must be a mapping, so if it's a BaseModel, dump the model to a dict
                 self.commit_parser_options = (
                     opts_obj.model_dump()
@@ -369,23 +415,52 @@
                 "no release will be made"
             ) from err
 
         # branch-specific configuration
         branch_config = cls.select_branch_options(raw.branches, active_branch)
 
         # commit_parser
-        commit_parser_cls = (
-            _known_commit_parsers[raw.commit_parser]
-            if raw.commit_parser in _known_commit_parsers
-            else dynamic_import(raw.commit_parser)
-        )
+        try:
+            commit_parser_cls = (
+                _known_commit_parsers[raw.commit_parser]
+                if raw.commit_parser in _known_commit_parsers
+                else dynamic_import(raw.commit_parser)
+            )
+        except ModuleNotFoundError as err:
+            raise ParserLoadError(
+                str.join(
+                    "\n",
+                    [
+                        str(err),
+                        "Unable to import your custom parser! Check your configuration!",
+                    ],
+                )
+            ) from err
+        except AttributeError as err:
+            raise ParserLoadError(
+                str.join(
+                    "\n",
+                    [
+                        str(err),
+                        "Unable to find the parser class inside the given module",
+                    ],
+                )
+            ) from err
 
-        commit_parser = commit_parser_cls(
-            options=commit_parser_cls.parser_options(**raw.commit_parser_options)
-        )
+        commit_parser_opts_class = commit_parser_cls.parser_options
+        # TODO: Breaking change v10
+        # commit_parser_opts_class = commit_parser_cls.get_default_options().__class__
+        try:
+            commit_parser = commit_parser_cls(
+                options=commit_parser_opts_class(**raw.commit_parser_options)
+            )
+        except TypeError as err:
+            raise ParserLoadError(
+                str.join("\n", [str(err), f"Failed to initialize {raw.commit_parser}"])
+            ) from err
 
         # We always exclude PSR's own release commits from the Changelog
         # when parsing commits
         _psr_release_commit_re = re.compile(
             raw.commit_message.replace(r"{version}", r"(?P<version>.*)")
         )
         changelog_excluded_commit_patterns = (
```

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.6.0/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.6.0/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/cli/util.py` & `python_semantic_release-9.6.0/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,23 @@
                 major_types: Tuple[str] = ("breaking",)
                 minor_types: Tuple[str] = ("fix", "patch")
                 ...
             def __init__(self, options: parser_options) -> None:
                 ...
     """
 
-    parser_options: type[_OPTS]
+    # TODO: Deprecate in lieu of get_default_options()
+    parser_options: type[ParserOptions] = ParserOptions
 
-    def __init__(self, options: _OPTS) -> None:
-        self.options = options
+    def __init__(self, options: _OPTS | None = None) -> None:
+        self.options: _OPTS = (
+            options if options is not None else self.get_default_options()
+        )
+
+    # TODO: BREAKING CHANGE v10, add abstract method for all custom parsers
+    # @staticmethod
+    # @abstractmethod
+    def get_default_options(self) -> _OPTS:
+        return self.parser_options()  # type: ignore
 
     @abstractmethod
     def parse(self, commit: Commit) -> _TT: ...
```

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/angular.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,29 +58,34 @@
 
 class AngularCommitParser(CommitParser[ParseResult, AngularParserOptions]):
     """
     A commit parser for projects conforming to the angular style of conventional
     commits. See https://www.conventionalcommits.org/en/v1.0.0-beta.4/
     """
 
+    # TODO: Deprecate in lieu of get_default_options()
     parser_options = AngularParserOptions
 
-    def __init__(self, options: AngularParserOptions) -> None:
+    def __init__(self, options: AngularParserOptions | None = None) -> None:
         super().__init__(options)
         self.re_parser = re.compile(
             rf"""
-            (?P<type>{"|".join(options.allowed_tags)})  # e.g. feat
+            (?P<type>{"|".join(self.options.allowed_tags)})  # e.g. feat
             (?:\((?P<scope>[^\n]+)\))?  # or feat(parser)
             (?P<break>!)?:\s+  # breaking if feat!:
             (?P<subject>[^\n]+)  # commit subject
             (:?\n\n(?P<text>.+))?  # commit body
             """,
             flags=re.VERBOSE | re.DOTALL,
         )
 
+    @staticmethod
+    def get_default_options() -> AngularParserOptions:
+        return AngularParserOptions()
+
     # Maybe this can be cached as an optimisation, similar to how
     # mypy/pytest use their own caching directories, for very large commit
     # histories?
     # The problem is the cache likely won't be present in CI environments
     def parse(self, commit: Commit) -> ParseResult:
         """
         Attempt to parse the commit message with a regular expression into a
```

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/emoji.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,21 @@
     If the message does not contain any known emojis, then the level to bump
     will be 0 and the type of change "Other". This parser never raises
     UnknownCommitMessageStyleError.
     Emojis are not removed from the description, and will appear alongside
     the commit subject in the changelog.
     """
 
+    # TODO: Deprecate in lieu of get_default_options()
     parser_options = EmojiParserOptions
 
+    @staticmethod
+    def get_default_options() -> EmojiParserOptions:
+        return EmojiParserOptions()
+
     def parse(self, commit: Commit) -> ParseResult:
         all_emojis = (
             self.options.major_tags + self.options.minor_tags + self.options.patch_tags
         )
 
         message = str(commit.message)
         subject = message.split("\n")[0]
```

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/scipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,34 +78,28 @@
 }
 
 _COMMIT_FILTER = "|".join(tag_to_section)
 
 
 @dataclass
 class ScipyParserOptions(ParserOptions):
+    major_tags: Tuple[str, ...] = ("API",)
+    minor_tags: Tuple[str, ...] = ("DEP", "DEV", "ENH", "REV", "FEAT")
+    patch_tags: Tuple[str, ...] = ("BLD", "BUG", "MAINT")
     allowed_tags: Tuple[str, ...] = (
-        "API",
-        "DEP",
-        "ENH",
-        "REV",
-        "BUG",
-        "MAINT",
+        *major_tags,
+        *minor_tags,
+        *patch_tags,
         "BENCH",
-        "BLD",
-        "DEV",
         "DOC",
         "STY",
         "TST",
         "REL",
-        "FEAT",
         "TEST",
     )
-    major_tags: Tuple[str, ...] = ("API",)
-    minor_tags: Tuple[str, ...] = ("DEP", "DEV", "ENH", "REV", "FEAT")
-    patch_tags: Tuple[str, ...] = ("BLD", "BUG", "MAINT")
     default_level_bump: LevelBump = LevelBump.NO_RELEASE
 
     def __post_init__(self) -> None:
         self.tag_to_level = {tag: LevelBump.NO_RELEASE for tag in self.allowed_tags}
         for tag in self.patch_tags:
             self.tag_to_level[tag] = LevelBump.PATCH
         for tag in self.minor_tags:
@@ -113,27 +107,32 @@
         for tag in self.major_tags:
             self.tag_to_level[tag] = LevelBump.MAJOR
 
 
 class ScipyCommitParser(CommitParser[ParseResult, ScipyParserOptions]):
     """Parser for scipy-style commit messages"""
 
+    # TODO: Deprecate in lieu of get_default_options()
     parser_options = ScipyParserOptions
 
-    def __init__(self, options: ScipyParserOptions) -> None:
+    def __init__(self, options: ScipyParserOptions | None = None) -> None:
         super().__init__(options)
         self.re_parser = re.compile(
             rf"(?P<tag>{_COMMIT_FILTER})?"
             r"(?:\((?P<scope>[^\n]+)\))?"
             r":? "
             r"(?P<subject>[^\n]+):?"
             r"(\n\n(?P<text>.*))?",
             re.DOTALL,
         )
 
+    @staticmethod
+    def get_default_options() -> ScipyParserOptions:
+        return ScipyParserOptions()
+
     def parse(self, commit: Commit) -> ParseResult:
         message = str(commit.message)
         parsed = self.re_parser.match(message)
 
         if not parsed:
             return _logged_parse_error(
                 commit, f"Unable to parse the given commit message: {message}"
```

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,21 @@
 class TagCommitParser(CommitParser[ParseResult, TagParserOptions]):
     """
     Parse a commit message according to the 1.0 version of python-semantic-release.
     It expects a tag of some sort in the commit message and will use the rest of the
     first line as changelog content.
     """
 
+    # TODO: Deprecate in lieu of get_default_options()
     parser_options = TagParserOptions
 
+    @staticmethod
+    def get_default_options() -> TagParserOptions:
+        return TagParserOptions()
+
     def parse(self, commit: Commit) -> ParseResult:
         message = str(commit.message)
 
         # Attempt to parse the commit message with a regular expression
         parsed = re_parser.match(message)
         if not parsed:
             return _logged_parse_error(
```

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/token.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/commit_parser/util.py` & `python_semantic_release-9.6.0/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/const.py` & `python_semantic_release-9.6.0/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.6.0/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/enums.py` & `python_semantic_release-9.6.0/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/helpers.py` & `python_semantic_release-9.6.0/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/bitbucket.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/bitbucket.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import os
 from functools import lru_cache
 from pathlib import PurePosixPath
 from typing import TYPE_CHECKING
 
 from urllib3.util.url import Url, parse_url
 
-from semantic_release.hvcs._base import HvcsBase
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 
 if TYPE_CHECKING:
-    from typing import Any
+    from typing import Any, Callable
 
 
 # Globals
 log = logging.getLogger(__name__)
 
 
-class Bitbucket(HvcsBase):
+class Bitbucket(RemoteHvcsBase):
     """
     Bitbucket HVCS interface for interacting with BitBucket repositories
 
     This class supports the following products:
 
         - BitBucket Cloud
         - BitBucket Data Center Server (on-premises installations)
@@ -42,17 +42,17 @@
     the BitBucket Data Center Server product. The on-prem server product uses a
     path prefix for handling api requests which is configured to be
     `server.domain/rest/api/1.0` based on the documentation in April 2024.
     """
 
     DEFAULT_DOMAIN = "bitbucket.org"
     DEFAULT_API_SUBDOMAIN_PREFIX = "api"
-    DEFAULT_API_DOMAIN = f"{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}"
     DEFAULT_API_PATH_CLOUD = "/2.0"
     DEFAULT_API_PATH_ONPREM = "/rest/api/1.0"
+    DEFAULT_API_URL_CLOUD = f"https://{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}{DEFAULT_API_PATH_CLOUD}"
     DEFAULT_ENV_TOKEN_NAME = "BITBUCKET_TOKEN"  # noqa: S105
 
     def __init__(
         self,
         remote_url: str,
         *,
         hvcs_domain: str | None = None,
@@ -64,156 +64,111 @@
         super().__init__(remote_url)
         self.token = token
         # NOTE: Uncomment in the future when we actually have functionalty to
         #       use the api, but currently there is none.
         # auth = None if not self.token else TokenAuth(self.token)
         # self.session = build_requests_session(auth=auth)
 
-        domain_url = parse_url(hvcs_domain or f"https://{self.DEFAULT_DOMAIN}")
-
-        if domain_url.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not domain_url.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
-
-        if domain_url.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
-                "Only http and https are supported."
-            )
+        domain_url = self._normalize_url(
+            hvcs_domain or f"https://{self.DEFAULT_DOMAIN}",
+            allow_insecure=allow_insecure,
+        )
 
         # Strip any auth, query or fragment from the domain
-        self.hvcs_domain = parse_url(
+        self._hvcs_domain = parse_url(
             Url(
                 scheme=domain_url.scheme,
                 host=domain_url.host,
                 port=domain_url.port,
                 path=str(PurePosixPath(domain_url.path or "/")),
             ).url.rstrip("/")
         )
 
         # Parse api domain if provided otherwise infer from domain
-        api_domain_parts = parse_url(
-            hvcs_api_domain
-            or Url(
-                # infer from Domain url and append the api path
-                **{
-                    **self.hvcs_domain._asdict(),
-                    "host": self.hvcs_domain.host,
-                    "path": str(
-                        PurePosixPath(
-                            str.lstrip(self.hvcs_domain.path or "", "/") or "/",
-                            self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
-                        )
-                    ),
-                }
-            ).url.rstrip("/")
+        api_domain_parts = self._normalize_url(
+            hvcs_api_domain or self._derive_api_url_from_base_domain(),
+            allow_insecure=allow_insecure,
         )
 
-        if api_domain_parts.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not api_domain_parts.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            api_domain_parts = Url(
-                **{**api_domain_parts._asdict(), "scheme": new_scheme}
-            )
-
-        if api_domain_parts.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {api_domain_parts.scheme} for api domain {api_domain_parts.host}. "
-                "Only http and https are supported."
-            )
-
         # As Bitbucket Cloud and Bitbucket Server (on-prem) have different api paths
         # lets check what we have been given and set the api url accordingly
         #   ref: https://developer.atlassian.com/server/bitbucket/how-tos/command-line-rest/
         #   NOTE: BitBucket Server (on premise) uses a path prefix '/rest/api/1.0' for the api
         #         while BitBucket Cloud uses a separate subdomain with '/2.0' path prefix
         is_bitbucket_cloud = bool(
             self.hvcs_domain.url == f"https://{self.DEFAULT_DOMAIN}"
         )
 
-        # Calculate out the api url that we expect for Bitbucket Cloud
-        default_cloud_api_url = parse_url(
-            Url(
-                # set api domain and append the default api path
-                **{
-                    **self.hvcs_domain._asdict(),
-                    "host": f"{self.DEFAULT_API_DOMAIN}",
-                    "path": self.DEFAULT_API_PATH_CLOUD,
-                }
-            ).url
-        )
-
         if (
             is_bitbucket_cloud
             and hvcs_api_domain
-            and api_domain_parts.url not in default_cloud_api_url.url
+            and api_domain_parts.url not in Bitbucket.DEFAULT_API_URL_CLOUD
         ):
             # Api was provied but is not a subset of the expected one, raise an error
             # we check for a subset because the user may not have provided the full api path
             # but the correct domain.  If they didn't, then we are erroring out here.
             raise ValueError(
                 f"Invalid api domain {api_domain_parts.url} for BitBucket Cloud. "
-                f"Expected {default_cloud_api_url.url}."
+                f"Expected {Bitbucket.DEFAULT_API_URL_CLOUD}."
             )
 
         # Set the api url to the default cloud one if we are on cloud, otherwise
         # use the verified api domain for a on-prem server
-        self.api_url = (
-            default_cloud_api_url
+        self._api_url = parse_url(
+            Bitbucket.DEFAULT_API_URL_CLOUD
             if is_bitbucket_cloud
-            else parse_url(
+            else Url(
                 # Strip any auth, query or fragment from the domain
-                Url(
-                    scheme=api_domain_parts.scheme,
-                    host=api_domain_parts.host,
-                    port=api_domain_parts.port,
-                    path=str(
+                scheme=api_domain_parts.scheme,
+                host=api_domain_parts.host,
+                port=api_domain_parts.port,
+                path=str(
+                    PurePosixPath(
+                        # pass any custom server prefix path but ensure we don't
+                        # double up the api path in the case the user provided it
+                        str.replace(
+                            api_domain_parts.path or "",
+                            self.DEFAULT_API_PATH_ONPREM,
+                            "",
+                        ).lstrip("/")
+                        or "/",
+                        # apply the on-prem api path
+                        self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
+                    )
+                ),
+            ).url.rstrip("/")
+        )
+
+    def _derive_api_url_from_base_domain(self) -> Url:
+        return parse_url(
+            Url(
+                # infer from Domain url and append the api path
+                **{
+                    **self.hvcs_domain._asdict(),
+                    "host": self.hvcs_domain.host,
+                    "path": str(
                         PurePosixPath(
-                            # pass any custom server prefix path but ensure we don't
-                            # double up the api path in the case the user provided it
-                            str.replace(
-                                api_domain_parts.path or "",
-                                self.DEFAULT_API_PATH_ONPREM,
-                                "",
-                            ).lstrip("/")
-                            or "/",
-                            # apply the on-prem api path
+                            str.lstrip(self.hvcs_domain.path or "", "/") or "/",
                             self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
                         )
                     ),
-                ).url.rstrip("/")
-            )
+                }
+            ).url.rstrip("/")
         )
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         # ref: https://support.atlassian.com/bitbucket-cloud/docs/variables-and-secrets/
         if "BITBUCKET_REPO_FULL_NAME" in os.environ:
             log.info("Getting repository owner and name from environment variables.")
             owner, name = os.environ["BITBUCKET_REPO_FULL_NAME"].rsplit("/", 1)
             return owner, name
 
         return super()._get_repository_owner_and_name()
 
-    def compare_url(self, from_rev: str, to_rev: str) -> str:
-        """
-        Get the Bitbucket comparison link between two version tags.
-        :param from_rev: The older version to compare.
-        :param to_rev: The newer version to compare.
-        :return: Link to view a comparison between the two versions.
-        """
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/branches/compare/{from_rev}%0D{to_rev}"
-        )
-
     def remote_url(self, use_token: bool = True) -> str:
         """Get the remote url including the token for authentication if requested"""
         if not use_token:
             return self._remote_url
 
         if not self.token:
             raise ValueError("Requested to use token but no token set.")
@@ -227,60 +182,52 @@
         user = os.environ.get("BITBUCKET_USER", "x-token-auth")
 
         return self.create_server_url(
             auth=f"{user}:{self.token}" if user else self.token,
             path=f"/{self.owner}/{self.repo_name}.git",
         )
 
-    def commit_hash_url(self, commit_hash: str) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/commits/{commit_hash}"
+    def compare_url(self, from_rev: str, to_rev: str) -> str:
+        """
+        Get the Bitbucket comparison link between two version tags.
+        :param from_rev: The older version to compare.
+        :param to_rev: The newer version to compare.
+        :return: Link to view a comparison between the two versions.
+        """
+        return self.create_repo_url(
+            repo_path=f"/branches/compare/{from_rev}%0D{to_rev}"
         )
 
+    def commit_hash_url(self, commit_hash: str) -> str:
+        return self.create_repo_url(repo_path=f"/commits/{commit_hash}")
+
     def pull_request_url(self, pr_number: str | int) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/pull-requests/{pr_number}"
-        )
+        return self.create_repo_url(repo_path=f"/pull-requests/{pr_number}")
 
-    def _derive_url(
-        self,
-        base_url: Url,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        overrides = dict(
-            filter(
-                lambda x: x[1] is not None,
-                {
-                    "auth": auth,
-                    "path": str(PurePosixPath("/", path)),
-                    "query": query,
-                    "fragment": fragment,
-                }.items(),
-            )
-        )
-        return Url(
-            **{
-                **base_url._asdict(),
-                **overrides,
-            }
-        ).url.rstrip("/")
+    def get_changelog_context_filters(self) -> tuple[Callable[..., Any], ...]:
+        return (
+            self.create_server_url,
+            self.create_repo_url,
+            self.commit_hash_url,
+            self.compare_url,
+            self.pull_request_url,
+        )
+
+    def upload_dists(self, tag: str, dist_glob: str) -> int:
+        return super().upload_dists(tag, dist_glob)
+
+    def create_or_update_release(
+        self, tag: str, release_notes: str, prerelease: bool = False
+    ) -> int | str:
+        return super().create_or_update_release(tag, release_notes, prerelease)
 
-    def create_server_url(
+    def create_release(
         self,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        return self._derive_url(self.hvcs_domain, path, auth, query, fragment)
+        tag: str,
+        release_notes: str,
+        prerelease: bool = False,
+        assets: list[str] | None = None,
+    ) -> int | str:
+        return super().create_release(tag, release_notes, prerelease, assets)
 
-    def create_api_url(
-        self,
-        endpoint: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        return self._derive_url(self.api_url, endpoint, auth, query, fragment)
+
+RemoteHvcsBase.register(Bitbucket)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/gitea.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 import os
 from pathlib import PurePosixPath
 from typing import TYPE_CHECKING
 
 from requests import HTTPError, JSONDecodeError
 from urllib3.util.url import Url, parse_url
 
-from semantic_release.errors import UnexpectedResponse
+from semantic_release.errors import (
+    AssetUploadError,
+    IncompleteReleaseError,
+    UnexpectedResponse,
+)
 from semantic_release.helpers import logged_function
-from semantic_release.hvcs._base import HvcsBase
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session, suppress_not_found
 
 if TYPE_CHECKING:
-    from typing import Any
+    from typing import Any, Callable
 
 
 # Globals
 log = logging.getLogger(__name__)
 
 
-class Gitea(HvcsBase):
+class Gitea(RemoteHvcsBase):
     """Gitea helper class"""
 
     DEFAULT_DOMAIN = "gitea.com"
     DEFAULT_API_PATH = "/api/v1"
     DEFAULT_ENV_TOKEN_NAME = "GITEA_TOKEN"  # noqa: S105
 
     def __init__(
@@ -42,57 +46,50 @@
         **kwargs: Any,
     ) -> None:
         super().__init__(remote_url)
         self.token = token
         auth = None if not self.token else TokenAuth(self.token)
         self.session = build_requests_session(auth=auth)
 
-        domain_url = parse_url(
+        domain_url = self._normalize_url(
             hvcs_domain
             or os.getenv("GITEA_SERVER_URL", "")
-            or f"https://{self.DEFAULT_DOMAIN}"
+            or f"https://{self.DEFAULT_DOMAIN}",
+            allow_insecure=allow_insecure,
         )
 
-        if domain_url.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not domain_url.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
-
-        if domain_url.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
-                "Only http and https are supported."
-            )
-
         # Strip any auth, query or fragment from the domain
-        self.hvcs_domain = parse_url(
+        self._hvcs_domain = parse_url(
             Url(
                 scheme=domain_url.scheme,
                 host=domain_url.host,
                 port=domain_url.port,
                 path=str(PurePosixPath(domain_url.path or "/")),
             ).url.rstrip("/")
         )
 
-        self.api_url = parse_url(
+        self._api_url = self._normalize_url(
             os.getenv("GITEA_API_URL", "").rstrip("/")
             or Url(
                 # infer from Domain url and append the default api path
                 **{
                     **self.hvcs_domain._asdict(),
                     "path": f"{self.hvcs_domain.path or ''}{self.DEFAULT_API_PATH}",
                 }
-            ).url
+            ).url,
+            allow_insecure=allow_insecure,
         )
 
     @logged_function(log)
     def create_release(
-        self, tag: str, release_notes: str, prerelease: bool = False
+        self,
+        tag: str,
+        release_notes: str,
+        prerelease: bool = False,
+        assets: list[str] | None = None,
     ) -> int:
         """
         Create a new release
 
         Ref: https://gitea.com/api/swagger#/repository/repoCreateRelease
 
         :param tag: Tag to create release for
@@ -119,21 +116,43 @@
             },
         )
 
         # Raise an error if the request was not successful
         response.raise_for_status()
 
         try:
-            data = response.json()
-            return data["id"]
+            release_id: int = response.json()["id"]
+            log.info("Successfully created release with ID: %s", release_id)
         except JSONDecodeError as err:
             raise UnexpectedResponse("Unreadable json response") from err
         except KeyError as err:
             raise UnexpectedResponse("JSON response is missing an id") from err
 
+        errors = []
+        for asset in assets or []:
+            log.info("Uploading asset %s", asset)
+            try:
+                self.upload_release_asset(release_id, asset)
+            except HTTPError as err:
+                errors.append(
+                    AssetUploadError(f"Failed asset upload for {asset}").with_traceback(
+                        err.__traceback__
+                    )
+                )
+
+        if len(errors) < 1:
+            return release_id
+
+        for error in errors:
+            log.exception(error)
+
+        raise IncompleteReleaseError(
+            f"Failed to upload asset{'s' if len(errors) > 1 else ''} to release!"
+        )
+
     @logged_function(log)
     @suppress_not_found
     def get_release_id_by_tag(self, tag: str) -> int | None:
         """
         Get a release by its tag name
         https://gitea.com/api/swagger#/repository/repoGetReleaseByTag
         :param tag: Tag to get release for
@@ -214,15 +233,15 @@
         :param release_id: ID of the release to upload to
         """
         return self.create_api_url(
             endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/{release_id}/assets",
         )
 
     @logged_function(log)
-    def upload_asset(
+    def upload_release_asset(
         self,
         release_id: int,
         file: str,
         label: str | None = None,  # noqa: ARG002
     ) -> bool:
         """
         Upload an asset to an existing release
@@ -278,15 +297,15 @@
 
         # Upload assets
         n_succeeded = 0
         for file_path in (
             f for f in glob.glob(dist_glob, recursive=True) if os.path.isfile(f)
         ):
             try:
-                self.upload_asset(release_id, file_path)
+                self.upload_release_asset(release_id, file_path)
                 n_succeeded += 1
             except HTTPError:  # noqa: PERF203
                 log.exception("error uploading asset %s", file_path)
 
         return n_succeeded
 
     def remote_url(self, use_token: bool = True) -> str:
@@ -296,55 +315,26 @@
 
         return self.create_server_url(
             auth=self.token,
             path=f"{self.owner}/{self.repo_name}.git",
         )
 
     def commit_hash_url(self, commit_hash: str) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/commit/{commit_hash}"
-        )
+        return self.create_repo_url(repo_path=f"/commit/{commit_hash}")
+
+    def issue_url(self, issue_num: str | int) -> str:
+        return self.create_repo_url(repo_path=f"/issues/{issue_num}")
 
     def pull_request_url(self, pr_number: str | int) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/pulls/{pr_number}"
-        )
+        return self.create_repo_url(repo_path=f"/pulls/{pr_number}")
 
-    def create_server_url(
-        self,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        overrides = dict(
-            filter(
-                lambda x: x[1] is not None,
-                {
-                    "auth": auth,
-                    "path": str(PurePosixPath(path or "/")),
-                    "query": query,
-                    "fragment": fragment,
-                }.items(),
-            )
+    def get_changelog_context_filters(self) -> tuple[Callable[..., Any], ...]:
+        return (
+            self.create_server_url,
+            self.create_repo_url,
+            self.commit_hash_url,
+            self.issue_url,
+            self.pull_request_url,
         )
-        return Url(
-            **{
-                **self.hvcs_domain._asdict(),
-                **overrides,
-            }
-        ).url.rstrip("/")
 
-    def create_api_url(
-        self,
-        endpoint: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        api_path = self.api_url.url.replace(self.hvcs_domain.url, "")
-        return self.create_server_url(
-            path=f"{api_path}/{endpoint.lstrip(api_path)}",
-            auth=auth,
-            query=query,
-            fragment=fragment,
-        )
+
+RemoteHvcsBase.register(Gitea)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/github.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/github.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from functools import lru_cache
 from pathlib import PurePosixPath
 from typing import TYPE_CHECKING
 
 from requests import HTTPError, JSONDecodeError
 from urllib3.util.url import Url, parse_url
 
-from semantic_release.errors import UnexpectedResponse
+from semantic_release.errors import (
+    AssetUploadError,
+    IncompleteReleaseError,
+    UnexpectedResponse,
+)
 from semantic_release.helpers import logged_function
-from semantic_release.hvcs._base import HvcsBase
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session, suppress_not_found
 
 if TYPE_CHECKING:
-    from typing import Any
+    from typing import Any, Callable
 
 
 # Globals
 log = logging.getLogger(__name__)
 
 
 # Add a mime type for wheels
@@ -41,15 +45,15 @@
 if mimetypes.guess_type("test.whl")[0] != "application/octet-stream":
     mimetypes.add_type("application/octet-stream", ".whl")
 
 if mimetypes.guess_type("test.md")[0] != "text/markdown":
     mimetypes.add_type("text/markdown", ".md")
 
 
-class Github(HvcsBase):
+class Github(RemoteHvcsBase):
     """
     GitHub HVCS interface for interacting with GitHub repositories
 
     This class supports the following products:
 
         - GitHub Free, Pro, & Team
         - GitHub Enterprise Cloud
@@ -68,14 +72,17 @@
     """
 
     DEFAULT_DOMAIN = "github.com"
     DEFAULT_API_SUBDOMAIN_PREFIX = "api"
     DEFAULT_API_DOMAIN = f"{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}"
     DEFAULT_API_PATH_CLOUD = "/"  # no path prefix!
     DEFAULT_API_PATH_ONPREM = "/api/v3"
+    DEFAULT_API_URL_CLOUD = f"https://{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}{DEFAULT_API_PATH_CLOUD}".rstrip(
+        "/"
+    )
     DEFAULT_ENV_TOKEN_NAME = "GH_TOKEN"  # noqa: S105
 
     def __init__(
         self,
         remote_url: str,
         *,
         hvcs_domain: str | None = None,
@@ -86,168 +93,141 @@
     ) -> None:
         super().__init__(remote_url)
         self.token = token
         auth = None if not self.token else TokenAuth(self.token)
         self.session = build_requests_session(auth=auth)
 
         # ref: https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
-        domain_url = parse_url(
+        domain_url_str = (
             hvcs_domain
             or os.getenv("GITHUB_SERVER_URL", "")
             or f"https://{self.DEFAULT_DOMAIN}"
         )
 
-        if domain_url.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not domain_url.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
-
-        if domain_url.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
-                "Only http and https are supported."
-            )
+        domain_url = self._normalize_url(
+            domain_url_str,
+            allow_insecure=allow_insecure,
+        )
 
         # Strip any auth, query or fragment from the domain
-        self.hvcs_domain = parse_url(
+        self._hvcs_domain = parse_url(
             Url(
                 scheme=domain_url.scheme,
                 host=domain_url.host,
                 port=domain_url.port,
                 path=str(PurePosixPath(domain_url.path or "/")),
             ).url.rstrip("/")
         )
 
         # ref: https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
-        api_domain_parts = parse_url(
+        api_url_str = (
             hvcs_api_domain
             or os.getenv("GITHUB_API_URL", "")
-            or Url(
-                # infer from Domain url and prepend the default api subdomain
-                **{
-                    **self.hvcs_domain._asdict(),
-                    "host": self.hvcs_domain.host,
-                    "path": str(
-                        PurePosixPath(
-                            str.lstrip(self.hvcs_domain.path or "", "/") or "/",
-                            self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
-                        )
-                    ),
-                }
-            ).url.rstrip("/")
+            or self._derive_api_url_from_base_domain()
         )
 
-        if api_domain_parts.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not api_domain_parts.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            api_domain_parts = Url(
-                **{**api_domain_parts._asdict(), "scheme": new_scheme}
-            )
-
-        if api_domain_parts.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {api_domain_parts.scheme} for api domain {api_domain_parts.host}. "
-                "Only http and https are supported."
-            )
+        api_domain_parts = self._normalize_url(
+            api_url_str,
+            allow_insecure=allow_insecure,
+        )
 
         # As GitHub Enterprise Cloud and GitHub Enterprise Server (on-prem) have different api locations
         # lets check what we have been given and set the api url accordingly
         #   NOTE: Github Server (on premise) uses a path prefix '/api/v3' for the api
         #         while GitHub Enterprise Cloud uses a separate subdomain as the base
         is_github_cloud = bool(self.hvcs_domain.url == f"https://{self.DEFAULT_DOMAIN}")
 
-        # Calculate out the api url that we expect for GitHub Cloud
-        default_cloud_api_url = parse_url(
-            Url(
-                # set api domain and append the default api path
-                **{
-                    **self.hvcs_domain._asdict(),
-                    "host": f"{self.DEFAULT_API_DOMAIN}",
-                    "path": self.DEFAULT_API_PATH_CLOUD,
-                }
-            ).url.rstrip("/")
-        )
-
         if (
             is_github_cloud
             and hvcs_api_domain
-            and api_domain_parts.url not in default_cloud_api_url.url
+            and api_domain_parts.url not in Github.DEFAULT_API_URL_CLOUD
         ):
             # Api was provied but is not a subset of the expected one, raise an error
             # we check for a subset because the user may not have provided the full api path
             # but the correct domain.  If they didn't, then we are erroring out here.
             raise ValueError(
                 f"Invalid api domain {api_domain_parts.url} for GitHub Enterprise Cloud. "
-                f"Expected {default_cloud_api_url.url}."
+                f"Expected {Github.DEFAULT_API_URL_CLOUD}."
             )
 
         # Set the api url to the default cloud one if we are on cloud, otherwise
         # use the verified api domain for a on-prem server
-        self.api_url = (
-            default_cloud_api_url
+        self._api_url = parse_url(
+            Github.DEFAULT_API_URL_CLOUD
             if is_github_cloud
-            else parse_url(
+            else Url(
                 # Strip any auth, query or fragment from the domain
-                Url(
-                    scheme=api_domain_parts.scheme,
-                    host=api_domain_parts.host,
-                    port=api_domain_parts.port,
-                    path=str(
+                scheme=api_domain_parts.scheme,
+                host=api_domain_parts.host,
+                port=api_domain_parts.port,
+                path=str(
+                    PurePosixPath(
+                        # pass any custom server prefix path but ensure we don't
+                        # double up the api path in the case the user provided it
+                        str.replace(
+                            api_domain_parts.path or "",
+                            self.DEFAULT_API_PATH_ONPREM,
+                            "",
+                        ).lstrip("/")
+                        or "/",
+                        # apply the on-prem api path
+                        self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
+                    )
+                ),
+            ).url.rstrip("/")
+        )
+
+    def _derive_api_url_from_base_domain(self) -> Url:
+        return parse_url(
+            Url(
+                # infer from Domain url and prepend the default api subdomain
+                **{
+                    **self.hvcs_domain._asdict(),
+                    "host": self.hvcs_domain.host,
+                    "path": str(
                         PurePosixPath(
-                            # pass any custom server prefix path but ensure we don't
-                            # double up the api path in the case the user provided it
-                            str.replace(
-                                api_domain_parts.path or "",
-                                self.DEFAULT_API_PATH_ONPREM,
-                                "",
-                            ).lstrip("/")
-                            or "/",
-                            # apply the on-prem api path
+                            str.lstrip(self.hvcs_domain.path or "", "/") or "/",
                             self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
                         )
                     ),
-                ).url.rstrip("/")
-            )
+                }
+            ).url.rstrip("/")
         )
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         # Github actions context
         if "GITHUB_REPOSITORY" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             owner, name = os.environ["GITHUB_REPOSITORY"].rsplit("/", 1)
             return owner, name
 
         return super()._get_repository_owner_and_name()
 
-    def compare_url(self, from_rev: str, to_rev: str) -> str:
-        """
-        Get the GitHub comparison link between two version tags.
-        :param from_rev: The older version to compare.
-        :param to_rev: The newer version to compare.
-        :return: Link to view a comparison between the two versions.
-        """
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/compare/{from_rev}...{to_rev}"
-        )
-
     @logged_function(log)
     def create_release(
-        self, tag: str, release_notes: str, prerelease: bool = False
+        self,
+        tag: str,
+        release_notes: str,
+        prerelease: bool = False,
+        assets: list[str] | None = None,
     ) -> int:
         """
         Create a new release
-        https://docs.github.com/rest/reference/repos#create-a-release
+
+        REF: https://docs.github.com/rest/reference/repos#create-a-release
+
         :param tag: Tag to create release for
+
         :param release_notes: The release notes for this version
+
         :param prerelease: Whether or not this release should be created as a prerelease
+
+        :param assets: a list of artifacts to upload to the release
+
         :return: the ID of the release
         """
         log.info("Creating release for tag %s", tag)
         releases_endpoint = self.create_api_url(
             endpoint=f"/repos/{self.owner}/{self.repo_name}/releases",
         )
         response = self.session.post(
@@ -263,20 +243,41 @@
 
         # Raise an error if the request was not successful
         response.raise_for_status()
 
         try:
             release_id: int = response.json()["id"]
             log.info("Successfully created release with ID: %s", release_id)
-            return release_id
         except JSONDecodeError as err:
             raise UnexpectedResponse("Unreadable json response") from err
         except KeyError as err:
             raise UnexpectedResponse("JSON response is missing an id") from err
 
+        errors = []
+        for asset in assets or []:
+            log.info("Uploading asset %s", asset)
+            try:
+                self.upload_release_asset(release_id, asset)
+            except HTTPError as err:
+                errors.append(
+                    AssetUploadError(f"Failed asset upload for {asset}").with_traceback(
+                        err.__traceback__
+                    )
+                )
+
+        if len(errors) < 1:
+            return release_id
+
+        for error in errors:
+            log.exception(error)
+
+        raise IncompleteReleaseError(
+            f"Failed to upload asset{'s' if len(errors) > 1 else ''} to release!"
+        )
+
     @logged_function(log)
     @suppress_not_found
     def get_release_id_by_tag(self, tag: str) -> int | None:
         """
         Get a release by its tag name
         https://docs.github.com/rest/reference/repos#get-a-release-by-tag-name
         :param tag: Tag to get release for
@@ -373,15 +374,15 @@
             raise UnexpectedResponse("Unreadable json response") from err
         except KeyError as err:
             raise UnexpectedResponse(
                 "JSON response is missing a key 'upload_url'"
             ) from err
 
     @logged_function(log)
-    def upload_asset(
+    def upload_release_asset(
         self, release_id: int, file: str, label: str | None = None
     ) -> bool:
         """
         Upload an asset to an existing release
         https://docs.github.com/rest/reference/repos#upload-a-release-asset
         :param release_id: ID of the release to upload to
         :param file: Path of the file to upload
@@ -438,15 +439,15 @@
 
         # Upload assets
         n_succeeded = 0
         for file_path in (
             f for f in glob.glob(dist_glob, recursive=True) if os.path.isfile(f)
         ):
             try:
-                self.upload_asset(release_id, file_path)
+                self.upload_release_asset(release_id, file_path)
                 n_succeeded += 1
             except HTTPError:  # noqa: PERF203
                 log.exception("error uploading asset %s", file_path)
 
         return n_succeeded
 
     def remote_url(self, use_token: bool = True) -> str:
@@ -457,74 +458,37 @@
 
         actor = os.getenv("GITHUB_ACTOR", None)
         return self.create_server_url(
             auth=f"{actor}:{self.token}" if actor else self.token,
             path=f"/{self.owner}/{self.repo_name}.git",
         )
 
+    def compare_url(self, from_rev: str, to_rev: str) -> str:
+        """
+        Get the GitHub comparison link between two version tags.
+        :param from_rev: The older version to compare.
+        :param to_rev: The newer version to compare.
+        :return: Link to view a comparison between the two versions.
+        """
+        return self.create_repo_url(repo_path=f"/compare/{from_rev}...{to_rev}")
+
     def commit_hash_url(self, commit_hash: str) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/commit/{commit_hash}"
-        )
+        return self.create_repo_url(repo_path=f"/commit/{commit_hash}")
+
+    def issue_url(self, issue_num: str | int) -> str:
+        return self.create_repo_url(repo_path=f"/issues/{issue_num}")
 
     def pull_request_url(self, pr_number: str | int) -> str:
-        return self.create_server_url(
-            path=f"/{self.owner}/{self.repo_name}/issues/{pr_number}"
-        )
+        return self.create_repo_url(repo_path=f"/pull/{pr_number}")
 
-    def _derive_url(
-        self,
-        base_url: Url,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        overrides = dict(
-            filter(
-                lambda x: x[1] is not None,
-                {
-                    "auth": auth,
-                    "path": str(PurePosixPath("/", path.lstrip("/"))),
-                    "query": query,
-                    "fragment": fragment,
-                }.items(),
-            )
+    def get_changelog_context_filters(self) -> tuple[Callable[..., Any], ...]:
+        return (
+            self.create_server_url,
+            self.create_repo_url,
+            self.commit_hash_url,
+            self.compare_url,
+            self.issue_url,
+            self.pull_request_url,
         )
-        return Url(
-            **{
-                **base_url._asdict(),
-                **overrides,
-            }
-        ).url.rstrip("/")
 
-    def create_server_url(
-        self,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        # Ensure any path prefix is transfered but not doubled up on the derived url
-        return self._derive_url(
-            self.hvcs_domain,
-            path=f"{self.hvcs_domain.path or ''}/{path.lstrip(self.hvcs_domain.path)}",
-            auth=auth,
-            query=query,
-            fragment=fragment,
-        )
 
-    def create_api_url(
-        self,
-        endpoint: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        # Ensure any api path prefix is transfered but not doubled up on the derived api url
-        return self._derive_url(
-            self.api_url,
-            path=f"{self.api_url.path or ''}/{endpoint.lstrip(self.api_url.path)}",
-            auth=auth,
-            query=query,
-            fragment=fragment,
-        )
+RemoteHvcsBase.register(Github)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/gitlab.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 from pathlib import PurePosixPath
 from typing import TYPE_CHECKING
 
 import gitlab
 from urllib3.util.url import Url, parse_url
 
 from semantic_release.helpers import logged_function
-from semantic_release.hvcs._base import HvcsBase
+from semantic_release.hvcs.remote_hvcs_base import RemoteHvcsBase
 
 if TYPE_CHECKING:
-    from typing import Any
+    from typing import Any, Callable
+
+
+log = logging.getLogger(__name__)
 
 
 # Globals
 log = logging.getLogger(__name__)
 
 
-class Gitlab(HvcsBase):
-    """
-    Gitlab helper class
-    Note Gitlab doesn't really have the concept of a separate
-    API domain
-    """
+class Gitlab(RemoteHvcsBase):
+    """Gitlab HVCS interface for interacting with Gitlab repositories"""
 
     DEFAULT_ENV_TOKEN_NAME = "GITLAB_TOKEN"  # noqa: S105
     # purposefully not CI_JOB_TOKEN as it is not a personal access token,
     # It is missing the permission to push to the repository, but has all others (releases, packages, etc.)
 
     DEFAULT_DOMAIN = "gitlab.com"
 
@@ -41,47 +40,35 @@
         *,
         hvcs_domain: str | None = None,
         token: str | None = None,
         allow_insecure: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(remote_url)
-        self._remote_url = remote_url
         self.token = token
 
-        domain_url = parse_url(
+        domain_url = self._normalize_url(
             hvcs_domain
             or os.getenv("CI_SERVER_URL", "")
-            or f"https://{self.DEFAULT_DOMAIN}"
+            or f"https://{self.DEFAULT_DOMAIN}",
+            allow_insecure=allow_insecure,
         )
 
-        if domain_url.scheme == "http" and not allow_insecure:
-            raise ValueError("Insecure connections are currently disabled.")
-
-        if not domain_url.scheme:
-            new_scheme = "http" if allow_insecure else "https"
-            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
-
-        if domain_url.scheme not in ["http", "https"]:
-            raise ValueError(
-                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
-                "Only http and https are supported."
-            )
-
         # Strip any auth, query or fragment from the domain
-        self.hvcs_domain = parse_url(
+        self._hvcs_domain = parse_url(
             Url(
                 scheme=domain_url.scheme,
                 host=domain_url.host,
                 port=domain_url.port,
                 path=str(PurePosixPath(domain_url.path or "/")),
             ).url.rstrip("/")
         )
 
         self._client = gitlab.Gitlab(self.hvcs_domain.url)
+        self._api_url = parse_url(self._client.url)
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         """
         Get the repository owner and name from GitLab CI environment variables, if
         available, otherwise from parsing the remote url
         """
@@ -93,14 +80,15 @@
 
     @logged_function(log)
     def create_release(
         self,
         tag: str,
         release_notes: str,
         prerelease: bool = False,  # noqa: ARG002
+        assets: list[str] | None = None,  # noqa: ARG002
     ) -> str:
         """
         Post release changelog
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
         :param prerelease: This parameter has no effect
         :return: The tag of the release
@@ -151,79 +139,49 @@
                 "Release %s could not be created for project %s/%s",
                 tag,
                 self.owner,
                 self.repo_name,
             )
             return self.edit_release_notes(release_id=tag, release_notes=release_notes)
 
-    def compare_url(self, from_rev: str, to_rev: str) -> str:
-        return self.create_server_url(
-            path=f"{self.owner}/{self.repo_name}/-/compare/{from_rev}...{to_rev}"
-        )
-
     def remote_url(self, use_token: bool = True) -> str:
         """Get the remote url including the token for authentication if requested"""
         if not (self.token and use_token):
             return self._remote_url
 
         return self.create_server_url(
             auth=f"gitlab-ci-token:{self.token}",
             path=f"{self.owner}/{self.repo_name}.git",
         )
 
+    def compare_url(self, from_rev: str, to_rev: str) -> str:
+        return self.create_repo_url(repo_path=f"/-/compare/{from_rev}...{to_rev}")
+
     def commit_hash_url(self, commit_hash: str) -> str:
-        return self.create_server_url(
-            path=f"{self.owner}/{self.repo_name}/-/commit/{commit_hash}"
-        )
+        return self.create_repo_url(repo_path=f"/-/commit/{commit_hash}")
 
     def issue_url(self, issue_number: str | int) -> str:
-        return self.create_server_url(
-            path=f"{self.owner}/{self.repo_name}/-/issues/{issue_number}"
-        )
+        return self.create_repo_url(repo_path=f"/-/issues/{issue_number}")
 
     def merge_request_url(self, mr_number: str | int) -> str:
-        return self.create_server_url(
-            path=f"{self.owner}/{self.repo_name}/-/merge_requests/{mr_number}"
-        )
+        return self.create_repo_url(repo_path=f"/-/merge_requests/{mr_number}")
 
     def pull_request_url(self, pr_number: str | int) -> str:
+        # TODO: deprecate in v11, add warning in v10
         return self.merge_request_url(mr_number=pr_number)
 
-    def create_server_url(
-        self,
-        path: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        overrides = dict(
-            filter(
-                lambda x: x[1] is not None,
-                {
-                    "auth": auth,
-                    "path": str(PurePosixPath(path or "/")),
-                    "query": query,
-                    "fragment": fragment,
-                }.items(),
-            )
-        )
-        return Url(
-            **{
-                **self.hvcs_domain._asdict(),
-                **overrides,
-            }
-        ).url.rstrip("/")
+    def upload_dists(self, tag: str, dist_glob: str) -> int:
+        return super().upload_dists(tag, dist_glob)
 
-    def create_api_url(
-        self,
-        endpoint: str,
-        auth: str | None = None,
-        query: str | None = None,
-        fragment: str | None = None,
-    ) -> str:
-        api_path = self._client.api_url.replace(self.hvcs_domain.url, "")
-        return self.create_server_url(
-            path=f"{api_path}/{endpoint.lstrip(api_path)}",
-            auth=auth,
-            query=query,
-            fragment=fragment,
+    def get_changelog_context_filters(self) -> tuple[Callable[..., Any], ...]:
+        return (
+            self.create_server_url,
+            self.create_repo_url,
+            self.commit_hash_url,
+            self.compare_url,
+            self.issue_url,
+            self.merge_request_url,
+            self.pull_request_url,
         )
+
+
+RemoteHvcsBase.register(Gitlab)
```

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/hvcs/util.py` & `python_semantic_release-9.6.0/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/version/algorithm.py` & `python_semantic_release-9.6.0/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/version/declaration.py` & `python_semantic_release-9.6.0/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/version/translator.py` & `python_semantic_release-9.6.0/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/semantic_release/version/version.py` & `python_semantic_release-9.6.0/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/conftest.py` & `python_semantic_release-9.6.0/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_changelog.py` & `python_semantic_release-9.6.0/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_generate_config.py` & `python_semantic_release-9.6.0/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_help.py` & `python_semantic_release-9.6.0/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_main.py` & `python_semantic_release-9.6.0/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_publish.py` & `python_semantic_release-9.6.0/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/command_line/test_version.py` & `python_semantic_release-9.6.0/tests/command_line/test_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,64 +98,71 @@
                 lazy_fixture("repo_with_no_tags_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "0.1.0"),
                 (["--build-metadata", "build.12345"], "0.1.0+build.12345"),
+                (["--prerelease"], "0.0.0-rc.1"),
                 (["--patch"], "0.0.1"),
                 (["--minor"], "0.1.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.0.1-rc.1"),
-                (["--minor", "--prerelease"], "0.1.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.0.0-rc.1"),
+                (["--patch", "--as-prerelease"], "0.0.1-rc.1"),
+                (["--minor", "--as-prerelease"], "0.1.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.0.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_single_branch_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "0.1.2"),
                 (["--build-metadata", "build.12345"], "0.1.2+build.12345"),
+                (["--prerelease"], "0.1.1-rc.1"),
                 (["--patch"], "0.1.2"),
                 (["--minor"], "0.2.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.1.2-rc.1"),
-                (["--minor", "--prerelease"], "0.2.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.1.1-rc.1"),
+                (["--patch", "--as-prerelease"], "0.1.2-rc.1"),
+                (["--minor", "--as-prerelease"], "0.2.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.1.2-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_single_branch_and_prereleases_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "0.2.1"),
                 (["--build-metadata", "build.12345"], "0.2.1+build.12345"),
+                # There is already a 0.2.0-rc.1
+                (["--prerelease"], "0.2.0-rc.2"),
                 (["--patch"], "0.2.1"),
                 (["--minor"], "0.3.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.2.1-rc.1"),
-                (["--minor", "--prerelease"], "0.3.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.2.0-rc.2"),
+                (["--patch", "--as-prerelease"], "0.2.1-rc.1"),
+                (["--minor", "--as-prerelease"], "0.3.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.2.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture(
@@ -163,64 +170,70 @@
                 ),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "0.3.0-beta.2"),
                 (["--build-metadata", "build.12345"], "0.3.0-beta.2+build.12345"),
+                (["--prerelease"], "0.3.0-beta.2"),
                 (["--patch"], "0.3.1"),
                 (["--minor"], "0.4.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.3.1-beta.1"),
-                (["--minor", "--prerelease"], "0.4.0-beta.1"),
-                (["--major", "--prerelease"], "1.0.0-beta.1"),
+                (["--prerelease", "--as-prerelease"], "0.3.0-beta.2"),
+                (["--patch", "--as-prerelease"], "0.3.1-beta.1"),
+                (["--minor", "--as-prerelease"], "0.4.0-beta.1"),
+                (["--major", "--as-prerelease"], "1.0.0-beta.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.3.1-beta.1",
+                    ["--patch", "--as-prerelease", "--prerelease-token", "rc"],
+                    "0.3.1-rc.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_git_flow_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "1.2.0-alpha.3"),
                 (["--build-metadata", "build.12345"], "1.2.0-alpha.3+build.12345"),
+                (["--prerelease"], "1.2.0-alpha.3"),
                 (["--patch"], "1.2.1"),
                 (["--minor"], "1.3.0"),
                 (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.2.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.3.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
+                (["--prerelease", "--as-prerelease"], "1.2.0-alpha.3"),
+                (["--patch", "--as-prerelease"], "1.2.1-alpha.1"),
+                (["--minor", "--as-prerelease"], "1.3.0-alpha.1"),
+                (["--major", "--as-prerelease"], "2.0.0-alpha.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "1.2.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_git_flow_and_release_channels_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 ([], "1.1.0-alpha.4"),
                 (["--build-metadata", "build.12345"], "1.1.0-alpha.4+build.12345"),
+                (["--prerelease"], "1.1.0-alpha.4"),
                 (["--patch"], "1.1.1"),
                 (["--minor"], "1.2.0"),
                 (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.1.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.2.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
+                (["--prerelease", "--as-prerelease"], "1.1.0-alpha.4"),
+                (["--patch", "--as-prerelease"], "1.1.1-alpha.1"),
+                (["--minor", "--as-prerelease"], "1.2.0-alpha.1"),
+                (["--major", "--as-prerelease"], "2.0.0-alpha.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "1.1.1-beta.1",
                 ),
             )
         ],
     ],
 )
 def test_version_print(
@@ -287,124 +300,137 @@
             (
                 lazy_fixture("repo_with_no_tags_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "0.1.0+build.12345"),
+                (["--prerelease"], "0.0.0-rc.1"),
                 (["--patch"], "0.0.1"),
                 (["--minor"], "0.1.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.0.1-rc.1"),
-                (["--minor", "--prerelease"], "0.1.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.0.0-rc.1"),
+                (["--patch", "--as-prerelease"], "0.0.1-rc.1"),
+                (["--minor", "--as-prerelease"], "0.1.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.0.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_single_branch_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "0.1.1+build.12345"),
+                (["--prerelease"], "0.1.1-rc.1"),
                 (["--patch"], "0.1.2"),
                 (["--minor"], "0.2.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.1.2-rc.1"),
-                (["--minor", "--prerelease"], "0.2.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.1.1-rc.1"),
+                (["--patch", "--as-prerelease"], "0.1.2-rc.1"),
+                (["--minor", "--as-prerelease"], "0.2.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.1.2-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_single_branch_and_prereleases_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "0.2.0+build.12345"),
+                # There is already a 0.2.0-rc.1
+                (["--prerelease"], "0.2.0-rc.2"),
                 (["--patch"], "0.2.1"),
                 (["--minor"], "0.3.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.2.1-rc.1"),
-                (["--minor", "--prerelease"], "0.3.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
+                (["--prerelease", "--as-prerelease"], "0.2.0-rc.2"),
+                (["--patch", "--as-prerelease"], "0.2.1-rc.1"),
+                (["--minor", "--as-prerelease"], "0.3.0-rc.1"),
+                (["--major", "--as-prerelease"], "1.0.0-rc.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "0.2.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture(
                     "repo_w_github_flow_w_feature_release_channel_angular_commits"
                 ),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "0.3.0-beta.1+build.12345"),
+                (["--prerelease"], "0.3.0-beta.2"),
                 (["--patch"], "0.3.1"),
                 (["--minor"], "0.4.0"),
                 (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.3.1-beta.1"),
-                (["--minor", "--prerelease"], "0.4.0-beta.1"),
-                (["--major", "--prerelease"], "1.0.0-beta.1"),
+                (["--prerelease", "--as-prerelease"], "0.3.0-beta.2"),
+                (["--patch", "--as-prerelease"], "0.3.1-beta.1"),
+                (["--minor", "--as-prerelease"], "0.4.0-beta.1"),
+                (["--major", "--as-prerelease"], "1.0.0-beta.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.3.1-beta.1",
+                    ["--patch", "--as-prerelease", "--prerelease-token", "rc"],
+                    "0.3.1-rc.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_git_flow_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "1.2.0-alpha.2+build.12345"),
+                (["--prerelease"], "1.2.0-alpha.3"),
                 (["--patch"], "1.2.1"),
                 (["--minor"], "1.3.0"),
                 (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.2.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.3.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
+                (["--prerelease", "--as-prerelease"], "1.2.0-alpha.3"),
+                (["--patch", "--as-prerelease"], "1.2.1-alpha.1"),
+                (["--minor", "--as-prerelease"], "1.3.0-alpha.1"),
+                (["--major", "--as-prerelease"], "2.0.0-alpha.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "1.2.1-beta.1",
                 ),
             )
         ],
         *[
             (
                 lazy_fixture("repo_with_git_flow_and_release_channels_angular_commits"),
                 cli_args,
                 expected_stdout,
             )
             for cli_args, expected_stdout in (
                 (["--build-metadata", "build.12345"], "1.1.0-alpha.3+build.12345"),
+                (["--prerelease"], "1.1.0-alpha.4"),
                 (["--patch"], "1.1.1"),
                 (["--minor"], "1.2.0"),
                 (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.1.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.2.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
+                (["--prerelease", "--as-prerelease"], "1.1.0-alpha.4"),
+                (["--patch", "--as-prerelease"], "1.1.1-alpha.1"),
+                (["--minor", "--as-prerelease"], "1.2.0-alpha.1"),
+                (["--major", "--as-prerelease"], "2.0.0-alpha.1"),
                 (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
+                    ["--patch", "--as-prerelease", "--prerelease-token", "beta"],
                     "1.1.1-beta.1",
                 ),
             )
         ],
     ],
 )
 def test_version_no_push_force_level(
@@ -763,15 +789,15 @@
     assert re.match('__version__ = ".*"', removed[0])
     assert added == [f'__version__ = "{expected_new_version}"\n']
 
 
 def test_version_print_last_released_prints_version(
     repo_with_single_branch_tag_commits: Repo, cli_runner: CliRunner
 ):
-    result = cli_runner.invoke(main, [version.name, "--print-last-released"])
+    result = cli_runner.invoke(main, [version_subcmd, "--print-last-released"])
     assert result.exit_code == 0
     assert result.stdout == "0.1.1\n"
 
 
 def test_version_print_last_released_prints_released_if_commits(
     repo_with_single_branch_tag_commits: Repo,
     example_project_dir: ExProjectDir,
@@ -779,19 +805,19 @@
 ):
     new_file = example_project_dir / "temp.txt"
     new_file.write_text("test --print-last-released")
 
     repo_with_single_branch_tag_commits.git.add(str(new_file.resolve()))
     repo_with_single_branch_tag_commits.git.commit(m="fix: temp new file")
 
-    result = cli_runner.invoke(main, [version.name, "--print-last-released"])
+    result = cli_runner.invoke(main, [version_subcmd, "--print-last-released"])
     assert result.exit_code == 0
     assert result.stdout == "0.1.1\n"
 
 
 def test_version_print_last_released_prints_nothing_if_no_tags(
     caplog, repo_with_no_tags_angular_commits: Repo, cli_runner: CliRunner
 ):
-    result = cli_runner.invoke(main, [version.name, "--print-last-released"])
+    result = cli_runner.invoke(main, [version_subcmd, "--print-last-released"])
     assert result.exit_code == 0
     assert result.stdout == ""
     assert "No release tags found." in caplog.text
```

### Comparing `python_semantic_release-9.5.0/tests/conftest.py` & `python_semantic_release-9.6.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 from __future__ import annotations
 
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING
 
 import pytest
+from git import Commit
 
 from tests.fixtures import *
 from tests.util import remove_dir_tree
 
 if TYPE_CHECKING:
     from tempfile import _TemporaryFileWrapper
     from typing import Generator, Protocol
 
+    class MakeCommitObjFn(Protocol):
+        def __call__(self, message: str) -> Commit: ...
+
     class NetrcFileFn(Protocol):
         def __call__(self, machine: str) -> _TemporaryFileWrapper[str]: ...
 
     class TeardownCachedDirFn(Protocol):
         def __call__(self, directory: Path) -> Path: ...
 
 
@@ -80,7 +84,15 @@
     try:
         yield _teardown_cached_dir
     finally:
         # clean up any registered cached directories
         for directory in directories:
             if directory.exists():
                 remove_dir_tree(directory, force=True)
+
+
+@pytest.fixture(scope="session")
+def make_commit_obj() -> MakeCommitObjFn:
+    def _make_commit(message: str) -> Commit:
+        return Commit(repo=Repo(), binsha=Commit.NULL_BIN_SHA, message=message)
+
+    return _make_commit
```

### Comparing `python_semantic_release-9.5.0/tests/const.py` & `python_semantic_release-9.6.0/tests/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,45 +64,16 @@
     "fix\n",
     # Emoji in description should not be used to evaluate change type
     ":sparkles: last minute rush order\n\n:boom: Good thing we're 10x developers",
 ]
 EMOJI_COMMITS_MAJOR = EMOJI_COMMITS_MINOR.copy()
 EMOJI_COMMITS_MAJOR.insert(4, ":boom: Move to the blockchain")
 
-SCIPY_FORMATTED_COMMIT_BODY_PARTS = [
-    # a squash merge that preserved PR commit messages
-    (
-        "DOC: import ropy.transform to test for numpy error",
-        "DOC: lower numpy version",
-        "DOC: lower numpy version further",
-        "MAINT: remove debugging import",
-    ),
-    # empty body
-    (),
-    # formatted body
-    (
-        """Bumps [sphinx](https://github.com/sphinx-doc/sphinx) from 3.5.3 to 4.1.1.
-            - [Release notes](https://github.com/sphinx-doc/sphinx/releases)
-            - [Changelog](https://github.com/sphinx-doc/sphinx/blob/4.x/CHANGES)
-            - [Commits](https://github.com/sphinx-doc/sphinx/commits/v4.1.1)""",
-        """---
-            updated-dependencies:
-            - dependency-name: sphinx
-            dependency-type: direct:development
-            update-type: version-update:semver-major""",
-    ),
-    (
-        "Bug spotted on Fedora, see https://src.fedoraproject.org/rpms/scipy/pull-request/22",
-        "The `int[::]` annotation is used to accept non-contiguous views.",
-    ),
-    ("[skip azp] [skip actions]",),
-]
 
-# Note - the scipy commit testing in v7 is very comprehensive -
-# fixtures for commits that should evaluate to the various scopes
+# Note - the scipy commit fixtures for commits that should evaluate to the various scopes
 # are in tests/fixtures/scipy
 
 
 TAG_COMMITS_PATCH = [
     ":nut_and_bolt: something annoying\n",
     "fixup the bugfix\n",
     "oops it broke again\n",
```

### Comparing `python_semantic_release-9.5.0/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.6.0/tests/fixtures/commit_parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import pytest
 
 from semantic_release.commit_parser import (
     AngularCommitParser,
+    AngularParserOptions,
     EmojiCommitParser,
+    EmojiParserOptions,
     TagCommitParser,
+    TagParserOptions,
 )
 
 # Note scipy defined in ./scipy.py as already used there
 
 
-@pytest.fixture
-def default_angular_parser_options():
-    return AngularCommitParser.parser_options()
+@pytest.fixture(scope="session")
+def default_angular_parser() -> AngularCommitParser:
+    return AngularCommitParser()
 
 
-@pytest.fixture
-def default_angular_parser(default_angular_parser_options):
-    return AngularCommitParser(options=default_angular_parser_options)
+@pytest.fixture(scope="session")
+def default_angular_parser_options(
+    default_angular_parser: AngularCommitParser,
+) -> AngularParserOptions:
+    return default_angular_parser.get_default_options()
 
 
-@pytest.fixture
-def default_emoji_parser_options():
-    return EmojiCommitParser.parser_options()
+@pytest.fixture(scope="session")
+def default_emoji_parser() -> EmojiCommitParser:
+    return EmojiCommitParser()
 
 
-@pytest.fixture
-def default_emoji_parser(default_emoji_parser_options):
-    return EmojiCommitParser(options=default_emoji_parser_options)
+@pytest.fixture(scope="session")
+def default_emoji_parser_options(
+    default_emoji_parser: EmojiCommitParser,
+) -> EmojiParserOptions:
+    return default_emoji_parser.get_default_options()
 
 
-@pytest.fixture
-def default_tag_parser_options():
-    return TagCommitParser.parser_options()
+@pytest.fixture(scope="session")
+def default_tag_parser() -> TagCommitParser:
+    return TagCommitParser()
 
 
-@pytest.fixture
-def default_tag_parser(default_tag_parser_options):
-    return TagCommitParser(options=default_tag_parser_options)
+@pytest.fixture(scope="session")
+def default_tag_parser_options(default_tag_parser: TagCommitParser) -> TagParserOptions:
+    return default_tag_parser.get_default_options()
```

### Comparing `python_semantic_release-9.5.0/tests/fixtures/example_project.py` & `python_semantic_release-9.6.0/tests/fixtures/example_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import os
+from importlib import import_module
 from pathlib import Path
 from textwrap import dedent
 from typing import TYPE_CHECKING, Generator
 
 import pytest
 import tomlkit
 
+import semantic_release
 from semantic_release.commit_parser import (
     AngularCommitParser,
     EmojiCommitParser,
     ScipyCommitParser,
     TagCommitParser,
 )
 from semantic_release.hvcs import Bitbucket, Gitea, Github, Gitlab
@@ -39,14 +41,17 @@
 
     class SetFlagFn(Protocol):
         def __call__(self, flag: bool) -> None: ...
 
     class UpdatePyprojectTomlFn(Protocol):
         def __call__(self, setting: str, value: Any) -> None: ...
 
+    class UseCustomParserFn(Protocol):
+        def __call__(self, module_import_str: str) -> type[CommitParser]: ...
+
     class UseHvcsFn(Protocol):
         def __call__(self, domain: str | None = None) -> type[HvcsBase]: ...
 
     class UseParserFn(Protocol):
         def __call__(self) -> type[CommitParser]: ...
 
     class UseReleaseNotesTemplateFn(Protocol):
@@ -266,79 +271,118 @@
 
         with open(cwd_pyproject_toml, "w") as wfd:
             tomlkit.dump(pyproject_toml, wfd)
 
     return _update_pyproject_toml
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
+def pyproject_toml_config_option_parser() -> str:
+    return f"tool.{semantic_release.__name__}.commit_parser"
+
+
+@pytest.fixture(scope="session")
 def set_major_on_zero(update_pyproject_toml: UpdatePyprojectTomlFn) -> SetFlagFn:
     """Turn on/off the major_on_zero setting."""
 
     def _set_major_on_zero(flag: bool) -> None:
         update_pyproject_toml("tool.semantic_release.major_on_zero", flag)
 
     return _set_major_on_zero
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def set_allow_zero_version(update_pyproject_toml: UpdatePyprojectTomlFn) -> SetFlagFn:
     """Turn on/off the allow_zero_version setting."""
 
     def _set_allow_zero_version(flag: bool) -> None:
         update_pyproject_toml("tool.semantic_release.allow_zero_version", flag)
 
     return _set_allow_zero_version
 
 
 @pytest.fixture(scope="session")
-def use_angular_parser(update_pyproject_toml: UpdatePyprojectTomlFn) -> UseParserFn:
+def use_angular_parser(
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+    pyproject_toml_config_option_parser: str,
+) -> UseParserFn:
     """Modify the configuration file to use the Angular parser."""
 
     def _use_angular_parser() -> type[CommitParser]:
-        update_pyproject_toml("tool.semantic_release.commit_parser", "angular")
+        update_pyproject_toml(pyproject_toml_config_option_parser, "angular")
         return AngularCommitParser
 
     return _use_angular_parser
 
 
 @pytest.fixture(scope="session")
-def use_emoji_parser(update_pyproject_toml: UpdatePyprojectTomlFn) -> UseParserFn:
+def use_emoji_parser(
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+    pyproject_toml_config_option_parser: str,
+) -> UseParserFn:
     """Modify the configuration file to use the Emoji parser."""
 
     def _use_emoji_parser() -> type[CommitParser]:
-        update_pyproject_toml("tool.semantic_release.commit_parser", "emoji")
+        update_pyproject_toml(pyproject_toml_config_option_parser, "emoji")
         return EmojiCommitParser
 
     return _use_emoji_parser
 
 
 @pytest.fixture(scope="session")
-def use_scipy_parser(update_pyproject_toml: UpdatePyprojectTomlFn) -> UseParserFn:
+def use_scipy_parser(
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+    pyproject_toml_config_option_parser: str,
+) -> UseParserFn:
     """Modify the configuration file to use the Scipy parser."""
 
     def _use_scipy_parser() -> type[CommitParser]:
-        update_pyproject_toml("tool.semantic_release.commit_parser", "scipy")
+        update_pyproject_toml(pyproject_toml_config_option_parser, "scipy")
         return ScipyCommitParser
 
     return _use_scipy_parser
 
 
 @pytest.fixture(scope="session")
-def use_tag_parser(update_pyproject_toml: UpdatePyprojectTomlFn) -> UseParserFn:
+def use_tag_parser(
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+    pyproject_toml_config_option_parser: str,
+) -> UseParserFn:
     """Modify the configuration file to use the Tag parser."""
 
     def _use_tag_parser() -> type[CommitParser]:
-        update_pyproject_toml("tool.semantic_release.commit_parser", "tag")
+        update_pyproject_toml(pyproject_toml_config_option_parser, "tag")
         return TagCommitParser
 
     return _use_tag_parser
 
 
 @pytest.fixture(scope="session")
+def use_custom_parser(
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+    pyproject_toml_config_option_parser: str,
+) -> UseCustomParserFn:
+    """Modify the configuration file to use a user defined string parser."""
+
+    def _use_custom_parser(module_import_str: str) -> type[CommitParser]:
+        # validate this is importable before writing to parser
+        module_name, attr = module_import_str.split(":", maxsplit=1)
+        try:
+            module = import_module(module_name)
+            custom_class = getattr(module, attr)
+        except (ModuleNotFoundError, AttributeError) as err:
+            raise ValueError("Custom parser object not found!") from err
+
+        update_pyproject_toml(pyproject_toml_config_option_parser, module_import_str)
+        return custom_class
+
+    return _use_custom_parser
+
+
+@pytest.fixture(scope="session")
 def use_github_hvcs(update_pyproject_toml: UpdatePyprojectTomlFn) -> UseHvcsFn:
     """Modify the configuration file to use GitHub as the HVCS."""
 
     def _use_github_hvcs(domain: str | None = None) -> type[HvcsBase]:
         update_pyproject_toml("tool.semantic_release.remote.type", "github")
         if domain is not None:
             update_pyproject_toml("tool.semantic_release.remote.domain", domain)
```

### Comparing `python_semantic_release-9.5.0/tests/fixtures/git_repo.py` & `python_semantic_release-9.6.0/tests/fixtures/git_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 
     from semantic_release.hvcs import HvcsBase
 
     from tests.conftest import TeardownCachedDirFn
     from tests.fixtures.example_project import (
         ExProjectDir,
         UpdatePyprojectTomlFn,
+        UseCustomParserFn,
         UseHvcsFn,
         UseParserFn,
     )
 
-    CommitConvention = Literal["angular", "emoji", "scipy", "tag"]
+    CommitConvention = Literal["angular", "emoji", "scipy", "tag"] | str
     VersionStr = str
     CommitMsg = str
     ChangelogTypeHeading = str
     TomlSerializableTypes = Union[dict, set, list, tuple, int, float, bool, str]
 
     class RepoVersionDef(TypedDict):
         """
@@ -249,14 +250,15 @@
     use_gitlab_hvcs: UseHvcsFn,
     use_gitea_hvcs: UseHvcsFn,
     use_bitbucket_hvcs: UseHvcsFn,
     use_angular_parser: UseParserFn,
     use_emoji_parser: UseParserFn,
     use_scipy_parser: UseParserFn,
     use_tag_parser: UseParserFn,
+    use_custom_parser: UseCustomParserFn,
     example_git_https_url: str,
     update_pyproject_toml: UpdatePyprojectTomlFn,
 ) -> BuildRepoFn:
     """
     This fixture is intended to simplify repo scenario building by initially
     creating the repo but also configuring semantic_release in the pyproject.toml
     for when the test executes semantic_release. It returns a function so that
@@ -285,15 +287,15 @@
             elif commit_type == "emoji":
                 use_emoji_parser()
             elif commit_type == "scipy":
                 use_scipy_parser()
             elif commit_type == "tag":
                 use_tag_parser()
             else:
-                raise ValueError(f"Unknown parser name: {commit_type}")
+                use_custom_parser(commit_type)
 
             # Set HVCS configuration
             if hvcs_client_name == "github":
                 hvcs_class = use_github_hvcs(hvcs_domain)
             elif hvcs_client_name == "gitlab":
                 hvcs_class = use_gitlab_hvcs(hvcs_domain)
             elif hvcs_client_name == "gitea":
```

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.6.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/scenario/test_next_version.py` & `python_semantic_release-9.6.0/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/scenario/test_release_history.py` & `python_semantic_release-9.6.0/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/scenario/test_template_render.py` & `python_semantic_release-9.6.0/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 from semantic_release.version.translator import Version
 
 from tests.const import TODAY_DATE_STR
 
 if TYPE_CHECKING:
     from git import Actor
 
-    from semantic_release.hvcs import HvcsBase
-
 
 @pytest.fixture
 def default_changelog_template() -> str:
     """Retrieve the semantic-release default changelog template."""
     version_notes_template = files(semantic_release.__name__).joinpath(
         Path("data", "templates", "CHANGELOG.md.j2")
     )
@@ -91,35 +89,36 @@
         },
     )
 
 
 @pytest.mark.parametrize("hvcs_client", [Github, Gitlab, Gitea, Bitbucket])
 def test_default_changelog_template(
     default_changelog_template: str,
-    hvcs_client: type[HvcsBase],
+    hvcs_client: type[Bitbucket | Gitea | Github | Gitlab],
     example_git_https_url: str,
     artificial_release_history: ReleaseHistory,
 ):
     version_str = "1.0.0"
     version = Version.parse(version_str)
     rh = artificial_release_history
     rh.unreleased = {}  # Wipe out unreleased
+    hvcs = hvcs_client(example_git_https_url)
 
     feat_commit_obj = artificial_release_history.released[version]["elements"][
         "feature"
     ][0]
-    feat_commit_url = hvcs_client(example_git_https_url).commit_hash_url(
-        feat_commit_obj.commit.hexsha
-    )
+    assert isinstance(feat_commit_obj, ParsedCommit)
+
+    feat_commit_url = hvcs.commit_hash_url(feat_commit_obj.commit.hexsha)
     feat_description = str.join("\n", feat_commit_obj.descriptions)
 
     fix_commit_obj = artificial_release_history.released[version]["elements"]["fix"][0]
-    fix_commit_url = hvcs_client(example_git_https_url).commit_hash_url(
-        fix_commit_obj.commit.hexsha
-    )
+    fix_commit_url = hvcs.commit_hash_url(fix_commit_obj.commit.hexsha)
+
+    assert isinstance(fix_commit_obj, ParsedCommit)
     fix_description = str.join("\n", fix_commit_obj.descriptions)
 
     expected_changelog = str.join(
         "\n",
         [
             "# CHANGELOG",
             f"## v{version_str} ({TODAY_DATE_STR})",
@@ -139,33 +138,34 @@
     actual_changelog = env.from_string(default_changelog_template).render()
     assert expected_changelog == actual_changelog
 
 
 @pytest.mark.parametrize("hvcs_client", [Github, Gitlab, Gitea, Bitbucket])
 def test_default_changelog_template_w_unreleased_changes(
     default_changelog_template: str,
-    hvcs_client: type[HvcsBase],
+    hvcs_client: type[Bitbucket | Gitea | Github | Gitlab],
     example_git_https_url: str,
     artificial_release_history: ReleaseHistory,
 ):
     version_str = "1.0.0"
     version = Version.parse(version_str)
+    hvcs = hvcs_client(example_git_https_url)
 
     feat_commit_obj = artificial_release_history.released[version]["elements"][
         "feature"
     ][0]
-    feat_commit_url = hvcs_client(example_git_https_url).commit_hash_url(
-        feat_commit_obj.commit.hexsha
-    )
+    assert isinstance(feat_commit_obj, ParsedCommit)
+
+    feat_commit_url = hvcs.commit_hash_url(feat_commit_obj.commit.hexsha)
     feat_description = str.join("\n", feat_commit_obj.descriptions)
 
     fix_commit_obj = artificial_release_history.released[version]["elements"]["fix"][0]
-    fix_commit_url = hvcs_client(example_git_https_url).commit_hash_url(
-        fix_commit_obj.commit.hexsha
-    )
+    fix_commit_url = hvcs.commit_hash_url(fix_commit_obj.commit.hexsha)
+
+    assert isinstance(fix_commit_obj, ParsedCommit)
     fix_description = str.join("\n", fix_commit_obj.descriptions)
 
     expected_changelog = str.join(
         "\n",
         [
             "# CHANGELOG",
             "## Unreleased",
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import json
 from textwrap import dedent
 
 import pytest
-from pytest import lazy_fixture
+from pytest_lazyfixture import lazy_fixture
 
 from semantic_release.cli.util import load_raw_config_file, parse_toml
 from semantic_release.errors import InvalidConfiguration
 
 
 @pytest.mark.parametrize(
     "toml_text, expected",
@@ -170,33 +172,36 @@
 
     return path
 
 
 @pytest.mark.parametrize(
     "raw_config_file, expected",
     [
-        (lazy_fixture("raw_toml_config_file"), {"foo": "bar", "abc": {"bar": "baz"}}),
         (
-            lazy_fixture("raw_pyproject_toml_config_file"),
+            lazy_fixture(raw_toml_config_file.__name__),
+            {"foo": "bar", "abc": {"bar": "baz"}},
+        ),
+        (
+            lazy_fixture(raw_pyproject_toml_config_file.__name__),
             {"foo": "bar", "abc": {"bar": "baz"}},
         ),
         (
-            lazy_fixture("raw_json_config_file"),
+            lazy_fixture(raw_json_config_file.__name__),
             {"foo": "bar", "abc": {"bar": "baz"}},
         ),
     ],
 )
 def test_load_raw_config_file_loads_config(raw_config_file, expected):
     assert load_raw_config_file(raw_config_file) == expected
 
 
 @pytest.mark.parametrize(
     "raw_config_file",
     [
-        lazy_fixture("invalid_toml_config_file"),
-        lazy_fixture("invalid_json_config_file"),
-        lazy_fixture("invalid_other_config_file"),
+        lazy_fixture(invalid_toml_config_file.__name__),
+        lazy_fixture(invalid_json_config_file.__name__),
+        lazy_fixture(invalid_other_config_file.__name__),
     ],
 )
 def test_load_raw_invalid_config_file_raises_error(raw_config_file):
     with pytest.raises(InvalidConfiguration):
         load_raw_config_file(raw_config_file)
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import pytest
 
-from semantic_release.commit_parser.angular import AngularCommitParser
+from semantic_release.commit_parser.angular import (
+    AngularCommitParser,
+    AngularParserOptions,
+)
 from semantic_release.commit_parser.token import ParsedCommit, ParseError
 from semantic_release.enums import LevelBump
 
-from tests.unit.semantic_release.commit_parser.helper import make_commit
-
-
-@pytest.fixture
-def default_options():
-    return AngularCommitParser.parser_options()
+if TYPE_CHECKING:
+    from tests.conftest import MakeCommitObjFn
 
 
-@pytest.fixture
-def default_angular_parser(default_options):
-    return AngularCommitParser(default_options)
-
-
-def test_parser_raises_unknown_message_style(default_angular_parser):
-    assert isinstance(default_angular_parser.parse(make_commit("")), ParseError)
+def test_parser_raises_unknown_message_style(
+    default_angular_parser: AngularCommitParser, make_commit_obj: MakeCommitObjFn
+):
+    assert isinstance(default_angular_parser.parse(make_commit_obj("")), ParseError)
     assert isinstance(
         default_angular_parser.parse(
-            make_commit("feat(parser\n): Add new parser pattern")
+            make_commit_obj("feat(parser\n): Add new parser pattern")
         ),
         ParseError,
     )
 
 
 @pytest.mark.parametrize(
     "commit_message, bump",
@@ -46,17 +46,20 @@
         ("test(parser): Add a test for angular parser", LevelBump.NO_RELEASE),
         ("feat(parser)!: Edit dat parsing stuff", LevelBump.MAJOR),
         ("fix!: Edit dat parsing stuff again", LevelBump.MAJOR),
         ("fix: superfix", LevelBump.PATCH),
     ],
 )
 def test_parser_returns_correct_bump_level(
-    default_angular_parser, commit_message, bump
+    default_angular_parser: AngularCommitParser,
+    commit_message: str,
+    bump: LevelBump,
+    make_commit_obj: MakeCommitObjFn,
 ):
-    result = default_angular_parser.parse(make_commit(commit_message))
+    result = default_angular_parser.parse(make_commit_obj(commit_message))
     assert isinstance(result, ParsedCommit)
     assert result.bump is bump
 
 
 @pytest.mark.parametrize(
     "message, type_",
     [
@@ -65,16 +68,21 @@
         ("test(parser): ...", "test"),
         ("docs(parser): ...", "documentation"),
         ("style(parser): ...", "style"),
         ("refactor(parser): ...", "refactor"),
         ("chore(parser): ...", "chore"),
     ],
 )
-def test_parser_return_type_from_commit_message(default_angular_parser, message, type_):
-    result = default_angular_parser.parse(make_commit(message))
+def test_parser_return_type_from_commit_message(
+    default_angular_parser: AngularCommitParser,
+    message: str,
+    type_: str,
+    make_commit_obj: MakeCommitObjFn,
+):
+    result = default_angular_parser.parse(make_commit_obj(message))
     assert isinstance(result, ParsedCommit)
     assert result.type == type_
 
 
 @pytest.mark.parametrize(
     "message, scope",
     [
@@ -86,17 +94,20 @@
         ("chore(a+part): ...", "a+part"),
         ("chore(a&part): ...", "a&part"),
         ("chore((part)): ...", "(part)"),
         ("chore((p):rt): ...", "(p):rt"),
     ],
 )
 def test_parser_return_scope_from_commit_message(
-    default_angular_parser, message, scope
+    default_angular_parser: AngularCommitParser,
+    message: str,
+    scope: str,
+    make_commit_obj: MakeCommitObjFn,
 ):
-    result = default_angular_parser.parse(make_commit(message))
+    result = default_angular_parser.parse(make_commit_obj(message))
     assert isinstance(result, ParsedCommit)
     assert result.scope == scope
 
 
 _long_text = (
     "This is an long explanatory part of a commit message. It should give "
     "some insight to the fix this commit adds to the codebase."
@@ -117,34 +128,39 @@
             f"fix(tox): Fix env \n\n{_long_text}\n\n{_footer}",
             ["Fix env ", _long_text, _footer],
         ),
         ("fix: superfix", ["superfix"]),
     ],
 )
 def test_parser_return_subject_from_commit_message(
-    default_angular_parser, message, descriptions
+    default_angular_parser: AngularCommitParser,
+    message: str,
+    descriptions: list[str],
+    make_commit_obj: MakeCommitObjFn,
 ):
-    result = default_angular_parser.parse(make_commit(message))
+    result = default_angular_parser.parse(make_commit_obj(message))
     assert isinstance(result, ParsedCommit)
     assert result.descriptions == descriptions
 
 
 ##############################
 # test custom parser options #
 ##############################
-def test_parser_custom_default_level():
-    options = AngularCommitParser.parser_options(default_bump_level=LevelBump.MINOR)
+def test_parser_custom_default_level(make_commit_obj: MakeCommitObjFn):
+    options = AngularParserOptions(default_bump_level=LevelBump.MINOR)
     parser = AngularCommitParser(options)
-    result = parser.parse(make_commit("test(parser): Add a test for angular parser"))
+    result = parser.parse(
+        make_commit_obj("test(parser): Add a test for angular parser")
+    )
     assert isinstance(result, ParsedCommit)
     assert result.bump is LevelBump.MINOR
 
 
-def test_parser_custom_allowed_types():
-    options = AngularCommitParser.parser_options(
+def test_parser_custom_allowed_types(make_commit_obj: MakeCommitObjFn):
+    options = AngularParserOptions(
         allowed_tags=(
             "custom",
             "build",
             "chore",
             "ci",
             "docs",
             "fix",
@@ -152,32 +168,32 @@
             "style",
             "refactor",
             "test",
         )
     )
     parser = AngularCommitParser(options)
 
-    res1 = parser.parse(make_commit("custom: ..."))
+    res1 = parser.parse(make_commit_obj("custom: ..."))
     assert isinstance(res1, ParsedCommit)
     assert res1.bump is LevelBump.NO_RELEASE
 
-    res2 = parser.parse(make_commit("custom(parser): ..."))
+    res2 = parser.parse(make_commit_obj("custom(parser): ..."))
     assert isinstance(res2, ParsedCommit)
     assert res2.type == "custom"
 
-    assert isinstance(parser.parse(make_commit("feat(parser): ...")), ParseError)
+    assert isinstance(parser.parse(make_commit_obj("feat(parser): ...")), ParseError)
 
 
-def test_parser_custom_minor_tags():
-    options = AngularCommitParser.parser_options(minor_tags=("docs",))
+def test_parser_custom_minor_tags(make_commit_obj: MakeCommitObjFn):
+    options = AngularParserOptions(minor_tags=("docs",))
     parser = AngularCommitParser(options)
-    res = parser.parse(make_commit("docs: write some docs"))
+    res = parser.parse(make_commit_obj("docs: write some docs"))
     assert isinstance(res, ParsedCommit)
     assert res.bump is LevelBump.MINOR
 
 
-def test_parser_custom_patch_tags():
-    options = AngularCommitParser.parser_options(patch_tags=("test",))
+def test_parser_custom_patch_tags(make_commit_obj: MakeCommitObjFn):
+    options = AngularParserOptions(patch_tags=("test",))
     parser = AngularCommitParser(options)
-    res = parser.parse(make_commit("test(this): added a test"))
+    res = parser.parse(make_commit_obj("test(this): added a test"))
     assert isinstance(res, ParsedCommit)
     assert res.bump is LevelBump.PATCH
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import pytest
-
-from semantic_release.commit_parser.emoji import EmojiCommitParser
-from semantic_release.enums import LevelBump
+from __future__ import annotations
 
-from tests.unit.semantic_release.commit_parser.helper import make_commit
+from typing import TYPE_CHECKING
 
+import pytest
 
-@pytest.fixture
-def default_options():
-    return EmojiCommitParser.parser_options()
+from semantic_release.commit_parser.token import ParsedCommit
+from semantic_release.enums import LevelBump
 
+if TYPE_CHECKING:
+    from semantic_release.commit_parser.emoji import EmojiCommitParser
 
-@pytest.fixture
-def default_emoji_parser(default_options):
-    return EmojiCommitParser(default_options)
+    from tests.conftest import MakeCommitObjFn
 
 
 @pytest.mark.parametrize(
     "commit_message, bump, type_, descriptions, breaking_descriptions",
     [
         # Major bump
         (
@@ -66,20 +63,23 @@
             ":sparkles:",
             [":sparkles: Add a new feature", ":boom: should not be detected"],
             [],
         ),
     ],
 )
 def test_default_emoji_parser(
-    default_emoji_parser,
-    commit_message,
-    bump,
-    type_,
-    descriptions,
-    breaking_descriptions,
+    default_emoji_parser: EmojiCommitParser,
+    commit_message: str,
+    bump: LevelBump,
+    type_: str,
+    descriptions: list[str],
+    breaking_descriptions: list[str],
+    make_commit_obj: MakeCommitObjFn,
 ):
-    commit = make_commit(commit_message)
-    parsed = default_emoji_parser.parse(commit)
-    assert parsed.bump is bump
-    assert parsed.type == type_
-    assert parsed.descriptions == descriptions
-    assert parsed.breaking_descriptions == breaking_descriptions
+    commit = make_commit_obj(commit_message)
+    result = default_emoji_parser.parse(commit)
+
+    assert isinstance(result, ParsedCommit)
+    assert bump is result.bump
+    assert type_ == result.type
+    assert descriptions == result.descriptions
+    assert breaking_descriptions == result.breaking_descriptions
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-import pytest
-
-from semantic_release.commit_parser.tag import TagCommitParser
-from semantic_release.commit_parser.token import ParseError
-from semantic_release.enums import LevelBump
+from __future__ import annotations
 
-from tests.unit.semantic_release.commit_parser.helper import make_commit
+from typing import TYPE_CHECKING
 
+import pytest
 
-@pytest.fixture
-def default_options():
-    return TagCommitParser.parser_options()
+from semantic_release.commit_parser.token import ParsedCommit, ParseError
+from semantic_release.enums import LevelBump
 
+if TYPE_CHECKING:
+    from semantic_release.commit_parser.tag import TagCommitParser
 
-@pytest.fixture
-def default_tag_parser(default_options):
-    return TagCommitParser(default_options)
+    from tests.conftest import MakeCommitObjFn
 
 
 text = (
     "This is an long explanatory part of a commit message. It should give "
     "some insight to the fix this commit adds to the codebase."
 )
 footer = "Closes #400"
 
 
-def test_parser_raises_unknown_message_style(default_tag_parser):
-    result = default_tag_parser.parse(make_commit(""))
+def test_parser_raises_unknown_message_style(
+    default_tag_parser: TagCommitParser, make_commit_obj: MakeCommitObjFn
+):
+    result = default_tag_parser.parse(make_commit_obj(""))
     assert isinstance(result, ParseError)
 
 
 @pytest.mark.parametrize(
     "commit_message, bump, type_, descriptions",
     [
         (
@@ -61,14 +59,21 @@
             LevelBump.PATCH,
             "fix",
             ["Fix regex in angular parser", text, footer],
         ),
     ],
 )
 def test_default_tag_parser(
-    default_tag_parser, commit_message, bump, type_, descriptions
+    default_tag_parser: TagCommitParser,
+    commit_message: str,
+    bump: LevelBump,
+    type_: str,
+    descriptions: list[str],
+    make_commit_obj: MakeCommitObjFn,
 ):
-    commit = make_commit(commit_message)
-    parsed = default_tag_parser.parse(commit)
-    assert parsed.bump is bump
-    assert parsed.type == type_
-    assert parsed.descriptions == descriptions
+    commit = make_commit_obj(commit_message)
+    result = default_tag_parser.parse(commit)
+
+    assert isinstance(result, ParsedCommit)
+    assert result.bump is bump
+    assert result.type == type_
+    assert result.descriptions == descriptions
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,64 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import pytest
 from pytest_lazyfixture import lazy_fixture
 
 from semantic_release.hvcs._base import HvcsBase
 
 from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
 
+if TYPE_CHECKING:
+    from typing import Any, Callable
+
+
+class ArbitraryHvcs(HvcsBase):
+    def remote_url(self, use_token: bool) -> str:
+        return super().remote_url(use_token)
+
+    def get_changelog_context_filters(self) -> tuple[Callable[..., Any], ...]:
+        return super().get_changelog_context_filters()
+
 
 @pytest.mark.parametrize(
     "remote_url, repo_name",
     [
         (lazy_fixture("example_git_ssh_url"), EXAMPLE_REPO_NAME),
         (lazy_fixture("example_git_https_url"), EXAMPLE_REPO_NAME),
         ("git@my.corp.custom.domain:very_serious/business.git", "business"),
     ],
 )
 def test_get_repository_owner(remote_url, repo_name):
-    client = HvcsBase(remote_url)
+    client = ArbitraryHvcs(remote_url)
     assert client.repo_name == repo_name
 
 
 @pytest.mark.parametrize(
     "remote_url, owner",
     [
         (lazy_fixture("example_git_ssh_url"), EXAMPLE_REPO_OWNER),
         (lazy_fixture("example_git_https_url"), EXAMPLE_REPO_OWNER),
         ("git@my.corp.custom.domain:very_serious/business.git", "very_serious"),
     ],
 )
 def test_get_repository_name(remote_url, owner):
-    client = HvcsBase(remote_url)
+    client = ArbitraryHvcs(remote_url)
     assert client.owner == owner
 
 
 @pytest.mark.parametrize(
     "bad_url",
     [
         "a" * 25,
         "https://a/b/c/d/.git",
         "https://github.com/wrong",
         "git@gitlab.com/somewhere",
     ],
 )
 def test_hvcs_parse_error(bad_url):
-    client = HvcsBase(bad_url)
+    client = ArbitraryHvcs(bad_url)
     with pytest.raises(ValueError):
         _ = client.repo_name
     with pytest.raises(ValueError):
         _ = client.owner
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,99 +35,99 @@
         # API paths are different in BitBucket Cloud (bitbucket.org) vs BitBucket Data Center
         (
             # Default values (BitBucket Cloud)
             {},
             None,
             None,
             f"https://{Bitbucket.DEFAULT_DOMAIN}",
-            f"https://{Bitbucket.DEFAULT_API_DOMAIN}{Bitbucket.DEFAULT_API_PATH_CLOUD}",
+            Bitbucket.DEFAULT_API_URL_CLOUD,
             False,
         ),
         (
             # Explicitly set default values
             {},
             Bitbucket.DEFAULT_DOMAIN,
-            Bitbucket.DEFAULT_API_DOMAIN,
+            Bitbucket.DEFAULT_API_URL_CLOUD,
             f"https://{Bitbucket.DEFAULT_DOMAIN}",
-            f"https://{Bitbucket.DEFAULT_API_DOMAIN}{Bitbucket.DEFAULT_API_PATH_CLOUD}",
+            Bitbucket.DEFAULT_API_URL_CLOUD,
             False,
         ),
-        # (
-        #     # Explicitly set custom values with full api path
-        #     {},
-        #     EXAMPLE_HVCS_DOMAIN,
-        #     f"{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     False,
-        # ),
-        # (
-        #     # Explicitly defined api as subdomain
-        #     # POSSIBLY WRONG ASSUMPTION of Api path for BitBucket Server
-        #     {},
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"https://api.{EXAMPLE_HVCS_DOMAIN}",
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"https://api.{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     False,
-        # ),
-        # (
-        #     # Custom domain for on premise BitBucket Server (derive api endpoint)
-        #     {},
-        #     EXAMPLE_HVCS_DOMAIN,
-        #     None,
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"https://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     False,
-        # ),
-        # (
-        #     # Custom domain with path prefix
-        #     {},
-        #     "special.custom.server/bitbucket",
-        #     None,
-        #     "https://special.custom.server/bitbucket",
-        #     "https://special.custom.server/bitbucket/rest/api/1.0",
-        #     False,
-        # ),
-        # (
-        #     # Allow insecure http connections explicitly
-        #     {},
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     True,
-        # ),
-        # (
-        #     # Allow insecure http connections explicitly & imply insecure api domain
-        #     {},
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     None,
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     True,
-        # ),
-        # (
-        #     # Infer insecure connection from user configuration
-        #     {},
-        #     EXAMPLE_HVCS_DOMAIN,
-        #     f"{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     True,
-        # ),
-        # (
-        #     # Infer insecure connection from user configuration & imply insecure api domain
-        #     {},
-        #     EXAMPLE_HVCS_DOMAIN,
-        #     None,
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}",
-        #     f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
-        #     True,
-        # ),
+        (
+            # Explicitly set custom values with full api path
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            f"{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            False,
+        ),
+        (
+            # Explicitly defined api as subdomain
+            # POSSIBLY WRONG ASSUMPTION of Api path for BitBucket Server
+            {},
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            False,
+        ),
+        (
+            # Custom domain for on premise BitBucket Server (derive api endpoint)
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            None,
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            False,
+        ),
+        (
+            # Custom domain with path prefix
+            {},
+            "special.custom.server/bitbucket",
+            None,
+            "https://special.custom.server/bitbucket",
+            "https://special.custom.server/bitbucket/rest/api/1.0",
+            False,
+        ),
+        (
+            # Allow insecure http connections explicitly
+            {},
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            True,
+        ),
+        (
+            # Allow insecure http connections explicitly & imply insecure api domain
+            {},
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            None,
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            True,
+        ),
+        (
+            # Infer insecure connection from user configuration
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            f"{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            True,
+        ),
+        (
+            # Infer insecure connection from user configuration & imply insecure api domain
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            None,
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/rest/api/1.0",
+            True,
+        ),
     ],
 )
 @pytest.mark.parametrize(
     "remote_url",
     [
         f"git@{Bitbucket.DEFAULT_DOMAIN}:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
         f"https://{Bitbucket.DEFAULT_DOMAIN}/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitea.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,25 @@
         owner=default_gitea_client.owner,
         repo=default_gitea_client.repo_name,
         sha=sha,
     )
     assert expected_url == default_gitea_client.commit_hash_url(sha)
 
 
+@pytest.mark.parametrize("issue_number", (420, "420"))
+def test_issue_url(default_gitea_client: Gitea, issue_number: int | str):
+    expected_url = "{server}/{owner}/{repo}/issues/{issue_number}".format(
+        server=default_gitea_client.hvcs_domain.url,
+        owner=default_gitea_client.owner,
+        repo=default_gitea_client.repo_name,
+        issue_number=issue_number,
+    )
+    assert expected_url == default_gitea_client.issue_url(issue_num=issue_number)
+
+
 @pytest.mark.parametrize("pr_number", (420, "420"))
 def test_pull_request_url(default_gitea_client: Gitea, pr_number: int | str):
     expected_url = "{server}/{owner}/{repo}/pulls/{pr_number}".format(
         server=default_gitea_client.hvcs_domain.url,
         owner=default_gitea_client.owner,
         repo=default_gitea_client.repo_name,
         pr_number=pr_number,
@@ -653,15 +664,15 @@
         mock_get_release_id_by_tag.assert_called_once_with(tag)
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.usefixtures(init_example_project.__name__)
-def test_upload_asset_succeeds(
+def test_upload_release_asset_succeeds(
     default_gitea_client: Gitea,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
     # Setup
     urlparams = {"name": example_changelog_md.name}
@@ -673,15 +684,15 @@
     )
     expected_changelog = example_changelog_md.read_bytes()
 
     with requests_mock.Mocker(session=default_gitea_client.session) as m:
         m.register_uri(
             "POST", gitea_api_matcher, json={"status": "ok"}, status_code=status_code
         )
-        result = default_gitea_client.upload_asset(
+        result = default_gitea_client.upload_release_asset(
             release_id=mock_release_id,
             file=example_changelog_md.resolve(),
             label="doesn't matter could be None",
         )
 
         # Evaluate (expected -> actual)
         assert result is True
@@ -691,15 +702,15 @@
         assert expected_request_url == m.last_request.url
         assert expected_changelog == m.last_request.body.split(b"\r\n")[4]
 
 
 @pytest.mark.parametrize("status_code", (400, 500, 503))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.usefixtures(init_example_project.__name__)
-def test_upload_asset_fails(
+def test_upload_release_asset_fails(
     default_gitea_client: Gitea,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
     # Setup
     urlparams = {"name": example_changelog_md.name}
@@ -715,15 +726,15 @@
         # mock the response
         m.register_uri(
             "POST", gitea_api_matcher, json={"status": "ok"}, status_code=status_code
         )
 
         # Execute method under test expecting an exception to be raised
         with pytest.raises(HTTPError):
-            default_gitea_client.upload_asset(
+            default_gitea_client.upload_release_asset(
                 release_id=mock_release_id,
                 file=example_changelog_md.resolve(),
                 label="doesn't matter could be None",
             )
 
         # Evaluate (expected -> actual)
         assert m.called
@@ -742,23 +753,23 @@
 
     # Set up mock environment
     with mock.patch.object(
         default_gitea_client,
         "get_release_id_by_tag",
         return_value=None,
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gitea_client, "upload_asset"
-    ) as mock_upload_asset:
+        default_gitea_client, "upload_release_asset"
+    ) as mock_upload_release_asset:
         # Execute method under test
         result = default_gitea_client.upload_dists(tag, path)
 
         # Evaluate
         assert expected_num_uploads == result
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
-        mock_upload_asset.assert_not_called()
+        mock_upload_release_asset.assert_not_called()
 
 
 @pytest.mark.parametrize(
     "files, glob_pattern, upload_statuses, expected_num_uploads",
     [
         (["foo.zip", "bar.whl"], "*.zip", [True], 1),
         (["foo.whl", "foo.egg", "foo.tar.gz"], "foo.*", [True, True, True], 3),
@@ -788,17 +799,17 @@
     # Set up mock environment
     with mocked_globber, mocked_isfile, mock.patch.object(
         default_gitea_client,
         "get_release_id_by_tag",
         return_value=release_id,
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gitea_client,
-        "upload_asset",
+        "upload_release_asset",
         side_effect=upload_statuses,
-    ) as mock_upload_asset:
+    ) as mock_upload_release_asset:
         # Execute method under test
         num_uploads = default_gitea_client.upload_dists(tag, glob_pattern)
 
         # Evaluate (expected -> actual)
         assert expected_num_uploads == num_uploads
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
-        assert expected_files_uploaded == mock_upload_asset.call_args_list
+        assert expected_files_uploaded == mock_upload_release_asset.call_args_list
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,17 +372,28 @@
         owner=default_gh_client.owner,
         repo=default_gh_client.repo_name,
         sha=sha,
     )
     assert expected_url == default_gh_client.commit_hash_url(sha)
 
 
+@pytest.mark.parametrize("issue_number", (420, "420"))
+def test_issue_url(default_gh_client: Github, issue_number: str | int):
+    expected_url = "{server}/{owner}/{repo}/issues/{issue_num}".format(
+        server=default_gh_client.hvcs_domain.url,
+        owner=default_gh_client.owner,
+        repo=default_gh_client.repo_name,
+        issue_num=issue_number,
+    )
+    assert expected_url == default_gh_client.issue_url(issue_num=issue_number)
+
+
 @pytest.mark.parametrize("pr_number", (420, "420"))
 def test_pull_request_url(default_gh_client: Github, pr_number: int | str):
-    expected_url = "{server}/{owner}/{repo}/issues/{pr_number}".format(
+    expected_url = "{server}/{owner}/{repo}/pull/{pr_number}".format(
         server=default_gh_client.hvcs_domain,
         owner=default_gh_client.owner,
         repo=default_gh_client.repo_name,
         pr_number=pr_number,
     )
     actual_url = default_gh_client.pull_request_url(pr_number=pr_number)
     assert expected_url == actual_url
@@ -857,15 +868,15 @@
         assert expected_http_method == m.last_request.method
         assert expected_asset_upload_request_url == m.last_request.url
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.usefixtures(init_example_project.__name__)
-def test_upload_asset_succeeds(
+def test_upload_release_asset_succeeds(
     default_gh_client: Github,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
     # Setup
     label = "abc123"
@@ -900,15 +911,15 @@
             status_code=status_code,
         )
         m.register_uri(
             "GET", github_api_matcher, json=json_get_up_url, status_code=status_code
         )
 
         # Execute method under test
-        result = default_gh_client.upload_asset(
+        result = default_gh_client.upload_release_asset(
             release_id=mock_release_id,
             file=example_changelog_md.resolve(),
             label=label,
         )
 
         # Evaluate (expected -> actual)
         assert result is True
@@ -922,15 +933,15 @@
         assert expected_upload_url == post_req.url
         assert expected_changelog == post_req.body
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.usefixtures(init_example_project.__name__)
-def test_upload_asset_fails(
+def test_upload_release_asset_fails(
     default_gh_client: Github,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
     # Setup
     label = "abc123"
@@ -966,15 +977,15 @@
             json={"message": "error"},
             status_code=status_code,
         )
         m.register_uri("GET", github_api_matcher, json=json_get_up_url, status_code=200)
 
         # Execute method under test expecting an exception to be raised
         with pytest.raises(HTTPError):
-            default_gh_client.upload_asset(
+            default_gh_client.upload_release_asset(
                 release_id=mock_release_id,
                 file=example_changelog_md.resolve(),
                 label=label,
             )
 
         # Evaluate (expected -> actual)
         assert m.called
@@ -994,23 +1005,23 @@
 
     # Set up mock environment
     with mock.patch.object(
         default_gh_client,
         "get_release_id_by_tag",
         return_value=None,
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gh_client, "upload_asset"
-    ) as mock_upload_asset:
+        default_gh_client, "upload_release_asset"
+    ) as mock_upload_release_asset:
         # Execute method under test
         result = default_gh_client.upload_dists(tag, path)
 
         # Evaluate
         assert expected_num_uploads == result
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
-        mock_upload_asset.assert_not_called()
+        mock_upload_release_asset.assert_not_called()
 
 
 @pytest.mark.parametrize(
     "files, glob_pattern, upload_statuses, expected_num_uploads",
     [
         (["foo.zip", "bar.whl"], "*.zip", [True], 1),
         (["foo.whl", "foo.egg", "foo.tar.gz"], "foo.*", [True, True, True], 3),
@@ -1040,17 +1051,17 @@
     # Set up mock environment
     with mocked_globber, mocked_isfile, mock.patch.object(
         default_gh_client,
         "get_release_id_by_tag",
         return_value=release_id,
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gh_client,
-        "upload_asset",
+        "upload_release_asset",
         side_effect=upload_statuses,
-    ) as mock_upload_asset:
+    ) as mock_upload_release_asset:
         # Execute method under test
         num_uploads = default_gh_client.upload_dists(tag, glob_pattern)
 
         # Evaluate (expected -> actual)
         assert expected_num_uploads == num_uploads
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
-        assert expected_files_uploaded == mock_upload_asset.call_args_list
+        assert expected_files_uploaded == mock_upload_release_asset.call_args_list
```

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.6.0/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.5.0/tests/util.py` & `python_semantic_release-9.6.0/tests/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 
 from pydantic.dataclasses import dataclass
 
 from semantic_release.changelog.context import make_changelog_context
 from semantic_release.changelog.release_history import ReleaseHistory
 from semantic_release.cli import config as cliConfigModule
 from semantic_release.commit_parser._base import CommitParser, ParserOptions
-from semantic_release.commit_parser.token import ParseResult
+from semantic_release.commit_parser.token import ParsedCommit, ParseResult
+from semantic_release.enums import LevelBump
 
 if TYPE_CHECKING:
     import filecmp
     from pathlib import Path
     from typing import Any, Generator, Iterable, TypeVar
 
     try:
         from typing import TypeAlias
     except ImportError:
         # for python 3.8 and 3.9
         from typing_extensions import TypeAlias
 
     from unittest.mock import MagicMock
 
-    from git import Repo
+    from git import Commit, Repo
 
     from semantic_release.cli.config import RuntimeContext
+    from semantic_release.commit_parser.token import ParseError
 
     _R = TypeVar("_R")
 
     GitCommandWrapperType: TypeAlias = cliConfigModule.Repo.GitCommandWrapperType
 
 
 def copy_dir_tree(src_dir: Path | str, dst_dir: Path | str) -> None:
@@ -169,17 +171,39 @@
 
     for name, method in mocked_methods.items():
         setattr(MockGitCommandWrapperType, f"mocked_{name}", method)
     return MockGitCommandWrapperType
 
 
 class CustomParserWithNoOpts(CommitParser[ParseResult, ParserOptions]):
-    parser_options = ParserOptions
+    def parse(self, commit: Commit) -> ParsedCommit | ParseError:
+        return ParsedCommit(
+            bump=LevelBump.NO_RELEASE,
+            type="",
+            scope="",
+            descriptions=[],
+            breaking_descriptions=[],
+            commit=commit,
+        )
 
 
 @dataclass
 class CustomParserOpts(ParserOptions):
     allowed_tags: Tuple[str, ...] = ("new", "custom")  # noqa: UP006
 
 
 class CustomParserWithOpts(CommitParser[ParseResult, CustomParserOpts]):
     parser_options = CustomParserOpts
+
+    def parse(self, commit: Commit) -> ParsedCommit | ParseError:
+        return ParsedCommit(
+            bump=LevelBump.NO_RELEASE,
+            type="custom",
+            scope="",
+            descriptions=[],
+            breaking_descriptions=[],
+            commit=commit,
+        )
+
+
+class IncompleteCustomParser(CommitParser):
+    pass
```

