# Comparing `tmp/pymilvus-2.4.0.tar.gz` & `tmp/pymilvus-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.4.0.tar", last modified: Wed Mar 20 10:41:34 2024, max compression
+gzip compressed data, was "pymilvus-2.4.1.tar", last modified: Mon Apr 29 11:33:42 2024, max compression
```

## Comparing `pymilvus-2.4.0.tar` & `pymilvus-2.4.1.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:34.002564 pymilvus-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.970564 pymilvus-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/enhancement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/check_milvus_proto.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/code_checker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/doc_update_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/nightly_ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.github/workflows/release_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 10:41:19.000000 pymilvus-2.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-20 10:41:19.000000 pymilvus-2.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-20 10:41:19.000000 pymilvus-2.4.0/CONTRIBUTING_CN.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-20 10:41:19.000000 pymilvus-2.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-03-20 10:41:19.000000 pymilvus-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-20 10:41:19.000000 pymilvus-2.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-20 10:41:19.000000 pymilvus-2.4.0/OWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-20 10:41:34.002564 pymilvus-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-20 10:41:19.000000 pymilvus-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-20 10:41:19.000000 pymilvus-2.4.0/_version_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-03-20 10:41:19.000000 pymilvus-2.4.0/check_proto_product.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.966564 pymilvus-2.4.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.966564 pymilvus-2.4.0/ci/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/ci/docker/milvus/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-20 10:41:19.000000 pymilvus-2.4.0/ci/docker/milvus/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/ci/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-03-20 10:41:19.000000 pymilvus-2.4.0/ci/scripts/docker_image_find_tag.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.974564 pymilvus-2.4.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.978564 pymilvus-2.4.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/_templates/autosummaryclass.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/about.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.978564 pymilvus-2.4.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/collection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/future.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/milvus_index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/partition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/search.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/api/utility.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/param.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.978564 pymilvus-2.4.0/docs/source/res/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/res/Intro_to_Indexes.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/res/about_documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-03-20 10:41:19.000000 pymilvus-2.4.0/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.986564 pymilvus-2.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/bfloat16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/binary_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.986564 pymilvus-2.4.0/examples/cert/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/cert/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/cert/client.key
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/cert/client.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/cert/server.pem
--rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.986564 pymilvus-2.4.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/data/train_embeddings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/dynamic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_bulkinsert_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_bulkinsert_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_bulkwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_gpu_brute_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_gpu_cagra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_tls1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/example_tls2.py
--rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/films.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/float16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/fuzzy_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_hybrid_sparse_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_milvus.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_milvus_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_milvus_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hello_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/hybrid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/inverted_index_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.990564 pymilvus-2.4.0/examples/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/customize_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/customize_schema_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/index_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/non_ascii_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/simple_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/milvus_client/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/multithreading_hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/old_style_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/old_style_example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/old_style_example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/old_style_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/role_and_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-20 10:41:19.000000 pymilvus-2.4.0/examples/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.990564 pymilvus-2.4.0/pymilvus/
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.990564 pymilvus-2.4.0/pymilvus/bulk_writer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/local_bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/bulk_writer/remote_bulk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.994564 pymilvus-2.4.0/pymilvus/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/asynch.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/entity_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    71852 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    46621 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/singleton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59057 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.998564 pymilvus-2.4.0/pymilvus/grpc_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28693 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/feder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/feder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    89954 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   102182 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   135246 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/msg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/msg_pb2.pyi
--rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/python_gen.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/rg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/rg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/grpc_gen/schema_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.998564 pymilvus-2.4.0/pymilvus/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/milvus_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/milvus_client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    35578 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/milvus_client/milvus_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.998564 pymilvus-2.4.0/pymilvus/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:33.998564 pymilvus-2.4.0/pymilvus/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65894 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    23292 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    48841 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/orm/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pymilvus/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:34.002564 pymilvus-2.4.0/pymilvus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-20 10:41:33.000000 pymilvus-2.4.0/pymilvus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-20 10:41:33.000000 pymilvus-2.4.0/pymilvus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:41:33.000000 pymilvus-2.4.0/pymilvus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-20 10:41:33.000000 pymilvus-2.4.0/pymilvus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 10:41:33.000000 pymilvus-2.4.0/pymilvus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-03-20 10:41:19.000000 pymilvus-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-20 10:41:19.000000 pymilvus-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:41:34.002564 pymilvus-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-20 10:41:19.000000 pymilvus-2.4.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:41:34.002564 pymilvus-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/mock_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14863 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-20 10:41:19.000000 pymilvus-2.4.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.706213 pymilvus-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/enhancement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/check_milvus_proto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/code_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/doc_update_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/nightly_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/release_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-29 11:33:31.000000 pymilvus-2.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-29 11:33:31.000000 pymilvus-2.4.1/CONTRIBUTING_CN.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 11:33:31.000000 pymilvus-2.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-29 11:33:31.000000 pymilvus-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 11:33:31.000000 pymilvus-2.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 11:33:31.000000 pymilvus-2.4.1/OWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-29 11:33:42.742213 pymilvus-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-29 11:33:31.000000 pymilvus-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-29 11:33:31.000000 pymilvus-2.4.1/_version_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-04-29 11:33:31.000000 pymilvus-2.4.1/check_proto_product.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.702213 pymilvus-2.4.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.702213 pymilvus-2.4.1/ci/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/ci/docker/milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 11:33:31.000000 pymilvus-2.4.1/ci/docker/milvus/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/ci/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-04-29 11:33:31.000000 pymilvus-2.4.1/ci/scripts/docker_image_find_tag.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/_templates/autosummaryclass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/about.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/future.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/milvus_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/partition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/utility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/param.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/res/Intro_to_Indexes.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/res/about_documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/bfloat16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/binary_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/cert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/client.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/server.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/data/train_embeddings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/dynamic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkinsert_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkinsert_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_gpu_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_gpu_cagra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_tls1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_tls2.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/films.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/float16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/fuzzy_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_hybrid_sparse_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hybrid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/inverted_index_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.726213 pymilvus-2.4.1/examples/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/customize_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/customize_schema_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/index_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/non_ascii_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/simple_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/multithreading_hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/resource_group_declarative_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/role_and_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.726213 pymilvus-2.4.1/pymilvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.730213 pymilvus-2.4.1/pymilvus/bulk_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/local_bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/remote_bulk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.734213 pymilvus-2.4.1/pymilvus/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/asynch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/entity_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72352 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46903 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/singleton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59505 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.734213 pymilvus-2.4.1/pymilvus/grpc_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    89972 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102932 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   136781 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/python_gen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35578 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/milvus_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66166 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23292 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23015 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50438 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/pymilvus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 11:33:31.000000 pymilvus-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:33:42.742213 pymilvus-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/mock_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/utils.py
```

### Comparing `pymilvus-2.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/ISSUE_TEMPLATE/enhancement.yaml` & `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/enhancement.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/mergify.yml` & `pymilvus-2.4.1/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.4.1/.github/workflows/check_milvus_proto.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Check proto on pull request
 
 on:
   pull_request:
     branches:
-      - master
+      - 2.4
 
 jobs:
   build:
     name: Run Check Proto
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `pymilvus-2.4.0/.github/workflows/doc_update_event.yml` & `pymilvus-2.4.1/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/workflows/nightly_ci.yml` & `pymilvus-2.4.1/.github/workflows/nightly_ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 jobs:
   nightly:
     name: Run Nightly CI
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7]
+        python-version: [3.11]
     env:
       IMAGE_REPO: "milvusdb"
       TAG_PREFIX: "master-"
     steps:
     - uses: actions/checkout@v4
 
     - name: Get the latest of Milvus dev image tag
```

### Comparing `pymilvus-2.4.0/.github/workflows/publish_dev_package.yml` & `pymilvus-2.4.1/.github/workflows/publish_dev_package.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Publish Python 🐍 distributions 📦 to TestPyPI
 
 on:
   push:
     branches:
-      - 'master'
+      - '2.4'
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to TestPyPI
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `pymilvus-2.4.0/.github/workflows/publish_on_release.yml` & `pymilvus-2.4.1/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/.github/workflows/pull_request.yml` & `pymilvus-2.4.1/.github/workflows/pull_request.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Test on pull request
 
 on:
   pull_request:
     branches:
-      - master
+      - 2.4
 
 jobs:
   build:
     name: Run Python Tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
@@ -24,13 +24,12 @@
       - name: Fetch tags
         run: |
           git fetch --prune --unshallow --tags
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -e .
-          pip install -r test_requirements.txt
+          pip install -e ".[test]"
 
       - name: Test with pytest
         run: |
           make unittest
```

### Comparing `pymilvus-2.4.0/.github/workflows/release_event.yml` & `pymilvus-2.4.1/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/CONTRIBUTING.md` & `pymilvus-2.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/CONTRIBUTING_CN.md` & `pymilvus-2.4.1/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/LICENSE` & `pymilvus-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/Makefile` & `pymilvus-2.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/PKG-INFO` & `pymilvus-2.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,16 +16,24 @@
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
 Requires-Dist: requests
 Requires-Dist: minio>=7.0.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: azure-storage-blob
