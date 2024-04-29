# Comparing `tmp/ragdaemon-0.2.9.tar.gz` & `tmp/ragdaemon-0.3.0.tar.gz`

## Comparing `ragdaemon-0.2.9.tar` & `ragdaemon-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/app.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/context.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/llm.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/test_sample.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/app.py
+-rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/context.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/graph.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.3.0/PKG-INFO
```

### Comparing `ragdaemon-0.2.9/tutorial.ipynb` & `ragdaemon-0.3.0/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/.github/workflows/run-tests.yml` & `ragdaemon-0.3.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/app.py` & `ragdaemon-0.3.0/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/context.py` & `ragdaemon-0.3.0/ragdaemon/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             elif len(data["lines"]) == data["document"].splitlines():
                 refs[path] = ""
                 continue
             segments = []
             current_segment = ""
             last_line = 0
             for line in sorted(data["lines"]):
-                if line - last_line > 1:
+                if current_segment and line - last_line > 1:
                     current_segment += f"-{last_line}"
                     segments.append(current_segment)
                     current_segment = ""
                 if not current_segment:
                     current_segment = str(line)
                 last_line = line
             if current_segment:
```

### Comparing `ragdaemon-0.2.9/ragdaemon/daemon.py` & `ragdaemon-0.3.0/ragdaemon/daemon.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import time
 from pathlib import Path
 from typing import Any, Optional
 
 from networkx.readwrite import json_graph
 from spice import Spice
+from spice.spice import Model
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
@@ -46,19 +47,23 @@
             self.graph_path = (cwd / graph_path).resolve()
         else:
             self.graph_path = (
                 mentat_dir_path / "ragdaemon" / f"ragdaemon-{self.cwd.name}.json"
             )
         self.graph_path.parent.mkdir(exist_ok=True)
         if spice_client is None:
+            logging_dir = mentat_dir_path / "ragdaemon" / "spice_logs"
+            logging_dir.mkdir(parents=True, exist_ok=True)
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
                 default_embeddings_model=model,
+                logging_dir=mentat_dir_path / "ragdaemon" / "spice_logs",
             )
         self.spice_client = spice_client
+        self.spice_client.load_dir(Path(__file__).parent / "prompts")
         self.embedding_model = model
         self.embedding_provider = provider
 
         # Initialize an empty graph
         self.graph = KnowledgeGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
@@ -78,14 +83,15 @@
     def db(self) -> Database:
         if not hasattr(self, "_db"):
             self._db = get_db(
                 self.cwd,
                 spice_client=self.spice_client,
                 embedding_model=self.embedding_model,
                 embedding_provider=self.embedding_provider,
+                verbose=self.verbose,
             )
         return self._db
 
     def save(self):
         """Saves the graph to disk."""
         data = json_graph.node_link_data(self.graph)
         with open(self.graph_path, "w") as f:
@@ -135,15 +141,15 @@
 
     def get_context(
         self,
         query: str,
         context_builder: Optional[ContextBuilder] = None,
         max_tokens: int = 8000,
         auto_tokens: int = 0,
-        model: str = DEFAULT_COMPLETION_MODEL,
+        model: Model | str = DEFAULT_COMPLETION_MODEL,
     ) -> ContextBuilder:
         if context_builder is None:
             context = ContextBuilder(self.graph, self.db, self.verbose)
         else:
             # TODO: Compare graph hashes, reconcile changes
             context = context_builder
         include_context_message = context.render()
```

### Comparing `ragdaemon-0.2.9/ragdaemon/get_paths.py` & `ragdaemon-0.3.0/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/graph.py` & `ragdaemon-0.3.0/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/utils.py` & `ragdaemon-0.3.0/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/__init__.py` & `ragdaemon-0.3.0/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.3.0/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.3.0/ragdaemon/annotators/chunker_line.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+from typing import Any, Coroutine
+
 from ragdaemon.annotators.chunker import Chunker
 
 
 class ChunkerLine(Chunker):
     name = "chunker_line"
