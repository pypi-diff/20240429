# Comparing `tmp/healthsageai-0.1.4.tar.gz` & `tmp/healthsageai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthsageai-0.1.4.tar", last modified: Tue Apr 16 08:31:47 2024, max compression
+gzip compressed data, was "healthsageai-0.1.7.tar", last modified: Mon Apr 29 08:52:54 2024, max compression
```

## Comparing `healthsageai-0.1.4.tar` & `healthsageai-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.253445 healthsageai-0.1.4/
--rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.4/LICENSE
--rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-16 08:31:47.253016 healthsageai-0.1.4/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)     5699 2024-04-04 09:53:35.000000 healthsageai-0.1.4/README.md
--rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-04-16 08:31:28.000000 healthsageai-0.1.4/pyproject.toml
--rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-04-16 08:31:47.253519 healthsageai-0.1.4/setup.cfg
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.247290 healthsageai-0.1.4/src/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.4/src/__init__.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.246518 healthsageai-0.1.4/src/healthsageai/
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.248938 healthsageai-0.1.4/src/healthsageai/note_to_fhir/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2950 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/data_utils.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.250753 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     4644 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/datamodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3592 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)    23029 2024-04-16 08:30:15.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/utils.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/visuals.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.251639 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/
--rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3315 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/parsers.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.251956 healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/
--rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/simple.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.252304 healthsageai-0.1.4/src/healthsageai.egg-info/
--rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/SOURCES.txt
--rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/dependency_links.txt
--rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/requires.txt
--rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/top_level.txt
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.599224 healthsageai-0.1.7/
+-rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.7/LICENSE
+-rw-r--r--   0 a.groen    (501) staff       (20)    47746 2024-04-29 08:52:54.598929 healthsageai-0.1.7/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)     6423 2024-04-29 08:43:38.000000 healthsageai-0.1.7/README.md
+-rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-04-29 08:43:57.000000 healthsageai-0.1.7/pyproject.toml
+-rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-04-29 08:52:54.599272 healthsageai-0.1.7/setup.cfg
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.594029 healthsageai-0.1.7/src/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.7/src/__init__.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.592965 healthsageai-0.1.7/src/healthsageai/
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.595549 healthsageai-0.1.7/src/healthsageai/note_to_fhir/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2950 2024-04-04 09:53:35.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/data_utils.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.597382 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     4732 2024-04-17 10:53:36.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/datamodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3592 2024-04-04 09:53:35.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)    23029 2024-04-16 08:30:15.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/utils.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/visuals.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.597938 healthsageai-0.1.7/src/healthsageai/note_to_fhir/inference/
+-rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/inference/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3355 2024-04-29 08:11:06.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/parsers.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.598222 healthsageai-0.1.7/src/healthsageai/note_to_fhir/templates/
+-rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.7/src/healthsageai/note_to_fhir/templates/simple.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-29 08:52:54.598499 healthsageai-0.1.7/src/healthsageai.egg-info/
+-rw-r--r--   0 a.groen    (501) staff       (20)    47746 2024-04-29 08:52:54.000000 healthsageai-0.1.7/src/healthsageai.egg-info/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-04-29 08:52:54.000000 healthsageai-0.1.7/src/healthsageai.egg-info/SOURCES.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-04-29 08:52:54.000000 healthsageai-0.1.7/src/healthsageai.egg-info/dependency_links.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-04-29 08:52:54.000000 healthsageai-0.1.7/src/healthsageai.egg-info/requires.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-04-29 08:52:54.000000 healthsageai-0.1.7/src/healthsageai.egg-info/top_level.txt
```

### Comparing `healthsageai-0.1.4/LICENSE` & `healthsageai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/PKG-INFO` & `healthsageai-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.4
+Version: 0.1.7
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -698,18 +698,17 @@
 Requires-Dist: bitsandbytes
 Requires-Dist: accelerate
 
 # HealthSage AI LLM - from clinical note to FHIR
 
 ## Introduction
 
