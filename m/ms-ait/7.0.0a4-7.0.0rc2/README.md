# Comparing `tmp/ms-ait-7.0.0a4.zip` & `tmp/ms-ait-7.0.0rc2.zip`

## zipinfo {}

```diff
@@ -1,429 +1,529 @@
-Zip file size: 501748 bytes, number of entries: 427
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/
--rwxrwxrwx  2.0 unx      298 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/PKG-INFO
--rwxrwxrwx  2.0 unx     4239 b- defN 24-Apr-02 10:25 ms-ait-7.0.0a4/README.md
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/requirements.txt
--rwxrwxrwx  2.0 unx       38 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/setup.cfg
--rwxrwxrwx  2.0 unx     2815 b- defN 24-Apr-07 18:44 ms-ait-7.0.0a4/setup.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/profile/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/tests/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/utils/
--rwxrwxrwx  2.0 unx      600 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/__init__.py
--rwxrwxrwx  2.0 unx     2009 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/
--rwxrwxrwx  2.0 unx       65 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/requirements.txt
--rwxrwxrwx  2.0 unx     1836 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/setup.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/data/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/__init__.py
--rwxrwxrwx  2.0 unx     5943 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/__main__.py
--rwxrwxrwx  2.0 unx      843 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/config.py
--rwxrwxrwx  2.0 unx      936 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/op_info.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/
--rwxrwxrwx  2.0 unx      882 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/const.py
--rwxrwxrwx  2.0 unx     1078 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/log.py
--rwxrwxrwx  2.0 unx     1917 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/utils.py
--rwxrwxrwx  2.0 unx       95 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/__init__.py
--rwxrwxrwx  2.0 unx     1072 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/atc_err.py
--rwxrwxrwx  2.0 unx      730 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/engine.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/framework.py
--rwxrwxrwx  2.0 unx      852 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
--rwxrwxrwx  2.0 unx      692 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/soc_type.py
--rwxrwxrwx  2.0 unx      305 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/
--rwxrwxrwx  2.0 unx     7722 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/analysis.py
--rwxrwxrwx  2.0 unx     4707 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/result.py
--rwxrwxrwx  2.0 unx     1236 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/rule.py
--rwxrwxrwx  2.0 unx       51 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/__init__.py
--rwxrwxrwx  2.0 unx     2495 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/onnx.py
--rwxrwxrwx  2.0 unx       59 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/__init__.py
--rwxrwxrwx  2.0 unx     4428 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/data/opp.py
--rwxrwxrwx  2.0 unx     2212 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/data/op_map.py
--rwxrwxrwx  2.0 unx      683 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/data/__init__.py
--rwxrwxrwx  2.0 unx     2210 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/onnx.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/__init__.py
--rwxrwxrwx  2.0 unx     4426 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/atc.py
--rwxrwxrwx  2.0 unx     5374 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/model.py
--rwxrwxrwx  2.0 unx     5339 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/om.py
--rwxrwxrwx  2.0 unx      750 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/backend/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/infer_analyser/
--rwxrwxrwx  2.0 unx      762 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_infer.py
--rwxrwxrwx  2.0 unx       26 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/requirements.txt
--rwxrwxrwx  2.0 unx     1247 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/setup.py
--rwxrwxrwx  2.0 unx      715 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/__init__.py
--rwxrwxrwx  2.0 unx      752 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/
--rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/interface.py
--rwxrwxrwx  2.0 unx      759 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/log.py
--rwxrwxrwx  2.0 unx     2433 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/recorder.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/__init__.py
--rwxrwxrwx  2.0 unx     3142 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
--rwxrwxrwx  2.0 unx     4606 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
--rwxrwxrwx  2.0 unx     1375 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
--rwxrwxrwx  2.0 unx     3978 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
--rwxrwxrwx  2.0 unx     4244 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/__init__.py
--rwxrwxrwx  2.0 unx     2999 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement.py
--rwxrwxrwx  2.0 unx     1260 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/
--rwxrwxrwx  2.0 unx     4614 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_adapter.py
--rwxrwxrwx  2.0 unx     7151 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_check.py
--rwxrwxrwx  2.0 unx    31048 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/benchmark_process.py
--rwxrwxrwx  2.0 unx    37710 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/interface.py
--rwxrwxrwx  2.0 unx    14389 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/io_oprations.py
--rwxrwxrwx  2.0 unx    10701 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/main_cli.py
--rwxrwxrwx  2.0 unx    10444 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/miscellaneous.py
--rwxrwxrwx  2.0 unx    12042 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/path_security_check.py
--rwxrwxrwx  2.0 unx     3260 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/registry.py
--rwxrwxrwx  2.0 unx     9472 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/summary.py
--rwxrwxrwx  2.0 unx    10122 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/__init__.py
--rwxrwxrwx  2.0 unx     8700 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/__main__.py
--rwxrwxrwx  2.0 unx     3025 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend.py
--rwxrwxrwx  2.0 unx     5400 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
--rwxrwxrwx  2.0 unx      960 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/__init__.py
--rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/backend/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/backend/__init__.py
--rwxrwxrwx  2.0 unx     2843 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/infer_analyser/analyser.py
--rwxrwxrwx  2.0 unx     1680 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/infer_analyser/info_convert_json.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/benchmark/infer_analyser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/convert_scripts/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/
--rwxrwxrwx  2.0 unx       53 b- defN 24-Apr-03 17:28 ms-ait-7.0.0a4/components/convert/requirements.txt
--rwxrwxrwx  2.0 unx     1984 b- defN 24-Apr-03 17:59 ms-ait-7.0.0a4/components/convert/setup.py
--rwxrwxrwx  2.0 unx      711 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-03 17:58 ms-ait-7.0.0a4/components/convert/convert_scripts/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/aie/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/aoe/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/atc/
--rwxrwxrwx  2.0 unx     3463 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/cmd_utils.py
--rwxrwxrwx  2.0 unx      590 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/__init__.py
--rwxrwxrwx  2.0 unx     4184 b- defN 24-Apr-03 17:41 ms-ait-7.0.0a4/components/convert/model_convert/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/convert/model_convert/aie/core/
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aie/__init__.py
--rwxrwxrwx  2.0 unx      775 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/config.py
--rwxrwxrwx  2.0 unx      646 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/__init__.py
--rwxrwxrwx  2.0 unx     2221 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aie/core/convert.py
--rwxrwxrwx  2.0 unx      591 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aie/core/__init__.py
--rwxrwxrwx  2.0 unx     9218 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aoe/aoe_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/aoe/__init__.py
--rwxrwxrwx  2.0 unx    12775 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/atc/atc_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/convert/model_convert/atc/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/
--rwxrwxrwx  2.0 unx     1352 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/
--rwxrwxrwx  2.0 unx      158 b- defN 24-Apr-07 18:32 ms-ait-7.0.0a4/components/debug/surgeon/requirements.txt
--rwxrwxrwx  2.0 unx     2508 b- defN 24-Apr-07 18:40 ms-ait-7.0.0a4/components/debug/surgeon/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/
--rwxrwxrwx  2.0 unx    15728 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/ait_main.py
--rwxrwxrwx  2.0 unx     5587 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/options.py
--rwxrwxrwx  2.0 unx      878 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__init__.py
--rwxrwxrwx  2.0 unx     6305 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__main__.py
--rwxrwxrwx  2.0 unx     6012 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/args_check.py
--rwxrwxrwx  2.0 unx     8604 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/click_utils.py
--rwxrwxrwx  2.0 unx     2307 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/config.py
--rwxrwxrwx  2.0 unx     1633 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/log.py
--rwxrwxrwx  2.0 unx     2265 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/register.py
--rwxrwxrwx  2.0 unx      880 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/singleton.py
--rwxrwxrwx  2.0 unx     5111 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/utils.py
--rwxrwxrwx  2.0 unx     1032 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/__init__.py
--rwxrwxrwx  2.0 unx    11302 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
--rwxrwxrwx  2.0 unx       85 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
--rwxrwxrwx  2.0 unx      784 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
--rwxrwxrwx  2.0 unx    28389 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
--rwxrwxrwx  2.0 unx     8101 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
--rwxrwxrwx  2.0 unx      755 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
--rwxrwxrwx  2.0 unx    28573 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
--rwxrwxrwx  2.0 unx     4880 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
--rwxrwxrwx  2.0 unx      747 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
--rwxrwxrwx  2.0 unx     4582 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
--rwxrwxrwx  2.0 unx     1024 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
--rwxrwxrwx  2.0 unx      736 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
--rwxrwxrwx  2.0 unx     1694 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
--rwxrwxrwx  2.0 unx     2074 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
--rwxrwxrwx  2.0 unx     1390 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
--rwxrwxrwx  2.0 unx     4242 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
--rwxrwxrwx  2.0 unx     1556 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
--rwxrwxrwx  2.0 unx     2736 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
--rwxrwxrwx  2.0 unx      719 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
--rwxrwxrwx  2.0 unx     2234 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
--rwxrwxrwx  2.0 unx      679 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
--rwxrwxrwx  2.0 unx     1342 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     1404 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
--rwxrwxrwx  2.0 unx     1387 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     5279 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/
--rwxrwxrwx  2.0 unx     1565 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
--rwxrwxrwx  2.0 unx    15557 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/matcher.py
--rwxrwxrwx  2.0 unx     7709 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/pattern.py
--rwxrwxrwx  2.0 unx     6596 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/utils.py
--rwxrwxrwx  2.0 unx     2028 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
--rwxrwxrwx  2.0 unx     5589 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
--rwxrwxrwx  2.0 unx     7914 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
--rwxrwxrwx  2.0 unx     6563 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
--rwxrwxrwx  2.0 unx     6124 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
--rwxrwxrwx  2.0 unx    12418 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
--rwxrwxrwx  2.0 unx     5534 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
--rwxrwxrwx  2.0 unx    11185 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
--rwxrwxrwx  2.0 unx    10165 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
--rwxrwxrwx  2.0 unx     6285 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
--rwxrwxrwx  2.0 unx     7235 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
--rwxrwxrwx  2.0 unx     6958 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
--rwxrwxrwx  2.0 unx     3107 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
--rwxrwxrwx  2.0 unx    10959 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
--rwxrwxrwx  2.0 unx    19159 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
--rwxrwxrwx  2.0 unx     5350 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
--rwxrwxrwx  2.0 unx     8097 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
--rwxrwxrwx  2.0 unx    25805 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
--rwxrwxrwx  2.0 unx     1665 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
--rwxrwxrwx  2.0 unx    16842 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
--rwxrwxrwx  2.0 unx     5031 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
--rwxrwxrwx  2.0 unx    13241 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
--rwxrwxrwx  2.0 unx     8003 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
--rwxrwxrwx  2.0 unx     6050 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/inference.py
--rwxrwxrwx  2.0 unx     1559 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/log.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/
--rwxrwxrwx  2.0 unx      122 b- defN 24-Apr-03 10:04 ms-ait-7.0.0a4/components/llm/requirements.txt
--rwxrwxrwx  2.0 unx     2010 b- defN 24-Apr-03 10:06 ms-ait-7.0.0a4/components/llm/setup.py
--rwxrwxrwx  2.0 unx      706 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/transform/
--rwxrwxrwx  2.0 unx      868 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/__init__.py
--rwxrwxrwx  2.0 unx    14363 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/__main__.py
--rwxrwxrwx  2.0 unx     2609 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/constant.py
--rwxrwxrwx  2.0 unx     4826 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/json_fitter.py
--rwxrwxrwx  2.0 unx     1581 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/log.py
--rwxrwxrwx  2.0 unx     3267 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/tool.py
--rwxrwxrwx  2.0 unx     4657 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/common/__init__.py
--rwxrwxrwx  2.0 unx    20620 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/atb_acc_cmp.py
--rwxrwxrwx  2.0 unx     4206 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/cmp_algorithm.py
--rwxrwxrwx  2.0 unx     8458 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/cmp_utils.py
--rwxrwxrwx  2.0 unx      957 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/op_mapping.py
--rwxrwxrwx  2.0 unx    19113 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/torchair_acc_cmp.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/compare/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/
--rwxrwxrwx  2.0 unx     8176 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/initial.py
--rwxrwxrwx  2.0 unx     2406 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/manual_dump.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/__init__.py
--rwxrwxrwx  2.0 unx     2341 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
--rwxrwxrwx  2.0 unx       91 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/__init__.py
--rwxrwxrwx  2.0 unx     3306 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_config.py
--rwxrwxrwx  2.0 unx     6471 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_hook.py
--rwxrwxrwx  2.0 unx     1647 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook.py
--rwxrwxrwx  2.0 unx     3067 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook_ops.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/topo.py
--rwxrwxrwx  2.0 unx      722 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/__init__.py
--rwxrwxrwx  2.0 unx     3074 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/initial.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/
--rwxrwxrwx  2.0 unx     1658 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/case_manager.py
--rwxrwxrwx  2.0 unx    13989 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opchecker.py
--rwxrwxrwx  2.0 unx    12453 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/operation_test.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/__init__.py
--rwxrwxrwx  2.0 unx     2904 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/activation.py
--rwxrwxrwx  2.0 unx      973 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_gather.py
--rwxrwxrwx  2.0 unx     2970 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_reduce.py
--rwxrwxrwx  2.0 unx     1061 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/as_strided.py
--rwxrwxrwx  2.0 unx     1098 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/broadcast.py
--rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/concat.py
--rwxrwxrwx  2.0 unx      967 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/cumsum.py
--rwxrwxrwx  2.0 unx     5404 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/elewise.py
--rwxrwxrwx  2.0 unx     1459 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmax.py
--rwxrwxrwx  2.0 unx     2003 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmaxgrad.py
--rwxrwxrwx  2.0 unx     1144 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fill.py
--rwxrwxrwx  2.0 unx     2535 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/gather.py
--rwxrwxrwx  2.0 unx     1094 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/genattentionmask.py
--rwxrwxrwx  2.0 unx     1045 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/kv_cache.py
--rwxrwxrwx  2.0 unx     4446 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/layer_norm.py
--rwxrwxrwx  2.0 unx     3154 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear.py
--rwxrwxrwx  2.0 unx     4893 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation.py
--rwxrwxrwx  2.0 unx     4915 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation_quant.py
--rwxrwxrwx  2.0 unx     1247 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_parallel.py
--rwxrwxrwx  2.0 unx     1219 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_quant.py
--rwxrwxrwx  2.0 unx     3020 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_sparse.py
--rwxrwxrwx  2.0 unx     2694 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/matmul.py
--rwxrwxrwx  2.0 unx     1650 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/multinomial.py
--rwxrwxrwx  2.0 unx     1440 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/pad.py
--rwxrwxrwx  2.0 unx     1229 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/paged_attention.py
--rwxrwxrwx  2.0 unx     1033 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reduce.py
--rwxrwxrwx  2.0 unx      951 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/repeat.py
--rwxrwxrwx  2.0 unx     1068 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reshape_and_cache.py
--rwxrwxrwx  2.0 unx     2751 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rms_norm.py
--rwxrwxrwx  2.0 unx     6620 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope.py
--rwxrwxrwx  2.0 unx     1725 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope_grad.py
--rwxrwxrwx  2.0 unx     9024 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/self_attention.py
--rwxrwxrwx  2.0 unx     1125 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/set_value.py
--rwxrwxrwx  2.0 unx     1762 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/slice.py
--rwxrwxrwx  2.0 unx      992 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/softmax.py
--rwxrwxrwx  2.0 unx     1031 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/sort.py
--rwxrwxrwx  2.0 unx      994 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/split.py
--rwxrwxrwx  2.0 unx     3220 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/stridebatchmatmul.py
--rwxrwxrwx  2.0 unx     2579 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/topk_topp_sampling.py
--rwxrwxrwx  2.0 unx     4625 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transdata.py
--rwxrwxrwx  2.0 unx      986 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transpose.py
--rwxrwxrwx  2.0 unx     2264 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/unpad.py
--rwxrwxrwx  2.0 unx      972 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/where.py
--rwxrwxrwx  2.0 unx     6493 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/__init__.py
--rwxrwxrwx  2.0 unx    12784 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant.py
--rwxrwxrwx  2.0 unx    22320 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
--rwxrwxrwx  2.0 unx     2542 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/transform/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/llm/ait_llm/transform/__init__.py
--rwxrwxrwx  2.0 unx      720 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/profile/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/tests/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/
--rwxrwxrwx  2.0 unx       89 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/requirements.txt
--rwxrwxrwx  2.0 unx     1765 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/setup.py
--rwxrwxrwx  2.0 unx      714 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/exception/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/report/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/solution/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/
--rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/__init__.py
--rwxrwxrwx  2.0 unx     3444 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/__main__.py
--rwxrwxrwx  2.0 unx    11196 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/common/kit_config.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/common/__init__.py
--rwxrwxrwx  2.0 unx     2257 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/exception/exception_information.py
--rwxrwxrwx  2.0 unx     3419 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/exception/source_scan_exception.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/exception/__init__.py
--rwxrwxrwx  2.0 unx     4850 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/model/model.py
--rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/model/project.py
--rwxrwxrwx  2.0 unx     3765 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/model/seq_project.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/model/__init__.py
--rwxrwxrwx  2.0 unx      983 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/app.py
--rwxrwxrwx  2.0 unx     5752 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/cmdline_input.py
--rwxrwxrwx  2.0 unx     1686 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/custom_input.py
--rwxrwxrwx  2.0 unx     1467 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/input_factory.py
--rwxrwxrwx  2.0 unx     2601 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/porting_input.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/porting/__init__.py
--rwxrwxrwx  2.0 unx     1760 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/report/csv_report.py
--rwxrwxrwx  2.0 unx     1775 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/report/json_report.py
--rwxrwxrwx  2.0 unx     2202 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/report/report.py
--rwxrwxrwx  2.0 unx     1814 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/report/report_factory.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/report/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/
-drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-07 18:45 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/
--rwxrwxrwx  2.0 unx    16004 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_parser.py
--rwxrwxrwx  2.0 unx    25628 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_utils.py
--rwxrwxrwx  2.0 unx    12287 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cmake_scanner.py
--rwxrwxrwx  2.0 unx     1750 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cxx_scanner.py
--rwxrwxrwx  2.0 unx     3043 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/func_parser.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_parser.py
--rwxrwxrwx  2.0 unx     1464 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_scanner.py
--rwxrwxrwx  2.0 unx     1048 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner.py
--rwxrwxrwx  2.0 unx     1930 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_factory.py
--rwxrwxrwx  2.0 unx     1381 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_utils.py
--rwxrwxrwx  2.0 unx     6416 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scan_api.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/__init__.py
--rwxrwxrwx  2.0 unx     5839 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/comment_delete.py
--rwxrwxrwx  2.0 unx     6934 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/file_matrix.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/__init__.py
--rwxrwxrwx  2.0 unx     4525 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/acc_libs.py
--rwxrwxrwx  2.0 unx     1940 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/api_filter.py
--rwxrwxrwx  2.0 unx    10552 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/ast_visitor.py
--rwxrwxrwx  2.0 unx     5793 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_desc.py
--rwxrwxrwx  2.0 unx     8617 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_handler.py
--rwxrwxrwx  2.0 unx     4199 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_matcher.py
--rwxrwxrwx  2.0 unx     5428 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/__init__.py
--rwxrwxrwx  2.0 unx     6677 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/solution/advisor.py
--rwxrwxrwx  2.0 unx     6732 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/solution/seq_advisor.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/solution/__init__.py
--rwxrwxrwx  2.0 unx     4697 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/clang_finder.py
--rwxrwxrwx  2.0 unx     3503 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/excel.py
--rwxrwxrwx  2.0 unx     1919 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/file_locker.py
--rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/io_util.py
--rwxrwxrwx  2.0 unx     1970 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/lib_util.py
--rwxrwxrwx  2.0 unx     2638 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/log_util.py
--rwxrwxrwx  2.0 unx     1851 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/security.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/transplt/app_analyze/utils/__init__.py
--rwxrwxrwx  2.0 unx    12245 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/utils/file_open_check.py
--rwxrwxrwx  2.0 unx     3912 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/utils/parser.py
--rwxrwxrwx  2.0 unx     8748 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/utils/security_check.py
--rwxrwxrwx  2.0 unx      599 b- defN 24-Apr-02 10:06 ms-ait-7.0.0a4/components/utils/__init__.py
--rwxrwxrwx  2.0 unx        1 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       49 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/entry_points.txt
--rwxrwxrwx  2.0 unx      298 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/PKG-INFO
--rwxrwxrwx  2.0 unx       27 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/requires.txt
--rwxrwxrwx  2.0 unx    19417 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/SOURCES.txt
--rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-07 18:45 ms-ait-7.0.0a4/ms_ait.egg-info/top_level.txt
-427 files, 1314606 bytes uncompressed, 410400 bytes compressed:  68.8%
+Zip file size: 662349 bytes, number of entries: 527
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/
+-rwxrwxrwx  2.0 unx      227 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/PKG-INFO
+-rwxrwxrwx  2.0 unx     4239 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/requirements.txt
+-rwxrwxrwx  2.0 unx       38 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/setup.cfg
+-rwxrwxrwx  2.0 unx     1714 b- defN 24-Apr-29 22:45 ms-ait-7.0.0rc2/setup.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/tests/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/utils/
+-rwxrwxrwx  2.0 unx      600 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/__init__.py
+-rwxrwxrwx  2.0 unx     2929 b- defN 24-Apr-29 22:24 ms-ait-7.0.0rc2/components/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/
+-rwxrwxrwx  2.0 unx     5220 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/README.md
+-rwxrwxrwx  2.0 unx       65 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/requirements.txt
+-rwxrwxrwx  2.0 unx     2199 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/analyze/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:42 ms-ait-7.0.0rc2/components/analyze/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__init__.py
+-rwxrwxrwx  2.0 unx      100 b- defN 24-Apr-29 21:54 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__install__.py
+-rwxrwxrwx  2.0 unx     5943 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py
+-rwxrwxrwx  2.0 unx      843 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py
+-rwxrwxrwx  2.0 unx      936 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/
+-rwxrwxrwx  2.0 unx      882 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py
+-rwxrwxrwx  2.0 unx     1078 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py
+-rwxrwxrwx  2.0 unx     1917 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py
+-rwxrwxrwx  2.0 unx       95 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/__init__.py
+-rwxrwxrwx  2.0 unx     1072 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py
+-rwxrwxrwx  2.0 unx      730 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py
+-rwxrwxrwx  2.0 unx      852 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+-rwxrwxrwx  2.0 unx      692 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py
+-rwxrwxrwx  2.0 unx      305 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/
+-rwxrwxrwx  2.0 unx     7722 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py
+-rwxrwxrwx  2.0 unx     4707 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py
+-rwxrwxrwx  2.0 unx     1236 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py
+-rwxrwxrwx  2.0 unx       51 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/__init__.py
+-rwxrwxrwx  2.0 unx     2495 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py
+-rwxrwxrwx  2.0 unx       59 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/__init__.py
+-rwxrwxrwx  2.0 unx     4428 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py
+-rwxrwxrwx  2.0 unx     2212 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py
+-rwxrwxrwx  2.0 unx      683 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py
+-rwxrwxrwx  2.0 unx     2210 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/__init__.py
+-rwxrwxrwx  2.0 unx     4426 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py
+-rwxrwxrwx  2.0 unx     5374 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py
+-rwxrwxrwx  2.0 unx     5339 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py
+-rwxrwxrwx  2.0 unx      750 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/backend/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/
+-rwxrwxrwx  2.0 unx      762 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_infer.py
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/install.sh
+-rwxrwxrwx  2.0 unx    51061 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/README.md
+-rwxrwxrwx  2.0 unx       26 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/requirements.txt
+-rwxrwxrwx  2.0 unx     1779 b- defN 24-Apr-29 21:35 ms-ait-7.0.0rc2/components/benchmark/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 11:18 ms-ait-7.0.0rc2/components/benchmark/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/
+-rwxrwxrwx  2.0 unx     1820 b- defN 24-Apr-29 21:41 ms-ait-7.0.0rc2/components/benchmark/ais_bench/install.sh
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__init__.py
+-rwxrwxrwx  2.0 unx      730 b- defN 24-Apr-29 21:32 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__install__.py
+-rwxrwxrwx  2.0 unx      752 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py
+-rwxrwxrwx  2.0 unx      759 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py
+-rwxrwxrwx  2.0 unx     1591 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/README.md
+-rwxrwxrwx  2.0 unx     2433 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx     3142 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+-rwxrwxrwx  2.0 unx     4606 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+-rwxrwxrwx  2.0 unx     1375 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+-rwxrwxrwx  2.0 unx     3978 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+-rwxrwxrwx  2.0 unx     4244 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+-rwxrwxrwx  2.0 unx     2999 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+-rwxrwxrwx  2.0 unx     1260 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/
+-rwxrwxrwx  2.0 unx     4614 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py
+-rwxrwxrwx  2.0 unx     7151 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py
+-rwxrwxrwx  2.0 unx    31048 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py
+-rwxrwxrwx  2.0 unx    37710 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py
+-rwxrwxrwx  2.0 unx    14389 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py
+-rwxrwxrwx  2.0 unx    10701 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py
+-rwxrwxrwx  2.0 unx    10444 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py
+-rwxrwxrwx  2.0 unx    12042 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py
+-rwxrwxrwx  2.0 unx     3260 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py
+-rwxrwxrwx  2.0 unx     9472 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py
+-rwxrwxrwx  2.0 unx    10122 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__init__.py
+-rwxrwxrwx  2.0 unx     8700 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py
+-rwxrwxrwx  2.0 unx     3025 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py
+-rwxrwxrwx  2.0 unx     5400 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+-rwxrwxrwx  2.0 unx      960 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py
+-rwxrwxrwx  2.0 unx     1587 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/install.sh
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/__init__.py
+-rwxrwxrwx  2.0 unx     2843 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py
+-rwxrwxrwx  2.0 unx     1680 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/
+-rwxrwxrwx  2.0 unx     3162 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/README.md
+-rwxrwxrwx  2.0 unx       35 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/requirements.txt
+-rwxrwxrwx  2.0 unx     2141 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/convert/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:53 ms-ait-7.0.0rc2/components/convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/atc/
+-rwxrwxrwx  2.0 unx     3463 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py
+-rwxrwxrwx  2.0 unx     1520 b- defN 24-Apr-29 21:57 ms-ait-7.0.0rc2/components/convert/model_convert/install.sh
+-rwxrwxrwx  2.0 unx      590 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py
+-rwxrwxrwx  2.0 unx      767 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/convert/model_convert/__install__.py
+-rwxrwxrwx  2.0 unx     3982 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/__init__.py
+-rwxrwxrwx  2.0 unx      775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py
+-rwxrwxrwx  2.0 unx      646 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py
+-rwxrwxrwx  2.0 unx     2221 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py
+-rwxrwxrwx  2.0 unx      591 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py
+-rwxrwxrwx  2.0 unx     9218 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/__init__.py
+-rwxrwxrwx  2.0 unx    12775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/atc/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/
+-rwxrwxrwx  2.0 unx      787 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/
+-rwxrwxrwx  2.0 unx     5324 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/main.py
+-rwxrwxrwx  2.0 unx    11876 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/README.md
+-rwxrwxrwx  2.0 unx      160 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/requirements.txt
+-rwxrwxrwx  2.0 unx     2291 b- defN 24-Apr-29 22:20 ms-ait-7.0.0rc2/components/debug/compare/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 20:05 ms-ait-7.0.0rc2/components/debug/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/
+-rwxrwxrwx  2.0 unx    24580 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/cmp_process.py
+-rwxrwxrwx  2.0 unx     2181 b- defN 24-Apr-29 21:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/install.sh
+-rwxrwxrwx  2.0 unx     5359 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+-rwxrwxrwx  2.0 unx     5175 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf_debug_runner.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__init__.py
+-rwxrwxrwx  2.0 unx     1110 b- defN 24-Apr-29 20:25 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__install__.py
+-rwxrwxrwx  2.0 unx     7990 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__main__.py
+-rwxrwxrwx  2.0 unx     5723 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+-rwxrwxrwx  2.0 unx     2293 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/__init__.py
+-rwxrwxrwx  2.0 unx     3526 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/atc_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/__init__.py
+-rwxrwxrwx  2.0 unx     5651 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/__init__.py
+-rwxrwxrwx  2.0 unx     8737 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/args_check.py
+-rwxrwxrwx  2.0 unx     3621 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/convert.py
+-rwxrwxrwx  2.0 unx     4757 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dump_data.py
+-rwxrwxrwx  2.0 unx     1309 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+-rwxrwxrwx  2.0 unx     6098 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/tf_common.py
+-rwxrwxrwx  2.0 unx    23392 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/__init__.py
+-rwxrwxrwx  2.0 unx    11004 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/analyser.py
+-rwxrwxrwx  2.0 unx    15491 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/net_compare.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/__init__.py
+-rwxrwxrwx  2.0 unx    26609 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/npu_dump_data.py
+-rwxrwxrwx  2.0 unx    14614 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/om_parser.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/__init__.py
+-rwxrwxrwx  2.0 unx     9202 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/custom_op.py
+-rwxrwxrwx  2.0 unx    15216 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/__init__.py
+-rwxrwxrwx  2.0 unx      619 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 20:42 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/__init__.py
+-rwxrwxrwx  2.0 unx     7707 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/single_op.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/__init__.py
+-rwxrwxrwx  2.0 unx    13711 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/tf_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/
+-rwxrwxrwx  2.0 unx    11087 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/README.md
+-rwxrwxrwx  2.0 unx      140 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/requirements.txt
+-rwxrwxrwx  2.0 unx     2785 b- defN 24-Apr-29 22:26 ms-ait-7.0.0rc2/components/debug/surgeon/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/
+-rwxrwxrwx  2.0 unx    15282 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py
+-rwxrwxrwx  2.0 unx     5587 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py
+-rwxrwxrwx  2.0 unx      878 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py
+-rwxrwxrwx  2.0 unx      587 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__install__.py
+-rwxrwxrwx  2.0 unx     6305 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py
+-rwxrwxrwx  2.0 unx     6012 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py
+-rwxrwxrwx  2.0 unx     8604 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py
+-rwxrwxrwx  2.0 unx     2307 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py
+-rwxrwxrwx  2.0 unx     1633 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py
+-rwxrwxrwx  2.0 unx     2265 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py
+-rwxrwxrwx  2.0 unx      880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py
+-rwxrwxrwx  2.0 unx     5111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py
+-rwxrwxrwx  2.0 unx     1032 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py
+-rwxrwxrwx  2.0 unx    11302 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+-rwxrwxrwx  2.0 unx       85 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+-rwxrwxrwx  2.0 unx     2102 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
+-rwxrwxrwx  2.0 unx      784 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+-rwxrwxrwx  2.0 unx    28389 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+-rwxrwxrwx  2.0 unx     8101 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+-rwxrwxrwx  2.0 unx      755 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+-rwxrwxrwx  2.0 unx    28573 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+-rwxrwxrwx  2.0 unx     4880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+-rwxrwxrwx  2.0 unx      747 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+-rwxrwxrwx  2.0 unx     4582 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+-rwxrwxrwx  2.0 unx     5214 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/README.md
+-rwxrwxrwx  2.0 unx     1024 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+-rwxrwxrwx  2.0 unx      736 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+-rwxrwxrwx  2.0 unx     1694 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+-rwxrwxrwx  2.0 unx     2074 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+-rwxrwxrwx  2.0 unx     1390 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+-rwxrwxrwx  2.0 unx     4242 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+-rwxrwxrwx  2.0 unx     1556 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+-rwxrwxrwx  2.0 unx     2736 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+-rwxrwxrwx  2.0 unx      719 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+-rwxrwxrwx  2.0 unx     2234 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+-rwxrwxrwx  2.0 unx      679 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+-rwxrwxrwx  2.0 unx     1342 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     1404 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+-rwxrwxrwx  2.0 unx     1387 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     5279 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+-rwxrwxrwx  2.0 unx     1565 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+-rwxrwxrwx  2.0 unx    15557 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+-rwxrwxrwx  2.0 unx     7709 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+-rwxrwxrwx  2.0 unx     6596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py
+-rwxrwxrwx  2.0 unx     2028 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+-rwxrwxrwx  2.0 unx     5589 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+-rwxrwxrwx  2.0 unx     7914 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+-rwxrwxrwx  2.0 unx     6563 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+-rwxrwxrwx  2.0 unx     6124 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+-rwxrwxrwx  2.0 unx    12418 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+-rwxrwxrwx  2.0 unx     5534 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+-rwxrwxrwx  2.0 unx    11185 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+-rwxrwxrwx  2.0 unx    10165 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+-rwxrwxrwx  2.0 unx     6285 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+-rwxrwxrwx  2.0 unx     7235 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+-rwxrwxrwx  2.0 unx     6958 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+-rwxrwxrwx  2.0 unx     3107 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+-rwxrwxrwx  2.0 unx    10959 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+-rwxrwxrwx  2.0 unx    19159 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+-rwxrwxrwx  2.0 unx     5350 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+-rwxrwxrwx  2.0 unx     8097 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+-rwxrwxrwx  2.0 unx    25805 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+-rwxrwxrwx  2.0 unx     1665 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+-rwxrwxrwx  2.0 unx    16842 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+-rwxrwxrwx  2.0 unx     5031 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+-rwxrwxrwx  2.0 unx    13241 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+-rwxrwxrwx  2.0 unx     8003 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+-rwxrwxrwx  2.0 unx     6050 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py
+-rwxrwxrwx  2.0 unx     1559 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py
+-rwxrwxrwx  2.0 unx      505 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/
+-rwxrwxrwx  2.0 unx     9351 b- defN 24-Apr-24 19:12 ms-ait-7.0.0rc2/components/llm/README.md
+-rwxrwxrwx  2.0 unx      108 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/requirements.txt
+-rwxrwxrwx  2.0 unx     2353 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/llm/setup.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-29 10:34 ms-ait-7.0.0rc2/components/llm/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/
+-rwxrwxrwx  2.0 unx      904 b- defN 24-Apr-29 22:07 ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh
+-rwxrwxrwx  2.0 unx      920 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py
+-rwxrwxrwx  2.0 unx      789 b- defN 24-Apr-29 22:45 ms-ait-7.0.0rc2/components/llm/ait_llm/__install__.py
+-rwxrwxrwx  2.0 unx    13398 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py
+-rwxrwxrwx  2.0 unx     2609 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py
+-rwxrwxrwx  2.0 unx     4826 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py
+-rwxrwxrwx  2.0 unx     1581 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py
+-rwxrwxrwx  2.0 unx     3267 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py
+-rwxrwxrwx  2.0 unx     4657 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py
+-rwxrwxrwx  2.0 unx     8522 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/common/validate.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/__init__.py
+-rwxrwxrwx  2.0 unx    22815 b- defN 24-Apr-25 16:27 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py
+-rwxrwxrwx  2.0 unx     3429 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_algorithm.py
+-rwxrwxrwx  2.0 unx     8458 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py
+-rwxrwxrwx  2.0 unx      957 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py
+-rwxrwxrwx  2.0 unx    19113 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/
+-rwxrwxrwx  2.0 unx     8268 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py
+-rwxrwxrwx  2.0 unx     2576 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/__init__.py
+-rwxrwxrwx  2.0 unx     2445 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+-rwxrwxrwx  2.0 unx       91 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/__init__.py
+-rwxrwxrwx  2.0 unx     3413 b- defN 24-Apr-24 19:12 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py
+-rwxrwxrwx  2.0 unx     7648 b- defN 24-Apr-25 16:29 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+-rwxrwxrwx  2.0 unx     1647 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py
+-rwxrwxrwx  2.0 unx     3067 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py
+-rwxrwxrwx  2.0 unx      722 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py
+-rwxrwxrwx  2.0 unx     4755 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/process.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/__init__.py
+-rwxrwxrwx  2.0 unx     5241 b- defN 24-Apr-25 15:33 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/case_filter.py
+-rwxrwxrwx  2.0 unx    10031 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/metrics.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/
+-rwxrwxrwx  2.0 unx     1645 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py
+-rwxrwxrwx  2.0 unx    15437 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py
+-rwxrwxrwx  2.0 unx    10880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/__init__.py
+-rwxrwxrwx  2.0 unx    29744 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+-rwxrwxrwx  2.0 unx     1354 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 22:29 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/__init__.py
+-rwxrwxrwx  2.0 unx     2904 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/activation.py
+-rwxrwxrwx  2.0 unx      973 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py
+-rwxrwxrwx  2.0 unx     2970 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py
+-rwxrwxrwx  2.0 unx     1061 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py
+-rwxrwxrwx  2.0 unx     1098 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py
+-rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py
+-rwxrwxrwx  2.0 unx      967 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py
+-rwxrwxrwx  2.0 unx     5404 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/elewise.py
+-rwxrwxrwx  2.0 unx     1459 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+-rwxrwxrwx  2.0 unx     2003 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+-rwxrwxrwx  2.0 unx     1144 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py
+-rwxrwxrwx  2.0 unx     2535 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py
+-rwxrwxrwx  2.0 unx     1094 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+-rwxrwxrwx  2.0 unx     1045 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py
+-rwxrwxrwx  2.0 unx     4446 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py
+-rwxrwxrwx  2.0 unx     2687 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py
+-rwxrwxrwx  2.0 unx     1247 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+-rwxrwxrwx  2.0 unx     3020 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+-rwxrwxrwx  2.0 unx     2694 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py
+-rwxrwxrwx  2.0 unx     1650 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py
+-rwxrwxrwx  2.0 unx     1440 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py
+-rwxrwxrwx  2.0 unx     1229 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/paged_attention.py
+-rwxrwxrwx  2.0 unx     1033 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py
+-rwxrwxrwx  2.0 unx      951 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py
+-rwxrwxrwx  2.0 unx     1068 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+-rwxrwxrwx  2.0 unx     2751 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rms_norm.py
+-rwxrwxrwx  2.0 unx     6620 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py
+-rwxrwxrwx  2.0 unx     1725 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py
+-rwxrwxrwx  2.0 unx     9619 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py
+-rwxrwxrwx  2.0 unx     1125 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py
+-rwxrwxrwx  2.0 unx     1762 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py
+-rwxrwxrwx  2.0 unx      992 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py
+-rwxrwxrwx  2.0 unx     1031 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py
+-rwxrwxrwx  2.0 unx      994 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py
+-rwxrwxrwx  2.0 unx     3220 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+-rwxrwxrwx  2.0 unx     2579 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+-rwxrwxrwx  2.0 unx     4625 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py
+-rwxrwxrwx  2.0 unx      986 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py
+-rwxrwxrwx  2.0 unx     2264 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py
+-rwxrwxrwx  2.0 unx      972 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py
+-rwxrwxrwx  2.0 unx     5680 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py
+-rwxrwxrwx  2.0 unx    12784 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py
+-rwxrwxrwx  2.0 unx    22320 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+-rwxrwxrwx  2.0 unx     2542 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/msprof/
+-rwxrwxrwx  2.0 unx      602 b- defN 24-Apr-29 11:18 ms-ait-7.0.0rc2/components/profile/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/install.sh
+-rwxrwxrwx  2.0 unx     5011 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/README.md
+-rwxrwxrwx  2.0 unx       10 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/requirements.txt
+-rwxrwxrwx  2.0 unx     1552 b- defN 24-Apr-29 22:24 ms-ait-7.0.0rc2/components/profile/msprof/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 22:34 ms-ait-7.0.0rc2/components/profile/msprof/__init__.py
+-rwxrwxrwx  2.0 unx     4154 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/api.py
+-rwxrwxrwx  2.0 unx     1277 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/args_adapter.py
+-rwxrwxrwx  2.0 unx     4565 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/main_cli.py
+-rwxrwxrwx  2.0 unx     4314 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/msprof_process.py
+-rwxrwxrwx  2.0 unx      760 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__init__.py
+-rwxrwxrwx  2.0 unx       99 b- defN 24-Apr-29 22:05 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__install__.py
+-rwxrwxrwx  2.0 unx     4513 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__main__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/tests/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/install.bat
+-rwxrwxrwx  2.0 unx     4111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/install.sh
+-rwxrwxrwx  2.0 unx    23645 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/README.md
+-rwxrwxrwx  2.0 unx       89 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/requirements.txt
+-rwxrwxrwx  2.0 unx     2210 b- defN 24-Apr-29 22:38 ms-ait-7.0.0rc2/components/transplt/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:37 ms-ait-7.0.0rc2/components/transplt/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/install.bat
+-rwxrwxrwx  2.0 unx     4111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/install.sh
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/__init__.py
+-rwxrwxrwx  2.0 unx      839 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/transplt/app_analyze/__install__.py
+-rwxrwxrwx  2.0 unx     3444 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py
+-rwxrwxrwx  2.0 unx    11196 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py
+-rwxrwxrwx  2.0 unx     2257 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py
+-rwxrwxrwx  2.0 unx     3419 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py
+-rwxrwxrwx  2.0 unx     4850 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py
+-rwxrwxrwx  2.0 unx     3765 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py
+-rwxrwxrwx  2.0 unx      983 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py
+-rwxrwxrwx  2.0 unx     5752 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py
+-rwxrwxrwx  2.0 unx     1686 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py
+-rwxrwxrwx  2.0 unx     1467 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py
+-rwxrwxrwx  2.0 unx     2601 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py
+-rwxrwxrwx  2.0 unx     1760 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py
+-rwxrwxrwx  2.0 unx     1775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py
+-rwxrwxrwx  2.0 unx     2202 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py
+-rwxrwxrwx  2.0 unx     1814 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/
+-rwxrwxrwx  2.0 unx    16004 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py
+-rwxrwxrwx  2.0 unx    25628 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py
+-rwxrwxrwx  2.0 unx    12287 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py
+-rwxrwxrwx  2.0 unx     1750 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py
+-rwxrwxrwx  2.0 unx     3043 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py
+-rwxrwxrwx  2.0 unx     1464 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py
+-rwxrwxrwx  2.0 unx     1048 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py
+-rwxrwxrwx  2.0 unx     1930 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py
+-rwxrwxrwx  2.0 unx     1381 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py
+-rwxrwxrwx  2.0 unx     6416 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py
+-rwxrwxrwx  2.0 unx     5839 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py
+-rwxrwxrwx  2.0 unx     6934 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/__init__.py
+-rwxrwxrwx  2.0 unx     4525 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py
+-rwxrwxrwx  2.0 unx     1940 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py
+-rwxrwxrwx  2.0 unx    10552 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+-rwxrwxrwx  2.0 unx     5793 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py
+-rwxrwxrwx  2.0 unx     8617 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py
+-rwxrwxrwx  2.0 unx     4199 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+-rwxrwxrwx  2.0 unx     5428 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/__init__.py
+-rwxrwxrwx  2.0 unx     6677 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py
+-rwxrwxrwx  2.0 unx     6732 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py
+-rwxrwxrwx  2.0 unx     4697 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py
+-rwxrwxrwx  2.0 unx     3503 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py
+-rwxrwxrwx  2.0 unx     1919 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py
+-rwxrwxrwx  2.0 unx     1970 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py
+-rwxrwxrwx  2.0 unx     2638 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py
+-rwxrwxrwx  2.0 unx     1851 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py
+-rwxrwxrwx  2.0 unx    12245 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/file_open_check.py
+-rwxrwxrwx  2.0 unx     4614 b- defN 24-Apr-29 22:32 ms-ait-7.0.0rc2/components/utils/install.py
+-rwxrwxrwx  2.0 unx     3987 b- defN 24-Apr-29 17:07 ms-ait-7.0.0rc2/components/utils/parser.py
+-rwxrwxrwx  2.0 unx     8748 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/security_check.py
+-rwxrwxrwx  2.0 unx      279 b- defN 24-Apr-29 15:52 ms-ait-7.0.0rc2/components/utils/util.py
+-rwxrwxrwx  2.0 unx      599 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/__init__.py
+-rwxrwxrwx  2.0 unx        1 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      147 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/entry_points.txt
+-rwxrwxrwx  2.0 unx      227 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/PKG-INFO
+-rwxrwxrwx  2.0 unx    23140 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt
+-rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/top_level.txt
+527 files, 1797886 bytes uncompressed, 550759 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,1282 +1,1582 @@
-Filename: ms-ait-7.0.0a4/
+Filename: ms-ait-7.0.0rc2/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/
+Filename: ms-ait-7.0.0rc2/components/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/PKG-INFO
+Filename: ms-ait-7.0.0rc2/PKG-INFO
 Comment: 
 
-Filename: ms-ait-7.0.0a4/README.md
+Filename: ms-ait-7.0.0rc2/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/requirements.txt
+Filename: ms-ait-7.0.0rc2/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/setup.cfg
+Filename: ms-ait-7.0.0rc2/setup.cfg
 Comment: 
 
-Filename: ms-ait-7.0.0a4/setup.py
+Filename: ms-ait-7.0.0rc2/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/
+Filename: ms-ait-7.0.0rc2/components/analyze/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/
+Filename: ms-ait-7.0.0rc2/components/benchmark/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/
+Filename: ms-ait-7.0.0rc2/components/convert/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/
+Filename: ms-ait-7.0.0rc2/components/debug/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/
+Filename: ms-ait-7.0.0rc2/components/llm/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/profile/
+Filename: ms-ait-7.0.0rc2/components/profile/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/tests/
+Filename: ms-ait-7.0.0rc2/components/tests/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/
+Filename: ms-ait-7.0.0rc2/components/transplt/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/utils/
+Filename: ms-ait-7.0.0rc2/components/utils/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/__init__.py
+Filename: ms-ait-7.0.0rc2/components/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/__main__.py
+Filename: ms-ait-7.0.0rc2/components/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/analyze/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/setup.py
+Filename: ms-ait-7.0.0rc2/components/analyze/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/
+Filename: ms-ait-7.0.0rc2/components/analyze/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/data/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/__main__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/config.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/op_info.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/const.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/log.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/atc_err.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/engine.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/framework.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/soc_type.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/analysis.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/result.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/rule.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/onnx.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/data/opp.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/data/op_map.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/data/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/onnx.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/atc.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/model.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/om.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/backend/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/infer_analyser/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_infer.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/setup.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_infer.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/
+Filename: ms-ait-7.0.0rc2/components/benchmark/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/
+Filename: ms-ait-7.0.0rc2/components/benchmark/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/__main__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/interface.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/log.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/recorder.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_adapter.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_check.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/benchmark_process.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/interface.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/io_oprations.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/main_cli.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/miscellaneous.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/path_security_check.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/registry.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/summary.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/utils.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/__main__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/backend/setup.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/backend/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/infer_analyser/analyser.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/infer_analyser/info_convert_json.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/benchmark/infer_analyser/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/convert_scripts/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/setup.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/convert_scripts/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aoe/
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/atc/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/cmd_utils.py
+Filename: ms-ait-7.0.0rc2/components/convert/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/__main__.py
+Filename: ms-ait-7.0.0rc2/components/convert/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/
+Filename: ms-ait-7.0.0rc2/components/convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/core/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/config.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/core/convert.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aie/core/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aoe/aoe_args_map.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/aoe/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/atc/atc_args_map.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/convert/model_convert/atc/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/setup.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/
+Filename: ms-ait-7.0.0rc2/components/debug/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/ait_main.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/options.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/main.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__main__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/args_check.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/click_utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/config.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/log.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/register.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/singleton.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/cmp_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf_debug_runner.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/atc_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/tf_common.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/net_compare.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/npu_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/om_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/custom_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/single_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/tf_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/inference.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/log.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/setup.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/transform/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/__main__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/constant.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/json_fitter.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/log.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/tool.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/atb_acc_cmp.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/cmp_algorithm.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/cmp_utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/op_mapping.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/torchair_acc_cmp.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/compare/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/initial.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/manual_dump.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_config.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/topo.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/initial.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/errcheck/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/case_manager.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opchecker.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/operation_test.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/activation.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_gather.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_reduce.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/as_strided.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/broadcast.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/concat.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/cumsum.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/elewise.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmax.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmaxgrad.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fill.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/gather.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/genattentionmask.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/kv_cache.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/layer_norm.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation_quant.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_parallel.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_quant.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_sparse.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/matmul.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/multinomial.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/pad.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/paged_attention.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reduce.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/repeat.py
+Filename: ms-ait-7.0.0rc2/components/llm/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reshape_and_cache.py
+Filename: ms-ait-7.0.0rc2/components/llm/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rms_norm.py
+Filename: ms-ait-7.0.0rc2/components/llm/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope.py
+Filename: ms-ait-7.0.0rc2/components/llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope_grad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/self_attention.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/set_value.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/slice.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/softmax.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/sort.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/split.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/stridebatchmatmul.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/topk_topp_sampling.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transdata.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transpose.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/unpad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/where.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/transform/utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/validate.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/llm/ait_llm/transform/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/profile/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/tests/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_algorithm.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/setup.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/common/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/exception/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/model/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/solution/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/__main__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/common/kit_config.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/exception/exception_information.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/exception/source_scan_exception.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/process.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/exception/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/model/model.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/case_filter.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/model/project.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/metrics.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/model/seq_project.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/model/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/app.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/cmdline_input.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/custom_input.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/input_factory.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/porting_input.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/porting/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/csv_report.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/json_report.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/report.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/activation.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/report_factory.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/report/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_parser.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cmake_scanner.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/elewise.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cxx_scanner.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/func_parser.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_parser.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_scanner.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_factory.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scan_api.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/comment_delete.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/file_matrix.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/acc_libs.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/api_filter.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/paged_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_desc.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_handler.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rms_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/solution/advisor.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/solution/seq_advisor.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/solution/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/clang_finder.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/excel.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/file_locker.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/io_util.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/lib_util.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/log_util.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/security.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/transplt/app_analyze/utils/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/utils/file_open_check.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/utils/parser.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/utils/security_check.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/components/utils/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/dependency_links.txt
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/entry_points.txt
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/PKG-INFO
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/requires.txt
+Filename: ms-ait-7.0.0rc2/components/profile/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/SOURCES.txt
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/
 Comment: 
 
-Filename: ms-ait-7.0.0a4/ms_ait.egg-info/top_level.txt
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/install.sh
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/README.md
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/requirements.txt
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/setup.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/api.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/args_adapter.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/main_cli.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/msprof_process.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/utils.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__install__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__main__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/tests/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/install.bat
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/install.sh
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/README.md
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/requirements.txt
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/setup.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/install.bat
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/install.sh
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__install__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/file_open_check.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/install.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/parser.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/security_check.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/util.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/components/utils/__init__.py
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/dependency_links.txt
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/entry_points.txt
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/PKG-INFO
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt
+Comment: 
+
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `ms-ait-7.0.0a4/README.md` & `ms-ait-7.0.0rc2/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/__init__.py` & `ms-ait-7.0.0rc2/components/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/__main__.py` & `ms-ait-7.0.0rc2/components/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,42 +10,92 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 
-from components.llm import llm_cmd
-from components.debug import debug_cmd
-from components.profile import profile_cmd
-from components.transplt import transplt_cmd
-from components.benchmark import benchmark_cmd
-from components.analyze import analyze_cmd
-from components.convert import convert_cmd
-from components.utils.parser import register_parser, AIT_FAQ_HOME, MIND_STUDIO_LOGO
+from components.utils.parser import BaseCommand, AIT_FAQ_HOME, MIND_STUDIO_LOGO
 from components.utils.file_open_check import UmaskWrapper
