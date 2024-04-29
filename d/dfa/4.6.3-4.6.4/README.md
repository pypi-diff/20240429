# Comparing `tmp/dfa-4.6.3.tar.gz` & `tmp/dfa-4.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfa-4.6.3.tar", max compression
+gzip compressed data, was "dfa-4.6.4.tar", max compression
```

## Comparing `dfa-4.6.3.tar` & `dfa-4.6.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1082 2022-09-27 18:24:23.678548 dfa-4.6.3/LICENSE
--rw-r--r--   0        0        0     7737 2022-11-03 04:44:43.584740 dfa-4.6.3/README.md
--rw-r--r--   0        0        0      230 2022-09-27 18:24:23.679549 dfa-4.6.3/dfa/__init__.py
--rw-r--r--   0        0        0    10955 2022-10-25 19:23:00.579182 dfa-4.6.3/dfa/dfa.py
--rw-r--r--   0        0        0      649 2022-09-27 18:24:23.679549 dfa-4.6.3/dfa/draw.py
--rw-r--r--   0        0        0     5695 2022-09-28 03:58:40.560740 dfa-4.6.3/dfa/utils.py
--rw-r--r--   0        0        0      666 2022-11-03 04:46:50.009605 dfa-4.6.3/pyproject.toml
--rw-r--r--   0        0        0     8907 2022-11-03 04:47:19.724910 dfa-4.6.3/setup.py
--rw-r--r--   0        0        0     8546 2022-11-03 04:47:19.725656 dfa-4.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-03-10 00:27:29.678094 dfa-4.6.4/LICENSE
+-rw-r--r--   0        0        0     7737 2024-03-10 00:27:29.678094 dfa-4.6.4/README.md
+-rw-r--r--   0        0        0      230 2024-03-10 00:27:29.678094 dfa-4.6.4/dfa/__init__.py
+-rw-r--r--   0        0        0    11108 2024-04-29 01:46:33.514822 dfa-4.6.4/dfa/dfa.py
+-rw-r--r--   0        0        0      649 2024-03-10 00:27:29.679094 dfa-4.6.4/dfa/draw.py
+-rw-r--r--   0        0        0     5695 2024-03-10 00:27:29.679094 dfa-4.6.4/dfa/utils.py
+-rw-r--r--   0        0        0      670 2024-04-29 02:01:18.341259 dfa-4.6.4/pyproject.toml
+-rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 dfa-4.6.4/PKG-INFO
```

### Comparing `dfa-4.6.3/LICENSE` & `dfa-4.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dfa-4.6.3/README.md` & `dfa-4.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dfa-4.6.3/dfa/dfa.py` & `dfa-4.6.4/dfa/dfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     return wrapped
 
 
 def bits_needed(n: int) -> int:
     return 0 if n < 2 else len(bin(n - 1)) - 2
 
 
