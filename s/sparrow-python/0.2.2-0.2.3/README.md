# Comparing `tmp/sparrow_python-0.2.2.tar.gz` & `tmp/sparrow_python-0.2.3.tar.gz`

## Comparing `sparrow_python-0.2.2.tar` & `sparrow_python-0.2.3.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/__init__.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/__main__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/constant.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/core.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/version_ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/ai_platform/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/ai_platform/nlp_preprocess.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/__init__.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/common.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/fetch.py
--rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/static/icon.png
--rw-r--r--   0        0        0  1042008 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/static/redoc.standalone.js
--rw-r--r--   0        0        0  1442694 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/static/swagger-ui-bundle.js
--rw-r--r--   0        0        0   150947 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/api/static/swagger-ui.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/async_api/__init__.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/async_api/core.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/async_api/example.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/async_api/example2.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/async_api/异步并发执行.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/core.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/demo.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/downloader.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/git.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/script.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cli/tree.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/color/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/color/color.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/color/constant.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cv/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/cv/utils.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/datasets/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/datasets/fake_data.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/debug/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/decorators/__init__.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/decorators/core.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/distance/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/distance/distance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/doc/__init__.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/docker/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/docker/nvidia_stat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/espec/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/espec/app.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/espec/date.py
--rw-r--r--   0        0        0    14472 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/espec/especial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/extras/__init__.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/extras/packages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/flow/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/flow/executor1/__init__.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/flow/executor1/executor.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/functions/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/functions/bezier.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/functions/core.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/functions/rate_function.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/git/__init__.py
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/git/monitor.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/inspect/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/inspect/core.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/io/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/io/core.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/io/ops.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/jupyter/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/jupyter/utils/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/log/__init__.py
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/log/core.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/log/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/algebra.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/common.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/geometry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/probability.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/math/sampling/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/models/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/__init__.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/client.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/config.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/kill_pid.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/mq/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/mq/client.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/multiprocess/mq/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nlp/__init__.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nlp/deduplicate.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nlp/ngram.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nn/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nn/activations.py
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nn/attention.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nn/losses.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/nn/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/path/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/path/core.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/__init__.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/_measure_time.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/_record_memory.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/_stat_memory.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/stat.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/performance/torch_cuda_memory.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/progress_bar/__init__.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/progress_bar/bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/__init__.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/build-proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/coordinate_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/coordinate_pb2_grpc.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/sparray_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/sparray_pb2_grpc.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/trainstatus_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/proto/python/trainstatus_pb2_grpc.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/string/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/string/color_string.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/string/ops.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/subtitles/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/table_ops/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/table_ops/core.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/__init__.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/core.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/.dockerignore
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/.gitignore
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/REAMEME.md
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/REAMEME_ZH.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/mainxit.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/pyproject.toml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/pytest.ini
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/start_entrypoint.sh
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/Examples/debug.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/conf/logging.yaml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/docker/Dockerfile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/__main__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/api/schemas.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/project_name/api/routes/index.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/template/scaffold/src/tests/conftest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/transform/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/transform/hilbert.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/transform/transform.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/trie/__init__.py
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/trie/trie.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/compress.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/core.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/cursor.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/net.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/web/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/web/share_page.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/sparrow/widgets/__init__.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/LICENSE
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/README.md
--rwxr-xr-x   0        0        0     3634 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 sparrow_python-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0      319 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/__init__.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/__main__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/constant.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/core.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/version_ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/ai_platform/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/ai_platform/nlp_preprocess.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/common.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/fetch.py
+-rw-r--r--   0        0        0    21806 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/static/icon.png
+-rw-r--r--   0        0        0  1042008 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/static/redoc.standalone.js
+-rw-r--r--   0        0        0  1442694 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   150947 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/api/static/swagger-ui.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/async_api/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/async_api/core.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/async_api/example.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/async_api/example2.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/async_api/异步并发执行.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/__init__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/core.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/demo.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/downloader.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/git.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/script.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cli/tree.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/color/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/color/color.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/color/constant.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cv/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/cv/utils.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/datasets/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/datasets/fake_data.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/debug/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/decorators/__init__.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/decorators/core.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/distance/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/distance/distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/doc/__init__.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/docker/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/docker/nvidia_stat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/espec/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/espec/app.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/espec/date.py
+-rw-r--r--   0        0        0    14472 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/espec/especial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/extras/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/extras/packages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/flow/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/flow/executor1/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/flow/executor1/executor.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/functions/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/functions/bezier.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/functions/core.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/functions/rate_function.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/git/__init__.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/git/monitor.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/inspect/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/inspect/core.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/io/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/io/core.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/io/ops.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/jupyter/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/jupyter/utils/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/log/__init__.py
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/log/core.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/log/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/algebra.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/common.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/geometry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/probability.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/math/sampling/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/models/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/__init__.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/client.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/config.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/kill_pid.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/mq/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/mq/client.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/multiprocess/mq/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nlp/__init__.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nlp/deduplicate.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nlp/ngram.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nn/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nn/activations.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nn/attention.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nn/losses.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/nn/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/path/__init__.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/path/core.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/_measure_time.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/_record_memory.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/_stat_memory.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/stat.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/performance/torch_cuda_memory.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/progress_bar/__init__.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/progress_bar/bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/__init__.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/build-proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/coordinate_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/coordinate_pb2_grpc.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/sparray_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/sparray_pb2_grpc.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/trainstatus_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/proto/python/trainstatus_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/string/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/string/color_string.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/string/ops.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/subtitles/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/table_ops/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/table_ops/core.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/__init__.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/core.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/.dockerignore
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/.gitignore
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/REAMEME.md
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/REAMEME_ZH.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/mainxit.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/pyproject.toml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/pytest.ini
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/start_entrypoint.sh
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/gh-release.yml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/Examples/debug.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/conf/logging.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/conf/uvicorn.log.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/docker/Dockerfile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/__main__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/api/schemas.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/api/routes/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/project_name/api/routes/index.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/template/scaffold/src/tests/conftest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/transform/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/transform/hilbert.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/transform/transform.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/trie/__init__.py
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/trie/trie.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/compress.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/core.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/cursor.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/net.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/web/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/web/share_page.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/sparrow/widgets/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/LICENSE
+-rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/README.md
+-rwxr-xr-x   0        0        0     3634 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 sparrow_python-0.2.3/PKG-INFO
```

### Comparing `sparrow_python-0.2.2/sparrow/__main__.py` & `sparrow_python-0.2.3/sparrow/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/constant.py` & `sparrow_python-0.2.3/sparrow/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/core.py` & `sparrow_python-0.2.3/sparrow/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/version_ops.py` & `sparrow_python-0.2.3/sparrow/version_ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/ai_platform/nlp_preprocess.py` & `sparrow_python-0.2.3/sparrow/ai_platform/nlp_preprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import streamlit as st
 import pandas as pd
 import io
 import jionlp as jio
 from sparrow.nlp.deduplicate import EditSimilarity
 