+from components.utils.install import check_tools, build_extra, install_tools
+
+
+class AitCommand(BaseCommand):
+    def add_arguments(self, parser):
+        all_sub_tools = [
+            'ait-llm',
+            'ait-compare',
+            'ait-surgeon',
+            'ait-analyze',
+            'ait-transplt',
+            'ait-convert',
+            'ait-msprof',
+            'ait-benchmark',
+            'all',
+        ]
+        parser.add_argument(
+            "--install",
+            nargs="+",
+            choices=all_sub_tools,
+            default=None,
+            help="install ait tools",
+        )
+
+        parser.add_argument(
+            "--check",
+            nargs="+",
+            choices=all_sub_tools,
+            default=None,
+            help="check ait tools status ",
+        )
+
+        parser.add_argument(
+            "--build-extra",
+            dest='build_extra',
+            type=str,
+            default=None,
+            help="install ait tools extra",
+        )
+
+    def handle(self, args):
+        handled = False
+        if args.install:
+            handled = True
+            install_tools(args.install)
+
+        if args.build_extra:
+            handled = True
+            build_extra(args.build_extra)
+
+        if args.check:
+            handled = True
+            check_tools(args.check)
+
+        if not handled:
+            return super().handle(args)
 
 
 def main():
-    subcommands = [debug_cmd, profile_cmd, transplt_cmd, benchmark_cmd, \
-                   analyze_cmd, convert_cmd, llm_cmd]
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=f"ait(Ascend Inference Tools), {MIND_STUDIO_LOGO}.\n"
         "Providing one-site debugging and optimization toolkit for inference on Ascend Devices.\n"
         f"For any issue, refer FAQ first: {AIT_FAQ_HOME}",
     )
