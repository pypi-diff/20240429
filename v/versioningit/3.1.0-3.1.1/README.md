# Comparing `tmp/versioningit-3.1.0.tar.gz` & `tmp/versioningit-3.1.1.tar.gz`

## Comparing `versioningit-3.1.0.tar` & `versioningit-3.1.1.tar`

### file list

```diff
@@ -1,288 +1,288 @@
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 versioningit-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 versioningit-3.1.0/tox.ini
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/api.rst
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/changelog.rst
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/command.rst
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/conf.py
--rw-r--r--   0        0        0    32463 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/configuration.rst
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/hatch.rst
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/how.rst
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/index.rst
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/notes.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/runtime-version.rst
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 versioningit-3.1.0/docs/writing-methods.rst
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/__init__.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/__main__.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/basics.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/cmdclass.py
--rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/config.py
--rw-r--r--   0        0        0    23315 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/core.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/errors.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/get_cmdclasses.py
--rw-r--r--   0        0        0    12907 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/git.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/hatch.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/hg.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/hook.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/logging.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/methods.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/next_version.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/onbuild.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/py.typed
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 versioningit-3.1.0/src/versioningit/util.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/conftest.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_config.py
--rw-r--r--   0        0        0    16531 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_end2end.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_get_version.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_logging.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_main.py
--rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_util.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/mypackage-0.1.0.post2+gd338b00.tar.gz
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/custom-methods.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/custom-methods.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/custom-paramless.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/custom-paramless.toml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/empty.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/empty.toml
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/hatch-and-std.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/hatch-and-std.toml
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/hatch.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/hatch.toml
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/other-hatch-and-std.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/other-hatch-and-std.toml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/paramless.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/paramless.toml
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/params.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/params.toml
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/step-args.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config/step-args.toml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-method.toml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-method.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-module-dir.toml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-module-dir.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-module.toml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-module.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-section.toml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-section.txt
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-value.toml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-value.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-ving.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/bad-ving.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-module.toml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-module.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-value.toml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-value.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-ving.toml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/no-ving.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/other-hatch.toml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/config-error/other-hatch.txt
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/distance.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/distance.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/exact.json
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/exact.txt
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/multi-latesttag.json
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/multi-latesttag.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/multi-tag.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/multi-tag.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/null-latesttag.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/hg-archival/null-latesttag.txt
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/desc-in-header.eml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/desc-in-payload.eml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/no-version-payload.eml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/no-version.eml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/version-after-desc.eml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/metadata/version-in-desc.eml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/append-newline.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/append-with-date.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/append.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/latin1-edited.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/line-sepped.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/line2block.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/multi-matches.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/nl-append.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/nomatch.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/not-source.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/replace-nonl.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/replacement.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/set-line.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/source.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/still-empty.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/with-date.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/comment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/empty.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/latin1.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/line-sep.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/no-eof-nl.dat
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/repeats.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/source_file.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/replace-version/base/wheel_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/no-git.zip
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/no-pyproject.zip
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/no-versioningit.txt
--rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/no-versioningit.zip
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/shallow.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/git-archive-distance.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/git-archive-distance.zip
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/git-archive-exact.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/git-archive-exact.zip
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-default-tag.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-default-tag.zip
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-distance.json
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-distance.zip
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-exact.json
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/archives/hg-archive-exact.zip
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/archive-no-tag.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/archive-no-tag.marks
--rw-r--r--   0        0        0    12304 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/archive-no-tag.zip
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/hatch-no-tag.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/hatch-no-tag.marks
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/hatch-no-tag.zip
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/hg-no-tag.json
--rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/hg-no-tag.zip
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/no-tag.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/no-tag.marks
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/no-tag.zip
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/template-fields-error.json
--rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/errors/template-fields-error.zip
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/added-no-commits-default-tag.json
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/added-no-commits-default-tag.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-exclude.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-exclude.marks
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-exclude.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-match.json
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-match.zip
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-mixed-tags.json
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-mixed-tags.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-mixed.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo-mixed.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo.json
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/archive-repo.zip
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-dirty.json
--rw-r--r--   0        0        0    10836 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-dirty.zip
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-distance-dirty.json
--rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-distance-dirty.zip
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-distance.json
--rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-format-distance.zip
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method-pkg.json
--rw-r--r--   0        0        0    12774 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method-pkg.zip
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method-src.json
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method-src.zip
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method.json
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/custom-method.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-tag.fields.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-tag.json
--rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-tag.zip
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version-bad.json
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version-bad.marks
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version-bad.zip
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version-onbuild-write.json
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version-onbuild-write.zip
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version.json
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/default-version.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/detached-exact.fields.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/detached-exact.json
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/detached-exact.zip
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/dirty.json
--rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/dirty.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance-dirty.fields.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance-dirty.json
--rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance-dirty.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance.fields.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance.json
--rw-r--r--   0        0        0    12241 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/distance.zip
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact-annotated.json
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact-annotated.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact.exclude.fields.json
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact.fields.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact.json
--rw-r--r--   0        0        0    10679 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exact.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exclude.fields.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exclude.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exclude.marks
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/exclude.zip
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/match.fields.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/match.json
--rw-r--r--   0        0        0    11208 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/match.zip
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-bases.json
--rw-r--r--   0        0        0    13206 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-bases.zip
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-cfg.json
--rw-r--r--   0        0        0    11657 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-cfg.zip
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-nonidem.json
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-nonidem.zip
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-write.json
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild-write.zip
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild.json
--rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/onbuild.zip
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-encoding.json
--rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-encoding.zip
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-py.json
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-py.zip
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-template.json
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-template.zip
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-txt.json
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/git/write-txt.zip
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/both-config.json
--rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/both-config.zip
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/dirty.json
--rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/dirty.zip
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/distance-dirty.json
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/distance-dirty.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/distance.json
--rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/distance.zip
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/exact.json
--rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/exact.zip
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/hatch-config-empty-std.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/hatch-config-empty-std.zip
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/hatch-config.json
--rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/hatch-config.zip
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/no-std-config.json
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/no-std-config.zip
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild-both-config.json
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild-both-config.zip
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild-fields.json
--rw-r--r--   0        0        0    12087 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild-fields.zip
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild.json
--rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/onbuild.zip
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/std-config.json
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/std-config.zip
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/write-py.json
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/write-py.zip
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/write-txt.json
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hatch/write-txt.zip
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/added-no-commits-default-tag.json
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/added-no-commits-default-tag.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag-fallback.fields.json
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag-fallback.json
--rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag-fallback.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag.fields.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag.json
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/default-tag.zip
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/dirty.json
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/dirty.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance-dirty.fields.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance-dirty.json
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance-dirty.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance.fields.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance.json
--rw-r--r--   0        0        0    12171 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/distance.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/exact.fields.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/exact.json
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/exact.zip
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/multi-tag.json
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/multi-tag.zip
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/pattern.fields.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/pattern.json
--rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/data/repos/hg/pattern.zip
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_format.py
--rw-r--r--   0        0        0    10780 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_git.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_hg.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_next_version.py
--rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_onbuild.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_tag2version.py
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_template_fields.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 versioningit-3.1.0/test/test_methods/test_write.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 versioningit-3.1.0/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 versioningit-3.1.0/LICENSE
--rw-r--r--   0        0        0     7624 2020-02-02 00:00:00.000000 versioningit-3.1.0/README.rst
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 versioningit-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 versioningit-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 versioningit-3.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 versioningit-3.1.1/tox.ini
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/api.rst
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/changelog.rst
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/command.rst
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/conf.py
+-rw-r--r--   0        0        0    32463 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/configuration.rst
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/hatch.rst
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/how.rst
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/index.rst
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/notes.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/runtime-version.rst
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 versioningit-3.1.1/docs/writing-methods.rst
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/__init__.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/__main__.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/basics.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/cmdclass.py
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/config.py
+-rw-r--r--   0        0        0    23315 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/core.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/errors.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/get_cmdclasses.py
+-rw-r--r--   0        0        0    12907 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/git.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/hatch.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/hg.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/hook.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/logging.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/methods.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/next_version.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/onbuild.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/py.typed
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 versioningit-3.1.1/src/versioningit/util.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/conftest.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_config.py
+-rw-r--r--   0        0        0    17311 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_end2end.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_get_version.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_logging.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_main.py
+-rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_util.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/mypackage-0.1.0.post2+gd338b00.tar.gz
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/custom-methods.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/custom-methods.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/custom-paramless.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/custom-paramless.toml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/empty.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/empty.toml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/hatch-and-std.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/hatch-and-std.toml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/hatch.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/hatch.toml
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/other-hatch-and-std.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/other-hatch-and-std.toml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/paramless.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/paramless.toml
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/params.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/params.toml
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/step-args.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config/step-args.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-method.toml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-method.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-module-dir.toml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-module-dir.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-module.toml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-module.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-section.toml
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-section.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-value.toml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-value.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-ving.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/bad-ving.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-module.toml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-module.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-value.toml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-value.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-ving.toml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/no-ving.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/other-hatch.toml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/config-error/other-hatch.txt
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/distance.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/distance.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/exact.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/exact.txt
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/multi-latesttag.json
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/multi-latesttag.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/multi-tag.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/multi-tag.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/null-latesttag.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/hg-archival/null-latesttag.txt
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/desc-in-header.eml
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/desc-in-payload.eml
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/no-version-payload.eml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/no-version.eml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/version-after-desc.eml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/metadata/version-in-desc.eml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/append-newline.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/append-with-date.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/append.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/latin1-edited.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/line-sepped.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/line2block.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/multi-matches.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/nl-append.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/nomatch.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/not-source.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/replace-nonl.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/replacement.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/set-line.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/source.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/still-empty.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/with-date.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/comment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/empty.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/latin1.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/line-sep.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/no-eof-nl.dat
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/repeats.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/source_file.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/replace-version/base/wheel_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/no-git.zip
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/no-pyproject.zip
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/no-versioningit.txt
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/no-versioningit.zip
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/shallow.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/git-archive-distance.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/git-archive-distance.zip
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/git-archive-exact.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/git-archive-exact.zip
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-default-tag.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-default-tag.zip
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-distance.json
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-distance.zip
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-exact.json
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/archives/hg-archive-exact.zip
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/added-no-commits-default-tag.json
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/added-no-commits-default-tag.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-exclude.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-exclude.marks
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-exclude.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-match.json
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-match.zip
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-mixed-tags.json
+-rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-mixed-tags.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-mixed.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo-mixed.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo.json
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/archive-repo.zip
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-dirty.json
+-rw-r--r--   0        0        0    10836 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-dirty.zip
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-distance-dirty.json
+-rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-distance-dirty.zip
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-distance.json
+-rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-format-distance.zip
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method-pkg.json
+-rw-r--r--   0        0        0    12774 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method-pkg.zip
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method-src.json
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method-src.zip
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method.json
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/custom-method.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-tag.fields.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-tag.json
+-rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-tag.zip
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version-bad.json
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version-bad.marks
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version-bad.zip
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version-onbuild-write.json
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version-onbuild-write.zip
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version.json
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/default-version.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/detached-exact.fields.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/detached-exact.json
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/detached-exact.zip
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/dirty.json
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/dirty.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance-dirty.fields.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance-dirty.json
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance-dirty.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance.fields.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance.json
+-rw-r--r--   0        0        0    12241 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/distance.zip
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact-annotated.json
+-rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact-annotated.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact.exclude.fields.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact.fields.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact.json
+-rw-r--r--   0        0        0    10679 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exact.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exclude.fields.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exclude.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exclude.marks
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/exclude.zip
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/match.fields.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/match.json
+-rw-r--r--   0        0        0    11208 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/match.zip
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-bases.json
+-rw-r--r--   0        0        0    13206 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-bases.zip
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-cfg.json
+-rw-r--r--   0        0        0    11657 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-cfg.zip
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-nonidem.json
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-nonidem.zip
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-write.json
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild-write.zip
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild.json
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/onbuild.zip
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-encoding.json
+-rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-encoding.zip
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-py.json
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-py.zip
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-template.json
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-template.zip
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-txt.json
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git/write-txt.zip
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/archive-no-tag.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/archive-no-tag.marks
+-rw-r--r--   0        0        0    12304 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/archive-no-tag.zip
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/hatch-no-tag.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/hatch-no-tag.marks
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/hatch-no-tag.zip
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/no-tag.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/no-tag.marks
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/no-tag.zip
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/template-fields-error.json
+-rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/git-errors/template-fields-error.zip
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/both-config.json
+-rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/both-config.zip
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/dirty.json
+-rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/dirty.zip
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/distance-dirty.json
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/distance-dirty.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/distance.json
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/distance.zip
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/exact.json
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/exact.zip
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/hatch-config-empty-std.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/hatch-config-empty-std.zip
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/hatch-config.json
+-rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/hatch-config.zip
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/no-std-config.json
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/no-std-config.zip
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild-both-config.json
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild-both-config.zip
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild-fields.json
+-rw-r--r--   0        0        0    12087 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild-fields.zip
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild.json
+-rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/onbuild.zip
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/std-config.json
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/std-config.zip
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/write-py.json
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/write-py.zip
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/write-txt.json
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hatch/write-txt.zip
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/added-no-commits-default-tag.json
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/added-no-commits-default-tag.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag-fallback.fields.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag-fallback.json
+-rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag-fallback.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag.fields.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag.json
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/default-tag.zip
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/dirty.json
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/dirty.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance-dirty.fields.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance-dirty.json
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance-dirty.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance.fields.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance.json
+-rw-r--r--   0        0        0    12171 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/distance.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/exact.fields.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/exact.json
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/exact.zip
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/multi-tag.json
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/multi-tag.zip
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/pattern.fields.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/pattern.json
+-rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg/pattern.zip
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg-errors/hg-no-tag.json
+-rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/data/repos/hg-errors/hg-no-tag.zip
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_format.py
+-rw-r--r--   0        0        0    10780 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_git.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_hg.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_next_version.py
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_onbuild.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_tag2version.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_template_fields.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 versioningit-3.1.1/test/test_methods/test_write.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 versioningit-3.1.1/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 versioningit-3.1.1/LICENSE
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 versioningit-3.1.1/README.rst
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 versioningit-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 versioningit-3.1.1/PKG-INFO
```