+    chunk_field_id = "chunks_line"
 
     def __init__(self, *args, lines_per_chunk=50, **kwargs):
         super().__init__(*args, **kwargs)
         self.n = lines_per_chunk
 
-    async def chunk_file(
-        self, file: str, file_lines: list[str], verbose: bool
-    ) -> list[dict[str, str]]:
-        """Split text files into chunks N lines long.
-
-        Chunker.annotate will generate a 'BASE' chunk from the lines
-        not assigned to chunks as a hierarchical root of all chunks.
-        Here we set aside the first N lines as the BASE chunk.
-        """
-        if len(file_lines) < self.n:
+    async def chunk_document(self, document: str) -> list[dict[str, Any]]:
+        lines = document.splitlines()
+        file = lines[0]
+        file_lines = lines[1:]
+        if not file_lines or not any(line for line in file_lines):
             return []
-        chunks = list[dict[str, str]]()
-        for i, start_line in enumerate(range(self.n, len(file_lines), self.n)):
+
+        chunks = list[dict[str, Any]]()
+        if len(file_lines) > self.n:
             chunks.append(
                 {
-                    "id": f"{file}:chunk_{i + 1}",
-                    "start_line": str(start_line),
-                    "end_line": str(min(start_line + self.n - 1, len(file_lines))),
+                    "id": f"{file}:BASE",
+                    "start_line": "1",
+                    "end_line": str(self.n),
                 }
-            )
-        return chunks
+            )  # First N lines is always the base chunk
+            for i, start_line in enumerate(range(self.n + 1, len(file_lines), self.n)):
+                chunks.append(
+                    {
+                        "id": f"{file}:chunk_{i + 1}",
+                        "start_line": str(start_line),
+                        "end_line": str(min(start_line + self.n - 1, len(file_lines))),
+                    }
+                )
+        # Convert start/end to refs
+        return [
+            {
+                "id": chunk["id"],
+                "ref": f"{file}:{chunk['start_line']}-{chunk['end_line']}",
+            }
+            for chunk in chunks
+        ]
```

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.3.0/ragdaemon/annotators/chunker_llm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,156 @@
 import asyncio
 import json
 from json.decoder import JSONDecodeError
+from typing import Any, Dict, List, Optional
 
-from ragdaemon.annotators.chunker import Chunker, is_chunk_valid
+from spice import SpiceMessages
+
+from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.errors import RagdaemonError
-from spice import SpiceMessage
 
-chunker_prompt = """\
-Split the provided code file into chunks.
-Return a list of functions, classes and methods in this code file as JSON data.
-Each item in the list should contain:
-1. `id` - the complete call path, e.g. `path/to/file:class.method`
-2. `start_line` - where the function, class or method begins
-3. `end_line` - where it ends - INCLUSIVE
-
-If there are no chunks, return an empty list.
-
-EXAMPLE:
---------------------------------------------------------------------------------
-src/graph.py
-1:import pathlib as Path
-2:
-3:
-4:class KnowledgeGraph:
-5:    def __init__(self, cwd: Path):
-6:        self.cwd = cwd
-7:
-8:_knowledge_graph = None
-9:def get_knowledge_graph():
-10:    global _knowledge_graph
-11:    if _knowledge_graph is None:
-12:        _knowledge_graph = KnowledgeGraph(Path.cwd())
-13:    return _knowledge_graph
-14:
-
-RESPONSE:
-{
-    "chunks": [
-        {"id": "src/graph.py:KnowledgeGraph", "start_line": 4, "end_line": 6},
-        {"id": "src/graph.py:KnowledgeGraph.__init__", "start_line": 5, "end_line": 6},
-        {"id": "src/graph.py:get_knowledge_graph", "start_line": 9, "end_line": 13}
-    ]
-}
---------------------------------------------------------------------------------
-"""
-
-
-file_splitter_prompt = """\
-Identify a good point in the provided code file to split it in half, and return the line 
-number of that point.
-
-You should choose a point which:
-- Is approximately halfway through the file
-- Is in between top-level functions or classes.
-
-EXAMPLE:
---------------------------------------------------------------------------------
-src/graph.py
-1:import pathlib as Path
-2:
-3:
-4:class KnowledgeGraph:
-5:    def __init__(self, cwd: Path):
-6:        self.cwd = cwd
-7:
-8:_knowledge_graph = None
-9:def get_knowledge_graph():
-10:    global _knowledge_graph
-11:    if _knowledge_graph is None:
-12:        _knowledge_graph = KnowledgeGraph(Path.cwd())
-13:    return _knowledge_graph
-14:
-
-RESPONSE:
-{
-    "split_line": 7
-}
---------------------------------------------------------------------------------
-src/graph.py
-1:import pathlib as Path
-2:
-3:
-4:_knowledge_graph = None
-5:class KnowledgeGraph:
-6:    def __init__(self, cwd: Path):
-7:        self.cwd = cwd
-8:
-9:    def get_knowledge_graph():
-10:        global _knowledge_graph
-11:        if _knowledge_graph is None:
-12:            _knowledge_graph = KnowledgeGraph(Path.cwd())
-13:        return _knowledge_graph
-14:
-15:def get_knowledge_graph():
-16:    return _knowledge_graph
-
-RESPONSE:
-{
-    "split_line": 14
-}
-"""
+
+def is_chunk_valid(chunk: dict) -> bool:
+    # Includes the correct fields
+    if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
+        return False
+    # ID is in the correct format
+    if not chunk["id"].count(":") == 1:
+        return False
+    # A chunk name is specified
+    if not len(chunk["id"].split(":")[1]):
+        return False
+    # TODO: Validate the ref, i.e. a parent chunk exists
+
+    return True
 
 
 semaphore = asyncio.Semaphore(50)
 
 
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
+    chunk_field_id = "chunks_llm"
 
-    async def get_llm_response(self, file_message: str, depth: int = 1) -> dict:
-        if depth > 3:
-            raise RagdaemonError("Maximum recursion depth reached for chunker.")
+    async def get_llm_response(
+        self,
+        file: str,
+        file_lines: list[str],
+        last_chunk: Optional[dict[str, Any]] = None,
+    ) -> List[Dict[str, Any]]:
+        """Get one chunking response from the LLM model."""
         if self.spice_client is None:
             raise RagdaemonError("Spice client is not initialized.")
+
+        messages = SpiceMessages(self.spice_client)
+        messages.add_system_prompt(name="chunker_llm.base")
+        if last_chunk is not None:
+            messages.add_system_prompt(
+                "chunker_llm.continuation", last_chunk=last_chunk
+            )
+        messages.add_user_prompt(
+            "chunker_llm.user", path=file, code="\n".join(file_lines)
+        )
+
         global semaphore
         async with semaphore:
-            messages: list[SpiceMessage] = [
-                {"role": "system", "content": chunker_prompt},
-                {"role": "user", "content": file_message},
-            ]
             response = await self.spice_client.get_response(
                 messages=messages,
                 response_format={"type": "json_object"},
             )
-            try:
-                return json.loads(response.text)
-            except JSONDecodeError:
-                # This probably means the output is too long, i.e. there are too many
-                # functions to chunk in one pass. We split it in half and try again.
-                messages: list[SpiceMessage] = [
-                    {"role": "system", "content": file_splitter_prompt},
-                    {"role": "user", "content": file_message},
-                ]
-                response = await self.spice_client.get_response(
-                    messages=messages,
-                    response_format={"type": "json_object"},
-                )
-                split_line = json.loads(response.text).get("split_line")
-                if split_line is None:
-                    raise RagdaemonError(
-                        "Could not split file in half. Please try again."
-                    )
-                file_as_lines = file_message.split("\n")
-                first_half = file_as_lines[:split_line]
-                second_half = file_as_lines[split_line:]
-                tasks = []
-                tasks.append(self.get_llm_response("\n".join(first_half), depth + 1))
-                tasks.append(self.get_llm_response("\n".join(second_half), depth + 1))
-                responses = await asyncio.gather(*tasks)
-                first_response, second_response = responses
-                return {
-                    "chunks": first_response.get("chunks", [])
-                    + second_response.get("chunks", [])
-                }
-
-    async def chunk_file(
-        self, file: str, file_lines: list[str], verbose: bool
-    ) -> list[dict[str, str]]:
-        tries: int = 1
-        for tries in range(tries, 0, -1):
-            tries -= 1
-            numbered_lines = "\n".join(
-                f"{i+1}:{line}" for i, line in enumerate(file_lines)
+        try:
+            chunks = json.loads(response.text)["chunks"]
+        except JSONDecodeError:
+            raise RagdaemonError(
+                "Failed to parse JSON response. This could mean that the output is too "
+                "long, i.e. there are too many functions to chunk in one pass. If this "
+                "is the case, decrease the batch size and try again."
             )
-            file_message = f"{file}\n{numbered_lines}"
-            response = await self.get_llm_response(file_message)
-            chunks = response.get("chunks", [])
-            if not chunks or all(is_chunk_valid(chunk) for chunk in chunks):
-                return chunks
-            if tries > 1 and verbose:
-                print(f"Error with chunker response:\n{response}.\n{tries} tries left.")
-        return []
+        for chunk in chunks:
+            if not is_chunk_valid(chunk):
+                raise RagdaemonError(f"Model returned chunk: {chunk}")
+        if last_chunk is not None:
+            if not any(chunk["id"] == last_chunk["id"] for chunk in chunks):
+                raise RagdaemonError(
+                    f"Last chunk replacement ({last_chunk['id']}) not found in response."
+                )
+        return chunks
+
+    async def chunk_document(
+        self, document: str, batch_size: int = 1000, retries: int = 1
+    ) -> list[dict[str, Any]]:
+        """Parse file_lines into a list of {id, ref} chunks."""
+        lines = document.splitlines()
+        file = lines[0]
+        file_lines = lines[1:]
+        if not file_lines or not any(line for line in file_lines):
+            return []
+        file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
+
+        # Get raw llm output
+        chunks = list[dict[str, Any]]()
+        n_batches = (len(file_lines) + batch_size - 1) // batch_size
+        for i in range(n_batches):
+            batch_lines = file_lines[i * batch_size : (i + 1) * batch_size]
+            last_chunk = chunks.pop() if chunks else None
+            for j in range(retries + 1, 0, -1):
+                try:
+                    _chunks = await self.get_llm_response(file, batch_lines, last_chunk)
+                    chunks.extend(_chunks)
+                    break
+                except RagdaemonError as e:
+                    if self.verbose:
+                        print(
+                            f"Error chunking {file} batch {i+1}/{n_batches}:\n{e}\n"
+                            + f"{j-1} retries left."
+                            if j > 1
+                            else "Skipping."
+                        )
+                    if j == 1:
+                        return []
+
+        # Make sure end_line of each 'parent' chunk covers all children
+        def update_end_lines(id: str, _chunks: list[dict[str, Any]]):
+            child_chunks = [c for c in _chunks if c["id"].startswith(id + ".")]
+            if child_chunks:
+                end_line = max(c["end_line"] for c in child_chunks)
+                parent_chunk = next(c for c in _chunks if c["id"] == id)
+                parent_chunk["end_line"] = end_line
+            return _chunks
+
+        for chunk in sorted(chunks, key=lambda c: len(c["id"]), reverse=True):
+            chunks = update_end_lines(chunk["id"], chunks)
+
+        # Generate a 'BASE chunk' with all lines not already part of a chunk
+        base_chunk_lines = set(range(1, len(file_lines) + 1))
+        for chunk in chunks:
+            for i in range(int(chunk["start_line"]), int(chunk["end_line"]) + 1):
+                base_chunk_lines.discard(i)
+        if len(base_chunk_lines) > 0:
+            base_chunk_lines_sorted = sorted(list(base_chunk_lines))
+            base_chunk_refs = []
+            start = base_chunk_lines_sorted[0]
+            end = start
+            for i in base_chunk_lines_sorted[1:]:
+                if i == end + 1:
+                    end = i
+                else:
+                    if start == end:
+                        base_chunk_refs.append(f"{start}")
+                    else:
+                        base_chunk_refs.append(f"{start}-{end}")
+                    start = end = i
+            base_chunk_refs.append(f"{start}-{end}")
+        else:
+            base_chunk_refs = []
+        lines_str = ":" + ",".join(base_chunk_refs) if base_chunk_refs else ""
+        base_chunk = {"id": f"{file}:BASE", "ref": f"{file}{lines_str}"}
+
+        # Convert to refs and return
+        output = [base_chunk]
+        for chunk in chunks:
+            if chunk["start_line"] == chunk["end_line"]:
+                lines_str = str(chunk["start_line"])
+            else:
+                lines_str = f"{chunk['start_line']}-{chunk['end_line']}"
+            output.append({"id": chunk["id"], "ref": f"{file}:{lines_str}"})
+        return output
```

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/diff.py` & `ragdaemon-0.3.0/ragdaemon/annotators/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import re
 from pathlib import Path
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import Database
+from ragdaemon.database import Database, remove_add_to_db_duplicates
 from ragdaemon.get_paths import get_git_root_for_path
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str, parse_path_ref, truncate
 
 
 def get_chunks_from_diff(id: str, diff: str) -> dict[str, str]:
