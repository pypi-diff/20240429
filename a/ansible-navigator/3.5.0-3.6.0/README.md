# Comparing `tmp/ansible-navigator-3.5.0.tar.gz` & `tmp/ansible-navigator-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.5.0.tar", last modified: Tue Sep 26 11:52:35 2023, max compression
+gzip compressed data, was "ansible-navigator-3.6.0.tar", last modified: Thu Jan 18 14:18:31 2024, max compression
```

## Comparing `ansible-navigator-3.5.0.tar` & `ansible-navigator-3.6.0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.202733 ansible-navigator-3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.github/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55005 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/images/test_tree_view.png
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2023-09-26 11:52:35.202733 ansible-navigator-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.178733 ansible-navigator-3.5.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.182733 ansible-navigator-3.5.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/contributing/guidelines.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.182733 ansible-navigator-3.5.0/docs/contributing/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55005 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/contributing/images/test_tree_view.png
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.182733 ansible-navigator-3.5.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 11:52:35.202733 ansible-navigator-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.174733 ansible-navigator-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.182733 ansible-navigator-3.5.0/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.186733 ansible-navigator-3.5.0/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    27768 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    14369 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21537 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    21313 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (127)    36366 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.186733 ansible-navigator-3.5.0/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.190733 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19988 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15202 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (127)    31838 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    49073 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.190733 ansible-navigator-3.5.0/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24964 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (127)    23617 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.190733 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)    60462 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)    50792 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)    48664 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (127)    48664 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (127)    60462 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (127)    50792 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.194733 ansible-navigator-3.5.0/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.194733 ansible-navigator-3.5.0/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.194733 ansible-navigator-3.5.0/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8697 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.194733 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.198733 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (127)    16065 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9315 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (127)    33455 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.198733 ansible-navigator-3.5.0/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    17966 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.198733 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9655 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 11:52:35.186733 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2023-09-26 11:52:35.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-26 11:52:34.000000 ansible-navigator-3.5.0/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-09-26 11:52:14.000000 ansible-navigator-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.301837 ansible-navigator-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.261838 ansible-navigator-3.6.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.darglint
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/.github/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55005 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-01-18 14:18:31.301837 ansible-navigator-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.265838 ansible-navigator-3.6.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/contributing/guidelines.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.269837 ansible-navigator-3.6.0/docs/contributing/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55005 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/contributing/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.269837 ansible-navigator-3.6.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 14:18:31.301837 ansible-navigator-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.257838 ansible-navigator-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.273837 ansible-navigator-3.6.0/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-18 14:18:30.000000 ansible-navigator-3.6.0/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.277837 ansible-navigator-3.6.0/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27768 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21537 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21313 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36366 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.281837 ansible-navigator-3.6.0/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.281837 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19988 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49053 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.281837 ansible-navigator-3.6.0/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24964 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.285837 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60462 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50792 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48664 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48664 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60462 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50792 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.285837 ansible-navigator-3.6.0/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.285837 ansible-navigator-3.6.0/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.289837 ansible-navigator-3.6.0/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.289837 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.297837 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33455 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.297837 ansible-navigator-3.6.0/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17966 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.297837 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:18:31.297837 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-18 14:18:31.000000 ansible-navigator-3.6.0/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-01-18 14:18:13.000000 ansible-navigator-3.6.0/tox.ini
```

### Comparing `ansible-navigator-3.5.0/.config/dictionary.txt` & `ansible-navigator-3.6.0/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.flake8` & `ansible-navigator-3.6.0/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.git_archival.txt` & `ansible-navigator-3.6.0/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/CONTRIBUTING.md` & `ansible-navigator-3.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/SECURITY.md` & `ansible-navigator-3.6.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/dependabot.yml` & `ansible-navigator-3.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/images/test_tree_view.png` & `ansible-navigator-3.6.0/.github/images/test_tree_view.png`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.github/workflows/release.yml` & `ansible-navigator-3.6.0/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       FORCE_COLOR: 1
       PY_COLORS: 1
       TOXENV: packaging
       TOX_PARALLEL_NO_SPINNER: 1
 
     steps:
       - name: Switch to using Python 3.9 by default
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.9
       - name: Install tox
         run: >-
           python3 -m
           pip install
           --user
```

### Comparing `ansible-navigator-3.5.0/.github/workflows/tox.yml` & `ansible-navigator-3.6.0/.github/workflows/tox.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,20 @@
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
           min_python: "3.9"
-          max_python: "3.11"
+          max_python: "3.12"
           default_python: "3.11" # used by jobs in other_names
           other_names: |
             lint
             docs
