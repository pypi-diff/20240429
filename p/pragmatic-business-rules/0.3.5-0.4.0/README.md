# Comparing `tmp/pragmatic-business-rules-0.3.5.tar.gz` & `tmp/pragmatic_business_rules-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pragmatic-business-rules-0.3.5.tar", last modified: Tue Nov 23 19:27:11 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pragmatic-business-rules-0.3.5.tar` & `pragmatic_business_rules-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-11-23 19:27:11.379206 pragmatic-business-rules-0.3.5/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1071 2021-11-22 17:43:15.000000 pragmatic-business-rules-0.3.5/LICENSE
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      497 2021-11-23 19:27:11.379206 pragmatic-business-rules-0.3.5/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       27 2021-11-22 17:47:05.000000 pragmatic-business-rules-0.3.5/README.md
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-11-23 19:27:11.375873 pragmatic-business-rules-0.3.5/pragmatic_business_rules/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       75 2021-11-23 19:26:46.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1216 2021-11-23 16:54:31.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/action.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1078 2021-11-23 16:57:52.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/asserts.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3937 2021-11-23 18:41:20.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/condition.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1952 2021-11-23 18:34:35.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/main.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      577 2021-11-22 18:18:14.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/types.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2523 2021-11-23 16:41:32.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules/validators.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-11-23 19:27:11.375873 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      497 2021-11-23 19:27:11.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      517 2021-11-23 19:27:11.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2021-11-23 19:27:11.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       11 2021-11-23 19:27:11.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/requires.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       25 2021-11-23 19:27:11.000000 pragmatic-business-rules-0.3.5/pragmatic_business_rules.egg-info/top_level.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2021-11-23 19:27:11.379206 pragmatic-business-rules-0.3.5/setup.cfg
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      743 2021-11-22 18:12:19.000000 pragmatic-business-rules-0.3.5/setup.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/dev_requirements.txt
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/dprint.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/mypy.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/examples/long.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/__init__.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/action.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/asserts.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/condition.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/main.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/types.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_action.py
+-rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_condition.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/tests/test_validators.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/LICENSE
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.0/PKG-INFO
```

### Comparing `pragmatic-business-rules-0.3.5/LICENSE` & `pragmatic_business_rules-0.4.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Steven Guerrero
+Copyright (c) (2021-2024) Steven Guerrero
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pragmatic-business-rules-0.3.5/pragmatic_business_rules/asserts.py` & `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/asserts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .types import Conditional
-from typing import Any
-
+from decimal import Decimal
+from typing import Any, Optional
 
 def assert_single_conditional(conditional: Conditional):
 	all = conditional.get("all")
 	any = conditional.get("any")
 
 	if all is not None and any is not None:
 		raise Exception(
@@ -12,27 +12,37 @@
 		)
 	elif all is None and any is None:
 		raise Exception(
 			"'all' or 'any' properties were not found in the conditional"
 		)
 
 
-def assert_comparable_type(value: Any, variable_name: str, variable_value: Any):
+def assert_comparable_type(
+	label_1: Optional[str],
+	value_1: Any,
+	label_2: Optional[str],
+	value_2: Any,
+):
 	# None is comparable to string and None
-	if (value is None and variable_value is None) or (
-		type(value) == str and variable_value is None
-	) or (value is None and type(variable_value) == str):
+	if (value_1 is None and value_2 is None) or (
+		type(value_1) == str and value_2 is None
+	) or (
+		value_1 is None and type(value_2) == str
+	):
 		return
 
-	# Ints and floats are comparable
-	if type(value) in [int, float] and type(variable_value) in [int, float]:
+	# Decimal, ints and floats are comparable
+	if type(value_1) in [Decimal, int, float] and type(value_2) in [Decimal, int, float]:
 		return
 
-	if type(value) != type(variable_value):
+	if type(value_1) != type(value_2):
 		raise Exception(
-			"The value '{}' to compare for variable '{}' doesn't match the defined type of '{}'"
+			'Can\'t compare values ({}"{}", {}) and ({}"{}", {})'
 			.format(
-				value,
-				variable_name,
-				type(variable_value).__name__,
+				f'"{label_1}", ' if label_1 is not None else "",
+				value_1,
+				type(value_1).__name__,
+				f'"{label_2}", ' if label_2 is not None else "",
+				value_2,
+				type(value_2).__name__,
 			)
 		)
```

### Comparing `pragmatic-business-rules-0.3.5/pragmatic_business_rules/main.py` & `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 from .action import apply_actions_to_variables
 from .asserts import assert_single_conditional
 from .condition import evaluate_conditional
-from .types import Rule
-from .validators import CustomValidationError, variable_schema, rule_schema, validate_schema_with_custom_errors
+from .types import Conditional, number, Rule
+from .validators import constant_schema, CustomValidationError, variable_schema, rule_schema, validate_schema_with_custom_errors
 from jsonschema.exceptions import ValidationError
