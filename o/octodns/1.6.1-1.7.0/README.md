# Comparing `tmp/octodns-1.6.1.tar.gz` & `tmp/octodns-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-1.6.1.tar", last modified: Sun Mar 17 19:47:36 2024, max compression
+gzip compressed data, was "octodns-1.7.0.tar", last modified: Mon Apr 29 21:46:52 2024, max compression
```

## Comparing `octodns-1.6.1.tar` & `octodns-1.7.0.tar`

### file list

```diff
@@ -1,267 +1,268 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.268018 octodns-1.6.1/
--rw-r--r--   0 ross       (501) staff       (20)    35246 2024-03-17 19:47:19.000000 octodns-1.6.1/CHANGELOG.md
--rw-r--r--   0 ross       (501) staff       (20)     3229 2024-03-17 19:47:19.000000 octodns-1.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 ross       (501) staff       (20)     3761 2024-03-17 19:47:19.000000 octodns-1.6.1/CONTRIBUTING.md
--rw-r--r--   0 ross       (501) staff       (20)     1129 2024-03-17 19:47:19.000000 octodns-1.6.1/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      292 2024-03-17 19:47:19.000000 octodns-1.6.1/MANIFEST.in
--rw-r--r--   0 ross       (501) staff       (20)    32485 2024-03-17 19:47:36.267536 octodns-1.6.1/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)    31501 2024-03-17 19:47:19.000000 octodns-1.6.1/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.190266 octodns-1.6.1/docs/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.191266 octodns-1.6.1/docs/assets/
--rw-r--r--   0 ross       (501) staff       (20)    82371 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/assets/deploy.png
--rw-r--r--   0 ross       (501) staff       (20)    75814 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/assets/noop.png
--rw-r--r--   0 ross       (501) staff       (20)   212872 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/assets/pr.png
--rw-r--r--   0 ross       (501) staff       (20)     3481 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/auto_arpa.md
--rw-r--r--   0 ross       (501) staff       (20)     7665 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/dynamic_records.md
--rw-r--r--   0 ross       (501) staff       (20)     3427 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/geo_records.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.191832 octodns-1.6.1/docs/logos/
--rw-r--r--   0 ross       (501) staff       (20)     3983 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/logos/octodns-logo.png
--rw-r--r--   0 ross       (501) staff       (20)     7726 2024-03-17 19:47:19.000000 octodns-1.6.1/docs/records.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.195630 octodns-1.6.1/octodns/
--rw-r--r--   0 ross       (501) staff       (20)      144 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.199772 octodns-1.6.1/octodns/cmds/
--rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     3554 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/args.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1423 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/compare.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1624 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/dump.py
--rwxr-xr-x   0 ross       (501) staff       (20)     3554 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/report.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1812 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/sync.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1049 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/validate.py
--rwxr-xr-x   0 ross       (501) staff       (20)      444 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/cmds/versions.py
--rw-r--r--   0 ross       (501) staff       (20)      641 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/context.py
--rw-r--r--   0 ross       (501) staff       (20)      135 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/deprecation.py
--rw-r--r--   0 ross       (501) staff       (20)      717 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/equality.py
--rw-r--r--   0 ross       (501) staff       (20)     2373 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/idna.py
--rw-r--r--   0 ross       (501) staff       (20)    39419 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/manager.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.203102 octodns-1.6.1/octodns/processor/
--rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     1824 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/acme.py
--rw-r--r--   0 ross       (501) staff       (20)     2334 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/arpa.py
--rw-r--r--   0 ross       (501) staff       (20)     4502 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/base.py
--rw-r--r--   0 ross       (501) staff       (20)    14464 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/filter.py
--rw-r--r--   0 ross       (501) staff       (20)     4999 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/meta.py
--rw-r--r--   0 ross       (501) staff       (20)     3836 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/ownership.py
--rw-r--r--   0 ross       (501) staff       (20)     2260 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/restrict.py
--rw-r--r--   0 ross       (501) staff       (20)     4010 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/spf.py
--rw-r--r--   0 ross       (501) staff       (20)     1493 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/processor/trailing_dots.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.204819 octodns-1.6.1/octodns/provider/
--rw-r--r--   0 ross       (501) staff       (20)      108 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/provider/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    12523 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/provider/base.py
--rw-r--r--   0 ross       (501) staff       (20)    11312 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/provider/plan.py
--rw-r--r--   0 ross       (501) staff       (20)    15812 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/provider/yaml.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.215079 octodns-1.6.1/octodns/record/
--rw-r--r--   0 ross       (501) staff       (20)     1471 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)      412 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/a.py
--rw-r--r--   0 ross       (501) staff       (20)      423 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/aaaa.py
--rw-r--r--   0 ross       (501) staff       (20)      488 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/alias.py
--rw-r--r--   0 ross       (501) staff       (20)    12299 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/base.py
--rw-r--r--   0 ross       (501) staff       (20)     2334 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/caa.py
--rw-r--r--   0 ross       (501) staff       (20)     1769 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/change.py
--rw-r--r--   0 ross       (501) staff       (20)     1750 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/chunked.py
--rw-r--r--   0 ross       (501) staff       (20)      534 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/cname.py
--rw-r--r--   0 ross       (501) staff       (20)      296 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/dname.py
--rw-r--r--   0 ross       (501) staff       (20)     5636 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/ds.py
--rw-r--r--   0 ross       (501) staff       (20)    15354 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/dynamic.py
--rw-r--r--   0 ross       (501) staff       (20)      611 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/exception.py
--rw-r--r--   0 ross       (501) staff       (20)     5531 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/geo.py
--rw-r--r--   0 ross       (501) staff       (20)    13426 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/geo_data.py
--rw-r--r--   0 ross       (501) staff       (20)     1385 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/ip.py
--rw-r--r--   0 ross       (501) staff       (20)    10692 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/loc.py
--rw-r--r--   0 ross       (501) staff       (20)     3299 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/mx.py
--rw-r--r--   0 ross       (501) staff       (20)     4458 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/naptr.py
--rw-r--r--   0 ross       (501) staff       (20)      235 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/ns.py
--rw-r--r--   0 ross       (501) staff       (20)      412 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/ptr.py
--rw-r--r--   0 ross       (501) staff       (20)      644 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/rr.py
--rw-r--r--   0 ross       (501) staff       (20)      512 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/spf.py
--rw-r--r--   0 ross       (501) staff       (20)     4305 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/srv.py
--rw-r--r--   0 ross       (501) staff       (20)     3468 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/sshfp.py
--rw-r--r--   0 ross       (501) staff       (20)      465 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/subnet.py
--rw-r--r--   0 ross       (501) staff       (20)     1951 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/target.py
--rw-r--r--   0 ross       (501) staff       (20)     4998 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/tlsa.py
--rw-r--r--   0 ross       (501) staff       (20)      257 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/txt.py
--rw-r--r--   0 ross       (501) staff       (20)     4048 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/record/urlfwd.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.216236 octodns-1.6.1/octodns/secret/
--rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/secret/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)      180 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/secret/base.py
--rw-r--r--   0 ross       (501) staff       (20)      861 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/secret/environ.py
--rw-r--r--   0 ross       (501) staff       (20)       52 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/secret/exception.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.217512 octodns-1.6.1/octodns/source/
--rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/source/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     1712 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/source/base.py
--rw-r--r--   0 ross       (501) staff       (20)     3280 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/source/envvar.py
--rwxr-xr-x   0 ross       (501) staff       (20)    15823 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/source/tinydns.py
--rw-r--r--   0 ross       (501) staff       (20)     3053 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    12776 2024-03-17 19:47:19.000000 octodns-1.6.1/octodns/zone.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.265686 octodns-1.6.1/octodns.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)    32485 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     7368 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      272 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/entry_points.txt
--rw-r--r--   0 ross       (501) staff       (20)      300 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)        8 2024-03-17 19:47:36.000000 octodns-1.6.1/octodns.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      275 2024-03-17 19:47:19.000000 octodns-1.6.1/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)      916 2024-03-17 19:47:19.000000 octodns-1.6.1/requirements-dev.txt
--rw-r--r--   0 ross       (501) staff       (20)      181 2024-03-17 19:47:19.000000 octodns-1.6.1/requirements.txt
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.221379 octodns-1.6.1/script/
--rwxr-xr-x   0 ross       (501) staff       (20)     1273 2024-03-17 19:47:19.000000 octodns-1.6.1/script/bootstrap
--rwxr-xr-x   0 ross       (501) staff       (20)      177 2024-03-17 19:47:19.000000 octodns-1.6.1/script/changelog
--rwxr-xr-x   0 ross       (501) staff       (20)     1115 2024-03-17 19:47:19.000000 octodns-1.6.1/script/cibuild
--rwxr-xr-x   0 ross       (501) staff       (20)     1728 2024-03-17 19:47:19.000000 octodns-1.6.1/script/cibuild-module
--rwxr-xr-x   0 ross       (501) staff       (20)      819 2024-03-17 19:47:19.000000 octodns-1.6.1/script/cibuild-setup-py
--rwxr-xr-x   0 ross       (501) staff       (20)      998 2024-03-17 19:47:19.000000 octodns-1.6.1/script/coverage
--rwxr-xr-x   0 ross       (501) staff       (20)      184 2024-03-17 19:47:19.000000 octodns-1.6.1/script/format
--rwxr-xr-x   0 ross       (501) staff       (20)     2486 2024-03-17 19:47:19.000000 octodns-1.6.1/script/generate-geo-data
--rwxr-xr-x   0 ross       (501) staff       (20)      387 2024-03-17 19:47:19.000000 octodns-1.6.1/script/lint
--rwxr-xr-x   0 ross       (501) staff       (20)      772 2024-03-17 19:47:19.000000 octodns-1.6.1/script/markdown-toc
--rwxr-xr-x   0 ross       (501) staff       (20)     1278 2024-03-17 19:47:19.000000 octodns-1.6.1/script/release
--rwxr-xr-x   0 ross       (501) staff       (20)      662 2024-03-17 19:47:19.000000 octodns-1.6.1/script/test
--rwxr-xr-x   0 ross       (501) staff       (20)     1940 2024-03-17 19:47:19.000000 octodns-1.6.1/script/update-requirements
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-03-17 19:47:36.268125 octodns-1.6.1/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     2781 2024-03-17 19:47:19.000000 octodns-1.6.1/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.237172 octodns-1.6.1/tests/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.248563 octodns-1.6.1/tests/config/
--rw-r--r--   0 ross       (501) staff       (20)      363 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/alias-zone-loop.yaml
--rw-r--r--   0 ross       (501) staff       (20)      447 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/always-dry-run.yaml
--rw-r--r--   0 ross       (501) staff       (20)      129 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/bad-plan-output-config.yaml
--rw-r--r--   0 ross       (501) staff       (20)       63 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/bad-plan-output-missing-class.yaml
--rw-r--r--   0 ross       (501) staff       (20)       81 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/bad-provider-class-module.yaml
--rw-r--r--   0 ross       (501) staff       (20)       59 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/bad-provider-class-no-module.yaml
--rw-r--r--   0 ross       (501) staff       (20)       67 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/bad-provider-class.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.249413 octodns-1.6.1/tests/config/dynamic-arpa/
--rw-r--r--   0 ross       (501) staff       (20)        0 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-arpa/3.2.2.in-addr.arpa.yaml
--rw-r--r--   0 ross       (501) staff       (20)        0 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-arpa/b.e.f.f.f.d.1.8.f.2.6.0.1.2.e.0.0.5.0.4.4.6.0.1.0.6.2.ip6.arpa.yaml
--rw-r--r--   0 ross       (501) staff       (20)      226 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-arpa/unit.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)      543 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-arpa-no-normal-source.yaml
--rw-r--r--   0 ross       (501) staff       (20)      552 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-arpa.yaml
--rw-r--r--   0 ross       (501) staff       (20)      303 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-config-no-list-zones.yaml
--rw-r--r--   0 ross       (501) staff       (20)      460 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic-config.yaml
--rw-r--r--   0 ross       (501) staff       (20)     4749 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/dynamic.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)        4 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/empty.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.249840 octodns-1.6.1/tests/config/hybrid/
--rw-r--r--   0 ross       (501) staff       (20)       66 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/hybrid/one.test.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.250582 octodns-1.6.1/tests/config/hybrid/two.test./
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/hybrid/two.test./$two.test.yaml
--rw-r--r--   0 ross       (501) staff       (20)       58 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/hybrid/two.test./split-zone-file.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.252514 octodns-1.6.1/tests/config/include/
--rw-r--r--   0 ross       (501) staff       (20)       24 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/array.yaml
--rw-r--r--   0 ross       (501) staff       (20)       15 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/dict.yaml
--rw-r--r--   0 ross       (501) staff       (20)        4 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/empty.yaml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/include-doesnt-exist.yaml
--rw-r--r--   0 ross       (501) staff       (20)      214 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/main.yaml
--rw-r--r--   0 ross       (501) staff       (20)       31 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/nested.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.252858 octodns-1.6.1/tests/config/include/subdir/
--rw-r--r--   0 ross       (501) staff       (20)       17 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/include/subdir/value.yaml
--rw-r--r--   0 ross       (501) staff       (20)       32 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/missing-provider-class.yaml
--rw-r--r--   0 ross       (501) staff       (20)       75 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/missing-provider-config.yaml
--rw-r--r--   0 ross       (501) staff       (20)      121 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/missing-provider-env.yaml
--rw-r--r--   0 ross       (501) staff       (20)       44 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/missing-sources.yaml
--rw-r--r--   0 ross       (501) staff       (20)      235 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/no-dump.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.253139 octodns-1.6.1/tests/config/override/
--rw-r--r--   0 ross       (501) staff       (20)      167 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/override/dynamic.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)      115 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/plan-output-filehandle.yaml
--rw-r--r--   0 ross       (501) staff       (20)      389 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/processors-missing-class.yaml
--rw-r--r--   0 ross       (501) staff       (20)      493 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/processors-wants-config.yaml
--rw-r--r--   0 ross       (501) staff       (20)      944 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/processors.yaml
--rw-r--r--   0 ross       (501) staff       (20)      461 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/provider-problems.yaml
--rw-r--r--   0 ross       (501) staff       (20)      537 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/secrets.yaml
--rw-r--r--   0 ross       (501) staff       (20)      400 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/simple-alias-zone.yaml
--rw-r--r--   0 ross       (501) staff       (20)      660 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/simple-arpa.yaml
--rw-r--r--   0 ross       (501) staff       (20)      841 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/simple-split.yaml
--rw-r--r--   0 ross       (501) staff       (20)      216 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/simple-validate.yaml
--rw-r--r--   0 ross       (501) staff       (20)     1016 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/simple.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.253710 octodns-1.6.1/tests/config/split/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.255483 octodns-1.6.1/tests/config/split/dynamic.tests.tst/
--rw-r--r--   0 ross       (501) staff       (20)      749 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/dynamic.tests.tst/a.yaml
--rw-r--r--   0 ross       (501) staff       (20)      993 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/dynamic.tests.tst/aaaa.yaml
--rw-r--r--   0 ross       (501) staff       (20)      785 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/dynamic.tests.tst/cname.yaml
--rw-r--r--   0 ross       (501) staff       (20)     1689 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/dynamic.tests.tst/real-ish-a.yaml
--rw-r--r--   0 ross       (501) staff       (20)      277 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/dynamic.tests.tst/simple-weighted.yaml
--rw-r--r--   0 ross       (501) staff       (20)       91 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/shared.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.256412 octodns-1.6.1/tests/config/split/subzone.unit.tests.tst/
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/subzone.unit.tests.tst/12.yaml
--rw-r--r--   0 ross       (501) staff       (20)       36 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/subzone.unit.tests.tst/2.yaml
--rw-r--r--   0 ross       (501) staff       (20)       37 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/subzone.unit.tests.tst/test.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.261882 octodns-1.6.1/tests/config/split/unit.tests.tst/
--rw-r--r--   0 ross       (501) staff       (20)      640 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/$unit.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)      198 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/_srv._tcp.yaml
--rw-r--r--   0 ross       (501) staff       (20)       81 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/aaaa.yaml
--rw-r--r--   0 ross       (501) staff       (20)       57 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/cname.yaml
--rw-r--r--   0 ross       (501) staff       (20)       57 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/dname.yaml
--rw-r--r--   0 ross       (501) staff       (20)       85 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/excluded.yaml
--rw-r--r--   0 ross       (501) staff       (20)       69 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/ignored.yaml
--rw-r--r--   0 ross       (501) staff       (20)       85 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/included.yaml
--rw-r--r--   0 ross       (501) staff       (20)      248 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/mx.yaml
--rw-r--r--   0 ross       (501) staff       (20)      313 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/naptr.yaml
--rw-r--r--   0 ross       (501) staff       (20)       57 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/ptr.yaml
--rw-r--r--   0 ross       (501) staff       (20)       71 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/spf.yaml
--rw-r--r--   0 ross       (501) staff       (20)       56 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/sub.yaml
--rw-r--r--   0 ross       (501) staff       (20)      166 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/txt.yaml
--rw-r--r--   0 ross       (501) staff       (20)      241 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/urlfwd.yaml
--rw-r--r--   0 ross       (501) staff       (20)       51 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/www.sub.yaml
--rw-r--r--   0 ross       (501) staff       (20)       47 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.tst/www.yaml
--rw-r--r--   0 ross       (501) staff       (20)       92 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unit.tests.yaml
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.262438 octodns-1.6.1/tests/config/split/unordered.tst/
--rw-r--r--   0 ross       (501) staff       (20)       36 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unordered.tst/abc.yaml
--rw-r--r--   0 ross       (501) staff       (20)       57 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/split/unordered.tst/xyz.yaml
--rw-r--r--   0 ross       (501) staff       (20)        4 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/sub.txt.unit.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)       99 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/subzone.unit.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)     3328 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/unit.tests.yaml
--rw-r--r--   0 ross       (501) staff       (20)      307 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/unknown-processor.yaml
--rw-r--r--   0 ross       (501) staff       (20)      217 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/unknown-provider.yaml
--rw-r--r--   0 ross       (501) staff       (20)      328 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/unknown-source-zone.yaml
--rw-r--r--   0 ross       (501) staff       (20)       89 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/config/unordered.yaml
--rw-r--r--   0 ross       (501) staff       (20)     3193 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/helpers.py
--rw-r--r--   0 ross       (501) staff       (20)     1579 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_equality.py
--rw-r--r--   0 ross       (501) staff       (20)     4690 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_idna.py
--rw-r--r--   0 ross       (501) staff       (20)    49846 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_manager.py
--rw-r--r--   0 ross       (501) staff       (20)    10810 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_plan.py
--rw-r--r--   0 ross       (501) staff       (20)     3135 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_acme.py
--rw-r--r--   0 ross       (501) staff       (20)     9011 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_arpa.py
--rw-r--r--   0 ross       (501) staff       (20)    17051 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_filter.py
--rw-r--r--   0 ross       (501) staff       (20)     9017 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_meta.py
--rw-r--r--   0 ross       (501) staff       (20)     5156 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_ownership.py
--rw-r--r--   0 ross       (501) staff       (20)     3653 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_restrict.py
--rw-r--r--   0 ross       (501) staff       (20)    12859 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_spf.py
--rw-r--r--   0 ross       (501) staff       (20)     5162 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_processor_trailing_dots.py
--rw-r--r--   0 ross       (501) staff       (20)    33602 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_provider_base.py
--rw-r--r--   0 ross       (501) staff       (20)    29948 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_provider_yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    28952 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record.py
--rw-r--r--   0 ross       (501) staff       (20)     6241 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_a.py
--rw-r--r--   0 ross       (501) staff       (20)     7294 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_aaaa.py
--rw-r--r--   0 ross       (501) staff       (20)     3468 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_alias.py
--rw-r--r--   0 ross       (501) staff       (20)     8989 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_caa.py
--rw-r--r--   0 ross       (501) staff       (20)     2926 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_change.py
--rw-r--r--   0 ross       (501) staff       (20)     1959 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_chunked.py
--rw-r--r--   0 ross       (501) staff       (20)     4291 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_cname.py
--rw-r--r--   0 ross       (501) staff       (20)     2879 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_dname.py
--rw-r--r--   0 ross       (501) staff       (20)     8304 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_ds.py
--rw-r--r--   0 ross       (501) staff       (20)    54758 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_dynamic.py
--rw-r--r--   0 ross       (501) staff       (20)     8972 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_geo.py
--rw-r--r--   0 ross       (501) staff       (20)      680 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_ip.py
--rw-r--r--   0 ross       (501) staff       (20)    24261 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_loc.py
--rw-r--r--   0 ross       (501) staff       (20)     8787 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_mx.py
--rw-r--r--   0 ross       (501) staff       (20)    13337 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_naptr.py
--rw-r--r--   0 ross       (501) staff       (20)     2537 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_ns.py
--rw-r--r--   0 ross       (501) staff       (20)     2801 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_ptr.py
--rw-r--r--   0 ross       (501) staff       (20)     2166 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_spf.py
--rw-r--r--   0 ross       (501) staff       (20)    14322 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_srv.py
--rw-r--r--   0 ross       (501) staff       (20)    10839 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_sshfp.py
--rw-r--r--   0 ross       (501) staff       (20)      737 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_target.py
--rw-r--r--   0 ross       (501) staff       (20)    14405 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_tlsa.py
--rw-r--r--   0 ross       (501) staff       (20)     6994 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_txt.py
--rw-r--r--   0 ross       (501) staff       (20)    15290 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_record_urlfwd.py
--rw-r--r--   0 ross       (501) staff       (20)     1137 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_secret_environ.py
--rw-r--r--   0 ross       (501) staff       (20)     1419 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_source_envvar.py
--rw-r--r--   0 ross       (501) staff       (20)     9293 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_source_tinydns.py
--rw-r--r--   0 ross       (501) staff       (20)     2272 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    22509 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/test_octodns_zone.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.264239 octodns-1.6.1/tests/zones/
--rw-r--r--   0 ross       (501) staff       (20)      599 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/2.0.192.in-addr.arpa.
--rw-r--r--   0 ross       (501) staff       (20)      474 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/ext.unit.tests.extension
--rw-r--r--   0 ross       (501) staff       (20)     1541 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/invalid.records.tst
--rw-r--r--   0 ross       (501) staff       (20)      362 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/invalid.zone.tst
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-17 19:47:36.265199 octodns-1.6.1/tests/zones/tinydns/
--rw-r--r--   0 ross       (501) staff       (20)     1024 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/tinydns/.is-needed-for-tests
--rwxr-xr-x   0 ross       (501) staff       (20)     2305 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/tinydns/example.com
--rw-r--r--   0 ross       (501) staff       (20)      207 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/tinydns/other.foo
--rw-r--r--   0 ross       (501) staff       (20)     1932 2024-03-17 19:47:19.000000 octodns-1.6.1/tests/zones/unit.tests.tst
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.244059 octodns-1.7.0/
+-rw-r--r--   0 ross       (501) staff       (20)    35675 2024-04-29 21:46:30.000000 octodns-1.7.0/CHANGELOG.md
+-rw-r--r--   0 ross       (501) staff       (20)     3229 2024-04-29 21:46:30.000000 octodns-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ross       (501) staff       (20)     3761 2024-04-29 21:46:30.000000 octodns-1.7.0/CONTRIBUTING.md
+-rw-r--r--   0 ross       (501) staff       (20)     1129 2024-04-29 21:46:30.000000 octodns-1.7.0/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      292 2024-04-29 21:46:30.000000 octodns-1.7.0/MANIFEST.in
+-rw-r--r--   0 ross       (501) staff       (20)    32533 2024-04-29 21:46:52.243440 octodns-1.7.0/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)    31501 2024-04-29 21:46:30.000000 octodns-1.7.0/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.151617 octodns-1.7.0/docs/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.153005 octodns-1.7.0/docs/assets/
+-rw-r--r--   0 ross       (501) staff       (20)    82371 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/assets/deploy.png
+-rw-r--r--   0 ross       (501) staff       (20)    75814 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/assets/noop.png
+-rw-r--r--   0 ross       (501) staff       (20)   212872 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/assets/pr.png
+-rw-r--r--   0 ross       (501) staff       (20)     3697 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/auto_arpa.md
+-rw-r--r--   0 ross       (501) staff       (20)     7665 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/dynamic_records.md
+-rw-r--r--   0 ross       (501) staff       (20)     3427 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/geo_records.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.153744 octodns-1.7.0/docs/logos/
+-rw-r--r--   0 ross       (501) staff       (20)     3983 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/logos/octodns-logo.png
+-rw-r--r--   0 ross       (501) staff       (20)     8514 2024-04-29 21:46:30.000000 octodns-1.7.0/docs/records.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.157122 octodns-1.7.0/octodns/
+-rw-r--r--   0 ross       (501) staff       (20)      144 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.163778 octodns-1.7.0/octodns/cmds/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     3554 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/args.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1423 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/compare.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1624 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/dump.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     3554 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/report.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1812 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/sync.py
+-rwxr-xr-x   0 ross       (501) staff       (20)     1049 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/validate.py
+-rwxr-xr-x   0 ross       (501) staff       (20)      444 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/cmds/versions.py
+-rw-r--r--   0 ross       (501) staff       (20)      641 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/context.py
+-rw-r--r--   0 ross       (501) staff       (20)      135 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/deprecation.py
+-rw-r--r--   0 ross       (501) staff       (20)      717 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/equality.py
+-rw-r--r--   0 ross       (501) staff       (20)     2373 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/idna.py
+-rw-r--r--   0 ross       (501) staff       (20)    39702 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/manager.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.168804 octodns-1.7.0/octodns/processor/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     1824 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/acme.py
+-rw-r--r--   0 ross       (501) staff       (20)     3722 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/arpa.py
+-rw-r--r--   0 ross       (501) staff       (20)     4502 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/base.py
+-rw-r--r--   0 ross       (501) staff       (20)    14464 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/filter.py
+-rw-r--r--   0 ross       (501) staff       (20)     4999 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/meta.py
+-rw-r--r--   0 ross       (501) staff       (20)     3836 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/ownership.py
+-rw-r--r--   0 ross       (501) staff       (20)     2260 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/restrict.py
+-rw-r--r--   0 ross       (501) staff       (20)     4010 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/spf.py
+-rw-r--r--   0 ross       (501) staff       (20)     1911 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/processor/trailing_dots.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.170516 octodns-1.7.0/octodns/provider/
+-rw-r--r--   0 ross       (501) staff       (20)      108 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/provider/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    12523 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/provider/base.py
+-rw-r--r--   0 ross       (501) staff       (20)    11690 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/provider/plan.py
+-rw-r--r--   0 ross       (501) staff       (20)    15812 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/provider/yaml.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.181640 octodns-1.7.0/octodns/record/
+-rw-r--r--   0 ross       (501) staff       (20)     1471 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)      412 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/a.py
+-rw-r--r--   0 ross       (501) staff       (20)      423 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/aaaa.py
+-rw-r--r--   0 ross       (501) staff       (20)      488 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/alias.py
+-rw-r--r--   0 ross       (501) staff       (20)    12299 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/base.py
+-rw-r--r--   0 ross       (501) staff       (20)     2334 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/caa.py
+-rw-r--r--   0 ross       (501) staff       (20)     1769 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/change.py
+-rw-r--r--   0 ross       (501) staff       (20)     1750 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/chunked.py
+-rw-r--r--   0 ross       (501) staff       (20)      534 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/cname.py
+-rw-r--r--   0 ross       (501) staff       (20)      296 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/dname.py
+-rw-r--r--   0 ross       (501) staff       (20)     5636 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/ds.py
+-rw-r--r--   0 ross       (501) staff       (20)    15354 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/dynamic.py
+-rw-r--r--   0 ross       (501) staff       (20)      611 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/exception.py
+-rw-r--r--   0 ross       (501) staff       (20)     5531 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/geo.py
+-rw-r--r--   0 ross       (501) staff       (20)    13426 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/geo_data.py
+-rw-r--r--   0 ross       (501) staff       (20)     1385 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/ip.py
+-rw-r--r--   0 ross       (501) staff       (20)    10692 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/loc.py
+-rw-r--r--   0 ross       (501) staff       (20)     3299 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/mx.py
+-rw-r--r--   0 ross       (501) staff       (20)     4379 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/naptr.py
+-rw-r--r--   0 ross       (501) staff       (20)      235 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/ns.py
+-rw-r--r--   0 ross       (501) staff       (20)      412 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/ptr.py
+-rw-r--r--   0 ross       (501) staff       (20)      644 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/rr.py
+-rw-r--r--   0 ross       (501) staff       (20)      512 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/spf.py
+-rw-r--r--   0 ross       (501) staff       (20)     4305 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/srv.py
+-rw-r--r--   0 ross       (501) staff       (20)     3468 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/sshfp.py
+-rw-r--r--   0 ross       (501) staff       (20)      465 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/subnet.py
+-rw-r--r--   0 ross       (501) staff       (20)     1951 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/target.py
+-rw-r--r--   0 ross       (501) staff       (20)     4998 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/tlsa.py
+-rw-r--r--   0 ross       (501) staff       (20)      257 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/txt.py
+-rw-r--r--   0 ross       (501) staff       (20)     4048 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/record/urlfwd.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.183242 octodns-1.7.0/octodns/secret/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/secret/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)      180 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/secret/base.py
+-rw-r--r--   0 ross       (501) staff       (20)      861 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/secret/environ.py
+-rw-r--r--   0 ross       (501) staff       (20)       52 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/secret/exception.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.184626 octodns-1.7.0/octodns/source/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/source/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     1712 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/source/base.py
+-rw-r--r--   0 ross       (501) staff       (20)     3280 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/source/envvar.py
+-rwxr-xr-x   0 ross       (501) staff       (20)    15823 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/source/tinydns.py
+-rw-r--r--   0 ross       (501) staff       (20)     3053 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    13121 2024-04-29 21:46:30.000000 octodns-1.7.0/octodns/zone.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.241293 octodns-1.7.0/octodns.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)    32533 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     7401 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      272 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/entry_points.txt
+-rw-r--r--   0 ross       (501) staff       (20)      317 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)        8 2024-04-29 21:46:52.000000 octodns-1.7.0/octodns.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      320 2024-04-29 21:46:30.000000 octodns-1.7.0/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)      915 2024-04-29 21:46:30.000000 octodns-1.7.0/requirements-dev.txt
+-rw-r--r--   0 ross       (501) staff       (20)      187 2024-04-29 21:46:30.000000 octodns-1.7.0/requirements.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.189233 octodns-1.7.0/script/
+-rwxr-xr-x   0 ross       (501) staff       (20)     1273 2024-04-29 21:46:30.000000 octodns-1.7.0/script/bootstrap
+-rwxr-xr-x   0 ross       (501) staff       (20)      177 2024-04-29 21:46:30.000000 octodns-1.7.0/script/changelog
+-rwxr-xr-x   0 ross       (501) staff       (20)     1115 2024-04-29 21:46:30.000000 octodns-1.7.0/script/cibuild
+-rwxr-xr-x   0 ross       (501) staff       (20)     1865 2024-04-29 21:46:30.000000 octodns-1.7.0/script/cibuild-module
+-rwxr-xr-x   0 ross       (501) staff       (20)      932 2024-04-29 21:46:30.000000 octodns-1.7.0/script/cibuild-setup-py
+-rwxr-xr-x   0 ross       (501) staff       (20)      998 2024-04-29 21:46:30.000000 octodns-1.7.0/script/coverage
+-rwxr-xr-x   0 ross       (501) staff       (20)      184 2024-04-29 21:46:30.000000 octodns-1.7.0/script/format
+-rwxr-xr-x   0 ross       (501) staff       (20)     2486 2024-04-29 21:46:30.000000 octodns-1.7.0/script/generate-geo-data
+-rwxr-xr-x   0 ross       (501) staff       (20)      387 2024-04-29 21:46:30.000000 octodns-1.7.0/script/lint
+-rwxr-xr-x   0 ross       (501) staff       (20)      772 2024-04-29 21:46:30.000000 octodns-1.7.0/script/markdown-toc
+-rwxr-xr-x   0 ross       (501) staff       (20)     1278 2024-04-29 21:46:30.000000 octodns-1.7.0/script/release
+-rwxr-xr-x   0 ross       (501) staff       (20)      662 2024-04-29 21:46:30.000000 octodns-1.7.0/script/test
+-rwxr-xr-x   0 ross       (501) staff       (20)     1940 2024-04-29 21:46:30.000000 octodns-1.7.0/script/update-requirements
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-29 21:46:52.244176 octodns-1.7.0/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     2946 2024-04-29 21:46:30.000000 octodns-1.7.0/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.208748 octodns-1.7.0/tests/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.221757 octodns-1.7.0/tests/config/
+-rw-r--r--   0 ross       (501) staff       (20)      363 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/alias-zone-loop.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      447 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/always-dry-run.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      129 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/bad-plan-output-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       63 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/bad-plan-output-missing-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       81 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/bad-provider-class-module.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       59 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/bad-provider-class-no-module.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       67 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/bad-provider-class.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.222691 octodns-1.7.0/tests/config/dynamic-arpa/
+-rw-r--r--   0 ross       (501) staff       (20)        0 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-arpa/3.2.2.in-addr.arpa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        0 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-arpa/b.e.f.f.f.d.1.8.f.2.6.0.1.2.e.0.0.5.0.4.4.6.0.1.0.6.2.ip6.arpa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      226 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-arpa/unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      543 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-arpa-no-normal-source.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      552 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-arpa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      303 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-config-no-list-zones.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      460 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     4749 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/dynamic.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        4 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/empty.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.223036 octodns-1.7.0/tests/config/hybrid/
+-rw-r--r--   0 ross       (501) staff       (20)       66 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/hybrid/one.test.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.223795 octodns-1.7.0/tests/config/hybrid/two.test./
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/hybrid/two.test./$two.test.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       58 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/hybrid/two.test./split-zone-file.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.225903 octodns-1.7.0/tests/config/include/
+-rw-r--r--   0 ross       (501) staff       (20)       24 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/array.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       15 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/dict.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        4 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/empty.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/include-doesnt-exist.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      214 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/main.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       31 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/nested.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.226189 octodns-1.7.0/tests/config/include/subdir/
+-rw-r--r--   0 ross       (501) staff       (20)       17 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/include/subdir/value.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       32 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/missing-provider-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       75 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/missing-provider-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      121 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/missing-provider-env.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       44 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/missing-sources.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      235 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/no-dump.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.226464 octodns-1.7.0/tests/config/override/
+-rw-r--r--   0 ross       (501) staff       (20)      167 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/override/dynamic.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      115 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/plan-output-filehandle.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      389 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/processors-missing-class.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      493 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/processors-wants-config.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      944 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/processors.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      461 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/provider-problems.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      537 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/secrets.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      400 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/simple-alias-zone.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      660 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/simple-arpa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      841 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/simple-split.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      216 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/simple-validate.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     1016 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/simple.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.227210 octodns-1.7.0/tests/config/split/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.229105 octodns-1.7.0/tests/config/split/dynamic.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)      749 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/dynamic.tests.tst/a.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      993 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/dynamic.tests.tst/aaaa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      785 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/dynamic.tests.tst/cname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     1689 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/dynamic.tests.tst/real-ish-a.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      277 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/dynamic.tests.tst/simple-weighted.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       91 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/shared.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.230496 octodns-1.7.0/tests/config/split/subzone.unit.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/subzone.unit.tests.tst/12.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       36 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/subzone.unit.tests.tst/2.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       37 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/subzone.unit.tests.tst/test.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.237434 octodns-1.7.0/tests/config/split/unit.tests.tst/
+-rw-r--r--   0 ross       (501) staff       (20)      640 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/$unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      198 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/_srv._tcp.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       81 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/aaaa.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/cname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/dname.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       85 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/excluded.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       69 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/ignored.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       85 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/included.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      248 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/mx.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      313 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/naptr.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/ptr.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       71 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/spf.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       56 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/sub.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      166 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/txt.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      241 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/urlfwd.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       51 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/www.sub.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       47 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.tst/www.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       92 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unit.tests.yaml
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.238252 octodns-1.7.0/tests/config/split/unordered.tst/
+-rw-r--r--   0 ross       (501) staff       (20)       36 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unordered.tst/abc.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       57 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/split/unordered.tst/xyz.yaml
+-rw-r--r--   0 ross       (501) staff       (20)        4 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/sub.txt.unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       99 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/subzone.unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     3328 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/unit.tests.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      307 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/unknown-processor.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      217 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/unknown-provider.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      328 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/unknown-source-zone.yaml
+-rw-r--r--   0 ross       (501) staff       (20)       89 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/unordered.yaml
+-rw-r--r--   0 ross       (501) staff       (20)      632 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/config/zone-threshold.yaml
+-rw-r--r--   0 ross       (501) staff       (20)     3193 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/helpers.py
+-rw-r--r--   0 ross       (501) staff       (20)     1579 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_equality.py
+-rw-r--r--   0 ross       (501) staff       (20)     4690 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_idna.py
+-rw-r--r--   0 ross       (501) staff       (20)    50769 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_manager.py
+-rw-r--r--   0 ross       (501) staff       (20)    14072 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_plan.py
+-rw-r--r--   0 ross       (501) staff       (20)     3135 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_acme.py
+-rw-r--r--   0 ross       (501) staff       (20)    12151 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_arpa.py
+-rw-r--r--   0 ross       (501) staff       (20)    17051 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_filter.py
+-rw-r--r--   0 ross       (501) staff       (20)     9017 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_meta.py
+-rw-r--r--   0 ross       (501) staff       (20)     5156 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_ownership.py
+-rw-r--r--   0 ross       (501) staff       (20)     3653 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_restrict.py
+-rw-r--r--   0 ross       (501) staff       (20)    12859 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_spf.py
+-rw-r--r--   0 ross       (501) staff       (20)     7640 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_processor_trailing_dots.py
+-rw-r--r--   0 ross       (501) staff       (20)    33602 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_provider_base.py
+-rw-r--r--   0 ross       (501) staff       (20)    29948 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_provider_yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    28952 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record.py
+-rw-r--r--   0 ross       (501) staff       (20)     6241 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_a.py
+-rw-r--r--   0 ross       (501) staff       (20)     7294 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_aaaa.py
+-rw-r--r--   0 ross       (501) staff       (20)     3468 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_alias.py
+-rw-r--r--   0 ross       (501) staff       (20)     8989 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_caa.py
+-rw-r--r--   0 ross       (501) staff       (20)     2926 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_change.py
+-rw-r--r--   0 ross       (501) staff       (20)     1959 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_chunked.py
+-rw-r--r--   0 ross       (501) staff       (20)     4291 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_cname.py
+-rw-r--r--   0 ross       (501) staff       (20)     2879 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_dname.py
+-rw-r--r--   0 ross       (501) staff       (20)     8304 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_ds.py
+-rw-r--r--   0 ross       (501) staff       (20)    54758 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_dynamic.py
+-rw-r--r--   0 ross       (501) staff       (20)     8972 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_geo.py
+-rw-r--r--   0 ross       (501) staff       (20)      680 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_ip.py
+-rw-r--r--   0 ross       (501) staff       (20)    24261 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_loc.py
+-rw-r--r--   0 ross       (501) staff       (20)     8787 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_mx.py
+-rw-r--r--   0 ross       (501) staff       (20)    13337 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_naptr.py
+-rw-r--r--   0 ross       (501) staff       (20)     2537 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_ns.py
+-rw-r--r--   0 ross       (501) staff       (20)     2801 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_ptr.py
+-rw-r--r--   0 ross       (501) staff       (20)     2166 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_spf.py
+-rw-r--r--   0 ross       (501) staff       (20)    14322 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_srv.py
+-rw-r--r--   0 ross       (501) staff       (20)    10839 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_sshfp.py
+-rw-r--r--   0 ross       (501) staff       (20)      737 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_target.py
+-rw-r--r--   0 ross       (501) staff       (20)    14405 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_tlsa.py
+-rw-r--r--   0 ross       (501) staff       (20)     6994 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_txt.py
+-rw-r--r--   0 ross       (501) staff       (20)    15290 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_record_urlfwd.py
+-rw-r--r--   0 ross       (501) staff       (20)     1137 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_secret_environ.py
+-rw-r--r--   0 ross       (501) staff       (20)     1419 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_source_envvar.py
+-rw-r--r--   0 ross       (501) staff       (20)     9293 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_source_tinydns.py
+-rw-r--r--   0 ross       (501) staff       (20)     2272 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_yaml.py
+-rw-r--r--   0 ross       (501) staff       (20)    22509 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/test_octodns_zone.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.240020 octodns-1.7.0/tests/zones/
+-rw-r--r--   0 ross       (501) staff       (20)      599 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/2.0.192.in-addr.arpa.
+-rw-r--r--   0 ross       (501) staff       (20)      474 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/ext.unit.tests.extension
+-rw-r--r--   0 ross       (501) staff       (20)     1541 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/invalid.records.tst
+-rw-r--r--   0 ross       (501) staff       (20)      362 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/invalid.zone.tst
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-29 21:46:52.240898 octodns-1.7.0/tests/zones/tinydns/
+-rw-r--r--   0 ross       (501) staff       (20)     1024 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/tinydns/.is-needed-for-tests
+-rwxr-xr-x   0 ross       (501) staff       (20)     2305 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/tinydns/example.com
+-rw-r--r--   0 ross       (501) staff       (20)      207 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/tinydns/other.foo
+-rw-r--r--   0 ross       (501) staff       (20)     1932 2024-04-29 21:46:30.000000 octodns-1.7.0/tests/zones/unit.tests.tst
```

### Comparing `octodns-1.6.1/CHANGELOG.md` & `octodns-1.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## v1.7.0 - 2024-04-29 - All the knobs and dials
+
+* Support for specifying per-zone change thresholds, to allow for zones
+  where lots of changes are expected frequently to live along side zones
+  where little or no churn is expected.
+* AutoArpa gained support for prioritizing values
+* Fix for EnsureTrailingDots reverting value types back to strings which then
+  failed when rr methods were used on them (e.g. w/octodns-bind)
+
 ## v1.6.1 - 2024-03-17 - Didn't we do this already
 
 * Fix env var type handling that was previously fixed in 1.5.1 and then
   regressed in 1.6.0.
 
 ## v1.6.0 - 2024-03-11 - It's a secret, if I told you I'd have to kill you