+Requires-Dist: scipy
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
+Provides-Extra: test
+Requires-Dist: pytest>=5.3.4; extra == "test"
+Requires-Dist: pytest-cov>=2.8.1; extra == "test"
+Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
+Requires-Dist: grpcio-testing; extra == "test"
+Requires-Dist: ruff>=0.3.3; extra == "test"
+Requires-Dist: black; extra == "test"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
 [![Downloads](https://static.pepy.tech/badge/pymilvus/month)](https://pepy.tech/project/pymilvus)
@@ -48,22 +56,24 @@
 |:-----:|:-----:|
 | 1.0.\* | 1.0.1 |
 | 1.1.\* | 1.1.2 |
 | 2.0.\* | 2.0.2 |
 | 2.1.\* | 2.1.3 |
 | 2.2.\* | 2.2.15 |
 | 2.3.\* | 2.3.7 |
+| 2.4.\* | 2.4.0 |
 
 
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
+$ pip3 install pymilvus[model] # for milvus-model
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -104,23 +114,36 @@
 A4.
 ```shell
 make lint
 ```
 
 Q5. How to fix the coding styles?
 
-Q5
+A5
 ```shell
 make format
 ```
 
+Q6. How to run unittests?
+
+A6
+```shell
+$ pip install ".[test]"
+$ make unittest
+```
+Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+
+A7
+```shell
+$ pip install "pymilvus[model]"
+```
 
 ## Documentation
 
-Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.3.x/About.md
+Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.4.x/About.md
 
 ## Developing package releases
 
 The commits on the development branch of each version will be packaged and uploaded to [Test PyPI](https://test.pypi.org/).
 
 The package name generated by the development branch is x.y.z.rc<dist>, where <dist> is the number of commits that differ from the most recent release.
```

### Comparing `pymilvus-2.4.0/README.md` & `pymilvus-2.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 |:-----:|:-----:|
 | 1.0.\* | 1.0.1 |
 | 1.1.\* | 1.1.2 |
 | 2.0.\* | 2.0.2 |
 | 2.1.\* | 2.1.3 |
 | 2.2.\* | 2.2.15 |
 | 2.3.\* | 2.3.7 |
+| 2.4.\* | 2.4.0 |
 
 
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
+$ pip3 install pymilvus[model] # for milvus-model
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -79,23 +81,36 @@
 A4.
 ```shell
 make lint
 ```
 
 Q5. How to fix the coding styles?
 
-Q5
+A5
 ```shell
 make format
 ```
 
+Q6. How to run unittests?
+
+A6
+```shell
+$ pip install ".[test]"
+$ make unittest
+```
+Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+
+A7
+```shell
+$ pip install "pymilvus[model]"
+```
 
 ## Documentation
 
-Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.3.x/About.md
+Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.4.x/About.md
 
 ## Developing package releases
 
 The commits on the development branch of each version will be packaged and uploaded to [Test PyPI](https://test.pypi.org/).
 
 The package name generated by the development branch is x.y.z.rc<dist>, where <dist> is the number of commits that differ from the most recent release.
```

### Comparing `pymilvus-2.4.0/_version_helper.py` & `pymilvus-2.4.1/_version_helper.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/check_proto_product.sh` & `pymilvus-2.4.1/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.4.1/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.4.1/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/Makefile` & `pymilvus-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/README.md` & `pymilvus-2.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/make.bat` & `pymilvus-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/collection.rst` & `pymilvus-2.4.1/docs/source/api/collection.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/connections.rst` & `pymilvus-2.4.1/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/future.rst` & `pymilvus-2.4.1/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/milvus_index.rst` & `pymilvus-2.4.1/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/partition.rst` & `pymilvus-2.4.1/docs/source/api/partition.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/schema.rst` & `pymilvus-2.4.1/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/search.rst` & `pymilvus-2.4.1/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/api/utility.rst` & `pymilvus-2.4.1/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/conf.py` & `pymilvus-2.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/contribute.rst` & `pymilvus-2.4.1/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/faq.rst` & `pymilvus-2.4.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/index.rst` & `pymilvus-2.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/install.rst` & `pymilvus-2.4.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.4.1/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/res/about_documentation.md` & `pymilvus-2.4.1/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/results.rst` & `pymilvus-2.4.1/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/docs/source/tutorial.rst` & `pymilvus-2.4.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/bfloat16_example.py` & `pymilvus-2.4.1/examples/bfloat16_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,46 +16,42 @@
 
 def gen_bf16_vectors(num, dim):
     raw_vectors = []
     bf16_vectors = []
     for _ in range(num):
         raw_vector = [random.random() for _ in range(dim)]
         raw_vectors.append(raw_vector)
-        # bf16_vector = np.array(raw_vector, dtype=tf.bfloat16).view(np.uint8).tolist()
-        bf16_vector = tf.cast(raw_vector, dtype=tf.bfloat16).numpy().view(np.uint8).tolist()
-        bf16_vectors.append(bytes(bf16_vector))
+        bf16_vector = tf.cast(raw_vector, dtype=tf.bfloat16).numpy()
+        bf16_vectors.append(bf16_vector)
     return raw_vectors, bf16_vectors
 
 def bf16_vector_search():
     connections.connect()
 
     int64_field = FieldSchema(name="int64", dtype=DataType.INT64, is_primary=True, auto_id=True)
     dim = 128
     nb = 3000
     vector_field_name = "bfloat16_vector"
     bf16_vector = FieldSchema(name=vector_field_name, dtype=DataType.BFLOAT16_VECTOR, dim=dim)
     schema = CollectionSchema(fields=[int64_field, bf16_vector])
 
-    has = utility.has_collection("hello_milvus")
-    if has:
-        hello_milvus = Collection("hello_milvus_fp16")
-        hello_milvus.drop()
-    else:
-        hello_milvus = Collection("hello_milvus_fp16", schema)
+    if utility.has_collection("hello_milvus_fp16"):
+        utility.drop_collection("hello_milvus_fp16")
+    hello_milvus = Collection("hello_milvus_fp16", schema, consistency_level="Strong")
 
     _, vectors = gen_bf16_vectors(nb, dim)
+    hello_milvus.insert([vectors[:6]])
     rows = [
-        {vector_field_name: vectors[0]},
-        {vector_field_name: vectors[1]},
-        {vector_field_name: vectors[2]},
-        {vector_field_name: vectors[3]},
-        {vector_field_name: vectors[4]},
-        {vector_field_name: vectors[5]},
+        {vector_field_name: vectors[6]},
+        {vector_field_name: vectors[7]},
+        {vector_field_name: vectors[8]},
+        {vector_field_name: vectors[9]},
+        {vector_field_name: vectors[10]},
+        {vector_field_name: vectors[11]},
     ]
-
     hello_milvus.insert(rows)
     hello_milvus.flush()
 
     for i, index_type in enumerate(bf16_index_types):
         index_params = default_bf16_index_params[i]
         hello_milvus.create_index(vector_field_name,
                                   index_params={"index_type": index_type, "params": index_params, "metric_type": "L2"})
@@ -65,8 +61,8 @@
         print(res)
         hello_milvus.release()
         hello_milvus.drop_index()
 
     hello_milvus.drop()
 
 if __name__ == "__main__":
-    bf16_vector_search()
+    bf16_vector_search()
```

### Comparing `pymilvus-2.4.0/examples/binary_example.py` & `pymilvus-2.4.1/examples/binary_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/cert/ca.pem` & `pymilvus-2.4.1/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/cert/client.key` & `pymilvus-2.4.1/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/cert/client.pem` & `pymilvus-2.4.1/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/cert/server.pem` & `pymilvus-2.4.1/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/collection.py` & `pymilvus-2.4.1/examples/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # or implied. See the License for the specific language governing permissions and limitations under the License.
 
 from pymilvus import Collection, connections, FieldSchema, CollectionSchema, DataType, utility
 from pymilvus.client.types import LoadState
 
 import random
 import numpy as np
-from sklearn import preprocessing
+import pandas
+
 import string
 
 from pymilvus.orm import db
 
 default_dim = 128
 default_nb = 3000
 default_float_vec_field_name = "float_vector"
@@ -96,38 +97,32 @@
         FieldSchema(name="double", dtype=DataType.DOUBLE),
         FieldSchema(name=default_binary_vec_field_name, dtype=DataType.BINARY_VECTOR, dim=default_dim)
     ]
     default_schema = CollectionSchema(fields=binary_fields, description="test collection")
     return default_schema
 
 
-def gen_float_vectors(num, dim, is_normal=True):
-    vectors = [[random.random() for _ in range(dim)] for _ in range(num)]
-    vectors = preprocessing.normalize(vectors, axis=1, norm='l2')
-    return vectors.tolist()
+def gen_float_vectors(num, dim):
+    return [[random.random() for _ in range(dim)] for _ in range(num)]
 
 
-def gen_float_data(nb, is_normal=False):
-    vectors = gen_float_vectors(nb, default_dim, is_normal)
+def gen_float_data(nb):
     entities = [
         [i for i in range(nb)],
         [float(i) for i in range(nb)],
-        vectors
+        gen_float_vectors(nb, default_dim),
     ]
     return entities
 
 
-def gen_dataframe(nb, is_normal=False):
-    import pandas
-    import numpy
-
-    vectors = gen_float_vectors(nb, default_dim, is_normal)
+def gen_dataframe(nb):
+    vectors = gen_float_vectors(nb, default_dim)
     data = {
         "int64": [i for i in range(nb)],
-        "float": numpy.array([i for i in range(nb)], dtype=numpy.float32),
+        "float": np.array([i for i in range(nb)], dtype=np.float32),
         "float_vector": vectors
     }
 
     return pandas.DataFrame(data)
 
 
 def gen_binary_vectors(num, dim):
```

### Comparing `pymilvus-2.4.0/examples/data/train_embeddings.csv` & `pymilvus-2.4.1/examples/data/train_embeddings.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/database.py` & `pymilvus-2.4.1/examples/database.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/dynamic_field.py` & `pymilvus-2.4.1/examples/dynamic_field.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example.py` & `pymilvus-2.4.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_bulkinsert_json.py` & `pymilvus-2.4.1/examples/example_bulkinsert_json.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_bulkinsert_numpy.py` & `pymilvus-2.4.1/examples/example_bulkinsert_numpy.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_bulkwriter.py` & `pymilvus-2.4.1/examples/example_bulkwriter.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_gpu_brute_force.py` & `pymilvus-2.4.1/examples/example_gpu_brute_force.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# WANNING:
+# Running this example code requires the deployment of a Milvus instance
+# that attached with GPU devices.
+# Please refer to this document (https://milvus.io/docs/install_standalone-helm-gpu.md) for deployment instructions
+
 import numpy as np
 import time 
 import random
 
 from pymilvus import (
     connections,
     list_collections,
```

### Comparing `pymilvus-2.4.0/examples/example_gpu_cagra.py` & `pymilvus-2.4.1/examples/example_gpu_cagra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# WANNING:
+# Running this example code requires the deployment of a Milvus instance
+# that attached with GPU devices.
+# Please refer to this document (https://milvus.io/docs/install_standalone-helm-gpu.md) for deployment instructions
+
 import numpy as np
 import time 
 import random
 
 from pymilvus import (
     connections,
     list_collections,
```

### Comparing `pymilvus-2.4.0/examples/example_group_by.py` & `pymilvus-2.4.1/examples/example_group_by.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_index.py` & `pymilvus-2.4.1/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_str.py` & `pymilvus-2.4.1/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_tls1.py` & `pymilvus-2.4.1/examples/example_tls1.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/example_tls2.py` & `pymilvus-2.4.1/examples/example_tls2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/films.csv` & `pymilvus-2.4.1/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/float16_example.py` & `pymilvus-2.4.1/examples/float16_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,45 +15,43 @@
 
 def gen_fp16_vectors(num, dim):
     raw_vectors = []
     fp16_vectors = []
     for _ in range(num):
         raw_vector = [random.random() for _ in range(dim)]
         raw_vectors.append(raw_vector)
-        fp16_vector = np.array(raw_vector, dtype=np.float16).view(np.uint8).tolist()
-        fp16_vectors.append(bytes(fp16_vector))
+        fp16_vector = np.array(raw_vector, dtype=np.float16)
+        fp16_vectors.append(fp16_vector)
     return raw_vectors, fp16_vectors
 
 def fp16_vector_search():
     connections.connect()
 
     int64_field = FieldSchema(name="int64", dtype=DataType.INT64, is_primary=True, auto_id=True)
     dim = 128
     nb = 3000
     vector_field_name = "float16_vector"
     fp16_vector = FieldSchema(name=vector_field_name, dtype=DataType.FLOAT16_VECTOR, dim=dim)
     schema = CollectionSchema(fields=[int64_field, fp16_vector])
 
-    has = utility.has_collection("hello_milvus")
-    if has:
-        hello_milvus = Collection("hello_milvus_fp16")
-        hello_milvus.drop()
-    else:
-        hello_milvus = Collection("hello_milvus_fp16", schema)
+    if utility.has_collection("hello_milvus_fp16"):
+        utility.drop_collection("hello_milvus_fp16")
+
+    hello_milvus = Collection("hello_milvus_fp16", schema)
 
     _, vectors = gen_fp16_vectors(nb, dim)
+    hello_milvus.insert([vectors[:6]])
     rows = [
-        {vector_field_name: vectors[0]},
-        {vector_field_name: vectors[1]},
-        {vector_field_name: vectors[2]},
-        {vector_field_name: vectors[3]},
-        {vector_field_name: vectors[4]},
-        {vector_field_name: vectors[5]},
+        {vector_field_name: vectors[6]},
+        {vector_field_name: vectors[7]},
+        {vector_field_name: vectors[8]},
+        {vector_field_name: vectors[9]},
+        {vector_field_name: vectors[10]},
+        {vector_field_name: vectors[11]},
     ]
-
     hello_milvus.insert(rows)
     hello_milvus.flush()
 
     for i, index_type in enumerate(fp16_index_types):
         index_params = default_fp16_index_params[i]
         hello_milvus.create_index(vector_field_name,
                                   index_params={"index_type": index_type, "params": index_params, "metric_type": "L2"})
@@ -63,8 +61,8 @@
         print(res)
         hello_milvus.release()
         hello_milvus.drop_index()
 
     hello_milvus.drop()
 
 if __name__ == "__main__":
-    fp16_vector_search()
+    fp16_vector_search()
```

### Comparing `pymilvus-2.4.0/examples/fuzzy_match.py` & `pymilvus-2.4.1/examples/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hello_hybrid_sparse_dense.py` & `pymilvus-2.4.1/examples/hello_hybrid_sparse_dense.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # A demo showing hybrid semantic search with dense and sparse vectors using Milvus.
+#
 # You can optionally choose to use the BGE-M3 model to embed the text as dense
-# and sparse vectors, or simply use random generated vectors as the example.
-
-# To use BGE-M3 model, you need to install the optional `model` module in pymilvus:
+# and sparse vectors, or simply use random generated vectors as an example.
+#
+# You can also use the BGE CrossEncoder model to rerank the search results.
+#
+# Note that the sparse vector search feature is only available in Milvus 2.4.0 or
+# higher version. Make sure you follow https://milvus.io/docs/install_standalone-docker.md
+# to set up the latest version of Milvus in your local environment.
+
+# To connect to Milvus server, you need the python client library called pymilvus.
+# To use BGE-M3 model, you need to install the optional `model` module in pymilvus.
+# You can get them by simply running the following commands:
+#
+# pip install pymilvus
 # pip install pymilvus[model]
+
+# If true, use BGE-M3 model to generate dense and sparse vectors.
+# If false, use random numbers to compose dense and sparse vectors.
 use_bge_m3 = True
+# If true, the search result will be reranked using BGE CrossEncoder model.
+use_reranker = True
 
 # The overall steps are as follows:
 # 1. embed the text as dense and sparse vectors
 # 2. setup a Milvus collection to store the dense and sparse vectors
 # 3. insert the data to Milvus
 # 4. search and inspect the result!
 import random
@@ -73,15 +89,15 @@
 # Now we can create the new collection with above name and schema.
 col = Collection(col_name, schema, consistency_level="Strong")
 
 # We need to create indices for the vector fields. The indices will be loaded
 # into memory for efficient search.
 sparse_index = {"index_type": "SPARSE_INVERTED_INDEX", "metric_type": "IP"}
 col.create_index("sparse_vector", sparse_index)
-dense_index = {"index_type": "FLAT", "metric_type": "L2"}
+dense_index = {"index_type": "FLAT", "metric_type": "IP"}
 col.create_index("dense_vector", dense_index)
 col.load()
 
 # 3. insert text and sparse/dense vector representations into the collection
 entities = [docs, docs_embeddings["sparse"], docs_embeddings["dense"]]
 col.insert(entities)
 col.flush()
@@ -89,27 +105,47 @@
 # 4. search and inspect the result!
 k = 2 # we want to get the top 2 docs closest to the query
 
 # Prepare the search requests for both vector fields
 sparse_search_params = {"metric_type": "IP"}
 sparse_req = AnnSearchRequest(query_embeddings["sparse"],
                               "sparse_vector", sparse_search_params, limit=k)
-dense_search_params = {"metric_type": "L2"}
+dense_search_params = {"metric_type": "IP"}
 dense_req = AnnSearchRequest(query_embeddings["dense"],
                              "dense_vector", dense_search_params, limit=k)
 
 # Search topK docs based on dense and sparse vectors and rerank with RRF.
 res = col.hybrid_search([sparse_req, dense_req], rerank=RRFRanker(),
                         limit=k, output_fields=['text'])
 
 # Currently Milvus only support 1 query in the same hybrid search request, so
 # we inspect res[0] directly. In future release Milvus will accept batch
 # hybrid search queries in the same call.
-for hit in res[0]:
-    print(f'text: {hit.fields["text"]} distance {hit.distance}')
+res = res[0]
 
-# If you are using BGE-M3 to generate the embedding, you should see the following:
+if use_reranker:
+    result_texts = [hit.fields["text"] for hit in res]
+    from pymilvus.model.reranker import BGERerankFunction
+    bge_rf = BGERerankFunction(device='cpu')
+    # rerank the results using BGE CrossEncoder model
+    results = bge_rf(query, result_texts, top_k=2)
+    for hit in results:
+        print(f'text: {hit.text} distance {hit.score}')
+else:
+    for hit in res:
+        print(f'text: {hit.fields["text"]} distance {hit.distance}')
+
+# If you used both BGE-M3 and the reranker, you should see the following:
+# text: Alan Turing was the first person to conduct substantial research in AI. distance 0.9306981017573297
+# text: Artificial intelligence was founded as an academic discipline in 1956. distance 0.03217001154515051
+#
+# If you used only BGE-M3, you should see the following:
 # text: Alan Turing was the first person to conduct substantial research in AI. distance 0.032786883413791656
 # text: Artificial intelligence was founded as an academic discipline in 1956. distance 0.016129031777381897
 
+# In this simple example the reranker yields the same result as the embedding based hybrid search, but in more complex
+# scenarios the reranker can provide more accurate results.
+
+# If you used random vectors, the result will be different each time you run the script.
+
 # Drop the collection to clean up the data.
-utility.drop_collection(col_name)
+utility.drop_collection(col_name)
```

### Comparing `pymilvus-2.4.0/examples/hello_milvus.ipynb` & `pymilvus-2.4.1/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hello_milvus.py` & `pymilvus-2.4.1/examples/hello_milvus.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,26 @@
 
 print(fmt.format("Start inserting entities"))
 rng = np.random.default_rng(seed=19530)
 entities = [
     # provide the pk field because `auto_id` is set to False
     [str(i) for i in range(num_entities)],
     rng.random(num_entities).tolist(),  # field random, only supports list
-    rng.random((num_entities, dim)),    # field embeddings, supports numpy.ndarray and list
+    rng.random((num_entities, dim), np.float32),    # field embeddings, supports numpy.ndarray and list
 ]
 
 insert_result = hello_milvus.insert(entities)
 
+row = {
+    "pk": "19530",
+    "random": 0.5,
+    "embeddings": rng.random((1, dim), np.float32)[0]
+}
+hello_milvus.insert(row)
+
 hello_milvus.flush()
 print(f"Number of entities in Milvus: {hello_milvus.num_entities}")  # check the num_entities
 
 ################################################################################
 # 4. create index
 # We are going to create an IVF_FLAT index for hello_milvus collection.
 # create_index() can only be applied to `FloatVector` and `BinaryVector` fields.
```

### Comparing `pymilvus-2.4.0/examples/hello_milvus_array.py` & `pymilvus-2.4.1/examples/hello_milvus_array.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hello_milvus_delete.py` & `pymilvus-2.4.1/examples/hello_milvus_delete.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hello_model.py` & `pymilvus-2.4.1/examples/hello_model.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hello_sparse.py` & `pymilvus-2.4.1/examples/hello_sparse.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/hybrid_search.py` & `pymilvus-2.4.1/examples/hybrid_search.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/inverted_index_example.py` & `pymilvus-2.4.1/examples/inverted_index_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/iterator.py` & `pymilvus-2.4.1/examples/iterator.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/alias.py` & `pymilvus-2.4.1/examples/milvus_client/alias.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/customize_schema.py` & `pymilvus-2.4.1/examples/milvus_client/customize_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/customize_schema_auto_id.py` & `pymilvus-2.4.1/examples/milvus_client/customize_schema_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/index.py` & `pymilvus-2.4.1/examples/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/index_params.py` & `pymilvus-2.4.1/examples/milvus_client/index_params.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/non_ascii_encode.py` & `pymilvus-2.4.1/examples/milvus_client/non_ascii_encode.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/partition.py` & `pymilvus-2.4.1/examples/milvus_client/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/rbac.py` & `pymilvus-2.4.1/examples/milvus_client/rbac.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/simple.py` & `pymilvus-2.4.1/examples/milvus_client/simple.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/simple_auto_id.py` & `pymilvus-2.4.1/examples/milvus_client/simple_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/milvus_client/sparse.py` & `pymilvus-2.4.1/examples/milvus_client/sparse.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/multithreading_hello_milvus.py` & `pymilvus-2.4.1/examples/multithreading_hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/old_style_example.py` & `pymilvus-2.4.1/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/old_style_example_index.py` & `pymilvus-2.4.1/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/old_style_example_str.py` & `pymilvus-2.4.1/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/old_style_query.py` & `pymilvus-2.4.1/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/examples/partition.py` & `pymilvus-2.4.1/examples/partition.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pymilvus import (
     connections, list_collections, has_partition,
     FieldSchema, CollectionSchema, DataType,
     Collection, Partition
 )
 
 import random
-from sklearn import preprocessing
 import string
 
 default_dim = 128
 default_nb = 3000
 default_float_vec_field_name = "float_vector"
 default_segment_row_limit = 1000
 
@@ -68,26 +67,19 @@
         FieldSchema(name=default_float_vec_field_name, dtype=DataType.FLOAT_VECTOR, dim=default_dim)
     ]
     default_schema = CollectionSchema(fields=default_fields, description="test collection",
                                       segment_row_limit=default_segment_row_limit, auto_id=False)
     return default_schema
 
 
-def gen_vectors(num, dim, is_normal=True):
-    vectors = [[random.random() for _ in range(dim)] for _ in range(num)]
-    vectors = preprocessing.normalize(vectors, axis=1, norm='l2')
-    return vectors.tolist()
-
-
-def gen_data(nb, is_normal=False):
-    vectors = gen_vectors(nb, default_dim, is_normal)
+def gen_data(nb):
     entities = [
         [i for i in range(nb)],
         [float(i) for i in range(nb)],
-        vectors
+        [[random.random() for _ in range(dim)] for _ in range(num)],
     ]
     return entities
 
 
 def gen_unique_str(str_value=None):
     prefix = "".join(random.choice(string.ascii_letters + string.digits) for _ in range(8))
     return "collection_" + prefix if str_value is None else str_value + "_" + prefix
```

### Comparing `pymilvus-2.4.0/examples/resource_group.py` & `pymilvus-2.4.1/examples/resource_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pymilvus import utility, connections, DEFAULT_RESOURCE_GROUP
+from pymilvus import utility, connections
+from pymilvus.client.constants import DEFAULT_RESOURCE_GROUP
 from example import *
 
 _HOST = '127.0.0.1'
 _PORT = '19530'
 
 _CONNECTION_NAME = "default"
 
@@ -48,15 +49,15 @@
 
 
 def transfer_replica(source, target, collection_name, num_replica):
     print(
         f"transfer {num_replica} replicas in {collection_name} from {source} to {target}")
     utility.transfer_replica(
         source, target, collection_name, num_replica, using=_CONNECTION_NAME)
-    
+
 def run(): 
     create_connection("root", "123456")
     coll = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
     vectors = insert(coll, 10000, _DIM)
     coll.flush()
     create_index(coll, _VECTOR_FIELD_NAME)
```

### Comparing `pymilvus-2.4.0/examples/role_and_privilege.py` & `pymilvus-2.4.1/examples/role_and_privilege.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pymilvus import utility, connections, Collection, CollectionSchema, FieldSchema, DataType
 from pymilvus.orm.role import Role
 
 import random
-from sklearn import preprocessing
 
 _CONNECTION = "demo"
 _FOO_CONNECTION = "foo_connection"
 _DB_NAME = "foo_db"
 _HOST = '127.0.0.1'
 _PORT = '19530'
 _ROOT = "root"
@@ -75,26 +74,23 @@
     print(f"has collection end")
 
 
 default_dim = 128
 default_nb = 1000
 
 
-def gen_float_vectors(num, dim, is_normal=True):
-    vectors = [[random.random() for _ in range(dim)] for _ in range(num)]
-    vectors = preprocessing.normalize(vectors, axis=1, norm='l2')
-    return vectors.tolist()
+def gen_float_vectors(num, dim):
+    return [[random.random() for _ in range(dim)] for _ in range(num)]
 
 
-def gen_float_data(nb, is_normal=False):
-    vectors = gen_float_vectors(nb, default_dim, is_normal)
+def gen_float_data(nb):
     entities = [
         [i for i in range(nb)],
         [float(i) for i in range(nb)],
-        vectors
+        gen_float_vectors(nb, default_dim),
     ]
     return entities
 
 
 # rbac I
 def rbac_collection(connection=_CONNECTION):
     print(f"rbac_collection")
```

### Comparing `pymilvus-2.4.0/examples/user.py` & `pymilvus-2.4.1/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/__init__.py` & `pymilvus-2.4.1/pymilvus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     mkts_from_datetime,
     mkts_from_hybridts,
     mkts_from_unixtime,
     reset_password,
     transfer_node,
     transfer_replica,
     update_password,
+    update_resource_groups,
     wait_for_index_building_complete,
     wait_for_loading_complete,
 )
 
 # Compatiable
 from .settings import Config as DefaultConfig
 
@@ -102,14 +103,15 @@
     "mkts_from_unixtime",
     "mkts_from_datetime",
     "hybridts_to_unixtime",
     "hybridts_to_datetime",
     "reset_password",
     "create_user",
     "update_password",
+    "update_resource_groups",
     "delete_user",
     "list_usernames",
     "SearchResult",
     "Hits",
     "Hit",
     "Replica",
     "Group",
```

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/buffer.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,20 @@
                     arr.append(np.array(val, dtype=np.dtype("float32")))
                 data[k] = pd.Series(arr)
             elif field_schema.dtype == DataType.BINARY_VECTOR:
                 arr = []
                 for val in self._buffer[k]:
                     arr.append(np.array(val, dtype=np.dtype("uint8")))
                 data[k] = pd.Series(arr)
+            elif field_schema.dtype == DataType.ARRAY:
+                dt = NUMPY_TYPE_CREATOR[field_schema.element_type.name]
+                arr = []
+                for val in self._buffer[k]:
+                    arr.append(np.array(val, dtype=dt))
+                data[k] = pd.Series(arr)
             elif field_schema.dtype.name in NUMPY_TYPE_CREATOR:
                 dt = NUMPY_TYPE_CREATOR[field_schema.dtype.name]
                 data[k] = pd.Series(self._buffer[k], dtype=dt)
             else:
                 # dtype is null, let pandas deduce the type, might not work
                 data[k] = pd.Series(self._buffer[k])
```

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/bulk_import.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/bulk_import.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/bulk_writer.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/constants.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/local_bulk_writer.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/local_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/bulk_writer/remote_bulk_writer.py` & `pymilvus-2.4.1/pymilvus/bulk_writer/remote_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/__init__.py` & `pymilvus-2.4.1/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/abstract.py` & `pymilvus-2.4.1/pymilvus/client/abstract.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/asynch.py` & `pymilvus-2.4.1/pymilvus/client/asynch.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/check.py` & `pymilvus-2.4.1/pymilvus/client/check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/entity_helper.py` & `pymilvus-2.4.1/pymilvus/client/entity_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -287,38 +287,77 @@
     )
 
 
 def entity_to_array_arr(entity: List[Any], field_info: Any):
     return convert_to_array_arr(entity.get("values", []), field_info)
 
 
-def pack_field_value_to_field_data(field_value: Any, field_data: Any, field_info: Any):
+def pack_field_value_to_field_data(
+    field_value: Any, field_data: schema_types.FieldData, field_info: Any
+):
     field_type = field_data.type
     if field_type == DataType.BOOL:
         field_data.scalars.bool_data.data.append(field_value)
     elif field_type in (DataType.INT8, DataType.INT16, DataType.INT32):
         field_data.scalars.int_data.data.append(field_value)
     elif field_type == DataType.INT64:
         field_data.scalars.long_data.data.append(field_value)
     elif field_type == DataType.FLOAT:
         field_data.scalars.float_data.data.append(field_value)
     elif field_type == DataType.DOUBLE:
         field_data.scalars.double_data.data.append(field_value)
     elif field_type == DataType.FLOAT_VECTOR:
-        field_data.vectors.dim = len(field_value)
-        field_data.vectors.float_vector.data.extend(field_value)
+        f_value = field_value
+        if isinstance(field_value, np.ndarray):
+            if field_value.dtype not in ("float32", "float64"):
+                raise ParamError(
+                    message="invalid input for float32 vector, expect np.ndarray with dtype=float32"
+                )
+            f_value = field_value.tolist()
+
+        field_data.vectors.dim = len(f_value)
+        field_data.vectors.float_vector.data.extend(f_value)
+
     elif field_type == DataType.BINARY_VECTOR:
         field_data.vectors.dim = len(field_value) * 8
         field_data.vectors.binary_vector += bytes(field_value)
+
     elif field_type == DataType.FLOAT16_VECTOR:
-        field_data.vectors.dim = len(field_value) // 2
-        field_data.vectors.float16_vector += bytes(field_value)
+        if isinstance(field_value, bytes):
+            v_bytes = field_value
+        elif isinstance(field_value, np.ndarray):
+            if field_value.dtype != "float16":
+                raise ParamError(
+                    message="invalid input for float16 vector, expect np.ndarray with dtype=float16"
+                )
+            v_bytes = field_value.view(np.uint8).tobytes()
+        else:
+            raise ParamError(
+                message="invalid input type for float16 vector, expect np.ndarray with dtype=float16"
+            )
+
+        field_data.vectors.dim = len(v_bytes) // 2
+        field_data.vectors.float16_vector += v_bytes
+
     elif field_type == DataType.BFLOAT16_VECTOR:
-        field_data.vectors.dim = len(field_value) // 2
-        field_data.vectors.bfloat16_vector += bytes(field_value)
+        if isinstance(field_value, bytes):
+            v_bytes = field_value
+        elif isinstance(field_value, np.ndarray):
+            if field_value.dtype != "bfloat16":
+                raise ParamError(
+                    message="invalid input for bfloat16 vector, expect np.ndarray with dtype=bfloat16"
+                )
+            v_bytes = field_value.view(np.uint8).tobytes()
+        else:
+            raise ParamError(
+                message="invalid input type for bfloat16 vector, expect np.ndarray with dtype=bfloat16"
+            )
+
+        field_data.vectors.dim = len(v_bytes) // 2
+        field_data.vectors.bfloat16_vector += v_bytes
     elif field_type == DataType.SPARSE_FLOAT_VECTOR:
         # field_value is a single row of sparse float vector in user provided format
         if not sparse_is_scipy_format(field_value):
             field_value = [field_value]
         elif field_value.shape[0] != 1:
             raise ParamError(message="invalid input for sparse float vector: expect 1 row")
         if not entity_is_sparse_matrix(field_value):
```

### Comparing `pymilvus-2.4.0/pymilvus/client/grpc_handler.py` & `pymilvus-2.4.1/pymilvus/client/grpc_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import copy
 import json
 import socket
 import time
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Mapping, Optional, Union
 from urllib import parse
 
 import grpc
 from grpc._cython import cygrpc
 
 from pymilvus.decorators import ignore_unimplemented, retry_on_rpc_failure, upgrade_reminder
 from pymilvus.exceptions import (
@@ -45,14 +45,15 @@
     DataType,
     GrantInfo,
     Group,
     IndexState,
     LoadState,
     Plan,
     Replica,
+    ResourceGroupConfig,
     ResourceGroupInfo,
     RoleInfo,
     Shard,
     State,
     Status,
     UserInfo,
 )
@@ -471,54 +472,57 @@
             schema = self.describe_collection(collection_name, timeout=timeout)
 
         fields_info = schema.get("fields")
         enable_dynamic = schema.get("enable_dynamic_field", False)
 
         return fields_info, enable_dynamic
 
-    def _prepare_row_insert_request(
+    @retry_on_rpc_failure()
+    def insert_rows(
         self,
         collection_name: str,
-        entity_rows: List,
+        entities: Union[Dict, List[Dict]],
         partition_name: Optional[str] = None,
+        schema: Optional[dict] = None,
         timeout: Optional[float] = None,
         **kwargs,
     ):
-        if not isinstance(entity_rows, list):
-            raise ParamError(message="None rows, please provide valid row data.")
-
-        fields_info, enable_dynamic = self._get_info(collection_name, timeout, **kwargs)
-        return Prepare.row_insert_param(
-            collection_name,
-            entity_rows,
-            partition_name,
-            fields_info,
-            enable_dynamic=enable_dynamic,
+        request = self._prepare_row_insert_request(
+            collection_name, entities, partition_name, timeout, **kwargs
         )
+        resp = self._stub.Insert(request=request, timeout=timeout)
+        check_status(resp.status)
+        ts_utils.update_collection_ts(collection_name, resp.timestamp)
+        return MutationResult(resp)
 
-    @retry_on_rpc_failure()
-    def insert_rows(
+    def _prepare_row_insert_request(
         self,
         collection_name: str,
-        entities: List,
+        entity_rows: Union[List[Dict], Dict],
         partition_name: Optional[str] = None,
+        schema: Optional[dict] = None,
         timeout: Optional[float] = None,
         **kwargs,
     ):
-        if isinstance(entities, dict):
-            entities = [entities]
-        request = self._prepare_row_insert_request(
-            collection_name, entities, partition_name, timeout, **kwargs
+        if isinstance(entity_rows, dict):
+            entity_rows = [entity_rows]
+
+        if not isinstance(schema, dict):
+            schema = self.describe_collection(collection_name, timeout=timeout)
+
+        fields_info = schema.get("fields")
+        enable_dynamic = schema.get("enable_dynamic_field", False)
+
+        return Prepare.row_insert_param(
+            collection_name,
+            entity_rows,
+            partition_name,
+            fields_info,
+            enable_dynamic=enable_dynamic,
         )
-        rf = self._stub.Insert.future(request, timeout=timeout)
-        response = rf.result()
-        check_status(response.status)
-        m = MutationResult(response)
-        ts_utils.update_collection_ts(collection_name, m.timestamp)
-        return m
 
     def _prepare_batch_insert_request(
         self,
         collection_name: str,
         entities: List,
         partition_name: Optional[str] = None,
         timeout: Optional[float] = None,
@@ -1372,15 +1376,15 @@
         while not flush_ret:
             flush_ret = self.get_flush_state(
                 segment_ids, collection_name, flush_ts, timeout, **kwargs
             )
             end = time.time()
             if timeout is not None and end - start > timeout:
                 raise MilvusException(
-                    message=f"wait for flush timeout, collection: {collection_name}"
+                    message=f"wait for flush timeout, collection: {collection_name}, flusht_ts: {flush_ts}"
                 )
 
             if not flush_ret:
                 time.sleep(0.5)
 
     @retry_on_rpc_failure()
     def flush(self, collection_names: list, timeout: Optional[float] = None, **kwargs):
@@ -1831,19 +1835,27 @@
         req = Prepare.get_server_version()
         resp = self._stub.GetVersion(req, timeout=timeout)
         check_status(resp.status)
         return resp.version
 
     @retry_on_rpc_failure()
     def create_resource_group(self, name: str, timeout: Optional[float] = None, **kwargs):
-        req = Prepare.create_resource_group(name)
+        req = Prepare.create_resource_group(name, **kwargs)
         resp = self._stub.CreateResourceGroup(req, wait_for_ready=True, timeout=timeout)
         check_status(resp)
 
     @retry_on_rpc_failure()
+    def update_resource_groups(
+        self, configs: Mapping[str, ResourceGroupConfig], timeout: Optional[float] = None, **kwargs
+    ):
+        req = Prepare.update_resource_groups(configs)
+        resp = self._stub.UpdateResourceGroups(req, wait_for_ready=True, timeout=timeout)
+        check_status(resp)
+
+    @retry_on_rpc_failure()
     def drop_resource_group(self, name: str, timeout: Optional[float] = None, **kwargs):
         req = Prepare.drop_resource_group(name)
         resp = self._stub.DropResourceGroup(req, wait_for_ready=True, timeout=timeout)
         check_status(resp)
 
     @retry_on_rpc_failure()
     def list_resource_groups(self, timeout: Optional[float] = None, **kwargs):
```

### Comparing `pymilvus-2.4.0/pymilvus/client/interceptor.py` & `pymilvus-2.4.1/pymilvus/client/interceptor.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/prepare.py` & `pymilvus-2.4.1/pymilvus/client/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import base64
 import datetime
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
 
-import ujson
+import numpy as np
 
 from pymilvus.client import __version__, entity_helper
 from pymilvus.exceptions import DataNotMatchException, ExceptionsMessage, ParamError
 from pymilvus.grpc_gen import common_pb2 as common_types
 from pymilvus.grpc_gen import milvus_pb2 as milvus_types
 from pymilvus.grpc_gen import schema_pb2 as schema_types
 from pymilvus.orm.schema import CollectionSchema
 
-from . import blob, ts_utils
+from . import blob, ts_utils, utils
 from .check import check_pass_param, is_legal_collection_properties
 from .constants import (
     DEFAULT_CONSISTENCY_LEVEL,
     GROUP_BY_FIELD,
     ITERATOR_FIELD,
     REDUCE_STOP_FOR_BEST,
 )
-from .types import DataType, PlaceholderType, get_consistency_level
+from .types import (
+    DataType,
+    PlaceholderType,
+    ResourceGroupConfig,
+    get_consistency_level,
+)
 from .utils import traverse_info, traverse_rows_info
 
 
 class Prepare:
     @classmethod
     def create_collection_request(
         cls,
@@ -360,20 +365,18 @@
             for field in fields_info
             if not field.get("auto_id", False)
         }
         field_info_map = {
             field["name"]: field for field in fields_info if not field.get("auto_id", False)
         }
 
-        meta_field = (
-            schema_types.FieldData(is_dynamic=True, type=DataType.JSON) if enable_dynamic else None
-        )
-        if meta_field is not None:
-            field_info_map[meta_field.field_name] = meta_field
-            fields_data[meta_field.field_name] = meta_field
+        if enable_dynamic:
+            d_field = schema_types.FieldData(is_dynamic=True, type=DataType.JSON)
+            fields_data[d_field.field_name] = d_field
+            field_info_map[d_field.field_name] = d_field
 
         try:
             for entity in entities:
                 if not isinstance(entity, Dict):
                     msg = f"expected Dict, got '{type(entity).__name__}'"
                     raise TypeError(msg)
                 for k, v in entity.items():
@@ -386,25 +389,25 @@
 
                 json_dict = {
                     k: v for k, v in entity.items() if k not in fields_data and enable_dynamic
                 }
 
                 if enable_dynamic:
                     json_value = entity_helper.convert_to_json(json_dict)
-                    meta_field.scalars.json_data.data.append(json_value)
+                    d_field.scalars.json_data.data.append(json_value)
 
         except (TypeError, ValueError) as e:
             raise DataNotMatchException(message=ExceptionsMessage.DataTypeInconsistent) from e
 
         request.fields_data.extend(
             [fields_data[field["name"]] for field in fields_info if not field.get("auto_id", False)]
         )
 
         if enable_dynamic:
-            request.fields_data.append(meta_field)
+            request.fields_data.append(d_field)
 
         _, _, auto_id_loc = traverse_rows_info(fields_info, entities)
         if auto_id_loc is not None:
             if (enable_dynamic and len(fields_data) != len(fields_info)) or (
                 not enable_dynamic and len(fields_data) + 1 != len(fields_info)
             ):
                 raise ParamError(ExceptionsMessage.FieldsNumInconsistent)
@@ -414,24 +417,26 @@
 
     @classmethod
     def row_insert_param(
         cls,
         collection_name: str,
         entities: List,
         partition_name: str,
-        fields_info: Any,
+        fields_info: Dict,
         enable_dynamic: bool = False,
     ):
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
         # insert_request.hash_keys won't be filled in client.
-        tag = partition_name if isinstance(partition_name, str) else ""
+        p_name = partition_name if isinstance(partition_name, str) else ""
         request = milvus_types.InsertRequest(
-            collection_name=collection_name, partition_name=tag, num_rows=len(entities)
+            collection_name=collection_name,
+            partition_name=p_name,
+            num_rows=len(entities),
         )
 
         return cls._parse_row_request(request, fields_info, enable_dynamic, entities)
 
     @classmethod
     def row_upsert_param(
         cls,
@@ -441,39 +446,41 @@
         fields_info: Any,
         enable_dynamic: bool = False,
     ):
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
         # upsert_request.hash_keys won't be filled in client.
-        tag = partition_name if isinstance(partition_name, str) else ""
+        p_name = partition_name if isinstance(partition_name, str) else ""
         request = milvus_types.UpsertRequest(
-            collection_name=collection_name, partition_name=tag, num_rows=len(entities)
+            collection_name=collection_name,
+            partition_name=p_name,
+            num_rows=len(entities),
         )
 
         return cls._parse_row_request(request, fields_info, enable_dynamic, entities)
 
     @staticmethod
     def _pre_batch_check(
         entities: List,
         fields_info: Any,
     ):
         for entity in entities:
             if (
-                not entity.get("name", None)
-                or entity.get("values", None) is None
-                or not entity.get("type", None)
+                entity.get("name") is None
+                or entity.get("values") is None
+                or entity.get("type") is None
             ):
                 raise ParamError(
                     message="Missing param in entities, a field must have type, name and values"
                 )
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
-        location, primary_key_loc, auto_id_loc = traverse_info(fields_info, entities)
+        location, primary_key_loc, auto_id_loc = traverse_info(fields_info)
 
         # though impossible from sdk
         if primary_key_loc is None:
             raise ParamError(message="primary key not found")
 
         if auto_id_loc is None and len(entities) != len(fields_info):
             msg = f"number of fields: {len(fields_info)}, number of entities: {len(entities)}"
@@ -571,30 +578,53 @@
             collection_name=collection_name,
             partition_name=partition_name,
             expr=expr,
             consistency_level=get_consistency_level(consistency_level),
         )
 
     @classmethod
-    def _prepare_placeholders(cls, vectors: Any, nq: int, tag: Any, pl_type: Any, is_binary: bool):
-        pl = common_types.PlaceholderValue(tag=tag)
-        pl.type = pl_type
+    def _prepare_placeholder_str(cls, data: Any):
         # sparse vector
-        if pl_type == PlaceholderType.SparseFloatVector:
-            sparse_float_array_proto = entity_helper.sparse_rows_to_proto(vectors)
-            pl.values.extend(sparse_float_array_proto.contents)
-            return pl
-
-        # dense or binary vector
-        for i in range(nq):
-            if is_binary:
-                pl.values.append(blob.vector_binary_to_bytes(vectors[i]))
+        if entity_helper.entity_is_sparse_matrix(data):
+            pl_type = PlaceholderType.SparseFloatVector
+            pl_values = entity_helper.sparse_rows_to_proto(data).contents
+
+        elif isinstance(data[0], np.ndarray):
+            dtype = data[0].dtype
+
+            if dtype == "bfloat16":
+                pl_type = PlaceholderType.BFLOAT16_VECTOR
+                pl_values = (array.tobytes() for array in data)
+            elif dtype == "float16":
+                pl_type = PlaceholderType.FLOAT16_VECTOR
+                pl_values = (array.tobytes() for array in data)
+            elif dtype in ("float32", "float64"):
+                pl_type = PlaceholderType.FloatVector
+                pl_values = (blob.vector_float_to_bytes(entity) for entity in data)
+
+            elif dtype == "byte":
+                pl_type = PlaceholderType.BinaryVector
+                pl_values = data
+
             else:
-                pl.values.append(blob.vector_float_to_bytes(vectors[i]))
-        return pl
+                err_msg = f"unsupported data type: {dtype}"
+                raise ParamError(message=err_msg)
+
+        elif isinstance(data[0], bytes):
+            pl_type = PlaceholderType.BinaryVector
+            pl_values = data  # data is already a list of bytes
+
+        else:
+            pl_type = PlaceholderType.FloatVector
+            pl_values = (blob.vector_float_to_bytes(entity) for entity in data)
+
+        pl = common_types.PlaceholderValue(tag="$0", type=pl_type, values=pl_values)
+        return common_types.PlaceholderGroup.SerializeToString(
+            common_types.PlaceholderGroup(placeholders=[pl])
+        )
 
     @classmethod
     def search_requests_with_expr(
         cls,
         collection_name: str,
         data: Union[List, entity_helper.SparseMatrixInputType],
         anns_field: str,
@@ -602,24 +632,14 @@
         limit: int,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
         round_decimal: int = -1,
         **kwargs,
     ) -> milvus_types.SearchRequest:
-        if entity_helper.entity_is_sparse_matrix(data):
-            is_binary = False
-            pl_type = PlaceholderType.SparseFloatVector
-        elif isinstance(data[0], bytes):
-            is_binary = True
-            pl_type = PlaceholderType.BinaryVector
-        else:
-            is_binary = False
-            pl_type = PlaceholderType.FloatVector
-
         use_default_consistency = ts_utils.construct_guarantee_ts(collection_name, kwargs)
 
         ignore_growing = param.get("ignore_growing", False) or kwargs.get("ignore_growing", False)
         params = param.get("params", {})
         if not isinstance(params, dict):
             raise ParamError(message=f"Search params must be a dict, got {type(params)}")
 
@@ -650,45 +670,35 @@
 
         if param.get("metric_type") is not None:
             search_params["metric_type"] = param["metric_type"]
 
         if anns_field:
             search_params["anns_field"] = anns_field
 
-        def dump(v: Dict):
-            if isinstance(v, dict):
-                return ujson.dumps(v)
-            return str(v)
-
+        req_params = [
+            common_types.KeyValuePair(key=str(key), value=utils.dumps(value))
+            for key, value in search_params.items()
+        ]
         nq = entity_helper.get_input_num_rows(data)
-        tag = "$0"
-        pl = cls._prepare_placeholders(data, nq, tag, pl_type, is_binary)
-        plg = common_types.PlaceholderGroup()
-        plg.placeholders.append(pl)
-        plg_str = common_types.PlaceholderGroup.SerializeToString(plg)
+        plg_str = cls._prepare_placeholder_str(data)
+
         request = milvus_types.SearchRequest(
             collection_name=collection_name,
             partition_names=partition_names,
             output_fields=output_fields,
             guarantee_timestamp=kwargs.get("guarantee_timestamp", 0),
             use_default_consistency=use_default_consistency,
             consistency_level=kwargs.get("consistency_level", 0),
             nq=nq,
+            placeholder_group=plg_str,
+            dsl_type=common_types.DslType.BoolExprV1,
+            search_params=req_params,
         )
-        request.placeholder_group = plg_str
-
-        request.dsl_type = common_types.DslType.BoolExprV1
         if expr is not None:
             request.dsl = expr
-        request.search_params.extend(
-            [
-                common_types.KeyValuePair(key=str(key), value=dump(value))
-                for key, value in search_params.items()
-            ]
-        )
 
         return request
 
     @classmethod
     def hybrid_search_request_with_ranker(
         cls,
         collection_name: str,
@@ -699,33 +709,29 @@
         output_fields: Optional[List[str]] = None,
         round_decimal: int = -1,
         **kwargs,
     ) -> milvus_types.HybridSearchRequest:
         use_default_consistency = ts_utils.construct_guarantee_ts(collection_name, kwargs)
         rerank_param["limit"] = limit
         rerank_param["round_decimal"] = round_decimal
-
-        def dump(v: Dict):
-            if isinstance(v, dict):
-                return ujson.dumps(v)
-            return str(v)
+        rerank_param["offset"] = kwargs.get("offset", 0)
 
         request = milvus_types.HybridSearchRequest(
             collection_name=collection_name,
             partition_names=partition_names,
             requests=reqs,
             output_fields=output_fields,
             guarantee_timestamp=kwargs.get("guarantee_timestamp", 0),
             use_default_consistency=use_default_consistency,
             consistency_level=kwargs.get("consistency_level", 0),
         )
 
         request.rank_params.extend(
             [
-                common_types.KeyValuePair(key=str(key), value=dump(value))
+                common_types.KeyValuePair(key=str(key), value=utils.dumps(value))
                 for key, value in rerank_param.items()
             ]
         )
 
         return request
 
     @classmethod
@@ -752,34 +758,28 @@
     def create_index_request(cls, collection_name: str, field_name: str, params: Dict, **kwargs):
         index_params = milvus_types.CreateIndexRequest(
             collection_name=collection_name,
             field_name=field_name,
             index_name=kwargs.get("index_name", ""),
         )
 
-        def dump(tv: Dict):
-            return ujson.dumps(tv) if isinstance(tv, dict) else str(tv)
-
         if isinstance(params, dict):
             for tk, tv in params.items():
                 if tk == "dim" and (not tv or not isinstance(tv, int)):
                     raise ParamError(message="dim must be of int!")
-                kv_pair = common_types.KeyValuePair(key=str(tk), value=dump(tv))
+                kv_pair = common_types.KeyValuePair(key=str(tk), value=utils.dumps(tv))
                 index_params.extra_params.append(kv_pair)
 
         return index_params
 
     @classmethod
     def alter_index_request(cls, collection_name: str, index_name: str, extra_params: dict):
-        def dump(tv: Dict):
-            return ujson.dumps(tv) if isinstance(tv, dict) else str(tv)
-
         params = []
         for k, v in extra_params.items():
-            params.append(common_types.KeyValuePair(key=str(k), value=dump(v)))
+            params.append(common_types.KeyValuePair(key=str(k), value=utils.dumps(v)))
         return milvus_types.AlterIndexRequest(
             collection_name=collection_name, index_name=index_name, extra_params=params
         )
 
     @classmethod
     def describe_index_request(
         cls, collection_name: str, index_name: str, timestamp: Optional[int] = None
@@ -1147,17 +1147,26 @@
         )
 
     @classmethod
     def get_server_version(cls):
         return milvus_types.GetVersionRequest()
 
     @classmethod
-    def create_resource_group(cls, name: str):
+    def create_resource_group(cls, name: str, **kwargs):
         check_pass_param(resource_group_name=name)
-        return milvus_types.CreateResourceGroupRequest(resource_group=name)
+        return milvus_types.CreateResourceGroupRequest(
+            resource_group=name,
+            config=kwargs.get("config"),
+        )
+
+    @classmethod
+    def update_resource_groups(cls, configs: Mapping[str, ResourceGroupConfig]):
+        return milvus_types.UpdateResourceGroupsRequest(
+            resource_groups=configs,
+        )
 
     @classmethod
     def drop_resource_group(cls, name: str):
         check_pass_param(resource_group_name=name)
         return milvus_types.DropResourceGroupRequest(resource_group=name)
 
     @classmethod
```

### Comparing `pymilvus-2.4.0/pymilvus/client/stub.py` & `pymilvus-2.4.1/pymilvus/client/stub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from urllib import parse
 
 from pymilvus.decorators import deprecated
 from pymilvus.exceptions import MilvusException, ParamError
 from pymilvus.settings import Config
+from typing import Mapping
 
 from .check import is_legal_host, is_legal_port
 from .grpc_handler import GrpcHandler
 from .types import (
     BulkInsertState,
     CompactionPlans,
     CompactionState,
     Replica,
     ResourceGroupInfo,
+    ResourceGroupConfig,
 )
 
 
 class Milvus:
     @deprecated
     def __init__(
         self, host=None, port=Config.GRPC_PORT, uri=Config.GRPC_URI, channel=None, **kwargs
@@ -1377,14 +1379,25 @@
 
         :param name: resource group name
         :type name: str
         """
         with self._connection() as handler:
             handler.create_resource_group(name, timeout=timeout, **kwargs)
 
+    def update_resource_groups(
+        self, configs: Mapping[str, ResourceGroupConfig], timeout=None, **kwargs
+    ):
+        """update resource groups with specific configs
+
+        :param configs: resource group configs
+        :type name: Mapping
+        """
+        with self._connection() as handler:
+            handler.update_resource_groups(configs=configs, timeout=timeout, **kwargs)
+
     def drop_resource_group(self, name, timeout=None, **kwargs):
         """drop resource group with specific name
 
         :param name: resource group name
         :type name: str
         """
         with self._connection() as handler:
```

### Comparing `pymilvus-2.4.0/pymilvus/client/ts_utils.py` & `pymilvus-2.4.1/pymilvus/client/ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/client/types.py` & `pymilvus-2.4.1/pymilvus/client/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, ClassVar, Dict, List, TypeVar, Union
 
 from pymilvus.exceptions import (
     AutoIDException,
     ExceptionsMessage,
     InvalidConsistencyLevel,
 )
-from pymilvus.grpc_gen import common_pb2
+from pymilvus.grpc_gen import common_pb2, rg_pb2
 from pymilvus.grpc_gen import milvus_pb2 as milvus_types
 
 Status = TypeVar("Status")
 ConsistencyLevel = common_pb2.ConsistencyLevel
 
 
 class Status:
@@ -759,29 +759,34 @@
     @property
     def groups(self):
         return self._groups
 
 
 class ResourceGroupInfo:
     def __init__(self, resource_group: Any) -> None:
+
         self._name = resource_group.name
         self._capacity = resource_group.capacity
         self._num_available_node = resource_group.num_available_node
         self._num_loaded_replica = resource_group.num_loaded_replica
         self._num_outgoing_node = resource_group.num_outgoing_node
         self._num_incoming_node = resource_group.num_incoming_node
+        self._config = resource_group.config
+        self._nodes = [NodeInfo(node) for node in resource_group.nodes]
 
     def __repr__(self) -> str:
         return f"""ResourceGroupInfo:
 <name:{self.name}>,
 <capacity:{self.capacity}>,
 <num_available_node:{self.num_available_node}>,
 <num_loaded_replica:{self.num_loaded_replica}>,
 <num_outgoing_node:{self.num_outgoing_node}>,
-<num_incoming_node:{self.num_incoming_node}>"""
+<num_incoming_node:{self.num_incoming_node}>,
+<config:{self.config}>,
+<nodes:{self.nodes}>"""
 
     @property
     def name(self):
         return self._name
 
     @property
     def capacity(self):
@@ -798,7 +803,88 @@
     @property
     def num_outgoing_node(self):
         return self._num_outgoing_node
 
     @property
     def num_incoming_node(self):
         return self._num_incoming_node
+
+    @property
+    def config(self):
+        return self._config
+
+    @property
+    def nodes(self):
+        return self._nodes
+
+
+class NodeInfo:
+    """
+    Represents information about a node in the system.
+    Attributes:
+        node_id (int): The ID of the node.
+        address (str): The ip address of the node.
+        hostname (str): The hostname of the node.
+    Example:
+        NodeInfo(
+            node_id=1,
+            address="127.0.0.1",
+            hostname="localhost",
+        )
+    """
+
+    def __init__(self, info: Any) -> None:
+        self._node_id = info.node_id
+        self._address = info.address
+        self._hostname = info.hostname
+
+    def __repr__(self) -> str:
+        return f"""NodeInfo:
+<node_id:{self.node_id}>,
+<address:{self.address}>,
+<hostname:{self.hostname}>"""
+
+    @property
+    def node_id(self) -> int:
+        return self._node_id
+
+    @property
+    def address(self) -> str:
+        return self._address
+
+    @property
+    def hostname(self) -> str:
+        return self._hostname
+
+
+ResourceGroupConfig = rg_pb2.ResourceGroupConfig
+"""
+Represents the configuration of a resource group.
+Attributes:
+    requests (ResourceGroupLimit): The requests of the resource group.
+    limits (ResourceGroupLimit): The limits of the resource group.
+    transfer_from (List[ResourceGroupTransfer]): The transfer config that resource group
+        can transfer node from the resource group of this field at high priority.
+    transfer_to (List[ResourceGroupTransfer]): The transfer config that resource group
+        can transfer node to the resource group of this field at high priority.
+Example:
+    ResourceGroupConfig(
+        requests={"node_num": 1},
+        limits={"node_num": 5},
+        transfer_from=[{"resource_group": "__default_resource_group"}],
+        transfer_to=[{"resource_group": "resource_group_2"}],
+    )
+"""
+
+ResourceGroupLimit = rg_pb2.ResourceGroupLimit
+"""
+Represents the limit of a resource group.
+Attributes:
+    node_num (int): The number of nodes that the resource group can hold.
+"""
+
+ResourceGroupTransfer = rg_pb2.ResourceGroupTransfer
+"""
+Represents the transfer config of a resource group.
+Attributes:
+    resource_group (str): The name of the resource group that can be transferred to or from.
+"""
```

### Comparing `pymilvus-2.4.0/pymilvus/client/utils.py` & `pymilvus-2.4.1/pymilvus/client/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 from datetime import timedelta
 from typing import Any, List, Optional, Union
 
+import ujson
+
 from pymilvus.exceptions import MilvusException, ParamError
 from pymilvus.grpc_gen.common_pb2 import Status
 
 from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
 from .types import DataType
 
 MILVUS = "milvus"
@@ -216,15 +218,14 @@
             is_auto_id = True
 
         if field.get("is_primary", False):
             primary_key_loc = i
 
         field_name = field["name"]
         location[field_name] = i
-        field_type = field["type"]
 
         if field.get("is_dynamic", False):
             is_dynamic = True
 
         for j, entity in enumerate(entities):
             if is_auto_id:
                 if field_name in entity:
@@ -237,100 +238,35 @@
                 raise ParamError(
                     message=f"dynamic field enabled, {field_name} shouldn't in entities[{j}]"
                 )
 
             value = entity.get(field_name, None)
             if value is None:
                 raise ParamError(message=f"Field {field_name} don't match in entities[{j}]")
-            # no special check for sparse float vector field
-            if field_type in [
-                DataType.FLOAT_VECTOR,
-                DataType.BINARY_VECTOR,
-                DataType.BFLOAT16_VECTOR,
-                DataType.FLOAT16_VECTOR,
-            ]:
-                field_dim = field["params"]["dim"]
-                entity_dim = len(value)
-                if field_type in [DataType.BINARY_VECTOR]:
-                    entity_dim = entity_dim * 8
-                elif field_type in [DataType.BFLOAT16_VECTOR, DataType.FLOAT16_VECTOR]:
-                    entity_dim = int(entity_dim // 2)
-                if entity_dim != field_dim:
-                    raise ParamError(
-                        message=f"Collection field dim is {field_dim}"
-                        f", but entities field dim is {entity_dim}"
-                    )
 
     # though impossible from sdk
     if primary_key_loc is None:
         raise ParamError(message="primary key not found")
 
     return location, primary_key_loc, auto_id_loc
 
 
-def traverse_info(fields_info: Any, entities: List):
+def traverse_info(fields_info: Any):
     location, primary_key_loc, auto_id_loc = {}, None, None
     for i, field in enumerate(fields_info):
         if field.get("is_primary", False):
             primary_key_loc = i
 
         if field.get("auto_id", False):
             auto_id_loc = i
             continue
-
-        match_flag = False
-        field_name = field["name"]
-        field_type = field["type"]
-
-        for entity in entities:
-            entity_name, entity_type = entity["name"], entity["type"]
-
-            if field_name == entity_name:
-                if field_type != entity_type:
-                    raise ParamError(
-                        message=f"Collection field type is {field_type}"
-                        f", but entities field type is {entity_type}"
-                    )
-
-                entity_dim, field_dim = 0, 0
-                if entity_type in [
-                    DataType.FLOAT_VECTOR,
-                    DataType.BINARY_VECTOR,
-                    DataType.BFLOAT16_VECTOR,
-                    DataType.FLOAT16_VECTOR,
-                ]:
-                    field_dim = field["params"]["dim"]
-                    entity_dim = len(entity["values"][0])
-
-                if entity_type in [DataType.FLOAT_VECTOR] and entity_dim != field_dim:
-                    raise ParamError(
-                        message=f"Collection field dim is {field_dim}"
-                        f", but entities field dim is {entity_dim}"
-                    )
-
-                if entity_type in [DataType.BINARY_VECTOR] and entity_dim * 8 != field_dim:
-                    raise ParamError(
-                        message=f"Collection field dim is {field_dim}"
-                        f", but entities field dim is {entity_dim * 8}"
-                    )
-
-                if (
-                    entity_type in [DataType.BFLOAT16_VECTOR, DataType.FLOAT16_VECTOR]
-                    and int(entity_dim // 2) != field_dim
-                ):
-                    raise ParamError(
-                        message=f"Collection field dim is {field_dim}"
-                        f", but entities field dim is {int(entity_dim // 2)}"
-                    )
-
-                location[field["name"]] = i
-                match_flag = True
-                break
-
-        if not match_flag:
-            raise ParamError(message=f"Field {field['name']} don't match in entities")
+        location[field["name"]] = i
 
     return location, primary_key_loc, auto_id_loc
 
 
 def get_server_type(host: str):
     return ZILLIZ if (isinstance(host, str) and "zilliz" in host.lower()) else MILVUS
+
+
+def dumps(v: Union[dict, str]) -> str:
+    return ujson.dumps(v) if isinstance(v, dict) else str(v)
```

### Comparing `pymilvus-2.4.0/pymilvus/decorators.py` & `pymilvus-2.4.1/pymilvus/decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/exceptions.py` & `pymilvus-2.4.1/pymilvus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/common_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x13milvus.proto.common\x1a google/protobuf/descriptor.proto\"\xf3\x01\n\x06Status\x12\x36\n\nerror_code\x18\x01 \x01(\x0e\x32\x1e.milvus.proto.common.ErrorCodeB\x02\x18\x01\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x05\x12\x11\n\tretriable\x18\x04 \x01(\x08\x12\x0e\n\x06\x64\x65tail\x18\x05 \x01(\t\x12>\n\nextra_info\x18\x06 \x03(\x0b\x32*.milvus.proto.common.Status.ExtraInfoEntry\x1a\x30\n\x0e\x45xtraInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\x0cKeyValuePair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0bKeyDataPair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x15\n\x04\x42lob\x12\r\n\x05value\x18\x01 \x01(\x0c\"c\n\x10PlaceholderValue\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32$.milvus.proto.common.PlaceholderType\x12\x0e\n\x06values\x18\x03 \x03(\x0c\"O\n\x10PlaceholderGroup\x12;\n\x0cplaceholders\x18\x01 \x03(\x0b\x32%.milvus.proto.common.PlaceholderValue\"#\n\x07\x41\x64\x64ress\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\"\xaf\x02\n\x07MsgBase\x12.\n\x08msg_type\x18\x01 \x01(\x0e\x32\x1c.milvus.proto.common.MsgType\x12\r\n\x05msgID\x18\x02 \x01(\x03\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\x12\x10\n\x08sourceID\x18\x04 \x01(\x03\x12\x10\n\x08targetID\x18\x05 \x01(\x03\x12@\n\nproperties\x18\x06 \x03(\x0b\x32,.milvus.proto.common.MsgBase.PropertiesEntry\x12\x39\n\rreplicateInfo\x18\x07 \x01(\x0b\x32\".milvus.proto.common.ReplicateInfo\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\rReplicateInfo\x12\x13\n\x0bisReplicate\x18\x01 \x01(\x08\x12\x14\n\x0cmsgTimestamp\x18\x02 \x01(\x04\"7\n\tMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"M\n\x0c\x44MLMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\tshardName\x18\x02 \x01(\t\"\xbb\x01\n\x0cPrivilegeExt\x12\x34\n\x0bobject_type\x18\x01 \x01(\x0e\x32\x1f.milvus.proto.common.ObjectType\x12>\n\x10object_privilege\x18\x02 \x01(\x0e\x32$.milvus.proto.common.ObjectPrivilege\x12\x19\n\x11object_name_index\x18\x03 \x01(\x05\x12\x1a\n\x12object_name_indexs\x18\x04 \x01(\x05\"2\n\x0cSegmentStats\x12\x11\n\tSegmentID\x18\x01 \x01(\x03\x12\x0f\n\x07NumRows\x18\x02 \x01(\x03\"\xd5\x01\n\nClientInfo\x12\x10\n\x08sdk_type\x18\x01 \x01(\t\x12\x13\n\x0bsdk_version\x18\x02 \x01(\t\x12\x12\n\nlocal_time\x18\x03 \x01(\t\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x0c\n\x04host\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ClientInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe3\x01\n\nServerInfo\x12\x12\n\nbuild_tags\x18\x01 \x01(\t\x12\x12\n\nbuild_time\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\ngo_version\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65ploy_mode\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ServerInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"=\n\x08NodeInfo\x12\x0e\n\x06nodeID\x18\x01 \x01(\x03\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t*\xc7\n\n\tErrorCode\x12\x0b\n\x07Success\x10\x00\x12\x13\n\x0fUnexpectedError\x10\x01\x12\x11\n\rConnectFailed\x10\x02\x12\x14\n\x10PermissionDenied\x10\x03\x12\x17\n\x13\x43ollectionNotExists\x10\x04\x12\x13\n\x0fIllegalArgument\x10\x05\x12\x14\n\x10IllegalDimension\x10\x07\x12\x14\n\x10IllegalIndexType\x10\x08\x12\x19\n\x15IllegalCollectionName\x10\t\x12\x0f\n\x0bIllegalTOPK\x10\n\x12\x14\n\x10IllegalRowRecord\x10\x0b\x12\x13\n\x0fIllegalVectorID\x10\x0c\x12\x17\n\x13IllegalSearchResult\x10\r\x12\x10\n\x0c\x46ileNotFound\x10\x0e\x12\x0e\n\nMetaFailed\x10\x0f\x12\x0f\n\x0b\x43\x61\x63heFailed\x10\x10\x12\x16\n\x12\x43\x61nnotCreateFolder\x10\x11\x12\x14\n\x10\x43\x61nnotCreateFile\x10\x12\x12\x16\n\x12\x43\x61nnotDeleteFolder\x10\x13\x12\x14\n\x10\x43\x61nnotDeleteFile\x10\x14\x12\x13\n\x0f\x42uildIndexError\x10\x15\x12\x10\n\x0cIllegalNLIST\x10\x16\x12\x15\n\x11IllegalMetricType\x10\x17\x12\x0f\n\x0bOutOfMemory\x10\x18\x12\x11\n\rIndexNotExist\x10\x19\x12\x13\n\x0f\x45mptyCollection\x10\x1a\x12\x1b\n\x17UpdateImportTaskFailure\x10\x1b\x12\x1a\n\x16\x43ollectionNameNotFound\x10\x1c\x12\x1b\n\x17\x43reateCredentialFailure\x10\x1d\x12\x1b\n\x17UpdateCredentialFailure\x10\x1e\x12\x1b\n\x17\x44\x65leteCredentialFailure\x10\x1f\x12\x18\n\x14GetCredentialFailure\x10 \x12\x18\n\x14ListCredUsersFailure\x10!\x12\x12\n\x0eGetUserFailure\x10\"\x12\x15\n\x11\x43reateRoleFailure\x10#\x12\x13\n\x0f\x44ropRoleFailure\x10$\x12\x1a\n\x16OperateUserRoleFailure\x10%\x12\x15\n\x11SelectRoleFailure\x10&\x12\x15\n\x11SelectUserFailure\x10\'\x12\x19\n\x15SelectResourceFailure\x10(\x12\x1b\n\x17OperatePrivilegeFailure\x10)\x12\x16\n\x12SelectGrantFailure\x10*\x12!\n\x1dRefreshPolicyInfoCacheFailure\x10+\x12\x15\n\x11ListPolicyFailure\x10,\x12\x12\n\x0eNotShardLeader\x10-\x12\x16\n\x12NoReplicaAvailable\x10.\x12\x13\n\x0fSegmentNotFound\x10/\x12\r\n\tForceDeny\x10\x30\x12\r\n\tRateLimit\x10\x31\x12\x12\n\x0eNodeIDNotMatch\x10\x32\x12\x14\n\x10UpsertAutoIDTrue\x10\x33\x12\x1c\n\x18InsufficientMemoryToLoad\x10\x34\x12\x18\n\x14MemoryQuotaExhausted\x10\x35\x12\x16\n\x12\x44iskQuotaExhausted\x10\x36\x12\x15\n\x11TimeTickLongDelay\x10\x37\x12\x11\n\rNotReadyServe\x10\x38\x12\x1b\n\x17NotReadyCoordActivating\x10\x39\x12\x0f\n\x0b\x44\x61taCoordNA\x10\x64\x12\x12\n\rDDRequestRace\x10\xe8\x07\x1a\x02\x18\x01*c\n\nIndexState\x12\x12\n\x0eIndexStateNone\x10\x00\x12\x0c\n\x08Unissued\x10\x01\x12\x0e\n\nInProgress\x10\x02\x12\x0c\n\x08\x46inished\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\t\n\x05Retry\x10\x05*\x82\x01\n\x0cSegmentState\x12\x14\n\x10SegmentStateNone\x10\x00\x12\x0c\n\x08NotExist\x10\x01\x12\x0b\n\x07Growing\x10\x02\x12\n\n\x06Sealed\x10\x03\x12\x0b\n\x07\x46lushed\x10\x04\x12\x0c\n\x08\x46lushing\x10\x05\x12\x0b\n\x07\x44ropped\x10\x06\x12\r\n\tImporting\x10\x07*\x94\x01\n\x0fPlaceholderType\x12\x08\n\x04None\x10\x00\x12\x10\n\x0c\x42inaryVector\x10\x64\x12\x0f\n\x0b\x46loatVector\x10\x65\x12\x11\n\rFloat16Vector\x10\x66\x12\x12\n\x0e\x42\x46loat16Vector\x10g\x12\x15\n\x11SparseFloatVector\x10h\x12\t\n\x05Int64\x10\x05\x12\x0b\n\x07VarChar\x10\x15*\xe0\x10\n\x07MsgType\x12\r\n\tUndefined\x10\x00\x12\x14\n\x10\x43reateCollection\x10\x64\x12\x12\n\x0e\x44ropCollection\x10\x65\x12\x11\n\rHasCollection\x10\x66\x12\x16\n\x12\x44\x65scribeCollection\x10g\x12\x13\n\x0fShowCollections\x10h\x12\x14\n\x10GetSystemConfigs\x10i\x12\x12\n\x0eLoadCollection\x10j\x12\x15\n\x11ReleaseCollection\x10k\x12\x0f\n\x0b\x43reateAlias\x10l\x12\r\n\tDropAlias\x10m\x12\x0e\n\nAlterAlias\x10n\x12\x13\n\x0f\x41lterCollection\x10o\x12\x14\n\x10RenameCollection\x10p\x12\x11\n\rDescribeAlias\x10q\x12\x0f\n\x0bListAliases\x10r\x12\x14\n\x0f\x43reatePartition\x10\xc8\x01\x12\x12\n\rDropPartition\x10\xc9\x01\x12\x11\n\x0cHasPartition\x10\xca\x01\x12\x16\n\x11\x44\x65scribePartition\x10\xcb\x01\x12\x13\n\x0eShowPartitions\x10\xcc\x01\x12\x13\n\x0eLoadPartitions\x10\xcd\x01\x12\x16\n\x11ReleasePartitions\x10\xce\x01\x12\x11\n\x0cShowSegments\x10\xfa\x01\x12\x14\n\x0f\x44\x65scribeSegment\x10\xfb\x01\x12\x11\n\x0cLoadSegments\x10\xfc\x01\x12\x14\n\x0fReleaseSegments\x10\xfd\x01\x12\x14\n\x0fHandoffSegments\x10\xfe\x01\x12\x18\n\x13LoadBalanceSegments\x10\xff\x01\x12\x15\n\x10\x44\x65scribeSegments\x10\x80\x02\x12\x1c\n\x17\x46\x65\x64\x65rListIndexedSegment\x10\x81\x02\x12\"\n\x1d\x46\x65\x64\x65rDescribeSegmentIndexData\x10\x82\x02\x12\x10\n\x0b\x43reateIndex\x10\xac\x02\x12\x12\n\rDescribeIndex\x10\xad\x02\x12\x0e\n\tDropIndex\x10\xae\x02\x12\x17\n\x12GetIndexStatistics\x10\xaf\x02\x12\x0f\n\nAlterIndex\x10\xb0\x02\x12\x0b\n\x06Insert\x10\x90\x03\x12\x0b\n\x06\x44\x65lete\x10\x91\x03\x12\n\n\x05\x46lush\x10\x92\x03\x12\x17\n\x12ResendSegmentStats\x10\x93\x03\x12\x0b\n\x06Upsert\x10\x94\x03\x12\x0b\n\x06Search\x10\xf4\x03\x12\x11\n\x0cSearchResult\x10\xf5\x03\x12\x12\n\rGetIndexState\x10\xf6\x03\x12\x1a\n\x15GetIndexBuildProgress\x10\xf7\x03\x12\x1c\n\x17GetCollectionStatistics\x10\xf8\x03\x12\x1b\n\x16GetPartitionStatistics\x10\xf9\x03\x12\r\n\x08Retrieve\x10\xfa\x03\x12\x13\n\x0eRetrieveResult\x10\xfb\x03\x12\x14\n\x0fWatchDmChannels\x10\xfc\x03\x12\x15\n\x10RemoveDmChannels\x10\xfd\x03\x12\x17\n\x12WatchQueryChannels\x10\xfe\x03\x12\x18\n\x13RemoveQueryChannels\x10\xff\x03\x12\x1d\n\x18SealedSegmentsChangeInfo\x10\x80\x04\x12\x17\n\x12WatchDeltaChannels\x10\x81\x04\x12\x14\n\x0fGetShardLeaders\x10\x82\x04\x12\x10\n\x0bGetReplicas\x10\x83\x04\x12\x13\n\x0eUnsubDmChannel\x10\x84\x04\x12\x14\n\x0fGetDistribution\x10\x85\x04\x12\x15\n\x10SyncDistribution\x10\x86\x04\x12\x10\n\x0bSegmentInfo\x10\xd8\x04\x12\x0f\n\nSystemInfo\x10\xd9\x04\x12\x14\n\x0fGetRecoveryInfo\x10\xda\x04\x12\x14\n\x0fGetSegmentState\x10\xdb\x04\x12\r\n\x08TimeTick\x10\xb0\t\x12\x13\n\x0eQueryNodeStats\x10\xb1\t\x12\x0e\n\tLoadIndex\x10\xb2\t\x12\x0e\n\tRequestID\x10\xb3\t\x12\x0f\n\nRequestTSO\x10\xb4\t\x12\x14\n\x0f\x41llocateSegment\x10\xb5\t\x12\x16\n\x11SegmentStatistics\x10\xb6\t\x12\x15\n\x10SegmentFlushDone\x10\xb7\t\x12\x0f\n\nDataNodeTt\x10\xb8\t\x12\x0c\n\x07\x43onnect\x10\xb9\t\x12\x14\n\x0fListClientInfos\x10\xba\t\x12\x13\n\x0e\x41llocTimestamp\x10\xbb\t\x12\x15\n\x10\x43reateCredential\x10\xdc\x0b\x12\x12\n\rGetCredential\x10\xdd\x0b\x12\x15\n\x10\x44\x65leteCredential\x10\xde\x0b\x12\x15\n\x10UpdateCredential\x10\xdf\x0b\x12\x16\n\x11ListCredUsernames\x10\xe0\x0b\x12\x0f\n\nCreateRole\x10\xc0\x0c\x12\r\n\x08\x44ropRole\x10\xc1\x0c\x12\x14\n\x0fOperateUserRole\x10\xc2\x0c\x12\x0f\n\nSelectRole\x10\xc3\x0c\x12\x0f\n\nSelectUser\x10\xc4\x0c\x12\x13\n\x0eSelectResource\x10\xc5\x0c\x12\x15\n\x10OperatePrivilege\x10\xc6\x0c\x12\x10\n\x0bSelectGrant\x10\xc7\x0c\x12\x1b\n\x16RefreshPolicyInfoCache\x10\xc8\x0c\x12\x0f\n\nListPolicy\x10\xc9\x0c\x12\x18\n\x13\x43reateResourceGroup\x10\xa4\r\x12\x16\n\x11\x44ropResourceGroup\x10\xa5\r\x12\x17\n\x12ListResourceGroups\x10\xa6\r\x12\x1a\n\x15\x44\x65scribeResourceGroup\x10\xa7\r\x12\x11\n\x0cTransferNode\x10\xa8\r\x12\x14\n\x0fTransferReplica\x10\xa9\r\x12\x19\n\x14UpdateResourceGroups\x10\xaa\r\x12\x13\n\x0e\x43reateDatabase\x10\x89\x0e\x12\x11\n\x0c\x44ropDatabase\x10\x8a\x0e\x12\x12\n\rListDatabases\x10\x8b\x0e*\"\n\x07\x44slType\x12\x07\n\x03\x44sl\x10\x00\x12\x0e\n\nBoolExprV1\x10\x01*B\n\x0f\x43ompactionState\x12\x11\n\rUndefiedState\x10\x00\x12\r\n\tExecuting\x10\x01\x12\r\n\tCompleted\x10\x02*X\n\x10\x43onsistencyLevel\x12\n\n\x06Strong\x10\x00\x12\x0b\n\x07Session\x10\x01\x12\x0b\n\x07\x42ounded\x10\x02\x12\x0e\n\nEventually\x10\x03\x12\x0e\n\nCustomized\x10\x04*\x9e\x01\n\x0bImportState\x12\x11\n\rImportPending\x10\x00\x12\x10\n\x0cImportFailed\x10\x01\x12\x11\n\rImportStarted\x10\x02\x12\x13\n\x0fImportPersisted\x10\x05\x12\x11\n\rImportFlushed\x10\x08\x12\x13\n\x0fImportCompleted\x10\x06\x12\x1a\n\x16ImportFailedAndCleaned\x10\x07*2\n\nObjectType\x12\x0e\n\nCollection\x10\x00\x12\n\n\x06Global\x10\x01\x12\x08\n\x04User\x10\x02*\xba\n\n\x0fObjectPrivilege\x12\x10\n\x0cPrivilegeAll\x10\x00\x12\x1d\n\x19PrivilegeCreateCollection\x10\x01\x12\x1b\n\x17PrivilegeDropCollection\x10\x02\x12\x1f\n\x1bPrivilegeDescribeCollection\x10\x03\x12\x1c\n\x18PrivilegeShowCollections\x10\x04\x12\x11\n\rPrivilegeLoad\x10\x05\x12\x14\n\x10PrivilegeRelease\x10\x06\x12\x17\n\x13PrivilegeCompaction\x10\x07\x12\x13\n\x0fPrivilegeInsert\x10\x08\x12\x13\n\x0fPrivilegeDelete\x10\t\x12\x1a\n\x16PrivilegeGetStatistics\x10\n\x12\x18\n\x14PrivilegeCreateIndex\x10\x0b\x12\x18\n\x14PrivilegeIndexDetail\x10\x0c\x12\x16\n\x12PrivilegeDropIndex\x10\r\x12\x13\n\x0fPrivilegeSearch\x10\x0e\x12\x12\n\x0ePrivilegeFlush\x10\x0f\x12\x12\n\x0ePrivilegeQuery\x10\x10\x12\x18\n\x14PrivilegeLoadBalance\x10\x11\x12\x13\n\x0fPrivilegeImport\x10\x12\x12\x1c\n\x18PrivilegeCreateOwnership\x10\x13\x12\x17\n\x13PrivilegeUpdateUser\x10\x14\x12\x1a\n\x16PrivilegeDropOwnership\x10\x15\x12\x1c\n\x18PrivilegeSelectOwnership\x10\x16\x12\x1c\n\x18PrivilegeManageOwnership\x10\x17\x12\x17\n\x13PrivilegeSelectUser\x10\x18\x12\x13\n\x0fPrivilegeUpsert\x10\x19\x12 \n\x1cPrivilegeCreateResourceGroup\x10\x1a\x12\x1e\n\x1aPrivilegeDropResourceGroup\x10\x1b\x12\"\n\x1ePrivilegeDescribeResourceGroup\x10\x1c\x12\x1f\n\x1bPrivilegeListResourceGroups\x10\x1d\x12\x19\n\x15PrivilegeTransferNode\x10\x1e\x12\x1c\n\x18PrivilegeTransferReplica\x10\x1f\x12\x1f\n\x1bPrivilegeGetLoadingProgress\x10 \x12\x19\n\x15PrivilegeGetLoadState\x10!\x12\x1d\n\x19PrivilegeRenameCollection\x10\"\x12\x1b\n\x17PrivilegeCreateDatabase\x10#\x12\x19\n\x15PrivilegeDropDatabase\x10$\x12\x1a\n\x16PrivilegeListDatabases\x10%\x12\x15\n\x11PrivilegeFlushAll\x10&\x12\x1c\n\x18PrivilegeCreatePartition\x10\'\x12\x1a\n\x16PrivilegeDropPartition\x10(\x12\x1b\n\x17PrivilegeShowPartitions\x10)\x12\x19\n\x15PrivilegeHasPartition\x10*\x12\x1a\n\x16PrivilegeGetFlushState\x10+\x12\x18\n\x14PrivilegeCreateAlias\x10,\x12\x16\n\x12PrivilegeDropAlias\x10-\x12\x1a\n\x16PrivilegeDescribeAlias\x10.\x12\x18\n\x14PrivilegeListAliases\x10/\x12!\n\x1dPrivilegeUpdateResourceGroups\x10\x30*S\n\tStateCode\x12\x10\n\x0cInitializing\x10\x00\x12\x0b\n\x07Healthy\x10\x01\x12\x0c\n\x08\x41\x62normal\x10\x02\x12\x0b\n\x07StandBy\x10\x03\x12\x0c\n\x08Stopping\x10\x04*c\n\tLoadState\x12\x15\n\x11LoadStateNotExist\x10\x00\x12\x14\n\x10LoadStateNotLoad\x10\x01\x12\x14\n\x10LoadStateLoading\x10\x02\x12\x13\n\x0fLoadStateLoaded\x10\x03:^\n\x11privilege_ext_obj\x12\x1f.google.protobuf.MessageOptions\x18\xe9\x07 \x01(\x0b\x32!.milvus.proto.common.PrivilegeExtBm\n\x0eio.milvus.grpcB\x0b\x43ommonProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x13milvus.proto.common\x1a google/protobuf/descriptor.proto\"\xf3\x01\n\x06Status\x12\x36\n\nerror_code\x18\x01 \x01(\x0e\x32\x1e.milvus.proto.common.ErrorCodeB\x02\x18\x01\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x05\x12\x11\n\tretriable\x18\x04 \x01(\x08\x12\x0e\n\x06\x64\x65tail\x18\x05 \x01(\t\x12>\n\nextra_info\x18\x06 \x03(\x0b\x32*.milvus.proto.common.Status.ExtraInfoEntry\x1a\x30\n\x0e\x45xtraInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\x0cKeyValuePair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0bKeyDataPair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x15\n\x04\x42lob\x12\r\n\x05value\x18\x01 \x01(\x0c\"c\n\x10PlaceholderValue\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32$.milvus.proto.common.PlaceholderType\x12\x0e\n\x06values\x18\x03 \x03(\x0c\"O\n\x10PlaceholderGroup\x12;\n\x0cplaceholders\x18\x01 \x03(\x0b\x32%.milvus.proto.common.PlaceholderValue\"#\n\x07\x41\x64\x64ress\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\"\xaf\x02\n\x07MsgBase\x12.\n\x08msg_type\x18\x01 \x01(\x0e\x32\x1c.milvus.proto.common.MsgType\x12\r\n\x05msgID\x18\x02 \x01(\x03\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\x12\x10\n\x08sourceID\x18\x04 \x01(\x03\x12\x10\n\x08targetID\x18\x05 \x01(\x03\x12@\n\nproperties\x18\x06 \x03(\x0b\x32,.milvus.proto.common.MsgBase.PropertiesEntry\x12\x39\n\rreplicateInfo\x18\x07 \x01(\x0b\x32\".milvus.proto.common.ReplicateInfo\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\rReplicateInfo\x12\x13\n\x0bisReplicate\x18\x01 \x01(\x08\x12\x14\n\x0cmsgTimestamp\x18\x02 \x01(\x04\"7\n\tMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"M\n\x0c\x44MLMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\tshardName\x18\x02 \x01(\t\"\xbb\x01\n\x0cPrivilegeExt\x12\x34\n\x0bobject_type\x18\x01 \x01(\x0e\x32\x1f.milvus.proto.common.ObjectType\x12>\n\x10object_privilege\x18\x02 \x01(\x0e\x32$.milvus.proto.common.ObjectPrivilege\x12\x19\n\x11object_name_index\x18\x03 \x01(\x05\x12\x1a\n\x12object_name_indexs\x18\x04 \x01(\x05\"2\n\x0cSegmentStats\x12\x11\n\tSegmentID\x18\x01 \x01(\x03\x12\x0f\n\x07NumRows\x18\x02 \x01(\x03\"\xd5\x01\n\nClientInfo\x12\x10\n\x08sdk_type\x18\x01 \x01(\t\x12\x13\n\x0bsdk_version\x18\x02 \x01(\t\x12\x12\n\nlocal_time\x18\x03 \x01(\t\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x0c\n\x04host\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ClientInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe3\x01\n\nServerInfo\x12\x12\n\nbuild_tags\x18\x01 \x01(\t\x12\x12\n\nbuild_time\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\ngo_version\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65ploy_mode\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ServerInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\">\n\x08NodeInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\x03\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t*\xc7\n\n\tErrorCode\x12\x0b\n\x07Success\x10\x00\x12\x13\n\x0fUnexpectedError\x10\x01\x12\x11\n\rConnectFailed\x10\x02\x12\x14\n\x10PermissionDenied\x10\x03\x12\x17\n\x13\x43ollectionNotExists\x10\x04\x12\x13\n\x0fIllegalArgument\x10\x05\x12\x14\n\x10IllegalDimension\x10\x07\x12\x14\n\x10IllegalIndexType\x10\x08\x12\x19\n\x15IllegalCollectionName\x10\t\x12\x0f\n\x0bIllegalTOPK\x10\n\x12\x14\n\x10IllegalRowRecord\x10\x0b\x12\x13\n\x0fIllegalVectorID\x10\x0c\x12\x17\n\x13IllegalSearchResult\x10\r\x12\x10\n\x0c\x46ileNotFound\x10\x0e\x12\x0e\n\nMetaFailed\x10\x0f\x12\x0f\n\x0b\x43\x61\x63heFailed\x10\x10\x12\x16\n\x12\x43\x61nnotCreateFolder\x10\x11\x12\x14\n\x10\x43\x61nnotCreateFile\x10\x12\x12\x16\n\x12\x43\x61nnotDeleteFolder\x10\x13\x12\x14\n\x10\x43\x61nnotDeleteFile\x10\x14\x12\x13\n\x0f\x42uildIndexError\x10\x15\x12\x10\n\x0cIllegalNLIST\x10\x16\x12\x15\n\x11IllegalMetricType\x10\x17\x12\x0f\n\x0bOutOfMemory\x10\x18\x12\x11\n\rIndexNotExist\x10\x19\x12\x13\n\x0f\x45mptyCollection\x10\x1a\x12\x1b\n\x17UpdateImportTaskFailure\x10\x1b\x12\x1a\n\x16\x43ollectionNameNotFound\x10\x1c\x12\x1b\n\x17\x43reateCredentialFailure\x10\x1d\x12\x1b\n\x17UpdateCredentialFailure\x10\x1e\x12\x1b\n\x17\x44\x65leteCredentialFailure\x10\x1f\x12\x18\n\x14GetCredentialFailure\x10 \x12\x18\n\x14ListCredUsersFailure\x10!\x12\x12\n\x0eGetUserFailure\x10\"\x12\x15\n\x11\x43reateRoleFailure\x10#\x12\x13\n\x0f\x44ropRoleFailure\x10$\x12\x1a\n\x16OperateUserRoleFailure\x10%\x12\x15\n\x11SelectRoleFailure\x10&\x12\x15\n\x11SelectUserFailure\x10\'\x12\x19\n\x15SelectResourceFailure\x10(\x12\x1b\n\x17OperatePrivilegeFailure\x10)\x12\x16\n\x12SelectGrantFailure\x10*\x12!\n\x1dRefreshPolicyInfoCacheFailure\x10+\x12\x15\n\x11ListPolicyFailure\x10,\x12\x12\n\x0eNotShardLeader\x10-\x12\x16\n\x12NoReplicaAvailable\x10.\x12\x13\n\x0fSegmentNotFound\x10/\x12\r\n\tForceDeny\x10\x30\x12\r\n\tRateLimit\x10\x31\x12\x12\n\x0eNodeIDNotMatch\x10\x32\x12\x14\n\x10UpsertAutoIDTrue\x10\x33\x12\x1c\n\x18InsufficientMemoryToLoad\x10\x34\x12\x18\n\x14MemoryQuotaExhausted\x10\x35\x12\x16\n\x12\x44iskQuotaExhausted\x10\x36\x12\x15\n\x11TimeTickLongDelay\x10\x37\x12\x11\n\rNotReadyServe\x10\x38\x12\x1b\n\x17NotReadyCoordActivating\x10\x39\x12\x0f\n\x0b\x44\x61taCoordNA\x10\x64\x12\x12\n\rDDRequestRace\x10\xe8\x07\x1a\x02\x18\x01*c\n\nIndexState\x12\x12\n\x0eIndexStateNone\x10\x00\x12\x0c\n\x08Unissued\x10\x01\x12\x0e\n\nInProgress\x10\x02\x12\x0c\n\x08\x46inished\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\t\n\x05Retry\x10\x05*\x82\x01\n\x0cSegmentState\x12\x14\n\x10SegmentStateNone\x10\x00\x12\x0c\n\x08NotExist\x10\x01\x12\x0b\n\x07Growing\x10\x02\x12\n\n\x06Sealed\x10\x03\x12\x0b\n\x07\x46lushed\x10\x04\x12\x0c\n\x08\x46lushing\x10\x05\x12\x0b\n\x07\x44ropped\x10\x06\x12\r\n\tImporting\x10\x07*\x94\x01\n\x0fPlaceholderType\x12\x08\n\x04None\x10\x00\x12\x10\n\x0c\x42inaryVector\x10\x64\x12\x0f\n\x0b\x46loatVector\x10\x65\x12\x11\n\rFloat16Vector\x10\x66\x12\x12\n\x0e\x42\x46loat16Vector\x10g\x12\x15\n\x11SparseFloatVector\x10h\x12\t\n\x05Int64\x10\x05\x12\x0b\n\x07VarChar\x10\x15*\xe0\x10\n\x07MsgType\x12\r\n\tUndefined\x10\x00\x12\x14\n\x10\x43reateCollection\x10\x64\x12\x12\n\x0e\x44ropCollection\x10\x65\x12\x11\n\rHasCollection\x10\x66\x12\x16\n\x12\x44\x65scribeCollection\x10g\x12\x13\n\x0fShowCollections\x10h\x12\x14\n\x10GetSystemConfigs\x10i\x12\x12\n\x0eLoadCollection\x10j\x12\x15\n\x11ReleaseCollection\x10k\x12\x0f\n\x0b\x43reateAlias\x10l\x12\r\n\tDropAlias\x10m\x12\x0e\n\nAlterAlias\x10n\x12\x13\n\x0f\x41lterCollection\x10o\x12\x14\n\x10RenameCollection\x10p\x12\x11\n\rDescribeAlias\x10q\x12\x0f\n\x0bListAliases\x10r\x12\x14\n\x0f\x43reatePartition\x10\xc8\x01\x12\x12\n\rDropPartition\x10\xc9\x01\x12\x11\n\x0cHasPartition\x10\xca\x01\x12\x16\n\x11\x44\x65scribePartition\x10\xcb\x01\x12\x13\n\x0eShowPartitions\x10\xcc\x01\x12\x13\n\x0eLoadPartitions\x10\xcd\x01\x12\x16\n\x11ReleasePartitions\x10\xce\x01\x12\x11\n\x0cShowSegments\x10\xfa\x01\x12\x14\n\x0f\x44\x65scribeSegment\x10\xfb\x01\x12\x11\n\x0cLoadSegments\x10\xfc\x01\x12\x14\n\x0fReleaseSegments\x10\xfd\x01\x12\x14\n\x0fHandoffSegments\x10\xfe\x01\x12\x18\n\x13LoadBalanceSegments\x10\xff\x01\x12\x15\n\x10\x44\x65scribeSegments\x10\x80\x02\x12\x1c\n\x17\x46\x65\x64\x65rListIndexedSegment\x10\x81\x02\x12\"\n\x1d\x46\x65\x64\x65rDescribeSegmentIndexData\x10\x82\x02\x12\x10\n\x0b\x43reateIndex\x10\xac\x02\x12\x12\n\rDescribeIndex\x10\xad\x02\x12\x0e\n\tDropIndex\x10\xae\x02\x12\x17\n\x12GetIndexStatistics\x10\xaf\x02\x12\x0f\n\nAlterIndex\x10\xb0\x02\x12\x0b\n\x06Insert\x10\x90\x03\x12\x0b\n\x06\x44\x65lete\x10\x91\x03\x12\n\n\x05\x46lush\x10\x92\x03\x12\x17\n\x12ResendSegmentStats\x10\x93\x03\x12\x0b\n\x06Upsert\x10\x94\x03\x12\x0b\n\x06Search\x10\xf4\x03\x12\x11\n\x0cSearchResult\x10\xf5\x03\x12\x12\n\rGetIndexState\x10\xf6\x03\x12\x1a\n\x15GetIndexBuildProgress\x10\xf7\x03\x12\x1c\n\x17GetCollectionStatistics\x10\xf8\x03\x12\x1b\n\x16GetPartitionStatistics\x10\xf9\x03\x12\r\n\x08Retrieve\x10\xfa\x03\x12\x13\n\x0eRetrieveResult\x10\xfb\x03\x12\x14\n\x0fWatchDmChannels\x10\xfc\x03\x12\x15\n\x10RemoveDmChannels\x10\xfd\x03\x12\x17\n\x12WatchQueryChannels\x10\xfe\x03\x12\x18\n\x13RemoveQueryChannels\x10\xff\x03\x12\x1d\n\x18SealedSegmentsChangeInfo\x10\x80\x04\x12\x17\n\x12WatchDeltaChannels\x10\x81\x04\x12\x14\n\x0fGetShardLeaders\x10\x82\x04\x12\x10\n\x0bGetReplicas\x10\x83\x04\x12\x13\n\x0eUnsubDmChannel\x10\x84\x04\x12\x14\n\x0fGetDistribution\x10\x85\x04\x12\x15\n\x10SyncDistribution\x10\x86\x04\x12\x10\n\x0bSegmentInfo\x10\xd8\x04\x12\x0f\n\nSystemInfo\x10\xd9\x04\x12\x14\n\x0fGetRecoveryInfo\x10\xda\x04\x12\x14\n\x0fGetSegmentState\x10\xdb\x04\x12\r\n\x08TimeTick\x10\xb0\t\x12\x13\n\x0eQueryNodeStats\x10\xb1\t\x12\x0e\n\tLoadIndex\x10\xb2\t\x12\x0e\n\tRequestID\x10\xb3\t\x12\x0f\n\nRequestTSO\x10\xb4\t\x12\x14\n\x0f\x41llocateSegment\x10\xb5\t\x12\x16\n\x11SegmentStatistics\x10\xb6\t\x12\x15\n\x10SegmentFlushDone\x10\xb7\t\x12\x0f\n\nDataNodeTt\x10\xb8\t\x12\x0c\n\x07\x43onnect\x10\xb9\t\x12\x14\n\x0fListClientInfos\x10\xba\t\x12\x13\n\x0e\x41llocTimestamp\x10\xbb\t\x12\x15\n\x10\x43reateCredential\x10\xdc\x0b\x12\x12\n\rGetCredential\x10\xdd\x0b\x12\x15\n\x10\x44\x65leteCredential\x10\xde\x0b\x12\x15\n\x10UpdateCredential\x10\xdf\x0b\x12\x16\n\x11ListCredUsernames\x10\xe0\x0b\x12\x0f\n\nCreateRole\x10\xc0\x0c\x12\r\n\x08\x44ropRole\x10\xc1\x0c\x12\x14\n\x0fOperateUserRole\x10\xc2\x0c\x12\x0f\n\nSelectRole\x10\xc3\x0c\x12\x0f\n\nSelectUser\x10\xc4\x0c\x12\x13\n\x0eSelectResource\x10\xc5\x0c\x12\x15\n\x10OperatePrivilege\x10\xc6\x0c\x12\x10\n\x0bSelectGrant\x10\xc7\x0c\x12\x1b\n\x16RefreshPolicyInfoCache\x10\xc8\x0c\x12\x0f\n\nListPolicy\x10\xc9\x0c\x12\x18\n\x13\x43reateResourceGroup\x10\xa4\r\x12\x16\n\x11\x44ropResourceGroup\x10\xa5\r\x12\x17\n\x12ListResourceGroups\x10\xa6\r\x12\x1a\n\x15\x44\x65scribeResourceGroup\x10\xa7\r\x12\x11\n\x0cTransferNode\x10\xa8\r\x12\x14\n\x0fTransferReplica\x10\xa9\r\x12\x19\n\x14UpdateResourceGroups\x10\xaa\r\x12\x13\n\x0e\x43reateDatabase\x10\x89\x0e\x12\x11\n\x0c\x44ropDatabase\x10\x8a\x0e\x12\x12\n\rListDatabases\x10\x8b\x0e*\"\n\x07\x44slType\x12\x07\n\x03\x44sl\x10\x00\x12\x0e\n\nBoolExprV1\x10\x01*B\n\x0f\x43ompactionState\x12\x11\n\rUndefiedState\x10\x00\x12\r\n\tExecuting\x10\x01\x12\r\n\tCompleted\x10\x02*X\n\x10\x43onsistencyLevel\x12\n\n\x06Strong\x10\x00\x12\x0b\n\x07Session\x10\x01\x12\x0b\n\x07\x42ounded\x10\x02\x12\x0e\n\nEventually\x10\x03\x12\x0e\n\nCustomized\x10\x04*\x9e\x01\n\x0bImportState\x12\x11\n\rImportPending\x10\x00\x12\x10\n\x0cImportFailed\x10\x01\x12\x11\n\rImportStarted\x10\x02\x12\x13\n\x0fImportPersisted\x10\x05\x12\x11\n\rImportFlushed\x10\x08\x12\x13\n\x0fImportCompleted\x10\x06\x12\x1a\n\x16ImportFailedAndCleaned\x10\x07*2\n\nObjectType\x12\x0e\n\nCollection\x10\x00\x12\n\n\x06Global\x10\x01\x12\x08\n\x04User\x10\x02*\xd6\n\n\x0fObjectPrivilege\x12\x10\n\x0cPrivilegeAll\x10\x00\x12\x1d\n\x19PrivilegeCreateCollection\x10\x01\x12\x1b\n\x17PrivilegeDropCollection\x10\x02\x12\x1f\n\x1bPrivilegeDescribeCollection\x10\x03\x12\x1c\n\x18PrivilegeShowCollections\x10\x04\x12\x11\n\rPrivilegeLoad\x10\x05\x12\x14\n\x10PrivilegeRelease\x10\x06\x12\x17\n\x13PrivilegeCompaction\x10\x07\x12\x13\n\x0fPrivilegeInsert\x10\x08\x12\x13\n\x0fPrivilegeDelete\x10\t\x12\x1a\n\x16PrivilegeGetStatistics\x10\n\x12\x18\n\x14PrivilegeCreateIndex\x10\x0b\x12\x18\n\x14PrivilegeIndexDetail\x10\x0c\x12\x16\n\x12PrivilegeDropIndex\x10\r\x12\x13\n\x0fPrivilegeSearch\x10\x0e\x12\x12\n\x0ePrivilegeFlush\x10\x0f\x12\x12\n\x0ePrivilegeQuery\x10\x10\x12\x18\n\x14PrivilegeLoadBalance\x10\x11\x12\x13\n\x0fPrivilegeImport\x10\x12\x12\x1c\n\x18PrivilegeCreateOwnership\x10\x13\x12\x17\n\x13PrivilegeUpdateUser\x10\x14\x12\x1a\n\x16PrivilegeDropOwnership\x10\x15\x12\x1c\n\x18PrivilegeSelectOwnership\x10\x16\x12\x1c\n\x18PrivilegeManageOwnership\x10\x17\x12\x17\n\x13PrivilegeSelectUser\x10\x18\x12\x13\n\x0fPrivilegeUpsert\x10\x19\x12 \n\x1cPrivilegeCreateResourceGroup\x10\x1a\x12\x1e\n\x1aPrivilegeDropResourceGroup\x10\x1b\x12\"\n\x1ePrivilegeDescribeResourceGroup\x10\x1c\x12\x1f\n\x1bPrivilegeListResourceGroups\x10\x1d\x12\x19\n\x15PrivilegeTransferNode\x10\x1e\x12\x1c\n\x18PrivilegeTransferReplica\x10\x1f\x12\x1f\n\x1bPrivilegeGetLoadingProgress\x10 \x12\x19\n\x15PrivilegeGetLoadState\x10!\x12\x1d\n\x19PrivilegeRenameCollection\x10\"\x12\x1b\n\x17PrivilegeCreateDatabase\x10#\x12\x19\n\x15PrivilegeDropDatabase\x10$\x12\x1a\n\x16PrivilegeListDatabases\x10%\x12\x15\n\x11PrivilegeFlushAll\x10&\x12\x1c\n\x18PrivilegeCreatePartition\x10\'\x12\x1a\n\x16PrivilegeDropPartition\x10(\x12\x1b\n\x17PrivilegeShowPartitions\x10)\x12\x19\n\x15PrivilegeHasPartition\x10*\x12\x1a\n\x16PrivilegeGetFlushState\x10+\x12\x18\n\x14PrivilegeCreateAlias\x10,\x12\x16\n\x12PrivilegeDropAlias\x10-\x12\x1a\n\x16PrivilegeDescribeAlias\x10.\x12\x18\n\x14PrivilegeListAliases\x10/\x12!\n\x1dPrivilegeUpdateResourceGroups\x10\x30\x12\x1a\n\x16PrivilegeAlterDatabase\x10\x31*S\n\tStateCode\x12\x10\n\x0cInitializing\x10\x00\x12\x0b\n\x07Healthy\x10\x01\x12\x0c\n\x08\x41\x62normal\x10\x02\x12\x0b\n\x07StandBy\x10\x03\x12\x0c\n\x08Stopping\x10\x04*c\n\tLoadState\x12\x15\n\x11LoadStateNotExist\x10\x00\x12\x14\n\x10LoadStateNotLoad\x10\x01\x12\x14\n\x10LoadStateLoading\x10\x02\x12\x13\n\x0fLoadStateLoaded\x10\x03:^\n\x11privilege_ext_obj\x12\x1f.google.protobuf.MessageOptions\x18\xe9\x07 \x01(\x0b\x32!.milvus.proto.common.PrivilegeExtBm\n\x0eio.milvus.grpcB\x0b\x43ommonProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\016io.milvus.grpcB\013CommonProtoP\001Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\240\001\001\252\002\022Milvus.Client.Grpc'
@@ -31,40 +31,40 @@
   _globals['_STATUS'].fields_by_name['error_code']._serialized_options = b'\030\001'
   _globals['_MSGBASE_PROPERTIESENTRY']._options = None
   _globals['_MSGBASE_PROPERTIESENTRY']._serialized_options = b'8\001'
   _globals['_CLIENTINFO_RESERVEDENTRY']._options = None
   _globals['_CLIENTINFO_RESERVEDENTRY']._serialized_options = b'8\001'
   _globals['_SERVERINFO_RESERVEDENTRY']._options = None
   _globals['_SERVERINFO_RESERVEDENTRY']._serialized_options = b'8\001'
-  _globals['_ERRORCODE']._serialized_start=1899
-  _globals['_ERRORCODE']._serialized_end=3250
-  _globals['_INDEXSTATE']._serialized_start=3252
-  _globals['_INDEXSTATE']._serialized_end=3351
-  _globals['_SEGMENTSTATE']._serialized_start=3354
-  _globals['_SEGMENTSTATE']._serialized_end=3484
-  _globals['_PLACEHOLDERTYPE']._serialized_start=3487
-  _globals['_PLACEHOLDERTYPE']._serialized_end=3635
-  _globals['_MSGTYPE']._serialized_start=3638
-  _globals['_MSGTYPE']._serialized_end=5782
-  _globals['_DSLTYPE']._serialized_start=5784
-  _globals['_DSLTYPE']._serialized_end=5818
-  _globals['_COMPACTIONSTATE']._serialized_start=5820
-  _globals['_COMPACTIONSTATE']._serialized_end=5886
-  _globals['_CONSISTENCYLEVEL']._serialized_start=5888
-  _globals['_CONSISTENCYLEVEL']._serialized_end=5976
-  _globals['_IMPORTSTATE']._serialized_start=5979
-  _globals['_IMPORTSTATE']._serialized_end=6137
-  _globals['_OBJECTTYPE']._serialized_start=6139
-  _globals['_OBJECTTYPE']._serialized_end=6189
-  _globals['_OBJECTPRIVILEGE']._serialized_start=6192
-  _globals['_OBJECTPRIVILEGE']._serialized_end=7530
-  _globals['_STATECODE']._serialized_start=7532
-  _globals['_STATECODE']._serialized_end=7615
-  _globals['_LOADSTATE']._serialized_start=7617
-  _globals['_LOADSTATE']._serialized_end=7716
+  _globals['_ERRORCODE']._serialized_start=1900
+  _globals['_ERRORCODE']._serialized_end=3251
+  _globals['_INDEXSTATE']._serialized_start=3253
+  _globals['_INDEXSTATE']._serialized_end=3352
+  _globals['_SEGMENTSTATE']._serialized_start=3355
+  _globals['_SEGMENTSTATE']._serialized_end=3485
+  _globals['_PLACEHOLDERTYPE']._serialized_start=3488
+  _globals['_PLACEHOLDERTYPE']._serialized_end=3636
+  _globals['_MSGTYPE']._serialized_start=3639
+  _globals['_MSGTYPE']._serialized_end=5783
+  _globals['_DSLTYPE']._serialized_start=5785
+  _globals['_DSLTYPE']._serialized_end=5819
+  _globals['_COMPACTIONSTATE']._serialized_start=5821
+  _globals['_COMPACTIONSTATE']._serialized_end=5887
+  _globals['_CONSISTENCYLEVEL']._serialized_start=5889
+  _globals['_CONSISTENCYLEVEL']._serialized_end=5977
+  _globals['_IMPORTSTATE']._serialized_start=5980
+  _globals['_IMPORTSTATE']._serialized_end=6138
+  _globals['_OBJECTTYPE']._serialized_start=6140
+  _globals['_OBJECTTYPE']._serialized_end=6190
+  _globals['_OBJECTPRIVILEGE']._serialized_start=6193
+  _globals['_OBJECTPRIVILEGE']._serialized_end=7559
+  _globals['_STATECODE']._serialized_start=7561
+  _globals['_STATECODE']._serialized_end=7644
+  _globals['_LOADSTATE']._serialized_start=7646
+  _globals['_LOADSTATE']._serialized_end=7745
   _globals['_STATUS']._serialized_start=72
   _globals['_STATUS']._serialized_end=315
   _globals['_STATUS_EXTRAINFOENTRY']._serialized_start=267
   _globals['_STATUS_EXTRAINFOENTRY']._serialized_end=315
   _globals['_KEYVALUEPAIR']._serialized_start=317
   _globals['_KEYVALUEPAIR']._serialized_end=359
   _globals['_KEYDATAPAIR']._serialized_start=361
@@ -96,9 +96,9 @@
   _globals['_CLIENTINFO_RESERVEDENTRY']._serialized_start=1556
   _globals['_CLIENTINFO_RESERVEDENTRY']._serialized_end=1603
   _globals['_SERVERINFO']._serialized_start=1606
   _globals['_SERVERINFO']._serialized_end=1833
   _globals['_SERVERINFO_RESERVEDENTRY']._serialized_start=1556
   _globals['_SERVERINFO_RESERVEDENTRY']._serialized_end=1603
   _globals['_NODEINFO']._serialized_start=1835
-  _globals['_NODEINFO']._serialized_end=1896
+  _globals['_NODEINFO']._serialized_end=1897
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/common_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,15 @@
     PrivilegeHasPartition: _ClassVar[ObjectPrivilege]
     PrivilegeGetFlushState: _ClassVar[ObjectPrivilege]
     PrivilegeCreateAlias: _ClassVar[ObjectPrivilege]
     PrivilegeDropAlias: _ClassVar[ObjectPrivilege]
     PrivilegeDescribeAlias: _ClassVar[ObjectPrivilege]
     PrivilegeListAliases: _ClassVar[ObjectPrivilege]
     PrivilegeUpdateResourceGroups: _ClassVar[ObjectPrivilege]
+    PrivilegeAlterDatabase: _ClassVar[ObjectPrivilege]
 
 class StateCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     Initializing: _ClassVar[StateCode]
     Healthy: _ClassVar[StateCode]
     Abnormal: _ClassVar[StateCode]
     StandBy: _ClassVar[StateCode]
@@ -554,14 +555,15 @@
 PrivilegeHasPartition: ObjectPrivilege
 PrivilegeGetFlushState: ObjectPrivilege
 PrivilegeCreateAlias: ObjectPrivilege
 PrivilegeDropAlias: ObjectPrivilege
 PrivilegeDescribeAlias: ObjectPrivilege
 PrivilegeListAliases: ObjectPrivilege
 PrivilegeUpdateResourceGroups: ObjectPrivilege
+PrivilegeAlterDatabase: ObjectPrivilege
 Initializing: StateCode
 Healthy: StateCode
 Abnormal: StateCode
 StandBy: StateCode
 Stopping: StateCode
 LoadStateNotExist: LoadState
 LoadStateNotLoad: LoadState
@@ -749,15 +751,15 @@
     git_commit: str
     go_version: str
     deploy_mode: str
     reserved: _containers.ScalarMap[str, str]
     def __init__(self, build_tags: _Optional[str] = ..., build_time: _Optional[str] = ..., git_commit: _Optional[str] = ..., go_version: _Optional[str] = ..., deploy_mode: _Optional[str] = ..., reserved: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class NodeInfo(_message.Message):
-    __slots__ = ("nodeID", "address", "hostname")
-    NODEID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ("node_id", "address", "hostname")
+    NODE_ID_FIELD_NUMBER: _ClassVar[int]
     ADDRESS_FIELD_NUMBER: _ClassVar[int]
     HOSTNAME_FIELD_NUMBER: _ClassVar[int]
-    nodeID: int
+    node_id: int
     address: str
     hostname: str
-    def __init__(self, nodeID: _Optional[int] = ..., address: _Optional[str] = ..., hostname: _Optional[str] = ...) -> None: ...
+    def __init__(self, node_id: _Optional[int] = ..., address: _Optional[str] = ..., hostname: _Optional[str] = ...) -> None: ...
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/feder_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/feder_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from . import rg_pb2 as rg__pb2
 from . import schema_pb2 as schema__pb2
 from . import feder_pb2 as feder__pb2
 from . import msg_pb2 as msg__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cmilvus.proto\x12\x13milvus.proto.milvus\x1a\x0c\x63ommon.proto\x1a\x08rg.proto\x1a\x0cschema.proto\x1a\x0b\x66\x65\x64\x65r.proto\x1a\tmsg.proto\x1a google/protobuf/descriptor.proto\"\x8d\x01\n\x12\x43reateAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x10\x44ropAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10-\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x8c\x01\n\x11\x41lterAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x14\x44\x65scribeAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10.\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"x\n\x15\x44\x65scribeAliasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t\x12\x12\n\ncollection\x18\x04 \x01(\t\"~\n\x12ListAliasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10/\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"}\n\x13ListAliasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0f\n\x07\x61liases\x18\x04 \x03(\t\"\xb8\x02\n\x17\x43reateCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\x0c\x12\x12\n\nshards_num\x18\x05 \x01(\x05\x12@\n\x11\x63onsistency_level\x18\x06 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x35\n\nproperties\x18\x07 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x16\n\x0enum_partitions\x18\x08 \x01(\x03:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x81\x01\n\x15\x44ropCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x02\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcf\x01\n\x16\x41lterCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x35\n\nproperties\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x80\x01\n\x14HasCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\ntime_stamp\x18\x04 \x01(\x04\"J\n\x0c\x42oolResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\x08\"L\n\x0eStringResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\t\"\xaf\x01\n\x19\x44\x65scribeCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x12\n\ntime_stamp\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x03\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xaa\x04\n\x1a\x44\x65scribeCollectionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x35\n\x06schema\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.CollectionSchema\x12\x14\n\x0c\x63ollectionID\x18\x03 \x01(\x03\x12\x1d\n\x15virtual_channel_names\x18\x04 \x03(\t\x12\x1e\n\x16physical_channel_names\x18\x05 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x06 \x01(\x04\x12\x1d\n\x15\x63reated_utc_timestamp\x18\x07 \x01(\x04\x12\x12\n\nshards_num\x18\x08 \x01(\x05\x12\x0f\n\x07\x61liases\x18\t \x03(\t\x12\x39\n\x0fstart_positions\x18\n \x03(\x0b\x32 .milvus.proto.common.KeyDataPair\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x17\n\x0f\x63ollection_name\x18\x0c \x01(\t\x12\x35\n\nproperties\x18\r \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x0e \x01(\t\x12\x16\n\x0enum_partitions\x18\x0f \x01(\x03\"\xb8\x01\n\x15LoadCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0ereplica_number\x18\x04 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x05 \x03(\t\x12\x0f\n\x07refresh\x18\x06 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"y\n\x18ReleaseCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x06\x18\x03\"\xab\x01\n\x14GetStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x1b\n\x13guarantee_timestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\n\x18\x03\"v\n\x15GetStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\x7f\n\x1eGetCollectionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\n\x18\x03\"\x80\x01\n\x1fGetCollectionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xc8\x01\n\x16ShowCollectionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x12\n\ntime_stamp\x18\x03 \x01(\x04\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowType\x12\x1c\n\x10\x63ollection_names\x18\x05 \x03(\tB\x02\x18\x01:\x12\xca>\x0f\x08\x01\x10\x04\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xf7\x01\n\x17ShowCollectionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x18\n\x10\x63ollection_names\x18\x02 \x03(\t\x12\x16\n\x0e\x63ollection_ids\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\x12\x1f\n\x17query_service_available\x18\x07 \x03(\x08\"\x8f\x01\n\x16\x43reatePartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\'\x18\x03\"\x8d\x01\n\x14\x44ropPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10(\x18\x03\"\x8c\x01\n\x13HasPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10*\x18\x03\"\xd1\x01\n\x15LoadPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x16\n\x0ereplica_number\x18\x05 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x06 \x03(\t\x12\x0f\n\x07refresh\x18\x07 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"\x92\x01\n\x18ReleasePartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t:\x07\xca>\x04\x10\x06\x18\x03\"\x8d\x01\n\x1dGetPartitionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\"\x7f\n\x1eGetPartitionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xd6\x01\n\x15ShowPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x17\n\x0fpartition_names\x18\x05 \x03(\t\x12/\n\x04type\x18\x06 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowTypeB\x02\x18\x01:\x07\xca>\x04\x10)\x18\x03\"\xd2\x01\n\x16ShowPartitionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fpartition_names\x18\x02 \x03(\t\x12\x14\n\x0cpartitionIDs\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\"m\n\x16\x44\x65scribeSegmentRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x11\n\tsegmentID\x18\x03 \x01(\x03\"\x8f\x01\n\x17\x44\x65scribeSegmentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x0f\n\x07\x62uildID\x18\x03 \x01(\x03\x12\x14\n\x0c\x65nable_index\x18\x04 \x01(\x08\x12\x0f\n\x07\x66ieldID\x18\x05 \x01(\x03\"l\n\x13ShowSegmentsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\"W\n\x14ShowSegmentsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x12\n\nsegmentIDs\x18\x02 \x03(\x03\"\xd4\x01\n\x12\x43reateIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nindex_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x0b\x18\x03\"\xbf\x01\n\x11\x41lterIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x07\xca>\x04\x10\x0b\x18\x03\"\xb0\x01\n\x14\x44\x65scribeIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x95\x02\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x31\n\x06params\x18\x03 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x14\n\x0cindexed_rows\x18\x05 \x01(\x03\x12\x12\n\ntotal_rows\x18\x06 \x01(\x03\x12.\n\x05state\x18\x07 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x1f\n\x17index_state_fail_reason\x18\x08 \x01(\t\x12\x1a\n\x12pending_index_rows\x18\t \x01(\x03\"\x87\x01\n\x15\x44\x65scribeIndexResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"\xa5\x01\n\x1cGetIndexBuildProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"v\n\x1dGetIndexBuildProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0cindexed_rows\x18\x02 \x01(\x03\x12\x12\n\ntotal_rows\x18\x03 \x01(\x03\"\x9d\x01\n\x14GetIndexStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"\x89\x01\n\x15GetIndexStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\t\"\x99\x01\n\x10\x44ropIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\r\x18\x03\"\xe0\x01\n\rInsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x08\x18\x03\"\xe0\x01\n\rUpsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x19\x18\x03\"\xf0\x01\n\x0eMutationResult\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12%\n\x03IDs\x18\x02 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x12\n\nsucc_index\x18\x03 \x03(\r\x12\x11\n\terr_index\x18\x04 \x03(\r\x12\x14\n\x0c\x61\x63knowledged\x18\x05 \x01(\x08\x12\x12\n\ninsert_cnt\x18\x06 \x01(\x03\x12\x12\n\ndelete_cnt\x18\x07 \x01(\x03\x12\x12\n\nupsert_cnt\x18\x08 \x01(\x03\x12\x11\n\ttimestamp\x18\t \x01(\x04\"\xe9\x01\n\rDeleteRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x05 \x01(\t\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12@\n\x11\x63onsistency_level\x18\x07 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel:\x07\xca>\x04\x10\t\x18\x03\"\xb0\x01\n\x10SubSearchRequest\x12\x0b\n\x03\x64sl\x18\x01 \x01(\t\x12\x19\n\x11placeholder_group\x18\x02 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x03 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x38\n\rsearch_params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02nq\x18\x05 \x01(\x03\"\xcc\x04\n\rSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x0b\n\x03\x64sl\x18\x05 \x01(\t\x12\x19\n\x11placeholder_group\x18\x06 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x07 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x15\n\routput_fields\x18\x08 \x03(\t\x12\x38\n\rsearch_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\n \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x0b \x01(\x04\x12\n\n\x02nq\x18\x0c \x01(\x03\x12\x1b\n\x13not_return_all_meta\x18\r \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0e \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0f \x01(\x08\x12\x1e\n\x16search_by_primary_keys\x18\x10 \x01(\x08\x12\x37\n\x08sub_reqs\x18\x11 \x03(\x0b\x32%.milvus.proto.milvus.SubSearchRequest:\x07\xca>\x04\x10\x0e\x18\x03\"5\n\x04Hits\x12\x0b\n\x03IDs\x18\x01 \x03(\x03\x12\x10\n\x08row_data\x18\x02 \x03(\x0c\x12\x0e\n\x06scores\x18\x03 \x03(\x02\"\x8d\x01\n\rSearchResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x36\n\x07results\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.SearchResultData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\"\xc9\x03\n\x13HybridSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x34\n\x08requests\x18\x05 \x03(\x0b\x32\".milvus.proto.milvus.SearchRequest\x12\x36\n\x0brank_params\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x1b\n\x13not_return_all_meta\x18\t \x01(\x08\x12\x15\n\routput_fields\x18\n \x03(\t\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x0e\x18\x03\"n\n\x0c\x46lushRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t:\x07\xca>\x04\x10\x0f \x03\"\x9b\x05\n\rFlushResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12G\n\x0b\x63oll_segIDs\x18\x03 \x03(\x0b\x32\x32.milvus.proto.milvus.FlushResponse.CollSegIDsEntry\x12R\n\x11\x66lush_coll_segIDs\x18\x04 \x03(\x0b\x32\x37.milvus.proto.milvus.FlushResponse.FlushCollSegIDsEntry\x12N\n\x0f\x63oll_seal_times\x18\x05 \x03(\x0b\x32\x35.milvus.proto.milvus.FlushResponse.CollSealTimesEntry\x12J\n\rcoll_flush_ts\x18\x06 \x03(\x0b\x32\x33.milvus.proto.milvus.FlushResponse.CollFlushTsEntry\x1aQ\n\x0f\x43ollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1aV\n\x14\x46lushCollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1a\x34\n\x12\x43ollSealTimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x1a\x32\n\x10\x43ollFlushTsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\"\x9b\x03\n\x0cQueryRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x04 \x01(\t\x12\x15\n\routput_fields\x18\x05 \x03(\t\x12\x17\n\x0fpartition_names\x18\x06 \x03(\t\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x37\n\x0cquery_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x1b\n\x13not_return_all_meta\x18\n \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x10\x18\x03\"\xa0\x01\n\x0cQueryResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x0b\x66ields_data\x18\x02 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x15\n\routput_fields\x18\x04 \x03(\t\"}\n\tVectorIDs\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12*\n\x08id_array\x18\x03 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\"\x83\x01\n\x0cVectorsArray\x12\x32\n\x08id_array\x18\x01 \x01(\x0b\x32\x1e.milvus.proto.milvus.VectorIDsH\x00\x12\x36\n\ndata_array\x18\x02 \x01(\x0b\x32 .milvus.proto.schema.VectorFieldH\x00\x42\x07\n\x05\x61rray\"\xdd\x01\n\x13\x43\x61lcDistanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x32\n\x07op_left\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x33\n\x08op_right\x18\x03 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x31\n\x06params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb5\x01\n\x13\x43\x61lcDistanceResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x31\n\x08int_dist\x18\x02 \x01(\x0b\x32\x1d.milvus.proto.schema.IntArrayH\x00\x12\x35\n\nfloat_dist\x18\x03 \x01(\x0b\x32\x1f.milvus.proto.schema.FloatArrayH\x00\x42\x07\n\x05\x61rray\"b\n\x0f\x46lushAllRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10&\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"U\n\x10\x46lushAllResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\"\x99\x01\n\x15PersistentSegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08num_rows\x18\x04 \x01(\x03\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.milvus.proto.common.SegmentState\"u\n\x1fGetPersistentSegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x8a\x01\n GetPersistentSegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x39\n\x05infos\x18\x02 \x03(\x0b\x32*.milvus.proto.milvus.PersistentSegmentInfo\"\xf0\x01\n\x10QuerySegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08mem_size\x18\x04 \x01(\x03\x12\x10\n\x08num_rows\x18\x05 \x01(\x03\x12\x12\n\nindex_name\x18\x06 \x01(\t\x12\x0f\n\x07indexID\x18\x07 \x01(\x03\x12\x12\n\x06nodeID\x18\x08 \x01(\x03\x42\x02\x18\x01\x12\x30\n\x05state\x18\t \x01(\x0e\x32!.milvus.proto.common.SegmentState\x12\x0f\n\x07nodeIds\x18\n \x03(\x03\"p\n\x1aGetQuerySegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x80\x01\n\x1bGetQuerySegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x05infos\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.QuerySegmentInfo\"$\n\x0c\x44ummyRequest\x12\x14\n\x0crequest_type\x18\x01 \x01(\t\"!\n\rDummyResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"\x15\n\x13RegisterLinkRequest\"r\n\x14RegisterLinkResponse\x12-\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.Address\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"P\n\x11GetMetricsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07request\x18\x02 \x01(\t\"k\n\x12GetMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08response\x18\x02 \x01(\t\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\x98\x01\n\rComponentInfo\x12\x0e\n\x06nodeID\x18\x01 \x01(\x03\x12\x0c\n\x04role\x18\x02 \x01(\t\x12\x32\n\nstate_code\x18\x03 \x01(\x0e\x32\x1e.milvus.proto.common.StateCode\x12\x35\n\nextra_info\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb2\x01\n\x0f\x43omponentStates\x12\x31\n\x05state\x18\x01 \x01(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12?\n\x13subcomponent_states\x18\x02 \x03(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"\x1b\n\x19GetComponentStatesRequest\"\xb6\x01\n\x12LoadBalanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x12\n\nsrc_nodeID\x18\x02 \x01(\x03\x12\x13\n\x0b\x64st_nodeIDs\x18\x03 \x03(\x03\x12\x19\n\x11sealed_segmentIDs\x18\x04 \x03(\x03\x12\x16\n\x0e\x63ollectionName\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x11\x18\x05\"e\n\x17ManualCompactionRequest\x12\x14\n\x0c\x63ollectionID\x18\x01 \x01(\x03\x12\x12\n\ntimetravel\x18\x02 \x01(\x04\x12\x17\n\x0fmajorCompaction\x18\x03 \x01(\x08:\x07\xca>\x04\x10\x07\x18\x01\"z\n\x18ManualCompactionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x63ompactionID\x18\x02 \x01(\x03\x12\x1b\n\x13\x63ompactionPlanCount\x18\x03 \x01(\x05\"1\n\x19GetCompactionStateRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xdd\x01\n\x1aGetCompactionStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12\x17\n\x0f\x65xecutingPlanNo\x18\x03 \x01(\x03\x12\x15\n\rtimeoutPlanNo\x18\x04 \x01(\x03\x12\x17\n\x0f\x63ompletedPlanNo\x18\x05 \x01(\x03\x12\x14\n\x0c\x66\x61iledPlanNo\x18\x06 \x01(\x03\"1\n\x19GetCompactionPlansRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xbc\x01\n\x1aGetCompactionPlansResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12<\n\nmergeInfos\x18\x03 \x03(\x0b\x32(.milvus.proto.milvus.CompactionMergeInfo\"6\n\x13\x43ompactionMergeInfo\x12\x0f\n\x07sources\x18\x01 \x03(\x03\x12\x0e\n\x06target\x18\x02 \x01(\x03\"o\n\x14GetFlushStateRequest\x12\x12\n\nsegmentIDs\x18\x01 \x03(\x03\x12\x10\n\x08\x66lush_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t:\x07\xca>\x04\x10+\x18\x04\"U\n\x15GetFlushStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"l\n\x17GetFlushAllStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"X\n\x18GetFlushAllStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"\xe0\x01\n\rImportRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0epartition_name\x18\x02 \x01(\t\x12\x15\n\rchannel_names\x18\x03 \x03(\t\x12\x11\n\trow_based\x18\x04 \x01(\x08\x12\r\n\x05\x66iles\x18\x05 \x03(\t\x12\x32\n\x07options\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x07 \x01(\t\x12\x17\n\x0f\x63lustering_info\x18\x08 \x01(\x0c:\x07\xca>\x04\x10\x12\x18\x01\"L\n\x0eImportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05tasks\x18\x02 \x03(\x03\"%\n\x15GetImportStateRequest\x12\x0c\n\x04task\x18\x01 \x01(\x03\"\x97\x02\n\x16GetImportStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12/\n\x05state\x18\x02 \x01(\x0e\x32 .milvus.proto.common.ImportState\x12\x11\n\trow_count\x18\x03 \x01(\x03\x12\x0f\n\x07id_list\x18\x04 \x03(\x03\x12\x30\n\x05infos\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02id\x18\x06 \x01(\x03\x12\x15\n\rcollection_id\x18\x07 \x01(\x03\x12\x13\n\x0bsegment_ids\x18\x08 \x03(\x03\x12\x11\n\tcreate_ts\x18\t \x01(\x03\"Q\n\x16ListImportTasksRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"\x82\x01\n\x17ListImportTasksResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x05tasks\x18\x02 \x03(\x0b\x32+.milvus.proto.milvus.GetImportStateResponse\"\x9a\x01\n\x12GetReplicasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x18\n\x10with_shard_nodes\x18\x03 \x01(\x08\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"v\n\x13GetReplicasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08replicas\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.ReplicaInfo\"\xc1\x02\n\x0bReplicaInfo\x12\x11\n\treplicaID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x15\n\rpartition_ids\x18\x03 \x03(\x03\x12\x39\n\x0eshard_replicas\x18\x04 \x03(\x0b\x32!.milvus.proto.milvus.ShardReplica\x12\x10\n\x08node_ids\x18\x05 \x03(\x03\x12\x1b\n\x13resource_group_name\x18\x06 \x01(\t\x12P\n\x11num_outbound_node\x18\x07 \x03(\x0b\x32\x35.milvus.proto.milvus.ReplicaInfo.NumOutboundNodeEntry\x1a\x36\n\x14NumOutboundNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"`\n\x0cShardReplica\x12\x10\n\x08leaderID\x18\x01 \x01(\x03\x12\x13\n\x0bleader_addr\x18\x02 \x01(\t\x12\x17\n\x0f\x64m_channel_name\x18\x03 \x01(\t\x12\x10\n\x08node_ids\x18\x04 \x03(\x03\"\xbe\x01\n\x17\x43reateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x04 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcd\x01\n\x17UpdateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x13\n\x0boldPassword\x18\x03 \x01(\t\x12\x13\n\x0bnewPassword\x18\x04 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x06 \x01(\x04:\t\xca>\x06\x08\x02\x10\x14\x18\x02\"k\n\x17\x44\x65leteCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"W\n\x15ListCredUsersResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tusernames\x18\x02 \x03(\t\"V\n\x14ListCredUsersRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x1a\n\nRoleEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1a\n\nUserEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x43reateRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12/\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"d\n\x0f\x44ropRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\trole_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb5\x01\n\x16OperateUserRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x11\n\trole_name\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.milvus.proto.milvus.OperateUserRoleType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x9d\x01\n\x11SelectRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04role\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x19\n\x11include_user_info\x18\x03 \x01(\x08:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"k\n\nRoleResult\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12.\n\x05users\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\"s\n\x12SelectRoleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleResult\"\x94\x01\n\x11SelectUserRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04user\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x19\n\x11include_role_info\x18\x03 \x01(\x08:\t\xca>\x06\x08\x02\x10\x18\x18\x02\"k\n\nUserResult\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12.\n\x05roles\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\"s\n\x12SelectUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserResult\"\x1c\n\x0cObjectEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1f\n\x0fPrivilegeEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"w\n\rGrantorEntity\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x37\n\tprivilege\x18\x02 \x01(\x0b\x32$.milvus.proto.milvus.PrivilegeEntity\"L\n\x14GrantPrivilegeEntity\x12\x34\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\".milvus.proto.milvus.GrantorEntity\"\xca\x01\n\x0bGrantEntity\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x31\n\x06object\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.ObjectEntity\x12\x13\n\x0bobject_name\x18\x03 \x01(\t\x12\x33\n\x07grantor\x18\x04 \x01(\x0b\x32\".milvus.proto.milvus.GrantorEntity\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"\x86\x01\n\x12SelectGrantRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x13SelectGrantResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08\x65ntities\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.GrantEntity\"\xc4\x01\n\x17OperatePrivilegeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).milvus.proto.milvus.OperatePrivilegeType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x93\x01\n\x19GetLoadingProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"u\n\x1aGetLoadingProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x18\n\x10refresh_progress\x18\x03 \x01(\x03\"\x8d\x01\n\x13GetLoadStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"r\n\x14GetLoadStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12-\n\x05state\x18\x02 \x01(\x0e\x32\x1e.milvus.proto.common.LoadState\"\x1c\n\tMilvusExt\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x13\n\x11GetVersionRequest\"R\n\x12GetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x14\n\x12\x43heckHealthRequest\"\x9d\x01\n\x13\x43heckHealthResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tisHealthy\x18\x02 \x01(\x08\x12\x0f\n\x07reasons\x18\x03 \x03(\t\x12\x35\n\x0cquota_states\x18\x04 \x03(\x0e\x32\x1f.milvus.proto.milvus.QuotaState\"\xaa\x01\n\x1a\x43reateResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t\x12\x34\n\x06\x63onfig\x18\x03 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x12\xca>\x0f\x08\x01\x10\x1a\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x99\x02\n\x1bUpdateResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12]\n\x0fresource_groups\x18\x02 \x03(\x0b\x32\x44.milvus.proto.milvus.UpdateResourceGroupsRequest.ResourceGroupsEntry\x1a[\n\x13ResourceGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x02\x38\x01:\x12\xca>\x0f\x08\x01\x10\x30\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x18\x44ropResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1b\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa5\x01\n\x13TransferNodeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x10\n\x08num_node\x18\x04 \x01(\x05:\x12\xca>\x0f\x08\x01\x10\x1e\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xd5\x01\n\x16TransferReplicaRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x13\n\x0bnum_replica\x18\x05 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1f\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"[\n\x19ListResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x1d\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"b\n\x1aListResourceGroupsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fresource_groups\x18\x02 \x03(\t\"v\n\x1c\x44\x65scribeResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1c\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x88\x01\n\x1d\x44\x65scribeResourceGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x0eresource_group\x18\x02 \x01(\x0b\x32\".milvus.proto.milvus.ResourceGroup\"\xd6\x04\n\rResourceGroup\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x1a\n\x12num_available_node\x18\x03 \x01(\x05\x12T\n\x12num_loaded_replica\x18\x04 \x03(\x0b\x32\x38.milvus.proto.milvus.ResourceGroup.NumLoadedReplicaEntry\x12R\n\x11num_outgoing_node\x18\x05 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumOutgoingNodeEntry\x12R\n\x11num_incoming_node\x18\x06 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumIncomingNodeEntry\x12\x34\n\x06\x63onfig\x18\x07 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig\x12,\n\x05nodes\x18\x08 \x03(\x0b\x32\x1d.milvus.proto.common.NodeInfo\x1a\x37\n\x15NumLoadedReplicaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumOutgoingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumIncomingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x9f\x01\n\x17RenameCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x0f\n\x07oldName\x18\x03 \x01(\t\x12\x0f\n\x07newName\x18\x04 \x01(\t\x12\x11\n\tnewDBName\x18\x05 \x01(\t:\x12\xca>\x0f\x08\x01\x10\"\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa1\x01\n\x19GetIndexStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x8c\x01\n\x1aGetIndexStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"r\n\x0e\x43onnectRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x34\n\x0b\x63lient_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ClientInfo\"\x88\x01\n\x0f\x43onnectResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x0bserver_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ServerInfo\x12\x12\n\nidentifier\x18\x03 \x01(\x03\"C\n\x15\x41llocTimestampRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"X\n\x16\x41llocTimestampResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\ttimestamp\x18\x02 \x01(\x04\"h\n\x15\x43reateDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10#\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"f\n\x13\x44ropDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10$\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"V\n\x14ListDatabasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10%\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x85\x01\n\x15ListDatabasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08\x64\x62_names\x18\x02 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x03 \x03(\x04:\x12\xca>\x0f\x08\x01\x10\x04\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xf5\x01\n\x17ReplicateMessageRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x42\x65ginTs\x18\x03 \x01(\x04\x12\r\n\x05\x45ndTs\x18\x04 \x01(\x04\x12\x0c\n\x04Msgs\x18\x05 \x03(\x0c\x12\x35\n\x0eStartPositions\x18\x06 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\x12\x33\n\x0c\x45ndPositions\x18\x07 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\"Y\n\x18ReplicateMessageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08position\x18\x02 \x01(\t\"b\n\x15ImportAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x16\n\x0epartition_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"<\n GetImportProgressAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"O\n\x1aListImportsAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01*%\n\x08ShowType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08InMemory\x10\x01\x1a\x02\x18\x01*@\n\x13OperateUserRoleType\x12\x11\n\rAddUserToRole\x10\x00\x12\x16\n\x12RemoveUserFromRole\x10\x01*-\n\x14OperatePrivilegeType\x12\t\n\x05Grant\x10\x00\x12\n\n\x06Revoke\x10\x01*]\n\nQuotaState\x12\x0b\n\x07Unknown\x10\x00\x12\x0f\n\x0bReadLimited\x10\x02\x12\x10\n\x0cWriteLimited\x10\x03\x12\x0e\n\nDenyToRead\x10\x04\x12\x0f\n\x0b\x44\x65nyToWrite\x10\x05\x32\xec\x42\n\rMilvusService\x12_\n\x10\x43reateCollection\x12,.milvus.proto.milvus.CreateCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12[\n\x0e\x44ropCollection\x12*.milvus.proto.milvus.DropCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\rHasCollection\x12).milvus.proto.milvus.HasCollectionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadCollection\x12*.milvus.proto.milvus.LoadCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleaseCollection\x12-.milvus.proto.milvus.ReleaseCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12\x44\x65scribeCollection\x12..milvus.proto.milvus.DescribeCollectionRequest\x1a/.milvus.proto.milvus.DescribeCollectionResponse\"\x00\x12\x86\x01\n\x17GetCollectionStatistics\x12\x33.milvus.proto.milvus.GetCollectionStatisticsRequest\x1a\x34.milvus.proto.milvus.GetCollectionStatisticsResponse\"\x00\x12n\n\x0fShowCollections\x12+.milvus.proto.milvus.ShowCollectionsRequest\x1a,.milvus.proto.milvus.ShowCollectionsResponse\"\x00\x12]\n\x0f\x41lterCollection\x12+.milvus.proto.milvus.AlterCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0f\x43reatePartition\x12+.milvus.proto.milvus.CreatePartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Y\n\rDropPartition\x12).milvus.proto.milvus.DropPartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0cHasPartition\x12(.milvus.proto.milvus.HasPartitionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadPartitions\x12*.milvus.proto.milvus.LoadPartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleasePartitions\x12-.milvus.proto.milvus.ReleasePartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x83\x01\n\x16GetPartitionStatistics\x12\x32.milvus.proto.milvus.GetPartitionStatisticsRequest\x1a\x33.milvus.proto.milvus.GetPartitionStatisticsResponse\"\x00\x12k\n\x0eShowPartitions\x12*.milvus.proto.milvus.ShowPartitionsRequest\x1a+.milvus.proto.milvus.ShowPartitionsResponse\"\x00\x12w\n\x12GetLoadingProgress\x12..milvus.proto.milvus.GetLoadingProgressRequest\x1a/.milvus.proto.milvus.GetLoadingProgressResponse\"\x00\x12\x65\n\x0cGetLoadState\x12(.milvus.proto.milvus.GetLoadStateRequest\x1a).milvus.proto.milvus.GetLoadStateResponse\"\x00\x12U\n\x0b\x43reateAlias\x12\'.milvus.proto.milvus.CreateAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Q\n\tDropAlias\x12%.milvus.proto.milvus.DropAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterAlias\x12&.milvus.proto.milvus.AlterAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeAlias\x12).milvus.proto.milvus.DescribeAliasRequest\x1a*.milvus.proto.milvus.DescribeAliasResponse\"\x00\x12\x62\n\x0bListAliases\x12\'.milvus.proto.milvus.ListAliasesRequest\x1a(.milvus.proto.milvus.ListAliasesResponse\"\x00\x12U\n\x0b\x43reateIndex\x12\'.milvus.proto.milvus.CreateIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterIndex\x12&.milvus.proto.milvus.AlterIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeIndex\x12).milvus.proto.milvus.DescribeIndexRequest\x1a*.milvus.proto.milvus.DescribeIndexResponse\"\x00\x12w\n\x12GetIndexStatistics\x12..milvus.proto.milvus.GetIndexStatisticsRequest\x1a/.milvus.proto.milvus.GetIndexStatisticsResponse\"\x00\x12k\n\rGetIndexState\x12).milvus.proto.milvus.GetIndexStateRequest\x1a*.milvus.proto.milvus.GetIndexStateResponse\"\x03\x88\x02\x01\x12\x83\x01\n\x15GetIndexBuildProgress\x12\x31.milvus.proto.milvus.GetIndexBuildProgressRequest\x1a\x32.milvus.proto.milvus.GetIndexBuildProgressResponse\"\x03\x88\x02\x01\x12Q\n\tDropIndex\x12%.milvus.proto.milvus.DropIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\x06Insert\x12\".milvus.proto.milvus.InsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06\x44\x65lete\x12\".milvus.proto.milvus.DeleteRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06Upsert\x12\".milvus.proto.milvus.UpsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12R\n\x06Search\x12\".milvus.proto.milvus.SearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12^\n\x0cHybridSearch\x12(.milvus.proto.milvus.HybridSearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12P\n\x05\x46lush\x12!.milvus.proto.milvus.FlushRequest\x1a\".milvus.proto.milvus.FlushResponse\"\x00\x12O\n\x05Query\x12!.milvus.proto.milvus.QueryRequest\x1a!.milvus.proto.milvus.QueryResults\"\x00\x12\x64\n\x0c\x43\x61lcDistance\x12(.milvus.proto.milvus.CalcDistanceRequest\x1a(.milvus.proto.milvus.CalcDistanceResults\"\x00\x12Y\n\x08\x46lushAll\x12$.milvus.proto.milvus.FlushAllRequest\x1a%.milvus.proto.milvus.FlushAllResponse\"\x00\x12h\n\rGetFlushState\x12).milvus.proto.milvus.GetFlushStateRequest\x1a*.milvus.proto.milvus.GetFlushStateResponse\"\x00\x12q\n\x10GetFlushAllState\x12,.milvus.proto.milvus.GetFlushAllStateRequest\x1a-.milvus.proto.milvus.GetFlushAllStateResponse\"\x00\x12\x89\x01\n\x18GetPersistentSegmentInfo\x12\x34.milvus.proto.milvus.GetPersistentSegmentInfoRequest\x1a\x35.milvus.proto.milvus.GetPersistentSegmentInfoResponse\"\x00\x12z\n\x13GetQuerySegmentInfo\x12/.milvus.proto.milvus.GetQuerySegmentInfoRequest\x1a\x30.milvus.proto.milvus.GetQuerySegmentInfoResponse\"\x00\x12\x62\n\x0bGetReplicas\x12\'.milvus.proto.milvus.GetReplicasRequest\x1a(.milvus.proto.milvus.GetReplicasResponse\"\x00\x12P\n\x05\x44ummy\x12!.milvus.proto.milvus.DummyRequest\x1a\".milvus.proto.milvus.DummyResponse\"\x00\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00\x12_\n\nGetMetrics\x12&.milvus.proto.milvus.GetMetricsRequest\x1a\'.milvus.proto.milvus.GetMetricsResponse\"\x00\x12l\n\x12GetComponentStates\x12..milvus.proto.milvus.GetComponentStatesRequest\x1a$.milvus.proto.milvus.ComponentStates\"\x00\x12U\n\x0bLoadBalance\x12\'.milvus.proto.milvus.LoadBalanceRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12GetCompactionState\x12..milvus.proto.milvus.GetCompactionStateRequest\x1a/.milvus.proto.milvus.GetCompactionStateResponse\"\x00\x12q\n\x10ManualCompaction\x12,.milvus.proto.milvus.ManualCompactionRequest\x1a-.milvus.proto.milvus.ManualCompactionResponse\"\x00\x12\x80\x01\n\x1bGetCompactionStateWithPlans\x12..milvus.proto.milvus.GetCompactionPlansRequest\x1a/.milvus.proto.milvus.GetCompactionPlansResponse\"\x00\x12S\n\x06Import\x12\".milvus.proto.milvus.ImportRequest\x1a#.milvus.proto.milvus.ImportResponse\"\x00\x12k\n\x0eGetImportState\x12*.milvus.proto.milvus.GetImportStateRequest\x1a+.milvus.proto.milvus.GetImportStateResponse\"\x00\x12n\n\x0fListImportTasks\x12+.milvus.proto.milvus.ListImportTasksRequest\x1a,.milvus.proto.milvus.ListImportTasksResponse\"\x00\x12_\n\x10\x43reateCredential\x12,.milvus.proto.milvus.CreateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10UpdateCredential\x12,.milvus.proto.milvus.UpdateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10\x44\x65leteCredential\x12,.milvus.proto.milvus.DeleteCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListCredUsers\x12).milvus.proto.milvus.ListCredUsersRequest\x1a*.milvus.proto.milvus.ListCredUsersResponse\"\x00\x12S\n\nCreateRole\x12&.milvus.proto.milvus.CreateRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12O\n\x08\x44ropRole\x12$.milvus.proto.milvus.DropRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fOperateUserRole\x12+.milvus.proto.milvus.OperateUserRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\nSelectRole\x12&.milvus.proto.milvus.SelectRoleRequest\x1a\'.milvus.proto.milvus.SelectRoleResponse\"\x00\x12_\n\nSelectUser\x12&.milvus.proto.milvus.SelectUserRequest\x1a\'.milvus.proto.milvus.SelectUserResponse\"\x00\x12_\n\x10OperatePrivilege\x12,.milvus.proto.milvus.OperatePrivilegeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x62\n\x0bSelectGrant\x12\'.milvus.proto.milvus.SelectGrantRequest\x1a(.milvus.proto.milvus.SelectGrantResponse\"\x00\x12_\n\nGetVersion\x12&.milvus.proto.milvus.GetVersionRequest\x1a\'.milvus.proto.milvus.GetVersionResponse\"\x00\x12\x62\n\x0b\x43heckHealth\x12\'.milvus.proto.milvus.CheckHealthRequest\x1a(.milvus.proto.milvus.CheckHealthResponse\"\x00\x12\x65\n\x13\x43reateResourceGroup\x12/.milvus.proto.milvus.CreateResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11\x44ropResourceGroup\x12-.milvus.proto.milvus.DropResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12g\n\x14UpdateResourceGroups\x12\x30.milvus.proto.milvus.UpdateResourceGroupsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0cTransferNode\x12(.milvus.proto.milvus.TransferNodeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fTransferReplica\x12+.milvus.proto.milvus.TransferReplicaRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12ListResourceGroups\x12..milvus.proto.milvus.ListResourceGroupsRequest\x1a/.milvus.proto.milvus.ListResourceGroupsResponse\"\x00\x12\x80\x01\n\x15\x44\x65scribeResourceGroup\x12\x31.milvus.proto.milvus.DescribeResourceGroupRequest\x1a\x32.milvus.proto.milvus.DescribeResourceGroupResponse\"\x00\x12_\n\x10RenameCollection\x12,.milvus.proto.milvus.RenameCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12u\n\x12ListIndexedSegment\x12-.milvus.proto.feder.ListIndexedSegmentRequest\x1a..milvus.proto.feder.ListIndexedSegmentResponse\"\x00\x12\x87\x01\n\x18\x44\x65scribeSegmentIndexData\x12\x33.milvus.proto.feder.DescribeSegmentIndexDataRequest\x1a\x34.milvus.proto.feder.DescribeSegmentIndexDataResponse\"\x00\x12V\n\x07\x43onnect\x12#.milvus.proto.milvus.ConnectRequest\x1a$.milvus.proto.milvus.ConnectResponse\"\x00\x12k\n\x0e\x41llocTimestamp\x12*.milvus.proto.milvus.AllocTimestampRequest\x1a+.milvus.proto.milvus.AllocTimestampResponse\"\x00\x12[\n\x0e\x43reateDatabase\x12*.milvus.proto.milvus.CreateDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0c\x44ropDatabase\x12(.milvus.proto.milvus.DropDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListDatabases\x12).milvus.proto.milvus.ListDatabasesRequest\x1a*.milvus.proto.milvus.ListDatabasesResponse\"\x00\x12q\n\x10ReplicateMessage\x12,.milvus.proto.milvus.ReplicateMessageRequest\x1a-.milvus.proto.milvus.ReplicateMessageResponse\"\x00\x32u\n\x0cProxyService\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00:U\n\x0emilvus_ext_obj\x12\x1c.google.protobuf.FileOptions\x18\xe9\x07 \x01(\x0b\x32\x1e.milvus.proto.milvus.MilvusExtBm\n\x0eio.milvus.grpcB\x0bMilvusProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cmilvus.proto\x12\x13milvus.proto.milvus\x1a\x0c\x63ommon.proto\x1a\x08rg.proto\x1a\x0cschema.proto\x1a\x0b\x66\x65\x64\x65r.proto\x1a\tmsg.proto\x1a google/protobuf/descriptor.proto\"\x8d\x01\n\x12\x43reateAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x10\x44ropAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10-\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x8c\x01\n\x11\x41lterAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x14\x44\x65scribeAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10.\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"x\n\x15\x44\x65scribeAliasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t\x12\x12\n\ncollection\x18\x04 \x01(\t\"~\n\x12ListAliasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10/\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"}\n\x13ListAliasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0f\n\x07\x61liases\x18\x04 \x03(\t\"\xb8\x02\n\x17\x43reateCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\x0c\x12\x12\n\nshards_num\x18\x05 \x01(\x05\x12@\n\x11\x63onsistency_level\x18\x06 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x35\n\nproperties\x18\x07 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x16\n\x0enum_partitions\x18\x08 \x01(\x03:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x81\x01\n\x15\x44ropCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x02\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcf\x01\n\x16\x41lterCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x35\n\nproperties\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x80\x01\n\x14HasCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\ntime_stamp\x18\x04 \x01(\x04\"J\n\x0c\x42oolResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\x08\"L\n\x0eStringResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\t\"\xaf\x01\n\x19\x44\x65scribeCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x12\n\ntime_stamp\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x03\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb9\x04\n\x1a\x44\x65scribeCollectionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x35\n\x06schema\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.CollectionSchema\x12\x14\n\x0c\x63ollectionID\x18\x03 \x01(\x03\x12\x1d\n\x15virtual_channel_names\x18\x04 \x03(\t\x12\x1e\n\x16physical_channel_names\x18\x05 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x06 \x01(\x04\x12\x1d\n\x15\x63reated_utc_timestamp\x18\x07 \x01(\x04\x12\x12\n\nshards_num\x18\x08 \x01(\x05\x12\x0f\n\x07\x61liases\x18\t \x03(\t\x12\x39\n\x0fstart_positions\x18\n \x03(\x0b\x32 .milvus.proto.common.KeyDataPair\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x17\n\x0f\x63ollection_name\x18\x0c \x01(\t\x12\x35\n\nproperties\x18\r \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x0e \x01(\t\x12\x16\n\x0enum_partitions\x18\x0f \x01(\x03\x12\r\n\x05\x64\x62_id\x18\x10 \x01(\x03\"\xb8\x01\n\x15LoadCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0ereplica_number\x18\x04 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x05 \x03(\t\x12\x0f\n\x07refresh\x18\x06 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"y\n\x18ReleaseCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x06\x18\x03\"\xab\x01\n\x14GetStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x1b\n\x13guarantee_timestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\n\x18\x03\"v\n\x15GetStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\x7f\n\x1eGetCollectionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\n\x18\x03\"\x80\x01\n\x1fGetCollectionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb4\x01\n\x16ShowCollectionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x12\n\ntime_stamp\x18\x03 \x01(\x04\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowType\x12\x1c\n\x10\x63ollection_names\x18\x05 \x03(\tB\x02\x18\x01\"\xf7\x01\n\x17ShowCollectionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x18\n\x10\x63ollection_names\x18\x02 \x03(\t\x12\x16\n\x0e\x63ollection_ids\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\x12\x1f\n\x17query_service_available\x18\x07 \x03(\x08\"\x8f\x01\n\x16\x43reatePartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\'\x18\x03\"\x8d\x01\n\x14\x44ropPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10(\x18\x03\"\x8c\x01\n\x13HasPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10*\x18\x03\"\xd1\x01\n\x15LoadPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x16\n\x0ereplica_number\x18\x05 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x06 \x03(\t\x12\x0f\n\x07refresh\x18\x07 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"\x92\x01\n\x18ReleasePartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t:\x07\xca>\x04\x10\x06\x18\x03\"\x8d\x01\n\x1dGetPartitionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\"\x7f\n\x1eGetPartitionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xd6\x01\n\x15ShowPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x17\n\x0fpartition_names\x18\x05 \x03(\t\x12/\n\x04type\x18\x06 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowTypeB\x02\x18\x01:\x07\xca>\x04\x10)\x18\x03\"\xd2\x01\n\x16ShowPartitionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fpartition_names\x18\x02 \x03(\t\x12\x14\n\x0cpartitionIDs\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\"m\n\x16\x44\x65scribeSegmentRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x11\n\tsegmentID\x18\x03 \x01(\x03\"\x8f\x01\n\x17\x44\x65scribeSegmentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x0f\n\x07\x62uildID\x18\x03 \x01(\x03\x12\x14\n\x0c\x65nable_index\x18\x04 \x01(\x08\x12\x0f\n\x07\x66ieldID\x18\x05 \x01(\x03\"l\n\x13ShowSegmentsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\"W\n\x14ShowSegmentsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x12\n\nsegmentIDs\x18\x02 \x03(\x03\"\xd4\x01\n\x12\x43reateIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nindex_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x0b\x18\x03\"\xbf\x01\n\x11\x41lterIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x07\xca>\x04\x10\x0b\x18\x03\"\xb0\x01\n\x14\x44\x65scribeIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x95\x02\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x31\n\x06params\x18\x03 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x14\n\x0cindexed_rows\x18\x05 \x01(\x03\x12\x12\n\ntotal_rows\x18\x06 \x01(\x03\x12.\n\x05state\x18\x07 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x1f\n\x17index_state_fail_reason\x18\x08 \x01(\t\x12\x1a\n\x12pending_index_rows\x18\t \x01(\x03\"\x87\x01\n\x15\x44\x65scribeIndexResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"\xa5\x01\n\x1cGetIndexBuildProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"v\n\x1dGetIndexBuildProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0cindexed_rows\x18\x02 \x01(\x03\x12\x12\n\ntotal_rows\x18\x03 \x01(\x03\"\x9d\x01\n\x14GetIndexStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"\x89\x01\n\x15GetIndexStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\t\"\x99\x01\n\x10\x44ropIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\r\x18\x03\"\xe0\x01\n\rInsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x08\x18\x03\"\xe0\x01\n\rUpsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x19\x18\x03\"\xf0\x01\n\x0eMutationResult\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12%\n\x03IDs\x18\x02 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x12\n\nsucc_index\x18\x03 \x03(\r\x12\x11\n\terr_index\x18\x04 \x03(\r\x12\x14\n\x0c\x61\x63knowledged\x18\x05 \x01(\x08\x12\x12\n\ninsert_cnt\x18\x06 \x01(\x03\x12\x12\n\ndelete_cnt\x18\x07 \x01(\x03\x12\x12\n\nupsert_cnt\x18\x08 \x01(\x03\x12\x11\n\ttimestamp\x18\t \x01(\x04\"\xe9\x01\n\rDeleteRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x05 \x01(\t\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12@\n\x11\x63onsistency_level\x18\x07 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel:\x07\xca>\x04\x10\t\x18\x03\"\xb0\x01\n\x10SubSearchRequest\x12\x0b\n\x03\x64sl\x18\x01 \x01(\t\x12\x19\n\x11placeholder_group\x18\x02 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x03 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x38\n\rsearch_params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02nq\x18\x05 \x01(\x03\"\xcc\x04\n\rSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x0b\n\x03\x64sl\x18\x05 \x01(\t\x12\x19\n\x11placeholder_group\x18\x06 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x07 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x15\n\routput_fields\x18\x08 \x03(\t\x12\x38\n\rsearch_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\n \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x0b \x01(\x04\x12\n\n\x02nq\x18\x0c \x01(\x03\x12\x1b\n\x13not_return_all_meta\x18\r \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0e \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0f \x01(\x08\x12\x1e\n\x16search_by_primary_keys\x18\x10 \x01(\x08\x12\x37\n\x08sub_reqs\x18\x11 \x03(\x0b\x32%.milvus.proto.milvus.SubSearchRequest:\x07\xca>\x04\x10\x0e\x18\x03\"5\n\x04Hits\x12\x0b\n\x03IDs\x18\x01 \x03(\x03\x12\x10\n\x08row_data\x18\x02 \x03(\x0c\x12\x0e\n\x06scores\x18\x03 \x03(\x02\"\x8d\x01\n\rSearchResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x36\n\x07results\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.SearchResultData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\"\xc9\x03\n\x13HybridSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x34\n\x08requests\x18\x05 \x03(\x0b\x32\".milvus.proto.milvus.SearchRequest\x12\x36\n\x0brank_params\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x1b\n\x13not_return_all_meta\x18\t \x01(\x08\x12\x15\n\routput_fields\x18\n \x03(\t\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x0e\x18\x03\"n\n\x0c\x46lushRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t:\x07\xca>\x04\x10\x0f \x03\"\x9b\x05\n\rFlushResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12G\n\x0b\x63oll_segIDs\x18\x03 \x03(\x0b\x32\x32.milvus.proto.milvus.FlushResponse.CollSegIDsEntry\x12R\n\x11\x66lush_coll_segIDs\x18\x04 \x03(\x0b\x32\x37.milvus.proto.milvus.FlushResponse.FlushCollSegIDsEntry\x12N\n\x0f\x63oll_seal_times\x18\x05 \x03(\x0b\x32\x35.milvus.proto.milvus.FlushResponse.CollSealTimesEntry\x12J\n\rcoll_flush_ts\x18\x06 \x03(\x0b\x32\x33.milvus.proto.milvus.FlushResponse.CollFlushTsEntry\x1aQ\n\x0f\x43ollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1aV\n\x14\x46lushCollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1a\x34\n\x12\x43ollSealTimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x1a\x32\n\x10\x43ollFlushTsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\"\x9b\x03\n\x0cQueryRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x04 \x01(\t\x12\x15\n\routput_fields\x18\x05 \x03(\t\x12\x17\n\x0fpartition_names\x18\x06 \x03(\t\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x37\n\x0cquery_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x1b\n\x13not_return_all_meta\x18\n \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x10\x18\x03\"\xa0\x01\n\x0cQueryResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x0b\x66ields_data\x18\x02 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x15\n\routput_fields\x18\x04 \x03(\t\"}\n\tVectorIDs\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12*\n\x08id_array\x18\x03 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\"\x83\x01\n\x0cVectorsArray\x12\x32\n\x08id_array\x18\x01 \x01(\x0b\x32\x1e.milvus.proto.milvus.VectorIDsH\x00\x12\x36\n\ndata_array\x18\x02 \x01(\x0b\x32 .milvus.proto.schema.VectorFieldH\x00\x42\x07\n\x05\x61rray\"\xdd\x01\n\x13\x43\x61lcDistanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x32\n\x07op_left\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x33\n\x08op_right\x18\x03 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x31\n\x06params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb5\x01\n\x13\x43\x61lcDistanceResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x31\n\x08int_dist\x18\x02 \x01(\x0b\x32\x1d.milvus.proto.schema.IntArrayH\x00\x12\x35\n\nfloat_dist\x18\x03 \x01(\x0b\x32\x1f.milvus.proto.schema.FloatArrayH\x00\x42\x07\n\x05\x61rray\"b\n\x0f\x46lushAllRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10&\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"U\n\x10\x46lushAllResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\"\x99\x01\n\x15PersistentSegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08num_rows\x18\x04 \x01(\x03\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.milvus.proto.common.SegmentState\"u\n\x1fGetPersistentSegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x8a\x01\n GetPersistentSegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x39\n\x05infos\x18\x02 \x03(\x0b\x32*.milvus.proto.milvus.PersistentSegmentInfo\"\xf0\x01\n\x10QuerySegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08mem_size\x18\x04 \x01(\x03\x12\x10\n\x08num_rows\x18\x05 \x01(\x03\x12\x12\n\nindex_name\x18\x06 \x01(\t\x12\x0f\n\x07indexID\x18\x07 \x01(\x03\x12\x12\n\x06nodeID\x18\x08 \x01(\x03\x42\x02\x18\x01\x12\x30\n\x05state\x18\t \x01(\x0e\x32!.milvus.proto.common.SegmentState\x12\x0f\n\x07nodeIds\x18\n \x03(\x03\"p\n\x1aGetQuerySegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x80\x01\n\x1bGetQuerySegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x05infos\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.QuerySegmentInfo\"$\n\x0c\x44ummyRequest\x12\x14\n\x0crequest_type\x18\x01 \x01(\t\"!\n\rDummyResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"\x15\n\x13RegisterLinkRequest\"r\n\x14RegisterLinkResponse\x12-\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.Address\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"P\n\x11GetMetricsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07request\x18\x02 \x01(\t\"k\n\x12GetMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08response\x18\x02 \x01(\t\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\x98\x01\n\rComponentInfo\x12\x0e\n\x06nodeID\x18\x01 \x01(\x03\x12\x0c\n\x04role\x18\x02 \x01(\t\x12\x32\n\nstate_code\x18\x03 \x01(\x0e\x32\x1e.milvus.proto.common.StateCode\x12\x35\n\nextra_info\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb2\x01\n\x0f\x43omponentStates\x12\x31\n\x05state\x18\x01 \x01(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12?\n\x13subcomponent_states\x18\x02 \x03(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"\x1b\n\x19GetComponentStatesRequest\"\xb6\x01\n\x12LoadBalanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x12\n\nsrc_nodeID\x18\x02 \x01(\x03\x12\x13\n\x0b\x64st_nodeIDs\x18\x03 \x03(\x03\x12\x19\n\x11sealed_segmentIDs\x18\x04 \x03(\x03\x12\x16\n\x0e\x63ollectionName\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x11\x18\x05\"e\n\x17ManualCompactionRequest\x12\x14\n\x0c\x63ollectionID\x18\x01 \x01(\x03\x12\x12\n\ntimetravel\x18\x02 \x01(\x04\x12\x17\n\x0fmajorCompaction\x18\x03 \x01(\x08:\x07\xca>\x04\x10\x07\x18\x01\"z\n\x18ManualCompactionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x63ompactionID\x18\x02 \x01(\x03\x12\x1b\n\x13\x63ompactionPlanCount\x18\x03 \x01(\x05\"1\n\x19GetCompactionStateRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xdd\x01\n\x1aGetCompactionStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12\x17\n\x0f\x65xecutingPlanNo\x18\x03 \x01(\x03\x12\x15\n\rtimeoutPlanNo\x18\x04 \x01(\x03\x12\x17\n\x0f\x63ompletedPlanNo\x18\x05 \x01(\x03\x12\x14\n\x0c\x66\x61iledPlanNo\x18\x06 \x01(\x03\"1\n\x19GetCompactionPlansRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xbc\x01\n\x1aGetCompactionPlansResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12<\n\nmergeInfos\x18\x03 \x03(\x0b\x32(.milvus.proto.milvus.CompactionMergeInfo\"6\n\x13\x43ompactionMergeInfo\x12\x0f\n\x07sources\x18\x01 \x03(\x03\x12\x0e\n\x06target\x18\x02 \x01(\x03\"o\n\x14GetFlushStateRequest\x12\x12\n\nsegmentIDs\x18\x01 \x03(\x03\x12\x10\n\x08\x66lush_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t:\x07\xca>\x04\x10+\x18\x04\"U\n\x15GetFlushStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"l\n\x17GetFlushAllStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"X\n\x18GetFlushAllStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"\xe0\x01\n\rImportRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0epartition_name\x18\x02 \x01(\t\x12\x15\n\rchannel_names\x18\x03 \x03(\t\x12\x11\n\trow_based\x18\x04 \x01(\x08\x12\r\n\x05\x66iles\x18\x05 \x03(\t\x12\x32\n\x07options\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x07 \x01(\t\x12\x17\n\x0f\x63lustering_info\x18\x08 \x01(\x0c:\x07\xca>\x04\x10\x12\x18\x01\"L\n\x0eImportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05tasks\x18\x02 \x03(\x03\"%\n\x15GetImportStateRequest\x12\x0c\n\x04task\x18\x01 \x01(\x03\"\x97\x02\n\x16GetImportStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12/\n\x05state\x18\x02 \x01(\x0e\x32 .milvus.proto.common.ImportState\x12\x11\n\trow_count\x18\x03 \x01(\x03\x12\x0f\n\x07id_list\x18\x04 \x03(\x03\x12\x30\n\x05infos\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02id\x18\x06 \x01(\x03\x12\x15\n\rcollection_id\x18\x07 \x01(\x03\x12\x13\n\x0bsegment_ids\x18\x08 \x03(\x03\x12\x11\n\tcreate_ts\x18\t \x01(\x03\"Q\n\x16ListImportTasksRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"\x82\x01\n\x17ListImportTasksResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x05tasks\x18\x02 \x03(\x0b\x32+.milvus.proto.milvus.GetImportStateResponse\"\x9a\x01\n\x12GetReplicasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x18\n\x10with_shard_nodes\x18\x03 \x01(\x08\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"v\n\x13GetReplicasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08replicas\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.ReplicaInfo\"\xc1\x02\n\x0bReplicaInfo\x12\x11\n\treplicaID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x15\n\rpartition_ids\x18\x03 \x03(\x03\x12\x39\n\x0eshard_replicas\x18\x04 \x03(\x0b\x32!.milvus.proto.milvus.ShardReplica\x12\x10\n\x08node_ids\x18\x05 \x03(\x03\x12\x1b\n\x13resource_group_name\x18\x06 \x01(\t\x12P\n\x11num_outbound_node\x18\x07 \x03(\x0b\x32\x35.milvus.proto.milvus.ReplicaInfo.NumOutboundNodeEntry\x1a\x36\n\x14NumOutboundNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"`\n\x0cShardReplica\x12\x10\n\x08leaderID\x18\x01 \x01(\x03\x12\x13\n\x0bleader_addr\x18\x02 \x01(\t\x12\x17\n\x0f\x64m_channel_name\x18\x03 \x01(\t\x12\x10\n\x08node_ids\x18\x04 \x03(\x03\"\xbe\x01\n\x17\x43reateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x04 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcd\x01\n\x17UpdateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x13\n\x0boldPassword\x18\x03 \x01(\t\x12\x13\n\x0bnewPassword\x18\x04 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x06 \x01(\x04:\t\xca>\x06\x08\x02\x10\x14\x18\x02\"k\n\x17\x44\x65leteCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"W\n\x15ListCredUsersResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tusernames\x18\x02 \x03(\t\"V\n\x14ListCredUsersRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x1a\n\nRoleEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1a\n\nUserEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x43reateRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12/\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"d\n\x0f\x44ropRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\trole_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb5\x01\n\x16OperateUserRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x11\n\trole_name\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.milvus.proto.milvus.OperateUserRoleType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x9d\x01\n\x11SelectRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04role\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x19\n\x11include_user_info\x18\x03 \x01(\x08:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"k\n\nRoleResult\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12.\n\x05users\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\"s\n\x12SelectRoleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleResult\"\x94\x01\n\x11SelectUserRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04user\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x19\n\x11include_role_info\x18\x03 \x01(\x08:\t\xca>\x06\x08\x02\x10\x18\x18\x02\"k\n\nUserResult\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12.\n\x05roles\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\"s\n\x12SelectUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserResult\"\x1c\n\x0cObjectEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1f\n\x0fPrivilegeEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"w\n\rGrantorEntity\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x37\n\tprivilege\x18\x02 \x01(\x0b\x32$.milvus.proto.milvus.PrivilegeEntity\"L\n\x14GrantPrivilegeEntity\x12\x34\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\".milvus.proto.milvus.GrantorEntity\"\xca\x01\n\x0bGrantEntity\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x31\n\x06object\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.ObjectEntity\x12\x13\n\x0bobject_name\x18\x03 \x01(\t\x12\x33\n\x07grantor\x18\x04 \x01(\x0b\x32\".milvus.proto.milvus.GrantorEntity\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"\x86\x01\n\x12SelectGrantRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x13SelectGrantResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08\x65ntities\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.GrantEntity\"\xc4\x01\n\x17OperatePrivilegeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).milvus.proto.milvus.OperatePrivilegeType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x93\x01\n\x19GetLoadingProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"u\n\x1aGetLoadingProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x18\n\x10refresh_progress\x18\x03 \x01(\x03\"\x8d\x01\n\x13GetLoadStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"r\n\x14GetLoadStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12-\n\x05state\x18\x02 \x01(\x0e\x32\x1e.milvus.proto.common.LoadState\"\x1c\n\tMilvusExt\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x13\n\x11GetVersionRequest\"R\n\x12GetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x14\n\x12\x43heckHealthRequest\"\x9d\x01\n\x13\x43heckHealthResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tisHealthy\x18\x02 \x01(\x08\x12\x0f\n\x07reasons\x18\x03 \x03(\t\x12\x35\n\x0cquota_states\x18\x04 \x03(\x0e\x32\x1f.milvus.proto.milvus.QuotaState\"\xaa\x01\n\x1a\x43reateResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t\x12\x34\n\x06\x63onfig\x18\x03 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x12\xca>\x0f\x08\x01\x10\x1a\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x99\x02\n\x1bUpdateResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12]\n\x0fresource_groups\x18\x02 \x03(\x0b\x32\x44.milvus.proto.milvus.UpdateResourceGroupsRequest.ResourceGroupsEntry\x1a[\n\x13ResourceGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x02\x38\x01:\x12\xca>\x0f\x08\x01\x10\x30\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x18\x44ropResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1b\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa5\x01\n\x13TransferNodeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x10\n\x08num_node\x18\x04 \x01(\x05:\x12\xca>\x0f\x08\x01\x10\x1e\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xd5\x01\n\x16TransferReplicaRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x13\n\x0bnum_replica\x18\x05 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1f\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"[\n\x19ListResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x1d\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"b\n\x1aListResourceGroupsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fresource_groups\x18\x02 \x03(\t\"v\n\x1c\x44\x65scribeResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1c\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x88\x01\n\x1d\x44\x65scribeResourceGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x0eresource_group\x18\x02 \x01(\x0b\x32\".milvus.proto.milvus.ResourceGroup\"\xd6\x04\n\rResourceGroup\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x1a\n\x12num_available_node\x18\x03 \x01(\x05\x12T\n\x12num_loaded_replica\x18\x04 \x03(\x0b\x32\x38.milvus.proto.milvus.ResourceGroup.NumLoadedReplicaEntry\x12R\n\x11num_outgoing_node\x18\x05 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumOutgoingNodeEntry\x12R\n\x11num_incoming_node\x18\x06 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumIncomingNodeEntry\x12\x34\n\x06\x63onfig\x18\x07 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig\x12,\n\x05nodes\x18\x08 \x03(\x0b\x32\x1d.milvus.proto.common.NodeInfo\x1a\x37\n\x15NumLoadedReplicaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumOutgoingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumIncomingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x9f\x01\n\x17RenameCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x0f\n\x07oldName\x18\x03 \x01(\t\x12\x0f\n\x07newName\x18\x04 \x01(\t\x12\x11\n\tnewDBName\x18\x05 \x01(\t:\x12\xca>\x0f\x08\x01\x10\"\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa1\x01\n\x19GetIndexStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x8c\x01\n\x1aGetIndexStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"r\n\x0e\x43onnectRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x34\n\x0b\x63lient_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ClientInfo\"\x88\x01\n\x0f\x43onnectResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x0bserver_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ServerInfo\x12\x12\n\nidentifier\x18\x03 \x01(\x03\"C\n\x15\x41llocTimestampRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"X\n\x16\x41llocTimestampResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\ttimestamp\x18\x02 \x01(\x04\"h\n\x15\x43reateDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10#\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"f\n\x13\x44ropDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10$\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"B\n\x14ListDatabasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"q\n\x15ListDatabasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08\x64\x62_names\x18\x02 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x03 \x03(\x04\"\xad\x01\n\x14\x41lterDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x64\x62_id\x18\x03 \x01(\t\x12\x35\n\nproperties\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x31\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xf5\x01\n\x17ReplicateMessageRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x42\x65ginTs\x18\x03 \x01(\x04\x12\r\n\x05\x45ndTs\x18\x04 \x01(\x04\x12\x0c\n\x04Msgs\x18\x05 \x03(\x0c\x12\x35\n\x0eStartPositions\x18\x06 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\x12\x33\n\x0c\x45ndPositions\x18\x07 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\"Y\n\x18ReplicateMessageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08position\x18\x02 \x01(\t\"b\n\x15ImportAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x16\n\x0epartition_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"<\n GetImportProgressAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"O\n\x1aListImportsAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01*%\n\x08ShowType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08InMemory\x10\x01\x1a\x02\x18\x01*@\n\x13OperateUserRoleType\x12\x11\n\rAddUserToRole\x10\x00\x12\x16\n\x12RemoveUserFromRole\x10\x01*-\n\x14OperatePrivilegeType\x12\t\n\x05Grant\x10\x00\x12\n\n\x06Revoke\x10\x01*]\n\nQuotaState\x12\x0b\n\x07Unknown\x10\x00\x12\x0f\n\x0bReadLimited\x10\x02\x12\x10\n\x0cWriteLimited\x10\x03\x12\x0e\n\nDenyToRead\x10\x04\x12\x0f\n\x0b\x44\x65nyToWrite\x10\x05\x32\xc7\x43\n\rMilvusService\x12_\n\x10\x43reateCollection\x12,.milvus.proto.milvus.CreateCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12[\n\x0e\x44ropCollection\x12*.milvus.proto.milvus.DropCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\rHasCollection\x12).milvus.proto.milvus.HasCollectionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadCollection\x12*.milvus.proto.milvus.LoadCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleaseCollection\x12-.milvus.proto.milvus.ReleaseCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12\x44\x65scribeCollection\x12..milvus.proto.milvus.DescribeCollectionRequest\x1a/.milvus.proto.milvus.DescribeCollectionResponse\"\x00\x12\x86\x01\n\x17GetCollectionStatistics\x12\x33.milvus.proto.milvus.GetCollectionStatisticsRequest\x1a\x34.milvus.proto.milvus.GetCollectionStatisticsResponse\"\x00\x12n\n\x0fShowCollections\x12+.milvus.proto.milvus.ShowCollectionsRequest\x1a,.milvus.proto.milvus.ShowCollectionsResponse\"\x00\x12]\n\x0f\x41lterCollection\x12+.milvus.proto.milvus.AlterCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0f\x43reatePartition\x12+.milvus.proto.milvus.CreatePartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Y\n\rDropPartition\x12).milvus.proto.milvus.DropPartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0cHasPartition\x12(.milvus.proto.milvus.HasPartitionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadPartitions\x12*.milvus.proto.milvus.LoadPartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleasePartitions\x12-.milvus.proto.milvus.ReleasePartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x83\x01\n\x16GetPartitionStatistics\x12\x32.milvus.proto.milvus.GetPartitionStatisticsRequest\x1a\x33.milvus.proto.milvus.GetPartitionStatisticsResponse\"\x00\x12k\n\x0eShowPartitions\x12*.milvus.proto.milvus.ShowPartitionsRequest\x1a+.milvus.proto.milvus.ShowPartitionsResponse\"\x00\x12w\n\x12GetLoadingProgress\x12..milvus.proto.milvus.GetLoadingProgressRequest\x1a/.milvus.proto.milvus.GetLoadingProgressResponse\"\x00\x12\x65\n\x0cGetLoadState\x12(.milvus.proto.milvus.GetLoadStateRequest\x1a).milvus.proto.milvus.GetLoadStateResponse\"\x00\x12U\n\x0b\x43reateAlias\x12\'.milvus.proto.milvus.CreateAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Q\n\tDropAlias\x12%.milvus.proto.milvus.DropAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterAlias\x12&.milvus.proto.milvus.AlterAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeAlias\x12).milvus.proto.milvus.DescribeAliasRequest\x1a*.milvus.proto.milvus.DescribeAliasResponse\"\x00\x12\x62\n\x0bListAliases\x12\'.milvus.proto.milvus.ListAliasesRequest\x1a(.milvus.proto.milvus.ListAliasesResponse\"\x00\x12U\n\x0b\x43reateIndex\x12\'.milvus.proto.milvus.CreateIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterIndex\x12&.milvus.proto.milvus.AlterIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeIndex\x12).milvus.proto.milvus.DescribeIndexRequest\x1a*.milvus.proto.milvus.DescribeIndexResponse\"\x00\x12w\n\x12GetIndexStatistics\x12..milvus.proto.milvus.GetIndexStatisticsRequest\x1a/.milvus.proto.milvus.GetIndexStatisticsResponse\"\x00\x12k\n\rGetIndexState\x12).milvus.proto.milvus.GetIndexStateRequest\x1a*.milvus.proto.milvus.GetIndexStateResponse\"\x03\x88\x02\x01\x12\x83\x01\n\x15GetIndexBuildProgress\x12\x31.milvus.proto.milvus.GetIndexBuildProgressRequest\x1a\x32.milvus.proto.milvus.GetIndexBuildProgressResponse\"\x03\x88\x02\x01\x12Q\n\tDropIndex\x12%.milvus.proto.milvus.DropIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\x06Insert\x12\".milvus.proto.milvus.InsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06\x44\x65lete\x12\".milvus.proto.milvus.DeleteRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06Upsert\x12\".milvus.proto.milvus.UpsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12R\n\x06Search\x12\".milvus.proto.milvus.SearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12^\n\x0cHybridSearch\x12(.milvus.proto.milvus.HybridSearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12P\n\x05\x46lush\x12!.milvus.proto.milvus.FlushRequest\x1a\".milvus.proto.milvus.FlushResponse\"\x00\x12O\n\x05Query\x12!.milvus.proto.milvus.QueryRequest\x1a!.milvus.proto.milvus.QueryResults\"\x00\x12\x64\n\x0c\x43\x61lcDistance\x12(.milvus.proto.milvus.CalcDistanceRequest\x1a(.milvus.proto.milvus.CalcDistanceResults\"\x00\x12Y\n\x08\x46lushAll\x12$.milvus.proto.milvus.FlushAllRequest\x1a%.milvus.proto.milvus.FlushAllResponse\"\x00\x12h\n\rGetFlushState\x12).milvus.proto.milvus.GetFlushStateRequest\x1a*.milvus.proto.milvus.GetFlushStateResponse\"\x00\x12q\n\x10GetFlushAllState\x12,.milvus.proto.milvus.GetFlushAllStateRequest\x1a-.milvus.proto.milvus.GetFlushAllStateResponse\"\x00\x12\x89\x01\n\x18GetPersistentSegmentInfo\x12\x34.milvus.proto.milvus.GetPersistentSegmentInfoRequest\x1a\x35.milvus.proto.milvus.GetPersistentSegmentInfoResponse\"\x00\x12z\n\x13GetQuerySegmentInfo\x12/.milvus.proto.milvus.GetQuerySegmentInfoRequest\x1a\x30.milvus.proto.milvus.GetQuerySegmentInfoResponse\"\x00\x12\x62\n\x0bGetReplicas\x12\'.milvus.proto.milvus.GetReplicasRequest\x1a(.milvus.proto.milvus.GetReplicasResponse\"\x00\x12P\n\x05\x44ummy\x12!.milvus.proto.milvus.DummyRequest\x1a\".milvus.proto.milvus.DummyResponse\"\x00\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00\x12_\n\nGetMetrics\x12&.milvus.proto.milvus.GetMetricsRequest\x1a\'.milvus.proto.milvus.GetMetricsResponse\"\x00\x12l\n\x12GetComponentStates\x12..milvus.proto.milvus.GetComponentStatesRequest\x1a$.milvus.proto.milvus.ComponentStates\"\x00\x12U\n\x0bLoadBalance\x12\'.milvus.proto.milvus.LoadBalanceRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12GetCompactionState\x12..milvus.proto.milvus.GetCompactionStateRequest\x1a/.milvus.proto.milvus.GetCompactionStateResponse\"\x00\x12q\n\x10ManualCompaction\x12,.milvus.proto.milvus.ManualCompactionRequest\x1a-.milvus.proto.milvus.ManualCompactionResponse\"\x00\x12\x80\x01\n\x1bGetCompactionStateWithPlans\x12..milvus.proto.milvus.GetCompactionPlansRequest\x1a/.milvus.proto.milvus.GetCompactionPlansResponse\"\x00\x12S\n\x06Import\x12\".milvus.proto.milvus.ImportRequest\x1a#.milvus.proto.milvus.ImportResponse\"\x00\x12k\n\x0eGetImportState\x12*.milvus.proto.milvus.GetImportStateRequest\x1a+.milvus.proto.milvus.GetImportStateResponse\"\x00\x12n\n\x0fListImportTasks\x12+.milvus.proto.milvus.ListImportTasksRequest\x1a,.milvus.proto.milvus.ListImportTasksResponse\"\x00\x12_\n\x10\x43reateCredential\x12,.milvus.proto.milvus.CreateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10UpdateCredential\x12,.milvus.proto.milvus.UpdateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10\x44\x65leteCredential\x12,.milvus.proto.milvus.DeleteCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListCredUsers\x12).milvus.proto.milvus.ListCredUsersRequest\x1a*.milvus.proto.milvus.ListCredUsersResponse\"\x00\x12S\n\nCreateRole\x12&.milvus.proto.milvus.CreateRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12O\n\x08\x44ropRole\x12$.milvus.proto.milvus.DropRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fOperateUserRole\x12+.milvus.proto.milvus.OperateUserRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\nSelectRole\x12&.milvus.proto.milvus.SelectRoleRequest\x1a\'.milvus.proto.milvus.SelectRoleResponse\"\x00\x12_\n\nSelectUser\x12&.milvus.proto.milvus.SelectUserRequest\x1a\'.milvus.proto.milvus.SelectUserResponse\"\x00\x12_\n\x10OperatePrivilege\x12,.milvus.proto.milvus.OperatePrivilegeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x62\n\x0bSelectGrant\x12\'.milvus.proto.milvus.SelectGrantRequest\x1a(.milvus.proto.milvus.SelectGrantResponse\"\x00\x12_\n\nGetVersion\x12&.milvus.proto.milvus.GetVersionRequest\x1a\'.milvus.proto.milvus.GetVersionResponse\"\x00\x12\x62\n\x0b\x43heckHealth\x12\'.milvus.proto.milvus.CheckHealthRequest\x1a(.milvus.proto.milvus.CheckHealthResponse\"\x00\x12\x65\n\x13\x43reateResourceGroup\x12/.milvus.proto.milvus.CreateResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11\x44ropResourceGroup\x12-.milvus.proto.milvus.DropResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12g\n\x14UpdateResourceGroups\x12\x30.milvus.proto.milvus.UpdateResourceGroupsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0cTransferNode\x12(.milvus.proto.milvus.TransferNodeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fTransferReplica\x12+.milvus.proto.milvus.TransferReplicaRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12ListResourceGroups\x12..milvus.proto.milvus.ListResourceGroupsRequest\x1a/.milvus.proto.milvus.ListResourceGroupsResponse\"\x00\x12\x80\x01\n\x15\x44\x65scribeResourceGroup\x12\x31.milvus.proto.milvus.DescribeResourceGroupRequest\x1a\x32.milvus.proto.milvus.DescribeResourceGroupResponse\"\x00\x12_\n\x10RenameCollection\x12,.milvus.proto.milvus.RenameCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12u\n\x12ListIndexedSegment\x12-.milvus.proto.feder.ListIndexedSegmentRequest\x1a..milvus.proto.feder.ListIndexedSegmentResponse\"\x00\x12\x87\x01\n\x18\x44\x65scribeSegmentIndexData\x12\x33.milvus.proto.feder.DescribeSegmentIndexDataRequest\x1a\x34.milvus.proto.feder.DescribeSegmentIndexDataResponse\"\x00\x12V\n\x07\x43onnect\x12#.milvus.proto.milvus.ConnectRequest\x1a$.milvus.proto.milvus.ConnectResponse\"\x00\x12k\n\x0e\x41llocTimestamp\x12*.milvus.proto.milvus.AllocTimestampRequest\x1a+.milvus.proto.milvus.AllocTimestampResponse\"\x00\x12[\n\x0e\x43reateDatabase\x12*.milvus.proto.milvus.CreateDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0c\x44ropDatabase\x12(.milvus.proto.milvus.DropDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListDatabases\x12).milvus.proto.milvus.ListDatabasesRequest\x1a*.milvus.proto.milvus.ListDatabasesResponse\"\x00\x12Y\n\rAlterDatabase\x12).milvus.proto.milvus.AlterDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12q\n\x10ReplicateMessage\x12,.milvus.proto.milvus.ReplicateMessageRequest\x1a-.milvus.proto.milvus.ReplicateMessageResponse\"\x00\x32u\n\x0cProxyService\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00:U\n\x0emilvus_ext_obj\x12\x1c.google.protobuf.FileOptions\x18\xe9\x07 \x01(\x0b\x32\x1e.milvus.proto.milvus.MilvusExtBm\n\x0eio.milvus.grpcB\x0bMilvusProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'milvus_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\016io.milvus.grpcB\013MilvusProtoP\001Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\240\001\001\252\002\022Milvus.Client.Grpc'
@@ -54,16 +54,14 @@
   _globals['_RELEASECOLLECTIONREQUEST']._serialized_options = b'\312>\004\020\006\030\003'
   _globals['_GETSTATISTICSREQUEST']._options = None
   _globals['_GETSTATISTICSREQUEST']._serialized_options = b'\312>\004\020\n\030\003'
   _globals['_GETCOLLECTIONSTATISTICSREQUEST']._options = None
   _globals['_GETCOLLECTIONSTATISTICSREQUEST']._serialized_options = b'\312>\004\020\n\030\003'
   _globals['_SHOWCOLLECTIONSREQUEST'].fields_by_name['collection_names']._options = None
   _globals['_SHOWCOLLECTIONSREQUEST'].fields_by_name['collection_names']._serialized_options = b'\030\001'
-  _globals['_SHOWCOLLECTIONSREQUEST']._options = None
-  _globals['_SHOWCOLLECTIONSREQUEST']._serialized_options = b'\312>\017\010\001\020\004\030\377\377\377\377\377\377\377\377\377\001'
   _globals['_SHOWCOLLECTIONSRESPONSE'].fields_by_name['inMemory_percentages']._options = None
   _globals['_SHOWCOLLECTIONSRESPONSE'].fields_by_name['inMemory_percentages']._serialized_options = b'\030\001'
   _globals['_CREATEPARTITIONREQUEST']._options = None
   _globals['_CREATEPARTITIONREQUEST']._serialized_options = b'\312>\004\020\'\030\003'
   _globals['_DROPPARTITIONREQUEST']._options = None
   _globals['_DROPPARTITIONREQUEST']._serialized_options = b'\312>\004\020(\030\003'
   _globals['_HASPARTITIONREQUEST']._options = None
@@ -178,36 +176,34 @@
   _globals['_RENAMECOLLECTIONREQUEST']._serialized_options = b'\312>\017\010\001\020\"\030\377\377\377\377\377\377\377\377\377\001'
   _globals['_GETINDEXSTATISTICSREQUEST']._options = None
   _globals['_GETINDEXSTATISTICSREQUEST']._serialized_options = b'\312>\004\020\014\030\003'
   _globals['_CREATEDATABASEREQUEST']._options = None
   _globals['_CREATEDATABASEREQUEST']._serialized_options = b'\312>\017\010\001\020#\030\377\377\377\377\377\377\377\377\377\001'
   _globals['_DROPDATABASEREQUEST']._options = None
   _globals['_DROPDATABASEREQUEST']._serialized_options = b'\312>\017\010\001\020$\030\377\377\377\377\377\377\377\377\377\001'
-  _globals['_LISTDATABASESREQUEST']._options = None
-  _globals['_LISTDATABASESREQUEST']._serialized_options = b'\312>\017\010\001\020%\030\377\377\377\377\377\377\377\377\377\001'
-  _globals['_LISTDATABASESRESPONSE']._options = None
-  _globals['_LISTDATABASESRESPONSE']._serialized_options = b'\312>\017\010\001\020\004\030\377\377\377\377\377\377\377\377\377\001'
+  _globals['_ALTERDATABASEREQUEST']._options = None
+  _globals['_ALTERDATABASEREQUEST']._serialized_options = b'\312>\017\010\001\0201\030\377\377\377\377\377\377\377\377\377\001'
   _globals['_IMPORTAUTHPLACEHOLDER']._options = None
   _globals['_IMPORTAUTHPLACEHOLDER']._serialized_options = b'\312>\004\020\022\030\001'
   _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._options = None
   _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_options = b'\312>\004\020\022\030\001'
   _globals['_LISTIMPORTSAUTHPLACEHOLDER']._options = None
   _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_options = b'\312>\004\020\022\030\001'
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexState']._options = None
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexState']._serialized_options = b'\210\002\001'
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexBuildProgress']._options = None
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexBuildProgress']._serialized_options = b'\210\002\001'
-  _globals['_SHOWTYPE']._serialized_start=24510
-  _globals['_SHOWTYPE']._serialized_end=24547
-  _globals['_OPERATEUSERROLETYPE']._serialized_start=24549
-  _globals['_OPERATEUSERROLETYPE']._serialized_end=24613
-  _globals['_OPERATEPRIVILEGETYPE']._serialized_start=24615
-  _globals['_OPERATEPRIVILEGETYPE']._serialized_end=24660
-  _globals['_QUOTASTATE']._serialized_start=24662
-  _globals['_QUOTASTATE']._serialized_end=24755
+  _globals['_SHOWTYPE']._serialized_start=24640
+  _globals['_SHOWTYPE']._serialized_end=24677
+  _globals['_OPERATEUSERROLETYPE']._serialized_start=24679
+  _globals['_OPERATEUSERROLETYPE']._serialized_end=24743
+  _globals['_OPERATEPRIVILEGETYPE']._serialized_start=24745
+  _globals['_OPERATEPRIVILEGETYPE']._serialized_end=24790
+  _globals['_QUOTASTATE']._serialized_start=24792
+  _globals['_QUOTASTATE']._serialized_end=24885
   _globals['_CREATEALIASREQUEST']._serialized_start=134
   _globals['_CREATEALIASREQUEST']._serialized_end=275
   _globals['_DROPALIASREQUEST']._serialized_start=277
   _globals['_DROPALIASREQUEST']._serialized_end=391
   _globals['_ALTERALIASREQUEST']._serialized_start=394
   _globals['_ALTERALIASREQUEST']._serialized_end=534
   _globals['_DESCRIBEALIASREQUEST']._serialized_start=536
@@ -229,323 +225,325 @@
   _globals['_BOOLRESPONSE']._serialized_start=1821
   _globals['_BOOLRESPONSE']._serialized_end=1895
   _globals['_STRINGRESPONSE']._serialized_start=1897
   _globals['_STRINGRESPONSE']._serialized_end=1973
   _globals['_DESCRIBECOLLECTIONREQUEST']._serialized_start=1976
   _globals['_DESCRIBECOLLECTIONREQUEST']._serialized_end=2151
   _globals['_DESCRIBECOLLECTIONRESPONSE']._serialized_start=2154
-  _globals['_DESCRIBECOLLECTIONRESPONSE']._serialized_end=2708
-  _globals['_LOADCOLLECTIONREQUEST']._serialized_start=2711
-  _globals['_LOADCOLLECTIONREQUEST']._serialized_end=2895
-  _globals['_RELEASECOLLECTIONREQUEST']._serialized_start=2897
-  _globals['_RELEASECOLLECTIONREQUEST']._serialized_end=3018
-  _globals['_GETSTATISTICSREQUEST']._serialized_start=3021
-  _globals['_GETSTATISTICSREQUEST']._serialized_end=3192
-  _globals['_GETSTATISTICSRESPONSE']._serialized_start=3194
-  _globals['_GETSTATISTICSRESPONSE']._serialized_end=3312
-  _globals['_GETCOLLECTIONSTATISTICSREQUEST']._serialized_start=3314
-  _globals['_GETCOLLECTIONSTATISTICSREQUEST']._serialized_end=3441
-  _globals['_GETCOLLECTIONSTATISTICSRESPONSE']._serialized_start=3444
-  _globals['_GETCOLLECTIONSTATISTICSRESPONSE']._serialized_end=3572
-  _globals['_SHOWCOLLECTIONSREQUEST']._serialized_start=3575
-  _globals['_SHOWCOLLECTIONSREQUEST']._serialized_end=3775
-  _globals['_SHOWCOLLECTIONSRESPONSE']._serialized_start=3778
-  _globals['_SHOWCOLLECTIONSRESPONSE']._serialized_end=4025
-  _globals['_CREATEPARTITIONREQUEST']._serialized_start=4028
-  _globals['_CREATEPARTITIONREQUEST']._serialized_end=4171
-  _globals['_DROPPARTITIONREQUEST']._serialized_start=4174
-  _globals['_DROPPARTITIONREQUEST']._serialized_end=4315
-  _globals['_HASPARTITIONREQUEST']._serialized_start=4318
-  _globals['_HASPARTITIONREQUEST']._serialized_end=4458
-  _globals['_LOADPARTITIONSREQUEST']._serialized_start=4461
-  _globals['_LOADPARTITIONSREQUEST']._serialized_end=4670
-  _globals['_RELEASEPARTITIONSREQUEST']._serialized_start=4673
-  _globals['_RELEASEPARTITIONSREQUEST']._serialized_end=4819
-  _globals['_GETPARTITIONSTATISTICSREQUEST']._serialized_start=4822
-  _globals['_GETPARTITIONSTATISTICSREQUEST']._serialized_end=4963
-  _globals['_GETPARTITIONSTATISTICSRESPONSE']._serialized_start=4965
-  _globals['_GETPARTITIONSTATISTICSRESPONSE']._serialized_end=5092
-  _globals['_SHOWPARTITIONSREQUEST']._serialized_start=5095
-  _globals['_SHOWPARTITIONSREQUEST']._serialized_end=5309
-  _globals['_SHOWPARTITIONSRESPONSE']._serialized_start=5312
-  _globals['_SHOWPARTITIONSRESPONSE']._serialized_end=5522
-  _globals['_DESCRIBESEGMENTREQUEST']._serialized_start=5524
-  _globals['_DESCRIBESEGMENTREQUEST']._serialized_end=5633
-  _globals['_DESCRIBESEGMENTRESPONSE']._serialized_start=5636
-  _globals['_DESCRIBESEGMENTRESPONSE']._serialized_end=5779
-  _globals['_SHOWSEGMENTSREQUEST']._serialized_start=5781
-  _globals['_SHOWSEGMENTSREQUEST']._serialized_end=5889
-  _globals['_SHOWSEGMENTSRESPONSE']._serialized_start=5891
-  _globals['_SHOWSEGMENTSRESPONSE']._serialized_end=5978
-  _globals['_CREATEINDEXREQUEST']._serialized_start=5981
-  _globals['_CREATEINDEXREQUEST']._serialized_end=6193
-  _globals['_ALTERINDEXREQUEST']._serialized_start=6196
-  _globals['_ALTERINDEXREQUEST']._serialized_end=6387
-  _globals['_DESCRIBEINDEXREQUEST']._serialized_start=6390
-  _globals['_DESCRIBEINDEXREQUEST']._serialized_end=6566
-  _globals['_INDEXDESCRIPTION']._serialized_start=6569
-  _globals['_INDEXDESCRIPTION']._serialized_end=6846
-  _globals['_DESCRIBEINDEXRESPONSE']._serialized_start=6849
-  _globals['_DESCRIBEINDEXRESPONSE']._serialized_end=6984
-  _globals['_GETINDEXBUILDPROGRESSREQUEST']._serialized_start=6987
-  _globals['_GETINDEXBUILDPROGRESSREQUEST']._serialized_end=7152
-  _globals['_GETINDEXBUILDPROGRESSRESPONSE']._serialized_start=7154
-  _globals['_GETINDEXBUILDPROGRESSRESPONSE']._serialized_end=7272
-  _globals['_GETINDEXSTATEREQUEST']._serialized_start=7275
-  _globals['_GETINDEXSTATEREQUEST']._serialized_end=7432
-  _globals['_GETINDEXSTATERESPONSE']._serialized_start=7435
-  _globals['_GETINDEXSTATERESPONSE']._serialized_end=7572
-  _globals['_DROPINDEXREQUEST']._serialized_start=7575
-  _globals['_DROPINDEXREQUEST']._serialized_end=7728
-  _globals['_INSERTREQUEST']._serialized_start=7731
-  _globals['_INSERTREQUEST']._serialized_end=7955
-  _globals['_UPSERTREQUEST']._serialized_start=7958
-  _globals['_UPSERTREQUEST']._serialized_end=8182
-  _globals['_MUTATIONRESULT']._serialized_start=8185
-  _globals['_MUTATIONRESULT']._serialized_end=8425
-  _globals['_DELETEREQUEST']._serialized_start=8428
-  _globals['_DELETEREQUEST']._serialized_end=8661
-  _globals['_SUBSEARCHREQUEST']._serialized_start=8664
-  _globals['_SUBSEARCHREQUEST']._serialized_end=8840
-  _globals['_SEARCHREQUEST']._serialized_start=8843
-  _globals['_SEARCHREQUEST']._serialized_end=9431
-  _globals['_HITS']._serialized_start=9433
-  _globals['_HITS']._serialized_end=9486
-  _globals['_SEARCHRESULTS']._serialized_start=9489
-  _globals['_SEARCHRESULTS']._serialized_end=9630
-  _globals['_HYBRIDSEARCHREQUEST']._serialized_start=9633
-  _globals['_HYBRIDSEARCHREQUEST']._serialized_end=10090
-  _globals['_FLUSHREQUEST']._serialized_start=10092
-  _globals['_FLUSHREQUEST']._serialized_end=10202
-  _globals['_FLUSHRESPONSE']._serialized_start=10205
-  _globals['_FLUSHRESPONSE']._serialized_end=10872
-  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_start=10597
-  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_end=10678
-  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_start=10680
-  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_end=10766
-  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_start=10768
-  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_end=10820
-  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_start=10822
-  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_end=10872
-  _globals['_QUERYREQUEST']._serialized_start=10875
-  _globals['_QUERYREQUEST']._serialized_end=11286
-  _globals['_QUERYRESULTS']._serialized_start=11289
-  _globals['_QUERYRESULTS']._serialized_end=11449
-  _globals['_VECTORIDS']._serialized_start=11451
-  _globals['_VECTORIDS']._serialized_end=11576
-  _globals['_VECTORSARRAY']._serialized_start=11579
-  _globals['_VECTORSARRAY']._serialized_end=11710
-  _globals['_CALCDISTANCEREQUEST']._serialized_start=11713
-  _globals['_CALCDISTANCEREQUEST']._serialized_end=11934
-  _globals['_CALCDISTANCERESULTS']._serialized_start=11937
-  _globals['_CALCDISTANCERESULTS']._serialized_end=12118
-  _globals['_FLUSHALLREQUEST']._serialized_start=12120
-  _globals['_FLUSHALLREQUEST']._serialized_end=12218
-  _globals['_FLUSHALLRESPONSE']._serialized_start=12220
-  _globals['_FLUSHALLRESPONSE']._serialized_end=12305
-  _globals['_PERSISTENTSEGMENTINFO']._serialized_start=12308
-  _globals['_PERSISTENTSEGMENTINFO']._serialized_end=12461
-  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_start=12463
-  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_end=12580
-  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_start=12583
-  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_end=12721
-  _globals['_QUERYSEGMENTINFO']._serialized_start=12724
-  _globals['_QUERYSEGMENTINFO']._serialized_end=12964
-  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_start=12966
-  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_end=13078
-  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_start=13081
-  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_end=13209
-  _globals['_DUMMYREQUEST']._serialized_start=13211
-  _globals['_DUMMYREQUEST']._serialized_end=13247
-  _globals['_DUMMYRESPONSE']._serialized_start=13249
-  _globals['_DUMMYRESPONSE']._serialized_end=13282
-  _globals['_REGISTERLINKREQUEST']._serialized_start=13284
-  _globals['_REGISTERLINKREQUEST']._serialized_end=13305
-  _globals['_REGISTERLINKRESPONSE']._serialized_start=13307
-  _globals['_REGISTERLINKRESPONSE']._serialized_end=13421
-  _globals['_GETMETRICSREQUEST']._serialized_start=13423
-  _globals['_GETMETRICSREQUEST']._serialized_end=13503
-  _globals['_GETMETRICSRESPONSE']._serialized_start=13505
-  _globals['_GETMETRICSRESPONSE']._serialized_end=13612
-  _globals['_COMPONENTINFO']._serialized_start=13615
-  _globals['_COMPONENTINFO']._serialized_end=13767
-  _globals['_COMPONENTSTATES']._serialized_start=13770
-  _globals['_COMPONENTSTATES']._serialized_end=13948
-  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_start=13950
-  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_end=13977
-  _globals['_LOADBALANCEREQUEST']._serialized_start=13980
-  _globals['_LOADBALANCEREQUEST']._serialized_end=14162
-  _globals['_MANUALCOMPACTIONREQUEST']._serialized_start=14164
-  _globals['_MANUALCOMPACTIONREQUEST']._serialized_end=14265
-  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_start=14267
-  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_end=14389
-  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_start=14391
-  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_end=14440
-  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_start=14443
-  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_end=14664
-  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_start=14666
-  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_end=14715
-  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_start=14718
-  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_end=14906
-  _globals['_COMPACTIONMERGEINFO']._serialized_start=14908
-  _globals['_COMPACTIONMERGEINFO']._serialized_end=14962
-  _globals['_GETFLUSHSTATEREQUEST']._serialized_start=14964
-  _globals['_GETFLUSHSTATEREQUEST']._serialized_end=15075
-  _globals['_GETFLUSHSTATERESPONSE']._serialized_start=15077
-  _globals['_GETFLUSHSTATERESPONSE']._serialized_end=15162
-  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_start=15164
-  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_end=15272
-  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_start=15274
-  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_end=15362
-  _globals['_IMPORTREQUEST']._serialized_start=15365
-  _globals['_IMPORTREQUEST']._serialized_end=15589
-  _globals['_IMPORTRESPONSE']._serialized_start=15591
-  _globals['_IMPORTRESPONSE']._serialized_end=15667
-  _globals['_GETIMPORTSTATEREQUEST']._serialized_start=15669
-  _globals['_GETIMPORTSTATEREQUEST']._serialized_end=15706
-  _globals['_GETIMPORTSTATERESPONSE']._serialized_start=15709
-  _globals['_GETIMPORTSTATERESPONSE']._serialized_end=15988
-  _globals['_LISTIMPORTTASKSREQUEST']._serialized_start=15990
-  _globals['_LISTIMPORTTASKSREQUEST']._serialized_end=16071
-  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_start=16074
-  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_end=16204
-  _globals['_GETREPLICASREQUEST']._serialized_start=16207
-  _globals['_GETREPLICASREQUEST']._serialized_end=16361
-  _globals['_GETREPLICASRESPONSE']._serialized_start=16363
-  _globals['_GETREPLICASRESPONSE']._serialized_end=16481
-  _globals['_REPLICAINFO']._serialized_start=16484
-  _globals['_REPLICAINFO']._serialized_end=16805
-  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_start=16751
-  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_end=16805
-  _globals['_SHARDREPLICA']._serialized_start=16807
-  _globals['_SHARDREPLICA']._serialized_end=16903
-  _globals['_CREATECREDENTIALREQUEST']._serialized_start=16906
-  _globals['_CREATECREDENTIALREQUEST']._serialized_end=17096
-  _globals['_UPDATECREDENTIALREQUEST']._serialized_start=17099
-  _globals['_UPDATECREDENTIALREQUEST']._serialized_end=17304
-  _globals['_DELETECREDENTIALREQUEST']._serialized_start=17306
-  _globals['_DELETECREDENTIALREQUEST']._serialized_end=17413
-  _globals['_LISTCREDUSERSRESPONSE']._serialized_start=17415
-  _globals['_LISTCREDUSERSRESPONSE']._serialized_end=17502
-  _globals['_LISTCREDUSERSREQUEST']._serialized_start=17504
-  _globals['_LISTCREDUSERSREQUEST']._serialized_end=17590
-  _globals['_ROLEENTITY']._serialized_start=17592
-  _globals['_ROLEENTITY']._serialized_end=17618
-  _globals['_USERENTITY']._serialized_start=17620
-  _globals['_USERENTITY']._serialized_end=17646
-  _globals['_CREATEROLEREQUEST']._serialized_start=17649
-  _globals['_CREATEROLEREQUEST']._serialized_end=17781
-  _globals['_DROPROLEREQUEST']._serialized_start=17783
-  _globals['_DROPROLEREQUEST']._serialized_end=17883
-  _globals['_OPERATEUSERROLEREQUEST']._serialized_start=17886
-  _globals['_OPERATEUSERROLEREQUEST']._serialized_end=18067
-  _globals['_SELECTROLEREQUEST']._serialized_start=18070
-  _globals['_SELECTROLEREQUEST']._serialized_end=18227
-  _globals['_ROLERESULT']._serialized_start=18229
-  _globals['_ROLERESULT']._serialized_end=18336
-  _globals['_SELECTROLERESPONSE']._serialized_start=18338
-  _globals['_SELECTROLERESPONSE']._serialized_end=18453
-  _globals['_SELECTUSERREQUEST']._serialized_start=18456
-  _globals['_SELECTUSERREQUEST']._serialized_end=18604
-  _globals['_USERRESULT']._serialized_start=18606
-  _globals['_USERRESULT']._serialized_end=18713
-  _globals['_SELECTUSERRESPONSE']._serialized_start=18715
-  _globals['_SELECTUSERRESPONSE']._serialized_end=18830
-  _globals['_OBJECTENTITY']._serialized_start=18832
-  _globals['_OBJECTENTITY']._serialized_end=18860
-  _globals['_PRIVILEGEENTITY']._serialized_start=18862
-  _globals['_PRIVILEGEENTITY']._serialized_end=18893
-  _globals['_GRANTORENTITY']._serialized_start=18895
-  _globals['_GRANTORENTITY']._serialized_end=19014
-  _globals['_GRANTPRIVILEGEENTITY']._serialized_start=19016
-  _globals['_GRANTPRIVILEGEENTITY']._serialized_end=19092
-  _globals['_GRANTENTITY']._serialized_start=19095
-  _globals['_GRANTENTITY']._serialized_end=19297
-  _globals['_SELECTGRANTREQUEST']._serialized_start=19300
-  _globals['_SELECTGRANTREQUEST']._serialized_end=19434
-  _globals['_SELECTGRANTRESPONSE']._serialized_start=19436
-  _globals['_SELECTGRANTRESPONSE']._serialized_end=19554
-  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_start=19557
-  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_end=19753
-  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_start=19756
-  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_end=19903
-  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_start=19905
-  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_end=20022
-  _globals['_GETLOADSTATEREQUEST']._serialized_start=20025
-  _globals['_GETLOADSTATEREQUEST']._serialized_end=20166
-  _globals['_GETLOADSTATERESPONSE']._serialized_start=20168
-  _globals['_GETLOADSTATERESPONSE']._serialized_end=20282
-  _globals['_MILVUSEXT']._serialized_start=20284
-  _globals['_MILVUSEXT']._serialized_end=20312
-  _globals['_GETVERSIONREQUEST']._serialized_start=20314
-  _globals['_GETVERSIONREQUEST']._serialized_end=20333
-  _globals['_GETVERSIONRESPONSE']._serialized_start=20335
-  _globals['_GETVERSIONRESPONSE']._serialized_end=20417
-  _globals['_CHECKHEALTHREQUEST']._serialized_start=20419
-  _globals['_CHECKHEALTHREQUEST']._serialized_end=20439
-  _globals['_CHECKHEALTHRESPONSE']._serialized_start=20442
-  _globals['_CHECKHEALTHRESPONSE']._serialized_end=20599
-  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_start=20602
-  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_end=20772
-  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_start=20775
-  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_end=21056
-  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_start=20945
-  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_end=21036
-  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_start=21058
-  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_end=21172
-  _globals['_TRANSFERNODEREQUEST']._serialized_start=21175
-  _globals['_TRANSFERNODEREQUEST']._serialized_end=21340
-  _globals['_TRANSFERREPLICAREQUEST']._serialized_start=21343
-  _globals['_TRANSFERREPLICAREQUEST']._serialized_end=21556
-  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_start=21558
-  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_end=21649
-  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_start=21651
-  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_end=21749
-  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_start=21751
-  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_end=21869
-  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_start=21872
-  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_end=22008
-  _globals['_RESOURCEGROUP']._serialized_start=22011
-  _globals['_RESOURCEGROUP']._serialized_end=22609
-  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_start=22442
-  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_end=22497
-  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_start=22499
-  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_end=22553
-  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_start=22555
-  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_end=22609
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=22612
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=22771
-  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_start=22774
-  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_end=22935
-  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_start=22938
-  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_end=23078
-  _globals['_CONNECTREQUEST']._serialized_start=23080
-  _globals['_CONNECTREQUEST']._serialized_end=23194
-  _globals['_CONNECTRESPONSE']._serialized_start=23197
-  _globals['_CONNECTRESPONSE']._serialized_end=23333
-  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_start=23335
-  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_end=23402
-  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_start=23404
-  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_end=23492
-  _globals['_CREATEDATABASEREQUEST']._serialized_start=23494
-  _globals['_CREATEDATABASEREQUEST']._serialized_end=23598
-  _globals['_DROPDATABASEREQUEST']._serialized_start=23600
-  _globals['_DROPDATABASEREQUEST']._serialized_end=23702
-  _globals['_LISTDATABASESREQUEST']._serialized_start=23704
-  _globals['_LISTDATABASESREQUEST']._serialized_end=23790
-  _globals['_LISTDATABASESRESPONSE']._serialized_start=23793
-  _globals['_LISTDATABASESRESPONSE']._serialized_end=23926
-  _globals['_REPLICATEMESSAGEREQUEST']._serialized_start=23929
-  _globals['_REPLICATEMESSAGEREQUEST']._serialized_end=24174
-  _globals['_REPLICATEMESSAGERESPONSE']._serialized_start=24176
-  _globals['_REPLICATEMESSAGERESPONSE']._serialized_end=24265
-  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_start=24267
-  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_end=24365
-  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_start=24367
-  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_end=24427
-  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_start=24429
-  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_end=24508
-  _globals['_MILVUSSERVICE']._serialized_start=24758
-  _globals['_MILVUSSERVICE']._serialized_end=33314
-  _globals['_PROXYSERVICE']._serialized_start=33316
-  _globals['_PROXYSERVICE']._serialized_end=33433
+  _globals['_DESCRIBECOLLECTIONRESPONSE']._serialized_end=2723
+  _globals['_LOADCOLLECTIONREQUEST']._serialized_start=2726
+  _globals['_LOADCOLLECTIONREQUEST']._serialized_end=2910
+  _globals['_RELEASECOLLECTIONREQUEST']._serialized_start=2912
+  _globals['_RELEASECOLLECTIONREQUEST']._serialized_end=3033
+  _globals['_GETSTATISTICSREQUEST']._serialized_start=3036
+  _globals['_GETSTATISTICSREQUEST']._serialized_end=3207
+  _globals['_GETSTATISTICSRESPONSE']._serialized_start=3209
+  _globals['_GETSTATISTICSRESPONSE']._serialized_end=3327
+  _globals['_GETCOLLECTIONSTATISTICSREQUEST']._serialized_start=3329
+  _globals['_GETCOLLECTIONSTATISTICSREQUEST']._serialized_end=3456
+  _globals['_GETCOLLECTIONSTATISTICSRESPONSE']._serialized_start=3459
+  _globals['_GETCOLLECTIONSTATISTICSRESPONSE']._serialized_end=3587
+  _globals['_SHOWCOLLECTIONSREQUEST']._serialized_start=3590
+  _globals['_SHOWCOLLECTIONSREQUEST']._serialized_end=3770
+  _globals['_SHOWCOLLECTIONSRESPONSE']._serialized_start=3773
+  _globals['_SHOWCOLLECTIONSRESPONSE']._serialized_end=4020
+  _globals['_CREATEPARTITIONREQUEST']._serialized_start=4023
+  _globals['_CREATEPARTITIONREQUEST']._serialized_end=4166
+  _globals['_DROPPARTITIONREQUEST']._serialized_start=4169
+  _globals['_DROPPARTITIONREQUEST']._serialized_end=4310
+  _globals['_HASPARTITIONREQUEST']._serialized_start=4313
+  _globals['_HASPARTITIONREQUEST']._serialized_end=4453
+  _globals['_LOADPARTITIONSREQUEST']._serialized_start=4456
+  _globals['_LOADPARTITIONSREQUEST']._serialized_end=4665
+  _globals['_RELEASEPARTITIONSREQUEST']._serialized_start=4668
+  _globals['_RELEASEPARTITIONSREQUEST']._serialized_end=4814
+  _globals['_GETPARTITIONSTATISTICSREQUEST']._serialized_start=4817
+  _globals['_GETPARTITIONSTATISTICSREQUEST']._serialized_end=4958
+  _globals['_GETPARTITIONSTATISTICSRESPONSE']._serialized_start=4960
+  _globals['_GETPARTITIONSTATISTICSRESPONSE']._serialized_end=5087
+  _globals['_SHOWPARTITIONSREQUEST']._serialized_start=5090
+  _globals['_SHOWPARTITIONSREQUEST']._serialized_end=5304
+  _globals['_SHOWPARTITIONSRESPONSE']._serialized_start=5307
+  _globals['_SHOWPARTITIONSRESPONSE']._serialized_end=5517
+  _globals['_DESCRIBESEGMENTREQUEST']._serialized_start=5519
+  _globals['_DESCRIBESEGMENTREQUEST']._serialized_end=5628
+  _globals['_DESCRIBESEGMENTRESPONSE']._serialized_start=5631
+  _globals['_DESCRIBESEGMENTRESPONSE']._serialized_end=5774
+  _globals['_SHOWSEGMENTSREQUEST']._serialized_start=5776
+  _globals['_SHOWSEGMENTSREQUEST']._serialized_end=5884
+  _globals['_SHOWSEGMENTSRESPONSE']._serialized_start=5886
+  _globals['_SHOWSEGMENTSRESPONSE']._serialized_end=5973
+  _globals['_CREATEINDEXREQUEST']._serialized_start=5976
+  _globals['_CREATEINDEXREQUEST']._serialized_end=6188
+  _globals['_ALTERINDEXREQUEST']._serialized_start=6191
+  _globals['_ALTERINDEXREQUEST']._serialized_end=6382
+  _globals['_DESCRIBEINDEXREQUEST']._serialized_start=6385
+  _globals['_DESCRIBEINDEXREQUEST']._serialized_end=6561
+  _globals['_INDEXDESCRIPTION']._serialized_start=6564
+  _globals['_INDEXDESCRIPTION']._serialized_end=6841
+  _globals['_DESCRIBEINDEXRESPONSE']._serialized_start=6844
+  _globals['_DESCRIBEINDEXRESPONSE']._serialized_end=6979
+  _globals['_GETINDEXBUILDPROGRESSREQUEST']._serialized_start=6982
+  _globals['_GETINDEXBUILDPROGRESSREQUEST']._serialized_end=7147
+  _globals['_GETINDEXBUILDPROGRESSRESPONSE']._serialized_start=7149
+  _globals['_GETINDEXBUILDPROGRESSRESPONSE']._serialized_end=7267
+  _globals['_GETINDEXSTATEREQUEST']._serialized_start=7270
+  _globals['_GETINDEXSTATEREQUEST']._serialized_end=7427
+  _globals['_GETINDEXSTATERESPONSE']._serialized_start=7430
+  _globals['_GETINDEXSTATERESPONSE']._serialized_end=7567
+  _globals['_DROPINDEXREQUEST']._serialized_start=7570
+  _globals['_DROPINDEXREQUEST']._serialized_end=7723
+  _globals['_INSERTREQUEST']._serialized_start=7726
+  _globals['_INSERTREQUEST']._serialized_end=7950
+  _globals['_UPSERTREQUEST']._serialized_start=7953
+  _globals['_UPSERTREQUEST']._serialized_end=8177
+  _globals['_MUTATIONRESULT']._serialized_start=8180
+  _globals['_MUTATIONRESULT']._serialized_end=8420
+  _globals['_DELETEREQUEST']._serialized_start=8423
+  _globals['_DELETEREQUEST']._serialized_end=8656
+  _globals['_SUBSEARCHREQUEST']._serialized_start=8659
+  _globals['_SUBSEARCHREQUEST']._serialized_end=8835
+  _globals['_SEARCHREQUEST']._serialized_start=8838
+  _globals['_SEARCHREQUEST']._serialized_end=9426
+  _globals['_HITS']._serialized_start=9428
+  _globals['_HITS']._serialized_end=9481
+  _globals['_SEARCHRESULTS']._serialized_start=9484
+  _globals['_SEARCHRESULTS']._serialized_end=9625
+  _globals['_HYBRIDSEARCHREQUEST']._serialized_start=9628
+  _globals['_HYBRIDSEARCHREQUEST']._serialized_end=10085
+  _globals['_FLUSHREQUEST']._serialized_start=10087
+  _globals['_FLUSHREQUEST']._serialized_end=10197
+  _globals['_FLUSHRESPONSE']._serialized_start=10200
+  _globals['_FLUSHRESPONSE']._serialized_end=10867
+  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_start=10592
+  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_end=10673
+  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_start=10675
+  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_end=10761
+  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_start=10763
+  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_end=10815
+  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_start=10817
+  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_end=10867
+  _globals['_QUERYREQUEST']._serialized_start=10870
+  _globals['_QUERYREQUEST']._serialized_end=11281
+  _globals['_QUERYRESULTS']._serialized_start=11284
+  _globals['_QUERYRESULTS']._serialized_end=11444
+  _globals['_VECTORIDS']._serialized_start=11446
+  _globals['_VECTORIDS']._serialized_end=11571
+  _globals['_VECTORSARRAY']._serialized_start=11574
+  _globals['_VECTORSARRAY']._serialized_end=11705
+  _globals['_CALCDISTANCEREQUEST']._serialized_start=11708
+  _globals['_CALCDISTANCEREQUEST']._serialized_end=11929
+  _globals['_CALCDISTANCERESULTS']._serialized_start=11932
+  _globals['_CALCDISTANCERESULTS']._serialized_end=12113
+  _globals['_FLUSHALLREQUEST']._serialized_start=12115
+  _globals['_FLUSHALLREQUEST']._serialized_end=12213
+  _globals['_FLUSHALLRESPONSE']._serialized_start=12215
+  _globals['_FLUSHALLRESPONSE']._serialized_end=12300
+  _globals['_PERSISTENTSEGMENTINFO']._serialized_start=12303
+  _globals['_PERSISTENTSEGMENTINFO']._serialized_end=12456
+  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_start=12458
+  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_end=12575
+  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_start=12578
+  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_end=12716
+  _globals['_QUERYSEGMENTINFO']._serialized_start=12719
+  _globals['_QUERYSEGMENTINFO']._serialized_end=12959
+  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_start=12961
+  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_end=13073
+  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_start=13076
+  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_end=13204
+  _globals['_DUMMYREQUEST']._serialized_start=13206
+  _globals['_DUMMYREQUEST']._serialized_end=13242
+  _globals['_DUMMYRESPONSE']._serialized_start=13244
+  _globals['_DUMMYRESPONSE']._serialized_end=13277
+  _globals['_REGISTERLINKREQUEST']._serialized_start=13279
+  _globals['_REGISTERLINKREQUEST']._serialized_end=13300
+  _globals['_REGISTERLINKRESPONSE']._serialized_start=13302
+  _globals['_REGISTERLINKRESPONSE']._serialized_end=13416
+  _globals['_GETMETRICSREQUEST']._serialized_start=13418
+  _globals['_GETMETRICSREQUEST']._serialized_end=13498
+  _globals['_GETMETRICSRESPONSE']._serialized_start=13500
+  _globals['_GETMETRICSRESPONSE']._serialized_end=13607
+  _globals['_COMPONENTINFO']._serialized_start=13610
+  _globals['_COMPONENTINFO']._serialized_end=13762
+  _globals['_COMPONENTSTATES']._serialized_start=13765
+  _globals['_COMPONENTSTATES']._serialized_end=13943
+  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_start=13945
+  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_end=13972
+  _globals['_LOADBALANCEREQUEST']._serialized_start=13975
+  _globals['_LOADBALANCEREQUEST']._serialized_end=14157
+  _globals['_MANUALCOMPACTIONREQUEST']._serialized_start=14159
+  _globals['_MANUALCOMPACTIONREQUEST']._serialized_end=14260
+  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_start=14262
+  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_end=14384
+  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_start=14386
+  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_end=14435
+  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_start=14438
+  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_end=14659
+  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_start=14661
+  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_end=14710
+  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_start=14713
+  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_end=14901
+  _globals['_COMPACTIONMERGEINFO']._serialized_start=14903
+  _globals['_COMPACTIONMERGEINFO']._serialized_end=14957
+  _globals['_GETFLUSHSTATEREQUEST']._serialized_start=14959
+  _globals['_GETFLUSHSTATEREQUEST']._serialized_end=15070
+  _globals['_GETFLUSHSTATERESPONSE']._serialized_start=15072
+  _globals['_GETFLUSHSTATERESPONSE']._serialized_end=15157
+  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_start=15159
+  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_end=15267
+  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_start=15269
+  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_end=15357
+  _globals['_IMPORTREQUEST']._serialized_start=15360
+  _globals['_IMPORTREQUEST']._serialized_end=15584
+  _globals['_IMPORTRESPONSE']._serialized_start=15586
+  _globals['_IMPORTRESPONSE']._serialized_end=15662
+  _globals['_GETIMPORTSTATEREQUEST']._serialized_start=15664
+  _globals['_GETIMPORTSTATEREQUEST']._serialized_end=15701
+  _globals['_GETIMPORTSTATERESPONSE']._serialized_start=15704
+  _globals['_GETIMPORTSTATERESPONSE']._serialized_end=15983
+  _globals['_LISTIMPORTTASKSREQUEST']._serialized_start=15985
+  _globals['_LISTIMPORTTASKSREQUEST']._serialized_end=16066
+  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_start=16069
+  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_end=16199
+  _globals['_GETREPLICASREQUEST']._serialized_start=16202
+  _globals['_GETREPLICASREQUEST']._serialized_end=16356
+  _globals['_GETREPLICASRESPONSE']._serialized_start=16358
+  _globals['_GETREPLICASRESPONSE']._serialized_end=16476
+  _globals['_REPLICAINFO']._serialized_start=16479
+  _globals['_REPLICAINFO']._serialized_end=16800
+  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_start=16746
+  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_end=16800
+  _globals['_SHARDREPLICA']._serialized_start=16802
+  _globals['_SHARDREPLICA']._serialized_end=16898
+  _globals['_CREATECREDENTIALREQUEST']._serialized_start=16901
+  _globals['_CREATECREDENTIALREQUEST']._serialized_end=17091
+  _globals['_UPDATECREDENTIALREQUEST']._serialized_start=17094
+  _globals['_UPDATECREDENTIALREQUEST']._serialized_end=17299
+  _globals['_DELETECREDENTIALREQUEST']._serialized_start=17301
+  _globals['_DELETECREDENTIALREQUEST']._serialized_end=17408
+  _globals['_LISTCREDUSERSRESPONSE']._serialized_start=17410
+  _globals['_LISTCREDUSERSRESPONSE']._serialized_end=17497
+  _globals['_LISTCREDUSERSREQUEST']._serialized_start=17499
+  _globals['_LISTCREDUSERSREQUEST']._serialized_end=17585
+  _globals['_ROLEENTITY']._serialized_start=17587
+  _globals['_ROLEENTITY']._serialized_end=17613
+  _globals['_USERENTITY']._serialized_start=17615
+  _globals['_USERENTITY']._serialized_end=17641
+  _globals['_CREATEROLEREQUEST']._serialized_start=17644
+  _globals['_CREATEROLEREQUEST']._serialized_end=17776
+  _globals['_DROPROLEREQUEST']._serialized_start=17778
+  _globals['_DROPROLEREQUEST']._serialized_end=17878
+  _globals['_OPERATEUSERROLEREQUEST']._serialized_start=17881
+  _globals['_OPERATEUSERROLEREQUEST']._serialized_end=18062
+  _globals['_SELECTROLEREQUEST']._serialized_start=18065
+  _globals['_SELECTROLEREQUEST']._serialized_end=18222
+  _globals['_ROLERESULT']._serialized_start=18224
+  _globals['_ROLERESULT']._serialized_end=18331
+  _globals['_SELECTROLERESPONSE']._serialized_start=18333
+  _globals['_SELECTROLERESPONSE']._serialized_end=18448
+  _globals['_SELECTUSERREQUEST']._serialized_start=18451
+  _globals['_SELECTUSERREQUEST']._serialized_end=18599
+  _globals['_USERRESULT']._serialized_start=18601
+  _globals['_USERRESULT']._serialized_end=18708
+  _globals['_SELECTUSERRESPONSE']._serialized_start=18710
+  _globals['_SELECTUSERRESPONSE']._serialized_end=18825
+  _globals['_OBJECTENTITY']._serialized_start=18827
+  _globals['_OBJECTENTITY']._serialized_end=18855
+  _globals['_PRIVILEGEENTITY']._serialized_start=18857
+  _globals['_PRIVILEGEENTITY']._serialized_end=18888
+  _globals['_GRANTORENTITY']._serialized_start=18890
+  _globals['_GRANTORENTITY']._serialized_end=19009
+  _globals['_GRANTPRIVILEGEENTITY']._serialized_start=19011
+  _globals['_GRANTPRIVILEGEENTITY']._serialized_end=19087
+  _globals['_GRANTENTITY']._serialized_start=19090
+  _globals['_GRANTENTITY']._serialized_end=19292
+  _globals['_SELECTGRANTREQUEST']._serialized_start=19295
+  _globals['_SELECTGRANTREQUEST']._serialized_end=19429
+  _globals['_SELECTGRANTRESPONSE']._serialized_start=19431
+  _globals['_SELECTGRANTRESPONSE']._serialized_end=19549
+  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_start=19552
+  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_end=19748
+  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_start=19751
+  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_end=19898
+  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_start=19900
+  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_end=20017
+  _globals['_GETLOADSTATEREQUEST']._serialized_start=20020
+  _globals['_GETLOADSTATEREQUEST']._serialized_end=20161
+  _globals['_GETLOADSTATERESPONSE']._serialized_start=20163
+  _globals['_GETLOADSTATERESPONSE']._serialized_end=20277
+  _globals['_MILVUSEXT']._serialized_start=20279
+  _globals['_MILVUSEXT']._serialized_end=20307
+  _globals['_GETVERSIONREQUEST']._serialized_start=20309
+  _globals['_GETVERSIONREQUEST']._serialized_end=20328
+  _globals['_GETVERSIONRESPONSE']._serialized_start=20330
+  _globals['_GETVERSIONRESPONSE']._serialized_end=20412
+  _globals['_CHECKHEALTHREQUEST']._serialized_start=20414
+  _globals['_CHECKHEALTHREQUEST']._serialized_end=20434
+  _globals['_CHECKHEALTHRESPONSE']._serialized_start=20437
+  _globals['_CHECKHEALTHRESPONSE']._serialized_end=20594
+  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_start=20597
+  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_end=20767
+  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_start=20770
+  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_end=21051
+  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_start=20940
+  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_end=21031
+  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_start=21053
+  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_end=21167
+  _globals['_TRANSFERNODEREQUEST']._serialized_start=21170
+  _globals['_TRANSFERNODEREQUEST']._serialized_end=21335
+  _globals['_TRANSFERREPLICAREQUEST']._serialized_start=21338
+  _globals['_TRANSFERREPLICAREQUEST']._serialized_end=21551
+  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_start=21553
+  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_end=21644
+  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_start=21646
+  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_end=21744
+  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_start=21746
+  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_end=21864
+  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_start=21867
+  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_end=22003
+  _globals['_RESOURCEGROUP']._serialized_start=22006
+  _globals['_RESOURCEGROUP']._serialized_end=22604
+  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_start=22437
+  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_end=22492
+  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_start=22494
+  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_end=22548
+  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_start=22550
+  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_end=22604
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=22607
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=22766
+  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_start=22769
+  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_end=22930
+  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_start=22933
+  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_end=23073
+  _globals['_CONNECTREQUEST']._serialized_start=23075
+  _globals['_CONNECTREQUEST']._serialized_end=23189
+  _globals['_CONNECTRESPONSE']._serialized_start=23192
+  _globals['_CONNECTRESPONSE']._serialized_end=23328
+  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_start=23330
+  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_end=23397
+  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_start=23399
+  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_end=23487
+  _globals['_CREATEDATABASEREQUEST']._serialized_start=23489
+  _globals['_CREATEDATABASEREQUEST']._serialized_end=23593
+  _globals['_DROPDATABASEREQUEST']._serialized_start=23595
+  _globals['_DROPDATABASEREQUEST']._serialized_end=23697
+  _globals['_LISTDATABASESREQUEST']._serialized_start=23699
+  _globals['_LISTDATABASESREQUEST']._serialized_end=23765
+  _globals['_LISTDATABASESRESPONSE']._serialized_start=23767
+  _globals['_LISTDATABASESRESPONSE']._serialized_end=23880
+  _globals['_ALTERDATABASEREQUEST']._serialized_start=23883
+  _globals['_ALTERDATABASEREQUEST']._serialized_end=24056
+  _globals['_REPLICATEMESSAGEREQUEST']._serialized_start=24059
+  _globals['_REPLICATEMESSAGEREQUEST']._serialized_end=24304
+  _globals['_REPLICATEMESSAGERESPONSE']._serialized_start=24306
+  _globals['_REPLICATEMESSAGERESPONSE']._serialized_end=24395
+  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_start=24397
+  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_end=24495
+  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_start=24497
+  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_end=24557
+  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_start=24559
+  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_end=24638
+  _globals['_MILVUSSERVICE']._serialized_start=24888
+  _globals['_MILVUSSERVICE']._serialized_end=33535
+  _globals['_PROXYSERVICE']._serialized_start=33537
+  _globals['_PROXYSERVICE']._serialized_end=33654
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     db_name: str
     collection_name: str
     collectionID: int
     time_stamp: int
     def __init__(self, base: _Optional[_Union[_common_pb2.MsgBase, _Mapping]] = ..., db_name: _Optional[str] = ..., collection_name: _Optional[str] = ..., collectionID: _Optional[int] = ..., time_stamp: _Optional[int] = ...) -> None: ...
 
 class DescribeCollectionResponse(_message.Message):
-    __slots__ = ("status", "schema", "collectionID", "virtual_channel_names", "physical_channel_names", "created_timestamp", "created_utc_timestamp", "shards_num", "aliases", "start_positions", "consistency_level", "collection_name", "properties", "db_name", "num_partitions")
+    __slots__ = ("status", "schema", "collectionID", "virtual_channel_names", "physical_channel_names", "created_timestamp", "created_utc_timestamp", "shards_num", "aliases", "start_positions", "consistency_level", "collection_name", "properties", "db_name", "num_partitions", "db_id")
     STATUS_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_FIELD_NUMBER: _ClassVar[int]
     COLLECTIONID_FIELD_NUMBER: _ClassVar[int]
     VIRTUAL_CHANNEL_NAMES_FIELD_NUMBER: _ClassVar[int]
     PHYSICAL_CHANNEL_NAMES_FIELD_NUMBER: _ClassVar[int]
     CREATED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     CREATED_UTC_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
@@ -225,14 +225,15 @@
     ALIASES_FIELD_NUMBER: _ClassVar[int]
     START_POSITIONS_FIELD_NUMBER: _ClassVar[int]
     CONSISTENCY_LEVEL_FIELD_NUMBER: _ClassVar[int]
     COLLECTION_NAME_FIELD_NUMBER: _ClassVar[int]
     PROPERTIES_FIELD_NUMBER: _ClassVar[int]
     DB_NAME_FIELD_NUMBER: _ClassVar[int]
     NUM_PARTITIONS_FIELD_NUMBER: _ClassVar[int]
+    DB_ID_FIELD_NUMBER: _ClassVar[int]
     status: _common_pb2.Status
     schema: _schema_pb2.CollectionSchema
     collectionID: int
     virtual_channel_names: _containers.RepeatedScalarFieldContainer[str]
     physical_channel_names: _containers.RepeatedScalarFieldContainer[str]
     created_timestamp: int
     created_utc_timestamp: int
@@ -240,15 +241,16 @@
     aliases: _containers.RepeatedScalarFieldContainer[str]
     start_positions: _containers.RepeatedCompositeFieldContainer[_common_pb2.KeyDataPair]
     consistency_level: _common_pb2.ConsistencyLevel
     collection_name: str
     properties: _containers.RepeatedCompositeFieldContainer[_common_pb2.KeyValuePair]
     db_name: str
     num_partitions: int
-    def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., schema: _Optional[_Union[_schema_pb2.CollectionSchema, _Mapping]] = ..., collectionID: _Optional[int] = ..., virtual_channel_names: _Optional[_Iterable[str]] = ..., physical_channel_names: _Optional[_Iterable[str]] = ..., created_timestamp: _Optional[int] = ..., created_utc_timestamp: _Optional[int] = ..., shards_num: _Optional[int] = ..., aliases: _Optional[_Iterable[str]] = ..., start_positions: _Optional[_Iterable[_Union[_common_pb2.KeyDataPair, _Mapping]]] = ..., consistency_level: _Optional[_Union[_common_pb2.ConsistencyLevel, str]] = ..., collection_name: _Optional[str] = ..., properties: _Optional[_Iterable[_Union[_common_pb2.KeyValuePair, _Mapping]]] = ..., db_name: _Optional[str] = ..., num_partitions: _Optional[int] = ...) -> None: ...
+    db_id: int
+    def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., schema: _Optional[_Union[_schema_pb2.CollectionSchema, _Mapping]] = ..., collectionID: _Optional[int] = ..., virtual_channel_names: _Optional[_Iterable[str]] = ..., physical_channel_names: _Optional[_Iterable[str]] = ..., created_timestamp: _Optional[int] = ..., created_utc_timestamp: _Optional[int] = ..., shards_num: _Optional[int] = ..., aliases: _Optional[_Iterable[str]] = ..., start_positions: _Optional[_Iterable[_Union[_common_pb2.KeyDataPair, _Mapping]]] = ..., consistency_level: _Optional[_Union[_common_pb2.ConsistencyLevel, str]] = ..., collection_name: _Optional[str] = ..., properties: _Optional[_Iterable[_Union[_common_pb2.KeyValuePair, _Mapping]]] = ..., db_name: _Optional[str] = ..., num_partitions: _Optional[int] = ..., db_id: _Optional[int] = ...) -> None: ...
 
 class LoadCollectionRequest(_message.Message):
     __slots__ = ("base", "db_name", "collection_name", "replica_number", "resource_groups", "refresh")
     BASE_FIELD_NUMBER: _ClassVar[int]
     DB_NAME_FIELD_NUMBER: _ClassVar[int]
     COLLECTION_NAME_FIELD_NUMBER: _ClassVar[int]
     REPLICA_NUMBER_FIELD_NUMBER: _ClassVar[int]
@@ -1879,14 +1881,26 @@
     DB_NAMES_FIELD_NUMBER: _ClassVar[int]
     CREATED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     status: _common_pb2.Status
     db_names: _containers.RepeatedScalarFieldContainer[str]
     created_timestamp: _containers.RepeatedScalarFieldContainer[int]
     def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., db_names: _Optional[_Iterable[str]] = ..., created_timestamp: _Optional[_Iterable[int]] = ...) -> None: ...
 
+class AlterDatabaseRequest(_message.Message):
+    __slots__ = ("base", "db_name", "db_id", "properties")
+    BASE_FIELD_NUMBER: _ClassVar[int]
+    DB_NAME_FIELD_NUMBER: _ClassVar[int]
+    DB_ID_FIELD_NUMBER: _ClassVar[int]
+    PROPERTIES_FIELD_NUMBER: _ClassVar[int]
+    base: _common_pb2.MsgBase
+    db_name: str
+    db_id: str
+    properties: _containers.RepeatedCompositeFieldContainer[_common_pb2.KeyValuePair]
+    def __init__(self, base: _Optional[_Union[_common_pb2.MsgBase, _Mapping]] = ..., db_name: _Optional[str] = ..., db_id: _Optional[str] = ..., properties: _Optional[_Iterable[_Union[_common_pb2.KeyValuePair, _Mapping]]] = ...) -> None: ...
+
 class ReplicateMessageRequest(_message.Message):
     __slots__ = ("base", "channel_name", "BeginTs", "EndTs", "Msgs", "StartPositions", "EndPositions")
     BASE_FIELD_NUMBER: _ClassVar[int]
     CHANNEL_NAME_FIELD_NUMBER: _ClassVar[int]
     BEGINTS_FIELD_NUMBER: _ClassVar[int]
     ENDTS_FIELD_NUMBER: _ClassVar[int]
     MSGS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,14 +427,19 @@
                 response_deserializer=common__pb2.Status.FromString,
                 )
         self.ListDatabases = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/ListDatabases',
                 request_serializer=milvus__pb2.ListDatabasesRequest.SerializeToString,
                 response_deserializer=milvus__pb2.ListDatabasesResponse.FromString,
                 )
+        self.AlterDatabase = channel.unary_unary(
+                '/milvus.proto.milvus.MilvusService/AlterDatabase',
+                request_serializer=milvus__pb2.AlterDatabaseRequest.SerializeToString,
+                response_deserializer=common__pb2.Status.FromString,
+                )
         self.ReplicateMessage = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/ReplicateMessage',
                 request_serializer=milvus__pb2.ReplicateMessageRequest.SerializeToString,
                 response_deserializer=milvus__pb2.ReplicateMessageResponse.FromString,
                 )
 
 
@@ -942,14 +947,20 @@
 
     def ListDatabases(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def AlterDatabase(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ReplicateMessage(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -1366,14 +1377,19 @@
                     response_serializer=common__pb2.Status.SerializeToString,
             ),
             'ListDatabases': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDatabases,
                     request_deserializer=milvus__pb2.ListDatabasesRequest.FromString,
                     response_serializer=milvus__pb2.ListDatabasesResponse.SerializeToString,
             ),
+            'AlterDatabase': grpc.unary_unary_rpc_method_handler(
+                    servicer.AlterDatabase,
+                    request_deserializer=milvus__pb2.AlterDatabaseRequest.FromString,
+                    response_serializer=common__pb2.Status.SerializeToString,
+            ),
             'ReplicateMessage': grpc.unary_unary_rpc_method_handler(
                     servicer.ReplicateMessage,
                     request_deserializer=milvus__pb2.ReplicateMessageRequest.FromString,
                     response_serializer=milvus__pb2.ReplicateMessageResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -2793,14 +2809,31 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/ListDatabases',
             milvus__pb2.ListDatabasesRequest.SerializeToString,
             milvus__pb2.ListDatabasesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def AlterDatabase(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/AlterDatabase',
+            milvus__pb2.AlterDatabaseRequest.SerializeToString,
+            common__pb2.Status.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ReplicateMessage(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/msg_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/msg_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/python_gen.sh` & `pymilvus-2.4.1/pymilvus/grpc_gen/python_gen.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/rg_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x08rg.proto\x12\x0fmilvus.proto.rg\"%\n\x12ResourceGroupLimit\x12\x0f\n\x07nodeNum\x18\x01 \x01(\x05\"/\n\x15ResourceGroupTransfer\x12\x16\n\x0eresource_group\x18\x01 \x01(\t\"\xeb\x01\n\x13ResourceGroupConfig\x12\x35\n\x08requests\x18\x01 \x01(\x0b\x32#.milvus.proto.rg.ResourceGroupLimit\x12\x33\n\x06limits\x18\x02 \x01(\x0b\x32#.milvus.proto.rg.ResourceGroupLimit\x12\x34\n\x04\x66rom\x18\x03 \x03(\x0b\x32&.milvus.proto.rg.ResourceGroupTransfer\x12\x32\n\x02to\x18\x04 \x03(\x0b\x32&.milvus.proto.rg.ResourceGroupTransferBp\n\x0eio.milvus.grpcB\x12ResourceGroupProtoP\x01Z0github.com/milvus-io/milvus-proto/go-api/v2/rgpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x08rg.proto\x12\x0fmilvus.proto.rg\"&\n\x12ResourceGroupLimit\x12\x10\n\x08node_num\x18\x01 \x01(\x05\"/\n\x15ResourceGroupTransfer\x12\x16\n\x0eresource_group\x18\x01 \x01(\t\"\xfd\x01\n\x13ResourceGroupConfig\x12\x35\n\x08requests\x18\x01 \x01(\x0b\x32#.milvus.proto.rg.ResourceGroupLimit\x12\x33\n\x06limits\x18\x02 \x01(\x0b\x32#.milvus.proto.rg.ResourceGroupLimit\x12=\n\rtransfer_from\x18\x03 \x03(\x0b\x32&.milvus.proto.rg.ResourceGroupTransfer\x12;\n\x0btransfer_to\x18\x04 \x03(\x0b\x32&.milvus.proto.rg.ResourceGroupTransferBp\n\x0eio.milvus.grpcB\x12ResourceGroupProtoP\x01Z0github.com/milvus-io/milvus-proto/go-api/v2/rgpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rg_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\016io.milvus.grpcB\022ResourceGroupProtoP\001Z0github.com/milvus-io/milvus-proto/go-api/v2/rgpb\240\001\001\252\002\022Milvus.Client.Grpc'
   _globals['_RESOURCEGROUPLIMIT']._serialized_start=29
-  _globals['_RESOURCEGROUPLIMIT']._serialized_end=66
-  _globals['_RESOURCEGROUPTRANSFER']._serialized_start=68
-  _globals['_RESOURCEGROUPTRANSFER']._serialized_end=115
-  _globals['_RESOURCEGROUPCONFIG']._serialized_start=118
-  _globals['_RESOURCEGROUPCONFIG']._serialized_end=353
+  _globals['_RESOURCEGROUPLIMIT']._serialized_end=67
+  _globals['_RESOURCEGROUPTRANSFER']._serialized_start=69
+  _globals['_RESOURCEGROUPTRANSFER']._serialized_end=116
+  _globals['_RESOURCEGROUPCONFIG']._serialized_start=119
+  _globals['_RESOURCEGROUPCONFIG']._serialized_end=372
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/rg_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ResourceGroupLimit(_message.Message):
-    __slots__ = ("nodeNum",)
-    NODENUM_FIELD_NUMBER: _ClassVar[int]
-    nodeNum: int
-    def __init__(self, nodeNum: _Optional[int] = ...) -> None: ...
+    __slots__ = ("node_num",)
+    NODE_NUM_FIELD_NUMBER: _ClassVar[int]
+    node_num: int
+    def __init__(self, node_num: _Optional[int] = ...) -> None: ...
 
 class ResourceGroupTransfer(_message.Message):
     __slots__ = ("resource_group",)
     RESOURCE_GROUP_FIELD_NUMBER: _ClassVar[int]
     resource_group: str
     def __init__(self, resource_group: _Optional[str] = ...) -> None: ...
 
 class ResourceGroupConfig(_message.Message):
-    __slots__ = ("requests", "limits", "to")
+    __slots__ = ("requests", "limits", "transfer_from", "transfer_to")
     REQUESTS_FIELD_NUMBER: _ClassVar[int]
     LIMITS_FIELD_NUMBER: _ClassVar[int]
-    FROM_FIELD_NUMBER: _ClassVar[int]
-    TO_FIELD_NUMBER: _ClassVar[int]
+    TRANSFER_FROM_FIELD_NUMBER: _ClassVar[int]
+    TRANSFER_TO_FIELD_NUMBER: _ClassVar[int]
     requests: ResourceGroupLimit
     limits: ResourceGroupLimit
-    to: _containers.RepeatedCompositeFieldContainer[ResourceGroupTransfer]
-    def __init__(self, requests: _Optional[_Union[ResourceGroupLimit, _Mapping]] = ..., limits: _Optional[_Union[ResourceGroupLimit, _Mapping]] = ..., to: _Optional[_Iterable[_Union[ResourceGroupTransfer, _Mapping]]] = ..., **kwargs) -> None: ...
+    transfer_from: _containers.RepeatedCompositeFieldContainer[ResourceGroupTransfer]
+    transfer_to: _containers.RepeatedCompositeFieldContainer[ResourceGroupTransfer]
+    def __init__(self, requests: _Optional[_Union[ResourceGroupLimit, _Mapping]] = ..., limits: _Optional[_Union[ResourceGroupLimit, _Mapping]] = ..., transfer_from: _Optional[_Iterable[_Union[ResourceGroupTransfer, _Mapping]]] = ..., transfer_to: _Optional[_Iterable[_Union[ResourceGroupTransfer, _Mapping]]] = ...) -> None: ...
```

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/schema_pb2.py` & `pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/grpc_gen/schema_pb2.pyi` & `pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/milvus_client/index.py` & `pymilvus-2.4.1/pymilvus/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/milvus_client/milvus_client.py` & `pymilvus-2.4.1/pymilvus/milvus_client/milvus_client.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/model/__init__.py` & `pymilvus-2.4.1/pymilvus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/__init__.py` & `pymilvus-2.4.1/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/collection.py` & `pymilvus-2.4.1/pymilvus/orm/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     AutoIDException,
     DataTypeNotMatchException,
     DataTypeNotSupportException,
     ExceptionsMessage,
     IndexNotExistException,
     PartitionAlreadyExistException,
     SchemaNotReadyException,
+    UpsertAutoIDTrueException,
 )
 from pymilvus.grpc_gen import schema_pb2
 from pymilvus.settings import Config
 
 from .connections import connections
 from .constants import UNLIMITED
 from .future import MutationFuture, SearchFuture
@@ -46,18 +47,19 @@
 from .mutation import MutationResult
 from .partition import Partition
 from .prepare import Prepare
 from .schema import (
     CollectionSchema,
     FieldSchema,
     check_insert_schema,
-    check_is_row_based,
     check_schema,
     check_upsert_schema,
     construct_fields_from_dataframe,
+    is_row_based,
+    is_valid_insert_data,
 )
 from .types import DataType
 from .utility import _get_connection
 
 
 class Collection:
     def __init__(
@@ -237,15 +239,15 @@
         conn = self._get_connection()
         resp = conn.describe_collection(self._name, **kwargs)
         return resp["aliases"]
 
     @property
     def description(self) -> str:
         """str: a text description of the collection."""
-        return self._schema.description
+        return self.schema.description
 
     @property
     def name(self) -> str:
         """str: the name of the collection."""
         return self._name
 
     @property
@@ -285,15 +287,15 @@
         result = {stat.key: stat.value for stat in stats}
         result["row_count"] = int(result["row_count"])
         return result["row_count"]
 
     @property
     def primary_field(self) -> FieldSchema:
         """FieldSchema: the primary field of the collection."""
-        return self._schema.primary_field
+        return self.schema.primary_field
 
     def flush(self, timeout: Optional[float] = None, **kwargs):
         """Seal all segments in the collection. Inserts after flushing will be written into
             new segments. Only sealed segments can be indexed.
 
         Args:
             timeout (float): an optional duration of time in seconds to allow for the RPCs.
@@ -486,33 +488,36 @@
             ...     [random.randint(1, 100) for _ in range(10)],
             ...     [[random.random() for _ in range(2)] for _ in range(10)],
             ... ]
             >>> res = collection.insert(data)
             >>> res.insert_count
             10
         """
-        if data is None:
-            return MutationResult(data)
-        row_based = check_is_row_based(data)
-        conn = self._get_connection()
-        if not row_based:
-            check_insert_schema(self._schema, data)
-            entities = Prepare.prepare_insert_data(data, self._schema)
-            return conn.batch_insert(
-                self._name,
-                entities,
-                partition_name,
+        if not is_valid_insert_data(data):
+            raise DataTypeNotSupportException(
+                message="The type of data should be List, pd.DataFrame or Dict"
+            )
+
+        conn = self._get_connection()
+        if is_row_based(data):
+            return conn.insert_rows(
+                collection_name=self._name,
+                entities=data,
+                partition_name=partition_name,
                 timeout=timeout,
                 schema=self._schema_dict,
                 **kwargs,
             )
-        return conn.insert_rows(
-            collection_name=self._name,
-            entities=data,
-            partition_name=partition_name,
+
+        check_insert_schema(self.schema, data)
+        entities = Prepare.prepare_insert_data(data, self.schema)
+        return conn.batch_insert(
+            self._name,
+            entities,
+            partition_name,
             timeout=timeout,
             schema=self._schema_dict,
             **kwargs,
         )
 
     def delete(
         self,
@@ -610,45 +615,47 @@
             ...     [random.randint(1, 100) for _ in range(10)],
             ...     [[random.random() for _ in range(2)] for _ in range(10)],
             ... ]
             >>> res = collection.upsert(data)
             >>> res.upsert_count
             10
         """
-        if data is None:
-            return MutationResult(data)
 
-        row_based = check_is_row_based(data)
-        conn = self._get_connection()
-        if not row_based:
-            check_upsert_schema(self._schema, data)
-            entities = Prepare.prepare_upsert_data(data, self._schema)
+        if self.schema.auto_id:
+            raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
 
-            res = conn.upsert(
-                self._name,
-                entities,
-                partition_name,
-                timeout=timeout,
-                schema=self._schema_dict,
-                **kwargs,
+        if not is_valid_insert_data(data):
+            raise DataTypeNotSupportException(
+                message="The type of data should be List, pd.DataFrame or Dict"
             )
 
-            if kwargs.get("_async", False):
-                return MutationFuture(res)
-        else:
+        conn = self._get_connection()
+        if is_row_based(data):
             res = conn.upsert_rows(
                 self._name,
                 data,
                 partition_name,
                 timeout=timeout,
                 schema=self._schema_dict,
                 **kwargs,
             )
+            return MutationResult(res)
 
-        return MutationResult(res)
+        check_upsert_schema(self.schema, data)
+        entities = Prepare.prepare_upsert_data(data, self.schema)
+        res = conn.upsert(
+            self._name,
+            entities,
+            partition_name,
+            timeout=timeout,
+            schema=self._schema_dict,
+            **kwargs,
+        )
+
+        return MutationFuture(res) if kwargs.get("_async", False) else MutationResult(res)
 
     def search(
         self,
         data: Union[List, entity_helper.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
```

### Comparing `pymilvus-2.4.0/pymilvus/orm/connections.py` & `pymilvus-2.4.1/pymilvus/orm/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,14 +250,16 @@
             if not is_legal_address(address):
                 raise ConnectionConfigException(
                     message=f"Illegal address: {address}, should be in form 'localhost:19530'"
                 )
             return address, None
 
         if uri != "":
+            if isinstance(uri, str) and uri.startswith("unix:"):
+                return uri, None
             address, parsed = self.__parse_address_from_uri(uri)
             return address, parsed
 
         _host = host if host != "" else Config.DEFAULT_HOST
         _port = port if port != "" else Config.DEFAULT_PORT
         self.__verify_host_port(_host, _port)
```

### Comparing `pymilvus-2.4.0/pymilvus/orm/constants.py` & `pymilvus-2.4.1/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/db.py` & `pymilvus-2.4.1/pymilvus/orm/db.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/future.py` & `pymilvus-2.4.1/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/index.py` & `pymilvus-2.4.1/pymilvus/orm/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/iterator.py` & `pymilvus-2.4.1/pymilvus/orm/iterator.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/mutation.py` & `pymilvus-2.4.1/pymilvus/orm/mutation.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/partition.py` & `pymilvus-2.4.1/pymilvus/orm/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/role.py` & `pymilvus-2.4.1/pymilvus/orm/role.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/schema.py` & `pymilvus-2.4.1/pymilvus/orm/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,21 +345,21 @@
             DataType.VARCHAR,
             DataType.ARRAY,
             DataType.SPARSE_FLOAT_VECTOR,
         ):
             return
         if not self._kwargs:
             return
-        # currently only support ndim
+        # currently only support "dim", "max_length", "max_capacity"
         if self._kwargs:
             for k in COMMON_TYPE_PARAMS:
                 if k in self._kwargs:
                     if self._type_params is None:
                         self._type_params = {}
-                    self._type_params[k] = self._kwargs[k]
+                    self._type_params[k] = int(self._kwargs[k])
 
     @classmethod
     def construct_from_dict(cls, raw: Dict):
         kwargs = {}
         kwargs.update(raw.get("params", {}))
         kwargs["is_primary"] = raw.get("is_primary", False)
         if raw.get("auto_id") is not None:
@@ -437,14 +437,26 @@
         return self._type_params
 
     @property
     def dtype(self) -> DataType:
         return self._dtype
 
 
+def is_valid_insert_data(data: Union[pd.DataFrame, list, dict]) -> bool:
+    """DataFrame, list, dict are valid insert data"""
+    return isinstance(data, (pd.DataFrame, list, dict))
+
+
+def is_row_based(data: Union[Dict, List[Dict]]) -> bool:
+    """Dict or List[Dict] are row-based"""
+    return isinstance(data, dict) or (
+        isinstance(data, list) and len(data) > 0 and isinstance(data[0], Dict)
+    )
+
+
 def check_is_row_based(data: Union[List[List], List[Dict], Dict, pd.DataFrame]) -> bool:
     if not isinstance(data, (pd.DataFrame, list, dict)):
         raise DataTypeNotSupportException(
             message="The type of data should be list or pandas.DataFrame or dict"
         )
 
     if isinstance(data, pd.DataFrame):
```

### Comparing `pymilvus-2.4.0/pymilvus/orm/types.py` & `pymilvus-2.4.1/pymilvus/orm/types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus/orm/utility.py` & `pymilvus-2.4.1/pymilvus/orm/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 from datetime import datetime, timedelta, timezone
-from typing import List, Optional
+from typing import List, Mapping, Optional
 
-from pymilvus.client.types import BulkInsertState
+from pymilvus.client.types import (
+    BulkInsertState,
+    ResourceGroupConfig,
+)
 from pymilvus.client.utils import hybridts_to_unixtime as _hybridts_to_unixtime
 from pymilvus.client.utils import mkts_from_datetime as _mkts_from_datetime
 from pymilvus.client.utils import mkts_from_hybridts as _mkts_from_hybridts
 from pymilvus.client.utils import mkts_from_unixtime as _mkts_from_unixtime
 from pymilvus.exceptions import MilvusException
 
 from .connections import connections
@@ -1071,26 +1074,65 @@
         >>> connections.connect()
         >>> utility.get_server_version()
         >>> "2.2.0"
     """
     return _get_connection(using).get_server_version(timeout=timeout)
 
 
-def create_resource_group(name: str, using: str = "default", timeout: Optional[float] = None):
+def create_resource_group(
+    name: str, using: str = "default", timeout: Optional[float] = None, **kwargs
+):
     """Create a resource group
         It will success whether or not the resource group exists.
 
     :example:
         >>> from pymilvus import connections, utility
         >>> connections.connect()
         >>> utility.create_resource_group(name)
         >>> rgs = utility.list_resource_groups()
         >>> print(f"resource groups in Milvus: {rgs}")
     """
-    return _get_connection(using).create_resource_group(name, timeout)
+    return _get_connection(using).create_resource_group(name, timeout, **kwargs)
+
+
+def update_resource_groups(
+    configs: Mapping[str, ResourceGroupConfig],
+    using: str = "default",
+    timeout: Optional[float] = None,
+):
+    """Update resource groups.
+        This function updates the resource groups based on the provided configurations.
+
+    :param configs: A mapping of resource group names to their configurations.
+    :type configs: Mapping[str, ResourceGroupConfig]
+    :param using: The name of the connection to use. Defaults to "default".
+    :type using: (str, optional)
+    :param timeout: The timeout value in seconds. Defaults to None.
+    :type timeout: (float, optional)
+
+    :example:
+        >>> from pymilvus import connections, utility
+        >>> connections.connect()
+        >>> configs = {
+        ...     "resource_group_1": ResourceGroupConfig(
+        ...         requests={"node_num": 1},
+        ...         limits={"node_num": 5},
+        ...         transfer_from=[{"resource_group": "resource_group_2"}],
+        ...         transfer_to=[{"resource_group": "resource_group_2"}],
+        ...     ),
+        ...     "resource_group_2": ResourceGroupConfig(
+        ...         requests={"node_num": 4},
+        ...         limits={"node_num": 4},
+        ...         transfer_from=[{"resource_group": "__default_resource_group"}],
+        ...         transfer_to=[{"resource_group": "resource_group_1"}],
+        ...     ),
+        ... }
+        >>> utility.update_resource_groups(configs)
+    """
+    return _get_connection(using).update_resource_groups(configs, timeout)
 
 
 def drop_resource_group(name: str, using: str = "default", timeout: Optional[float] = None):
     """Drop a resource group
         It will success if the resource group is existed and empty, otherwise fail.
 
     :example:
```

### Comparing `pymilvus-2.4.0/pymilvus/settings.py` & `pymilvus-2.4.1/pymilvus/settings.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.4.1/pymilvus.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,16 +16,24 @@
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
 Requires-Dist: requests
 Requires-Dist: minio>=7.0.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: azure-storage-blob
+Requires-Dist: scipy
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
+Provides-Extra: test
+Requires-Dist: pytest>=5.3.4; extra == "test"
+Requires-Dist: pytest-cov>=2.8.1; extra == "test"
+Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
+Requires-Dist: grpcio-testing; extra == "test"
+Requires-Dist: ruff>=0.3.3; extra == "test"
+Requires-Dist: black; extra == "test"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
 [![Downloads](https://static.pepy.tech/badge/pymilvus/month)](https://pepy.tech/project/pymilvus)
@@ -48,22 +56,24 @@
 |:-----:|:-----:|
 | 1.0.\* | 1.0.1 |
 | 1.1.\* | 1.1.2 |
 | 2.0.\* | 2.0.2 |
 | 2.1.\* | 2.1.3 |
 | 2.2.\* | 2.2.15 |
 | 2.3.\* | 2.3.7 |
+| 2.4.\* | 2.4.0 |
 
 
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
+$ pip3 install pymilvus[model] # for milvus-model
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -104,23 +114,36 @@
 A4.
 ```shell
 make lint
 ```
 
 Q5. How to fix the coding styles?
 
-Q5
+A5
 ```shell
 make format
 ```
 
+Q6. How to run unittests?
+
+A6
+```shell
+$ pip install ".[test]"
+$ make unittest
+```
+Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+
+A7
+```shell
+$ pip install "pymilvus[model]"
+```
 
 ## Documentation
 
-Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.3.x/About.md
+Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.4.x/About.md
 
 ## Developing package releases
 
 The commits on the development branch of each version will be packaged and uploaded to [Test PyPI](https://test.pypi.org/).
 
 The package name generated by the development branch is x.y.z.rc<dist>, where <dist> is the number of commits that differ from the most recent release.
```

### Comparing `pymilvus-2.4.0/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.4.1/pymilvus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Makefile
 OWNERS
 README.md
 _version_helper.py
 check_proto_product.sh
 pyproject.toml
 requirements.txt
-test_requirements.txt
 .github/mergify.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/enhancement.yaml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/ISSUE_TEMPLATE/general-question.yaml
 .github/workflows/check_milvus_proto.yml
@@ -87,14 +86,15 @@
 examples/multithreading_hello_milvus.py
 examples/old_style_example.py
 examples/old_style_example_index.py
 examples/old_style_example_str.py
 examples/old_style_query.py
 examples/partition.py
 examples/resource_group.py
+examples/resource_group_declarative_api.py
 examples/role_and_privilege.py
 examples/user.py
 examples/cert/ca.pem
 examples/cert/client.key
 examples/cert/client.pem
 examples/cert/server.pem
 examples/data/train_embeddings.csv
```

### Comparing `pymilvus-2.4.0/pyproject.toml` & `pymilvus-2.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "ujson>=2.0.0",
     "pandas>=1.2.4",
     "numpy<1.25.0;python_version<='3.8'",
     "requests",
     "minio>=7.0.0",
     "pyarrow>=12.0.0",
     "azure-storage-blob",
+    "scipy",
 ]
 
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 
@@ -41,22 +42,31 @@
 "repository" = 'https://github.com/milvus-io/pymilvus'
 
 [project.optional-dependencies]
 model = [
     "milvus-model>=0.1.0",
 ]
 
+test = [
+    "pytest>=5.3.4",
+    "pytest-cov>=2.8.1",
+    "pytest-timeout>=1.3.4",
+    "grpcio-testing",
+    "ruff>=0.3.3",
+    "black",
+]
+
 [tool.setuptools.dynamic]
 version = { attr = "_version_helper.version"}
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 100
-target-version = ['py37']
+target-version = ['py38']
 include = '\.pyi?$'
 extend-ignore = ["E203", "E501"]
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
 (
@@ -96,14 +106,15 @@
     "COM812",
     "FBT003", # [ruff] FBT003 Boolean positional value in function call [E] TODO
     "ARG002",
     "E501", # black takes care of it
     "ARG005", # [ruff] ARG005 Unused lambda argument: `disable` [E]
     "TRY400",
     "PLR0912", # TODO
+    "PLR0915", # To many statements TODO
     "C901", # TODO
     "PYI041", # TODO
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 lint.fixable = [
     "A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W",
```

### Comparing `pymilvus-2.4.0/requirements.txt` & `pymilvus-2.4.1/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 packaging==20.9
 pep517==0.10.0
 pyparsing==2.4.7
 six==1.16.0
 toml==0.10.2
 ujson>=2.0.0
 urllib3==1.26.18
-sklearn==0.0
 m2r==0.3.1
 scipy>=1.9.3
 Sphinx==4.0.0
 sphinx-copybutton
 sphinx-rtd-theme
 sphinxcontrib-applehelp
 sphinxcontrib-devhelp
```

### Comparing `pymilvus-2.4.0/tests/conftest.py` & `pymilvus-2.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/mock_milvus.py` & `pymilvus-2.4.1/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/mock_result.py` & `pymilvus-2.4.1/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_abstract.py` & `pymilvus-2.4.1/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_check.py` & `pymilvus-2.4.1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_collection.py` & `pymilvus-2.4.1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_connections.py` & `pymilvus-2.4.1/tests/test_connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import os
 
 import pytest
 import pymilvus
+from pymilvus import *
 from unittest import mock
 
 from pymilvus import connections
 from pymilvus import DefaultConfig, MilvusException
 from pymilvus.exceptions import ErrorCode
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `pymilvus-2.4.0/tests/test_create_collection.py` & `pymilvus-2.4.1/tests/test_create_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_decorators.py` & `pymilvus-2.4.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_grpc_handler.py` & `pymilvus-2.4.1/tests/test_grpc_handler.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_index.py` & `pymilvus-2.4.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_partition.py` & `pymilvus-2.4.1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_prepare.py` & `pymilvus-2.4.1/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_schema.py` & `pymilvus-2.4.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/test_ts_utils.py` & `pymilvus-2.4.1/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.0/tests/utils.py` & `pymilvus-2.4.1/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 import pandas
-from sklearn import preprocessing
+import numpy as np
 
 from pymilvus import DataType
 
 default_dim = 128
 default_nb = 1200
 default_nq = 10
 default_float_vec_field_name = "float_vector"
@@ -65,40 +65,37 @@
         FieldSchema(gen_field_name(), DataType.FLOAT),
         FieldSchema(gen_field_name(), DataType.FLOAT_VECTOR, dim=default_dim)
     ]
     collection_schema = CollectionSchema(fields)
     return collection_schema
 
 
-def gen_vectors(num, dim, is_normal=True):
-    vectors = [[random.random() for _ in range(dim)] for _ in range(num)]
-    vectors = preprocessing.normalize(vectors, axis=1, norm='l2')
-    return vectors.tolist()
+def gen_vectors(num, dim):
+    return [[random.random() for _ in range(dim)] for _ in range(num)]
 
 
 def gen_int_attr(row_num):
     return [random.randint(0, 255) for _ in range(row_num)]
 
 
 # pandas.DataFrame
-def gen_pd_data(nb, is_normal=False):
-    import numpy
-    vectors = gen_vectors(nb, default_dim, is_normal)
+def gen_pd_data(nb):
+    vectors = gen_vectors(nb, default_dim)
     datas = {
         "int64": [i for i in range(nb)],
-        "float": numpy.array([i for i in range(nb)], dtype=numpy.float32),
+        "float": np.array([i for i in range(nb)], dtype=np.float32),
         default_float_vec_field_name: vectors
     }
     data = pandas.DataFrame(datas)
     return data
 
 
 # list or tuple data
-def gen_list_data(nb, is_normal=False):
-    vectors = gen_vectors(nb, default_dim, is_normal)
+def gen_list_data(nb):
+    vectors = gen_vectors(nb, default_dim)
     datas = [[i for i in range(nb)], [float(i) for i in range(nb)], vectors]
     return datas
 
 
 def gen_index():
     nlists = [1, 1024, 16384]
     pq_ms = [128, 64, 32, 16, 8, 4]
```