-HealthSage AI's LLM is a fine-tuned version of Meta's Llama 2 13B to create structured information - FHIR Resources - from
-unstructured clinical notes - plain text.
+HealthSage AI's LLM's are fine-tuned versions of LLama-13b and Mixtral-8x7b to create structured information - FHIR Resources - from unstructured clinical notes - plain text.
 
-The model is optimized to process English notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
+The model is optimized to process English and/or Dutch notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
 
 ## Getting started
 
 This repository consists of the following modules:
 
 - healthsageai.note_to_fhir.evaluation - compare generated FHIR resources against ground truth/reference resource.
 - healthsageai.note_to_fhir.inference - running inference on the model, either locally or in a containerized environment.
@@ -721,20 +720,29 @@
 [![Open inference-note-to-fhir-colab-notebook in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/healthsage-ai/healthsage-ai-llm/blob/main/docs/inference_note_to_fhir_colab_notebook.ipynb)
 
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
-from healthsageai.note_to_fhir.inference import NoteToFhir13b
+from healthsageai.note_to_fhir.inference import NoteToFhir13b, NoteToFhir8x7b
+```
 
+To run our first beta model, based on LLama-13b:
+```python
 model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
+To run our second beta model, based on LLama-8x7b:
+```python
+model = NoteToFhir8x7b()
+model.translate("Patient Sofie de Jong woont in Amsterdam")
+```
+
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
 For that we designed the FhirScore and FhirDiff models as well as several functions to process and visualize these models. 
 
 ```python
@@ -780,26 +788,28 @@
   5. Organization
   6. Immunization
   7. Observation
   8. Condition
   9. AllergyIntolerance
   10. Procedure. 
 - English language
-
+- Dutch language (8x7b version only)
 
 ### The following features are out of scope of the current release:
 - Support for Coding systems such as SNOMED CT and Loinc.
 - FHIR extensions and profiles
 - Any language, resource type or FHIR version not mentioned under "in scope".
 
 We are continuously training our model and will make updates available - that address some of these items and more - on a regular basis.
 
 ### Furthermore, please note:
 - **No Relative dates:** HealthSage AI Note-to-FHIR will not provide accurate FHIR datetime fields based on text that contains relative time information like "today" or "yesterday". Furthermore, relative dates like "Patient John Doe is 50 years old." will not result in an accurate birthdate estimation, since the precise birthday and -month is unknown, and since the LLM is not aware of the current date. 
 - **Designed as Patient-centric:** HealthSage AI Note-to-FHIR is trained on notes describing one patient each. 
-- **<4k Context window:** The training data for this application contained at most 3686 tokens, which is 90% of the context window for Llama-2 (4096)
+- **<4k Context window:** The training data for this application contained at most 4096 tokens. Technically the model supports of to 32k tokens.
 - **Explicit Null:** If a certain FHIR element is not present in the provided text, it is explictely predicted as NULL. Explictely modeling the absence of information reduces the chance of hallucinations. 
-- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are Bundled.
+- **Major European languages:** We've seen encouraging results on German, French, Spanish and Italian. However, these are not trained and tested on fully.
+- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are transaction Bundles.
 - **Conservative estimates:** Our model is designed to stick to the information explicitely provided in the text. 
 - **ID's are local:** ID fields and references are local enumerations (1,2,3, etc.). They are not yet tested on referential correctness. 
 - **Generation design:** The model is designed to generate a seperate resource if there is information about that resource in the text beyond what can be described in reference fields of related resources.
 - **Test results:** Our preliminary results suggest that HealthSage AI Note-to-FHIR is superior to the GPT-4 foundation model within the scope of our application in terms of FHIR Syntax and ability to replicate the original FHIR resources in our test dataset. We are currently analyzing our model on its performance for out-of-distribution data and out-of-scope data.
+- **Evaluation of datetime:** Datetime values are evaluation up to the minute level, since second and sub-second timing is typically not reported in clinical notes. For applications where second or sub-second timing is relevant, we advise changing this in your evaluation.
```

### Comparing `healthsageai-0.1.4/README.md` & `healthsageai-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # HealthSage AI LLM - from clinical note to FHIR
 
 ## Introduction
 
-HealthSage AI's LLM is a fine-tuned version of Meta's Llama 2 13B to create structured information - FHIR Resources - from
-unstructured clinical notes - plain text.
+HealthSage AI's LLM's are fine-tuned versions of LLama-13b and Mixtral-8x7b to create structured information - FHIR Resources - from unstructured clinical notes - plain text.
 
-The model is optimized to process English notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
+The model is optimized to process English and/or Dutch notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
 
 ## Getting started
 
 This repository consists of the following modules:
 
 - healthsageai.note_to_fhir.evaluation - compare generated FHIR resources against ground truth/reference resource.
 - healthsageai.note_to_fhir.inference - running inference on the model, either locally or in a containerized environment.
@@ -21,20 +20,29 @@
 [![Open inference-note-to-fhir-colab-notebook in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/healthsage-ai/healthsage-ai-llm/blob/main/docs/inference_note_to_fhir_colab_notebook.ipynb)
 
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
-from healthsageai.note_to_fhir.inference import NoteToFhir13b
+from healthsageai.note_to_fhir.inference import NoteToFhir13b, NoteToFhir8x7b
+```
 
+To run our first beta model, based on LLama-13b:
+```python
 model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
+To run our second beta model, based on LLama-8x7b:
+```python
+model = NoteToFhir8x7b()
+model.translate("Patient Sofie de Jong woont in Amsterdam")
+```
+
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
 For that we designed the FhirScore and FhirDiff models as well as several functions to process and visualize these models. 
 
 ```python
@@ -80,26 +88,28 @@
   5. Organization
   6. Immunization
   7. Observation
   8. Condition
   9. AllergyIntolerance
   10. Procedure. 
 - English language
-
+- Dutch language (8x7b version only)
 
 ### The following features are out of scope of the current release:
 - Support for Coding systems such as SNOMED CT and Loinc.
 - FHIR extensions and profiles
 - Any language, resource type or FHIR version not mentioned under "in scope".
 
 We are continuously training our model and will make updates available - that address some of these items and more - on a regular basis.
 
 ### Furthermore, please note:
 - **No Relative dates:** HealthSage AI Note-to-FHIR will not provide accurate FHIR datetime fields based on text that contains relative time information like "today" or "yesterday". Furthermore, relative dates like "Patient John Doe is 50 years old." will not result in an accurate birthdate estimation, since the precise birthday and -month is unknown, and since the LLM is not aware of the current date. 
 - **Designed as Patient-centric:** HealthSage AI Note-to-FHIR is trained on notes describing one patient each. 
-- **<4k Context window:** The training data for this application contained at most 3686 tokens, which is 90% of the context window for Llama-2 (4096)
+- **<4k Context window:** The training data for this application contained at most 4096 tokens. Technically the model supports of to 32k tokens.
 - **Explicit Null:** If a certain FHIR element is not present in the provided text, it is explictely predicted as NULL. Explictely modeling the absence of information reduces the chance of hallucinations. 
-- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are Bundled.
+- **Major European languages:** We've seen encouraging results on German, French, Spanish and Italian. However, these are not trained and tested on fully.
+- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are transaction Bundles.
 - **Conservative estimates:** Our model is designed to stick to the information explicitely provided in the text. 
 - **ID's are local:** ID fields and references are local enumerations (1,2,3, etc.). They are not yet tested on referential correctness. 
 - **Generation design:** The model is designed to generate a seperate resource if there is information about that resource in the text beyond what can be described in reference fields of related resources.
 - **Test results:** Our preliminary results suggest that HealthSage AI Note-to-FHIR is superior to the GPT-4 foundation model within the scope of our application in terms of FHIR Syntax and ability to replicate the original FHIR resources in our test dataset. We are currently analyzing our model on its performance for out-of-distribution data and out-of-scope data.
+- **Evaluation of datetime:** Datetime values are evaluation up to the minute level, since second and sub-second timing is typically not reported in clinical notes. For applications where second or sub-second timing is relevant, we advise changing this in your evaluation.
```

### Comparing `healthsageai-0.1.4/pyproject.toml` & `healthsageai-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "healthsageai"
-version = "0.1.4"
+version = "0.1.7"
 description = "HealthSage AI LLMs, Healthcare genAI platform"
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 license = {file = "LICENSE"}
```

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/data_utils.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/data_utils.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/datamodels.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/datamodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pydantic import BaseModel, computed_field, field_validator, Field
 from typing import Any, Optional
 from collections import defaultdict
 
+
 class FhirValiditionScore(BaseModel):
     n_nodes: int = 0
     n_valid_nodes: int = 0
     n_invalid_nodes: int = 0
     self_is_valid: Optional[bool] = None
 
     @computed_field
@@ -34,14 +35,15 @@
 
 class FhirScore(BaseModel):
     n_leaves: int = 0  # The number of leaf nodes in this object
     n_additions: int = 0  # n hallucinated leaf nodes, a.k.a. "False Positives"
     n_deletions: int = 0  #  n of missing leaf nodes, a.k.a. "False Negatives"
     n_modifications: int = 0  # n of changes leaf nodes a.k.a. "Mistakes"
     n_matches: int = 0  # n of identical leaf nodes, a.k.a. "True Positives"
+    is_valid: Optional[bool] = None
 
     @computed_field
     @property
     def accuracy(self) -> float:  # The overall accuracy
         if self.n_leaves == 0:
             return None
         return self.n_matches / self.n_leaves
@@ -67,14 +69,15 @@
             return self
         return FhirScore(
             n_leaves=self.n_leaves + other.n_leaves,
             n_additions=self.n_additions + other.n_additions,
             n_deletions=self.n_deletions + other.n_deletions,
             n_modifications=self.n_modifications + other.n_modifications,
             n_matches=self.n_matches + other.n_matches,
+            is_valid=self.is_valid and other.is_valid,
         )
 
     def __radd__(self, other: Any):
         if not isinstance(other, FhirScore):
             return self
         else:
             return self.__add__(other)
@@ -124,8 +127,7 @@
     @field_validator("fhir_true", "fhir_pred", mode="before")
     def convert_to_defaultdict(cls, v):
         if isinstance(v, dict):
             return defaultdict(lambda: {}, v)
         if v is None:
             return defaultdict(lambda: {})
         return v
-
```

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/utils.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/visuals.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/evaluation/visuals.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/note_to_fhir.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/inference/note_to_fhir.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,80 +9,91 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 #
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from transformers import BitsAndBytesConfig, AutoModelForCausalLM, AutoTokenizer, pipeline
+from transformers import (
+    BitsAndBytesConfig,
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    pipeline,
+)
 import torch
 from healthsageai.note_to_fhir.data_utils import drop_snomed_loinc, drop_nones
 from healthsageai.note_to_fhir.templates.simple import template_dict
 from healthsageai.note_to_fhir.parsers import parse_note_to_fhir
 
-class NoteToFhir(object):
 
+class NoteToFhir(object):
     def __init__(self, model_name: str, adapter_name: str, template_style: str) -> None:
         """_summary_
 
         Args:
             model_name (str or os.PathLike): The base model
             adapter_name (str or os.PathLike): The Q-LoRA adapter
             template_style (str): "gpt", "llama" or "mixtral"
         """
         self.template = template_dict[template_style]
         bnb_config = BitsAndBytesConfig(
-        load_in_4bit=True,
-        bnb_4bit_use_double_quant=True,
-        bnb_4bit_quant_type="nf4",
-        bnb_4bit_compute_dtype=torch.float16,
+            load_in_4bit=True,
+            bnb_4bit_use_double_quant=True,
+            bnb_4bit_quant_type="nf4",
+            bnb_4bit_compute_dtype=torch.float16,
         )
 
         model = AutoModelForCausalLM.from_pretrained(
             model_name,
             trust_remote_code=True,
             quantization_config=bnb_config,
-            device_map='auto',
+            device_map="auto",
         )
 
         model.config.use_cache = False
         model.load_adapter(adapter_name)
 
-        tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True, return_tensor="pt", padding=True)
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_name, trust_remote_code=True, return_tensor="pt", padding=True
+        )
         tokenizer.pad_token = tokenizer.bos_token