+          platforms: linux,macos
   tox:
     name: ${{ matrix.name }} / python ${{ matrix.python_version }}
     environment: test
     runs-on: ubuntu-20.04
     needs: pre
     strategy:
       fail-fast: false
@@ -50,15 +51,15 @@
         uses: actions/cache@v3
         with:
           path: |
             ~/.local/share/containers
           key: ${{ runner.os }}-${{ hashFiles('src/ansible_navigator/data/images_dockerfile') }}
 
       - name: Set up Python ${{ matrix.python_version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python_version }}
 
       - name: Install tox
         run: python3 -m pip install --upgrade "tox>=4.0.2"
 
       - name: Log Python info (${{ matrix.python_version }})
@@ -74,18 +75,17 @@
       - name: tox -e no-test-deps
         if: ${{ startsWith(matrix.passed_name, 'py') }}
         continue-on-error: ${{ matrix.devel || false }}
         run: python3 -m tox -e no-test-deps
 
       - name: Upload coverage data
         if: ${{ startsWith(matrix.passed_name, 'py') }}
-        uses: codecov/codecov-action@v4.0.0-beta.3
+        uses: codecov/codecov-action@v3
         with:
           name: ${{ matrix.passed_name }}
-          fail_ci_if_error: false # see https://github.com/codecov/codecov-action/issues/598
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true # optional (default = false)
       - name: Change accessibility for cache
         if: ${{ startsWith(matrix.passed_name, 'py') }}
         run: podman unshare chmod -R 755 ~/.local/share/containers/
 
   check: # This job does nothing and is only used for the branch protection
```

### Comparing `ansible-navigator-3.5.0/.gitignore` & `ansible-navigator-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.pre-commit-config.yaml` & `ansible-navigator-3.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 exclude: >
   (?x)^(
     _readthedocs|
     .tox
   )$
 repos:
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.3"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         # Original hook implementation is flaky due to *several* bugs described
         # in https://github.com/prettier/prettier/issues/12364
         # a) CI=1 needed to avoid incomplete output
         # b) two executions are needed because --list-different works correctly
         # only when run with --check as with --write the output will also
@@ -30,39 +30,44 @@
         pass_filenames: false
         args: []
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
 
   - repo: https://github.com/psf/black.git
-    rev: 23.9.1
+    rev: 23.12.1
     hooks:
       - id: black
         language_version: python3
 
+  - repo: https://github.com/pappasam/toml-sort
+    rev: v0.23.1
+    hooks:
+      - id: toml-sort-fix
+
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.291"
+    rev: "v0.1.9"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v7.3.0
+    rev: v8.2.0
     hooks:
       - id: cspell
         name: Spell check with cspell
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
     rev: v1.5.4
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       # Side-effects:
       - id: trailing-whitespace
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: requirements-txt-fixer
       - id: check-added-large-files
@@ -85,15 +90,15 @@
     # Allow json comments, trailing commas
     # https://github.com/pre-commit/pre-commit-hooks/issues/395
     rev: v1.0.0
     hooks:
       - id: check-json5
 
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.37.0
+    rev: v0.38.0
     hooks:
       - id: markdownlint
         exclude: >
           (?x)^
             (
               \.github/ISSUE_TEMPLATE/\w+|
               docs/(
@@ -102,15 +107,15 @@
               )|
               README|
               src/ansible_navigator/data/(help|welcome)
             )\.md
           $
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.6
     hooks:
       - id: codespell
         # NOTE: dout is part of the stdout action regex
         args: ["-L", "dout"]
         # We exclude generated and external files as they are not directly under
         # our control, so we cannot fix spelling in them.
         exclude: >
@@ -118,15 +123,15 @@
             (
               tests/fixtures/integration/actions/.*\.json|
               src/ansible_navigator/data/grammar/.*\.json
             )
           $
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.32.0
+    rev: v1.33.0
     hooks:
       - id: yamllint
         args:
           - --strict
         types: [file, yaml]
 
   - repo: https://github.com/PyCQA/flake8.git
@@ -136,20 +141,20 @@
         language_version: python3
         additional_dependencies:
           - darglint
           - flake8-docstrings # uses pydocstyle
 
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
-    rev: v3.13.0
+    rev: v3.15.0
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.5.1
+    rev: v1.7.1
     hooks:
       - id: mypy
         additional_dependencies:
           - jinja2
           - libtmux
           - pytest
           - pytest-mock
@@ -157,15 +162,15 @@
           - types-docutils
           - types-mock
           - types-PyYAML
           - types-setuptools # Needed logging version
           - types-typed-ast
 
   - repo: https://github.com/pycqa/pylint.git