```

### Comparing `octodns-1.6.1/CODE_OF_CONDUCT.md` & `octodns-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/CONTRIBUTING.md` & `octodns-1.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/LICENSE` & `octodns-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/PKG-INFO` & `octodns-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns
-Version: 1.6.1
+Version: 1.7.0
 Summary: OctoDNS: DNS as code - Tools for managing DNS across multiple providers
 Home-page: https://github.com/octodns/octodns
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,16 +15,17 @@
 Requires-Dist: idna>=3.3
 Requires-Dist: natsort>=5.5.0
 Requires-Dist: python-dateutil>=2.8.1
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: pytest-network>=0.0.1; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pycountry>=19.8.18; extra == "dev"
 Requires-Dist: pycountry-convert>=0.7.2; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
```

### Comparing `octodns-1.6.1/README.md` & `octodns-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/assets/deploy.png` & `octodns-1.7.0/docs/assets/deploy.png`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/assets/noop.png` & `octodns-1.7.0/docs/assets/noop.png`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/assets/pr.png` & `octodns-1.7.0/docs/assets/pr.png`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/auto_arpa.md` & `octodns-1.7.0/docs/auto_arpa.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 Alternatively the value can be a dictionary with configuration options for the AutoArpa processor/provider.
 
 ```yaml
 ---
 manager:
   auto_arpa:
     # Whether duplicate records should replace rather than error