-        tokenizer.padding_side = 'right'
+        tokenizer.padding_side = "left"
 
         self.generator = pipeline(
-            model=model, 
+            model=model,
             tokenizer=tokenizer,
             task="text-generation",
             do_sample=True,
             eos_token_id=model.config.eos_token_id,
-            max_length=4096
+            max_length=4096,
         )
 
-    def translate(self, note : str) -> dict:
+    def translate(self, note: str) -> dict:
         """Convert a note to FHIR
 
         Args:
             note (str): clinical note
         """
         prompt = self.template.format(note=note)
         generated_output = self.generator(prompt)
-        fhir = parse_note_to_fhir(generated_output[0]['generated_text'])
+        fhir = parse_note_to_fhir(generated_output[0]["generated_text"])
         fhir = drop_nones(fhir)
         fhir = drop_snomed_loinc(fhir)
         return fhir
-    
-class NoteToFhir13b(NoteToFhir):
 
+
+class NoteToFhir13b(NoteToFhir):
     def __init__(self):
-        super().__init__(model_name="meta-llama/Llama-2-13b-chat-hf",
-                        adapter_name="healthsageai/note-to-fhir-13b-adapter",
-                        template_style="llama")
-        
-class NoteToFhir8x7b(NoteToFhir):
+        super().__init__(
+            model_name="meta-llama/Llama-2-13b-chat-hf",
+            adapter_name="healthsageai/note-to-fhir-13b-adapter",
+            template_style="llama",
+        )
+
 
