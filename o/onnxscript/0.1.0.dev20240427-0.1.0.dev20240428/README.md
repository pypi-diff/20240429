# Comparing `tmp/onnxscript-0.1.0.dev20240427.tar.gz` & `tmp/onnxscript-0.1.0.dev20240428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240427.tar", last modified: Sat Apr 27 00:02:12 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240428.tar", last modified: Sun Apr 28 00:00:50 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240427.tar` & `onnxscript-0.1.0.dev20240428.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.032933 onnxscript-0.1.0.dev20240427/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.996933 onnxscript-0.1.0.dev20240427/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.000933 onnxscript-0.1.0.dev20240427/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.004933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:11.992933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.012933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.016933 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.016933 onnxscript-0.1.0.dev20240427/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.020933 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.024933 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.024933 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24160 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-27 00:02:12.028933 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-27 00:02:11.000000 onnxscript-0.1.0.dev20240427/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-27 00:02:12.032933 onnxscript-0.1.0.dev20240427/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-27 00:00:56.000000 onnxscript-0.1.0.dev20240427/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.943124 onnxscript-0.1.0.dev20240428/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.947124 onnxscript-0.1.0.dev20240428/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.947124 onnxscript-0.1.0.dev20240428/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.947124 onnxscript-0.1.0.dev20240428/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.947124 onnxscript-0.1.0.dev20240428/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.939124 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.947124 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.955124 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.939124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.939124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.955124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.955124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.955124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.955124 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.959124 onnxscript-0.1.0.dev20240428/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.959124 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.963124 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.963124 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-28 00:00:50.000000 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-28 00:00:50.000000 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-28 00:00:50.000000 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-28 00:00:50.000000 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-28 00:00:50.000000 onnxscript-0.1.0.dev20240428/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-28 00:00:50.967124 onnxscript-0.1.0.dev20240428/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-28 00:00:34.000000 onnxscript-0.1.0.dev20240428/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240427/LICENSE` & `onnxscript-0.1.0.dev20240428/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/PKG-INFO` & `onnxscript-0.1.0.dev20240428/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240427
+Version: 0.1.0.dev20240428
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240427/README.md` & `onnxscript-0.1.0.dev20240428/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240428/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240428/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240428/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240428/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240428/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240428/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240428/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240428/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/main.py` & `onnxscript-0.1.0.dev20240428/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240428/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240428/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,12 @@
     multihead_attention,
 )
 
 TRANSFORMERS_FUNCTION_REWRITE_RULES: list[type[function_rule.FunctionRewriteRule]] = [
     multihead_attention.GQALlama2RewriteRule,
     multihead_attention.GQALlamaSdpa2RewriteRule,
     multihead_attention.AttnPhi15RewriteRule,
+    multihead_attention.MHAStableDiffusionUnetRewriteRule,
     layernorm.LNRewriteRule,
     fastgelu.GeluRewriteRule,
     biassplitgelu.GegluRewriteRule,
 ]