-    # (optiona, default False)
+    # (optional, default False)
     populate_should_replace: false
     # Explicitly set the TTL of auto-created records, default is 3600s, 1hr
     ttl: 1800
+    # Set how many PTR records will be created for the same IP, default: 999
+    max_auto_arpa: 1
+    # Inherit the TTL value of the corresponding A/AAAA record (optional,
+    # default False)
+    inherit_ttl: True
 ```
 
 Once enabled, a singleton `AutoArpa` instance, `auto-arpa`, will be added to the pool of providers and globally configured to run as the very last global processor so that it will see all records as they will be seen by targets. Further all zones ending with `arpa.` will be held back and processed after all other zones have been completed so that all `A` and `AAAA` records will have been seen prior to planning the `arpa.` zones.
 
 In order to add `PTR` records for a zone the `auto-arpa` source should be added to the list of sources for the zone.
 
 ```yaml
```

### Comparing `octodns-1.6.1/docs/dynamic_records.md` & `octodns-1.7.0/docs/dynamic_records.md`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/geo_records.md` & `octodns-1.7.0/docs/geo_records.md`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/logos/octodns-logo.png` & `octodns-1.7.0/docs/logos/octodns-logo.png`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/docs/records.md` & `octodns-1.7.0/docs/records.md`

 * *Files 12% similar despite different names*