+class NoteToFhir8x7b(NoteToFhir):
     def __init__(self):
-        super().__init__(model_name="mistralai/Mixtral-8x7B-Instruct-v0.1",
-                        adapter_name="healthsageai/note-to-fhir-8x7b-mixtral-dev",
-                        template_style="mixtral")
+        super().__init__(
+            model_name="mistralai/Mixtral-8x7B-Instruct-v0.1",
+            adapter_name="healthsageai/note-to-fhir-8x7b-adapter",
+            template_style="mixtral",
+        )
```

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/parsers.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/parsers.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/simple.py` & `healthsageai-0.1.7/src/healthsageai/note_to_fhir/templates/simple.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.4/src/healthsageai.egg-info/PKG-INFO` & `healthsageai-0.1.7/src/healthsageai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.4
+Version: 0.1.7
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -698,18 +698,17 @@
 Requires-Dist: bitsandbytes
 Requires-Dist: accelerate
 
 # HealthSage AI LLM - from clinical note to FHIR
 
 ## Introduction
 
-HealthSage AI's LLM is a fine-tuned version of Meta's Llama 2 13B to create structured information - FHIR Resources - from
-unstructured clinical notes - plain text.
+HealthSage AI's LLM's are fine-tuned versions of LLama-13b and Mixtral-8x7b to create structured information - FHIR Resources - from unstructured clinical notes - plain text.
 
-The model is optimized to process English notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
+The model is optimized to process English and/or Dutch notes and populate 10 FHIR resource types. For a full description of the scope and limitations, see the performance and limitations header below. 
 
 ## Getting started
 
 This repository consists of the following modules:
 
 - healthsageai.note_to_fhir.evaluation - compare generated FHIR resources against ground truth/reference resource.
 - healthsageai.note_to_fhir.inference - running inference on the model, either locally or in a containerized environment.
@@ -721,20 +720,29 @@
 [![Open inference-note-to-fhir-colab-notebook in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/healthsage-ai/healthsage-ai-llm/blob/main/docs/inference_note_to_fhir_colab_notebook.ipynb)
 
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
-from healthsageai.note_to_fhir.inference import NoteToFhir13b
+from healthsageai.note_to_fhir.inference import NoteToFhir13b, NoteToFhir8x7b
+```
 