-    rev: v3.0.0a7
+    rev: v3.0.3
     hooks:
       - id: pylint
         args:
           - docs/
           - src/
           - tests/
         additional_dependencies:
```

### Comparing `ansible-navigator-3.5.0/.prettierignore` & `ansible-navigator-3.6.0/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.vscode/launch.json` & `ansible-navigator-3.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/.vscode/settings.json` & `ansible-navigator-3.6.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/LICENSE` & `ansible-navigator-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/PKG-INFO` & `ansible-navigator-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.5.0
+Version: 3.6.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
@@ -19,14 +19,15 @@
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-builder>=3.0.0
 Requires-Dist: ansible-runner<3,>=2.3.1
```

### Comparing `ansible-navigator-3.5.0/README.md` & `ansible-navigator-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/cspell.config.yaml` & `ansible-navigator-3.6.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.6.0/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/contributing/guidelines.md` & `ansible-navigator-3.6.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/contributing/images/test_tree_view.png` & `ansible-navigator-3.6.0/docs/contributing/images/test_tree_view.png`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/contributing/security.md` & `ansible-navigator-3.6.0/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/faq.md` & `ansible-navigator-3.6.0/docs/faq.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ### What is an execution environment?
 
 An execution environment is a container image serving as an Ansible control
 node.
 
 See the
-[Getting started with Execution Environments guide](https://docs.ansible.com/ansible/devel/getting_started_ee/index.html)
+[Getting started with Execution Environments guide](https://ansible.readthedocs.io/en/latest/getting_started_ee/index.html)
 for details.
 
 ## The `ansible.cfg` file
 
 ### Where should the `ansible.cfg` file go when using an execution environment?
 
 The easiest place to have the `ansible.cfg` is in the project directory adjacent
@@ -31,15 +31,15 @@
 
 ## Placement of ansible collections
 
 ### Where should ansible collections be placed when using an execution environment?
 
 The easiest place to have ansible collections is in the project directory, in a
 playbook adjacent collections directory. (eg
-`ansible-galaxy collections install ansible.utils -p ./collections`). The
+`ansible-galaxy collection install ansible.utils -p ./collections`). The
 playbook directory is automatically mounted in the execution environment and the
 collections should be found. Another option is to build the collections into an
 execution environment using
 [ansible builder](https://ansible-builder.readthedocs.io/en/latest/). This was
 done to help playbook developers author playbooks that are production ready, as
 both ansible controller and awx support playbook adjacent collection
 directories. If the collections are in another directory, the
@@ -247,14 +247,28 @@
 `ansible-navigator` parameters or delimited by a `--`
 
 ```bash
 $ ansible-navigator run site.yml --forks 15
 $ ansible-navigator run site.yml -- --forks 15
 ```
 
+### How can I use syntax-check with `ansible-navigator`?
+
+To check for basic syntax errors in an Ansible playbook, one can use
+`ansible-navigator run` command to validate the syntax of a playbook. This also
+allows user to specify an EE while validating the syntax.
+
+```bash
+$ ansible-navigator run site.yml -m stdout --syntax-check
+```
+
+In case of any failure in syntax validation, a syntax error is reported with the
+output that includes the approximate location of the syntax issue in the
+playbook.
+
 ### How can I use a vault password with `ansible-navigator`?
 
 The following options provide a vault password to `ansible-navigator` when using
 the text-based user interface (TUI). **Please ensure these do not conflict with
 your enterprise security standards. Do not add password files to source
 control.**
```

### Comparing `ansible-navigator-3.5.0/docs/index.md` & `ansible-navigator-3.6.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 A demo of the interface can be found [on YouTube][yt demo].
 
 [yt demo]: https://www.youtube.com/watch?v=J9PBKi8ydi4
 
 To learn how to easily start leveraging the container technology with
 `ansible-navigator`, see the
