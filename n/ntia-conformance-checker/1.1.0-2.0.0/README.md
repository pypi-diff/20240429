# Comparing `tmp/ntia_conformance_checker-1.1.0.tar.gz` & `tmp/ntia_conformance_checker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntia_conformance_checker-1.1.0.tar", last modified: Thu Dec 28 19:47:27 2023, max compression
+gzip compressed data, was "ntia_conformance_checker-2.0.0.tar", last modified: Mon Apr 29 19:58:48 2024, max compression
```

## Comparing `ntia_conformance_checker-1.1.0.tar` & `ntia_conformance_checker-2.0.0.tar`

### file list

```diff
@@ -1,194 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.108248 ntia_conformance_checker-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.044248 ntia_conformance_checker-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.044248 ntia_conformance_checker-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/bandit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.048248 ntia_conformance_checker-1.1.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.048248 ntia_conformance_checker-1.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/ntia-conformance-checker.iml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2023-12-28 19:47:27.108248 ntia_conformance_checker-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.048248 ntia_conformance_checker-1.1.0/ntia_conformance_checker/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    13174 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker/sbom_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.104248 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2023-12-28 19:47:26.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2023-12-28 19:47:27.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 19:47:26.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-28 19:47:26.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-28 19:47:26.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-28 19:47:26.000000 ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/release.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 19:47:27.108248 ntia_conformance_checker-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.048248 ntia_conformance_checker-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.040248 ntia_conformance_checker-1.1.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.052248 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13451 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/alpine.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    25506 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    27752 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.052248 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    35758 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16603 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    21925 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18436 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.052248 ntia_conformance_checker-1.1.0/tests/data/missing_component_name/
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXJsonExample.json
--rw-r--r--   0 runner    (1001) docker     (127)    17744 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXRdfExample.rdf
--rw-r--r--   0 runner    (1001) docker     (127)    15054 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXXmlExample.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXYamlExample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.052248 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    36044 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18504 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.056248 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    20074 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17453 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.056248 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/
--rw-r--r--   0 runner    (1001) docker     (127)    20983 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    24068 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19863 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.056248 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/
--rw-r--r--   0 runner    (1001) docker     (127)    19312 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    35921 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16672 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    22022 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18503 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.060248 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/
--rw-r--r--   0 runner    (1001) docker     (127)    19298 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    34397 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16654 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18448 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.060248 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    35941 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16693 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.060248 ntia_conformance_checker-1.1.0/tests/data/other_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/other_tests/SPDXSimpleTag.tag
--rw-r--r--   0 runner    (1001) docker     (127)    16777 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/data/other_tests/test_components_without_functions.spdx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.040248 ntia_conformance_checker-1.1.0/tests/doc_fest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.060248 ntia_conformance_checker-1.1.0/tests/doc_fest/FOSSology/
--rw-r--r--   0 runner    (1001) docker     (127)   265354 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   265322 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.076248 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    25724 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127) 10020640 2023-12-28 19:47:13.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    58486 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   177744 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.076248 ntia_conformance_checker-1.1.0/tests/doc_fest/MetaSpdxscanner/
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   298947 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.080248 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    42218 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   440190 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   112550 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.080248 ntia_conformance_checker-1.1.0/tests/doc_fest/Philips/
--rw-r--r--   0 runner    (1001) docker     (127)   243446 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Philips/keyclock_sbom.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.084248 ntia_conformance_checker-1.1.0/tests/doc_fest/REA/
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/REA/AppBOM-inationVDR.xml
--rw-r--r--   0 runner    (1001) docker     (127)   191631 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   230822 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/REA/PyYamlVDR.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.092248 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json
--rw-r--r--   0 runner    (1001) docker     (127)   250152 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   190258 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   182863 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   754185 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)   140277 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   162052 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   272289 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   706941 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (127)   976785 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig
--rw-r--r--   0 runner    (1001) docker     (127)   184179 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   217286 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.092248 ntia_conformance_checker-1.1.0/tests/doc_fest/SynopsysBlackDuck/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.096248 ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/
--rw-r--r--   0 runner    (1001) docker     (127)    52051 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/appbomination_container.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   994639 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)   965989 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.100248 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/app.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   514309 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    57063 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    53845 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    16876 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   140247 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    40468 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.100248 ntia_conformance_checker-1.1.0/tests/doc_fest/metaeffekt/
--rw-r--r--   0 runner    (1001) docker     (127)  3246600 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:47:27.104248 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/
--rw-r--r--   0 runner    (1001) docker     (127)    36870 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/App-BOM-ination.json
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   363611 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json
--rw-r--r--   0 runner    (1001) docker     (127)    44486 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)   744585 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/gnu_time-v1.9.json
--rw-r--r--   0 runner    (1001) docker     (127)    74530 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)    25719 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/serve-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2023-12-28 19:47:14.000000 ntia_conformance_checker-1.1.0/tests/test_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.371568 ntia_conformance_checker-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.311568 ntia_conformance_checker-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.311568 ntia_conformance_checker-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/bandit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 19:58:48.371568 ntia_conformance_checker-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.315568 ntia_conformance_checker-2.0.0/ntia_conformance_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker/sbom_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.371568 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 19:58:48.000000 ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:58:48.371568 ntia_conformance_checker-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.315568 ntia_conformance_checker-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.307568 ntia_conformance_checker-2.0.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.315568 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/alpine.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    25506 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27752 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.319568 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35758 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    21925 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.319568 ntia_conformance_checker-2.0.0/tests/data/missing_component_name/
+-rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXJsonExample.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17744 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXRdfExample.rdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXXmlExample.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXYamlExample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.319568 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36044 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18504 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.319568 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/
+-rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    20074 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17453 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.323568 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/
+-rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40191 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    24025 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19820 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.323568 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/
+-rw-r--r--   0 runner    (1001) docker     (127)    19312 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16672 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    22022 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18503 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.323568 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19298 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34397 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18448 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.327568 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35941 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16693 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.327568 ntia_conformance_checker-2.0.0/tests/data/other_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/other_tests/SPDXSimpleTag.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/data/other_tests/test_components_without_functions.spdx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.307568 ntia_conformance_checker-2.0.0/tests/doc_fest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.327568 ntia_conformance_checker-2.0.0/tests/doc_fest/FOSSology/
+-rw-r--r--   0 runner    (1001) docker     (127)   265354 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   265322 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.339568 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    25724 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127) 10020640 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    58486 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   177744 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.343568 ntia_conformance_checker-2.0.0/tests/doc_fest/MetaSpdxscanner/
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   298947 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.347568 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42218 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   440190 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   112550 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.347568 ntia_conformance_checker-2.0.0/tests/doc_fest/Philips/
+-rw-r--r--   0 runner    (1001) docker     (127)   243446 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Philips/keyclock_sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.347568 ntia_conformance_checker-2.0.0/tests/doc_fest/REA/
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/REA/AppBOM-inationVDR.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   191631 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   230822 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/REA/PyYamlVDR.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.355568 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json
+-rw-r--r--   0 runner    (1001) docker     (127)   250152 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   190258 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   182863 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   754185 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   140277 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   162052 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   272289 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   706941 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   976785 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig
+-rw-r--r--   0 runner    (1001) docker     (127)   184179 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   217286 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.359568 ntia_conformance_checker-2.0.0/tests/doc_fest/SynopsysBlackDuck/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.359568 ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/
+-rw-r--r--   0 runner    (1001) docker     (127)    52051 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/appbomination_container.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   994639 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)   965989 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.363568 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/app.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   514309 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    57063 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    53845 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   140247 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    40468 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.363568 ntia_conformance_checker-2.0.0/tests/doc_fest/metaeffekt/
+-rw-r--r--   0 runner    (1001) docker     (127)  3246600 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:58:48.371568 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/
+-rw-r--r--   0 runner    (1001) docker     (127)    36870 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/App-BOM-ination.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   363611 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44486 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)   744585 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/gnu_time-v1.9.json
+-rw-r--r--   0 runner    (1001) docker     (127)    74530 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    25719 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/serve-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-04-29 19:58:41.000000 ntia_conformance_checker-2.0.0/tests/test_checker.py
```

### Comparing `ntia_conformance_checker-1.1.0/.github/workflows/build.yml` & `ntia_conformance_checker-2.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/.github/workflows/codeql.yml` & `ntia_conformance_checker-2.0.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/.github/workflows/pylint.yml` & `ntia_conformance_checker-2.0.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/.github/workflows/python-publish.yml` & `ntia_conformance_checker-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/.gitignore` & `ntia_conformance_checker-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/CONTRIBUTING.md` & `ntia_conformance_checker-2.0.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,25 +43,26 @@
    retroactively signs a range of past commits.
 
 5. Test your changes:
    ```sh
    python setup.py test # in the repo root
    ```
    You may use other test runners, such as `pytest` or `nose` at your preference.