@@ -134,15 +134,15 @@
                     "id": chunk_id,
                     "ref": chunk_ref,
                     "type": "diff",
                     "checksum": chunk_checksum,
                     "active": False,
                 }
                 document, truncate_ratio = truncate(document, db.embedding_model)
-                if truncate_ratio < 1 and self.verbose:
+                if truncate_ratio > 0 and self.verbose:
                     print(f"Truncated diff chunk {chunk_id} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(chunk_checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(data)
             else:
                 data = existing_records["metadatas"][0]
             graph.add_node(chunk_id, **data)
@@ -172,10 +172,11 @@
                     _link_to_successors(successor, visited)
 
             _link_to_successors(file_str)
 
         for source, origin in edges_to_add:
             graph.add_edge(source, origin, type="diff")
         if len(add_to_db["ids"]) > 0:
+            add_to_db = remove_add_to_db_duplicates(**add_to_db)
             db.upsert(**add_to_db)
 
         return graph
```

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.3.0/ragdaemon/annotators/hierarchy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import Database
+from ragdaemon.database import Database, remove_add_to_db_duplicates
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str, truncate
 
 
 def get_active_checksums(
@@ -47,14 +47,15 @@
             checksums[path] = checksum
         except UnicodeDecodeError:  # Ignore non-text files
             pass
         except RagdaemonError as e:
             if verbose:
                 print(f"Error processing path {path}: {e}")
     if len(add_to_db["ids"]) > 0:
+        add_to_db = remove_add_to_db_duplicates(**add_to_db)
         db.upsert(**add_to_db)
     return checksums
 
 
 def files_checksum(cwd: Path, ignore_patterns: set[Path] = set()) -> str:
     timestamps = ""
     for path in get_paths_for_directory(cwd, exclude_patterns=ignore_patterns):
```

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.3.0/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.3.0/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/database/__init__.py` & `ragdaemon-0.3.0/ragdaemon/database/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 from pathlib import Path
 from typing import Optional
 
 from spice import Spice
 from spice.errors import SpiceError
 
-from ragdaemon.database.chroma_database import ChromaDB
+from ragdaemon.database.chroma_database import ChromaDB, remove_add_to_db_duplicates
 from ragdaemon.database.database import Database
 from ragdaemon.database.lite_database import LiteDB
 from ragdaemon.utils import mentat_dir_path
 
 DEFAULT_EMBEDDING_MODEL = "text-embedding-3-large"
 
 
 def get_db(
     cwd: Path,
     spice_client: Spice,
     embedding_model: str | None = None,
     embedding_provider: Optional[str] = None,
+    verbose: bool = False,
 ) -> Database:
     db_path = mentat_dir_path / "chroma"
     db_path.mkdir(parents=True, exist_ok=True)
     if embedding_model is not None and "PYTEST_CURRENT_TEST" not in os.environ:
         try:
             db = ChromaDB(
                 cwd=cwd,
@@ -30,10 +31,12 @@
                 embedding_model=embedding_model,
                 embedding_provider=embedding_provider,
             )
             # In case the api key is wrong, try to embed something to trigger an error.
             _ = db.add(ids="test", documents="test doc")
             db.delete(ids="test")
             return db
-        except Exception:
+        except Exception as e:
+            if verbose:
+                print(f"Failed to initialize ChromaDB: {e}. Falling back to LiteDB.")
             pass
     return LiteDB(cwd=cwd, db_path=db_path)
```

### Comparing `ragdaemon-0.2.9/ragdaemon/database/chroma_database.py` & `ragdaemon-0.3.0/ragdaemon/database/chroma_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 from pathlib import Path
-from typing import cast, TYPE_CHECKING, Optional
+from typing import Any, TYPE_CHECKING, Optional, cast
 
 from spice import Spice
 
 from ragdaemon.database.database import Database
 from ragdaemon.errors import RagdaemonError
+from ragdaemon import __version__
 
 MAX_INPUTS_PER_CALL = 2048
 
 if TYPE_CHECKING:
     from chromadb.api.types import (
-        Metadata,
         GetResult,
-    )  # noqa: F401
+        Metadata,
+    )
+
+
+def remove_add_to_db_duplicates(
+    ids: list[str], documents: list[str], metadatas: list[dict]
+) -> dict[str, Any]:
+    seen = set()
+    output = {"ids": [], "documents": [], "metadatas": []}
+    for id, document, metadata in zip(ids, documents, metadatas):
+        if id not in seen:
+            output["ids"].append(id)
+            output["documents"].append(document)
+            output["metadatas"].append(metadata)
+            seen.add(id)
+    return output
 
 
 class ChromaDB(Database):
     def __init__(
         self,
         cwd: Path,
         db_path: Path,
@@ -25,15 +40,19 @@
         embedding_provider: Optional[str] = None,
     ) -> None:
         self.cwd = cwd
         self.db_path = db_path
         self.embedding_model = embedding_model
 
         import chromadb  # Imports are slow so do it lazily