-[Getting started with Execution Environments guide](https://docs.ansible.com/ansible/devel/getting_started_ee/index.html).
+[Getting started with Execution Environments guide](https://ansible.readthedocs.io/en/latest/getting_started_ee/index.html).
 
 - [Installation](installation.md)
 - [Settings](settings.md)
 - [Subcommands](subcommands.md)
 - [FAQ](faq.md)
 
 Contributions
```

### Comparing `ansible-navigator-3.5.0/docs/installation.md` & `ansible-navigator-3.6.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/settings.md` & `ansible-navigator-3.6.0/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/docs/subcommands.md` & `ansible-navigator-3.6.0/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.6.0/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/mkdocs.yml` & `ansible-navigator-3.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/mypy.ini` & `ansible-navigator-3.6.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/pyproject.toml` & `ansible-navigator-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
   # Essentials
   "setuptools >= 45",
   # Plugins
   "setuptools_scm[toml] >= 6.2",
-  "setuptools_scm_git_archive >= 1.1",
+  "setuptools_scm_git_archive >= 1.1"
 ]
 
 [project]
 requires-python = ">=3.9"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
@@ -20,35 +20,36 @@
   'Topic :: Utilities',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
   'Programming Language :: Python :: Implementation :: CPython',
-  'Programming Language :: Python :: Implementation :: PyPy',
+  'Programming Language :: Python :: Implementation :: PyPy'
 ]
 dynamic = ["version", "dependencies", "optional-dependencies"]
 name = "ansible-navigator"
 description = "A text-based user interface (TUI) for the Red Hat Ansible Automation Platform"
 readme = "README.md"
-authors = [{ "name" = "Bradley A. Thornton", "email" = "bthornto@redhat.com" }]
-maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
-license = { text = "Apache" }
+authors = [{"name" = "Bradley A. Thornton", "email" = "bthornto@redhat.com"}]
+maintainers = [{"name" = "Ansible by Red Hat", "email" = "info@ansible.com"}]
+license = {text = "Apache"}
 keywords = ["ansible"]
 
+[project.scripts]
+ansible-navigator = "ansible_navigator.cli:main"
+
 [project.urls]
 homepage = "https://github.com/ansible/ansible-navigator"
 documentation = "https://ansible-navigator.readthedocs.io/en/latest/"
 repository = "https://github.com/ansible/ansible-navigator"
 changelog = "https://github.com/ansible/ansible-navigator/releases"
 
-[project.scripts]
-ansible-navigator = "ansible_navigator.cli:main"
-
 [tool]
 
 [tool.black]
 line-length = 100
 
 [tool.coverage.paths]
 source = ["src", ".tox/*/site-packages"]
@@ -71,22 +72,21 @@
 max-line-length = 100
 
 [tool.pylint.imports]
 preferred-modules = [
   # NOTE: The unittest replacements below help keep
   # NOTE: the tests pytest ecosystem-oriented.
   "unittest:pytest",
-  "unittest.mock:pytest-mock",
+  "unittest.mock:pytest-mock"
 ]
 
 [tool.pylint.master]
 ignore = [
   "_version.py", # built by setuptools_scm
-  "tm_tokenize", # tm_tokenize is virtually vendored and shouldn't be linted as such
-
+  "tm_tokenize" # tm_tokenize is virtually vendored and shouldn't be linted as such
 ]
 # pylint defaults + fh for with open .. as (f|fh)
 good-names = "i,j,k,ex,Run,_,f,fh"
 jobs = 0
 no-docstring-rgx = "__.*__"
 
 [tool.pylint.messages_control]
@@ -204,28 +204,28 @@
   "W1304", # unused-format-string-argument / ruff F507
   "W1308", # duplicate-string-formatting-argument / ruff PLW1308
   "W1309", # f-string-without-interpolation / ruff F541
   "W1310", # format-string-without-interpolation / ruff PLW1310
   "W1401", # anomalous-backslash-in-string / ruff W605
   "W1405", # inconsistent-quotes / ruff Q000
   "W1508", # invalid-envvar-default / ruff PLW1508
-  "W1515", # forgotten-debug-statement / ruff T100
-
+  "W1515" # forgotten-debug-statement / ruff T100
 ]
 enable = [
-  "useless-suppression", # Identify unneeded pylint disable statements
-
+  "useless-suppression" # Identify unneeded pylint disable statements
 ]
 
 [tool.pytest.ini_options]
 addopts = "-n=auto --dist=loadfile --maxfail=10 --durations=30 --showlocals"
 filterwarnings = [
   "error",
   # https://github.com/ansible/ansible-runner/issues/1246
   "ignore::ResourceWarning:ansible_runner",
+  "ignore::pytest.PytestUnraisableExceptionWarning",
+  "ignore::DeprecationWarning:ansible_runner"
 ]
 
 [tool.ruff]
 fix = true
 line-length = 100
 builtins = ["__"]
 select = ["ALL"]
@@ -261,16 +261,14 @@
   'D101', # Missing docstring in public class
   'D102', # Missing docstring in public method
   'D103', # Missing docstring in public function
   'D104', # Missing docstring in public package
   'D105', # Missing docstring in magic method
   'D400', # [*] First line should end with a period
   'D403', # [*] First word of the first line should be capitalized: `tokenize` -> `Tokenize`