-6. Push the branch to your fork on GitHub:
+6. Format your changes with [`black`](https://github.com/psf/black) and [`pylint`](https://github.com/pylint-dev/pylint).
+7. Push the branch to your fork on GitHub:
    ```sh
    git push origin fix-or-improve-something
    ```
-7. Make a pull request on GitHub.
-8. Continue making more changes and commits on the branch, with `git commit --signoff` and `git push`.
-9. When done, write a comment on the PR asking for a code review.
-10. Some other developer will review your changes and accept your PR. The merge should be done with `rebase`, if
+8. Make a pull request on GitHub.
+9. Continue making more changes and commits on the branch, with `git commit --signoff` and `git push`.
+10. When done, write a comment on the PR asking for a code review.
+11. Some other developer will review your changes and accept your PR. The merge should be done with `rebase`, if
     possible, or with `squash`.
-11. The temporary branch on GitHub should be deleted (there is a button for deleting it).
-12. Delete the local branch as well:
+12. The temporary branch on GitHub should be deleted (there is a button for deleting it).
+13. Delete the local branch as well:
     ```sh
     git checkout master
     git pull -p
     git branch -a
     git branch -d fix-or-improve-something
     ```
```

### Comparing `ntia_conformance_checker-1.1.0/LICENSE` & `ntia_conformance_checker-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/PKG-INFO` & `ntia_conformance_checker-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntia_conformance_checker
-Version: 1.1.0
+Version: 2.0.0
 Summary: Check SPDX SBOM for NTIA minimum elements
 Author-email: Josh Lin <linynjosh@gmail.com>, John Speed Meyers <johnmeyersster@gmail.com>
 Maintainer-email: John Speed Meyers <johnmeyersster@gmail.com>, Gary O'Neall <gary@sourceauditor.com>, Josh Lin <linynjosh@gmail.com>, SPDX group at the Linux Foundation and others <spdx-implementers+owner@lists.spdx.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/ntia-conformance-checker
 Keywords: spdx,sbom,ntia
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,15 @@
 
 `pip install ntia-conformance-checker`
 
 Alternatively, just clone the repo and install dependencies using the following commands:
 
 ```bash
 git clone https://github.com/spdx/ntia-conformance-checker.git
+cd ntia-conformance-checker
 pip install .
 ```
 
 The tool requires Python 3 (3.8+). It is recommended to use a virtual python environment especially
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
@@ -90,15 +91,15 @@
 
 ```python
 
 import ntia_conformance_checker as ntia
 
 sbom = ntia.SbomChecker("SBOM_filepath")
 
-print(sbom.ntia_mininum_elements_compliant)
+print(sbom.ntia_minimum_elements_compliant)
 ```
 
 Additional properties and methods associated with `SbomChecker()` can be found in [`sbom_checker.py`](ntia_conformance_checker/sbom_checker.py).
 
 # History
 
 This is the result of an initial [Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/) contribution in 2022 by
```

### Comparing `ntia_conformance_checker-1.1.0/Pipfile.lock` & `ntia_conformance_checker-2.0.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/README.md` & `ntia_conformance_checker-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 `pip install ntia-conformance-checker`
 
 Alternatively, just clone the repo and install dependencies using the following commands:
 
 ```bash
 git clone https://github.com/spdx/ntia-conformance-checker.git
+cd ntia-conformance-checker
 pip install .
 ```
 
 The tool requires Python 3 (3.8+). It is recommended to use a virtual python environment especially
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
@@ -67,15 +68,15 @@
 
 ```python
 
 import ntia_conformance_checker as ntia
 
 sbom = ntia.SbomChecker("SBOM_filepath")
 
-print(sbom.ntia_mininum_elements_compliant)
+print(sbom.ntia_minimum_elements_compliant)
 ```
 
 Additional properties and methods associated with `SbomChecker()` can be found in [`sbom_checker.py`](ntia_conformance_checker/sbom_checker.py).
 
 # History
 
 This is the result of an initial [Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/) contribution in 2022 by
```

### Comparing `ntia_conformance_checker-1.1.0/ntia_conformance_checker/main.py` & `ntia_conformance_checker-2.0.0/ntia_conformance_checker/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,12 +70,12 @@
                 json.dump(result_dict, outfile)
         else:
             print(json.dumps(result_dict, indent=2))
     if args.output == "html":
         html_output = sbom.output_html()
         print(html_output)
     # 0 indicates success
-    sys.exit(0 if sbom.ntia_mininum_elements_compliant else 1)
+    sys.exit(0 if sbom.ntia_minimum_elements_compliant else 1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ntia_conformance_checker-1.1.0/ntia_conformance_checker/sbom_checker.py` & `ntia_conformance_checker-2.0.0/ntia_conformance_checker/sbom_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # pylint: disable=import-error
 
 import logging
 import os
 import sys
 
+from spdx_tools.spdx.model import RelationshipType
 from spdx_tools.spdx.parser import parse_anything
 from spdx_tools.spdx.model.spdx_no_assertion import SpdxNoAssertion
 from spdx_tools.spdx.parser.error import SPDXParsingError
 from spdx_tools.spdx.validation.document_validator import validate_full_spdx_document
 
 
 # pylint: disable=too-many-instance-attributes
@@ -17,15 +18,15 @@
     """SBOM minimum elements check."""
 
     def __init__(self, file, validate=True):
         self.file = file
         self.parsing_error = []
         self.doc = self.parse_file()
         if not self.doc:
-            self.ntia_mininum_elements_compliant = False
+            self.ntia_minimum_elements_compliant = False
         else:
             self.validation_messages = None
             if validate:
                 self.validation_messages = validate_full_spdx_document(self.doc)
             self.sbom_name = self.doc.creation_info.name
             self.doc_version = self.check_doc_version()
             self.doc_author = True
@@ -33,15 +34,15 @@
             self.dependency_relationships = self.check_dependency_relationships()
             self.components_without_names = self.get_components_without_names()
             self.components_without_versions = self.get_components_without_versions()
             self.components_without_suppliers = self.get_components_without_suppliers()
             self.components_without_identifiers = (
                 self.get_components_without_identifiers()
             )
-            self.ntia_mininum_elements_compliant = (
+            self.ntia_minimum_elements_compliant = (
                 self.check_ntia_minimum_elements_compliance()
             )
 
     def parse_file(self):
         """Parse SBOM document."""
         # check if file exists
         if not os.path.exists(self.file):
@@ -57,18 +58,27 @@
     def check_doc_version(self):
         """Check for SPDX document version."""
         if str(self.doc.creation_info.spdx_version) not in ["SPDX-2.2", "SPDX-2.3"]:
             return False
         return True
 
     def check_dependency_relationships(self):
-        """Check for existence of any relationships."""
-        if len(self.doc.relationships) == 0:
-            return False
-        return True
+        """Check that the document DESCRIBES at least one package."""
+        describes_relationships = [
+            rel
+            for rel in self.doc.relationships
+            if rel.relationship_type == RelationshipType.DESCRIBES
+        ]
+
+        # Check if any of the "DESCRIBES" relationships describe a Package
+        describes_package = any(
+            "Package" in rel.related_spdx_element_id for rel in describes_relationships
+        )
+
+        return describes_package
 
     def get_components_without_names(self):
         """Retrieve SPDX ID of components without names."""
         components_without_names = []
         for package in self.doc.packages:
             if not package.name:
                 components_without_names.append(package.spdx_id)
@@ -85,24 +95,18 @@
                     components_without_versions.append(package.name)
         return components_without_versions
 
     def get_components_without_suppliers(self, return_tuples=False):
         """Retrieve name and/or SPDX ID of components without suppliers."""
         components_without_suppliers = []
         for package in self.doc.packages:
-            # both package supplier and package originator satisfy the "supplier"
-            # requirement
-            # https://spdx.github.io/spdx-spec/v2.3/package-information/#76-package-originator-field
-            no_package_supplier = package.supplier is None or isinstance(
+            no_supplier = package.supplier is None or isinstance(
                 package.supplier, SpdxNoAssertion
             )
-            no_package_originator = package.originator is None or isinstance(
-                package.originator, SpdxNoAssertion
-            )
-            if no_package_supplier and no_package_originator:
+            if no_supplier:
                 if return_tuples:
                     components_without_suppliers.append((package.name, package.spdx_id))
                 else:
                     components_without_suppliers.append(package.name)
 
         return components_without_suppliers
 
@@ -134,26 +138,26 @@
         return len(self.doc.packages)
 
     def print_table_output(self):
         """Print element-by-element result table."""
         # pylint: disable=line-too-long
         if self.parsing_error:
             print(
-                f"\nIs this SBOM NTIA minimum element conformant? {self.ntia_mininum_elements_compliant}\n"
+                f"\nIs this SBOM NTIA minimum element conformant? {self.ntia_minimum_elements_compliant}\n"
             )
             print(
                 "The provided document couldn't be parsed, check for ntia minimum elements couldn't be performed.\n"
             )
             print("The following SPDXParsingError was raised:\n")
             for error in self.parsing_error:
                 print(error)
 
         else:
             print(
-                f"\nIs this SBOM NTIA minimum element conformant? {self.ntia_mininum_elements_compliant}\n"
+                f"\nIs this SBOM NTIA minimum element conformant? {self.ntia_minimum_elements_compliant}\n"
             )
             print("Individual elements                            | Status")
             print("-------------------------------------------------------")
             print(
                 f"All component names provided?                  | {not self.components_without_names}"
             )
             print(
@@ -253,24 +257,24 @@
             ] = not self.components_without_suppliers
             result["totalNumberComponents"] = self.get_total_number_components()
             if self.validation_messages:
                 result["validationMessages"] = list(map(str, self.validation_messages))
         else:
             result["parsingError"] = self.parsing_error
 
-        result["isNtiaConformant"] = self.ntia_mininum_elements_compliant
+        result["isNtiaConformant"] = self.ntia_minimum_elements_compliant
 
         return result
 
     def output_html(self):
         """Print HTML of output."""
         if self.doc:
             result = (
                 f" <h2>NTIA Conformance Results</h2> "
-                f"<h3>Conformant: {self.ntia_mininum_elements_compliant} </h3>"
+                f"<h3>Conformant: {self.ntia_minimum_elements_compliant} </h3>"
                 f"<table> <tr> "
                 f"<th>Individual Elements</th> <th>Conformant</th> </tr> "
                 f"<tr> <td>All component names provided</td>"
                 f" <td>{not self.components_without_names}</td> </tr> "
                 f"<tr> <td>All component versions provided</td>"
                 f" <td>{not self.components_without_versions}</td> </tr> "
                 f"<tr> <td>All component identifiers provided</td> "
@@ -291,15 +295,15 @@
                     "The following errors were found:</p>\n"
                 )
             for message in self.validation_messages:
                 result += f"<p>{message.validation_message}</p>\n"
         else:
             result = f"""
             <h2>NTIA Conformance Results</h2>
-            <h3>Conformant: {self.ntia_mininum_elements_compliant} </h3>
+            <h3>Conformant: {self.ntia_minimum_elements_compliant} </h3>
             <p>The provided document couldn't be parsed, check for ntia minimum elements couldn't be performed.</p>
             <p>The following SPDXParsingError was raised:<p><ul>"""
             for error in self.parsing_error:
                 result += f"""<li>{error}</li>"""
 
             result += """</ul>"""
```

### Comparing `ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/PKG-INFO` & `ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntia_conformance_checker
-Version: 1.1.0
+Version: 2.0.0
 Summary: Check SPDX SBOM for NTIA minimum elements
 Author-email: Josh Lin <linynjosh@gmail.com>, John Speed Meyers <johnmeyersster@gmail.com>
 Maintainer-email: John Speed Meyers <johnmeyersster@gmail.com>, Gary O'Neall <gary@sourceauditor.com>, Josh Lin <linynjosh@gmail.com>, SPDX group at the Linux Foundation and others <spdx-implementers+owner@lists.spdx.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/ntia-conformance-checker
 Keywords: spdx,sbom,ntia
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,15 @@
 
 `pip install ntia-conformance-checker`
 
 Alternatively, just clone the repo and install dependencies using the following commands:
 
 ```bash
 git clone https://github.com/spdx/ntia-conformance-checker.git
+cd ntia-conformance-checker
 pip install .
 ```
 
 The tool requires Python 3 (3.8+). It is recommended to use a virtual python environment especially
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
@@ -90,15 +91,15 @@
 
 ```python
 
 import ntia_conformance_checker as ntia
 
 sbom = ntia.SbomChecker("SBOM_filepath")
 
-print(sbom.ntia_mininum_elements_compliant)
+print(sbom.ntia_minimum_elements_compliant)
 ```
 
 Additional properties and methods associated with `SbomChecker()` can be found in [`sbom_checker.py`](ntia_conformance_checker/sbom_checker.py).
 
 # History
 
 This is the result of an initial [Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/) contribution in 2022 by
```

### Comparing `ntia_conformance_checker-1.1.0/ntia_conformance_checker.egg-info/SOURCES.txt` & `ntia_conformance_checker-2.0.0/ntia_conformance_checker.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,14 @@
 .github/dependabot.yml
 .github/workflows/bandit.yml
 .github/workflows/black.yml
 .github/workflows/build.yml
 .github/workflows/codeql.yml
 .github/workflows/pylint.yml
 .github/workflows/python-publish.yml
-.idea/.gitignore
-.idea/misc.xml
-.idea/modules.xml
-.idea/ntia-conformance-checker.iml
-.idea/vcs.xml
-.idea/inspectionProfiles/Project_Default.xml
-.idea/inspectionProfiles/profiles_settings.xml
 ntia_conformance_checker/__init__.py
 ntia_conformance_checker/main.py
 ntia_conformance_checker/sbom_checker.py
 ntia_conformance_checker.egg-info/PKG-INFO
 ntia_conformance_checker.egg-info/SOURCES.txt
 ntia_conformance_checker.egg-info/dependency_links.txt
 ntia_conformance_checker.egg-info/entry_points.txt
```

### Comparing `ntia_conformance_checker-1.1.0/pyproject.toml` & `ntia_conformance_checker-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=3.4.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ntia_conformance_checker"
-version = "1.1.0"
+version = "2.0.0"
 authors = [
     {name = "Josh Lin", email = "linynjosh@gmail.com"},
     {name = "John Speed Meyers", email = "johnmeyersster@gmail.com"}
 ]
 maintainers = [
     {name = "John Speed Meyers", email = "johnmeyersster@gmail.com"},
     {name = "Gary O'Neall", email = "gary@sourceauditor.com"},
```

### Comparing `ntia_conformance_checker-1.1.0/release.md` & `ntia_conformance_checker-2.0.0/release.md`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/alpine.spdx` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/alpine.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXJsonExample.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXJsonExample.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXRdfExample.rdf` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXRdfExample.rdf`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXXmlExample.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXXmlExample.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_name/SPDXYamlExample.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_name/SPDXYamlExample.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987179487179486%*

 * *Differences: {"'packages'": "{0: {'originator': 'NOASSERTION', 'supplier': 'Organization: ExampleCodeInspect "*

 * *               "(contact@example.com)'}}"}*

```diff
@@ -280,27 +280,27 @@
             "licenseDeclared": "(LGPL-2.0-only AND LicenseRef-3)",
             "licenseInfoFromFiles": [
                 "GPL-2.0-only",
                 "LicenseRef-2",
                 "LicenseRef-1"
             ],
             "name": "glibc",
-            "originator": "Organization: ExampleCodeInspect (contact@example.com)",
+            "originator": "NOASSERTION",
             "packageFileName": "glibc-2.11.1.tar.gz",
             "packageVerificationCode": {
                 "packageVerificationCodeExcludedFiles": [
                     "./package.spdx"
                 ],
                 "packageVerificationCodeValue": "d6a770ba38583ed4bb4525bd96e50461655d2758"
             },
             "primaryPackagePurpose": "SOURCE",
             "releaseDate": "2012-01-29T18:30:22Z",
             "sourceInfo": "uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.",
             "summary": "GNU C library.",
-            "supplier": "NOASSERTION",
+            "supplier": "Organization: ExampleCodeInspect (contact@example.com)",
             "validUntilDate": "2014-01-29T18:30:22Z"
         }
     ],
     "relationships": [
         {
             "relatedSpdxElement": "SPDXRef-Package",
             "relationshipType": "CONTAINS",
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml`

```diff
@@ -280,17 +280,17 @@
                 <rdfs:comment>Package level annotation</rdfs:comment>
                 <spdx:annotationDate>2011-01-29T18:30:22Z</spdx:annotationDate>
               </spdx:Annotation>
             </spdx:annotation>
             <spdx:downloadLocation>http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz</spdx:downloadLocation>
             <spdx:name>glibc</spdx:name>
             <doap:homepage>http://ftp.gnu.org/gnu/glibc</doap:homepage>
-            <spdx:originator>Organization: ExampleCodeInspect (contact@example.com)</spdx:originator>
+            <spdx:originator>NOASSERTION</spdx:originator>
             <spdx:builtDate>2011-01-29T18:30:22Z</spdx:builtDate>
-            <spdx:supplier>NOASSERTION</spdx:supplier>
+            <spdx:supplier>Organization: ExampleCodeInspect (contact@example.com)</spdx:supplier>
             <spdx:licenseDeclared>
               <spdx:ConjunctiveLicenseSet rdf:nodeID="Nab63afe52f1e4b309875af1ea705781f">
                 <spdx:member rdf:resource="http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#LicenseRef-3"/>
                 <spdx:member rdf:resource="http://spdx.org/licenses/LGPL-2.0-only"/>
               </spdx:ConjunctiveLicenseSet>
             </spdx:licenseDeclared>
           </spdx:Package>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 FileContributor: Modified by Paul Mundt lethal@linux-sh.org
 FileContributor: The Regents of the University of California
 
 ## Package Information
 PackageName: glibc
 SPDXID: SPDXRef-Package
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -216,25 +216,25 @@
     <licenseComments>The license for this project changed with the release of version x.y.  The version of the project included here post-dates the license change.</licenseComments>
     <licenseConcluded>LGPL-2.0-only OR LicenseRef-3</licenseConcluded>
     <licenseDeclared>LGPL-2.0-only AND LicenseRef-3</licenseDeclared>
     <licenseInfoFromFiles>GPL-2.0-only</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-2</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-1</licenseInfoFromFiles>
     <name>glibc</name>
-    <originator>Organization: ExampleCodeInspect (contact@example.com)</originator>
+    <originator>NOASSERTION</originator>
     <packageFileName>glibc-2.11.1.tar.gz</packageFileName>
     <packageVerificationCode>
       <packageVerificationCodeExcludedFiles>./package.spdx</packageVerificationCodeExcludedFiles>
       <packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</packageVerificationCodeValue>
     </packageVerificationCode>
     <primaryPackagePurpose>SOURCE</primaryPackagePurpose>
     <releaseDate>2012-01-29T18:30:22Z</releaseDate>
     <sourceInfo>uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.</sourceInfo>
     <summary>GNU C library.</summary>
-    <supplier>NOASSERTION</supplier>
+    <supplier>Organization: ExampleCodeInspect (contact@example.com)</supplier>
     <validUntilDate>2014-01-29T18:30:22Z</validUntilDate>
   </packages>
   <files>
     <SPDXID>SPDXRef-DoapSource</SPDXID>
     <checksums>
       <algorithm>SHA1</algorithm>
       <checksumValue>2fd4e1c67a2d28fced849ee1bb76e7391b93eb12</checksumValue>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -299,25 +299,25 @@
   licenseConcluded: LGPL-2.0-only OR LicenseRef-3
   licenseDeclared: LGPL-2.0-only AND LicenseRef-3
   licenseInfoFromFiles:
   - GPL-2.0-only
   - LicenseRef-2
   - LicenseRef-1
   name: glibc
-  originator: 'Organization: ExampleCodeInspect (contact@example.com)'
+  originator: NOASSERTION
   packageFileName: glibc-2.11.1.tar.gz
   packageVerificationCode:
     packageVerificationCodeExcludedFiles:
     - ./package.spdx
     packageVerificationCodeValue: d6a770ba38583ed4bb4525bd96e50461655d2758
   primaryPackagePurpose: SOURCE
   releaseDate: '2012-01-29T18:30:22Z'
   sourceInfo: uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.
   summary: GNU C library.
-  supplier: NOASSERTION
+  supplier: 'Organization: ExampleCodeInspect (contact@example.com)'
   validUntilDate: '2014-01-29T18:30:22Z'
 relationships:
 - relatedSpdxElement: SPDXRef-Package
   relationshipType: CONTAINS
   spdxElementId: SPDXRef-DOCUMENT
 - relatedSpdxElement: DocumentRef-spdx-tool-1.2:SPDXRef-ToolsElement
   relationshipType: COPY_OF
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985207100591715%*

 * *Differences: {"'packages'": "{0: {'originator': 'NOASSERTION', 'supplier': 'Organization: ExampleCodeInspect "*

 * *               "(contact@example.com)'}}"}*

```diff
@@ -260,27 +260,27 @@
             "licenseDeclared": "(LGPL-2.0-only AND LicenseRef-3)",
             "licenseInfoFromFiles": [
                 "GPL-2.0-only",
                 "LicenseRef-2",
                 "LicenseRef-1"
             ],
             "name": "glibc",
-            "originator": "Organization: ExampleCodeInspect (contact@example.com)",
+            "originator": "NOASSERTION",
             "packageFileName": "glibc-2.11.1.tar.gz",
             "packageVerificationCode": {
                 "packageVerificationCodeExcludedFiles": [
                     "./package.spdx"
                 ],
                 "packageVerificationCodeValue": "d6a770ba38583ed4bb4525bd96e50461655d2758"
             },
             "primaryPackagePurpose": "SOURCE",
             "releaseDate": "2012-01-29T18:30:22Z",
             "sourceInfo": "uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.",
             "summary": "GNU C library.",
-            "supplier": "NOASSERTION",
+            "supplier": "Organization: ExampleCodeInspect (contact@example.com)",
             "validUntilDate": "2014-01-29T18:30:22Z",
             "versionInfo": "2.11.1"
         }
     ],
     "snippets": [
         {
             "SPDXID": "SPDXRef-Snippet",
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 FileContributor: The Regents of the University of California
 
 ## Package Information
 PackageName: glibc
 SPDXID: SPDXRef-Package
 PackageVersion: 2.11.1
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 1% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -216,25 +216,25 @@
     <licenseComments>The license for this project changed with the release of version x.y.  The version of the project included here post-dates the license change.</licenseComments>
     <licenseConcluded>LGPL-2.0-only OR LicenseRef-3</licenseConcluded>
     <licenseDeclared>LGPL-2.0-only AND LicenseRef-3</licenseDeclared>
     <licenseInfoFromFiles>GPL-2.0-only</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-2</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-1</licenseInfoFromFiles>
     <name>glibc</name>
-    <originator>Organization: ExampleCodeInspect (contact@example.com)</originator>
+    <originator>NOASSERTION</originator>
     <packageFileName>glibc-2.11.1.tar.gz</packageFileName>
     <packageVerificationCode>
       <packageVerificationCodeExcludedFiles>./package.spdx</packageVerificationCodeExcludedFiles>
       <packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</packageVerificationCodeValue>
     </packageVerificationCode>
     <primaryPackagePurpose>SOURCE</primaryPackagePurpose>
     <releaseDate>2012-01-29T18:30:22Z</releaseDate>
     <sourceInfo>uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.</sourceInfo>
     <summary>GNU C library.</summary>
-    <supplier>NOASSERTION</supplier>
+    <supplier>Organization: ExampleCodeInspect (contact@example.com)</supplier>
     <validUntilDate>2014-01-29T18:30:22Z</validUntilDate>
     <versionInfo>2.11.1</versionInfo>
   </packages>
   <files>
     <SPDXID>SPDXRef-DoapSource</SPDXID>
     <checksums>
       <algorithm>SHA1</algorithm>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -299,25 +299,25 @@
   licenseConcluded: LGPL-2.0-only OR LicenseRef-3
   licenseDeclared: LGPL-2.0-only AND LicenseRef-3
   licenseInfoFromFiles:
   - GPL-2.0-only
   - LicenseRef-2
   - LicenseRef-1
   name: glibc
-  originator: 'Organization: ExampleCodeInspect (contact@example.com)'
+  originator: NOASSERTION
   packageFileName: glibc-2.11.1.tar.gz
   packageVerificationCode:
     packageVerificationCodeExcludedFiles:
     - ./package.spdx
     packageVerificationCodeValue: d6a770ba38583ed4bb4525bd96e50461655d2758
   primaryPackagePurpose: SOURCE
   releaseDate: '2012-01-29T18:30:22Z'
   sourceInfo: uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.
   summary: GNU C library.
-  supplier: NOASSERTION
+  supplier: 'Organization: ExampleCodeInspect (contact@example.com)'
   validUntilDate: '2014-01-29T18:30:22Z'
   versionInfo: 2.11.1
 snippets:
 - SPDXID: SPDXRef-Snippet
   comment: This snippet was identified as significant and highlighted in this Apache-2.0
     file, when a commercial scanner identified it as being derived from file foo.c
     in package xyz which is licensed under GPL-2.0.
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997942386831276%*

 * *Differences: {"'packages'": "{0: {'originator': 'NOASSERTION'}}"}*

```diff
@@ -280,15 +280,15 @@
             "licenseDeclared": "(LGPL-2.0-only AND LicenseRef-3)",
             "licenseInfoFromFiles": [
                 "GPL-2.0-only",
                 "LicenseRef-2",
                 "LicenseRef-1"
             ],
             "name": "glibc",
-            "originator": "Organization: ExampleCodeInspect (contact@example.com)",
+            "originator": "NOASSERTION",
             "packageFileName": "glibc-2.11.1.tar.gz",
             "packageVerificationCode": {
                 "packageVerificationCodeExcludedFiles": [
                     "./package.spdx"
                 ],
                 "packageVerificationCodeValue": "d6a770ba38583ed4bb4525bd96e50461655d2758"
             },
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml`

```diff
@@ -294,15 +294,15 @@
               <spdx:Checksum rdf:nodeID="N4a15c1ba914149179a3102e6fe30b07f">
                 <spdx:checksumValue>aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706</spdx:checksumValue>
                 <spdx:algorithm rdf:resource="http://spdx.org/rdf/terms#checksumAlgorithm_blake2b384"/>
               </spdx:Checksum>
             </spdx:checksum>
             <spdx:attributionText>The GNU C Library is free software.  See the file COPYING.LIB for copying conditions, and LICENSES for notices about a few contributions that require these additional notices to be distributed.  License copyright years may be listed using range notation, e.g., 1996-2015, indicating that every year in the range, inclusive, is a copyrightable year that would otherwise be listed individually.</spdx:attributionText>
             <spdx:versionInfo>2.11.1</spdx:versionInfo>
-            <spdx:originator>Organization: ExampleCodeInspect (contact@example.com)</spdx:originator>
+            <spdx:originator>NOASSERTION</spdx:originator>
             <spdx:licenseComments>The license for this project changed with the release of version x.y.  The version of the project included here post-dates the license change.</spdx:licenseComments>
             <spdx:validUntilDate>2014-01-29T18:30:22Z</spdx:validUntilDate>
             <spdx:packageFileName>glibc-2.11.1.tar.gz</spdx:packageFileName>
             <spdx:packageVerificationCode>
               <spdx:PackageVerificationCode rdf:nodeID="Nbd27d2dfb85e44db99ba7947ddced5d9">
                 <spdx:packageVerificationCodeExcludedFile>./package.spdx</spdx:packageVerificationCodeExcludedFile>
                 <spdx:packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</spdx:packageVerificationCodeValue>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ## Package Information
 PackageName: glibc
 SPDXID: SPDXRef-Package
 PackageVersion: 2.11.1
 PackageFileName: glibc-2.11.1.tar.gz
 PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 1% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -216,15 +216,15 @@
     <licenseComments>The license for this project changed with the release of version x.y.  The version of the project included here post-dates the license change.</licenseComments>
     <licenseConcluded>LGPL-2.0-only OR LicenseRef-3</licenseConcluded>
     <licenseDeclared>LGPL-2.0-only AND LicenseRef-3</licenseDeclared>
     <licenseInfoFromFiles>GPL-2.0-only</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-2</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-1</licenseInfoFromFiles>
     <name>glibc</name>
-    <originator>Organization: ExampleCodeInspect (contact@example.com)</originator>
+    <originator>NOASSERTION</originator>
     <packageFileName>glibc-2.11.1.tar.gz</packageFileName>
     <packageVerificationCode>
       <packageVerificationCodeExcludedFiles>./package.spdx</packageVerificationCodeExcludedFiles>
       <packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</packageVerificationCodeValue>
     </packageVerificationCode>
     <primaryPackagePurpose>SOURCE</primaryPackagePurpose>
     <releaseDate>2012-01-29T18:30:22Z</releaseDate>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
   licenseConcluded: LGPL-2.0-only OR LicenseRef-3
   licenseDeclared: LGPL-2.0-only AND LicenseRef-3
   licenseInfoFromFiles:
   - GPL-2.0-only
   - LicenseRef-2
   - LicenseRef-1
   name: glibc
-  originator: 'Organization: ExampleCodeInspect (contact@example.com)'
+  originator: 'NOASSERTION'
   packageFileName: glibc-2.11.1.tar.gz
   packageVerificationCode:
     packageVerificationCodeExcludedFiles:
     - ./package.spdx
     packageVerificationCodeValue: d6a770ba38583ed4bb4525bd96e50461655d2758
   primaryPackagePurpose: SOURCE
   releaseDate: '2012-01-29T18:30:22Z'
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987654320987654%*

 * *Differences: {"'packages'": "{0: {'originator': 'NOASSERTION', 'supplier': 'Organization: ExampleCodeInspect "*

 * *               "(contact@example.com)'}}"}*

```diff
@@ -280,27 +280,27 @@
             "licenseDeclared": "(LGPL-2.0-only AND LicenseRef-3)",
             "licenseInfoFromFiles": [
                 "GPL-2.0-only",
                 "LicenseRef-2",
                 "LicenseRef-1"
             ],
             "name": "glibc",
-            "originator": "Organization: ExampleCodeInspect (contact@example.com)",
+            "originator": "NOASSERTION",
             "packageFileName": "glibc-2.11.1.tar.gz",
             "packageVerificationCode": {
                 "packageVerificationCodeExcludedFiles": [
                     "./package.spdx"
                 ],
                 "packageVerificationCodeValue": "d6a770ba38583ed4bb4525bd96e50461655d2758"
             },
             "primaryPackagePurpose": "SOURCE",
             "releaseDate": "2012-01-29T18:30:22Z",
             "sourceInfo": "uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.",
             "summary": "GNU C library.",
-            "supplier": "NOASSERTION",
+            "supplier": "Organization: ExampleCodeInspect (contact@example.com)",
             "validUntilDate": "2014-01-29T18:30:22Z",
             "versionInfo": "2.11.1"
         }
     ],
     "relationships": [
         {
             "relatedSpdxElement": "SPDXRef-Package",
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml`

```diff
@@ -302,15 +302,15 @@
               <spdx:ExternalRef rdf:nodeID="N6f077514d2c24828bb45bff322ba61b3">
                 <spdx:referenceType rdf:resource="http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#LocationRef-acmeforge"/>
                 <rdfs:comment>This is the external ref for Acme</rdfs:comment>
                 <spdx:referenceCategory rdf:resource="http://spdx.org/rdf/terms#referenceCategory_other"/>
                 <spdx:referenceLocator>acmecorp/acmenator/4.1.3-alpha</spdx:referenceLocator>
               </spdx:ExternalRef>
             </spdx:externalRef>
-            <spdx:supplier>NOASSERTION</spdx:supplier>
+            <spdx:supplier>Organization: ExampleCodeInspect (contact@example.com)</spdx:supplier>
             <spdx:checksum>
               <spdx:Checksum rdf:nodeID="N98510266a7284a1686da4e459dd5e58b">
                 <spdx:checksumValue>aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706</spdx:checksumValue>
                 <spdx:algorithm rdf:resource="http://spdx.org/rdf/terms#checksumAlgorithm_blake2b384"/>
               </spdx:Checksum>
             </spdx:checksum>
             <spdx:checksum>
@@ -346,15 +346,15 @@
             <spdx:packageVerificationCode>
               <spdx:PackageVerificationCode rdf:nodeID="Ne806fa90587c4eb7a4b5e7139d58671f">
                 <spdx:packageVerificationCodeExcludedFile>./package.spdx</spdx:packageVerificationCodeExcludedFile>
                 <spdx:packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</spdx:packageVerificationCodeValue>
               </spdx:PackageVerificationCode>
             </spdx:packageVerificationCode>
             <spdx:summary>GNU C library.</spdx:summary>
-            <spdx:originator>Organization: ExampleCodeInspect (contact@example.com)</spdx:originator>
+            <spdx:originator>NOASSERTION</spdx:originator>
             <spdx:builtDate>2011-01-29T18:30:22Z</spdx:builtDate>
             <spdx:licenseDeclared>
               <spdx:ConjunctiveLicenseSet rdf:nodeID="N45c3c34ce93d4d769c3edee387495c95">
                 <spdx:member rdf:resource="http://spdx.org/licenses/LGPL-2.0-only"/>
                 <spdx:member rdf:resource="http://spdx.org/spdxdocs/spdx-example-444504E0-4F89-41D3-9A0C-0305E82C3301#LicenseRef-3"/>
               </spdx:ConjunctiveLicenseSet>
             </spdx:licenseDeclared>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 FileContributor: The Regents of the University of California
 
 ## Package Information
 PackageName: glibc
 SPDXID: SPDXRef-Package
 PackageVersion: 2.11.1
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml`

 * *Files 0% similar despite different names*

#### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml`

```diff
@@ -216,25 +216,25 @@
     <licenseComments>The license for this project changed with the release of version x.y.  The version of the project included here post-dates the license change.</licenseComments>
     <licenseConcluded>LGPL-2.0-only OR LicenseRef-3</licenseConcluded>
     <licenseDeclared>LGPL-2.0-only AND LicenseRef-3</licenseDeclared>
     <licenseInfoFromFiles>GPL-2.0-only</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-2</licenseInfoFromFiles>
     <licenseInfoFromFiles>LicenseRef-1</licenseInfoFromFiles>
     <name>glibc</name>
-    <originator>Organization: ExampleCodeInspect (contact@example.com)</originator>
+    <originator>NOASSERTION</originator>
     <packageFileName>glibc-2.11.1.tar.gz</packageFileName>
     <packageVerificationCode>
       <packageVerificationCodeExcludedFiles>./package.spdx</packageVerificationCodeExcludedFiles>
       <packageVerificationCodeValue>d6a770ba38583ed4bb4525bd96e50461655d2758</packageVerificationCodeValue>
     </packageVerificationCode>
     <primaryPackagePurpose>SOURCE</primaryPackagePurpose>
     <releaseDate>2012-01-29T18:30:22Z</releaseDate>
     <sourceInfo>uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.</sourceInfo>
     <summary>GNU C library.</summary>
-    <supplier>NOASSERTION</supplier>
+    <supplier>Organization: ExampleCodeInspect (contact@example.com)</supplier>
     <validUntilDate>2014-01-29T18:30:22Z</validUntilDate>
     <versionInfo>2.11.1</versionInfo>
   </packages>
   <files>
     <SPDXID>SPDXRef-DoapSource</SPDXID>
     <checksums>
       <algorithm>SHA1</algorithm>
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -299,25 +299,25 @@
   licenseConcluded: LGPL-2.0-only OR LicenseRef-3
   licenseDeclared: LGPL-2.0-only AND LicenseRef-3
   licenseInfoFromFiles:
   - GPL-2.0-only
   - LicenseRef-2
   - LicenseRef-1
   name: glibc
-  originator: 'Organization: ExampleCodeInspect (contact@example.com)'
+  originator: NOASSERTION
   packageFileName: glibc-2.11.1.tar.gz
   packageVerificationCode:
     packageVerificationCodeExcludedFiles:
     - ./package.spdx
     packageVerificationCodeValue: d6a770ba38583ed4bb4525bd96e50461655d2758
   primaryPackagePurpose: SOURCE
   releaseDate: '2012-01-29T18:30:22Z'
   sourceInfo: uses glibc-2_11-branch from git://sourceware.org/git/glibc.git.
   summary: GNU C library.
-  supplier: NOASSERTION
+  supplier: 'Organization: ExampleCodeInspect (contact@example.com)'
   validUntilDate: '2014-01-29T18:30:22Z'
   versionInfo: 2.11.1
 relationships:
 - relatedSpdxElement: SPDXRef-Package
   relationshipType: CONTAINS
   spdxElementId: SPDXRef-DOCUMENT
 - relatedSpdxElement: DocumentRef-spdx-tool-1.2:SPDXRef-ToolsElement
```

### Comparing `ntia_conformance_checker-1.1.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml` & `ntia_conformance_checker-2.0.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/other_tests/SPDXSimpleTag.tag` & `ntia_conformance_checker-2.0.0/tests/data/other_tests/SPDXSimpleTag.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/data/other_tests/test_components_without_functions.spdx` & `ntia_conformance_checker-2.0.0/tests/data/other_tests/test_components_without_functions.spdx`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 compatible system run time libraries.</text>
 
 ## Package Information
 PackageName: glibc
 SPDXID: SPDXRef-Package
 PackageVersion: 2.4.57+dfsg-3+deb11u1
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
@@ -52,16 +52,16 @@
 
 
 ## Package Information without name
 PackageName: 
 SPDXID: SPDXRef-Package1
 PackageVersion: 2.4.57+dfsg-3+deb11u1
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
@@ -85,16 +85,16 @@
 BuiltDate: 2011-01-29T18:30:22Z
 ValidUntilDate: 2014-01-29T18:30:22Z
 
 ## Package Information without version
 PackageName: glibc-no-version-1
 SPDXID: SPDXRef-Package2
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
@@ -118,16 +118,16 @@
 BuiltDate: 2011-01-29T18:30:22Z
 ValidUntilDate: 2014-01-29T18:30:22Z
 
 ## Package Information without version
 PackageName: glibc-no-version-2
 SPDXID: SPDXRef-Package3
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
@@ -184,16 +184,16 @@
 ValidUntilDate: 2014-01-29T18:30:22Z
 
 ## Package Information without identiyer
 PackageName: glibc-no-identifier
 SPDXID: SPDXRef-Package5
 PackageVersion: 2.4.57+dfsg-3+deb11u1
 PackageFileName: glibc-2.11.1.tar.gz
-PackageSupplier: NOASSERTION
-PackageOriginator: Organization: ExampleCodeInspect (contact@example.com)
+PackageSupplier: Organization: ExampleCodeInspect (contact@example.com)
+PackageOriginator: NOASSERTION
 PackageDownloadLocation: http://ftp.gnu.org/gnu/glibc/glibc-ports-2.15.tar.gz
 FilesAnalyzed: true
 PackageVerificationCode: d6a770ba38583ed4bb4525bd96e50461655d2758 (excludes: ./package.spdx)
 PackageChecksum: MD5: 624c1abb3664f4b35547e7c73864ad24
 PackageChecksum: SHA1: 85ed0817af83a24ad8da68c2b5094de69833983c
 PackageChecksum: SHA256: 11b6d3ee554eedf79299905a98f9b9a04e498210b59f15094c916c91d150efcd
 PackageChecksum: BLAKE2b-384: aaabd89c926ab525c242e6621f2f5fa73aa4afe3d9e24aed727faaadd6af38b620bdb623dd2b4788b1c8086984af8706
```

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/OpenEmbedded/time.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/OpenEmbedded/time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Philips/keyclock_sbom.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Philips/keyclock_sbom.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/REA/AppBOM-inationVDR.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/REA/AppBOM-inationVDR.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/REA/PyYamlVDR.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/REA/PyYamlVDR.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/appbomination_container.spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/appbomination_container.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/app.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/app.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/build.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/build.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml` & `ntia_conformance_checker-2.0.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/App-BOM-ination.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/App-BOM-ination.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/gnu_time-v1.9.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/gnu_time-v1.9.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/serve-1.0.0.json` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/serve-1.0.0.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag` & `ntia_conformance_checker-2.0.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-1.1.0/tests/test_checker.py` & `ntia_conformance_checker-2.0.0/tests/test_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,44 +21,44 @@
     assert sbom.doc_author
     assert sbom.doc_timestamp
     assert sbom.dependency_relationships
     assert not sbom.components_without_names
     assert not sbom.components_without_versions
     assert not sbom.components_without_suppliers
     assert not sbom.components_without_identifiers
-    assert sbom.ntia_mininum_elements_compliant
+    assert sbom.ntia_minimum_elements_compliant
 
 
 dirname = os.path.join(os.path.dirname(__file__), "data", "missing_author_name")
 test_files_missing_author_name = [
     os.path.join(dirname, fn) for fn in os.listdir(dirname)
 ]
 
 
 @pytest.mark.parametrize("test_file", test_files_missing_author_name)
 def test_sbomchecker_missing_author_name(test_file):
     """The parser from spdx-tools will raise an SPDXParsingError if
     the document does not contain a creator."""
     sbom_check = sbom_checker.SbomChecker(test_file)
 
-    assert not sbom_check.ntia_mininum_elements_compliant
+    assert not sbom_check.ntia_minimum_elements_compliant
     assert sbom_check.parsing_error
 
 
 dirname = os.path.join(os.path.dirname(__file__), "data", "missing_timestamp")
 test_files_missing_timestamp = [os.path.join(dirname, fn) for fn in os.listdir(dirname)]
 
 
 @pytest.mark.parametrize("test_file", test_files_missing_timestamp)
 def test_sbomchecker_missing_timestamp(test_file):
     """The parser from spdx-tools will raise an SPDXParsingError if
     the document does not contain a created date."""
     sbom_check = sbom_checker.SbomChecker(test_file)
 
-    assert not sbom_check.ntia_mininum_elements_compliant
+    assert not sbom_check.ntia_minimum_elements_compliant
     assert sbom_check.parsing_error
 
 
 dirname = os.path.join(
     os.path.dirname(__file__), "data", "missing_dependency_relationships"
 )
 test_files_missing_dependency_relationships = [
@@ -74,15 +74,15 @@
     assert sbom.doc_author
     assert sbom.doc_timestamp
     assert not sbom.dependency_relationships
     assert not sbom.components_without_names
     assert not sbom.components_without_versions
     assert not sbom.components_without_suppliers
     assert not sbom.components_without_identifiers
-    assert not sbom.ntia_mininum_elements_compliant
+    assert not sbom.ntia_minimum_elements_compliant
 
 
 dirname = os.path.join(os.path.dirname(__file__), "data", "missing_component_version")
 test_files_missing_component_version = [
     os.path.join(dirname, fn) for fn in os.listdir(dirname)
 ]
 
@@ -95,15 +95,15 @@
     assert sbom.doc_author
     assert sbom.doc_timestamp
     assert sbom.dependency_relationships
     assert not sbom.components_without_names
     TestCase().assertCountEqual(sbom.components_without_versions, ["glibc"])
     assert not sbom.components_without_suppliers
     assert not sbom.components_without_identifiers
-    assert not sbom.ntia_mininum_elements_compliant
+    assert not sbom.ntia_minimum_elements_compliant
 
 
 dirname = os.path.join(os.path.dirname(__file__), "data", "missing_supplier_name")
 files = [os.path.join(dirname, fn) for fn in os.listdir(dirname)]
 
 
 @pytest.mark.parametrize("test_file", files)
@@ -112,32 +112,34 @@
     assert sbom.file == test_file
     assert sbom.doc_version
     assert sbom.doc_author
     assert sbom.doc_timestamp
     assert sbom.dependency_relationships
     assert not sbom.components_without_names
     assert not sbom.components_without_versions
-    TestCase().assertCountEqual(sbom.components_without_suppliers, ["Jena", "Saxon"])
+    TestCase().assertCountEqual(
+        sbom.components_without_suppliers, ["glibc", "Jena", "Saxon"]
+    )
     assert not sbom.components_without_identifiers
-    assert not sbom.ntia_mininum_elements_compliant
+    assert not sbom.ntia_minimum_elements_compliant
 
 
 dirname = os.path.join(os.path.dirname(__file__), "data", "missing_unique_identifiers")
 test_files_missing_unique_identifiers = [
     os.path.join(dirname, fn) for fn in os.listdir(dirname)
 ]
 
 
 @pytest.mark.parametrize("test_file", test_files_missing_unique_identifiers)
 def test_sbomchecker_missing_unique_identifiers(test_file):
     """The parser from spdx-tools will raise an SPDXParsingError if
     the document contains an element without SPDXID."""
     sbom_check = sbom_checker.SbomChecker(test_file)
 
-    assert not sbom_check.ntia_mininum_elements_compliant
+    assert not sbom_check.ntia_minimum_elements_compliant
     assert sbom_check.parsing_error
 
 
 def test_sbomchecker_tern_photon_example():
     """Check that SBOM from Tern for Photon has an author."""
     test_file = os.path.join(
         os.path.dirname(__file__), "data", "SPDXSBOMExampleTests", "photon.spdx.tag"
```