-from typing import Dict, List, Union
+from typing import Literal, Union
 import jsonschema
 
 
-def assert_valid_rules(rules: List[Rule]):
+def assert_valid_rules(rules: list[Rule]):
 	"""
 	This function runs a validation over the rules passed and raises a detailed message with any
 	inconsistencies found
 	"""
 	validate_schema_with_custom_errors(rules, rule_schema)
 
 
 def process_rules(
-	rules: List[Rule],
-	variables: Dict[str, Union[int, float, str]],
-) -> Dict[str, Union[int, float, str]]:
+	rules: list[Rule],
+	constants: dict[str, Union[number, str]] = {},
+	variables: dict[str, Union[number, str]] = {},
+) -> dict[str, Union[number, str]]:
 	"""
 	Process the rules and execute the result of the actions over the passed variables argument
 
 	This function does not mutate the original variables object passed to it
 	"""
-	result = variables.copy()
-
 	try:
 		assert_valid_rules(rules)
 	except CustomValidationError as validation_error:
 		raise Exception(
 			f"Invalid input for 'rules': {str(validation_error)}"
 		) from validation_error
 	except ValidationError as validation_error:
 		raise Exception(
 			f"Invalid input for 'rules': {str(validation_error)}"
 		) from validation_error
 
 	try:
+		jsonschema.validate(constants, constant_schema)
+	except ValidationError as validation_error:
+		raise Exception(
+			f"Invalid input for 'constants': {validation_error.message}"
+		) from validation_error
+
+	try:
 		jsonschema.validate(variables, variable_schema)
 	except ValidationError as validation_error:
 		raise Exception(
 			f"Invalid input for 'variables': {validation_error.message}"
 		) from validation_error
-
+	
+	result = variables.copy()
 	for rule in rules:
-		actions = rule.get("actions")
-		conditions = rule.get("conditions")
+		actions = rule["actions"]
+		conditions: Conditional = rule["conditions"]
 
-		# Make sure the condition has at least one usable condition
+		# Make sure the condition has one single conditional defined
 		assert_single_conditional(conditions)
 
 		all = conditions.get("all")
 		any = conditions.get("any")
 
-		conditional = all if all is not None else any
-		type = "all" if all is not None else "any"
+		conditional = all if all is not None else any if any is not None else []
+		type: Literal["all", "any"] = "all" if all is not None else "any"
 
-		if evaluate_conditional(conditional, result, type):
+		if evaluate_conditional(conditional, constants, result, type):
 			apply_actions_to_variables(actions, result)
 
 	return result
```

### Comparing `pragmatic-business-rules-0.3.5/pragmatic_business_rules/validators.py` & `pragmatic_business_rules-0.4.0/src/pragmatic_business_rules/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,43 @@
-import jsonschema
 from jsonschema.exceptions import ValidationError
-
+from typing import Any
+import jsonschema
 
 class CustomValidationError(Exception):
 
 	def __init__(self, message: str):
 		self.message = message
 		super().__init__(self.message)
 
 
-def validate_schema_with_custom_errors(data: dict, schema: dict):
+def validate_schema_with_custom_errors(data: Any, schema: dict):
 	try:
 		jsonschema.validate(data, schema)
 	except ValidationError as e:
 		error_message = e.schema.get("error_message")
 		if error_message is not None:
 			raise CustomValidationError(f"{error_message}: {e.message}")
 		else:
 			raise e
 
+# This object will match any object with no nested properties and all items being
+# either None, strings or numbers
+constant_schema = {
+	"additionalProperties": False,
+	"patternProperties": {
+		".+": {
+			"type": [
+				"null",
+				"number",
+				"string",
+			]
+		},
+	},
+	"type": "object",
+}
 
 # This object will match any object with no nested properties and all items being
 # either None, strings or numbers
 variable_schema = {
 	"additionalProperties": False,
 	"patternProperties": {
 		".+": {
@@ -35,16 +50,17 @@
 	},
 	"type": "object",
 }
 
 rule_schema = {
 	"$defs": {
 		"condition": {
+			"additionalProperties": False,
 			"properties": {
-				"name": {
+				"constant": {
 					"type": "string",
 				},
 				"operator": {
 					"enum": [
 						"equal_to",
 						"greater_than_or_equal_to",
 						"greater_than",
@@ -57,19 +73,20 @@
 				"value": {
 					"type": [
 						"null",
 						"number",
 						"string",
 					],
 				},
+				"variable": {
+					"type": "string",
+				},
 			},
 			"required": [
-				"name",
 				"operator",
-				"value",
 			],
 			"type": "object",
 		},
 		"conditional": {
 			"additionalProperties": False,
 			"properties": {
 				"all": {
```