```diff
@@ -90,14 +90,25 @@
 
 ### Lenience
 
 octoDNS is fairly strict in terms of standards compliance and is opinionated in terms of best practices. Examples of the former include SRV record naming requirements and the latter that ALIAS records are constrained to the root of zones. The strictness and support of providers varies so you may encounter existing records that fail validation when you try to dump them or you may even have use cases for which you need to create or preserve records that don't validate. octoDNS's solution to this is the `lenient` flag.
 
 It's best to think of the `lenient` flag as "I know what I'm doing and accept any problems I run across." The main reason being is that some providers may allow the non-compliant setup and others may not. The behavior of the non-compliant records may even vary from one provider to another. Caveat emptor.
 
+#### Record priority for AutoArpa
+When multiple A or AAAA records point to the same IP, it is possible to set an optional priority on each record. The records with the lowest priority will have the highest preference when being processed by AutoArpa. The AutoArpa provider will create PTR records in order of preference, up to a set limit defined by the `max_auto_arpa` option in the provider configuration.
+
+```yaml
+test:
+- type: A
+  value: 1.2.3.4
+  octodns:
+    auto_arpa_priority: 1
+```
+
 #### octodns-dump
 
 If you're trying to import a zone into octoDNS config file using `octodns-dump` which fails due to validation errors you can supply the `--lenient` argument to tell octoDNS that you acknowledge that things aren't lining up with its expectations, but you'd like it to go ahead anyway. This will do its best to populate the zone and dump the results out into an octoDNS zone file and include the non-compliant bits. If you go to use that config file octoDNS will again complain about the validation problems. You can correct them in cases where that makes sense, but if you need to preserve the non-compliant records read on for options.
 
 #### Record level lenience
 
 When there are non-compliant records configured in Yaml you can add the following to tell octoDNS to do it's best to proceed with them anyway. If you use `--lenient` above to dump a zone and you'd like to sync it as-is you can mark the problematic records this way.
@@ -122,26 +133,37 @@
     targets:
     - ns1
 ```
 
 #### Restrict Record manipulations
 
 octoDNS currently provides the ability to limit the number of updates/deletes on