-  'DTZ003', # The use of `datetime.datetime.utcnow()` is not allowed, use `datetime.datetime.now(tz=)` instead
-  'DTZ005', # The use of `datetime.datetime.now()` without `tz` argument is not allowed
   'ERA001', # [*] Found commented-out code
   'F401', # [*] `ansible_navigator.version.__version__` imported but unused
   'FBT001', # Boolean positional arg in function definition
   'FBT002', # Boolean default value in function definition
   'FBT003', # Boolean positional value in function call
   'FIX001', # Line contains FIXME
   'FIX002', # Line contains TODO
@@ -354,33 +352,32 @@
   'TD002', # Missing author in TODO
   'TD003', # Missing issue link on the line following this TODO
   'TRY003', # Avoid specifying long messages outside the exception class
   'TRY004', # Prefer `TypeError` exception for invalid type
   'TRY300', # Consider moving this statement to an `else` block
   'TRY301', # Abstract `raise` to an inner function
   'TRY400', # Use `logging.exception` instead of `logging.error`
-  'TRY401', # Redundant exception object included in `logging.exception` call
-
+  'TRY401' # Redundant exception object included in `logging.exception` call
 ]
 exclude = ["tests/fixtures/**", ".git"]
 
+[tool.ruff.flake8-pytest-style]
+parametrize-values-type = "tuple"
+
 [tool.ruff.isort]
 force-single-line = true # Force from .. import to be 1 per line
 known-first-party = ["ansible_navigator"]
 lines-after-imports = 2 # Ensures consistency for cases when there's variable vs function/class definitions after imports
 lines-between-types = 1 # Separate import/from with 1 line
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
-[tool.ruff.flake8-pytest-style]
-parametrize-values-type = "tuple"
-
 [tool.setuptools.dynamic]
-optional-dependencies.test = { file = [".config/requirements-test.txt"] }
-optional-dependencies.lock = { file = [".config/requirements-lock.txt"] }
-optional-dependencies.docs = { file = [".config/requirements-docs.txt"] }
-dependencies = { file = [".config/requirements.in"] }
+dependencies = {file = [".config/requirements.in"]}
+optional-dependencies.test = {file = [".config/requirements-test.txt"]}
+optional-dependencies.lock = {file = [".config/requirements-lock.txt"]}
+optional-dependencies.docs = {file = [".config/requirements-docs.txt"]}
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/ansible_navigator/_version.py"
```

### Comparing `ansible-navigator-3.5.0/requirements.txt` & `ansible-navigator-3.6.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,132 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # To update, run:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=resolvelib --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
 ansible-builder==3.0.0
-ansible-core==2.15.1
-ansible-lint==6.19.0
-ansible-runner==2.3.3
-attrs==23.1.0
+ansible-compat==4.1.10
+ansible-core==2.15.8
+ansible-lint==6.22.1
+ansible-runner==2.3.4
+attrs==23.2.0
+babel==2.14.0
 beautifulsoup4==4.12.2
 bindep==2.11.0
-cairocffi==1.6.0
-cairosvg==2.7.0
-certifi==2023.5.7
-cffi==1.15.1
-cfgv==3.3.1
-charset-normalizer==3.1.0
-click==8.1.3
+black==23.12.1
+bracex==2.4
+cairocffi==1.6.1
+cairosvg==2.7.1
+certifi==2023.11.17
+cffi==1.16.0
+cfgv==3.4.0
+charset-normalizer==3.3.2
+click==8.1.7
 colorama==0.4.6
-coverage==7.2.7
+coverage==7.4.0
 coverage-enable-subprocess==1.0
-cryptography==41.0.1
+cryptography==41.0.7
 csscompressor==0.9.5
 cssselect2==0.7.0
 darglint==1.8.1
 defusedxml==0.7.1
-distlib==0.3.6
-distro==1.8.0
+distlib==0.3.8
+distro==1.9.0
 docutils==0.20.1
-exceptiongroup==1.1.2
-execnet==1.9.0
-filelock==3.12.2
-flake8==6.0.0
+exceptiongroup==1.2.0
+execnet==2.0.2
+filelock==3.13.1
+flake8==6.1.0
 flake8-docstrings==1.7.0
 ghp-import==2.1.0
-griffe==0.31.0
+griffe==0.38.1
 htmlmin2==0.1.13
-identify==2.5.24
-idna==3.4
+identify==2.5.33
+idna==3.6
 importlib-metadata==6.2.1 ; python_version < "3.10.0"
 importlib-resources==5.0.7
 iniconfig==2.0.0
 jinja2==3.1.2
 jsmin==3.0.1
-jsonschema==4.18.0
-jsonschema-specifications==2023.6.1
+jsonschema==4.20.0
+jsonschema-specifications==2023.12.1
 libtmux==0.16.1
 lockfile==0.12.2