### Comparing `versioningit-3.1.0/CHANGELOG.md` & `versioningit-3.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v3.1.1 (2024-04-29)
+-------------------
+- Correctly mark a certain test as requiring Mercurial
+
 v3.1.0 (2024-03-16)
 -------------------
 - When `git describe` fails to retrieve a tag, the resulting log/error message
   now includes all options passed to the command (based on contribution by
   [@jenshnielsen](https://github.com/jenshnielsen))
 - When `hg log` fails to retrieve a tag, the resulting log/error message now
   includes the tag pattern passed to `latesttag()`, if any
```

### Comparing `versioningit-3.1.0/tox.ini` & `versioningit-3.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/api.rst` & `versioningit-3.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/changelog.rst` & `versioningit-3.1.1/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. currentmodule:: versioningit
 
 Changelog
 =========
 
+v3.1.1 (2024-04-29)
+-------------------
+- Correctly mark a certain test as requiring Mercurial
+
+
 v3.1.0 (2024-03-16)
 -------------------
 - When :command:`git describe` fails to retrieve a tag, the resulting log/error
   message now includes all options passed to the command (based on contribution
   by `@jenshnielsen <https://github.com/jenshnielsen>`_)
 - When :command:`hg log` fails to retrieve a tag, the resulting log/error
   message now includes the tag pattern passed to ``latesttag()``, if any
```

### Comparing `versioningit-3.1.0/docs/command.rst` & `versioningit-3.1.1/docs/command.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/conf.py` & `versioningit-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/configuration.rst` & `versioningit-3.1.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/hatch.rst` & `versioningit-3.1.1/docs/hatch.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/how.rst` & `versioningit-3.1.1/docs/how.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/index.rst` & `versioningit-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/notes.rst` & `versioningit-3.1.1/docs/notes.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/runtime-version.rst` & `versioningit-3.1.1/docs/runtime-version.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/docs/writing-methods.rst` & `versioningit-3.1.1/docs/writing-methods.rst`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/__init__.py` & `versioningit-3.1.1/src/versioningit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   Git repository, especially not without a way to turn it off, because that
   would just be rude.
 
 Visit <https://github.com/jwodder/versioningit> or
 <https://versioningit.rtfd.io> for more information.
 """
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "versioningit@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/versioningit"
 
 from .core import (
     FallbackReport,
```

### Comparing `versioningit-3.1.0/src/versioningit/__main__.py` & `versioningit-3.1.1/src/versioningit/__main__.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/basics.py` & `versioningit-3.1.1/src/versioningit/basics.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/config.py` & `versioningit-3.1.1/src/versioningit/config.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/core.py` & `versioningit-3.1.1/src/versioningit/core.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/errors.py` & `versioningit-3.1.1/src/versioningit/errors.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/get_cmdclasses.py` & `versioningit-3.1.1/src/versioningit/get_cmdclasses.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/git.py` & `versioningit-3.1.1/src/versioningit/git.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/hatch.py` & `versioningit-3.1.1/src/versioningit/hatch.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/hg.py` & `versioningit-3.1.1/src/versioningit/hg.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/hook.py` & `versioningit-3.1.1/src/versioningit/hook.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/logging.py` & `versioningit-3.1.1/src/versioningit/logging.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/methods.py` & `versioningit-3.1.1/src/versioningit/methods.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/next_version.py` & `versioningit-3.1.1/src/versioningit/next_version.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/onbuild.py` & `versioningit-3.1.1/src/versioningit/onbuild.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/src/versioningit/util.py` & `versioningit-3.1.1/src/versioningit/util.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/conftest.py` & `versioningit-3.1.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_config.py` & `versioningit-3.1.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_end2end.py` & `versioningit-3.1.1/test/test_end2end.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,17 +236,40 @@
     assert (
         get_version(project_dir=tmp_path, config={}, write=False, fallback=True)
         == version
     )
 
 
 @pytest.mark.parametrize(
-    "repozip,details", mkcases("errors", [needs_git], details_cls=ErrorDetails)
+    "repozip,details", mkcases("git-errors", [needs_git], details_cls=ErrorDetails)
 )
-def test_end2end_error(tmp_path: Path, repozip: Path, details: ErrorDetails) -> None:
+def test_end2end_git_error(
+    tmp_path: Path, repozip: Path, details: ErrorDetails
+) -> None:
+    shutil.unpack_archive(repozip, tmp_path)
+    with pytest.raises(Error) as excinfo:
+        get_version(project_dir=tmp_path, write=False, fallback=True)
+    assert type(excinfo.value).__name__ == details.type
+    assert str(excinfo.value) == details.message
+    r = subprocess.run(
+        [sys.executable, "-m", "build", "--no-isolation", str(tmp_path)],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        text=True,
+    )
+    assert r.returncode != 0
+    out = r.stdout
+    assert isinstance(out, str)
+    assert details.message in out
+
+
+@pytest.mark.parametrize(
+    "repozip,details", mkcases("hg-errors", [needs_hg], details_cls=ErrorDetails)
+)
+def test_end2end_hg_error(tmp_path: Path, repozip: Path, details: ErrorDetails) -> None:
     shutil.unpack_archive(repozip, tmp_path)
     with pytest.raises(Error) as excinfo:
         get_version(project_dir=tmp_path, write=False, fallback=True)
     assert type(excinfo.value).__name__ == details.type
     assert str(excinfo.value) == details.message
     r = subprocess.run(
         [sys.executable, "-m", "build", "--no-isolation", str(tmp_path)],
```

### Comparing `versioningit-3.1.0/test/test_get_version.py` & `versioningit-3.1.1/test/test_get_version.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_logging.py` & `versioningit-3.1.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_main.py` & `versioningit-3.1.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_util.py` & `versioningit-3.1.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/mypackage-0.1.0.post2+gd338b00.tar.gz` & `versioningit-3.1.1/test/data/mypackage-0.1.0.post2+gd338b00.tar.gz`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/custom-methods.py` & `versioningit-3.1.1/test/data/config/custom-methods.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/custom-paramless.py` & `versioningit-3.1.1/test/data/config/custom-paramless.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/empty.py` & `versioningit-3.1.1/test/data/config/empty.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/hatch-and-std.py` & `versioningit-3.1.1/test/data/config/hatch-and-std.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/hatch.py` & `versioningit-3.1.1/test/data/config/hatch.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/other-hatch-and-std.py` & `versioningit-3.1.1/test/data/config/other-hatch-and-std.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/paramless.py` & `versioningit-3.1.1/test/data/config/paramless.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/params.py` & `versioningit-3.1.1/test/data/config/params.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/params.toml` & `versioningit-3.1.1/test/data/config/params.toml`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/step-args.py` & `versioningit-3.1.1/test/data/config/step-args.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/config/step-args.toml` & `versioningit-3.1.1/test/data/config/step-args.toml`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/no-git.zip` & `versioningit-3.1.1/test/data/repos/no-git.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/no-pyproject.zip` & `versioningit-3.1.1/test/data/repos/no-pyproject.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/no-versioningit.zip` & `versioningit-3.1.1/test/data/repos/no-versioningit.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/shallow.zip` & `versioningit-3.1.1/test/data/repos/shallow.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/archives/git-archive-distance.zip` & `versioningit-3.1.1/test/data/repos/archives/git-archive-distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/archives/git-archive-exact.zip` & `versioningit-3.1.1/test/data/repos/archives/git-archive-exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/archives/hg-archive-default-tag.zip` & `versioningit-3.1.1/test/data/repos/archives/hg-archive-default-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/archives/hg-archive-distance.zip` & `versioningit-3.1.1/test/data/repos/archives/hg-archive-distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/archives/hg-archive-exact.zip` & `versioningit-3.1.1/test/data/repos/archives/hg-archive-exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/errors/archive-no-tag.zip` & `versioningit-3.1.1/test/data/repos/git-errors/archive-no-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/errors/hatch-no-tag.zip` & `versioningit-3.1.1/test/data/repos/git-errors/hatch-no-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/errors/hg-no-tag.zip` & `versioningit-3.1.1/test/data/repos/hg-errors/hg-no-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/errors/no-tag.zip` & `versioningit-3.1.1/test/data/repos/git-errors/no-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/errors/template-fields-error.zip` & `versioningit-3.1.1/test/data/repos/git-errors/template-fields-error.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/added-no-commits-default-tag.zip` & `versioningit-3.1.1/test/data/repos/git/added-no-commits-default-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/archive-repo-exclude.zip` & `versioningit-3.1.1/test/data/repos/git/archive-repo-exclude.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/archive-repo-match.zip` & `versioningit-3.1.1/test/data/repos/git/archive-repo-match.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/archive-repo-mixed-tags.zip` & `versioningit-3.1.1/test/data/repos/git/archive-repo-mixed-tags.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/archive-repo-mixed.zip` & `versioningit-3.1.1/test/data/repos/git/archive-repo-mixed.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/archive-repo.zip` & `versioningit-3.1.1/test/data/repos/git/archive-repo.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-format-dirty.zip` & `versioningit-3.1.1/test/data/repos/git/custom-format-dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-format-distance-dirty.zip` & `versioningit-3.1.1/test/data/repos/git/custom-format-distance-dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-format-distance.zip` & `versioningit-3.1.1/test/data/repos/git/custom-format-distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-method-pkg.zip` & `versioningit-3.1.1/test/data/repos/git/custom-method-pkg.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-method-src.zip` & `versioningit-3.1.1/test/data/repos/git/custom-method-src.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/custom-method.zip` & `versioningit-3.1.1/test/data/repos/git/custom-method.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-tag.zip` & `versioningit-3.1.1/test/data/repos/git/default-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-version-bad.json` & `versioningit-3.1.1/test/data/repos/git/default-version-bad.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-version-bad.zip` & `versioningit-3.1.1/test/data/repos/git/default-version-bad.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-version-onbuild-write.json` & `versioningit-3.1.1/test/data/repos/git/default-version-onbuild-write.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-version-onbuild-write.zip` & `versioningit-3.1.1/test/data/repos/git/default-version-onbuild-write.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/default-version.zip` & `versioningit-3.1.1/test/data/repos/git/default-version.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/detached-exact.zip` & `versioningit-3.1.1/test/data/repos/git/detached-exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/dirty.zip` & `versioningit-3.1.1/test/data/repos/git/dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/distance-dirty.zip` & `versioningit-3.1.1/test/data/repos/git/distance-dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/distance.zip` & `versioningit-3.1.1/test/data/repos/git/distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/exact-annotated.zip` & `versioningit-3.1.1/test/data/repos/git/exact-annotated.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/exact.zip` & `versioningit-3.1.1/test/data/repos/git/exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/exclude.zip` & `versioningit-3.1.1/test/data/repos/git/exclude.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/match.zip` & `versioningit-3.1.1/test/data/repos/git/match.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-bases.json` & `versioningit-3.1.1/test/data/repos/git/onbuild-bases.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-bases.zip` & `versioningit-3.1.1/test/data/repos/git/onbuild-bases.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-cfg.zip` & `versioningit-3.1.1/test/data/repos/git/onbuild-cfg.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-nonidem.zip` & `versioningit-3.1.1/test/data/repos/git/onbuild-nonidem.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-write.json` & `versioningit-3.1.1/test/data/repos/git/onbuild-write.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild-write.zip` & `versioningit-3.1.1/test/data/repos/git/onbuild-write.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/onbuild.zip` & `versioningit-3.1.1/test/data/repos/git/onbuild.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/write-encoding.zip` & `versioningit-3.1.1/test/data/repos/git/write-encoding.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/write-py.zip` & `versioningit-3.1.1/test/data/repos/git/write-py.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/write-template.zip` & `versioningit-3.1.1/test/data/repos/git/write-template.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/git/write-txt.zip` & `versioningit-3.1.1/test/data/repos/git/write-txt.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/both-config.zip` & `versioningit-3.1.1/test/data/repos/hatch/both-config.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/dirty.zip` & `versioningit-3.1.1/test/data/repos/hatch/dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/distance-dirty.zip` & `versioningit-3.1.1/test/data/repos/hatch/distance-dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/distance.zip` & `versioningit-3.1.1/test/data/repos/hatch/distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/exact.zip` & `versioningit-3.1.1/test/data/repos/hatch/exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/hatch-config-empty-std.zip` & `versioningit-3.1.1/test/data/repos/hatch/hatch-config-empty-std.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/hatch-config.zip` & `versioningit-3.1.1/test/data/repos/hatch/hatch-config.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/no-std-config.zip` & `versioningit-3.1.1/test/data/repos/hatch/no-std-config.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/onbuild-both-config.json` & `versioningit-3.1.1/test/data/repos/hatch/onbuild-both-config.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/onbuild-both-config.zip` & `versioningit-3.1.1/test/data/repos/hatch/onbuild-both-config.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/onbuild-fields.json` & `versioningit-3.1.1/test/data/repos/hatch/onbuild-fields.json`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/onbuild-fields.zip` & `versioningit-3.1.1/test/data/repos/hatch/onbuild-fields.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/onbuild.zip` & `versioningit-3.1.1/test/data/repos/hatch/onbuild.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/std-config.zip` & `versioningit-3.1.1/test/data/repos/hatch/std-config.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/write-py.zip` & `versioningit-3.1.1/test/data/repos/hatch/write-py.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hatch/write-txt.zip` & `versioningit-3.1.1/test/data/repos/hatch/write-txt.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/added-no-commits-default-tag.zip` & `versioningit-3.1.1/test/data/repos/hg/added-no-commits-default-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/default-tag-fallback.zip` & `versioningit-3.1.1/test/data/repos/hg/default-tag-fallback.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/default-tag.zip` & `versioningit-3.1.1/test/data/repos/hg/default-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/dirty.zip` & `versioningit-3.1.1/test/data/repos/hg/dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/distance-dirty.zip` & `versioningit-3.1.1/test/data/repos/hg/distance-dirty.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/distance.zip` & `versioningit-3.1.1/test/data/repos/hg/distance.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/exact.zip` & `versioningit-3.1.1/test/data/repos/hg/exact.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/multi-tag.zip` & `versioningit-3.1.1/test/data/repos/hg/multi-tag.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/data/repos/hg/pattern.zip` & `versioningit-3.1.1/test/data/repos/hg/pattern.zip`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_format.py` & `versioningit-3.1.1/test/test_methods/test_format.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_git.py` & `versioningit-3.1.1/test/test_methods/test_git.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_hg.py` & `versioningit-3.1.1/test/test_methods/test_hg.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_next_version.py` & `versioningit-3.1.1/test/test_methods/test_next_version.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_onbuild.py` & `versioningit-3.1.1/test/test_methods/test_onbuild.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_tag2version.py` & `versioningit-3.1.1/test/test_methods/test_tag2version.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_template_fields.py` & `versioningit-3.1.1/test/test_methods/test_template_fields.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/test/test_methods/test_write.py` & `versioningit-3.1.1/test/test_methods/test_write.py`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/LICENSE` & `versioningit-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/README.rst` & `versioningit-3.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-.. image:: https://www.repostatus.org/badges/latest/active.svg
+|repostatus| |ci-status| |coverage| |pyversions| |conda| |license|
+
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
     :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/versioningit/actions/workflows/test.yml/badge.svg
+.. |ci-status| image:: https://github.com/jwodder/versioningit/actions/workflows/test.yml/badge.svg
     :target: https://github.com/jwodder/versioningit/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/versioningit/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/versioningit/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/versioningit
 
-.. image:: https://img.shields.io/pypi/pyversions/versioningit.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/versioningit.svg
     :target: https://pypi.org/project/versioningit/
 
-.. image:: https://img.shields.io/conda/vn/conda-forge/versioningit.svg
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/versioningit.svg
     :target: https://anaconda.org/conda-forge/versioningit
     :alt: Conda Version
 
-.. image:: https://img.shields.io/github/license/jwodder/versioningit.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/versioningit.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/versioningit>`_
 | `PyPI <https://pypi.org/project/versioningit/>`_
 | `Documentation <https://versioningit.readthedocs.io>`_
 | `Issues <https://github.com/jwodder/versioningit/issues>`_
```

### Comparing `versioningit-3.1.0/pyproject.toml` & `versioningit-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `versioningit-3.1.0/PKG-INFO` & `versioningit-3.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: versioningit
-Version: 3.1.0
+Version: 3.1.1
 Summary: Versioning It with your Version In Git
 Project-URL: Source Code, https://github.com/jwodder/versioningit
 Project-URL: Bug Tracker, https://github.com/jwodder/versioningit/issues
 Project-URL: Documentation, https://versioningit.readthedocs.io
 Author-email: John Thorvald Wodder II <versioningit@varonathe.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -31,34 +31,36 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: packaging>=17.1
 Requires-Dist: tomli<3.0,>=1.2; python_version < '3.11'
 Description-Content-Type: text/x-rst
 
-.. image:: https://www.repostatus.org/badges/latest/active.svg
+|repostatus| |ci-status| |coverage| |pyversions| |conda| |license|
+
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
     :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/versioningit/actions/workflows/test.yml/badge.svg
+.. |ci-status| image:: https://github.com/jwodder/versioningit/actions/workflows/test.yml/badge.svg
     :target: https://github.com/jwodder/versioningit/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/versioningit/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/versioningit/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/versioningit
 
-.. image:: https://img.shields.io/pypi/pyversions/versioningit.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/versioningit.svg
     :target: https://pypi.org/project/versioningit/
 
-.. image:: https://img.shields.io/conda/vn/conda-forge/versioningit.svg
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/versioningit.svg
     :target: https://anaconda.org/conda-forge/versioningit
     :alt: Conda Version
 
-.. image:: https://img.shields.io/github/license/jwodder/versioningit.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/versioningit.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/versioningit>`_
 | `PyPI <https://pypi.org/project/versioningit/>`_
 | `Documentation <https://versioningit.readthedocs.io>`_
 | `Issues <https://github.com/jwodder/versioningit/issues>`_
```