-DNS records by configuring a percentage of allowed operations as a threshold.
+DNS records by configuring a percentage of allowed operations as a provider threshold.
 If left unconfigured, suitable defaults take over instead. In the below example,
 the Dyn provider is configured with limits of 40% on both update and
 delete operations over all the records present.
 
 ````yaml
 dyn:
     class: octodns.provider.dyn.DynProvider
     update_pcent_threshold: 0.4
     delete_pcent_threshold: 0.4
 ````
 
+Additionally, thresholds can be configured at the zone level. Zone thresholds
+take precedence over any provider default or explicit configuration. Zone
+thresholds do not have a default.
+
+```yaml
+zones:
+  example.com.:
+    update_pcent_threshold: 0.2
+    delete_pcent_threshold: 0.1
+```
+
 ## Provider specific record types
 
 ### Creating and registering
 
 octoDNS has support for provider specific record types through a dynamic type registration system. This functionality is powered by `Route.register_type` and can be used as follows.
 
 ```python
```

### Comparing `octodns-1.6.1/octodns/cmds/args.py` & `octodns-1.7.0/octodns/cmds/args.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/cmds/compare.py` & `octodns-1.7.0/octodns/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/cmds/dump.py` & `octodns-1.7.0/octodns/cmds/dump.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/cmds/report.py` & `octodns-1.7.0/octodns/cmds/report.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/cmds/sync.py` & `octodns-1.7.0/octodns/cmds/sync.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/cmds/validate.py` & `octodns-1.7.0/octodns/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/context.py` & `octodns-1.7.0/octodns/context.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/equality.py` & `octodns-1.7.0/octodns/equality.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/idna.py` & `octodns-1.7.0/octodns/idna.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/manager.py` & `octodns-1.7.0/octodns/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1048,10 +1048,17 @@
             raise ManagerException(
                 f'Invalid zone name {idna_decode(zone_name)}, missing ending dot'
             )
 
         zone = self.config['zones'].get(zone_name)
         if zone is not None:
             sub_zones = self.configured_sub_zones(zone_name)
-            return Zone(idna_encode(zone_name), sub_zones)
+            update_pcent_threshold = zone.get("update_pcent_threshold", None)
+            delete_pcent_threshold = zone.get("delete_pcent_threshold", None)
+            return Zone(
+                idna_encode(zone_name),
+                sub_zones,
+                update_pcent_threshold,
+                delete_pcent_threshold,
+            )
 
         raise ManagerException(f'Unknown zone name {idna_decode(zone_name)}')
```

### Comparing `octodns-1.6.1/octodns/processor/acme.py` & `octodns-1.7.0/octodns/processor/acme.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/arpa.py` & `octodns-1.7.0/octodns/processor/arpa.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,25 +7,36 @@
 from logging import getLogger
 
 from ..record import Record
 from .base import BaseProcessor
 
 
 class AutoArpa(BaseProcessor):
-    def __init__(self, name, ttl=3600, populate_should_replace=False):
+    def __init__(
+        self,
+        name,
+        ttl=3600,
+        populate_should_replace=False,
+        max_auto_arpa=999,
+        inherit_ttl=False,
+    ):
         super().__init__(name)
         self.log = getLogger(f'AutoArpa[{name}]')
         self.log.info(
-            '__init__: ttl=%d, populate_should_replace=%s',
+            '__init__: ttl=%d, populate_should_replace=%s, max_auto_arpa=%d, inherit_ttl=%s',
             ttl,
             populate_should_replace,
+            max_auto_arpa,
+            inherit_ttl,
         )
         self.ttl = ttl
         self.populate_should_replace = populate_should_replace
-        self._records = defaultdict(set)
+        self.max_auto_arpa = max_auto_arpa
+        self.inherit_ttl = inherit_ttl
+        self._records = defaultdict(list)
 
     def process_source_zone(self, desired, sources):
         for record in desired.records:
             if record._type in ('A', 'AAAA'):
                 ips = record.values
                 if record.geo:
                     for geo in record.geo.values():
@@ -33,18 +44,41 @@
                 if record.dynamic:
                     for pool in record.dynamic.pools.values():
                         for value in pool.data['values']:
                             ips.append(value['value'])
 
                 for ip in ips:
                     ptr = ip_address(ip).reverse_pointer
-                    self._records[f'{ptr}.'].add(record.fqdn)
+                    auto_arpa_priority = record.octodns.get(
+                        'auto_arpa_priority', 999
+                    )
+                    if self.inherit_ttl:
+                        record_ttl = record.ttl
+                    else:
+                        record_ttl = self.ttl
+                    self._records[f'{ptr}.'].append(
+                        (auto_arpa_priority, record_ttl, record.fqdn)
+                    )
 
         return desired
 
+    def _order_and_unique_fqdns(self, fqdns, max_auto_arpa):
+        seen = set()
+        # order the fqdns making a copy so we can reset the list below
+        ordered = sorted(fqdns)
+        fqdns = []
+        for _, record_ttl, fqdn in ordered:
+            if fqdn in seen:
+                continue
+            fqdns.append((record_ttl, fqdn))
+            seen.add(fqdn)
+            if len(seen) >= max_auto_arpa:
+                break
+        return fqdns
+
     def populate(self, zone, target=False, lenient=False):
         self.log.debug(
             'populate: name=%s, target=%s, lenient=%s',
             zone.name,
             target,
             lenient,
         )
@@ -52,26 +86,30 @@
         before = len(zone.records)
 
         zone_name = zone.name
         n = len(zone_name) + 1
         for arpa, fqdns in self._records.items():
             if arpa.endswith(f'.{zone_name}'):
                 name = arpa[:-n]