+def evolve(d: DFA, *args, **kwargs) -> DFA:
+    kwargs.setdefault('states', None)
+    kwargs.setdefault('hash', None)
+    return attr.evolve(d, *args, **kwargs)
+
+
 @attr.frozen(auto_detect=True)
 class DFA:
     start: State
     _label: Callable[[State], Letter] = attr.ib(
         converter=cache
     )
     _transition: Callable[[State, Letter], State] = attr.ib(
@@ -232,15 +238,15 @@
             state = self._transition(state, char)
             yield state
 
     def transition(self, word, *, start=None):
         return fn.last(self.trace(word, start=start))
 
     def advance(self, word, *, start=None):
-        return attr.evolve(self, start=self.transition(word, start=start))
+        return evolve(self, start=self.transition(word, start=start))
 
     def label(self, word, *, start=None):
         output = self._label(self.transition(word, start=start))
         assert (self.outputs is None) or (output in self.outputs)
         return output
 
     def transduce(self, word, *, start=None):
@@ -284,15 +290,15 @@
 
         Returns shortest word if one exists. Otherwise None.
         """
         return fn.first(w for s, w in self.walk() if self._label(s) == label)
 
     @boolean_only
     def __invert__(self):
-        return attr.evolve(self, label=lambda s: not self._label(s))
+        return evolve(self, label=lambda s: not self._label(s))
 
     def _bin_op(self, other, op):
         if self.inputs != other.inputs:
             raise ValueError(f"{op} requires shared inputs.")
         return DFA(
             start=(self.start, other.start),
             inputs=self.inputs,  # Assumed shared alphabet
```

### Comparing `dfa-4.6.3/dfa/draw.py` & `dfa-4.6.4/dfa/draw.py`

 * *Files identical despite different names*

### Comparing `dfa-4.6.3/dfa/utils.py` & `dfa-4.6.4/dfa/utils.py`

 * *Files identical despite different names*

### Comparing `dfa-4.6.3/pyproject.toml` & `dfa-4.6.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "dfa"
 readme="README.md"
-version = "4.6.3"
+version = "4.6.4"
 description = "Python library for modeling DFAs, Moore Machines, and Transition Systems."
 authors = ["Marcell Vazquez-Chanlatte <marcell.vc@eecs.berkeley.edu>"]
 repository = "https://github.com/mvcisback/dfa"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-attrs = "^22"
-funcy = "^1.12"
-pydot = {version = "^1.4", optional = true}
-bidict = "^0.22"
+attrs = ">=22"
+funcy = ">=1,<3"
+pydot = {version = ">=1.4", optional = true}
+bidict = ">=0.22"
 bitarray = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pydot = "^1.4"
 pytest = "^7.2"
 dill = "^0.3.5"
 hypothesis = "^6.56.4"
```

### Comparing `dfa-4.6.3/setup.py` & `dfa-4.6.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,340 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dfa
+Version: 4.6.4
+Summary: Python library for modeling DFAs, Moore Machines, and Transition Systems.
+Home-page: https://github.com/mvcisback/dfa
+License: MIT
+Author: Marcell Vazquez-Chanlatte
+Author-email: marcell.vc@eecs.berkeley.edu
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: draw
+Requires-Dist: attrs (>=22)
+Requires-Dist: bidict (>=0.22)
+Requires-Dist: bitarray (>=2.4.0,<3.0.0)
+Requires-Dist: funcy (>=1,<3)
+Requires-Dist: pydot (>=1.4) ; extra == "draw"
+Project-URL: Repository, https://github.com/mvcisback/dfa
+Description-Content-Type: text/markdown
 
-packages = \
-['dfa']
+# DFA
 
-package_data = \
-{'': ['*']}
+A simple python implementation of a DFA. 
 
-install_requires = \
-['attrs>=22,<23',
- 'bidict>=0.22,<0.23',
- 'bitarray>=2.4.0,<3.0.0',
- 'funcy>=1.12,<2.0']
-
-extras_require = \
-{'draw': ['pydot>=1.4,<2.0']}
-
-setup_kwargs = {
-    'name': 'dfa',
-    'version': '4.6.3',
-    'description': 'Python library for modeling DFAs, Moore Machines, and Transition Systems.',
-    'long_description': '# DFA\n\nA simple python implementation of a DFA. \n\n[![Build Status](https://cloud.drone.io/api/badges/mvcisback/dfa/status.svg)](https://cloud.drone.io/mvcisback/dfa)\n[![PyPI version](https://badge.fury.io/py/dfa.svg)](https://badge.fury.io/py/dfa)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n<!-- markdown-toc start - Don\'t edit this section. Run M-x markdown-toc-generate-toc again -->\n**Table of Contents**\n\n- [Installation](#installation)\n- [Usage](#usage)\n    - [Membership Queries](#membership-queries)\n    - [Transitions and Traces](#transitions-and-traces)\n    - [Non-boolean output alphabets](#non-boolean-output-alphabets)\n    - [Moore Machines](#moore-machines)\n    - [DFA <-> Dictionary](#dfa---dictionary)\n    - [Computing Reachable States](#computing-reachable-states)\n    - [Sampling Paths](#sampling-paths)\n    - [Running interactively (Co-Routine API)](#running-interactively-co-routine-api)\n    - [Visualizing DFAs](#visualizing-dfas)\n\n<!-- markdown-toc end -->\n\n\n**Features:**\n\n1. State can be any Hashable object.\n2. Alphabet can be any finite sequence of Hashable objects.\n3. Designed to be immutable and hashable (assuming components are\n   immutable and hashable).\n4. Design choice to allow transition map and accepting set to be\n   given as functions rather than an explicit `dict` or `set`.\n\n# Installation\n\nIf you just need to use `dfa`, you can just run:\n\n`$ pip install dfa`\n\nFor developers, note that this project uses the\n[poetry](https://poetry.eustace.io/) python package/dependency\nmanagement tool. Please familarize yourself with it and then\nrun:\n\n`$ poetry install`\n\n# Usage\n\nThe `dfa` api is centered around the `DFA` object. \n\nBy default, the `DFA` object models a `Deterministic Finite Acceptor`,\ne.g., a recognizer of a Regular Language. \n\n**Example Usage:**\n```python\nfrom dfa import DFA\n\ndfa1 = DFA(\n    start=0,\n    inputs={0, 1},\n    label=lambda s: (s % 4) == 3,\n    transition=lambda s, c: (s + c) % 4,\n)\n\ndfa2 = DFA(\n    start="left",\n    inputs={"move right", "move left"},\n    label=lambda s: s == "left",\n    transition=lambda s, c: "left" if c == "move left" else "right",\n)\n```\n\n## Membership Queries\n\n```python\nassert dfa1.label([1, 1, 1, 1])\nassert not dfa1.label([1, 0])\n\nassert dfa2.label(["move right"]*100 + ["move left"])\nassert not dfa2.label(["move left", "move right"])\n```\n\n## Transitions and Traces\n\n```python\nassert dfa1.transition([1, 1, 1]) == 3\nassert list(dfa1.trace([1, 1, 1])) == [0, 1, 2, 3]\n```\n\n## Non-boolean output alphabets\n\nSometimes, it is useful to model an automata which can label a word\nusing a non-Boolean alphabet. For example, `{True, False, UNSURE}`.\n\nThe `DFA` object supports this by specifying the output alphabet.\n\n```python\nUNSURE = None\n\ndef my_labeler(s):\n    if s % 4 == 2:\n       return None\n    return (s % 4) == 3\n\n\ndfa3 = DFA(\n    start=0,\n    inputs={0, 1},\n    label=my_labeler,\n    transition=lambda s, c: (s + c) % 4,\n    outputs={True, False, UNSURE},\n)\n```\n\n**Note:** If `outputs` is set to `None`, then no checks are done that\nthe outputs are within the output alphabet.\n\n```python\ndfa3 = DFA(\n    start=0,\n    inputs={0, 1},\n    label=my_labeler,\n    transition=lambda s, c: (s + c) % 4,\n    outputs=None,\n)\n```\n\n## Moore Machines\n\nFinally, by reinterpreting the structure of the `DFA` object, one can\nmodel a Moore Machine. For example, in 3 state counter, `dfa1`, the\nMoore Machine can output the current count.\n\n```python\nassert dfa1.transduce(()) == ()\nassert dfa1.transduce((1,)) == (False,)\nassert dfa1.transduce((1, 1, 1, 1)) == (False, False, False, True)\n```\n\n## Language Queries\n\nUtility functions are available for testing if a language:\n\n1. Is empty: `utils.find_word`\n2. Is equivilent to another language: `utils.find_equiv_counterexample`\n3. Is a subset of a another language: `utils.find_subset_counterexample`\n\nThese operate by returning `None` if the property holds, i.e.,\n`lang(dfa1) = ∅, lang(dfa1) ≡ lang(dfa2), lang(dfa1) ⊆ lang(dfa2)`, and\nreturning a counterexample `Word` otherwise.\n\n## DFA <-> Dictionary\n\nNote that `dfa` provides helper functions for going from a dictionary\nbased representation of a deterministic transition system to a `DFA`\nobject and back.\n\n```python\nfrom dfa import dfa2dict, dict2dfa\n\n# DFA encoded a nested dictionaries with the following\n# signature.\n#     <state>: (<label>, {<action>: <next state>})\n\ndfa_dict = {\n    0: (False, {0: 0, 1: 1}),\n    1: (False, {0: 1, 1: 2}),\n    2: (False, {0: 2, 1: 3}), \n    3: (True, {0: 3, 1: 0})\n}\n\n# Dictionary -> DFA\ndfa = dict2dfa(dfa_dict, start=0)\n\n# DFA -> Dictionary\ndfa_dict2, start = dfa2dict(dfa)\n\nassert (dfa_dict, 0) == (dfa_dict2, start)\n```\n\n## Computing Reachable States\n\n```python\n# Perform a depth first traversal to collect all reachable states.\nassert dfa1.states() == {0, 1, 2, 3}\n```\n\n## Finding Words and Access strings\n\nTo generate accepting strings (words) in a DFA (breadth first using string length) one can use the `dfa.utils.words` function:\n\n```python\nfrom dfa.utils.import dfa2dict, words, find_words\n\ndfa_dict = {\n    0: (False, {0: 0, 1: 1}),\n    1: (False, {0: 1, 1: 2}),\n    2: (False, {0: 2, 1: 3}),\n    3: (True, {0: 3, 1: 0})\n}\nlang = dict2dfa(dfa_dict, start=0)\n\nxs = set(fn.take(5, words(lang)))\nassert len(xs) == 5\nassert all(lang.label(x) for x in xs)\n```\n\nTo get a single word, a helper function is provided in `dfa.utils.find_word` which returns `None` if the language of the DFA is empty:\n\n```python\n# ... Same as above ...\n\nx = find_word(lang)\nassert x is not None\nassert lang.label(x)\n```\n\n\nOften times, it is useful to sample a path between two states, say `a`\nand `b`. `dfa` supports this using `dfa.utils.paths`. This function\nreturns a generator of words, `w`, such that `dfa.transition(w,\nstart=b) == a`. For example:\n\n\n```python\nfrom dfa.utils import paths\n\naccess_strings = paths(\n    dfa1, \n    start=0,\n    end=1,  # Optional. If not specified returns all paths\n            # starting at `start`.\n    max_length=7,  #  Defaults to float(\'inf\')\n    randomize=True,  #  Randomize the order. Shorter paths still found first.\n)\n\nfor word in access_strings:\n    assert dfa1.transition(word, start=0) == 1\n```\n\n## DFA minimization\n\nDFAs can be minimized using the `minimize` method.\n\n```python\nmy_dfa = my_dfa.minimize()\n```\n\n## DFA advancement (progression)\n\nOne can create the DFA starting at the state indexed by a given word by using\nthe `advance` method. \n\n```python\nmy_dfa = my_dfa.advance(word)\n```\n\n\n## Running interactively (Co-Routine API)\n\n`dfa` supports interactively stepping through a `DFA` object via\nco-routines. This is particularly useful when using DFA in a control\nloop. For example, the following code counts how many `1`\'s it takes\nto advance `dfa1`\'s state back to the start state.\n\n```python\n\nmachine = dfa1.run()\n\nnext(machine)\nstate = None\n\ncount = 0\nwhile state != dfa1.start:\n    count += 1\n    state = machine.send(1)\n```\n\n## Visualizing DFAs\n\n`dfa` optionally supports visualizing DFAs using graphviz. To use this\nfunctionality be sure to install `dfa` using with the `draw` option:\n\n```python\npip install dfa[draw]\n```\n\nor \n\n```python\npoetry install -E draw\n```\n\nThen one can simply use `dfa.draw.write_dot` to write a `.dot` file\nrepresenting the DFA. This `.dot` file can be rendered using any\ngraphviz supporting tool.\n\n```python\nfrom dfa.draw import write_dot\n\nwrite_dot(dfa1, "path/to/dfa1.dot")\n```\n\nUsing the `dot` command in linux results in the following rendering of `dfa1`.\n\n`$ dot -Tsvg path/to/dfa1.dot > dfa1.svg`\n\n<figure>\n  <img src="assets/dfa1.svg" alt="visualization of dfa1" width=500px>\n  <figcaption>\n    Visualization of dfa1 using graphviz.\n  </figcaption>\n</figure>\n',
-    'author': 'Marcell Vazquez-Chanlatte',
-    'author_email': 'marcell.vc@eecs.berkeley.edu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mvcisback/dfa',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
+[![Build Status](https://cloud.drone.io/api/badges/mvcisback/dfa/status.svg)](https://cloud.drone.io/mvcisback/dfa)
+[![PyPI version](https://badge.fury.io/py/dfa.svg)](https://badge.fury.io/py/dfa)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
+**Table of Contents**
+
+- [Installation](#installation)
+- [Usage](#usage)
+    - [Membership Queries](#membership-queries)
+    - [Transitions and Traces](#transitions-and-traces)
+    - [Non-boolean output alphabets](#non-boolean-output-alphabets)
+    - [Moore Machines](#moore-machines)
+    - [DFA <-> Dictionary](#dfa---dictionary)
+    - [Computing Reachable States](#computing-reachable-states)
+    - [Sampling Paths](#sampling-paths)
+    - [Running interactively (Co-Routine API)](#running-interactively-co-routine-api)
+    - [Visualizing DFAs](#visualizing-dfas)
+
+<!-- markdown-toc end -->
+
+
+**Features:**
+
+1. State can be any Hashable object.
+2. Alphabet can be any finite sequence of Hashable objects.
+3. Designed to be immutable and hashable (assuming components are
+   immutable and hashable).
+4. Design choice to allow transition map and accepting set to be
+   given as functions rather than an explicit `dict` or `set`.
+
+# Installation
+
+If you just need to use `dfa`, you can just run:
+
+`$ pip install dfa`
+
+For developers, note that this project uses the
+[poetry](https://poetry.eustace.io/) python package/dependency
+management tool. Please familarize yourself with it and then
+run:
+
+`$ poetry install`
+
+# Usage
+
+The `dfa` api is centered around the `DFA` object. 
+
+By default, the `DFA` object models a `Deterministic Finite Acceptor`,
+e.g., a recognizer of a Regular Language. 
+
+**Example Usage:**
+```python
+from dfa import DFA
+
+dfa1 = DFA(
+    start=0,
+    inputs={0, 1},
+    label=lambda s: (s % 4) == 3,
+    transition=lambda s, c: (s + c) % 4,
+)
+
+dfa2 = DFA(
+    start="left",
+    inputs={"move right", "move left"},
+    label=lambda s: s == "left",
+    transition=lambda s, c: "left" if c == "move left" else "right",
+)
+```
+
+## Membership Queries
+
+```python
+assert dfa1.label([1, 1, 1, 1])
+assert not dfa1.label([1, 0])
+
+assert dfa2.label(["move right"]*100 + ["move left"])
+assert not dfa2.label(["move left", "move right"])
+```
+
+## Transitions and Traces
+
+```python
+assert dfa1.transition([1, 1, 1]) == 3
+assert list(dfa1.trace([1, 1, 1])) == [0, 1, 2, 3]
+```
+
+## Non-boolean output alphabets
+
+Sometimes, it is useful to model an automata which can label a word
+using a non-Boolean alphabet. For example, `{True, False, UNSURE}`.
+
+The `DFA` object supports this by specifying the output alphabet.
+
+```python
+UNSURE = None
+
+def my_labeler(s):
+    if s % 4 == 2:
+       return None
+    return (s % 4) == 3
+
+
+dfa3 = DFA(
+    start=0,
+    inputs={0, 1},
+    label=my_labeler,
+    transition=lambda s, c: (s + c) % 4,
+    outputs={True, False, UNSURE},
+)
+```
+
+**Note:** If `outputs` is set to `None`, then no checks are done that
+the outputs are within the output alphabet.
+
+```python
+dfa3 = DFA(
+    start=0,
+    inputs={0, 1},
+    label=my_labeler,
+    transition=lambda s, c: (s + c) % 4,
+    outputs=None,
+)
+```
+
+## Moore Machines
+
+Finally, by reinterpreting the structure of the `DFA` object, one can
+model a Moore Machine. For example, in 3 state counter, `dfa1`, the
+Moore Machine can output the current count.
+
+```python
+assert dfa1.transduce(()) == ()
+assert dfa1.transduce((1,)) == (False,)
+assert dfa1.transduce((1, 1, 1, 1)) == (False, False, False, True)
+```
+
+## Language Queries
+
+Utility functions are available for testing if a language:
+
+1. Is empty: `utils.find_word`
+2. Is equivilent to another language: `utils.find_equiv_counterexample`
+3. Is a subset of a another language: `utils.find_subset_counterexample`
+
+These operate by returning `None` if the property holds, i.e.,
+`lang(dfa1) = ∅, lang(dfa1) ≡ lang(dfa2), lang(dfa1) ⊆ lang(dfa2)`, and
+returning a counterexample `Word` otherwise.
+
+## DFA <-> Dictionary
+
+Note that `dfa` provides helper functions for going from a dictionary
+based representation of a deterministic transition system to a `DFA`
+object and back.
+
+```python
+from dfa import dfa2dict, dict2dfa
+
+# DFA encoded a nested dictionaries with the following
+# signature.
+#     <state>: (<label>, {<action>: <next state>})
+
+dfa_dict = {
+    0: (False, {0: 0, 1: 1}),
+    1: (False, {0: 1, 1: 2}),
+    2: (False, {0: 2, 1: 3}), 
+    3: (True, {0: 3, 1: 0})
 }
 
+# Dictionary -> DFA
+dfa = dict2dfa(dfa_dict, start=0)
+
+# DFA -> Dictionary
+dfa_dict2, start = dfa2dict(dfa)
+
+assert (dfa_dict, 0) == (dfa_dict2, start)
+```
+
+## Computing Reachable States
+
+```python
+# Perform a depth first traversal to collect all reachable states.
+assert dfa1.states() == {0, 1, 2, 3}
+```
+
+## Finding Words and Access strings
+
+To generate accepting strings (words) in a DFA (breadth first using string length) one can use the `dfa.utils.words` function:
+
+```python
+from dfa.utils.import dfa2dict, words, find_words
+
+dfa_dict = {
+    0: (False, {0: 0, 1: 1}),
+    1: (False, {0: 1, 1: 2}),
+    2: (False, {0: 2, 1: 3}),
+    3: (True, {0: 3, 1: 0})
+}
+lang = dict2dfa(dfa_dict, start=0)
+
+xs = set(fn.take(5, words(lang)))
+assert len(xs) == 5
+assert all(lang.label(x) for x in xs)
+```
+
+To get a single word, a helper function is provided in `dfa.utils.find_word` which returns `None` if the language of the DFA is empty:
+
+```python
+# ... Same as above ...
+
+x = find_word(lang)
+assert x is not None
+assert lang.label(x)
+```
+
+
+Often times, it is useful to sample a path between two states, say `a`
+and `b`. `dfa` supports this using `dfa.utils.paths`. This function
+returns a generator of words, `w`, such that `dfa.transition(w,
+start=b) == a`. For example:
+
+
+```python
+from dfa.utils import paths
+
+access_strings = paths(
+    dfa1, 
+    start=0,
+    end=1,  # Optional. If not specified returns all paths
+            # starting at `start`.
+    max_length=7,  #  Defaults to float('inf')
+    randomize=True,  #  Randomize the order. Shorter paths still found first.
+)
+
+for word in access_strings:
+    assert dfa1.transition(word, start=0) == 1
+```
+
+## DFA minimization
+
+DFAs can be minimized using the `minimize` method.
+
+```python
+my_dfa = my_dfa.minimize()
+```
+
+## DFA advancement (progression)
+
+One can create the DFA starting at the state indexed by a given word by using
+the `advance` method. 
+
+```python
+my_dfa = my_dfa.advance(word)
+```
+
+
+## Running interactively (Co-Routine API)
+
+`dfa` supports interactively stepping through a `DFA` object via
+co-routines. This is particularly useful when using DFA in a control
+loop. For example, the following code counts how many `1`'s it takes
+to advance `dfa1`'s state back to the start state.
+
+```python
+
+machine = dfa1.run()
+
+next(machine)
+state = None
+
+count = 0
+while state != dfa1.start:
+    count += 1
+    state = machine.send(1)
+```
+
+## Visualizing DFAs
+
+`dfa` optionally supports visualizing DFAs using graphviz. To use this
+functionality be sure to install `dfa` using with the `draw` option:
+
+```python
+pip install dfa[draw]
+```
+
+or 
+
+```python
+poetry install -E draw
+```
+
+Then one can simply use `dfa.draw.write_dot` to write a `.dot` file
+representing the DFA. This `.dot` file can be rendered using any
+graphviz supporting tool.
+
+```python
+from dfa.draw import write_dot
+
+write_dot(dfa1, "path/to/dfa1.dot")
+```
+
+Using the `dot` command in linux results in the following rendering of `dfa1`.
+
+`$ dot -Tsvg path/to/dfa1.dot > dfa1.svg`
+
+<figure>
+  <img src="assets/dfa1.svg" alt="visualization of dfa1" width=500px>
+  <figcaption>
+    Visualization of dfa1 using graphviz.
+  </figcaption>
+</figure>
 
-setup(**setup_kwargs)
```