-        from chromadb.api.types import Embeddable, EmbeddingFunction, Embeddings  # noqa: F811
+        from chromadb.api.types import (
+            Embeddable,
+            EmbeddingFunction,
+            Embeddings,
+        )
 
         class SpiceEmbeddingFunction(EmbeddingFunction[Embeddable]):
             def __call__(self, input_texts: Embeddable) -> Embeddings:
                 if not all(isinstance(item, str) for item in input_texts):
                     raise RagdaemonError("SpiceEmbeddings only enabled for text files.")
                 input_texts = cast(list[str], input_texts)
                 # Embed in batches
@@ -49,15 +68,16 @@
                     ).embeddings
                     output.extend(embeddings)
                 return output
 
         embedding_function = SpiceEmbeddingFunction()
 
         _client = chromadb.PersistentClient(path=str(db_path))
-        name = f"ragdaemon-{self.cwd.name}-{self.embedding_model}"
+        minor_version = ".".join(__version__.split(".")[:2])
+        name = f"ragdaemon-{minor_version}-{self.embedding_model}"
         self._collection = _client.get_or_create_collection(
             name=name,
             embedding_function=embedding_function,
         )
 
     def query(self, query: str, active_checksums: list[str]) -> list[dict]:
         # Flag active records
```

### Comparing `ragdaemon-0.2.9/ragdaemon/database/database.py` & `ragdaemon-0.3.0/ragdaemon/database/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,19 +44,19 @@
                 name = result["id"].split(":")[1]
                 if "." in name:
                     name = name.split(".")[-1]
             else:
                 name = ""  # not applicable for diffs
 
             if query in name:
-                distance *= 2
+                distance *= 0.5
             elif query in result["id"]:
-                distance *= 1.5
+                distance *= 0.75
             elif query in result["document"]:
-                distance *= 1.1
+                distance *= 0.9
 
             result["distance"] = distance
-        results = sorted(results, key=lambda x: x["distance"], reverse=True)
+        results = sorted(results, key=lambda x: x["distance"])
 
         if n:
             results = results[:n]
         return results
```

### Comparing `ragdaemon-0.2.9/ragdaemon/database/lite_database.py` & `ragdaemon-0.3.0/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/favicon.ico` & `ragdaemon-0.3.0/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.3.0/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/js/main.js` & `ragdaemon-0.3.0/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.3.0/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/js/three/node.js` & `ragdaemon-0.3.0/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.3.0/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/ragdaemon/templates/index.html` & `ragdaemon-0.3.0/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/conftest.py` & `ragdaemon-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/test_comments.py` & `ragdaemon-0.3.0/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/test_context.py` & `ragdaemon-0.3.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/test_daemon.py` & `ragdaemon-0.3.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/test_get_paths.py` & `ragdaemon-0.3.0/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/test_sample.py` & `ragdaemon-0.3.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/annotators/test_chunker.py` & `ragdaemon-0.3.0/tests/annotators/test_chunker.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ragdaemon.graph import KnowledgeGraph
 
 
 @pytest.fixture
 def mock_get_llm_response():
     with patch(
         "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
-        return_value={"chunks": []},
+        return_value={"chunks_llm": []},
     ) as mock:
         yield mock
 
 
 def test_chunker_is_complete(cwd, mock_db):
     chunker = Chunker()
 