-                fqdns = sorted(fqdns)
+                # Note: this takes a list of (priority, ttl, fqdn) tuples and returns the ordered and uniqified list of fqdns.
+                fqdns = self._order_and_unique_fqdns(fqdns, self.max_auto_arpa)
                 record = Record.new(
                     zone,
                     name,
-                    {'ttl': self.ttl, 'type': 'PTR', 'values': fqdns},
+                    {
+                        'ttl': fqdns[0][0],
+                        'type': 'PTR',
+                        'values': [fqdn[1] for fqdn in fqdns],
+                    },
                     lenient=lenient,
                 )
                 zone.add_record(
                     record,
                     replace=self.populate_should_replace,
                     lenient=lenient,
                 )
-
         self.log.info(
             'populate:   found %s records', len(zone.records) - before
         )
 
     def list_zones(self):
         return set()
```

### Comparing `octodns-1.6.1/octodns/processor/base.py` & `octodns-1.7.0/octodns/processor/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/filter.py` & `octodns-1.7.0/octodns/processor/filter.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/meta.py` & `octodns-1.7.0/octodns/processor/meta.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/ownership.py` & `octodns-1.7.0/octodns/processor/ownership.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/restrict.py` & `octodns-1.7.0/octodns/processor/restrict.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/processor/spf.py` & `octodns-1.7.0/octodns/processor/spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/provider/base.py` & `octodns-1.7.0/octodns/provider/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/provider/plan.py` & `octodns-1.7.0/octodns/provider/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,24 @@
         self.desired = desired
         # Sort changes to ensure we always have a consistent ordering for
         # things that make assumptions about that. Many providers will do their
         # own ordering to ensure things happen in a way that makes sense to
         # them and/or is as safe as possible.
         self.changes = sorted(changes)
         self.exists = exists
-        self.update_pcent_threshold = update_pcent_threshold
-        self.delete_pcent_threshold = delete_pcent_threshold
 
+        # Zone thresholds take precedence over provider
+        if existing and existing.update_pcent_threshold is not None:
+            self.update_pcent_threshold = existing.update_pcent_threshold
+        else:
+            self.update_pcent_threshold = update_pcent_threshold
+        if existing and existing.delete_pcent_threshold is not None:
+            self.delete_pcent_threshold = existing.delete_pcent_threshold
+        else:
+            self.delete_pcent_threshold = delete_pcent_threshold
         change_counts = {'Create': 0, 'Delete': 0, 'Update': 0}
         for change in changes:
             change_counts[change.__class__.__name__] += 1
         self.change_counts = change_counts
 
         try:
             existing_n = len(self.existing.records)
```

### Comparing `octodns-1.6.1/octodns/provider/yaml.py` & `octodns-1.7.0/octodns/provider/yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/__init__.py` & `octodns-1.7.0/octodns/record/__init__.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/base.py` & `octodns-1.7.0/octodns/record/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/caa.py` & `octodns-1.7.0/octodns/record/caa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/change.py` & `octodns-1.7.0/octodns/record/change.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/chunked.py` & `octodns-1.7.0/octodns/record/chunked.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/cname.py` & `octodns-1.7.0/octodns/record/cname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/ds.py` & `octodns-1.7.0/octodns/record/ds.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/dynamic.py` & `octodns-1.7.0/octodns/record/dynamic.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/exception.py` & `octodns-1.7.0/octodns/record/exception.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/geo.py` & `octodns-1.7.0/octodns/record/geo.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/geo_data.py` & `octodns-1.7.0/octodns/record/geo_data.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/ip.py` & `octodns-1.7.0/octodns/record/ip.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/loc.py` & `octodns-1.7.0/octodns/record/loc.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/mx.py` & `octodns-1.7.0/octodns/record/mx.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/naptr.py` & `octodns-1.7.0/octodns/record/naptr.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,17 @@
 
 class NaptrValue(EqualityTupleMixin, dict):
     VALID_FLAGS = ('S', 'A', 'U', 'P')
 
     @classmethod
     def parse_rdata_text(cls, value):
         try:
-            (
-                order,
-                preference,
-                flags,
-                service,
-                regexp,
-                replacement,
-            ) = value.split(' ')
+            (order, preference, flags, service, regexp, replacement) = (
+                value.split(' ')
+            )
         except ValueError:
             raise RrParseError()
         try:
             order = int(order)
             preference = int(preference)
         except ValueError:
             pass
```

### Comparing `octodns-1.6.1/octodns/record/rr.py` & `octodns-1.7.0/octodns/record/rr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/spf.py` & `octodns-1.7.0/octodns/record/spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/srv.py` & `octodns-1.7.0/octodns/record/srv.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/sshfp.py` & `octodns-1.7.0/octodns/record/sshfp.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/target.py` & `octodns-1.7.0/octodns/record/target.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/tlsa.py` & `octodns-1.7.0/octodns/record/tlsa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/record/urlfwd.py` & `octodns-1.7.0/octodns/record/urlfwd.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/secret/environ.py` & `octodns-1.7.0/octodns/secret/environ.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/source/base.py` & `octodns-1.7.0/octodns/source/base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/source/envvar.py` & `octodns-1.7.0/octodns/source/envvar.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/source/tinydns.py` & `octodns-1.7.0/octodns/source/tinydns.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/yaml.py` & `octodns-1.7.0/octodns/yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/octodns/zone.py` & `octodns-1.7.0/octodns/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,21 @@
 
         super().__init__(msg)
 
 
 class Zone(object):
     log = getLogger('Zone')
 
-    def __init__(self, name, sub_zones):
+    def __init__(
+        self,
+        name,
+        sub_zones,
+        update_pcent_threshold=None,
+        delete_pcent_threshold=None,
+    ):
         if not name[-1] == '.':
             raise Exception(f'Invalid zone name {name}, missing ending dot')
         elif ' ' in name or '\t' in name:
             raise Exception(f'Invalid zone name {name}, whitespace not allowed')
 
         # internally everything is idna
         self.name = idna_encode(str(name)) if name else name
@@ -74,14 +80,17 @@
         self._records = defaultdict(set)
         self._root_ns = None
         # optional leading . to match empty hostname
         # optional trailing . b/c some sources don't have it on their fqdn
         self._utf8_name_re = re.compile(fr'\.?{idna_decode(name)}?$')
         self._idna_name_re = re.compile(fr'\.?{self.name}?$')
 
+        self.update_pcent_threshold = update_pcent_threshold
+        self.delete_pcent_threshold = delete_pcent_threshold
+
         # Copy-on-write semantics support, when `not None` this property will
         # point to a location with records for this `Zone`. Once `hydrated`
         # this property will be set to None
         self._origin = None
 
         self.log.debug('__init__: zone=%s, sub_zones=%s', self, sub_zones)
 