+# streamlit run main.py --server.maxUploadSize=1024
 simi = EditSimilarity()
 
 
 def load_data(file):
     return pd.read_excel(file)
 
 
@@ -33,20 +34,23 @@
     # 获取 Excel 文件中的列名
     columns = df.columns.tolist()
 
     # 让用户选择要清理的多个列
     selected_columns = st.multiselect("选择要清理的列", columns)
     # 选择操作
     operation = st.multiselect("选择操作", [ "去重", "清洗文本", ])
+    dedup_threshold = 0.7
+    if "去重" in operation:
+        dedup_threshold = st.slider("选择去重阈值（越小越严格）", 0.0, 1.0, 0.7)
 
     if st.button('执行'):
         for column in selected_columns:
             if "去重" in operation:
                 simi.load_from_df(df, target_col=column)
-                df = simi.deduplicate()
+                df = simi.deduplicate(threshold=dedup_threshold)
             if "删除文本中的冗余字符" in operation:
                 df[column] = df[column].apply(lambda x: jio.remove_redundant_char(x))
 
             if "清洗文本" in operation:
                 df[column] = df[column].apply(lambda x: jio.clean_text(x))
 
         st.write("清理后的数据预览：")
```

### Comparing `sparrow_python-0.2.2/sparrow/api/common.py` & `sparrow_python-0.2.3/sparrow/api/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/api/fetch.py` & `sparrow_python-0.2.3/sparrow/api/fetch.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/api/static/icon.png` & `sparrow_python-0.2.3/sparrow/api/static/icon.png`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/api/static/redoc.standalone.js` & `sparrow_python-0.2.3/sparrow/api/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/api/static/swagger-ui-bundle.js` & `sparrow_python-0.2.3/sparrow/api/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/api/static/swagger-ui.css` & `sparrow_python-0.2.3/sparrow/api/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/async_api/core.py` & `sparrow_python-0.2.3/sparrow/async_api/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/async_api/example.py` & `sparrow_python-0.2.3/sparrow/async_api/example.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/async_api/example2.py` & `sparrow_python-0.2.3/sparrow/async_api/example2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/async_api/异步并发执行.py` & `sparrow_python-0.2.3/sparrow/async_api/异步并发执行.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/core.py` & `sparrow_python-0.2.3/sparrow/cli/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/demo.py` & `sparrow_python-0.2.3/sparrow/cli/demo.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/downloader.py` & `sparrow_python-0.2.3/sparrow/cli/downloader.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/git.py` & `sparrow_python-0.2.3/sparrow/cli/git.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/script.py` & `sparrow_python-0.2.3/sparrow/cli/script.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cli/tree.py` & `sparrow_python-0.2.3/sparrow/cli/tree.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/color/color.py` & `sparrow_python-0.2.3/sparrow/color/color.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/color/constant.py` & `sparrow_python-0.2.3/sparrow/color/constant.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/cv/utils.py` & `sparrow_python-0.2.3/sparrow/cv/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/datasets/fake_data.py` & `sparrow_python-0.2.3/sparrow/datasets/fake_data.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/decorators/core.py` & `sparrow_python-0.2.3/sparrow/decorators/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/distance/distance.py` & `sparrow_python-0.2.3/sparrow/distance/distance.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/docker/__init__.py` & `sparrow_python-0.2.3/sparrow/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/docker/nvidia_stat.py` & `sparrow_python-0.2.3/sparrow/docker/nvidia_stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/espec/date.py` & `sparrow_python-0.2.3/sparrow/espec/date.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/espec/especial.py` & `sparrow_python-0.2.3/sparrow/espec/especial.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/extras/packages.py` & `sparrow_python-0.2.3/sparrow/extras/packages.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/flow/executor1/executor.py` & `sparrow_python-0.2.3/sparrow/flow/executor1/executor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/functions/core.py` & `sparrow_python-0.2.3/sparrow/functions/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/functions/rate_function.py` & `sparrow_python-0.2.3/sparrow/functions/rate_function.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/functions/utils.py` & `sparrow_python-0.2.3/sparrow/functions/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/git/monitor.py` & `sparrow_python-0.2.3/sparrow/git/monitor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/inspect/core.py` & `sparrow_python-0.2.3/sparrow/inspect/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/io/__init__.py` & `sparrow_python-0.2.3/sparrow/io/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/io/core.py` & `sparrow_python-0.2.3/sparrow/io/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/io/ops.py` & `sparrow_python-0.2.3/sparrow/io/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/jupyter/utils/__init__.py` & `sparrow_python-0.2.3/sparrow/jupyter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/log/core.py` & `sparrow_python-0.2.3/sparrow/log/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/log/setup.py` & `sparrow_python-0.2.3/sparrow/log/setup.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/math/common.py` & `sparrow_python-0.2.3/sparrow/math/common.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/math/geometry.py` & `sparrow_python-0.2.3/sparrow/math/geometry.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/__init__.py` & `sparrow_python-0.2.3/sparrow/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/client.py` & `sparrow_python-0.2.3/sparrow/multiprocess/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/kill_pid.py` & `sparrow_python-0.2.3/sparrow/multiprocess/kill_pid.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/server.py` & `sparrow_python-0.2.3/sparrow/multiprocess/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/mq/client.py` & `sparrow_python-0.2.3/sparrow/multiprocess/mq/client.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/multiprocess/mq/server.py` & `sparrow_python-0.2.3/sparrow/multiprocess/mq/server.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/nlp/deduplicate.py` & `sparrow_python-0.2.3/sparrow/nlp/deduplicate.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/nn/activations.py` & `sparrow_python-0.2.3/sparrow/nn/activations.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/nn/attention.py` & `sparrow_python-0.2.3/sparrow/nn/attention.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/nn/losses.py` & `sparrow_python-0.2.3/sparrow/nn/losses.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/nn/utils.py` & `sparrow_python-0.2.3/sparrow/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/path/core.py` & `sparrow_python-0.2.3/sparrow/path/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/performance/_measure_time.py` & `sparrow_python-0.2.3/sparrow/performance/_measure_time.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/performance/_record_memory.py` & `sparrow_python-0.2.3/sparrow/performance/_record_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/performance/_stat_memory.py` & `sparrow_python-0.2.3/sparrow/performance/_stat_memory.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/performance/stat.py` & `sparrow_python-0.2.3/sparrow/performance/stat.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/progress_bar/bar.py` & `sparrow_python-0.2.3/sparrow/progress_bar/bar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,51 @@
 from rich.live import Live
 from rich.panel import Panel
-from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn
+from rich.progress import Progress, SpinnerColumn, TextColumn, BarColumn, TimeElapsedColumn
 from rich.table import Table
 
 
+class Bar:
+    def __init__(self, total, title='Progress'):
+        """
+        bar = Bar(100, title='Processing').start()
+        for i in range(100):
+            bar(f"Processing item {i}")
+        bar.stop()
+
+        # Using with context manager
+        with Bar(100, title='Processing') as bar:
+            for i in range(100):
+                bar(f"Processing item {i}")
+        """
+        self.progress = Progress(
+            TextColumn("[progress.description]{task.description}"),
+            BarColumn(),
+            TimeElapsedColumn(),
+        )
+        self.task = self.progress.add_task(title, total=total)
+
+    def __call__(self, description, advance=1):
+        self.progress.update(self.task, advance=advance, description=description)
+
+    def start(self):
+        self.progress.start()
+        return self
+
+    def stop(self):
+        self.progress.stop()
+
+    def __enter__(self):
+        self.progress.start()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.progress.stop()
+
+
 class probar:
     def __init__(self, iterable, total_steps=None, title=None):
         """
         """
         self.iterable = iterable
         if total_steps is None:
             try:
@@ -79,14 +117,15 @@
         self._progress.stop()
 
 
 if __name__ == "__main__":
     import time
     import threading
 
+
     # for i in probar(range(100), title="emmm"):
     #     time.sleep(0.1)
 
     def test1():
         def show(progress, task, total: int):
             for i in range(total):
                 progress.update(task, advance=1)
@@ -114,15 +153,14 @@
             while not progress.finished:
                 progress.update(task1, advance=0.5)
                 progress.update(task2, advance=0.3)
                 progress.update(task3, advance=0.9)
                 time.sleep(0.02)
 
 
-
     def test3():
         from time import sleep
 
         job_progress = Progress(
             "{task.description}",
             SpinnerColumn(),
             BarColumn(),
@@ -151,13 +189,18 @@
                     if not job.finished:
                         job_progress.advance(job.id)
 
                 completed = sum(task.completed for task in job_progress.tasks)
                 overall_progress.update(overall_task, completed=completed)
 
 
-
-
-    test1()
+    # test1()
     # test2()
     # test3()
     # test4()
+    with Bar(100, title='Bar') as bar:
+        for i in range(100):
+            bar(f"Processing item {i}")
+            time.sleep(0.01)
+
+    for i in probar(range(100), title="probar"):
+        time.sleep(0.01)
```