-markdown==3.3.7
-markdown-exec==1.6.0
+markdown==3.5.1
+markdown-exec==1.7.0
 markdown-include==0.8.1
+markdown-it-py==3.0.0
 markupsafe==2.1.3
 mccabe==0.7.0
+mdurl==0.1.2
 mergedeep==1.3.4
-mkdocs==1.4.3
-mkdocs-ansible==0.1.6
-mkdocs-autorefs==0.4.1
+mkdocs==1.5.3
+mkdocs-ansible==0.2.0
+mkdocs-autorefs==0.5.0
 mkdocs-gen-files==0.5.0
-mkdocs-htmlproofer-plugin==0.13.1
-mkdocs-material==9.1.18
-mkdocs-material-extensions==1.1.1
-mkdocs-minify-plugin==0.6.4
+mkdocs-htmlproofer-plugin==1.0.0
+mkdocs-material==9.5.3
+mkdocs-material-extensions==1.3.1
+mkdocs-minify-plugin==0.7.2
 mkdocs-monorepo-plugin==1.0.5
-mkdocstrings==0.22.0
-mkdocstrings-python==1.1.2
+mkdocstrings==0.24.0
+mkdocstrings-python==1.7.5
+mypy-extensions==1.0.0
 nodeenv==1.8.0
-onigurumacffi==1.2.0
-packaging==23.1
+onigurumacffi==1.3.0
+packaging==23.2
+paginate==0.5.6
 parsley==1.3
-pbr==5.11.1
-pexpect==4.8.0
-pillow==10.0.0
-pipdeptree==2.9.3
-platformdirs==3.8.0
-pluggy==1.2.0
-pre-commit==3.3.3
+pathspec==0.12.1
+pbr==6.0.0
+pexpect==4.9.0
+pillow==10.2.0
+pipdeptree==2.13.1
+platformdirs==4.1.0
+pluggy==1.3.0
+pre-commit==3.6.0
 ptyprocess==0.7.0
-pycodestyle==2.10.0
+pycodestyle==2.11.1
 pycparser==2.21
 pydocstyle==6.3.0
-pyflakes==3.0.1
-pygments==2.15.1
-pymdown-extensions==10.0.1
-pytest==7.4.0
-pytest-mock==3.11.1
+pyflakes==3.1.0
+pygments==2.17.2
+pymdown-extensions==10.7
+pytest==7.4.4
+pytest-mock==3.12.0
 pytest-plus==0.4.0
 pytest-subtests==0.11.0
-pytest-xdist==3.3.1
+pytest-xdist==3.5.0
 python-daemon==3.0.1
 python-dateutil==2.8.2
 python-slugify==8.0.1
-pyyaml==6.0
+pyyaml==6.0.1
 pyyaml-env-tag==0.1
-referencing==0.29.1
-regex==2023.6.3
+referencing==0.32.0
+regex==2023.12.25
 requests==2.31.0
 requirements-parser==0.5.0
-rpds-py==0.7.1
+rich==13.7.0
+rpds-py==0.16.2
+ruamel-yaml==0.18.5
 six==1.16.0
 snowballstemmer==2.2.0
-soupsieve==2.4.1
+soupsieve==2.5
+subprocess-tee==0.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
-types-setuptools==68.0.0.1
-typing-extensions==4.7.1 ; python_version < "3.10.0"
-tzdata==2023.3
-urllib3==2.0.3
-virtualenv==20.23.1
+types-setuptools==69.0.0.0
+typing-extensions==4.9.0 ; python_version < "3.10.0"
+tzdata==2023.4
+urllib3==2.1.0
+virtualenv==20.25.0
 watchdog==3.0.0
+wcmatch==8.5
 webencodings==0.5.1
-zipp==3.15.0
+yamllint==1.33.0
+zipp==3.17.0
 
 # The following packages are considered to be unsafe in a requirements file:
 # resolvelib
+# ruamel-yaml-clib
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.6.0/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/action_base.py` & `ansible-navigator-3.6.0/src/ansible_navigator/action_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.6.0/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.6.0/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/exec.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/help_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/images.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import json
 import os
 import shlex
 
 from collections.abc import Mapping
 from datetime import datetime
+from datetime import timezone
 from enum import IntEnum
 from typing import Any
 
 from ansible_navigator.action_base import ActionBase
 from ansible_navigator.action_defs import RunStdoutReturn
 from ansible_navigator.app_public import AppPublic
 from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
@@ -351,15 +352,15 @@
         return None
 
     def update(self):
         """Request calling app update, and update modification time if needed."""
         self._calling_app.update()
 
         # Do this only every 2 seconds