-    register_parser(parser, subcommands)
-    parser.set_defaults(print_help=parser.print_help)
+
+    cmd = AitCommand("ait", None, "ait_sub_task")
+    cmd.register_parser(parser)
+
     args = parser.parse_args()
 
     if hasattr(args, 'handle'):
         with UmaskWrapper():
             try:
                 args.handle(args)
             except Exception as err:
-                raise Exception(f"[ERROR] Refer FAQ if a known issue: {AIT_FAQ_HOME}") from err
-    elif hasattr(args, "print_help"):
-        args.print_help()
+                raise Exception(
+                    f"[ERROR] Refer FAQ if a known issue: {AIT_FAQ_HOME}"
+                ) from err
+
 
 if __name__ == "__main__":
-    main()
+    main()
```

## Comparing `ms-ait-7.0.0a4/components/analyze/setup.py` & `ms-ait-7.0.0rc2/components/debug/compare/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+# http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from setuptools import setup, find_packages  # type: ignore
 
-
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
+debug_sub_tasks = [{
+    "name": "compare",
+    "help_info": "one-click network-wide accuracy analysis of golden models.",
+    "module": "msquickcmp.__main__",
+    "attr": "get_cmd_instance"
+}]
+
+debug_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in debug_sub_tasks]
+
 setup(
-    name='analyze_tool',
-    version='0.1.0',
-    description='inference analyze tool',
+    name='ait-compare',
+    version='7.0.0c2',
+    description='This tool enables one-click network-wide accuracy analysis of gold model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://gitee.com/ascend/ait',
+    url='https://gitee.com/ascend/ait/tree/master/ait/components/debug/compare',
     packages=find_packages(),
-    package_data={
-        'model_evaluation': ['data/op_map/*.yaml']
-    },
+    package_data={'': ['LICENSE', 'install.sh', 'libsaveom.so', '*.cpp']},
     license='Apache-2.0',
-    keywords='analyze tool',
+    keywords='compare',
     install_requires=required,
     classifiers=[
         'Development Status :: Alpha',
         'Intended Audience :: Developers',
         'License :: Apache-2.0 Software License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
     ],
     python_requires='>=3.7',
     entry_points={
-        'analyze_sub_task': ['model=model_evaluation.__main__:get_cmd_instance'],
+        'debug_sub_task': debug_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-compare=msquickcmp.__install__:CompareInstall'],
     },
 )
```

## Comparing `ms-ait-7.0.0a4/components/analyze/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+#!/usr/bin/env bash
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+CURRENT_DIR=$(dirname $(readlink -f $0))
+
 
-from components.utils.parser import load_command_instance
+build_opchecker_so() {
+    echo ""
+    echo "Try building libatb_speed_torch.so for ait llm. If not using opecheck, ignore errors if any"
+    cd ${CURRENT_DIR}/opcheck/atb_operators
+    bash build.sh
+    cd -
+    echo ""
+}
 
-analyze_cmd = load_command_instance('analyze_sub_task')
+build_opchecker_so
```

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/__main__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/config.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/op_info.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/bean/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/const.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/log.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/utils.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/atc_err.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/engine.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/framework.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/onnx_checker_err.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/common/enum/soc_type.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/core/analysis.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/core/result.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/core/rule.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/core/checker/onnx.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/data/opp.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/data/op_map.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/data/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/graph/onnx.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/atc.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/model.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/om.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/analyze/model_evaluation/parser/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_infer.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_infer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/setup.py` & `ms-ait-7.0.0rc2/components/benchmark/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,34 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
+ait_sub_tasks = [{
+    "name": "benchmark",
+    "help_info": "benchmark tool to get performance data including latency and throughput",
+    "module": "ais_bench.infer.main_cli",
+    "attr": "get_cmd_instance"
+}]
+
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
+
 setup(
-    name='ais_bench',
-    version='0.0.2',
-    description='ais_bench tool',
+    name='ait-benchmark', # 不与ais_bench冲突
+    version='7.0.0c2',
+    description='ais_bench tool(ait)',
     long_description=long_description,
     url='ais_bench url',
     packages=find_packages(),
+    package_data={'': ['LICENSE', 'README.md', 'requirements.txt', 'install.bat', 'install.sh', '*.cpp', '*.h']},
     include_package_data=True,
     keywords='ais_bench tool',
     install_requires=required,
     python_requires='>=3.7',
     entry_points={
-        'benchmark_sub_task': ['benchmark=ais_bench.infer.main_cli:get_cmd_instance'],
+        'ait_sub_task': ait_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-benchmark=ais_bench.__install__:BenchmarkInstall'],
     },
 
 )
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ms-ait-7.0.0a4/components/benchmark/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from components.utils.parser import load_command_instance
-
-benchmark_cmd = load_command_instance('benchmark_sub_task')
+# Copyright (c) 2024 Huawei Technologies Co., Ltd.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from ait_llm.dump.torch_dump.dump_config import DumpConfig
+from ait_llm.dump.torch_dump.hook import register_hook
```

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/__main__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/interface.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/log.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/recorder.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_adapter.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/args_check.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/benchmark_process.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/interface.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/io_oprations.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/main_cli.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/miscellaneous.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/path_security_check.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/registry.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/summary.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/utils.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/__main__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/backend_trtexec.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/ais_bench/infer/backends/__init__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/backend/setup.py` & `ms-ait-7.0.0rc2/components/benchmark/backend/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/infer_analyser/analyser.py` & `ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/benchmark/infer_analyser/info_convert_json.py` & `ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/setup.py` & `ms-ait-7.0.0rc2/components/llm/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,50 +8,59 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from setuptools import setup, find_packages  # type: ignore
-from distutils.command.install import install
+import subprocess
+import site
+import os
+
+from setuptools import setup, find_packages
 
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
+opchecker_lib_src = []
+for root, dirs, files in os.walk('components/llm/ait_llm/opcheck/test_framework/'):
+    opchecker_lib_src.append((os.path.join("/", root), [os.path.join(root, f) for f in files]))
+
+ait_sub_tasks = [{
+    "name": "llm",
+    "help_info": "Large Language Model(llm) Debugger Tools.",
+    "module": "ait_llm.__main__",
+    "attr": "get_cmd_instance"
+}]
 
-class convert_install(install):
-    def run(self):
-        super().run()
-        import os
-        from subprocess import call
-
-        call(os.path.join(os.path.dirname(os.path.realpath(__file__)), "convert_scripts", "build.sh"))
-
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
-    name='convert_tool',
-    cmdclass={"install": convert_install},
-    version='7.0.0a1',
-    description='model convert tool',
-    url='https://gitee.com/ascend/ait',
-    packages=find_packages(),
+    name='ait-llm',
+    version='7.0.0c2',
+    description='Debug tools for large language model(llm)',
+    url='https://gitee.com/ascend/ait/ait/components/llm',
+    packages=find_packages(),    
+    package_data={'': ['*.sh', '*.cpp', '*.h', 'CMakeLists.txt']},
     license='Apache-2.0',
-    keywords='convert tool',
+    keywords='ait_llm',
     install_requires=required,
     classifiers=[
         'Development Status :: Alpha',
         'Intended Audience :: Developers',
         'License :: Apache-2.0 Software License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
-        'Topic :: Software Development',
+        'Topic :: Software Development'
     ],
+    data_dir=f"{site.getsitepackages()[0]}",
+    data_files=opchecker_lib_src,
+    include_package_data=True,
     python_requires='>=3.7',
     entry_points={
-        'convert_sub_task': ['convert=model_convert.__main__:get_cmd_instance'],
-        'console_scripts': ['ait-build-aie=model_convert.__main__:build_aie'],
+        'ait_sub_task': ait_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-llm=ait_llm.__install__:LlmInstall'],
     },
-)
+)
```

## Comparing `ms-ait-7.0.0a4/components/convert/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from components.utils.parser import load_command_instance
+from dataclasses import dataclass
+
+from typing import Any
+
 
-convert_cmd = load_command_instance('convert_sub_task')
+@dataclass
+class InferenceResult:
+    label: Any = None
+    data: Any = None
```

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/cmd_utils.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/__main__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,14 @@
     return ConvertConfig(
         model=model,
         output=output,
         soc_version=soc_version
     )
 
 
-class ConvertCommand(BaseCommand):
-    pass
-
-
 class ModelConvertCommand(BaseCommand):
     def __init__(self, backend, *args, **kwargs):
         super(ModelConvertCommand, self).__init__(*args, **kwargs)
         self.conf_args = None
         self.backend = backend
 
     def add_arguments(self, parser, **kwargs):
@@ -92,20 +88,14 @@
         logger.info('convert model finished.')
 
 
 def get_cmd_instance():
     aie_cmd = AieCommand("aie", help_info="Convert onnx to om by aie.")
     atc_cmd = ModelConvertCommand(name="atc", help_info="Convert onnx to om by atc.", backend="atc")
     aoe_cmd = ModelConvertCommand(name="aoe", help_info="Convert onnx to om by aoe.", backend="aoe")
-    convert_cmd = ConvertCommand(
+    convert_cmd = BaseCommand(
         name="convert",
         help_info="convert tool converts the model from ONNX, TensorFlow, Caffe and MindSpore to OM. \
                    It supports atc, aoe and aie.",
         children=[atc_cmd, aoe_cmd, aie_cmd]
     )
     return convert_cmd
-
-def build_aie():
-    import os
-    from subprocess import call
-
-    call(os.path.join(os.path.dirname(os.path.realpath(__file__)), "build.sh"))
```

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/config.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/aie/bean/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/aie/core/convert.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/aie/core/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/aoe/aoe_args_map.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/convert/model_convert/atc/atc_args_map.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/setup.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,54 +15,62 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
+debug_sub_tasks = [{
+    "name": "surgeon",
+    "help_info": "surgeon tool for onnx modifying functions.",
+    "module": "auto_optimizer.ait_main",
+    "attr": "get_cmd_instance"
+}]
+
+debug_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in debug_sub_tasks]
+
 setup(
     name='ait-surgeon',
-    version='0.1.1',
+    version='7.0.0c2',
     description='auto optimizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitee.com/ascend/ait',
     packages=find_packages(),
-    package_data={'': ['LICENSE', 'model.cfg']},
+    package_data={'': ['LICENSE', 'model.cfg']},    
+
     license='Apache-2.0',
     keywords='auto optimizer',
     install_requires=required,
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
+        'License :: Apache-2.0 Software License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
-        'Topic :: Software Development'
-    ],
-    data_files=[
-        ('', ['requirements.txt']),
+        'Topic :: Software Development',
     ],
     extras_require={
-    #     'inference': [
-    #         (
-    #             'aclruntime @ git+https://gitee.com/ascend/ait.git'
-    #             '#egg=aclruntime&subdirectory=ait/components/benchmark/backend'
-    #         ),
-    #         (
-    #             'ais_bench @ git+https://gitee.com/ascend/ait.git'
-    #             '#egg=ais_bench&subdirectory=ait/components/benchmark/'
-    #         ),
-    #         'pillow >= 9.0.0',
-    #         'tqdm >= 4.63.0',
-    #     ],
+        'inference': [
+            (
+                'aclruntime @ git+https://gitee.com/ascend/ait.git'
+                '#egg=aclruntime&subdirectory=ait/components/benchmark/backend'
+            ),
+            (
+                'ais_bench @ git+https://gitee.com/ascend/ait.git'
+                '#egg=ais_bench&subdirectory=ait/components/benchmark/'
+            ),
+            'pillow >= 9.0.0',
+            'tqdm >= 4.63.0',
+        ],
         'simplify': ['onnx-simplifier >= 0.3.6'],
     },
     python_requires='>=3.7',
     entry_points={
         'console_scripts': ['auto_optimizer=auto_optimizer.__main__:cli'],
-        'debug_sub_task': ['surgeon=auto_optimizer.ait_main:get_cmd_instance'],
+        'debug_sub_task': debug_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-surgeon=auto_optimizer.__install__:SurgeonInstall'],
     },
 )