### Comparing `sparrow_python-0.2.2/sparrow/proto/build-proto.py` & `sparrow_python-0.2.3/sparrow/proto/build-proto.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/proto/python/coordinate_pb2.py` & `sparrow_python-0.2.3/sparrow/proto/python/coordinate_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/proto/python/sparray_pb2.py` & `sparrow_python-0.2.3/sparrow/proto/python/sparray_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/proto/python/trainstatus_pb2.py` & `sparrow_python-0.2.3/sparrow/proto/python/trainstatus_pb2.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/string/color_string.py` & `sparrow_python-0.2.3/sparrow/string/color_string.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/string/ops.py` & `sparrow_python-0.2.3/sparrow/string/ops.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/subtitles/__init__.py` & `sparrow_python-0.2.3/sparrow/subtitles/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/table_ops/core.py` & `sparrow_python-0.2.3/sparrow/table_ops/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/core.py` & `sparrow_python-0.2.3/sparrow/template/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/core.py` & `sparrow_python-0.2.3/sparrow/template/scaffold/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/.gitignore` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/REAMEME.md` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/REAMEME.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/REAMEME_ZH.md` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/REAMEME_ZH.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/pyproject.toml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/gh-release.yml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/gh-release.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/.github/workflows/python-publish.yml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/conf/logging.yaml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/conf/logging.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/conf/uvicorn.log.yaml` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/conf/uvicorn.log.yaml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/template/scaffold/src/docker/Dockerfile` & `sparrow_python-0.2.3/sparrow/template/scaffold/src/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/transform/transform.py` & `sparrow_python-0.2.3/sparrow/transform/transform.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/trie/trie.py` & `sparrow_python-0.2.3/sparrow/trie/trie.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/utils/compress.py` & `sparrow_python-0.2.3/sparrow/utils/compress.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/utils/core.py` & `sparrow_python-0.2.3/sparrow/utils/core.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/utils/cursor.py` & `sparrow_python-0.2.3/sparrow/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/utils/net.py` & `sparrow_python-0.2.3/sparrow/utils/net.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/web/share_page.py` & `sparrow_python-0.2.3/sparrow/web/share_page.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/sparrow/widgets/__init__.py` & `sparrow_python-0.2.3/sparrow/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/.gitignore` & `sparrow_python-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/LICENSE` & `sparrow_python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/README.md` & `sparrow_python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/pyproject.toml` & `sparrow_python-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparrow_python-0.2.2/PKG-INFO` & `sparrow_python-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sparrow-python
-Version: 0.2.2
+Version: 0.2.3
 Project-URL: homepage, https://github.com/beidongjiedeguang/sparrow
 Project-URL: repository, https://github.com/beidongjiedeguang/sparrow
 Project-URL: documentation, https://github.com/beidongjiedeguang/sparrow#sparrow_tool
 Project-URL: Issues, https://github.com/beidongjiedeguang/sparrow/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/sparrow
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
```