-        if (datetime.now() - self._modification_times_last_updated).total_seconds() > 2:
+        if (datetime.now(timezone.utc) - self._modification_times_last_updated).total_seconds() > 2:
             rerun_lint = self._rerun_needed()
             if rerun_lint:
                 self._build_issues_menu()
 
     @property
     def _max_severity_color(self):
         """Determine the color of the maximum severity issue.
@@ -502,11 +503,11 @@
                     rerun_lint = True
                     continue
 
                 # Has the file changed
                 if unix_ts > previous_ts:
                     rerun_lint = True
 
-        self._modification_times_last_updated = datetime.now()
+        self._modification_times_last_updated = datetime.now(timezone.utc)
         if rerun_lint:
             self._logger.debug("Files modified")
         return rerun_lint
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/log.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/settings.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.6.0/src/ansible_navigator/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/app_public.py` & `ansible-navigator-3.6.0/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/cli.py` & `ansible-navigator-3.6.0/src/ansible_navigator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.6.0/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 
 navigator_subcommands = [
     SubCommand(
         name="builder",
         description=(
             "Build [execution environment]"
-            "(https://docs.ansible.com/ansible/devel/getting_started_ee/index.html) "
+            "(https://ansible.readthedocs.io/en/latest/getting_started_ee/index.html) "
             "(container image)"
         ),
         epilog=(
             "Note: 'ansible-navigator builder' additionally supports"
             " the same parameters as the 'ansible-builder' command."
             " For more information about these, try "
             " 'ansible-navigator builder --help-builder --mode stdout'"
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,15 +866,15 @@
                 "--snippet",  # Print a snippet
                 "--metadata-dump",  # Print a metadata dump
             }
             cmdline = config.entry("cmdline").value.current
             if isinstance(cmdline, list) and force_stdout_for.intersection(cmdline):
                 mode = Mode.STDOUT
                 self._requested_mode.append(ModeChangeRequest(entry=entry.name, mode=mode))
-                message = message = f"`{entry.name} requesting mode {mode.value}"
+                message = f"`{entry.name} requesting mode {mode.value}"
                 messages.append(LogMessage(level=logging.DEBUG, message=message))
                 return messages, exit_messages
 
         is_not_set = entry.value.current is C.NOT_SET
         if is_not_set:
             # A plugin name is required
             exit_msg = "A plugin name or other parameter is required when using the doc subcommand"
@@ -1069,15 +1069,15 @@
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
 
         if entry.value.source is not C.DEFAULT_CFG and config.app == "settings":
             mode = Mode.STDOUT
             self._requested_mode.append(ModeChangeRequest(entry=entry.name, mode=mode))
-            message = message = f"`{entry.name} requesting mode {mode.value}"
+            message = f"`{entry.name} requesting mode {mode.value}"
             messages.append(LogMessage(level=logging.DEBUG, message=message))
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def set_environment_variable(
         entry: SettingsEntry,
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.6.0/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/constants.py` & `ansible-navigator-3.6.0/src/ansible_navigator/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants for ansible-navigator."""
 import importlib.resources as importlib_resources
 
-from importlib.abc import Traversable
+from ansible_navigator.utils.compatibility import Traversable
 
 
 PKG_NAME: str = "ansible_navigator"
 DATA_DIR: Traversable = importlib_resources.files(PKG_NAME).joinpath("data")
 
 THEME_DIR: Traversable = DATA_DIR.joinpath("themes")
 THEME_NAME: str = "dark_vs.json"
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.6.0/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/ansible-navigator.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.6.0/src/ansible_navigator/data/catalog_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import subprocess
 import sys
 
 from collections import Counter
 from collections import OrderedDict
 from collections.abc import Generator
 from datetime import datetime
+from datetime import timezone
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Any
 
 import yaml
 
@@ -389,15 +390,15 @@
             q_message = {
                 "plugin": {
                     "doc": doc,
                     "examples": examples,
                     "returndocs": returndocs,
                     "metadata": metadata,
                 },
-                "timestamp": datetime.utcnow().isoformat(),
+                "timestamp": datetime.now(timezone.utc).isoformat(),
             }
             completed_queue.put(("plugin", (checksum, json.dumps(q_message, default=str))))
         except JSONDecodeError as exc:
             err_message = f"{type(exc).__name__} (json_decode_doc): {exc!s}"
             completed_queue.put(("error", (checksum, plugin_path, err_message)))
 
 
@@ -585,24 +586,24 @@
         "errors": errors,
         "stats": stats,
         "messages": cc_obj._messages,
     }
 
 
 if __name__ == "__main__":