```

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/ait_main.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,15 @@
     check_nodes_string, check_single_node_string, check_normal_string, check_shapes_range_string, check_ints_string, \
     check_path_string, check_in_path_legality
 from auto_optimizer.common.click_utils import default_off_knowledges
 from auto_optimizer.pattern.knowledge_factory import KnowledgeFactory
 
 
 class ListCommand(BaseCommand):
-    def add_arguments(self, parser):
-        pass
-
-    def handle(self, args):
+    def handle(self, _):
         list_knowledges()
 
 
 class EvaluateCommand(BaseCommand):
     def add_arguments(self, parser):
         parser.add_argument('--path', required=True, type=check_in_path_legality,
                             help='Target onnx file or directory containing onnx file')
@@ -283,30 +280,19 @@
             combined_graph.save(combined_graph_path)
         except Exception as err:
             logger.error(err)
 
         logger.info(f"Combined ONNX model saved in: {combined_graph_path}")
 
 
-class SurgeonCommand(BaseCommand):
-    def __init__(self, name="", help_info="", children=None, has_handle=False, **kwargs):
-        super().__init__(name, help_info, children, has_handle, **kwargs)
-
-    def add_arguments(self, parser, **kwargs):
-        return super().add_arguments(parser, **kwargs)
-
-    def handle(self, args, **kwargs):
-        return super().handle(args, **kwargs)
-
-
 def get_cmd_instance():
     surgeon_help_info = "surgeon tool for onnx modifying functions."
     list_cmd_instance = ListCommand("list", "List available Knowledges")
     evaluate_cmd_instance = EvaluateCommand("evaluate", "Evaluate model matching specified knowledges", alias_name="eva")
     optimize_cmd_instance = OptimizeCommand("optimize", "Optimize model with specified knowledges", alias_name="opt")
     extract_cmd_instance = ExtractCommand("extract", "Extract subgraph from onnx model", alias_name="ext")
     concatenate_cmd_instance = ConcatenateCommand("concatenate",
                                                   "Concatenate two onnxgraph into combined one onnxgraph",
                                                   alias_name="concat")
-    return SurgeonCommand("surgeon", surgeon_help_info, [list_cmd_instance, evaluate_cmd_instance,
+    return BaseCommand("surgeon", surgeon_help_info, [list_cmd_instance, evaluate_cmd_instance,
                                                          optimize_cmd_instance, extract_cmd_instance,
                                                          concatenate_cmd_instance])
```

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/options.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/__main__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/args_check.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/click_utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/config.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/log.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/register.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/singleton.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/common/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
+import sys
+import os
+import unittest
+import torch
+import torch_npu
 
-from typing import Any
+from ait_llm.opcheck import operation_test
 
 
-@dataclass
-class InferenceResult:
-    label: Any = None
-    data: Any = None
+class OpcheckCumsumOperation(operation_test.OperationTest):
+    def golden_calc(self, in_tensors):
+        golden_result = torch.cumsum(in_tensors[0], dim=self.op_param['axes'][0])
+        return [golden_result]
+
+    def test(self):
+        self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/matcher.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/pattern.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/debug/surgeon/auto_optimizer/tools/log.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/setup.py` & `ms-ait-7.0.0rc2/components/analyze/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import subprocess
-import site
-import os
+from setuptools import setup, find_packages  # type: ignore
 
-from setuptools import setup, find_packages
 
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
-opchecker_lib_src = []
-for root, dirs, files in os.walk('components/llm/ait_llm/opcheck/test_framework/'):
-    opchecker_lib_src.append((os.path.join("/", root), [os.path.join(root, f) for f in files]))
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
+ait_sub_tasks = [{
+    "name": "model",
+    "help_info": "Analyze tool to evaluate compatibility of model conversion",
+    "module": "model_evaluation.__main__",
+    "attr": "get_cmd_instance"
+}]
+
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
-    name='ait-llm',
-    version='1.0',
-    description='Debug tools for large language model(llm)',
-    url='https://gitee.com/ascend/ait/ait/components/llm',
+    name='ait-analyze',
+    version='7.0.0c2',
+    description='inference analyze tool',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://gitee.com/ascend/ait',
     packages=find_packages(),
+    package_data={'model_evaluation': ['data/op_map/*.yaml']},
     license='Apache-2.0',
-    keywords='ait_llm',
+    keywords='analyze tool',
     install_requires=required,
     classifiers=[
         'Development Status :: Alpha',
         'Intended Audience :: Developers',
         'License :: Apache-2.0 Software License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
-        'Topic :: Software Development'
+        'Topic :: Software Development',
     ],
-    data_dir=f"{site.getsitepackages()[0]}",
-    data_files=opchecker_lib_src,
-    include_package_data=True,
     python_requires='>=3.7',
     entry_points={
-        'llm_sub_task': ['llm=ait_llm.__main__:get_cmd_instance'],
+        'ait_sub_task': ait_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-analyze=model_evaluation.__install__:AnalyzeInstall'],
     },
-    dependency_links= [
-        "https://download.pytorch.org/whl/cpu"
-    ]
-)
+)
```

## Comparing `ms-ait-7.0.0a4/components/llm/__init__.py` & `ms-ait-7.0.0rc2/components/debug/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-from components.utils.parser import load_command_instance
-
-llm_cmd = load_command_instance('llm_sub_task')
+# Copyright 2023 Huawei Technologies Co., Ltd
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import pkg_resources
+
+from components.utils.parser import BaseCommand
+
+
+def debug_task():
+    return BaseCommand("debug", "debug a wide variety of model issues", "debug_sub_task")
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 # limitations under the License.
 
 from ait_llm.common.tool import read_atb_data
 from ait_llm.compare.cmp_utils import compare_data
 from ait_llm.common.json_fitter import atb_json_to_onnx
 from ait_llm.dump.torch_dump import DumpConfig
 from ait_llm.dump.torch_dump import register_hook
+from ait_llm.metrics.case_filter import CaseFilter
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/__main__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 import subprocess
 
 from components.utils.parser import BaseCommand
 from ait_llm.dump.initial import init_dump_task, clear_dump_task
 from ait_llm.opcheck.opchecker import OpChecker
-from ait_llm.errcheck.initial import init_error_check
+from ait_llm.errcheck.process import process_error_check
 from ait_llm.common.utils import str2bool, check_positive_integer, check_device_integer, safe_string, check_exec_cmd, \
     check_ids_string, check_number_list, check_output_path_legality, check_input_path_legality
 from ait_llm.common.log import logger, set_log_level, LOG_LEVELS
 
 
 LOG_LEVELS_LOWER = [ii.lower() for ii in LOG_LEVELS.keys()]
 
@@ -170,14 +170,23 @@
         parser.add_argument(
             '--my-path',
             '-mp',
             dest="my_path",
             required=True,
             type=check_input_path_legality,
             help='Compared data path. It supports directory or file.')
+        
+        parser.add_argument(
+            '--cmp-level',
+            '-cl',
+            dest="cmp_level",
+            required=False,
+            default="layer",
+            choices=["layer", "token"],
+            help='Compare level. only enabled for atb.')
 
         parser.add_argument(
             '--log-level',
             '-l',
             dest="log_level",
             required=False,
             default="info",
@@ -211,36 +220,28 @@
             from ait_llm.compare.torchair_acc_cmp import acc_compare
 
             acc_compare(args.golden_path, args.my_path, args.output, torchair_ge_graph_path)
         else:
             from ait_llm.compare.atb_acc_cmp import acc_compare
 
             acc_compare(os.path.abspath(args.golden_path), os.path.abspath(args.my_path),
-                        args.output, args.mapping_file)
+                        args.output, args.mapping_file, args.cmp_level)
 
 
 class OpcheckCommand(BaseCommand):
     def add_arguments(self, parser, **kwargs):
         parser.add_argument(
             '--input',
             '-i',
             dest="input",
             required=True,
             type=check_input_path_legality,
             help='input directory.E.g:--input OUTPUT_DIR/PID_TID/0/')
 
         parser.add_argument(
-            '--csv-path',
-            '-c',
-            dest="csv_path",
-            required=True,
-            type=check_input_path_legality,
-            help='csv file path.E.g:--csv-path OUTPUT_DIR/ait_dump/operation_io_tensors/PID/operation_tensors_0.csv')
-
-        parser.add_argument(
             '--output',
             '-o',
             dest="output",
             required=False,
             type=check_output_path_legality,
             default='./',
             help='Data output directory.E.g:--output /xx/xxxx/xx')
@@ -338,25 +339,15 @@
             action='store_true',
             default=False,
             help="Flag determines whether to exit the program after detecting an error.\n"
                  "Defaults to False."
         )
 
     def handle(self, args, **kwargs) -> None:
-        if args.exec:
-            logger.info("Preparing to execute the command: %s", args.exec)
-            logger.warning("Please make sure that the executable command is safe.")
-            init_error_check(args)
-            # 有的大模型推理任务启动后，输入对话时有提示符，使用subprocess拉起子进程无法显示提示符
-            cmds = args.exec.split()
-            subprocess.run(cmds, shell=False)
-
-            # finished inference
-            logger.info("Inference finished.")
-            logger.info("Results are stored under the directory: %s.", os.environ['ATB_OUTPUT_DIR'])
+        process_error_check(args)       
 
 
 class Transform(BaseCommand):
     def add_arguments(self, parser, **kwargs) -> None:
         parser.add_argument(
             "-s",
             "--source",
@@ -373,32 +364,21 @@
     def handle(self, args, **kwargs) -> None:
         from ait_llm.transform import transform_quant
 
         set_log_level(args.log_level)
         transform_quant.transform_quant(source_path=args.source, enable_sparse=args.enable_sparse)
 
 
-class LlmCommand(BaseCommand):
-    def __init__(self, name="", help_info="", children=None, has_handle=False, **kwargs):
-        super().__init__(name, help_info, children, has_handle, **kwargs)
-
-    def add_arguments(self, parser, **kwargs):
-        return super().add_arguments(parser, **kwargs)
-
-    def handle(self, args, **kwargs):
-        return super().handle(args, **kwargs)
-
-
 def get_cmd_instance():
     llm_help_info = "Large Language Model(llm) Debugger Tools."
     dump_cmd_instance = DumpCommand("dump", "Dump tool for ascend transformer boost", alias_name="dd")
     compare_cmd_instance = CompareCommand("compare", "Accuracy compare tool for large language model", alias_name="cc")
     opcheck_cmd_instance = OpcheckCommand("opcheck", "Operation check tool for large language model", alias_name='oo')
     errcheck_cmd_instance = ErrCheck("errcheck", "Error check tool for large language model.", alias_name='ee')
     transform_cmd_instance = Transform(
         "transform", "Transform tool for large language model. Curretly only float to quant or sparse-quant model"
     )
 
     instances = [
         dump_cmd_instance, compare_cmd_instance, opcheck_cmd_instance, errcheck_cmd_instance, transform_cmd_instance
     ]
-    return LlmCommand("llm", llm_help_info, instances)
+    return BaseCommand("llm", llm_help_info, instances)
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/common/constant.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/common/json_fitter.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/common/log.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/common/tool.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/common/utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/compare/atb_acc_cmp.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 from ait_llm.compare.cmp_utils import BasicDataInfo, fill_row_data, save_compare_reault_to_csv
 from ait_llm.compare.op_mapping import ATB_TORCH_BUILT_IN_OP_OUTPUT_MAPPING, ATB_TORCH_CUSTOM_OP_OUTPUT_MAPPING
 from ait_llm.dump.torch_dump.topo import ModelTree
 
 from tqdm import tqdm
 
 
-def acc_compare(golden_path, my_path, output_path=".", mapping_file_path="."):
+def acc_compare(golden_path, my_path, output_path=".", mapping_file_path=".", cmp_level="layer"):
     if os.path.isdir(golden_path):
         golden_tensor_path = os.path.join(golden_path, "golden_tensor")
-        golden_topo_flag, golden_topo_json_path = is_model_topo_exist(golden_path)
-        my_topo_flag, my_topo_json_path = is_model_topo_exist(my_path)
-        torch_model_topo_file = os.path.join(golden_path, "..", "model_tree.json")
+        golden_topo_flag, golden_topo_json_path = is_model_topo_exist(golden_path, cmp_level)
+        my_topo_flag, my_topo_json_path = is_model_topo_exist(my_path, cmp_level)
+        torch_model_topo_file = os.path.join(golden_path, ".." if cmp_level == "layer" else "", "model_tree.json")
         if os.path.isdir(golden_tensor_path):
             # 存在golden_tensor路径，走手动映射比对逻辑
             logger.info("Manual mapping comparing starts! Comparing manual dump tensors and ATB tensors...")
             compare_metadata(golden_tensor_path, output_path)
         elif os.path.exists(torch_model_topo_file):
             # 存在torch_model_topo_file路径，走torch模型和加速库模型比对逻辑
             logger.info("Automatic mapping comparison starts! Comparing torch tensors and ATB tensors...")
-            cmp_torch_atb(torch_model_topo_file, golden_path, my_path, output_path, mapping_file_path)
+            cmp_torch_atb(torch_model_topo_file, (golden_path, my_path, output_path), mapping_file_path, cmp_level)
         elif golden_topo_flag and my_topo_flag:
             # 存在ATB模型的拓扑信息，走加速库模型间的比对逻辑
             compare_atb_metadata_auto(golden_path, my_path, golden_topo_json_path, my_topo_json_path, output_path)
         else:
             logger.warn("Unsupported comparison type, please refer to README")
 
     elif os.path.isfile(golden_path) and os.path.isfile(my_path):
         res = compare_file(golden_path, my_path)
         logger.info("Compared results: %s", res)
     else:
         logger.error("The golden_path and my_path must both be directory or file.")
 
 
-def is_model_topo_exist(golden_path):
+def is_model_topo_exist(golden_path, cmp_level="layer"):
     # 判断用户输入路径的ait_dump目录下是否包括/model路径，即是否包括模型拓扑信息
     absolute_path = os.path.abspath(golden_path)
-    model_dir_path = os.path.join(absolute_path, '../../../', 'model')
+    model_dir_path = os.path.join(absolute_path, '../../../' if cmp_level == "layer" else '../../', 'model')
     model_dir_path = os.path.normpath(model_dir_path)
     if not os.path.isdir(model_dir_path):
         msg = f"Cannot find {model_dir_path}, please check! Use ait llm dump if needed."
         logger.info(msg)
         return False, ""
     # 搜索/model目录下的所有文件，查找JSON文件
     for root, _, files in os.walk(model_dir_path):
@@ -351,14 +351,45 @@
         m_layer_all_nodes = my_layer.get_all_nodes()
         compared_result.extend(pair_custom_op(g_layer_all_nodes, m_layer_all_nodes,
                                               mapping_dic.get("ATB_TORCH_CUSTOM_OP_OUTPUT_MAPPING")))
 
     return save_compare_reault_to_csv(compared_result, output_path)
 
 
+def get_only_dir_in_path(p_path):
+    file_list = os.listdir(p_path)
+
+    if len(file_list) != 1 or not os.path.isdir(os.path.join(p_path, file_list[0])):
+        logger.warning(f"There must be only one directory in the {p_path}")
+        return None
+    
+    return os.path.join(p_path, file_list[0])
+
+
+
+def cmp_torch_atb_token(torch_tensor_path, atb_tensor_path, token_id):
+    compare_result = []
+
+    torch_layer_path = get_only_dir_in_path(torch_tensor_path)
+    atb_layer_path = get_only_dir_in_path(atb_tensor_path)
+
+    if atb_tensor_path is None or torch_tensor_path is None:
+        return compare_result
+    
+    golden_tensor_path = os.path.join(torch_layer_path, "output.pth")
+    my_tensor_path = os.path.join(atb_layer_path, "after", "outtensor0.bin")
+
+    if os.path.exists(golden_tensor_path) and os.path.exists(my_tensor_path):
+        data_info = BasicDataInfo(golden_tensor_path, my_tensor_path, data_id=0, token_id=token_id)
+        row_data = fill_row_data(data_info)
+        compare_result.append(row_data)
+
+    return compare_result
+
+
 def validate_json(json_obj):
     for key, value in json_obj.items():
         if not re.match(r"^[a-zA-Z0-9_]*$", key):
             return False
         if not isinstance(value, str) and not isinstance(value, list):
             return False
         if isinstance(value, str):
@@ -389,36 +420,56 @@
             msg = f"Invalid op_mapping file: {mapping_file}"
             logger.error(msg)
     else:
         logger.debug("Using built-in op_mapping")
     return mapping_dic
 
 
-def cmp_torch_atb(torch_model_topo_file, golden_path, my_path, output_path, mapping_file_path):
+def cmp_torch_atb(torch_model_topo_file, cmp_paths, mapping_file_path, cmp_level="layer"):
+    golden_path, my_path, output_path = cmp_paths
     try:
-        pid = str(my_path.split("/")[-2].split("_")[1])
+        path_index = -2 if cmp_level == "layer" else -1
+        pid = str(my_path.split("/")[path_index].split("_")[1])
     except IndexError as e:
         pid = ""
         msg = f"Cannot parse the right pid from my_path! my_path: {my_path}"
         logger.error(msg)
     
     csv_file_path = ""
-    atb_model_topo_file_path = os.path.join(my_path, "../../..", "model", pid)
+    atb_model_topo_file_path = os.path.join(my_path, "../../.." if cmp_level == "layer" else "../..", "model", pid)
     if os.path.exists(atb_model_topo_file_path):
         atb_model_topo_name = os.listdir(atb_model_topo_file_path)[0]
         atb_model_topo_file = os.path.join(atb_model_topo_file_path, atb_model_topo_name)
-        if os.path.exists(atb_model_topo_file):
+        if os.path.exists(atb_model_topo_file) and cmp_level == "layer":
             mapping_dic = load_mapping(mapping_file_path)
             data_info = {
                 "golden_json": torch_model_topo_file,
                 "my_json": atb_model_topo_file,
                 "torch_tensor_path": golden_path,
                 "atb_tensor_path": my_path,
             }
             csv_file_path = cmp_torch_atb_model(data_info, output_path, mapping_dic)
+        elif cmp_level == "token":
+            compared_results = []
+
+            for token_id in os.listdir(my_path):
+                torch_token_path = os.path.join(golden_path, str(token_id))
+                atb_token_path = os.path.join(my_path, str(token_id))
+
+                if not os.path.exists(torch_token_path) or not os.path.exists(atb_token_path):
+                    continue
+
+                if not os.path.isdir(torch_token_path) or not os.path.isdir(atb_token_path):
+                    continue
+
+                compare_result = cmp_torch_atb_token(torch_token_path, atb_token_path, token_id)
+
+                compared_results.extend(compare_result)
+                
+            csv_file_path = save_compare_reault_to_csv(compared_results, output_path)
         else:
             msg = f"Cannot find atb model file: {atb_model_topo_file}"
             logger.error(msg)
     else:
         msg = f"Cannot find atb model file path: {atb_model_topo_file_path}"
         logger.error(msg)
     return csv_file_path
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/compare/cmp_utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/compare/op_mapping.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/compare/torchair_acc_cmp.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/initial.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 import site
 import subprocess
 import shutil
 import re
 
 from components.utils.file_open_check import FileStat
 from ait_llm.common.log import logger
+from ait_llm.common.utils import safe_string
 from ait_llm.common.constant import ATB_HOME_PATH, ATB_SAVE_TENSOR_TIME, ATB_SAVE_TENSOR_IDS, \
     ATB_SAVE_TENSOR_RUNNER, ATB_SAVE_TENSOR, ATB_SAVE_TENSOR_RANGE, \
     ATB_SAVE_TILING, LD_PRELOAD, ATB_OUTPUT_DIR, ATB_SAVE_CHILD, ATB_SAVE_TENSOR_PART, \
     ASCEND_TOOLKIT_HOME, ATB_PROB_LIB_WITH_ABI, ATB_PROB_LIB_WITHOUT_ABI, ATB_SAVE_CPU_PROFILING, \
     ATB_CUR_PID, ATB_DUMP_SUB_PROC_INFO_SAVE_PATH, ATB_DEVICE_ID, ATB_AIT_LOG_LEVEL, ATB_DUMP_TYPE
 
 
 def is_use_cxx11():
     atb_home_path = os.environ.get(ATB_HOME_PATH, "")
     if not atb_home_path or not os.path.exists(atb_home_path):
         raise OSError("ATB_HOME_PATH from atb is required, but it is empty or invalid.")
+    atb_home_path = safe_string(atb_home_path)
     lib_atb_path = os.path.join(atb_home_path, "lib", "libatb.so")
     if not os.path.exists(lib_atb_path):
         raise OSError(f"{lib_atb_path} not exists, please make sure atb is compiled correctly")
 
     result_code, abi_result = subprocess.getstatusoutput(f"nm -D {lib_atb_path} | grep Probe | grep cxx11")
     if result_code == 1 and len(abi_result) == 0:  # Execute succesfully but not found
         return False
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/manual_dump.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 
 import numpy as np
 import torch
 
 from components.utils.file_open_check import ms_open
 from ait_llm.common.log import logger
+from ait_llm.common.utils import check_input_path_legality, check_output_path_legality
 
 
 def dump_data(token_id=-1, data_id=-1, golden_data=None, my_path='', output_path='./'):
     # 传参失败的提示
     if token_id == -1:
         logger.warning('Please check whether token_id passed in are correct')
         return
@@ -30,14 +31,16 @@
         return
     elif not isinstance(golden_data, torch.Tensor):
         logger.warning('The golden_data is not a torch tensor!')
         return
     elif my_path == '':
         logger.warning('Please check whether my_path passed in are correct')
         return
+    check_input_path_legality(my_path)
+    check_output_path_legality(output_path)
 
     if golden_data is not None:
         cur_pid = os.getpid()
         device_id = golden_data.get_device()
         golden_data_dir = os.path.join(output_path, "ait_dump", f"{cur_pid}_{device_id}", "golden_tensor",
                                        str(token_id))
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import time
 
 from ait_llm.common.log import logger
+from ait_llm.common.utils import check_output_path_legality
 
 
 def try_import_torchair():
     try:
         import torch
         import torch_npu
         import torchair
@@ -29,14 +30,15 @@
 
 def get_ge_dump_config(dump_path="ait_ge_dump", dump_mode="all", fusion_switch_file=None):
     try_import_torchair()
 
     from torchair.configs.compiler_config import CompilerConfig
 
     config = CompilerConfig()
+    check_output_path_legality(dump_path)
     dump_path = os.path.join(dump_path, "dump_" + time.strftime('%Y%m%d_%H%M%S'))  # Timestamp like '20240222_095519'
     if not os.path.exists(dump_path):
         os.makedirs(dump_path, mode=0o750)
 
     # Generate GE mapping graph
     config.debug.graph_dump.type = "txt"
     if hasattr(config.debug.graph_dump, "_path"):  # interface changed since 8.0.RC1.b080
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_config.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,29 @@
         return ins.get(cls)
 
     return run
 
 
 @singleton
 class DumpConfig:
-    def __init__(self, dump_path=None, token_range=None, module_list=None, tensor_part=2, device_id=None):
+    def __init__(self, dump_path=None, token_range=None, module_list=None, tensor_part=2, device_id=None, dump_last_logits=False):
         self.dump_path = dump_path or "./"
         self.mode = "module"
         self.token_range = token_range or [0]
         self.module_list = module_list or []
         self.tensor_part = tensor_part
         self.device_id = device_id
         self.is_dump_cur_device = True
         self.dump_flag = True
         self.token_id = 0
         self.module_ids = {}
         self.cur_module_id = 0
         self.dump_dir = ""
+        self.dump_last_logits = dump_last_logits
+        self.last_logits = None
 
         if not self._check_args():
             raise ValueError("Invalid args of DumpConfig.")
 
     def set_dump_device_and_dump_dir(self, device):
         if self.device_id is not None and device != "cpu":
             # Get the first position of a digit char, and cut out like cuda0 -> cuda, npu12 -> npu
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/dump_hook.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,20 +46,24 @@
             module.ait_forward_handle = module.register_forward_hook(dump_module_data())
             module.name = prefix
             for name, child_module in module.named_children():
                 add_hook(child_module, prefix + "." + name)
 
         self.model.name = model_name
         self.model.ait_forward_pre_handle = self.model.register_forward_pre_hook(set_dump_flag())
+        self.model.model_ait_forward_handle = self.model.register_forward_hook(dump_logits())
         add_hook(self.model, prefix=model_name)
 
     def _remove_module_hook(self):
         if hasattr(self.model, "ait_forward_pre_handle"):
             self.model.ait_forward_pre_handle.remove()
 
+        if hasattr(self.model, "model_ait_forward_handle"):
+            self.model.model_ait_forward_handle.remove()
+
         def _remove_hook(module):
             if hasattr(module, "ait_forward_handle"):
                 module.ait_forward_handle.remove()
             for _, _child_module in module.named_children():
                 _remove_hook(_child_module)
 
         _remove_hook(self.model)
@@ -148,14 +152,19 @@
                 os.makedirs(dump_config.dump_dir, mode=0o750)
             model_tree_path = os.path.join(dump_config.dump_dir, "model_tree.json")
             obj = ModelTree()
             obj.create_tree(module, dump_config.module_ids, model_tree_path)
 
         if dump_config.mode == "api" or not dump_config.dump_flag:
             return
+        
+        if dump_config.dump_last_logits:
+            if has_tensor(outputs):
+                dump_config.last_logits = (module.name, outputs)
+            return 
 
         if dump_config.module_list and not isinstance(module, tuple(dump_config.module_list)):
             return
 
         module_name = module.name
         dump_path = os.path.join(dump_config.dump_dir, str(dump_config.token_id), module_name)
         if not os.path.exists(dump_path):
@@ -178,7 +187,34 @@
             config.dump_flag = True
         else:
             config.dump_flag = False
 
         cur_token_id += 1
 
     return hook_func
+
+
+def has_tensor(feat):
+    if isinstance(feat, (tuple, list)):
+        for tensor in feat:
+            if has_tensor(tensor):
+                return True
+    elif isinstance(feat, torch.Tensor):
+        return True 
+    return False
+
+
+def dump_logits():
+    # 将缓存的输出dump到文件中
+    def hook_func(*args):
+        config = DumpConfig()
+        if config.dump_last_logits and config.last_logits is not None:
+            module_name, outputs = config.last_logits
+
+            dump_path = os.path.join(config.dump_dir, str(config.token_id), module_name)
+
+            if not os.path.exists(dump_path):
+                os.makedirs(dump_path, mode=0o750)
+            dump_tensor(outputs, os.path.join(dump_path, "output"))
+
+    return hook_func
+
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/hook_ops.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/topo.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/dump/torch_dump/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-# Copyright (c) 2024 Huawei Technologies Co., Ltd.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-from ait_llm.dump.torch_dump.dump_config import DumpConfig
-from ait_llm.dump.torch_dump.hook import register_hook
+# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import sys
+import os
+import unittest
+import torch
+import torch_npu
+
+from ait_llm.opcheck import operation_test
+
+
+class OpcheckRepeatOperation(operation_test.OperationTest):
+    def golden_calc(self, in_tensors):
+        outtensor = in_tensors[0].repeat(self.op_param["multiples"])
+        return [outtensor]
+
+    def test(self):
+        self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/case_manager.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
-from ait_llm.opcheck.opcheck_checkcases import OP_NAME_DICT
+from ait_llm.opcheck.check_case import OP_NAME_DICT
 
 
 class CaseManager:
     def __init__(self, excuted_ids=None):
         self.suite = unittest.TestSuite()
         self.cases = []
         self.excuted_ids = excuted_ids
-    
+
     def add_case(self, case_info):
         op_name = case_info['op_name']
         if op_name not in OP_NAME_DICT.keys():
             #没有该op_name
             return False 
         else:
             if OP_NAME_DICT[op_name]:
@@ -41,8 +41,8 @@
             self.suite.addTest(op.parametrize(optest_class=op, case_info=case_info, excuted_ids=self.excuted_ids))
 
     def excute_cases(self):
         self.add_cases_to_suite()
 
         #拉起测试套
         runner = unittest.TextTestRunner(verbosity=2)
-        runner.run(self.suite)
+        runner.run(self.suite)
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opchecker.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     def __init__(self):
         '''
         cases_info结构：
             'op_id': string
             'op_name': string
             'op_param': dict
             'tensor_path': string
-            'out_dtype: list
         '''
         self.csv_data = {}
         self.cases_info = {}
         self.completed_op_id_queue = queue.Queue()
         self.special_cases = ['KvCacheOperation', 'ReshapeAndCacheOperation', 'SelfAttentionOperation']
+        self.base_path = ''
         self.tensor_path = ''
         self.op_path = ''
         self.output_dir = ''
         self.output_path = ''
         self.ids = ''
         self.check_ids_string = []
         self.opname = None
@@ -52,46 +52,92 @@
         self.precision_type = []
         utc_time = datetime.datetime.now(tz=pytz.utc)
         self.timestamp = utc_time.astimezone(pytz.timezone('Asia/Shanghai')).strftime("%Y%m%d_%H%M%S")
         self.rerun = False
 
     @staticmethod
     def third_party_init():
-        execution_flag = True
-
         import ait_llm
+        import ctypes
 
-        lib_path = os.environ.get("AIT_OPCHECK_LIB_PATH")
-        if not lib_path:
+        # Loading libopchecker.so with ctypes
+        lib_opchecker_path = os.environ.get("AIT_OPCHECK_LIB_PATH", "")
+        if not lib_opchecker_path:
             lib_path_dir = os.path.dirname(os.path.abspath(ait_llm.__file__))
-            lib_path = os.path.join(lib_path_dir, "opcheck", "libopchecker.so")
+            lib_opchecker_path = os.path.join(lib_path_dir, "opcheck", "libopchecker.so")
 
-        if os.path.exists(lib_path):
-            try:
-                logger.info(lib_path)
-                torch.classes.load_library(lib_path)
-            except OSError as e:
-                logger_text = "Failed to load libopchecker.so, please check. Error: {}".format(e)
-                logger.error(logger_text)
-                execution_flag = False
+        logger.info(f"lib_opchecker_path is {lib_opchecker_path}")
+        if not os.path.exists(lib_opchecker_path):
+            logger.error(f"{lib_opchecker_path} not exists, check if ait_llm installed correctly")
+            return False
+
+        try:
+            ctypes.cdll.LoadLibrary(lib_opchecker_path).RegisterAll()
+        except Exception as e:
+            logger.error(f"{lib_opchecker_path} loading failed, check if ait_llm installed correctly")
+            return False
+
+        # Loading libatb_speed_torch.so with torch
+        atb_speed_path = os.getenv('ATB_SPEED_HOME_PATH', "")
+        if not atb_speed_path:
+            logger.error("ATB_SPEED_HOME_PATH is empty, check if mindie_atb_models configured correctly")
+            return False
+
+        libatb_speed_torch_path = os.path.join(atb_speed_path, 'lib', 'libatb_speed_torch.so')
+        logger.info(f"libatb_speed_torch_path is {libatb_speed_torch_path}")
+        if not os.path.exists(libatb_speed_torch_path):
+            logger.error(f"{libatb_speed_torch_path} not exists, check if mindie_atb_models configured correctly")
+            return False
+
+        try:
+            torch.classes.load_library(libatb_speed_torch_path)
+        except Exception as e:
+            logger.error(f"{libatb_speed_torch_path} loading failed, check if mindie_atb_models configured correctly")
+            return False
+
+        return True
+
+    def get_base_path(self, cur_path):
+        dirseg = cur_path.split(os.path.sep)
+        if len(dirseg) >= 4 and dirseg[-3] == 'tensors' and dirseg[-4] == 'ait_dump':
+            return cur_path
+        elif cur_path == os.path.dirname(cur_path):
+            return None
         else:
-            logger_text = "libopchecker.so not found in {}".format(lib_path)
-            logger.error(logger_text)
-            execution_flag = False
+            return self.get_base_path(os.path.dirname(cur_path))
 
-        return execution_flag
+    def check_input_legality(self, input_path):
+        ret = False
+        base_path = None
+
+        input_path = os.path.realpath(input_path)
+        if not os.path.exists(input_path):
+            logger_text = f"Input path not found: {input_path}"
+            logger.error(logger_text)
+            return input_path, base_path, ret
+        
+        base_path = self.get_base_path(input_path)
+        if base_path is None:
+            logger_text = f"input path is not in ait_dump tensors directory: {input_path}"
+            logger.error(logger_text)
+            return input_path, base_path, ret
+        
+        ret = True
+        return input_path, base_path, ret
 
     def args_init(self, args):
         import torch_npu
 
         execution_flag = True
 
-        self.tensor_path = args.input
-        self.op_path = args.csv_path
-        self.output_dir = args.output
+        self.tensor_path, self.base_path, ret = self.check_input_legality(args.input)
+        if not ret:
+            execution_flag = False
+        
+        self.output_dir = os.path.realpath(args.output) 
         self.output_path = os.path.join(self.output_dir, f"opcheck_result_{self.timestamp}.xlsx")
         self.ids = args.ids
         if self.ids != '':
             try:
                 self.check_ids_string = [x.lower().strip() for x in self.ids.split(',')]
             except ValueError as e:
                 logger_text = "Failed to parse ids. Error: {}".format(e)
@@ -132,22 +178,22 @@
         # 0.初始化
         execution_flag_res = self.args_init(args)
         if not execution_flag_res:
             return
 
         from ait_llm.opcheck.case_manager import CaseManager
         case_manager = CaseManager(self.completed_op_id_queue)
-
-        # 1.将csv文件中的算子信息添加到self.cases_info
-        execution_flag_res = self.add_file_info_to_cases()
-        if not execution_flag_res:
-            return
-        result_info = 'excuted_information'
+        
+        # 1.遍历tensor_path，将算子信息添加到self.cases_info
+        self.walk_tensor_path(self.tensor_path)
+        logger_text = f"Total {len(self.cases_info)} cases found under path: {self.tensor_path}"
+        logger.info(logger_text)
 
         # 2.将self.cases_info中的用例添加到case_manager
+        result_info = 'excuted_information'
         for _, case_info in self.cases_info.items():
             if_successed_add_case = case_manager.add_case(case_info)
             if if_successed_add_case:
                 case_info[result_info] = 'addition successed'
             else:
                 case_info[result_info] = 'addition failed'
 
@@ -155,137 +201,120 @@
         self.excute_cases(case_manager)
 
         # 4.写入未添加成功的算子
         for v in self.cases_info.values():
             if v[result_info] == 'addition failed':
                 v['res_detail'] = []
                 self.write_op_result_to_csv(v)
+        logger.info(f"\nOpcheck results saved to: {self.output_path}")
 
-    def parse_in_tensor_path(self, ids):
-        in_tensor_path = os.path.join(self.tensor_path, '_*/'.join(ids.split("_")) + '_*', "after")
-        files = glob.glob(in_tensor_path)
-        if not len(files) == 1:
-            logger_text = "{} could not find a dir!".format(in_tensor_path)
+    def parse_op_id_name(self, dirpath):
+        basename = os.path.basename(dirpath)
+        try:
+            op_name = basename.split('_')[-1]
+        except IndexError as e:
+            logger_text = f"{dirpath} is not a valid tensor dir, please check"
             logger.debug(logger_text)
-            return ""
-        return files[0]
+            op_name = None
 
-    def parse_csv_files(self):
+        rel_path = os.path.relpath(dirpath, self.base_path)
         try:
-            df = pd.read_csv(self.op_path, sep='|')
-        except Exception as e:
-            logger_text = f"Cannot read csv file: {self.op_path}"
-            logger.error(logger_text)
-            df = pd.DataFrame()
-
-        op_name_str = "OpName"
-        if op_name_str in df.columns and "OutDType" in df.columns:
-            df = df.loc[~df['OutDType'].isnull() & ~df[op_name_str].isnull()]
-            try:
-                df['Ids'] = df[op_name_str].apply(lambda x: x.split("_", 1)[1])
-                df['RealOpName'] = df[op_name_str].apply(lambda x: x.split("_", 1)[0])
-                df['InTensorPath'] = df['Ids'].apply(lambda x: self.parse_in_tensor_path(x))
-                df['OutDTypeParse'] = df['OutDType'].apply(lambda x: x.split(";"))
-            except Exception as e:
-                logger_text = f"Cannot parse csv file: {self.op_path}"
-                logger.error(logger_text)
-                df = pd.DataFrame()
-        else:
-            logger_text = f"Cannot find enough info in csv file: {self.op_path}"
-            logger.error(logger_text)
-            df = pd.DataFrame()
+            op_id = '_'.join([x.split('_')[0] for x in rel_path.split(os.path.sep)])
+        except IndexError as e:
+            logger_text = f"{dirpath} is not a valid tensor dir, please check"
+            logger.debug(logger_text)
+            op_id = None
 
-        return df
+        return op_id, op_name
 
     def check_id_range(self, op_id):
+        if op_id is None:
+            return False
         if self.ids == '':
             return True
-        else:
-            for p in self.check_ids_string:
-                ret = re.match("^" + p + "(_[0-9]+){0,20}$", op_id)
-                if ret:
-                    return True
-            return False
+
+        for p in self.check_ids_string:
+            ret = re.match("^" + p + "(_[0-9]+){0,20}$", op_id)
+            if ret:
+                return True
+        return False
 
     def check_name(self, op_name):
+        if op_name is None:
+            return False
         if self.opname is None:
             return True
-        else:  # 应该是LinearOps，SelfAttention
-            for p in self.check_patterns:
-                if p in op_name.lower():
-                    return True
-            return False
-
-    def check_path_valid(self, path):
-        return path and os.path.isdir(path)
 
-    def if_exec_node(self, row):
-        flag0 = self.check_path_valid(row["InTensorPath"])
-        if not flag0:
-            return False
+        for p in self.check_patterns:
+            if p in op_name.lower():
+                return True
+        return False
 
+    def is_exec_node(self, case_info):
         if self.ids == '' and self.opname is None:
             return True
 
-        flag1 = self.check_id_range(row["Ids"])
-        flag2 = self.check_name(row["RealOpName"])
-        if flag1 and flag2:
-            return True
-
-        return False
-
-    def add_case_to_cases_info(self, row):
-        op_id = row['Ids']
-        op_name = row['RealOpName']
-        try:
-            op_param = json.loads(row['OpParam'])
-        except TypeError:
-            logger_text = f"Cannot loads OpParam to json! OpParam: {row['OpParam']}"
-            logger.debug(logger_text)
-            op_param = {}
-
-        tensor_path = row["InTensorPath"]
-        out_dtype = row["OutDTypeParse"]
-
-        case_info = {
-            'op_id': op_id, 'op_name': op_name, 'op_param': op_param, 'tensor_path': tensor_path,
-            'out_dtype': out_dtype, 'precision_type': self.precision_type, 'rerun': self.rerun
-        }
-
+        flag1 = self.check_id_range(case_info.get("op_id", None))
+        flag2 = self.check_name(case_info.get("op_name", None))
+        return flag1 and flag2
+
+    def add_case_to_cases(self, case_info):
+        op_name = case_info.get("op_name", None)
+        op_id = case_info.get("op_id", None)
         if op_name == 'KvCacheOperation':
             case_info['inplace_idx'] = [2]
             self.cases_info[op_id] = case_info
         elif op_name == 'ReshapeAndCacheOperation':
             case_info['inplace_idx'] = [2, 3]
             self.cases_info[op_id] = case_info
         elif op_name == 'SelfAttentionOperation':
             self.cases_info[op_id] = case_info
         else:
             self.cases_info[op_id] = case_info
 
-    def add_parse_info_to_cases(self, csv_data):
-        for _, row in csv_data.iterrows():
-            flag = self.if_exec_node(row)
-            if flag:
-                self.add_case_to_cases_info(row)
+    def add_op_info_to_cases_info(self, dirpath):
+        tensor_path = os.path.join(dirpath, 'after')
 
-    def add_file_info_to_cases(self):
-        execution_flag = True
-        if os.path.exists(self.op_path):
-            csv_data = self.parse_csv_files()
-            if csv_data.empty:
-                execution_flag = False
-            else:
-                self.add_parse_info_to_cases(csv_data)
-        else:
-            logger_text = f"{self.op_path} not exists"
-            logger.error(logger_text)
-            execution_flag = False
+        json_path = os.path.join(dirpath, 'op_param.json')
+        try:
+            with open(json_path, 'r') as f:
+                op_param = json.load(f)
+        except Exception as e:
+            logger_text = f"Cannot loads json file to json! Json file: {json_path} \n Exception: {e}"
+            logger.debug(logger_text)
+            return
 
-        return execution_flag
+        op_id, op_name = self.parse_op_id_name(dirpath)
+        if op_id is None or op_name is None:
+            return
+
+        case_info = {
+            'op_id': op_id, 'op_name': op_name, 'op_param': op_param, 'tensor_path': tensor_path,
+            'precision_type': self.precision_type, 'rerun': self.rerun
+        }
+
+        ret = self.is_exec_node(case_info)
+        if ret:
+            self.add_case_to_cases(case_info)
+        return
+
+    def walk_tensor_path(self, cur_path):
+        files_and_dirs = os.listdir(cur_path)
+        dirnames, filenames = [], []
+        for item in files_and_dirs:
+            item_path = os.path.join(cur_path, item)
+            if os.path.isdir(item_path):
+                dirnames.append(item)
+            else:
+                filenames.append(item)
+        if 'after' in dirnames and 'op_param.json' in filenames:
+            self.add_op_info_to_cases_info(cur_path)
+        for dirname in dirnames:
+            if dirname != 'after':
+                self.walk_tensor_path(os.path.join(cur_path, dirname))
 
     def excute_cases(self, case_manager):
         # 定义监控队列函数
         def watching_queue():
             cases_num = len([1 for v in self.cases_info.values() if v["excuted_information"] == 'addition successed'])
             cases_index = 0
             while cases_index < cases_num:
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/operation_test.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,47 +22,45 @@
 import torch_npu
 
 from ait_llm.common.tool import read_atb_data
 from ait_llm.common.log import logger
 from ait_llm.compare.cmp_algorithm import CMP_ALG_MAP
 
 
+FLOAT_EPSILON = torch.finfo(torch.float).eps
+
+
 class OperationTest(unittest.TestCase):
     def __init__(self, methodName='opTest', case_info=None, excuted_ids=None):
         super(OperationTest, self).__init__(methodName)
 
         self.case_info = case_info
         self.case_info['res_detail'] = []
         self.excuted_ids = excuted_ids
         self.op_id = case_info['op_id']
         self.op_name = case_info['op_name']
         self.op_param = case_info['op_param']
         self.tensor_path = case_info['tensor_path']
         self.in_tensors = []
         self.out_tensors = []
-        self.out_dtype = self.case_info["out_dtype"]
         self.rerun = self.case_info["rerun"]
-        
+
         error1 = 'Error0.1‰'
         error2 = 'Error0.5‰'
         error3 = 'Error1‰'
         error4 = 'Error4‰'
         error5 = 'Error5‰'
         error6 = 'Error+/-1'
 
         self.precision_standard = {
-            'ACL_DOUBLE': [error1, 99.99], 'ACL_UINT32': [error1, 99.99], 'ACL_INT64': [error1, 99.99], 
-            'ACL_FLOAT': [error1, 99.99], 'ACL_INT32': [error1, 99.99], 'ACL_UINT64': [error1, 99.99], 
-            'ACL_FLOAT16': [error3, 99.9], 'ACL_BF16': [error4, 99.6], 'ACL_INT8': [error6, 99.9], 
-            'ACL_UINT8': [error6, 99], 'ACL_INT16': [error6, 99.9], 'ACL_UINT16': [error6, 99.9], 
-            'ACL_BOOL': [error1, 100], 'double': [error1, 99.99], 'uint32': [error1, 99.99], 
-            'int64': [error1, 99.99], 'float': [error1, 99.99], 'int32': [error1, 99.99], 
-            'uint64': [error1, 99.99], 'float16': [error3, 99.9], 'bf16': [error4, 99.6], 
-            'int8': [error6, 99.9], 'uint8': [error6, 99], 'int16': [error6, 99.9], 
-            'uint16': [error6, 99.9], 'bool': [error1, 100]
+            'torch.double': [error1, 99.99], 'torch.uint32': [error1, 99.99], 'torch.int64': [error1, 99.99],
+            'torch.float': [error1, 99.99], 'torch.int32': [error1, 99.99], 'torch.uint64': [error1, 99.99],
+            'torch.float16': [error3, 99.9], 'torch.bf16': [error4, 99.6], 'torch.int8': [error6, 99.9],
+            'torch.uint8': [error6, 99], 'torch.int16': [error6, 99.9], 'torch.uint16': [error6, 99.9],
+            'torch.bool': [error1, 100]
         }
 
         self.erol_dict = {
             error1: 0.0001,
             error2: 0.0005,
             error3: 0.001,
             error4: 0.004,
@@ -74,15 +72,15 @@
     def parametrize(optest_class, case_info=None, excuted_ids=None):
         testloader = unittest.TestLoader()
         testnames = testloader.getTestCaseNames(optest_class)
         suite = unittest.TestSuite()
         for name in testnames:
             suite.addTest(optest_class(name, case_info=case_info, excuted_ids=excuted_ids))
         return suite
-    
+
     def setUp(self):
         def get_tensor_path(tensor_type):
             _tensor_path = [x for x in os.listdir(self.tensor_path) if x.startswith(tensor_type)]
             _tensor_path.sort(key=lambda x:int(x.split(tensor_type)[1].split('.')[0]))  
             _tensor_path = [os.path.join(self.tensor_path, x) for x in _tensor_path]
             return _tensor_path
 
@@ -96,20 +94,20 @@
                 for path in _out_tensor_path:
                     _out_tensor = read_atb_data(path).npu()
                     self.out_tensors.append(_out_tensor)
             else:
                 raise RuntimeError(f"{self.tensor_path} not valid")
         else:
             raise RuntimeError(f"{self.tensor_path} not valid")
-    
+
     def tearDown(self):
         self.excuted_ids.put(self.op_id)
         if self.case_info['excuted_information'] != 'execution successful':
             self.case_info['excuted_information'] = 'execution failed'
-    
+
     def rerun_op(self, excute_type): 
         operation = torch.classes.OperationTorch.OperationTorch(self.op_name)
         if isinstance(self.op_param, dict):
             operation.set_param(json.dumps(self.op_param))
         elif isinstance(self.op_param, str):
             operation.set_param(self.op_param)
         if excute_type == "inplace":
@@ -147,80 +145,56 @@
     def execute_with_param(self):
         self.excute_common("with_param")
 
     def execute_inplace(self):
         self.excute_common("inplace")
 
     def get_rel_pass_rate(self, out, golden, etol):
-        out, golden = out.reshape(-1), golden.reshape(-1)
+        out, golden = out.reshape(-1).cpu(), golden.reshape(-1).cpu()
         size = out.shape[0]
-        golden_denom = golden.clone().float()
-        golden_denom[golden_denom == 0] += torch.finfo(torch.bfloat16).eps
-        try:
-            rel_errors = torch.abs((out - golden) / golden_denom)
-            rel_pass_rate = torch.sum(rel_errors <= etol) / size
-        except ZeroDivisionError as e:
-            logger_text = "Pass rate of rel error cannot be calculated because the denom is 0. Exception: {}".format(e)
-            logger.debug(logger_text)
-            raise e
-        return rel_pass_rate
-    
-    def get_max_rel_error(self, out, golden):
-        out, golden = out.reshape(-1).float().cpu(), golden.reshape(-1).float().cpu()
-        max_rel_error, _ = CMP_ALG_MAP["max_relative_error"](golden, out)
-        return max_rel_error
+        rel_errors = torch.where(
+            torch.abs(golden) > FLOAT_EPSILON,
+            torch.abs(out / golden - 1),  # abs(aa - bb) / abs(bb) -> abs(aa / bb - 1)
+            torch.tensor(0, dtype=out.dtype),
+        )
+        rel_pass_rate = torch.sum(rel_errors <= etol) / size if size != 0 else 0
+        max_rel_error = torch.max(rel_errors)
+        return rel_pass_rate.item() * 100, max_rel_error.item()
 
     def get_abs_pass_rate(self, out, golden, etol):
+        out, golden = out.cpu(), golden.cpu()
         size = out.shape[0]
-        abs_errors = torch.abs(out - golden)
+        abs_errors = torch.where(
+            torch.abs(golden) > FLOAT_EPSILON,
+            torch.abs(out - golden),  # abs(aa - bb) / abs(bb) -> abs(aa / bb - 1)
+            torch.tensor(0, dtype=out.dtype),
+        )
+        abs_pass_rate = torch.sum(abs_errors <= etol) / size if size != 0 else 0
         max_abs_error = torch.max(abs_errors)
-        try:
-            abs_pass_rate = torch.sum(abs_errors <= etol) / size if size != 0 else 0
-        except ZeroDivisionError as e:
-            logger_text = "Pass rate of abs error cannot be calculated because the denom is 0. Exception: {}".format(e)
-            logger.debug(logger_text)
-            abs_pass_rate = None
-        return abs_pass_rate, max_abs_error
+        return abs_pass_rate.item() * 100, max_abs_error.item()
 
-    def get_cos_similarity(self, out, golden):
-        cos_sim, _ = CMP_ALG_MAP["cosine_similarity"](golden, out)
-        return cos_sim      
-    
-    def get_kl_divergence(self, out, golden):
-        out, golden = out.tolist(), golden.tolist()
-        try:
-            out_prob = out / np.sum(out)
-            golden_prob = golden / np.sum(golden)
-            kl = np.sum(np.where(out_prob != 0, out_prob * np.log(out_prob / golden_prob), 0))
-            kl = kl if kl > 0 else 0
-        except ZeroDivisionError as e:
-            logger_text = "Kl divergence cannot be calculated because the denom is 0. Exception: {}".format(e)
-            logger.debug(logger_text)
-            kl = None
-        return kl
-    
     def get_other_precisions(self, out, golden, etol):
         precision_type = self.case_info['precision_type']
         default_str = 'NaN'
-        abs_pass_rate, max_abs_error, kl_div = None, None, None
-        cos_sim_str = default_str
-        
-        out, golden = out.reshape(-1).float(), golden.reshape(-1).float()
+        abs_pass_rate, max_abs_error, cos_sim, kl = None, None, None, None
+
+        out, golden = out.reshape(-1), golden.reshape(-1)
         if 'abs' in precision_type:
             abs_pass_rate, max_abs_error = self.get_abs_pass_rate(out, golden, etol)
         if 'cos_sim' in precision_type:
-            cos_sim_str = self.get_cos_similarity(out, golden)
+            cos_sim, _ = CMP_ALG_MAP["cosine_similarity"](golden, out)
         if 'kl' in precision_type:
-            kl_div = self.get_kl_divergence(out, golden)
-        abs_pass_rate_str = "%.16f" % float(abs_pass_rate.item() * 100) if abs_pass_rate is not None else default_str
-        max_abs_error_str = "%.16f" % float(max_abs_error.item()) if max_abs_error is not None else default_str
-        kl_div_str = "%.16f" % kl_div if kl_div is not None else default_str
+            kl, _ = CMP_ALG_MAP["kl_divergence"](golden, out)
+        abs_pass_rate_str = "%.16f" % float(abs_pass_rate) if abs_pass_rate is not None else default_str
+        max_abs_error_str = "%.16f" % float(max_abs_error) if max_abs_error is not None else default_str
+        cos_sim_str = "%.10f" % cos_sim if cos_sim is not None else default_str
+        kl_div_str = "%.16f" % kl if kl is not None else default_str
 
         return abs_pass_rate_str, max_abs_error_str, cos_sim_str, kl_div_str
-        
+
     def get_npu_device(self):
         npu_device = os.environ.get("NPU_DEVICE")
         if npu_device is None:
             npu_device = "npu:0"
         else:
             npu_device = f"npu:{npu_device}"
         return npu_device
@@ -231,57 +205,56 @@
             soc_version = 'Ascend910B'
         elif re.search("Ascend310P", device_name, re.I):
             soc_version = 'Ascend310P'
         else:
             raise RuntimeError(f"{device_name} is not supported")
         device_count = torch.npu.device_count()
         current_device = torch.npu.current_device()
-        logger_text = "Device Properties: device_name: {}, soc_version: {}, device_count: {}, current_device: {}"\
+        logger_text = "Device Properties: device_name: {}, soc_version: {}, device_count: {}, current_device: {}" \
                     .format(device_name, soc_version, device_count, current_device)
         logger.debug(logger_text)
         return soc_version
 
     def __golden_compare_all(self, out_tensors, golden_out_tensors):
         flag = True
 
         try:
             self.assertEqual(len(out_tensors), len(golden_out_tensors))
-            self.assertEqual(len(out_tensors), len(self.out_dtype))
         except AssertionError as e:
             flag = False
             logger.debug(e)
 
         tensor_count = len(out_tensors)
         for i in range(tensor_count):
-            p_s = self.precision_standard.get(self.out_dtype[i], [])
+            out_dtype = str(out_tensors[i].dtype)
+            p_s = self.precision_standard.get(out_dtype, [])
             if len(p_s) != 2:
-                raise RuntimeError(f"{self.out_dtype[i]} not supported!")
+                raise RuntimeError(f"{out_dtype} not supported!")
             etol = self.erol_dict.get(p_s[0], 0.001)
             err_rate = p_s[1]
             ps_standard = f"{err_rate}%(error<{etol})"
 
-            rel_pass_rate = self.get_rel_pass_rate(out_tensors[i], golden_out_tensors[i], etol)
-            max_rel = self.get_max_rel_error(out_tensors[i], golden_out_tensors[i])
+            rel_pass_rate, max_rel = self.get_rel_pass_rate(out_tensors[i], golden_out_tensors[i], etol)
 
             try:
-                self.assertLess(err_rate, rel_pass_rate * 100)
+                self.assertLess(err_rate, rel_pass_rate)
             except AssertionError as e:
                 flag = False
                 logger.debug(e)
-            
-            rel_pass_rate = "%.16f" % float(rel_pass_rate.item() * 100)
+
+            rel_pass_rate = "%.16f" % float(rel_pass_rate)
             max_rel = "%.16f" % float(max_rel)
             abs_pass_rate, max_abs, cos_sim, kl_div = self.get_other_precisions(out_tensors[i], golden_out_tensors[i], 
                                                                                 etol)
 
             self.case_info['res_detail'].append({"precision_standard": ps_standard,
                                                 "rel_pass_rate": rel_pass_rate,
                                                 "max_rel": max_rel,
                                                 "abs_pass_rate": abs_pass_rate,
                                                 "max_abs": max_abs,
                                                 "cos_sim": cos_sim,
                                                 "kl_div": kl_div})
-            
+
             if flag:
                 self.case_info['excuted_information'] = 'execution successful'
             else:
                 self.case_info['excuted_information'] = 'execution failed'
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/activation.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/activation.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_gather.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/all_reduce.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/as_strided.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/broadcast.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/concat.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/cumsum.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckCumsumOperation(operation_test.OperationTest):
+class OpcheckTransposeOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden_result = torch.cumsum(in_tensors[0], dim=self.op_param['axes'][0])
+        perm = self.op_param["perm"]
+        golden_result = in_tensors[0].permute(perm)
         return [golden_result]
 
-    def test(self):
+    def test_2d_float(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/elewise.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/elewise.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmax.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmaxgrad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/fill.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/gather.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/genattentionmask.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/kv_cache.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/layer_norm.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,66 +8,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import sys
-import json
-import unittest
 import torch
 import torch_npu
-import numpy as np
 
 from ait_llm.opcheck import operation_test
+from ait_llm.common.log import logger
 
 
 class OpcheckLinearOperation(operation_test.OperationTest):
     def golden_flp(self, transpose_a: bool, transpose_b: bool, in_tensor_0, in_tensor_1):
         if transpose_a:
             if len(in_tensor_0.shape) == 2:
-                in_tensor_0 = in_tensor_0.permute(1, 0)
+                in_tensor_0 = torch.permute(in_tensor_0, (1, 0))
             if len(in_tensor_0.shape) == 3:
-                in_tensor_0 = in_tensor_0.permute(0, 2, 1)
+                in_tensor_0 = torch.permute(in_tensor_0, (0, 2, 1))
         if len(in_tensor_1.shape) == 4:
-            in_tensor_1 = in_tensor_1.permute(0, 2, 1, 3)
+            in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1, 3))
             if in_tensor_1.shape[0] == 1:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[1], in_tensor_1.shape[2] * in_tensor_1.shape[3])
             else:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[0], in_tensor_1.shape[1],
                                                   in_tensor_1.shape[2] * in_tensor_1.shape[3])
         if transpose_b:
             if len(in_tensor_1.shape) == 2:
-                in_tensor_1 = in_tensor_1.permute(1, 0)
+                in_tensor_1 = torch.permute(in_tensor_1, (1, 0))
             if len(in_tensor_1.shape) == 3:
-                in_tensor_1 = in_tensor_1.permute(0, 2, 1)
-
-        if self.op_param["linearType"] == 0:
-            golden_result = torch.matmul(in_tensor_0.to(torch.float32), in_tensor_1.to(torch.float32))
-            golden_result = golden_result.to(torch.float16)
-        elif self.op_param["linearType"] == 1:
-            golden_result = torch.matmul(in_tensor_0.to(torch.float32), in_tensor_1.to(torch.float32))
-            golden_result = golden_result.to(torch.bfloat16)
-        else:
-            golden_result = torch.matmul(in_tensor_0.to(torch.int32), in_tensor_1.to(torch.int32))
-
+                in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1))
+        golden_result = torch.matmul(in_tensor_0, in_tensor_1)
         return golden_result
 
     def golden_calc(self, in_tensors):
-        transpose_a = self.op_param["transposeA"]
-        transpose_b = self.op_param["transposeB"]
+        transpose_a = self.op_param.get("transposeA", None)
+        transpose_b = self.op_param.get("transposeB", None)
         golden_result = self.golden_flp(transpose_a, transpose_b, in_tensors[0], in_tensors[1])
-        if self.op_param["hasBias"]:
-            if self.op_param["linearType"] == 0:
-                in_tensors[2] = in_tensors[2].to(torch.float16)
-            elif self.op_param["linearType"] == 1:
-                in_tensors[2] = in_tensors[2].to(torch.bfloat16)
-            else:
-                in_tensors[2] = in_tensors[2].to(torch.int32)
+        has_bias = self.op_param.get("hasBias", False)
+        if has_bias:
             golden_result = golden_result + in_tensors[2]
-        golden_result = torch.tensor(golden_result).half()
-        return [golden_result.npu()]
+        return [golden_result]
 
     def test(self):
-        self.execute()
+        transpose_a = self.op_param.get("transposeA", None)
+        transpose_b = self.op_param.get("transposeB", None)
+        if transpose_a is None or transpose_b is None:
+            msg = "Cannot get golden data because opParam is not correctly set!"
+            logger.error(msg)
+            return
+        self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_parallel.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_quant.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import math
 import os
+import random
 import sys
 import unittest
+
+import numpy as np
 import torch
 import torch_npu
-import numpy as np
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckLinearQuantOperation(operation_test.OperationTest):
+class OpcheckReshapeAndCacheOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden_result = torch.matmul(in_tensors[0].to(torch.int32), in_tensors[1].to(torch.int32))
-        if self.op_param["hasBias"]:
-            golden_result = golden_result + in_tensors[2]
-        golden_result = golden_result * in_tensors[3]
-        golden_result = golden_result.to(torch.float16)
-        return [golden_result.npu()]
+        golden = []
+        for index in self.case_info['inplace_idx']:
+            golden.append(in_tensors[index])
+        return golden
 
     def test(self):
-        self.execute()
+        self.execute_inplace()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/linear_sparse.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/matmul.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/multinomial.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/pad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/paged_attention.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/paged_attention.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reduce.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/repeat.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckRepeatOperation(operation_test.OperationTest):
+class OpcheckAddOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        outtensor = in_tensors[0].repeat(self.op_param["multiples"])
-        return [outtensor]
+        split_output = torch.chunk(in_tensors[0], chunks=self.op_param['splitNum'], dim=self.op_param['splitDim'])
+        return split_output
 
     def test(self):
-        self.execute()
+        self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/reshape_and_cache.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import math
-import os
-import random
 import sys
+import os
 import unittest
-
-import numpy as np
 import torch
 import torch_npu
+import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckReshapeAndCacheOperation(operation_test.OperationTest):
+class OpcheckSoftmaxOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden = []
-        for index in self.case_info['inplace_idx']:
-            golden.append(in_tensors[index])
-        return golden
+        softmax_func = torch.nn.Softmax(dim=self.op_param['axes'][0])
+        return [softmax_func(in_tensors[0])]
 
     def test(self):
-        self.execute_inplace()
+        self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rms_norm.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rms_norm.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/rope_grad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/self_attention.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
-import os
-import unittest
 import json
 import math
 import torch
 import torch_npu
 import numpy as np
 
 from ait_llm.opcheck import operation_test
@@ -29,100 +26,39 @@
     def group_matmul(self, heads, group_num, in_a, in_b):
         try:
             group_head = heads // group_num
         except ZeroDivisionError as e:
             raise e       
         score = None
         for i in range(group_num):
-            group_score = np.matmul(in_a[i * group_head: (i + 1) * group_head, :, :].astype(np.float32),
-                                    in_b[i:(i + 1), :, :].astype(np.float32)).astype(np.float16)
+            group_score = torch.matmul(in_a[i * group_head: (i + 1) * group_head, :, :], in_b[i:(i + 1), :, :])
             if score is None:
                 score = group_score
             else:
-                score = np.concatenate((score, group_score), 0)
+                score = torch.concat((score, group_score), 0)
         logger.debug(score.shape)
         return score
 