```

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,63 +51,98 @@
 import logging
 
 import onnx
 from onnx import helper as onnx_helper
 
 import onnxscript
 from onnxscript import ir
-from onnxscript.rewriter import function_rule
+from onnxscript.rewriter import _ir_utils, function_rule
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class AttnSizeConfig:
     num_attention_heads: int
-    num_key_value_heads: int
+    num_key_value_heads: int | None
     head_size: int
     hidden_size: int
 
 
 class AttentionRewriteRule(function_rule.FunctionRewriteRule, abc.ABC):
     def infer_attn_size_config(self, function: ir.Function) -> AttnSizeConfig:
-        if len(function.outputs) != 3:
+        if len(function.outputs) == 3:
+            # Usually the Attention related modules have 3 outputs:
+            # present_value, present_key, attn_output
+            present_value, _, attn_output = function.outputs
+            if present_value.shape is None:
+                raise function_rule.FunctionRewriteError(
+                    "Failed to find shape for present_value."
+                )
+            if attn_output.shape is None:
+                raise function_rule.FunctionRewriteError(
+                    "Failed to find shape for attn_output."
+                )
+            head_size = present_value.shape[3]
+            num_key_value_heads = present_value.shape[1]
+            hidden_size = attn_output.shape[2]
+            num_attention_heads = hidden_size // head_size
+            return AttnSizeConfig(
+                num_attention_heads=num_attention_heads,
+                num_key_value_heads=num_key_value_heads,
+                head_size=head_size,
+                hidden_size=hidden_size,
+            )
+        elif any("scaled_dot_product_attention" in node.op_type for node in function):
+            # If the Attention related modules use scaled_dot_product_attention,
+            # present_value and present_key are not present in the output.
+            hidden_size = function.outputs[0].shape[2]
+            # Get head size and number of heads from the Reshape node.
+            # Reference:
+            # https://github.com/huggingface/diffusers/blob/ae05050db9d37d5af48a6cd0d6510a5ffb1c1cd4/src/diffusers/models/attention_processor.py#L1269
+            reshape_nodes = [node for node in function if node.op_type == "Reshape"]
+            assert (
+                len(reshape_nodes) == 4
+            ), "Expected 3 Reshape nodes for Q, K and V, and 1 reshape node for output of scaled_dot_product_attention."
+            for reshape_node in reshape_nodes:
+                constant_node = reshape_node.inputs[1].producer()
+                assert (
+                    constant_node.op_type == "Constant"
+                ), "Expected the second input to Reshape to be a Constant node."
+                value = _ir_utils.propagate_const_value(reshape_node.inputs[1])
+                constant_numpy_value = _ir_utils.get_numpy_from_ir_value(value)
+                if constant_numpy_value.shape[0] == 4:
+                    num_attention_heads = constant_numpy_value[2]
+                    head_size = constant_numpy_value[3]
+                    return AttnSizeConfig(
+                        num_attention_heads=num_attention_heads,
+                        num_key_value_heads=None,
+                        head_size=head_size,
+                        hidden_size=hidden_size,
+                    )
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of outputs. Expected 3, got {len(function.outputs)}."
+                "Failed to infer head size and number of heads from QKV Reshape nodes. \
+                Expected 4D shape in the constant node (batch_size, seq_length, num_attention_heads, head_size)."
             )
-        present_value, _, attn_output = function.outputs
-        if present_value.shape is None:
-            raise function_rule.FunctionRewriteError("Failed to find shape for present_value.")
-        if attn_output.shape is None:
-            raise function_rule.FunctionRewriteError("Failed to find shape for attn_output.")
-        head_size = present_value.shape[3]
-        num_key_value_heads = present_value.shape[1]
-        hidden_size = attn_output.shape[2]
-        num_attention_heads = hidden_size // head_size
-        return AttnSizeConfig(
-            num_attention_heads=num_attention_heads,
-            num_key_value_heads=num_key_value_heads,
-            head_size=head_size,
-            hidden_size=hidden_size,
+        raise function_rule.FunctionRewriteError(
+            f"Attenion modules should have 3 outputs or scaled_dot_product_attention node, "
+            f"got output: {len(function.outputs)} and no scaled_dot_product_attention."
         )
 
 
 class MHALlama2RewriteRule(AttentionRewriteRule):
     FUNCTION_KEYWORD = "LlamaAttention"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
-    def __init__(self) -> None:
-        super().__init__()
-
     @_version_controller.register_version(min_version="4.33", max_version="4.36")
     def _fusion_with_4d_cache(self, function: ir.Function) -> ir.Function:
-        if len(function.input) != 9:
+        if len(function.inputs) != 9:
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
+                f"Unexpected number of inputs. Expected 9, got {len(function.inputs)}."
             )
 
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
@@ -168,17 +203,17 @@
         return ir.serde.deserialize_function(function_proto)
 
     @_version_controller.register_version(min_version="4.36", max_version="4.38")
     def _fusion_with_2d_cache(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
-        if len(function.input) != 9:
+        if len(function.inputs) != 9:
             raise function_rule.FunctionRewriteError(
-                f"Unexpected number of inputs. Expected 9, got {len(function.input)}."
+                f"Unexpected number of inputs. Expected 9, got {len(function.inputs)}."
             )
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_op = onnxscript.values.Opset("com.microsoft", 1)
 
         # Workaround onnxscript error by specifying the output shape here.
@@ -230,17 +265,14 @@
 
 
 class GQALlama2RewriteRule(AttentionRewriteRule):
     FUNCTION_KEYWORD = "LlamaAttention"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
-    def __init__(self) -> None:
-        super().__init__()
-
     @_version_controller.register_version(min_version="4.33", max_version="4.36")
     def _fusion_with_4d_cache(self, function: ir.Function) -> ir.Function:
         if len(function.inputs) != 9:
             raise function_rule.FunctionRewriteError(
                 f"Unexpected number of inputs. Expected 9, got {len(function.inputs)}."
             )
 
@@ -380,17 +412,14 @@
     # The pitfall is that the source function signature is slightly different.
     # One has `attention_mask` as input while the other does not.
     # Possibly designing a function template system could help reduce the boilerplate.
     FUNCTION_KEYWORD = "LlamaSdpaAttention"
     PACKAGE_NAME = "transformers"
     _version_controller = function_rule.VersionController()
 
-    def __init__(self) -> None:
-        super().__init__()
-
     @_version_controller.register_version(min_version="4.36", max_version="4.38")
     def _fusion(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
@@ -447,15 +476,14 @@
         ).to_function_proto()
         return ir.serde.deserialize_function(function_proto)
 
     @_version_controller.register_version(min_version="4.38")
     def _fusion_without_cos_sin_cache(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
-
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
         msft_op = onnxscript.values.Opset("com.microsoft", 1)
 
         cos_sin_gather_size = [attn_size_config.head_size // 2]
 
         def gqa(
@@ -524,17 +552,14 @@
 
 
 class AttnPhi15RewriteRule(AttentionRewriteRule):
     FUNCTION_KEYWORD = "PhiAttention"
     PACKAGE_NAME = "transformers_modules"
     _version_controller = function_rule.VersionController()
 
-    def __init__(self) -> None:
-        super().__init__()
-
     @_version_controller.register_version()
     def _fusion(self, function: ir.Function) -> ir.Function:
         # Infer size configurations from the function.
         attn_size_config = self.infer_attn_size_config(function)
 
         # Code new pattern with onnxscript.
         op = onnxscript.opset18
@@ -588,7 +613,94 @@
 
             return present_value, present_key, output
 
         function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
             phi_attention
         ).to_function_proto()
         return ir.serde.deserialize_function(function_proto)
+
+
+class MHAStableDiffusionUnetRewriteRule(AttentionRewriteRule):
+    """Rewrite rule for Attention in diffusers."""
+
+    FUNCTION_KEYWORD = "Attention"
+    PACKAGE_NAME = "diffusers"
+    _version_controller = function_rule.VersionController()
+
+    @_version_controller.register_version()
+    def _fusion(self, function: ir.Function) -> ir.Function:
+        # Attention inputs could be 6 or 7:
+        # hidden_states, encoder_hidden_states(optional), q_weight, k_weight, v_weight, o_weight, o_bias
+        if len(function.inputs) != 6 and len(function.inputs) != 7:
+            raise function_rule.FunctionRewriteError(
+                f"Unexpected number of inputs. Expected 6 or 7, got {len(function.inputs)}."
+            )
+
+        # Infer size configurations from the function.
+        attn_size_config = self.infer_attn_size_config(function)
+
+        # Code new pattern with onnxscript.
+        op = onnxscript.opset18
+        msft_op = onnxscript.values.Opset("com.microsoft", 1)
+
+        def attention(
+            hidden_states,
+            q_weight,
+            k_weight,
+            v_weight,
+            o_weight,
+            o_bias,
+        ):
+            qkv_weight = op.Transpose(
+                op.Concat(q_weight, k_weight, v_weight, axis=0),
+                perm=[1, 0],
+            )
+
+            # NOTE: MHA does not work when Q, K, and V has the same root inputs.
+            attn_output, _ = msft_op.Attention(
+                hidden_states,
+                qkv_weight,
+                None,
+                None,
+                num_heads=attn_size_config.num_attention_heads,
+            )
+
+            # linear projection
+            output = op.Add(op.MatMul(attn_output, op.Transpose(o_weight, [1, 0])), o_bias)
+            return output
+
+        def mha(
+            hidden_states,
+            encoder_hidden_states,
+            q_weight,
+            k_weight,
+            v_weight,
+            o_weight,
+            o_bias,
+        ):
+            q = op.MatMul(hidden_states, op.Transpose(q_weight, [1, 0]))
+            k = op.MatMul(encoder_hidden_states, op.Transpose(k_weight, [1, 0]))
+            v = op.MatMul(encoder_hidden_states, op.Transpose(v_weight, [1, 0]))
+
+            # NOTE: Q and K needs to have the sequence length (dim 1) to use
+            # GQA.
+            mha_output, _, _ = msft_op.MultiHeadAttention(
+                q,
+                k,
+                v,
+                None,
+                None,
+                num_heads=attn_size_config.num_attention_heads,
+            )
+            attn_output = op.Add(op.MatMul(mha_output, op.Transpose(o_weight, [1, 0])), o_bias)
+            return attn_output
+
+        if len(function.inputs) == 6:
+            function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+                attention
+            ).to_function_proto()
+            return ir.serde.deserialize_function(function_proto)
+
+        function_proto = onnxscript.script(default_opset=onnxscript.opset18)(
+            mha
+        ).to_function_proto()
+        return ir.serde.deserialize_function(function_proto)
```

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240428/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240428/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240428/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240428/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240428/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240428/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript/values.py` & `onnxscript-0.1.0.dev20240428/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240428/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240427
+Version: 0.1.0.dev20240428
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240427/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240428/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/pyproject.toml` & `onnxscript-0.1.0.dev20240428/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240427/setup.py` & `onnxscript-0.1.0.dev20240428/setup.py`

 * *Files identical despite different names*