-    start_time = datetime.now()
+    start_time = datetime.now(timezone.utc)
 
     collection_paths = retrieve_collections_paths()
     if "error" in collection_paths:
         sys.exit(collection_paths["error"])
     else:
         current_collection_paths = collection_paths["result"]
 
     args, parent_directories = parse_args()
 
     COLLECTION_SCAN_PATHS = ":".join(str(parent) for parent in parent_directories)
     os.environ["ANSIBLE_COLLECTIONS_PATHS"] = COLLECTION_SCAN_PATHS
 
     result = main()
-    result["stats"]["duration"] = (datetime.now() - start_time).total_seconds()
+    result["stats"]["duration"] = (datetime.now(timezone.utc) - start_time).total_seconds()
     result["collection_scan_paths"] = COLLECTION_SCAN_PATHS
     print(json.dumps(result, default=str))
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/help.md` & `ansible-navigator-3.6.0/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.6.0/src/ansible_navigator/data/image_introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.6.0/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.6.0/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.6.0/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.6.0/src/ansible_navigator/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Produce a diagnostics report in json format."""
 from __future__ import annotations
 
-import datetime
 import sys
 import traceback
 
 from collections.abc import Iterator
 from dataclasses import asdict
 from dataclasses import dataclass
+from datetime import datetime
+from datetime import timezone
 from importlib.util import find_spec
 from pathlib import Path
 from sys import stdout
 from typing import Any
 from typing import Callable
 from typing import Union
 
@@ -138,32 +139,32 @@
         """Wrap and run the collector.
 
         :param args: The positional arguments
         :param kwargs: The keyword arguments
         :returns: The result of the function with elapsed or error information
         """
         global DIAGNOSTIC_FAILURES
-        start = datetime.datetime.now()
+        start = datetime.now(timezone.utc)
         color = args[0].color
         collector = func.__collector__
         collector.start(color=color)
         try:
             result = func(*args, **kwargs)
-            duration = (datetime.datetime.now() - start).total_seconds()
+            duration = (datetime.now(timezone.utc) - start).total_seconds()
             collector.finish(color=color, duration=duration)
         except FailedCollectionError as error:
             # A collector exception, has data
             result = error.errors
-            duration = (datetime.datetime.now() - start).total_seconds()
+            duration = (datetime.now(timezone.utc) - start).total_seconds()
             collector.fail(color=color, duration=duration)
             DIAGNOSTIC_FAILURES += 1
         except Exception as error:  # noqa: BLE001
             # Any other exception, has no data
             result = {"error": str(error) + "\n" + traceback.format_exc()}
-            duration = (datetime.datetime.now() - start).total_seconds()
+            duration = (datetime.now(timezone.utc) - start).total_seconds()
             collector.fail(color=color, duration=duration)
             DIAGNOSTIC_FAILURES += 1
         result["duration"] = round(duration)
         return result
 
     return wrapper
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.6.0/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.6.0/src/ansible_navigator/image_manager/introspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.6.0/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/initialization.py` & `ansible-navigator-3.6.0/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/logger.py` & `ansible-navigator-3.6.0/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.6.0/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/steps.py` & `ansible-navigator-3.6.0/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.6.0/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import copy
 import curses
 import functools
 import json
 import logging
 import re
 
-from importlib.abc import Traversable
 from itertools import chain
 
 from ansible_navigator.tm_tokenize.grammars import Grammars
 from ansible_navigator.tm_tokenize.region import Regions
 from ansible_navigator.tm_tokenize.tokenize import tokenize
+from ansible_navigator.utils.compatibility import Traversable
 
 from .curses_defs import CursesLine
 from .curses_defs import CursesLinePart
 from .curses_defs import CursesLines
 from .curses_defs import RgbTuple
 from .curses_defs import SimpleLinePart
 from .ui_constants import Color
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Object to hold basic UI settings."""
 
 from dataclasses import dataclass
-from importlib.abc import Traversable
+
+from ansible_navigator.utils.compatibility import Traversable
 
 
 @dataclass
 class UIConfig:
     """Object to hold basic UI settings.
 
     Used to determine properties about rendering things. An instance of this
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.6.0/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.6.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.6.0/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.5.0
+Version: 3.6.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
@@ -19,14 +19,15 @@
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ansible-builder>=3.0.0
 Requires-Dist: ansible-runner<3,>=2.3.1
```

### Comparing `ansible-navigator-3.5.0/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.6.0/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.5.0/tox.ini` & `ansible-navigator-3.6.0/tox.ini`

 * *Files identical despite different names*