-    def encoder_golden_func(self, in_tensors):
-        mixed_q, mixed_k, mixed_v, attention_mask, seq_len = in_tensors[0], in_tensors[1], in_tensors[2], \
-            in_tensors[3], in_tensors[4]
-        
-        if self.op_param["batchRunStatusEnable"]:
-            batch_status = in_tensors[5]
-        else:
-            batch_status = len(seq_len)
-
-        heads, group_num, embed = self.op_param["headNum"], self.op_param["kvHeadNum"], 128
-        q_seqlen = kv_seqlen = seq_len # crossattention时，q_seqlen != k_seqlen 
-        max_s, ntokens2 = np.max(q_seqlen), (q_seqlen * kv_seqlen).sum()
-
-        q_offset, k_offset, v_offset = 0, 0, 0
-        s, _p, out = None, None, None
-
-        for idx, _ in enumerate(range(batch_status)):
-            q_s, kv_s = q_seqlen[idx], kv_seqlen[idx]
-            q_slice = mixed_q[q_offset:q_offset + q_s][:].reshape(q_s, heads, embed)
-            q_slice = np.transpose(q_slice, (1, 0, 2))  # (heads, q_seq, embed)
-            k_slice = mixed_k[k_offset:k_offset + kv_s][:].reshape(kv_s, group_num, embed)
-            k_slice = np.transpose(k_slice, (1, 0, 2))
-            k_slice_t = np.transpose(k_slice, (0, 2, 1))   # get K^T (kv_heads, embed, k_seq)
-            v_slice = mixed_v[v_offset:v_offset + kv_s][:].reshape(kv_s, group_num, embed)
-            v_slice = np.transpose(v_slice, (1, 0, 2))
-            score = self.group_matmul(heads, group_num, q_slice, k_slice_t)
-            s = score.reshape([-1, ]) if s is None else np.concatenate((s, score.reshape([-1, ])), 0)
-            
-            try:
-                score = score * np.float16(1.0 / math.sqrt(1.0 * embed))
-            except ZeroDivisionError as e:
-                raise e
-
-            score = score + attention_mask[:, :q_s, :kv_s] if self.op_param["isTriuMask"] else score
-            score_max = np.max(score, axis=-1)
-            score = score - score_max.reshape((heads, q_s, 1))
-            score_exp = np.exp(score.astype(np.float32))
-            if not self.op_param["isFp32"]:
-                score_sum = np.sum(score_exp.astype(np.float16), axis=-1)
-                _p = score_exp.astype(np.float16).reshape([-1, ]) if _p is None else \
-                    np.concatenate((_p, score_exp.astype(np.float16).reshape([-1, ])), 0)
-                try:
-                    p = score_exp.astype(np.float16) / score_sum.reshape((heads, q_s, 1)).astype(np.float16)
-                except ZeroDivisionError as e:
-                    raise e
-                out_sub = self.group_matmul(heads, group_num, p, v_slice)
-            else:
-                score_sum = np.sum(score_exp, axis=-1)
-                _p = score_exp.astype(np.float16).reshape([-1, ]) if _p is None else \
-                    np.concatenate((_p, score_exp.astype(np.float16).reshape([-1, ])), 0)
-                p = score_exp.astype(np.float16)
-                out_sub = self.group_matmul(heads, group_num, p, v_slice)
-                try:
-                    out_sub = out_sub / score_sum.reshape((heads, q_s, 1)).astype(np.float16)
-                except ZeroDivisionError as e:
-                    raise e
-            out_sub = out_sub.reshape(heads, q_s, embed)
-            out_sub = np.transpose(out_sub, (1, 0, 2))
-            out_sub = np.ascontiguousarray(out_sub)
-            out = out_sub if out is None else np.concatenate((out, out_sub), 0)
-
-        return out.astype("float16").reshape(-1, heads, 128)
-
-    def not_encoder_golden_func(self, in_tensors):
+    def undefined_golden_func(self, in_tensors):
         mixed_q, mixed_k, mixed_v, cache_k, cache_v, attention_mask, token_offset, seq_len, layerid = in_tensors[0], \
             in_tensors[1], in_tensors[2], in_tensors[3], in_tensors[4], in_tensors[5], in_tensors[6], in_tensors[7], \
             int(in_tensors[8][0])
-        if self.op_param["batchRunStatusEnable"]:
+        
+        batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
+        if batch_run_status_enable:
             batch_status = in_tensors[9]
         else:
             batch_status = len(seq_len)
-        q_scale, qk_scale, head_num, head_size = self.op_param["qScale"], self.op_param["qkScale"], \
-            self.op_param["headNum"], self.op_param["headDim"]
+        q_scale, qk_scale, head_num, head_size = self.op_param.get("qScale", 1.0), self.op_param.get("qkScale", 1.0), \
+            self.op_param.get("headNum", 32), mixed_k.size(-1)
+        
         offset = 0
         context_list = []
 
-        for i, _ in enumerate(range(batch_status)):
+        for i in range(batch_status):
             cur_seqlen = seq_len[i]
             cur_token_offset = token_offset[i]
             cur_token_offset_start = cur_token_offset - cur_seqlen
             next_offset = offset + cur_seqlen
             cur_q = mixed_q[offset:next_offset]
             cur_k = mixed_k[offset:next_offset]
             cur_v = mixed_v[offset:next_offset]
@@ -130,57 +66,133 @@
                 past_k = cache_k[layerid, i, :cur_token_offset_start, :]
                 past_v = cache_v[layerid, i, :cur_token_offset_start, :]
                 cur_k = torch.concat([past_k, cur_k], dim=0)
                 cur_v = torch.concat([past_v, cur_v], dim=0)
             cur_q = (cur_q * q_scale).view(cur_seqlen, head_num, head_size).transpose(0, 1)
             cur_k = cur_k.view(cur_token_offset, head_num, head_size).permute(1, 2, 0)
             cur_qk = torch.bmm(cur_q, cur_k) # [head_num, seqlen, token_offset]
-            if self.op_param["isClamp"]:
-                clamp_min = self.op_param["clampMin"]
-                clamp_max = self.op_param["clampMax"]
+            if self.op_param.get("clampType", 0):
+                clamp_min = self.op_param.get("clampMin", 0.0)
+                clamp_max = self.op_param.get("clampMax", 0.0)
                 cur_qk = torch.clamp(cur_qk, clamp_min, clamp_max)
             if attention_mask.ndim == 3: # masked_fill
                 cur_qk = cur_qk + attention_mask[i, :cur_seqlen, :cur_token_offset]
             else:
                 cur_qk = cur_qk + attention_mask[:cur_seqlen, :cur_token_offset]
             cur_qk = cur_qk * qk_scale
-            cur_qk = torch.nn.functional.softmax(cur_qk.type(torch.float32), dim=-1).type(torch.float16)
-
+            cur_qk = torch.nn.functional.softmax(cur_qk, dim=-1)
             cur_v = cur_v.view(cur_token_offset, head_num, head_size).transpose(0, 1)
             cur_context = torch.bmm(cur_qk, cur_v).transpose(0, 1).contiguous().view(cur_seqlen, head_num * head_size)
             context_list.append(cur_context)
 
             offset = next_offset
 
         out = torch.concat(context_list, dim=0)
         return out
 
+    def encoder_golden_func(self, in_tensors):
+        mixed_q, mixed_k, mixed_v, attention_mask, seq_len = in_tensors[0], in_tensors[1], in_tensors[2], \
+            in_tensors[3], in_tensors[4]
+        
+        batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
+        if batch_run_status_enable:
+            batch_status = in_tensors[5]
+        else:
+            batch_status = len(seq_len)
+
+        heads, group_num, embed = self.op_param.get("headNum", 32), self.op_param.get("kvHeadNum", 32), mixed_k.size(-1)
+        q_seqlen = kv_seqlen = seq_len # crossattention时，q_seqlen != k_seqlen
+
+        q_offset, k_offset, v_offset = 0, 0, 0
+        s, _p, out = None, None, None
+
+        for idx in range(batch_status):
+            q_s, kv_s = q_seqlen[idx], kv_seqlen[idx]
+            q_slice = mixed_q[q_offset:q_offset + q_s][:].view(q_s, heads, embed)
+            q_slice = torch.permute(q_slice, (1, 0, 2))  # (heads, q_seq, embed)
+            k_slice = mixed_k[k_offset:k_offset + kv_s][:].view(kv_s, group_num, embed)
+            k_slice = torch.permute(k_slice, (1, 0, 2))
+            k_slice_t = torch.permute(k_slice, (0, 2, 1))   # get K^T (kv_heads, embed, k_seq)
+            v_slice = mixed_v[v_offset:v_offset + kv_s][:].view(kv_s, group_num, embed)
+            v_slice = torch.permute(v_slice, (1, 0, 2))
+            score = self.group_matmul(heads, group_num, q_slice, k_slice_t)
+            s = score.view(-1) if s is None else torch.concat((s, score.view(-1)), 0)
+            
+            score = score / math.sqrt(1.0 * embed)
+            score = score + attention_mask[:, :q_s, :kv_s] if self.op_param.get("isTriuMask", False) else score
+            score_max = torch.max(score, axis=-1)
+            score = score - score_max.view((heads, q_s, 1))
+            score_exp = torch.exp(score)
+            if not self.op_param.get("isFp32", True):
+                score_sum = torch.sum(score_exp, axis=-1)
+                _p = score_exp.view(-1) if _p is None else torch.concat((_p, score_exp.view(-1)), 0)
+                p = score_exp / score_sum.view(heads, q_s, 1)
+                out_sub = self.group_matmul(heads, group_num, p, v_slice)
+            else:
+                score_sum = torch.sum(score_exp, axis=-1)
+                _p = score_exp.view(-1) if _p is None else torch.concat((_p, score_exp.view(-1)), 0)
+                p = score_exp
+                out_sub = self.group_matmul(heads, group_num, p, v_slice)
+                out_sub = out_sub / score_sum.view(heads, q_s, 1)
+            out_sub = out_sub.view(heads, q_s, embed)
+            out_sub = torch.permute(out_sub, (1, 0, 2))
+            out = out_sub if out is None else torch.concat((out, out_sub), 0)
+
+        return out.view(-1, heads, embed)
+
+    def decoder_golden_func(self, in_tensors):
+        return self.undefined_golden_func(in_tensors)
+
+    def pa_encoder_golden_func(self, in_tensors):
+        return self.encoder_golden_func(in_tensors)
+
     def golden_calc(self, in_tensors):
-        if self.op_param["isEncoder"]:
+        calc_type = self.op_param.get("calcType", 0)
+        if calc_type == 0:
+            logger_text = f"CalcType: {calc_type}. Undefined calcType!"
+            logger.debug(logger_text)
+            out = self.undefined_golden_func(in_tensors)
+        elif calc_type == 1:
+            logger_text = f"CalcType: {calc_type}. Using encoder of FlashAttention!"
+            logger.debug(logger_text)
             out = self.encoder_golden_func(in_tensors)
+        elif calc_type == 2:
+            logger_text = f"CalcType: {calc_type}. Using decoder of FlashAttention!"
+            logger.debug(logger_text)
+            out = self.decoder_golden_func(in_tensors)
         else:
-            out = self.not_encoder_golden_func(in_tensors)
+            logger_text = f"CalcType: {calc_type}. Using encoder of PageAttention!"
+            logger.debug(logger_text)
+            out = self.pa_encoder_golden_func(in_tensors)
         return [out]
 
     def test(self):
         soc_version = self.get_soc_version()
         if soc_version != 'Ascend910B':
-            logger_text = "{} is not supported! Only supports Ascend910B!".format(soc_version)
+            logger_text = f"{soc_version} is not supported! Only supports Ascend910B!"
             logger.error(logger_text)
             return
+        
+        batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
 
-        if self.op_param["isEncoder"]:
-            if self.op_param["batchRunStatusEnable"]:
+        if len(self.in_tensors) <= 6:
+            if batch_run_status_enable:
+                batch_run_status = self.in_tensors[5].tolist()
+                logger_text = f"Enabling batchRunStatus: {batch_run_status}"
+                logger.debug(logger_text)
                 self.case_info["run_param"] = json.dumps({"seqLen": self.in_tensors[4].tolist(),
-                                                        "batchRunStatus": self.in_tensors[5].tolist()})
+                                                        "batchRunStatus": batch_run_status})
             else:
                 self.case_info["run_param"] = json.dumps({"seqLen": self.in_tensors[4].tolist()})
         else:
-            if self.op_param["batchRunStatusEnable"]:
-                self.case_info['run_param'] = json.dumps({"tokenOffset": self.in_tensors[6].tolist(), 
+            if batch_run_status_enable:
+                batch_run_status = self.in_tensors[9].tolist()
+                logger_text = f"Enabling batchRunStatus: {batch_run_status}"
+                logger.debug(logger_text)
+                self.case_info['run_param'] = json.dumps({"tokenOffset": self.in_tensors[6].tolist(),
                                                         "seqLen": self.in_tensors[7].tolist(),
-                                                        "batchRunStatus": self.in_tensors[9].tolist()})
+                                                        "batchRunStatus": batch_run_status})
             else:
-                self.case_info["run_param"] = json.dumps({"tokenOffset": self.in_tensors[6].tolist(), 
+                self.case_info["run_param"] = json.dumps({"tokenOffset": self.in_tensors[6].tolist(),
                                                         "seqLen": self.in_tensors[7].tolist()})
 
         self.execute_with_param()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/set_value.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/slice.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/softmax.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 import os
+import json
 import unittest
 import torch
 import torch_npu
 import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckSoftmaxOperation(operation_test.OperationTest):
+class OpcheckSortOperation(operation_test.OperationTest):    
     def golden_calc(self, in_tensors):
-        softmax_func = torch.nn.Softmax(dim=self.op_param['axes'][0])
-        return [softmax_func(in_tensors[0])]
+        values, indices = torch.topk(in_tensors[0], k=self.op_param["num"][0], largest=True)
+        return [values, indices.int()]
 
-    def test(self):
+    def test_3d_float(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/sort.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 import os
-import json
 import unittest
 import torch
 import torch_npu
-import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckSortOperation(operation_test.OperationTest):    
+class OpcheckWhereOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        values, indices = torch.topk(in_tensors[0], k=self.op_param["num"][0], largest=True)
-        return [values, indices.int()]
+        golden_result = torch.where(in_tensors[0].bool(), in_tensors[1], in_tensors[2])
+        return [golden_result]
 
-    def test_3d_float(self):
+    def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/split.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
-import os
-import unittest
-import torch
-import torch_npu
-
-from ait_llm.opcheck import operation_test
-
-
-class OpcheckAddOperation(operation_test.OperationTest):
-    def golden_calc(self, in_tensors):
-        split_output = torch.chunk(in_tensors[0], chunks=self.op_param['splitNum'], dim=self.op_param['splitDim'])
-        return split_output
+import logging
+
+logging.raiseExceptions = False
+
+
+class Scanner:
+    """
+    Scanner类作为扫描器的基类存在，仅定义必要的属性和方法接口。
+    """
+    __slots__ = ['files', 'porting_results', 'name', 'pool_numbers']
+
+    def __init__(self, files):
+        self.files = files
+        self.porting_results = {}
 
-    def test(self):
-        self.execute()
+    def do_scan(self):
+        raise NotImplementedError('{} must implement do_scan method!'.format(self.__class__))
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/stridebatchmatmul.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/topk_topp_sampling.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transdata.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/transpose.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
-import os
-import unittest
-import torch
-import torch_npu
-
-from ait_llm.opcheck import operation_test
-
-
-class OpcheckTransposeOperation(operation_test.OperationTest):
-    def golden_calc(self, in_tensors):
-        perm = self.op_param["perm"]
-        golden_result = in_tensors[0].permute(perm)
-        return [golden_result]
+from enum import Enum
 
-    def test_2d_float(self):
-        self.execute()
+
+class Arg(object):
+    def __init__(self, benchmark_arg, atc_arg, msquickcmp_arg):
+        self.atc_arg = atc_arg
+        self.benchmark_arg = benchmark_arg
+        self.msquickcmp_arg = msquickcmp_arg
+
+
+class DynamicArgumentEnum(Enum):
+    # enum struct Arg(benchmark_arg, atc_arg, msquickcmp_arg)
+    DYM_BATCH = Arg("--dymBatch", "--dynamic_batch_size", None)
+    DYM_SHAPE = Arg("--dymShape", "--input_shape_range", "input_shape")
+    DYM_DIMS = Arg("--dymDims", "--dynamic_dims", "input_shape")
+
+    @staticmethod
+    def get_all_args() -> list:
+        """
+        get all argument enum, return as a list
+        """
+        return list(map(lambda arg: arg, DynamicArgumentEnum))
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/unpad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/opcheck/opcheck_checkcases/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,57 +8,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ait_llm.opcheck.opcheck_checkcases.activation import OpcheckActivationOperation
-from ait_llm.opcheck.opcheck_checkcases.all_gather import OpcheckAllGatherOperation
-from ait_llm.opcheck.opcheck_checkcases.all_reduce import OpcheckAllReduceOperation
-from ait_llm.opcheck.opcheck_checkcases.broadcast import OpcheckBroadcastOperation
-from ait_llm.opcheck.opcheck_checkcases.concat import OpcheckConcatOperation
-from ait_llm.opcheck.opcheck_checkcases.cumsum import OpcheckCumsumOperation
-from ait_llm.opcheck.opcheck_checkcases.elewise import OpcheckElewiseAddOperation
-from ait_llm.opcheck.opcheck_checkcases.fastsoftmax import OpcheckFastSoftMaxOperation
-from ait_llm.opcheck.opcheck_checkcases.fastsoftmaxgrad import OpcheckFastSoftMaxGradOperation
-from ait_llm.opcheck.opcheck_checkcases.fill import OpcheckFillOperation
-from ait_llm.opcheck.opcheck_checkcases.gather import OpcheckGatherOperation
-from ait_llm.opcheck.opcheck_checkcases.genattentionmask import OpcheckElewiseSubOperation
-from ait_llm.opcheck.opcheck_checkcases.kv_cache import OpcheckKvCacheOperation
-from ait_llm.opcheck.opcheck_checkcases.linear_activation import OpcheckLinearActivationOperation
-from ait_llm.opcheck.opcheck_checkcases.linear import OpcheckLinearOperation
-from ait_llm.opcheck.opcheck_checkcases.linear_activation_quant import OpcheckLinearActivationQuantOperation
-from ait_llm.opcheck.opcheck_checkcases.linear_quant import OpcheckLinearQuantOperation
-from ait_llm.opcheck.opcheck_checkcases.linear_sparse import OpcheckLinearSparseOperation
-from ait_llm.opcheck.opcheck_checkcases.matmul import OpcheckMatmulOperation
-from ait_llm.opcheck.opcheck_checkcases.pad import OpcheckPadOperation
-from ait_llm.opcheck.opcheck_checkcases.paged_attention import OpcheckPagedAttentionAttentionOperation
-from ait_llm.opcheck.opcheck_checkcases.repeat import OpcheckRepeatOperation
-from ait_llm.opcheck.opcheck_checkcases.reshape_and_cache import OpcheckReshapeAndCacheOperation
-from ait_llm.opcheck.opcheck_checkcases.rms_norm import OpcheckRmsNormOperation
-from ait_llm.opcheck.opcheck_checkcases.rope_grad import OpcheckRopeGradOperation
-from ait_llm.opcheck.opcheck_checkcases.rope import OpcheckUnpadRopeOperation
-from ait_llm.opcheck.opcheck_checkcases.self_attention import OpcheckUnpadSelfAttentionOperation
-from ait_llm.opcheck.opcheck_checkcases.set_value import OpcheckSetValueOperation
-from ait_llm.opcheck.opcheck_checkcases.slice import OpcheckSliceOperation
-from ait_llm.opcheck.opcheck_checkcases.softmax import OpcheckSoftmaxOperation
-from ait_llm.opcheck.opcheck_checkcases.sort import OpcheckSortOperation
-from ait_llm.opcheck.opcheck_checkcases.split import OpcheckAddOperation
-from ait_llm.opcheck.opcheck_checkcases.stridebatchmatmul import OpcheckStridedBatchMatmulOperation
-from ait_llm.opcheck.opcheck_checkcases.topk_topp_sampling import OpcheckToppOperation
-from ait_llm.opcheck.opcheck_checkcases.transpose import OpcheckTransposeOperation
-from ait_llm.opcheck.opcheck_checkcases.unpad import OpcheckUnpadOperation
-from ait_llm.opcheck.opcheck_checkcases.as_strided import OpcheckAsStridedOperation
-from ait_llm.opcheck.opcheck_checkcases.layer_norm import OpcheckLayerNormOperation
-from ait_llm.opcheck.opcheck_checkcases.linear_parallel import OpcheckLinearParallelOperation
-from ait_llm.opcheck.opcheck_checkcases.multinomial import OpcheckMultinomialOperation
-from ait_llm.opcheck.opcheck_checkcases.reduce import OpcheckReduceOperation
-from ait_llm.opcheck.opcheck_checkcases.transdata import OpcheckTransdataOperation
-from ait_llm.opcheck.opcheck_checkcases.where import OpcheckWhereOperation
+from ait_llm.opcheck.check_case.activation import OpcheckActivationOperation
+from ait_llm.opcheck.check_case.all_gather import OpcheckAllGatherOperation
+from ait_llm.opcheck.check_case.all_reduce import OpcheckAllReduceOperation
+from ait_llm.opcheck.check_case.broadcast import OpcheckBroadcastOperation
+from ait_llm.opcheck.check_case.concat import OpcheckConcatOperation
+from ait_llm.opcheck.check_case.cumsum import OpcheckCumsumOperation
+from ait_llm.opcheck.check_case.elewise import OpcheckElewiseAddOperation
+from ait_llm.opcheck.check_case.fastsoftmax import OpcheckFastSoftMaxOperation
+from ait_llm.opcheck.check_case.fastsoftmaxgrad import OpcheckFastSoftMaxGradOperation
+from ait_llm.opcheck.check_case.fill import OpcheckFillOperation
+from ait_llm.opcheck.check_case.gather import OpcheckGatherOperation
+from ait_llm.opcheck.check_case.genattentionmask import OpcheckElewiseSubOperation
+from ait_llm.opcheck.check_case.kv_cache import OpcheckKvCacheOperation
+from ait_llm.opcheck.check_case.linear import OpcheckLinearOperation
+from ait_llm.opcheck.check_case.linear_sparse import OpcheckLinearSparseOperation
+from ait_llm.opcheck.check_case.matmul import OpcheckMatmulOperation
+from ait_llm.opcheck.check_case.pad import OpcheckPadOperation
+from ait_llm.opcheck.check_case.paged_attention import OpcheckPagedAttentionAttentionOperation
+from ait_llm.opcheck.check_case.repeat import OpcheckRepeatOperation
+from ait_llm.opcheck.check_case.reshape_and_cache import OpcheckReshapeAndCacheOperation
+from ait_llm.opcheck.check_case.rms_norm import OpcheckRmsNormOperation
+from ait_llm.opcheck.check_case.rope_grad import OpcheckRopeGradOperation
+from ait_llm.opcheck.check_case.rope import OpcheckUnpadRopeOperation
+from ait_llm.opcheck.check_case.self_attention import OpcheckUnpadSelfAttentionOperation
+from ait_llm.opcheck.check_case.set_value import OpcheckSetValueOperation
+from ait_llm.opcheck.check_case.slice import OpcheckSliceOperation
+from ait_llm.opcheck.check_case.softmax import OpcheckSoftmaxOperation
+from ait_llm.opcheck.check_case.sort import OpcheckSortOperation
+from ait_llm.opcheck.check_case.split import OpcheckAddOperation
+from ait_llm.opcheck.check_case.stridebatchmatmul import OpcheckStridedBatchMatmulOperation
+from ait_llm.opcheck.check_case.topk_topp_sampling import OpcheckToppOperation
+from ait_llm.opcheck.check_case.transpose import OpcheckTransposeOperation
+from ait_llm.opcheck.check_case.unpad import OpcheckUnpadOperation
+from ait_llm.opcheck.check_case.as_strided import OpcheckAsStridedOperation
+from ait_llm.opcheck.check_case.layer_norm import OpcheckLayerNormOperation
+from ait_llm.opcheck.check_case.linear_parallel import OpcheckLinearParallelOperation
+from ait_llm.opcheck.check_case.multinomial import OpcheckMultinomialOperation
+from ait_llm.opcheck.check_case.reduce import OpcheckReduceOperation
+from ait_llm.opcheck.check_case.transdata import OpcheckTransdataOperation
+from ait_llm.opcheck.check_case.where import OpcheckWhereOperation
 
 
 OP_NAME_DICT = dict({
     "ActivationOperation":OpcheckActivationOperation,
     "AllGatherOperation":OpcheckAllGatherOperation,
     "AllReduceOperation":OpcheckAllReduceOperation,
     "BroadcastOperation":OpcheckBroadcastOperation,
@@ -68,17 +65,14 @@
     "FastSoftMaxOperation":OpcheckFastSoftMaxOperation,
     "FastSoftMaxGradOperation":OpcheckFastSoftMaxGradOperation,
     "FillOperation":OpcheckFillOperation,
     "GatherOperation":OpcheckGatherOperation,
     "GenAttentionMaskOperation":OpcheckElewiseSubOperation,
     "KvCacheOperation":OpcheckKvCacheOperation,
     "LinearOperation":OpcheckLinearOperation,
-    "LinearActivationOperation":OpcheckLinearActivationOperation,
-    "LinearActivationQuantOperation":OpcheckLinearActivationQuantOperation,
-    "LinearQuantOperation":OpcheckLinearQuantOperation,
     "LinearSparseOperation":OpcheckLinearSparseOperation,
     "MatmulOperation":OpcheckMatmulOperation,
     "PadOperation":OpcheckPadOperation,
     "PagedAttentionOperation":OpcheckPagedAttentionAttentionOperation,
     "RepeatOperation":OpcheckRepeatOperation,
     "ReshapeAndCacheOperation":OpcheckReshapeAndCacheOperation,
     "RmsNormOperation":OpcheckRmsNormOperation,
```

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/llm/ait_llm/transform/utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/setup.py` & `ms-ait-7.0.0rc2/components/convert/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+# http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages  # type: ignore
 
+
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
-with open('README.md', encoding='utf-8') as f:
-    long_description = f.read()
+ait_sub_tasks = [{
+    "name": "convert",
+    "help_info": "convert tool converts the model from ONNX, TensorFlow, Caffe and MindSpore to OM. \
+                   It supports atc, aoe and aie.",
+    "module": "model_convert.__main__",
+    "attr": "get_cmd_instance"
+}]
+
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
-    name='transplt',
-    version='0.1.0',
-    description='app analyze for cpu and gpu projects',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    name='ait-convert',
+    version='7.0.0c2',
+    description='model convert tool',
     url='https://gitee.com/ascend/ait',
     packages=find_packages(),
+    package_data={'': ['LICENSE', 'README.md', 'requirements.txt', 'install.bat', 'install.sh', '*.cpp', '*.h']},
     license='Apache-2.0',
-    keywords='app_analyze',
+    keywords='convert tool',
     install_requires=required,
     classifiers=[
         'Development Status :: Alpha',
         'Intended Audience :: Developers',
         'License :: Apache-2.0 Software License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
     ],
     python_requires='>=3.7',
     entry_points={
-        'transplt_sub_task': ['transplt=app_analyze.__main__:get_cmd_instance'],
+        'ait_sub_task': ait_sub_task_entry_points,
+        'ait_sub_task_installer': ['ait-convert=model_convert.__install__:ConvertInstall'],
     },
-)
+)
```

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/__main__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/common/kit_config.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/common/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/exception/exception_information.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/exception/source_scan_exception.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/exception/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/model/model.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/model/project.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/model/seq_project.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/model/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/app.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/cmdline_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/custom_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/input_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/porting_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/porting/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/report/csv_report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/report/json_report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/report/report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/report/report_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/report/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/clang_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cmake_scanner.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/cxx_scanner.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/func_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/python_scanner.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scanner_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/scan_api.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/comment_delete.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/file_matrix.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/module/__init__.py` & `ms-ait-7.0.0rc2/components/benchmark/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/acc_libs.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/api_filter.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/ast_visitor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_desc.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_handler.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_matcher.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/scan/sequence/seq_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/solution/advisor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/solution/seq_advisor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/solution/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/clang_finder.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/excel.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/file_locker.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/io_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/lib_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/log_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/security.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/transplt/app_analyze/utils/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/utils/file_open_check.py` & `ms-ait-7.0.0rc2/components/utils/file_open_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/utils/security_check.py` & `ms-ait-7.0.0rc2/components/utils/security_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/components/utils/__init__.py` & `ms-ait-7.0.0rc2/components/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0a4/ms_ait.egg-info/SOURCES.txt` & `ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 README.md
 requirements.txt
 setup.py
 components/__init__.py
 components/__main__.py
+components/analyze/README.md
 components/analyze/__init__.py
 components/analyze/requirements.txt
 components/analyze/setup.py
 components/analyze/model_evaluation/__init__.py
+components/analyze/model_evaluation/__install__.py
 components/analyze/model_evaluation/__main__.py
 components/analyze/model_evaluation/bean/__init__.py
 components/analyze/model_evaluation/bean/config.py
 components/analyze/model_evaluation/bean/op_info.py
 components/analyze/model_evaluation/common/__init__.py
 components/analyze/model_evaluation/common/const.py
 components/analyze/model_evaluation/common/log.py
@@ -32,20 +34,25 @@
 components/analyze/model_evaluation/data/opp.py
 components/analyze/model_evaluation/graph/__init__.py
 components/analyze/model_evaluation/graph/onnx.py
 components/analyze/model_evaluation/parser/__init__.py
 components/analyze/model_evaluation/parser/atc.py
 components/analyze/model_evaluation/parser/model.py
 components/analyze/model_evaluation/parser/om.py
+components/benchmark/README.md
 components/benchmark/__init__.py
 components/benchmark/ais_infer.py
+components/benchmark/install.sh
 components/benchmark/requirements.txt
 components/benchmark/setup.py
 components/benchmark/ais_bench/__init__.py
+components/benchmark/ais_bench/__install__.py
 components/benchmark/ais_bench/__main__.py
+components/benchmark/ais_bench/install.sh
+components/benchmark/ais_bench/evaluate/README.md
 components/benchmark/ais_bench/evaluate/__init__.py
 components/benchmark/ais_bench/evaluate/interface.py
 components/benchmark/ais_bench/evaluate/log.py
 components/benchmark/ais_bench/evaluate/recorder.py
 components/benchmark/ais_bench/evaluate/dataset/__init__.py
 components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
 components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
@@ -68,59 +75,108 @@
 components/benchmark/ais_bench/infer/registry.py
 components/benchmark/ais_bench/infer/summary.py
 components/benchmark/ais_bench/infer/utils.py
 components/benchmark/ais_bench/infer/backends/__init__.py
 components/benchmark/ais_bench/infer/backends/backend.py
 components/benchmark/ais_bench/infer/backends/backend_trtexec.py
 components/benchmark/backend/__init__.py
+components/benchmark/backend/install.sh
 components/benchmark/backend/setup.py
 components/benchmark/infer_analyser/__init__.py
 components/benchmark/infer_analyser/analyser.py
 components/benchmark/infer_analyser/info_convert_json.py
+components/convert/README.md
 components/convert/__init__.py
 components/convert/requirements.txt
 components/convert/setup.py
-components/convert/convert_scripts/__init__.py
 components/convert/model_convert/__init__.py
+components/convert/model_convert/__install__.py
 components/convert/model_convert/__main__.py
 components/convert/model_convert/cmd_utils.py
+components/convert/model_convert/install.sh
 components/convert/model_convert/aie/__init__.py
 components/convert/model_convert/aie/bean/__init__.py
 components/convert/model_convert/aie/bean/config.py
 components/convert/model_convert/aie/core/__init__.py
 components/convert/model_convert/aie/core/convert.py
 components/convert/model_convert/aoe/__init__.py
 components/convert/model_convert/aoe/aoe_args_map.py
 components/convert/model_convert/atc/__init__.py
 components/convert/model_convert/atc/atc_args_map.py
 components/debug/__init__.py
+components/debug/compare/README.md
+components/debug/compare/__init__.py
+components/debug/compare/main.py
+components/debug/compare/requirements.txt
+components/debug/compare/setup.py
+components/debug/compare/msquickcmp/__init__.py
+components/debug/compare/msquickcmp/__install__.py
+components/debug/compare/msquickcmp/__main__.py
+components/debug/compare/msquickcmp/cmp_process.py
+components/debug/compare/msquickcmp/install.sh
+components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+components/debug/compare/msquickcmp/tf_debug_runner.py
+components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+components/debug/compare/msquickcmp/adapter_cli/__init__.py
+components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+components/debug/compare/msquickcmp/atc/__init__.py
+components/debug/compare/msquickcmp/atc/atc_utils.py
+components/debug/compare/msquickcmp/caffe_model/__init__.py
+components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+components/debug/compare/msquickcmp/common/__init__.py
+components/debug/compare/msquickcmp/common/args_check.py
+components/debug/compare/msquickcmp/common/convert.py
+components/debug/compare/msquickcmp/common/dump_data.py
+components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+components/debug/compare/msquickcmp/common/tf_common.py
+components/debug/compare/msquickcmp/common/utils.py
+components/debug/compare/msquickcmp/net_compare/__init__.py
+components/debug/compare/msquickcmp/net_compare/analyser.py
+components/debug/compare/msquickcmp/net_compare/net_compare.py
+components/debug/compare/msquickcmp/npu/__init__.py
+components/debug/compare/msquickcmp/npu/npu_dump_data.py
+components/debug/compare/msquickcmp/npu/om_parser.py
+components/debug/compare/msquickcmp/onnx_model/__init__.py
+components/debug/compare/msquickcmp/onnx_model/custom_op.py
+components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+components/debug/compare/msquickcmp/save_om_model/__init__.py
+components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+components/debug/compare/msquickcmp/single_op/__init__.py
+components/debug/compare/msquickcmp/single_op/single_op.py
+components/debug/compare/msquickcmp/tf/__init__.py
+components/debug/compare/msquickcmp/tf/tf_dump_data.py
+components/debug/surgeon/README.md
 components/debug/surgeon/__init__.py
 components/debug/surgeon/requirements.txt
 components/debug/surgeon/setup.py
 components/debug/surgeon/auto_optimizer/__init__.py
+components/debug/surgeon/auto_optimizer/__install__.py
 components/debug/surgeon/auto_optimizer/__main__.py
 components/debug/surgeon/auto_optimizer/ait_main.py
 components/debug/surgeon/auto_optimizer/options.py
 components/debug/surgeon/auto_optimizer/common/__init__.py
 components/debug/surgeon/auto_optimizer/common/args_check.py
 components/debug/surgeon/auto_optimizer/common/click_utils.py
 components/debug/surgeon/auto_optimizer/common/config.py
 components/debug/surgeon/auto_optimizer/common/log.py
 components/debug/surgeon/auto_optimizer/common/register.py
 components/debug/surgeon/auto_optimizer/common/singleton.py
 components/debug/surgeon/auto_optimizer/common/utils.py
 components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
 components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+components/debug/surgeon/auto_optimizer/graph_refactor/README.md
 components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
 components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
 components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
 components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
 components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
 components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
 components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+components/debug/surgeon/auto_optimizer/inference_engine/README.md
 components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
 components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
 components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
 components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
 components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
 components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
 components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
@@ -175,28 +231,33 @@
 components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
 components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+components/debug/surgeon/auto_optimizer/tools/README.md
 components/debug/surgeon/auto_optimizer/tools/__init__.py
 components/debug/surgeon/auto_optimizer/tools/inference.py
 components/debug/surgeon/auto_optimizer/tools/log.py
+components/llm/README.md
 components/llm/__init__.py
 components/llm/requirements.txt
 components/llm/setup.py
 components/llm/ait_llm/__init__.py
+components/llm/ait_llm/__install__.py
 components/llm/ait_llm/__main__.py
+components/llm/ait_llm/install.sh
 components/llm/ait_llm/common/__init__.py
 components/llm/ait_llm/common/constant.py
 components/llm/ait_llm/common/json_fitter.py
 components/llm/ait_llm/common/log.py
 components/llm/ait_llm/common/tool.py
 components/llm/ait_llm/common/utils.py
+components/llm/ait_llm/common/validate.py
 components/llm/ait_llm/compare/__init__.py
 components/llm/ait_llm/compare/atb_acc_cmp.py
 components/llm/ait_llm/compare/cmp_algorithm.py
 components/llm/ait_llm/compare/cmp_utils.py
 components/llm/ait_llm/compare/op_mapping.py
 components/llm/ait_llm/compare/torchair_acc_cmp.py
 components/llm/ait_llm/dump/__init__.py
@@ -207,74 +268,96 @@
 components/llm/ait_llm/dump/torch_dump/dump_hook.py
 components/llm/ait_llm/dump/torch_dump/hook.py
 components/llm/ait_llm/dump/torch_dump/hook_ops.py
 components/llm/ait_llm/dump/torch_dump/topo.py
 components/llm/ait_llm/dump/torchair_dump/__init__.py
 components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
 components/llm/ait_llm/errcheck/__init__.py
-components/llm/ait_llm/errcheck/initial.py
+components/llm/ait_llm/errcheck/process.py
+components/llm/ait_llm/metrics/__init__.py
+components/llm/ait_llm/metrics/case_filter.py
+components/llm/ait_llm/metrics/metrics.py
 components/llm/ait_llm/opcheck/__init__.py
 components/llm/ait_llm/opcheck/case_manager.py
 components/llm/ait_llm/opcheck/opchecker.py
 components/llm/ait_llm/opcheck/operation_test.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/__init__.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/activation.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/all_gather.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/all_reduce.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/as_strided.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/broadcast.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/concat.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/cumsum.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/elewise.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmax.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/fastsoftmaxgrad.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/fill.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/gather.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/genattentionmask.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/kv_cache.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/layer_norm.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear_activation_quant.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear_parallel.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear_quant.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/linear_sparse.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/matmul.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/multinomial.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/pad.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/paged_attention.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/reduce.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/repeat.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/reshape_and_cache.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/rms_norm.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/rope.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/rope_grad.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/self_attention.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/set_value.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/slice.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/softmax.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/sort.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/split.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/stridebatchmatmul.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/topk_topp_sampling.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/transdata.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/transpose.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/unpad.py
-components/llm/ait_llm/opcheck/opcheck_checkcases/where.py
+components/llm/ait_llm/opcheck/atb_operators/__init__.py
+components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+components/llm/ait_llm/opcheck/check_case/__init__.py
+components/llm/ait_llm/opcheck/check_case/activation.py
+components/llm/ait_llm/opcheck/check_case/all_gather.py
+components/llm/ait_llm/opcheck/check_case/all_reduce.py
+components/llm/ait_llm/opcheck/check_case/as_strided.py
+components/llm/ait_llm/opcheck/check_case/broadcast.py
+components/llm/ait_llm/opcheck/check_case/concat.py
+components/llm/ait_llm/opcheck/check_case/cumsum.py
+components/llm/ait_llm/opcheck/check_case/elewise.py
+components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+components/llm/ait_llm/opcheck/check_case/fill.py
+components/llm/ait_llm/opcheck/check_case/gather.py
+components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+components/llm/ait_llm/opcheck/check_case/kv_cache.py
+components/llm/ait_llm/opcheck/check_case/layer_norm.py
+components/llm/ait_llm/opcheck/check_case/linear.py
+components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+components/llm/ait_llm/opcheck/check_case/matmul.py
+components/llm/ait_llm/opcheck/check_case/multinomial.py
+components/llm/ait_llm/opcheck/check_case/pad.py
+components/llm/ait_llm/opcheck/check_case/paged_attention.py
+components/llm/ait_llm/opcheck/check_case/reduce.py
+components/llm/ait_llm/opcheck/check_case/repeat.py
+components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+components/llm/ait_llm/opcheck/check_case/rms_norm.py
+components/llm/ait_llm/opcheck/check_case/rope.py
+components/llm/ait_llm/opcheck/check_case/rope_grad.py
+components/llm/ait_llm/opcheck/check_case/self_attention.py
+components/llm/ait_llm/opcheck/check_case/set_value.py
+components/llm/ait_llm/opcheck/check_case/slice.py
+components/llm/ait_llm/opcheck/check_case/softmax.py
+components/llm/ait_llm/opcheck/check_case/sort.py
+components/llm/ait_llm/opcheck/check_case/split.py
+components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+components/llm/ait_llm/opcheck/check_case/transdata.py
+components/llm/ait_llm/opcheck/check_case/transpose.py
+components/llm/ait_llm/opcheck/check_case/unpad.py
+components/llm/ait_llm/opcheck/check_case/where.py
 components/llm/ait_llm/transform/__init__.py
 components/llm/ait_llm/transform/transform_quant.py
 components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
 components/llm/ait_llm/transform/utils.py
 components/profile/__init__.py
+components/profile/msprof/README.md
+components/profile/msprof/__init__.py
+components/profile/msprof/install.sh
+components/profile/msprof/requirements.txt
+components/profile/msprof/setup.py
+components/profile/msprof/ait_prof/__init__.py
+components/profile/msprof/ait_prof/__install__.py
+components/profile/msprof/ait_prof/__main__.py
+components/profile/msprof/ait_prof/api.py
+components/profile/msprof/ait_prof/args_adapter.py
+components/profile/msprof/ait_prof/main_cli.py
+components/profile/msprof/ait_prof/msprof_process.py
+components/profile/msprof/ait_prof/utils.py
 components/tests/__init__.py
+components/transplt/README.md
 components/transplt/__init__.py
+components/transplt/install.bat
+components/transplt/install.sh
 components/transplt/requirements.txt
 components/transplt/setup.py
 components/transplt/app_analyze/__init__.py
+components/transplt/app_analyze/__install__.py
 components/transplt/app_analyze/__main__.py
+components/transplt/app_analyze/install.bat
+components/transplt/app_analyze/install.sh
 components/transplt/app_analyze/common/__init__.py
 components/transplt/app_analyze/common/kit_config.py
 components/transplt/app_analyze/exception/__init__.py
 components/transplt/app_analyze/exception/exception_information.py
 components/transplt/app_analyze/exception/source_scan_exception.py
 components/transplt/app_analyze/model/__init__.py
 components/transplt/app_analyze/model/model.py
@@ -323,15 +406,16 @@
 components/transplt/app_analyze/utils/file_locker.py
 components/transplt/app_analyze/utils/io_util.py
 components/transplt/app_analyze/utils/lib_util.py
 components/transplt/app_analyze/utils/log_util.py
 components/transplt/app_analyze/utils/security.py
 components/utils/__init__.py
 components/utils/file_open_check.py
+components/utils/install.py
 components/utils/parser.py
 components/utils/security_check.py
+components/utils/util.py
 ms_ait.egg-info/PKG-INFO
 ms_ait.egg-info/SOURCES.txt
 ms_ait.egg-info/dependency_links.txt
 ms_ait.egg-info/entry_points.txt
-ms_ait.egg-info/requires.txt
 ms_ait.egg-info/top_level.txt
```