@@ -57,8 +57,8 @@
     )
     chunker = ChunkerLLM(spice_client=AsyncMock())
     actual = await chunker.annotate(daemon.graph, mock_db)
 
     for node, data in actual.nodes(data=True):
         assert data, f"Node {node} is missing data"
         if data["type"] == "file" and Path(node).suffix in chunker.chunk_extensions:
-            assert "chunks" in data, f"File {node} is missing chunks"
+            assert "chunks_llm" in data, f"File {node} is missing chunks"
```

### Comparing `ragdaemon-0.2.9/tests/annotators/test_diff.py` & `ragdaemon-0.3.0/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/annotators/test_hierarchy.py` & `ragdaemon-0.3.0/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.3.0/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/annotators/test_summarizer.py` & `ragdaemon-0.3.0/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/data/chunker_graph.json` & `ragdaemon-0.3.0/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/data/context_message.txt` & `ragdaemon-0.3.0/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/data/diff_graph.json` & `ragdaemon-0.3.0/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/data/hierarchy_graph.json` & `ragdaemon-0.3.0/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.3.0/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/tests/sample/src/interface.py` & `ragdaemon-0.3.0/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/LICENSE` & `ragdaemon-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/README.md` & `ragdaemon-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.9/pyproject.toml` & `ragdaemon-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.9"
+version = "0.3.0"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.2.9/PKG-INFO` & `ragdaemon-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.9
+Version: 0.3.0
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