@@ -348,13 +357,18 @@
         `remove_record` is called.
 
         This allows low-cost copies of things to be made in situations where
         changes are unlikely and only incurs the "expense" of actually
         copying the records when required. The actual record copy will not be
         "deep" meaning that records should not be modified directly.
         '''
-        copy = Zone(self.name, self.sub_zones)
+        copy = Zone(
+            self.name,
+            self.sub_zones,
+            self.update_pcent_threshold,
+            self.delete_pcent_threshold,
+        )
         copy._origin = self
         return copy
 
     def __repr__(self):
         return f'Zone<{self.decoded_name}>'
```

### Comparing `octodns-1.6.1/octodns.egg-info/PKG-INFO` & `octodns-1.7.0/octodns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns
-Version: 1.6.1
+Version: 1.7.0
 Summary: OctoDNS: DNS as code - Tools for managing DNS across multiple providers
 Home-page: https://github.com/octodns/octodns
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,16 +15,17 @@
 Requires-Dist: idna>=3.3
 Requires-Dist: natsort>=5.5.0
 Requires-Dist: python-dateutil>=2.8.1
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: pytest-network>=0.0.1; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pycountry>=19.8.18; extra == "dev"
 Requires-Dist: pycountry-convert>=0.7.2; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
```

### Comparing `octodns-1.6.1/octodns.egg-info/SOURCES.txt` & `octodns-1.7.0/octodns.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 tests/config/sub.txt.unit.tests.yaml
 tests/config/subzone.unit.tests.yaml
 tests/config/unit.tests.yaml
 tests/config/unknown-processor.yaml
 tests/config/unknown-provider.yaml
 tests/config/unknown-source-zone.yaml
 tests/config/unordered.yaml
+tests/config/zone-threshold.yaml
 tests/config/dynamic-arpa/3.2.2.in-addr.arpa.yaml
 tests/config/dynamic-arpa/b.e.f.f.f.d.1.8.f.2.6.0.1.2.e.0.0.5.0.4.4.6.0.1.0.6.2.ip6.arpa.yaml
 tests/config/dynamic-arpa/unit.tests.yaml
 tests/config/hybrid/one.test.yaml
 tests/config/hybrid/two.test./$two.test.yaml
 tests/config/hybrid/two.test./split-zone-file.yaml
 tests/config/include/array.yaml
```

### Comparing `octodns-1.6.1/requirements-dev.txt` & `octodns-1.7.0/requirements-dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # DO NOT EDIT THIS FILE DIRECTLY - use ./script/update-requirements to update
 Pygments==2.17.2
-black==23.11.0
-build==1.0.3
-certifi==2023.11.17
+black==24.4.0
+build==1.2.1
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
-cmarkgfm==2022.10.27
-coverage==7.3.2
+cmarkgfm==2024.1.14
+coverage==7.4.4
 docutils==0.20.1
-exceptiongroup==1.2.0
-importlib-metadata==6.8.0
+importlib_metadata==7.1.0
 iniconfig==2.0.0
-isort==5.12.0
-jaraco.classes==3.3.0
-keyring==24.3.0
+isort==5.13.2
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.0
+keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
-more-itertools==10.1.0
+more-itertools==10.2.0
 mypy-extensions==1.0.0
-nh3==0.2.14
-packaging==23.2
-pathspec==0.11.2
-pkginfo==1.9.6
-platformdirs==4.0.0
-pluggy==1.3.0
+nh3==0.2.17
+packaging==24.0
+pathspec==0.12.1
+pkginfo==1.10.0
+platformdirs==4.2.0
+pluggy==1.4.0
 pprintpp==0.4.0
 pycountry-convert==0.7.2
-pycountry==22.3.5
-pycparser==2.21
-pyflakes==3.1.0
+pycountry==23.12.11
+pycparser==2.22
+pyflakes==3.2.0
 pyproject_hooks==1.0.0
-pytest-cov==4.1.0
-pytest-mock==3.12.0
+pytest-cov==5.0.0
+pytest-mock==3.14.0
 pytest-network==0.0.1
-pytest==7.4.3
-readme-renderer==42.0
+pytest==8.1.1
+readme_renderer==43.0
 repoze.lru==0.7
 requests-toolbelt==1.0.0
 requests==2.31.0
 rfc3986==2.0.0
-rich==13.7.0
-tomli==2.0.1
-twine==4.0.2
-typing_extensions==4.8.0
-urllib3==2.1.0
-zipp==3.17.0
+rich==13.7.1
+twine==5.0.0
+urllib3==2.2.1
+wheel==0.43.0
+zipp==3.18.1
```

### Comparing `octodns-1.6.1/script/bootstrap` & `octodns-1.7.0/script/bootstrap`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/cibuild` & `octodns-1.7.0/script/cibuild`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/cibuild-module` & `octodns-1.7.0/script/cibuild-module`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 TMP_DIR=$(mktemp -d -t ci-XXXXXXXXXX)
 
 echo "## venv ########################################################################"
 VENV_PYTHON=$(command -v python3)
 VENV_NAME="${TMP_DIR}/env"
 "$VENV_PYTHON" -m venv "$VENV_NAME"
 . "${VENV_NAME}/bin/activate"
-pip install setuptools
+pip install build setuptools
 echo "## environment & versions ######################################################"
 python --version
 pip --version
 echo "## install octodns from pwd ####################################################"
-python setup.py install
+VERSION="$(grep "^__version__" "./octodns/__init__.py" | sed -e "s/.* = '//" -e "s/'$//")"
+python -m build --sdist --wheel
+pip install dist/*$VERSION*.whl
 echo "## checkout provider module ####################################################"
 cd $TMP_DIR
 git clone "https://github.com/${module}.git"
 cd $(basename $module)
 echo "## install module dev requirements #############################################"
 if [ -e setup.py ]; then
   pip install -e .[dev] pytest-network
```

### Comparing `octodns-1.6.1/script/cibuild-setup-py` & `octodns-1.7.0/script/cibuild-setup-py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/bin/sh
 set -e
 
 cd "$(dirname "$0")/.."
 
+VERSION="$(grep "^__version__" "./octodns/__init__.py" | sed -e "s/.* = '//" -e "s/'$//")"
+
 echo "## create test venv ############################################################"
 TMP_DIR=$(mktemp -d -t ci-XXXXXXXXXX)
 python3 -m venv $TMP_DIR
 . "$TMP_DIR/bin/activate"
-pip install setuptools
+pip install build setuptools
 echo "## environment & versions ######################################################"
 python --version
 pip --version
 echo "## validate setup.py build #####################################################"
-python setup.py build
-echo "## validate setup.py install ###################################################"
-python setup.py install
+python -m build --sdist --wheel
+echo "## validate wheel install ###################################################"
+pip install dist/*$VERSION*.whl
 echo "## validate tests can run against installed code ###############################"
 pip install pytest pytest-network
 pytest --disable-network
 echo "## complete ####################################################################"
```

### Comparing `octodns-1.6.1/script/coverage` & `octodns-1.7.0/script/coverage`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/generate-geo-data` & `octodns-1.7.0/script/generate-geo-data`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/markdown-toc` & `octodns-1.7.0/script/markdown-toc`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/release` & `octodns-1.7.0/script/release`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/test` & `octodns-1.7.0/script/test`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/script/update-requirements` & `octodns-1.7.0/script/update-requirements`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/setup.py` & `octodns-1.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,16 +57,19 @@
     extras_require={
         'dev': tests_require
         + (
             # we need to manually/explicitely bump major versions as they're
             # likely to result in formatting changes that should happen in their
             # own PR. This will basically happen yearly
             # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
-            'black>=23.1.0,<24.0.0',
+            'black>=24.3.0,<25.0.0',
             'build>=0.7.0',
+            # docutils 0.21.x bumped to >=3.9 and 3.8 is still active. we'll
+            # have to clamp it down until we remove 3.8
+            'docutils<=0.20.1',
             'isort>=5.11.5',
             'pycountry>=19.8.18',
             'pycountry-convert>=0.7.2',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         )
```

### Comparing `octodns-1.6.1/tests/config/dynamic-arpa-no-normal-source.yaml` & `octodns-1.7.0/tests/config/dynamic-arpa-no-normal-source.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/dynamic-arpa.yaml` & `octodns-1.7.0/tests/config/dynamic-arpa.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/dynamic.tests.yaml` & `octodns-1.7.0/tests/config/dynamic.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/processors.yaml` & `octodns-1.7.0/tests/config/processors.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/secrets.yaml` & `octodns-1.7.0/tests/config/secrets.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/simple-arpa.yaml` & `octodns-1.7.0/tests/config/simple-arpa.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/simple-split.yaml` & `octodns-1.7.0/tests/config/simple-split.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/simple.yaml` & `octodns-1.7.0/tests/config/simple.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/split/dynamic.tests.tst/a.yaml` & `octodns-1.7.0/tests/config/split/dynamic.tests.tst/a.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/split/dynamic.tests.tst/aaaa.yaml` & `octodns-1.7.0/tests/config/split/dynamic.tests.tst/aaaa.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/split/dynamic.tests.tst/cname.yaml` & `octodns-1.7.0/tests/config/split/dynamic.tests.tst/cname.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/split/dynamic.tests.tst/real-ish-a.yaml` & `octodns-1.7.0/tests/config/split/dynamic.tests.tst/real-ish-a.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/split/unit.tests.tst/$unit.tests.yaml` & `octodns-1.7.0/tests/config/split/unit.tests.tst/$unit.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/config/unit.tests.yaml` & `octodns-1.7.0/tests/config/unit.tests.yaml`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/helpers.py` & `octodns-1.7.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_equality.py` & `octodns-1.7.0/tests/test_octodns_equality.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_idna.py` & `octodns-1.7.0/tests/test_octodns_idna.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_manager.py` & `octodns-1.7.0/tests/test_octodns_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1290,14 +1290,37 @@
         # but failed to fetch a secret from dummy so we just get the configured
         # value as it was in the yaml for prefix
         self.assertEqual(
             'dummy/FROM_DUMMY_WONT_WORK:hello',
             requires_dummy.fetch(':hello', None),
         )
 
+    def test_zone_threshold(self):
+        with TemporaryDirectory() as tmpdir:
+            environ['YAML_TMP_DIR'] = tmpdir.dirname
+
+            manager = Manager(get_config_filename('zone-threshold.yaml'))
+
+            zone = manager.get_zone('unit.tests.')
+
+            self.assertEqual(0.2, zone.update_pcent_threshold)
+            self.assertEqual(0.1, zone.delete_pcent_threshold)
+
+            # subzone has different threshold
+            subzone = manager.get_zone('subzone.unit.tests.')
+
+            self.assertEqual(0.02, subzone.update_pcent_threshold)
+            self.assertEqual(0.01, subzone.delete_pcent_threshold)
+
+            # test default of None to ensure Provider precedence
+            zone_with_defaults = manager.get_zone('defaultthresholds.tests.')
+
+            self.assertIsNone(zone_with_defaults.update_pcent_threshold)
+            self.assertIsNone(zone_with_defaults.delete_pcent_threshold)
+
 
 class TestMainThreadExecutor(TestCase):
     def test_success(self):
         mte = MainThreadExecutor()
 
         future = mte.submit(self.success, 42)
         self.assertEqual(42, future.result())
```

### Comparing `octodns-1.6.1/tests/test_octodns_plan.py` & `octodns-1.7.0/tests/test_octodns_plan.py`

 * *Files 17% similar despite different names*

```diff
@@ -161,16 +161,35 @@
     )
     record_3 = Record.new(
         existing, '3', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
     )
     record_4 = Record.new(
         existing, '4', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
     )
+    record_5 = Record.new(
+        existing, '5', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
+    )
+    record_6 = Record.new(
+        existing, '6', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
+    )
+    record_7 = Record.new(
+        existing, '7', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
+    )
+    record_8 = Record.new(
+        existing, '8', data={'type': 'A', 'ttl': 42, 'value': '1.2.3.4'}
+    )
 
-    def test_too_many_updates(self):
+    # manager loads the zone's config, so existing also holds providers & other config
+    update_threshold = 0.2
+    delete_threshold = 0.1
+    existing_with_thresholds = Zone(
+        'cautious.tests.', [], update_threshold, delete_threshold
+    )
+
+    def test_too_many_provider_updates(self):
         existing = self.existing.copy()
         changes = []
 
         # No records, no changes, we're good
         plan = HelperPlan(existing, None, changes, True)
         plan.raise_if_unsafe()
 
@@ -202,15 +221,54 @@
             plan.raise_if_unsafe()
         self.assertTrue('Too many updates', str(ctx.exception))
 
         # If we require more records before applying we're still OK though
         plan = HelperPlan(existing, None, changes, True, min_existing=10)
         plan.raise_if_unsafe()
 
-    def test_too_many_deletes(self):
+    def test_too_many_zone_updates(self):
+        existing = self.existing_with_thresholds.copy()
+        changes = []
+
+        # No records, no changes, we're good
+        plan = HelperPlan(existing, None, changes, True)
+        plan.raise_if_unsafe()
+
+        # Setup quite a few records, so that
+        # zone can be more cautious than provider's default
+        existing.add_record(self.record_1)
+        existing.add_record(self.record_2)
+        existing.add_record(self.record_3)
+        existing.add_record(self.record_4)
+        existing.add_record(self.record_5)
+        existing.add_record(self.record_6)
+        existing.add_record(self.record_7)
+        existing.add_record(self.record_8)
+        plan = HelperPlan(existing, None, changes, True)
+        plan.raise_if_unsafe()
+
+        # One update is ok: 12.5% < 20%
+        changes.append(Update(self.record_1, self.record_1))
+        plan = HelperPlan(existing, None, changes, True)
+        plan.raise_if_unsafe()
+
+        # Still ok, zone takes precedence
+        plan = HelperPlan(
+            existing, None, changes, True, update_pcent_threshold=0
+        )
+        plan.raise_if_unsafe()
+
+        # Two exceeds threshold, 25% > 20%
+        changes.append(Update(self.record_2, self.record_2))
+        plan = HelperPlan(existing, None, changes, True)
+        with self.assertRaises(TooMuchChange) as ctx:
+            plan.raise_if_unsafe()
+        self.assertTrue('Too many updates', str(ctx.exception))
+
+    def test_too_many_provider_deletes(self):
         existing = self.existing.copy()
         changes = []
 
         # No records, no changes, we're good
         plan = HelperPlan(existing, None, changes, True)
         plan.raise_if_unsafe()
 
@@ -242,14 +300,42 @@
             plan.raise_if_unsafe()
         self.assertTrue('Too many deletes', str(ctx.exception))
 
         # If we require more records before applying we're still OK though
         plan = HelperPlan(existing, None, changes, True, min_existing=10)
         plan.raise_if_unsafe()
 
+    def test_too_many_zone_deletes(self):
+        existing = self.existing_with_thresholds.copy()
+        changes = []
+
+        # No records, no changes, we're good
+        plan = HelperPlan(existing, None, changes, True)
+        plan.raise_if_unsafe()
+
+        # Setup quite a few records, so that
+        # zone can be more cautious than provider's default
+        existing.add_record(self.record_1)
+        existing.add_record(self.record_2)
+        existing.add_record(self.record_3)
+        existing.add_record(self.record_4)
+        existing.add_record(self.record_5)
+        existing.add_record(self.record_6)
+        existing.add_record(self.record_7)
+        existing.add_record(self.record_8)
+        plan = HelperPlan(existing, None, changes, True)
+        plan.raise_if_unsafe()
+
+        # One delete exceeds Zone threshold
+        changes.append(Delete(self.record_1))
+        plan = HelperPlan(existing, None, changes, True)
+        with self.assertRaises(TooMuchChange) as ctx:
+            plan.raise_if_unsafe()
+        self.assertTrue('Too many deletes', str(ctx.exception))
+
     def test_root_ns_change(self):
         existing = self.existing.copy()
         changes = []
 
         # No records, no changes, we're good
         plan = HelperPlan(existing, None, changes, True)
         plan.raise_if_unsafe()
```

### Comparing `octodns-1.6.1/tests/test_octodns_processor_acme.py` & `octodns-1.7.0/tests/test_octodns_processor_acme.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_filter.py` & `octodns-1.7.0/tests/test_octodns_processor_filter.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_meta.py` & `octodns-1.7.0/tests/test_octodns_processor_meta.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_ownership.py` & `octodns-1.7.0/tests/test_octodns_processor_ownership.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_restrict.py` & `octodns-1.7.0/tests/test_octodns_processor_restrict.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_spf.py` & `octodns-1.7.0/tests/test_octodns_processor_spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_processor_trailing_dots.py` & `octodns-1.7.0/tests/test_octodns_processor_trailing_dots.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 from octodns.processor.trailing_dots import (
     EnsureTrailingDots,
     _ensure_trailing_dots,
     _no_trailing_dot,
 )
 from octodns.record import Record
+from octodns.record.alias import AliasValue
+from octodns.record.cname import CnameValue
+from octodns.record.dname import DnameValue
+from octodns.record.ns import NsValue
+from octodns.record.ptr import PtrValue
 from octodns.zone import Zone
 
 
 def _find(zone, name):
     return next(r for r in zone.records if r.name == name)
 
 
@@ -33,30 +38,69 @@
             'missing',
             {'type': 'CNAME', 'ttl': 42, 'value': 'relative.target'},
             lenient=True,
         )
         zone.add_record(missing)
 
         got = etd.process_source_zone(zone, None)
+
         self.assertEqual('absolute.target.', _find(got, 'has').value)
         self.assertEqual('relative.target.', _find(got, 'missing').value)
+        # ensure types were preserved
+        self.assertIsInstance(_find(got, 'has').value, CnameValue)
+        self.assertIsInstance(_find(got, 'missing').value, CnameValue)
+
+    def test_alias(self):
+        etd = EnsureTrailingDots('test')
+
+        zone = Zone('unit.tests.', [])
+        has = Record.new(
+            zone,
+            'has',
+            {'type': 'ALIAS', 'ttl': 42, 'value': 'absolute.target.'},
+            lenient=True,
+        )
+        zone.add_record(has)
+        missing = Record.new(
+            zone,
+            'missing',
+            {'type': 'ALIAS', 'ttl': 42, 'value': 'relative.target'},
+            lenient=True,
+        )
+        zone.add_record(missing)
 
-        # HACK: this should never be done to records outside of specific testing
-        # situations like this
-        has._type = 'ALIAS'
-        missing._type = 'ALIAS'
         got = etd.process_source_zone(zone, None)
         self.assertEqual('absolute.target.', _find(got, 'has').value)
         self.assertEqual('relative.target.', _find(got, 'missing').value)
+        self.assertIsInstance(_find(got, 'has').value, AliasValue)
+        self.assertIsInstance(_find(got, 'missing').value, AliasValue)
+
+    def test_dname(self):
+        etd = EnsureTrailingDots('test')
+
+        zone = Zone('unit.tests.', [])
+        has = Record.new(
+            zone,
+            'has',
+            {'type': 'DNAME', 'ttl': 42, 'value': 'absolute.target.'},
+        )
+        zone.add_record(has)
+        missing = Record.new(
+            zone,
+            'missing',
+            {'type': 'DNAME', 'ttl': 42, 'value': 'relative.target'},
+            lenient=True,
+        )
+        zone.add_record(missing)
 
-        has._type = 'DNAME'
-        missing._type = 'DNAME'
         got = etd.process_source_zone(zone, None)
         self.assertEqual('absolute.target.', _find(got, 'has').value)
         self.assertEqual('relative.target.', _find(got, 'missing').value)
+        self.assertIsInstance(_find(got, 'has').value, DnameValue)
+        self.assertIsInstance(_find(got, 'missing').value, DnameValue)
 
     def test_mx(self):
         etd = EnsureTrailingDots('test')
 
         zone = Zone('unit.tests.', [])
         record = Record.new(
             zone,
@@ -110,21 +154,56 @@
             lenient=True,
         )
         zone.add_record(record)
 
         got = etd.process_source_zone(zone, None)
         got = next(iter(got.records))
         self.assertEqual(['absolute.target.', 'relative.target.'], got.values)
+        self.assertIsInstance(got.values[0], NsValue)
+        self.assertIsInstance(got.values[1], NsValue)
+
+        # again, but this time nothing to fix so that we fully use up the
+        # generator
+        zone = Zone('unit.tests.', [])
+        record = Record.new(
+            zone,
+            'record',
+            {
+                'type': 'NS',
+                'ttl': 42,
+                'values': ['absolute.target.', 'another.target.'],
+            },
+        )
+        zone.add_record(record)
+
+        got = etd.process_source_zone(zone, None)
+        got = next(iter(got.records))
+        self.assertEqual(['absolute.target.', 'another.target.'], got.values)
+
+    def test_ptr(self):
+        etd = EnsureTrailingDots('test')
+
+        zone = Zone('unit.tests.', [])
+        record = Record.new(
+            zone,
+            'record',
+            {
+                'type': 'PTR',
+                'ttl': 42,
+                'values': ['absolute.target.', 'relative.target'],
+            },
+            lenient=True,
+        )
+        zone.add_record(record)
 
-        # HACK: this should never be done to records outside of specific testing
-        # situations like this
-        record._type = 'PTR'
         got = etd.process_source_zone(zone, None)
         got = next(iter(got.records))
         self.assertEqual(['absolute.target.', 'relative.target.'], got.values)
+        self.assertIsInstance(got.values[0], PtrValue)
+        self.assertIsInstance(got.values[1], PtrValue)
 
     def test_srv(self):
         etd = EnsureTrailingDots('test')
 
         zone = Zone('unit.tests.', [])
         record = Record.new(
             zone,
```

### Comparing `octodns-1.6.1/tests/test_octodns_provider_base.py` & `octodns-1.7.0/tests/test_octodns_provider_base.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_provider_yaml.py` & `octodns-1.7.0/tests/test_octodns_provider_yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record.py` & `octodns-1.7.0/tests/test_octodns_record.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_a.py` & `octodns-1.7.0/tests/test_octodns_record_a.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_aaaa.py` & `octodns-1.7.0/tests/test_octodns_record_aaaa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_alias.py` & `octodns-1.7.0/tests/test_octodns_record_alias.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_caa.py` & `octodns-1.7.0/tests/test_octodns_record_caa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_change.py` & `octodns-1.7.0/tests/test_octodns_record_change.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_chunked.py` & `octodns-1.7.0/tests/test_octodns_record_chunked.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_cname.py` & `octodns-1.7.0/tests/test_octodns_record_cname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_dname.py` & `octodns-1.7.0/tests/test_octodns_record_dname.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_ds.py` & `octodns-1.7.0/tests/test_octodns_record_ds.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_dynamic.py` & `octodns-1.7.0/tests/test_octodns_record_dynamic.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_geo.py` & `octodns-1.7.0/tests/test_octodns_record_geo.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_ip.py` & `octodns-1.7.0/tests/test_octodns_record_ip.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_loc.py` & `octodns-1.7.0/tests/test_octodns_record_loc.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_mx.py` & `octodns-1.7.0/tests/test_octodns_record_mx.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_naptr.py` & `octodns-1.7.0/tests/test_octodns_record_naptr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_ns.py` & `octodns-1.7.0/tests/test_octodns_record_ns.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_ptr.py` & `octodns-1.7.0/tests/test_octodns_record_ptr.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_spf.py` & `octodns-1.7.0/tests/test_octodns_record_spf.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_srv.py` & `octodns-1.7.0/tests/test_octodns_record_srv.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_sshfp.py` & `octodns-1.7.0/tests/test_octodns_record_sshfp.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_target.py` & `octodns-1.7.0/tests/test_octodns_record_target.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_tlsa.py` & `octodns-1.7.0/tests/test_octodns_record_tlsa.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_txt.py` & `octodns-1.7.0/tests/test_octodns_record_txt.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_record_urlfwd.py` & `octodns-1.7.0/tests/test_octodns_record_urlfwd.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_secret_environ.py` & `octodns-1.7.0/tests/test_octodns_secret_environ.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_source_envvar.py` & `octodns-1.7.0/tests/test_octodns_source_envvar.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_source_tinydns.py` & `octodns-1.7.0/tests/test_octodns_source_tinydns.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_yaml.py` & `octodns-1.7.0/tests/test_octodns_yaml.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/test_octodns_zone.py` & `octodns-1.7.0/tests/test_octodns_zone.py`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/zones/2.0.192.in-addr.arpa.` & `octodns-1.7.0/tests/zones/2.0.192.in-addr.arpa.`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/zones/invalid.records.tst` & `octodns-1.7.0/tests/zones/invalid.records.tst`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/zones/tinydns/.is-needed-for-tests` & `octodns-1.7.0/tests/zones/tinydns/.is-needed-for-tests`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/zones/tinydns/example.com` & `octodns-1.7.0/tests/zones/tinydns/example.com`

 * *Files identical despite different names*

### Comparing `octodns-1.6.1/tests/zones/unit.tests.tst` & `octodns-1.7.0/tests/zones/unit.tests.tst`

 * *Files identical despite different names*