+To run our first beta model, based on LLama-13b:
+```python
 model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
+To run our second beta model, based on LLama-8x7b:
+```python
+model = NoteToFhir8x7b()
+model.translate("Patient Sofie de Jong woont in Amsterdam")
+```
+
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
 For that we designed the FhirScore and FhirDiff models as well as several functions to process and visualize these models. 
 
 ```python
@@ -780,26 +788,28 @@
   5. Organization
   6. Immunization
   7. Observation
   8. Condition
   9. AllergyIntolerance
   10. Procedure. 
 - English language
-
+- Dutch language (8x7b version only)
 
 ### The following features are out of scope of the current release:
 - Support for Coding systems such as SNOMED CT and Loinc.
 - FHIR extensions and profiles
 - Any language, resource type or FHIR version not mentioned under "in scope".
 
 We are continuously training our model and will make updates available - that address some of these items and more - on a regular basis.
 
 ### Furthermore, please note:
 - **No Relative dates:** HealthSage AI Note-to-FHIR will not provide accurate FHIR datetime fields based on text that contains relative time information like "today" or "yesterday". Furthermore, relative dates like "Patient John Doe is 50 years old." will not result in an accurate birthdate estimation, since the precise birthday and -month is unknown, and since the LLM is not aware of the current date. 
 - **Designed as Patient-centric:** HealthSage AI Note-to-FHIR is trained on notes describing one patient each. 
-- **<4k Context window:** The training data for this application contained at most 3686 tokens, which is 90% of the context window for Llama-2 (4096)
+- **<4k Context window:** The training data for this application contained at most 4096 tokens. Technically the model supports of to 32k tokens.
 - **Explicit Null:** If a certain FHIR element is not present in the provided text, it is explictely predicted as NULL. Explictely modeling the absence of information reduces the chance of hallucinations. 
-- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are Bundled.
+- **Major European languages:** We've seen encouraging results on German, French, Spanish and Italian. However, these are not trained and tested on fully.
+- **Uses Bundles:** For consistency and simplicity, all predicted FHIR resources are transaction Bundles.
 - **Conservative estimates:** Our model is designed to stick to the information explicitely provided in the text. 
 - **ID's are local:** ID fields and references are local enumerations (1,2,3, etc.). They are not yet tested on referential correctness. 
 - **Generation design:** The model is designed to generate a seperate resource if there is information about that resource in the text beyond what can be described in reference fields of related resources.
 - **Test results:** Our preliminary results suggest that HealthSage AI Note-to-FHIR is superior to the GPT-4 foundation model within the scope of our application in terms of FHIR Syntax and ability to replicate the original FHIR resources in our test dataset. We are currently analyzing our model on its performance for out-of-distribution data and out-of-scope data.
+- **Evaluation of datetime:** Datetime values are evaluation up to the minute level, since second and sub-second timing is typically not reported in clinical notes. For applications where second or sub-second timing is relevant, we advise changing this in your evaluation.
```

### Comparing `healthsageai-0.1.4/src/healthsageai.egg-info/SOURCES.txt` & `healthsageai-0.1.7/src/healthsageai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

