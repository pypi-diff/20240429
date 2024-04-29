# Comparing `tmp/pyrsistent-extras-0.1.0.tar.gz` & `tmp/pyrsistent-extras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsistent-extras-0.1.0.tar", last modified: Fri Sep 23 19:47:09 2022, max compression
+gzip compressed data, was "pyrsistent-extras-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyrsistent-extras-0.1.0.tar` & `pyrsistent-extras-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:47:09.501417 pyrsistent-extras-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/LICENSE.mit
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-09-23 19:47:09.497417 pyrsistent-extras-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:47:09.497417 pyrsistent-extras-0.1.0/pyrsistent_extras/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20420 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_pheap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:47:09.497417 pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19741 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)   130759 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/_c_ext.c
--rw-r--r--   0 runner    (1001) docker     (121)    30784 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/pyrsistent_extras/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 19:47:09.497417 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-09-23 19:47:09.000000 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-09-23 19:47:09.000000 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 19:47:09.000000 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-23 19:47:09.000000 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-23 19:47:09.000000 pyrsistent-extras-0.1.0/pyrsistent_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 19:47:09.501417 pyrsistent-extras-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-09-23 19:46:58.000000 pyrsistent-extras-0.1.0/setup.py
+-rw-r--r--   0        0        0     3351 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/.github/workflows/mypy.yaml
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/.gitignore
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/LICENSE.mit
+-rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/README.rst
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      741 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/docs/source/api/pheap.rst
+-rw-r--r--   0        0        0      365 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/docs/source/api/psequence.rst
+-rw-r--r--   0        0        0      754 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/__init__.py
+-rw-r--r--   0        0        0    21070 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_pheap.py
+-rw-r--r--   0        0        0      916 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/__init__.py
+-rw-r--r--   0        0        0    19486 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/_base.py
+-rw-r--r--   0        0        0   126647 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/_c_ext.c
+-rw-r--r--   0        0        0    20777 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/_c_ext.h
+-rw-r--r--   0        0        0     1881 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_utility.py
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/_version.py
+-rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/lenses.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/src/pyrsistent_extras/py.typed
+-rw-r--r--   0        0        0     8872 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/tests/pheap_test.py
+-rw-r--r--   0        0        0    36378 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/tests/psequence_test.py
+-rwxr-xr-x   0        0        0      691 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/tools/test_coverage.sh
+-rwxr-xr-x   0        0        0      321 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/tools/test_wheels.sh
+-rw-r--r--   0        0        0     5276 2022-11-09 12:37:21.000000 pyrsistent-extras-0.1.1/PKG-INFO
```

### Comparing `pyrsistent-extras-0.1.0/LICENSE.mit` & `pyrsistent-extras-0.1.1/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `pyrsistent-extras-0.1.0/PKG-INFO` & `pyrsistent-extras-0.1.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1
-Name: pyrsistent-extras
-Version: 0.1.0
-Summary: Extra data structures for pyrsistent
-Home-page: http://github.com/mingmingrr/pyrsistent-extras
-Author: mingmingrr
-Author-email: mingmingrr@gmail.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE.mit
+Pyrsistent-Extras
+=================
 
+|docs-badge| |coverage-badge| |tests-badge| |mypy-badge| |pypi-badge|
+
+.. |docs-badge| image:: https://readthedocs.org/projects/pyrsistent-extras/badge/?version=latest
+	:target: https://pyrsistent-extras.readthedocs.io/en/latest/?badge=latest
+.. |coverage-badge| image:: https://coveralls.io/repos/github/mingmingrr/pyrsistent-extras/badge.svg?branch=main
+	:target: https://coveralls.io/github/mingmingrr/pyrsistent-extras?branch=main
+.. |tests-badge| image:: https://github.com/mingmingrr/pyrsistent-extras/actions/workflows/tests.yaml/badge.svg
+	:target: https://github.com/mingmingrr/pyrsistent-extras/actions/workflows/tests.yaml
+.. |mypy-badge| image:: https://github.com/mingmingrr/pyrsistent-extras/actions/workflows/mypy.yaml/badge.svg
+	:target: https://github.com/mingmingrr/pyrsistent-extras/actions/workflows/mypy.yaml
+.. |pypi-badge| image:: https://badge.fury.io/py/pyrsistent-extras.svg
+	:target: https://badge.fury.io/py/pyrsistent-extras
 
 Extra data structures for `pyrsistent <http://github.com/tobgu/pyrsistent>`_
 
 Below are examples of common usage patterns for some of the structures and
 features. More information and full documentation for all data structures is
 available in the `documentation <http://pyrsistent-extras.readthedocs.org>`_.
```

### Comparing `pyrsistent-extras-0.1.0/pyrsistent_extras/_pheap.py` & `pyrsistent-extras-0.1.1/src/pyrsistent_extras/_pheap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 from __future__ import annotations
-from typing import Collection, Iterable, Iterator, Hashable, \
-	ClassVar, TypeVar, Generic, Optional, Callable, Tuple, Any, Union, cast
+from typing import Collection, Iterable, Iterator, Hashable, ClassVar, \
+	TypeVar, Generic, Optional, Callable, Tuple, Any, Union, cast, overload
 from abc import abstractmethod
 
 import itertools
 import operator
 import builtins
 
-from ._util import Comparable, compare_next, compare_iter, sphinx_build
+from ._utility import Comparable, compare_next, compare_iter, sphinx_build
 
 T = TypeVar('T')
 K = TypeVar('K', bound=Comparable)
 V = TypeVar('V')
 
 class Tree(Generic[K,V]):
+	# binomial tree with child nodes stored as a linked list
+
+	# a "classic" binomial tree looks like the left
+	# this implementation looks like the right
+	#       A           A
+	#     / | \        /
+	#   B   F  H      B--F--H
+	#  / \  |        /   |
+	# C   D G       C--D G
+	# |             |
+	# E             E
+
 	__slots__ = ('_key', '_value', '_child', '_sibling')
 
 	_key: K
 	_value: V
 	_child: Optional[Tree[K,V]]
 	_sibling: Optional[Tree[K,V]]
 
@@ -102,23 +114,23 @@
 			return Forest(other._order, other._tree,
 				Forest.merge(other._next, self, down))
 		forest = Forest.merge(self._next, other._next, down)
 		return Forest.push(forest, down, self._order + 1,
 			self._tree.merge(other._tree, down))
 
 class PHeapView(Generic[K,V,T], Collection[T]):
-	__slots__ = ('_queue', '_sorted')
+	__slots__ = ('_heap', '_sorted')
 
 	if not sphinx_build:
-		_queue: PHeap[K,V]
+		_heap: PHeap[K,V]
 		_sorted: bool
 
-	def __new__(cls, _queue, _sorted):
+	def __new__(cls, _heap, _sorted):
 		self = super().__new__(cls)
-		self._queue = _queue
+		self._heap = _heap
 		self._sorted = _sorted
 		return self
 
 	def __contains__(self, item):
 		r'''
 		Check if the item is in the heap
 
@@ -142,37 +154,37 @@
 		>>> len(pminheap([(1,'a'), (2,'b'), (3,'c')]).keys())
 		3
 		>>> len(pminheap([(1,'a'), (2,'b'), (3,'c')]).values())
 		3
 		>>> len(pminheap([(1,'a'), (2,'b'), (3,'c')]).items())
 		3
 		'''
-		return self._queue._size
+		return self._heap._size
 
 	def _iter_unsorted(self) -> Iterator[Tuple[K,V]]:
-		if self._queue._size == 0: return
-		yield self._queue._key, self._queue._value
-		forest = self._queue._forest
+		if self._heap._size == 0: return
+		yield self._heap._key, self._heap._value
+		forest = self._heap._forest
 		stack:list[Tree[K,V]] = []
 		while forest is not None:
 			stack.append(forest._tree)
 			while stack:
 				item = stack.pop()
 				if isinstance(item, Tree):
 					yield item._key, item._value
 					if item._sibling is not None:
 						stack.append(item._sibling)
 					if item._child is not None:
 						stack.append(item._child)
 			forest = forest._next
 
 	def _iter_sorted(self) -> Iterator[Tuple[K,V]]:
-		queue = self._queue
-		while queue._size > 0:
-			key, value, queue = queue.pop()
+		heap = self._heap
+		while heap._size > 0:
+			key, value, heap = heap.pop()
 			yield key, value
 
 	def _iter(self) -> Iterator[Tuple[K,V]]:
 		if self._sorted:
 			return self._iter_sorted()
 		return self._iter_unsorted()
 
@@ -259,15 +271,19 @@
 		self = super().__new__(cls)
 		self._size = _size
 		self._key = _key
 		self._value = _value
 		self._forest = _forest
 		return self
 
-	def push(self, key:K, value:V=cast(V,None)) -> PHeap[K,V]:
+	@overload
+	def push(self:PHeap[K,None], key:K) -> PHeap[K,None]: ...
+	@overload
+	def push(self:PHeap[K,V], key:K, value:V) -> PHeap[K,V]: ...
+	def push(self, key, value=None):
 		r'''
 		Inserts a value with the specified key
 
 		amortized :math:`O(1)`, worst case :math:`O(\log{n})`
 
 		>>> pminheap([(1,'a'), (2,'b')]).push(3,'c')
 		pminheap([(1, 'a'), (2, 'b'), (3, 'c')])
@@ -326,14 +342,15 @@
 			self, other = other, self
 		forest = Forest.merge(self._forest, other._forest, self._down)
 		forest = Forest.push(forest, self._down, 0,
 			Tree(other._key, other._value, None, None))
 		return type(self)(self._size + other._size, self._key, self._value, forest)
 
 	__add__ = merge
+	__or__ = merge
 
 	def peek(self) -> Tuple[K,V]:
 		r'''
 		Find the min/max element
 
 		:math:`O(1)`
 
@@ -668,27 +685,30 @@
 	>>> pminheap()
 	pminheap([])
 	>>> pminheap([(1,'a'), (2,'b'), (3,'c')])
 	pminheap([(1, 'a'), (2, 'b'), (3, 'c')])
 	'''
 	return cast(PMinHeap, PMinHeap._fromitems(items))
 
-def pminheap_fromkeys(items:Iterable[K], value:V=None) -> PMinHeap[K,V]:
+@overload
+def pminheap_fromkeys(items:Iterable[K]) -> PMinHeap[K,None]: ...
+@overload
+def pminheap_fromkeys(items:Iterable[K], value:V) -> PMinHeap[K,V]: ...
+def pminheap_fromkeys(items, value=None):
 	r'''
 	Create a :class:`PMinHeap` using a default value
 
 	:math:`O(n)`
 
 	>>> pminheap.fromkeys([1, 2, 3])
 	pminheap([(1, None), (2, None), (3, None)])
 	>>> pminheap.fromkeys([1, 2, 3], value='a')
 	pminheap([(1, 'a'), (2, 'a'), (3, 'a')])
 	'''
-	val: V = cast(V, value)
-	return pminheap((item, val) for item in items)
+	return pminheap((item, value) for item in items)
 setattr(pminheap, 'fromkeys', pminheap_fromkeys)
 
 def hl(*items:Tuple[K,V]) -> PMinHeap[K,V]:
 	'''
 	Shorthand for :func:`pminheap`
 
 	Mnemonic: Heap Less-than
@@ -714,27 +734,30 @@
 	>>> pmaxheap()
 	pmaxheap([])
 	>>> pmaxheap([(1,'a'), (2,'b'), (3,'c')])
 	pmaxheap([(3, 'c'), (2, 'b'), (1, 'a')])
 	'''
 	return cast(PMaxHeap, PMaxHeap._fromitems(items))
 
-def pmaxheap_fromkeys(items:Iterable[K], value:V=None) -> PMaxHeap[K,V]:
+@overload
+def pmaxheap_fromkeys(items:Iterable[K]) -> PMaxHeap[K,None]: ...
+@overload
+def pmaxheap_fromkeys(items:Iterable[K], value:V) -> PMaxHeap[K,V]: ...
+def pmaxheap_fromkeys(items, value=None):
 	r'''
 	Create a :class:`PMaxHeap` using a default value
 
 	:math:`O(n)`
 
 	>>> pmaxheap.fromkeys([1, 2, 3])
 	pmaxheap([(3, None), (2, None), (1, None)])
 	>>> pmaxheap.fromkeys([1, 2, 3], value='a')
 	pmaxheap([(3, 'a'), (2, 'a'), (1, 'a')])
 	'''
-	val: V = cast(V, value)
-	return pmaxheap((item, val) for item in items)
+	return pmaxheap((item, value) for item in items)
 setattr(pmaxheap, 'fromkeys', pmaxheap_fromkeys)
 
 def hg(*items:Tuple[K,V]) -> PMaxHeap[K,V]:
 	'''
 	Shorthand for :func:`pmaxheap`
 
 	Mnemonic: Heap Greater-than
```

### Comparing `pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/_base.py` & `pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # - the Digit and Node types are converted from sum types to
 #   a single product type, storing child Nodes in the field "items"
 # - the Digit type stores its size
 # - in the C implementation, the Deep constructor is converted into its
 #   own type to avoid packing FingerTree with three extra pointers
 # - indexing by negative indices operates on items starting from the right
 
-class PSequenceBase(Generic[T]):
+class PSequence(Generic[T]):
 	r'''
 	Persistent sequence
 
 	Meant for cases where you need random access and fast merging/splitting.
 
 	Tries to follow the same naming conventions
 	as the built in list/deque where feasible.
@@ -157,28 +157,28 @@
 		>>> psequence([1,2,3]) > psequence([2,3,4])
 		False
 		>>> psequence([1,2,3]) > psequence([0,1,2])
 		True
 		'''
 
 	@abstractmethod
-	def extendleft(self, other:Union[PSequenceBase[T], Iterable[T]]) -> PSequenceBase[T]:
+	def extendleft(self, other:Union[PSequence[T], Iterable[T]]) -> PSequence[T]:
 		r'''
 		Concatenate two sequences
 
 		:math:`O(\log(\min(n,k)))` extend with :class:`PSequence`
 
 		:math:`O(\log{n}+k)` extend with iterable
 
 		>>> psequence([1,2]).extendleft([3,4])
 		psequence([3, 4, 1, 2])
 		'''
 
 	@abstractmethod
-	def extendright(self, other:Union[PSequenceBase[T], Iterable[T]]) -> PSequenceBase[T]:
+	def extendright(self, other:Union[PSequence[T], Iterable[T]]) -> PSequence[T]:
 		r'''
 		Concatenate two sequences
 
 		:math:`O(\log(\min(n,k)))` extend with PSequence
 
 		:math:`O(\log{n}+k)` extend with iterable
 
@@ -188,15 +188,15 @@
 		psequence([1, 2, 3, 4])
 		>>> psequence([1,2]) + [3,4]
 		psequence([1, 2, 3, 4])
 		'''
 
 	extend = extendright
 
-	def __add__(self, other:Union[PSequenceBase[T], Iterable[T]]) -> PSequenceBase[T]:
+	def __add__(self, other:Union[PSequence[T], Iterable[T]]) -> PSequence[T]:
 		r'''
 		Concatenate two sequences
 
 		:math:`O(\log(\min(n,k)))` extend with PSequence
 
 		:math:`O(\log{n}+k)` extend with iterable
 
@@ -206,15 +206,15 @@
 		psequence([1, 2, 3, 4])
 		'''
 		return self.extendright(other)
 
 	@overload
 	def __getitem__(self, index:int) -> T: ...
 	@overload
-	def __getitem__(self, index:slice) -> PSequenceBase[T]: ...
+	def __getitem__(self, index:slice) -> PSequence[T]: ...
 	@abstractmethod
 	def __getitem__(self, index):
 		r'''
 		Get the element(s) at the specified position(s)
 
 		Time complexities for `n[i]`:
 
@@ -231,17 +231,17 @@
 		>>> psequence([1,2,3,4])[5]
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@overload
-	def set(self, index:int, value:T) -> PSequenceBase[T]: ...
+	def set(self, index:int, value:T) -> PSequence[T]: ...
 	@overload
-	def set(self, index:slice, value:Iterable[T]) -> PSequenceBase[T]: ...
+	def set(self, index:slice, value:Iterable[T]) -> PSequence[T]: ...
 	@abstractmethod
 	def set(self, index, value):
 		r'''
 		Replace the element(s) at the specified position(s)
 
 		Time complexities for `n.set(i,x)`:
 
@@ -258,15 +258,15 @@
 		>>> psequence([1,2,3,4]).set(5, 0)
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def mset(self, *values:Tuple[int,T]) -> PSequenceBase[T]:
+	def mset(self, *values:Tuple[int,T]) -> PSequence[T]:
 		r'''
 		Replace multiple elements
 
 		:math:`O(k\log{n}+k\log{k})`
 
 		:raises IndexError: if any index is out of bounds
 
@@ -277,34 +277,34 @@
 		>>> psequence([1,2,3,4]).mset(5, 0)
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def insert(self, index:int, value:T) -> PSequenceBase[T]:
+	def insert(self, index:int, value:T) -> PSequence[T]:
 		r'''
 		Insert an element at the specified position
 
 		:math:`O(\log(\min(i,n−i)))`
 
 		>>> psequence([1,2,3,4]).insert(2, 0)
 		psequence([1, 2, 0, 3, 4])
 		>>> psequence([1,2,3,4]).insert(-10, 0)
 		psequence([0, 1, 2, 3, 4])
 		>>> psequence([1,2,3,4]).insert(10, 0)
 		psequence([1, 2, 3, 4, 0])
 		'''
 
 	@overload
-	def delete(self, index:int) -> PSequenceBase[T]: ...
+	def delete(self, index:int) -> PSequence[T]: ...
 	@overload
-	def delete(self, index:slice) -> PSequenceBase[T]: ...
+	def delete(self, index:slice) -> PSequence[T]: ...
 	@abstractmethod
-	def delete(self, index) -> PSequenceBase[T]:
+	def delete(self, index) -> PSequence[T]:
 		r'''
 		Delete the element(s) at the specified position(s)
 
 		Time complexities for `n.delete(i)`:
 
 		- :math:`O(\log(\min(i,n−i)))` deleting a single item.
 		- :math:`O(\log{n})` deleting a contiguous slice.
@@ -319,15 +319,15 @@
 		>>> psequence([1,2,3,4]).delete(5)
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def remove(self, value:T) -> PSequenceBase[T]:
+	def remove(self, value:T) -> PSequence[T]:
 		r'''
 		Remove an element by value
 
 		:math:`O(n)`
 
 		:raises ValueError: if the value is not in the sequence
 
@@ -336,15 +336,15 @@
 		>>> psequence([1,2,3,4]).remove(0)
 		Traceback (most recent call last):
 		...
 		ValueError: ...
 		'''
 
 	@abstractmethod
-	def __mul__(self, times:int) -> PSequenceBase[T]:
+	def __mul__(self, times:int) -> PSequence[T]:
 		r'''
 		Repeat the sequence k times
 
 		:math:`O(\log{n}\log{k})`
 
 		>>> psequence([1,2,3]) * 3
 		psequence([1, 2, 3, 1, 2, 3, 1, 2, 3])
@@ -431,26 +431,26 @@
 		>>> repr(psequence([1,2,3]))
 		'psequence([1, 2, 3])'
 		'''
 
 	__str__ = __repr__
 
 	@abstractmethod
-	def appendleft(self, value:T) -> PSequenceBase[T]:
+	def appendleft(self, value:T) -> PSequence[T]:
 		r'''
 		Add an element to the left end
 
 		:math:`O(1)`
 
 		>>> psequence([1,2,3]).appendleft(0)
 		psequence([0, 1, 2, 3])
 		'''
 
 	@abstractmethod
-	def appendright(self, value:T) -> PSequenceBase[T]:
+	def appendright(self, value:T) -> PSequence[T]:
 		r'''
 		Add an element to the right end
 
 		:math:`O(1)`
 
 		>>> psequence([1,2,3]).append(4)
 		psequence([1, 2, 3, 4])
@@ -485,15 +485,15 @@
 		>>> psequence([]).index(3)
 		Traceback (most recent call last):
 		...
 		ValueError: ...
 		'''
 
 	@abstractmethod
-	def splitat(self, index:int) -> Tuple[PSequenceBase[T], PSequenceBase[T]]:
+	def splitat(self, index:int) -> Tuple[PSequence[T], PSequence[T]]:
 		r'''
 		Split a sequence at a given position
 
 		:math:`O(\log(\min(i,n−i)))`
 
 		Equivalent to ``(seq.take(i), seq.drop(i))``.
 		Does not raise :exc:`python:IndexError`, unlike :meth:`view`.
@@ -505,15 +505,15 @@
 		>>> psequence([1,2,3,4]).splitat(-1)
 		(psequence([1, 2, 3]), psequence([4]))
 		>>> psequence([1,2,3,4]).splitat(-5)
 		(psequence([]), psequence([1, 2, 3, 4]))
 		'''
 
 	@abstractmethod
-	def chunksof(self, size:int) -> PSequenceBase[Sequence[T]]:
+	def chunksof(self, size:int) -> PSequence[Sequence[T]]:
 		r'''
 		Split the sequence into chunks
 
 		:math:`O(\frac{n}{k}\log{n})`
 
 		>>> psequence([1,2,3,4,5,6,7,8]).chunksof(3)
 		psequence([psequence([1, 2, 3]), psequence([4, 5, 6]), psequence([7, 8])])
@@ -552,15 +552,15 @@
 		>>> psequence([]).right
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def viewleft(self) -> Tuple[T, PSequenceBase[T]]:
+	def viewleft(self) -> Tuple[T, PSequence[T]]:
 		r'''
 		Analyse the left end
 
 		:math:`O(1)`
 
 		:raises IndexError: if the sequence is empty
 
@@ -569,15 +569,15 @@
 		>>> psequence([]).viewleft()
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def viewright(self) -> Tuple[PSequenceBase[T], T]:
+	def viewright(self) -> Tuple[PSequence[T], T]:
 		r'''
 		Analyse the right end
 
 		:math:`O(1)`
 
 		:raises IndexError: if the sequence is empty
 
@@ -586,15 +586,15 @@
 		>>> psequence([]).viewright()
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def view(self, *index:int) -> Tuple[Union[T, PSequenceBase[T]], ...]:
+	def view(self, *index:int) -> Tuple[Union[T, PSequence[T]], ...]:
 		r'''
 		Split a sequence on the given position(s)
 
 		:math:`O(k\log{n})`
 
 		Useful for pattern matching:
 
@@ -617,15 +617,15 @@
 		>>> psequence([1,2,3,4]).view(5)
 		Traceback (most recent call last):
 		...
 		IndexError: ...
 		'''
 
 	@abstractmethod
-	def reverse(self) -> PSequenceBase[T]:
+	def reverse(self) -> PSequence[T]:
 		r'''
 		Reverse the sequence
 
 		:math:`O(n)`
 
 		>>> psequence([1,2,3,4]).reverse()
 		psequence([4, 3, 2, 1])
@@ -650,59 +650,50 @@
 		:math:`O(n)`
 
 		>>> psequence([1,2,3,4]).totuple()
 		(1, 2, 3, 4)
 		'''
 
 	@abstractmethod
-	def transform(self, transformations) -> PSequenceBase[T]:
+	def transform(self, transformations) -> PSequence[T]:
 		r'''
 		Apply one or more transformations
 
 		>>> from pyrsistent import ny
 		>>> psequence([1,2,3,4]).transform([ny], lambda x: x*2)
 		psequence([2, 4, 6, 8])
 		'''
 
 	@abstractmethod
-	def evolver(self) -> PSequenceEvolverBase[T]:
+	def evolver(self) -> PSequenceEvolver[T]:
 		r'''
 		Create an :class:`Evolver`
 
 		:math:`O(1)`
 		'''
 
 	@abstractmethod
-	def sort(self, *args, **kwargs) -> PSequenceBase[T]:
+	def sort(self, *args, **kwargs) -> PSequence[T]:
 		r'''
 		Creat a sorted copy of the sequence
 
 		:math:`O(n\log{n})`
 
 		Arguments are the same as :meth:`python:list.sort`.
 
 		>>> psequence([3,1,4,2]).sort()
 		psequence([1, 2, 3, 4])
 		'''
 
 	@staticmethod
 	@abstractmethod
-	def _fromitems(iterable:Optional[Iterable[T]]=None) -> PSequenceBase[T]:
-		r'''
-		Create a :class:`PSequence` from the given items
-
-		:math:`O(n)`
-
-		>>> psequence()
-		psequence([])
-		>>> psequence([1,2,3,4])
-		psequence([1, 2, 3, 4])
-		'''
+	def _fromitems(iterable:Optional[Iterable[T]]=None) -> PSequence[T]:
+		pass
 
-class PSequenceEvolverBase(PSequenceBase[T]):
+class PSequenceEvolver(PSequence[T]):
 	r'''
 	Evolver for :class:`PSequence`
 
 	The evolver acts as a mutable view of the sequence with "transaction
 	like" semantics. No part of the underlying sequence is updated, it is
 	still fully immutable. Furthermore multiple evolvers created from the
 	same psequence do not interfere with each other.
@@ -793,15 +784,15 @@
 		...
 		IndexError: ...
 		'''
 
 	@overload
 	def pop(self, index:Optional[int]=None) -> T: ...
 	@overload
-	def pop(self, index:slice) -> PSequenceBase[T]: ...
+	def pop(self, index:slice) -> PSequence[T]: ...
 	@abstractmethod
 	def pop(self, index=None):
 		r'''
 		Remove and return an element at the specified index
 
 		See `PSequence.delete` and `list.pop`.
 
@@ -815,15 +806,15 @@
 		>>> seq.pop(1)
 		2
 		>>> seq
 		psequence([1, 3]).evolver()
 		'''
 
 	@abstractmethod
-	def copy(self) -> PSequenceEvolverBase[T]:
+	def copy(self) -> PSequenceEvolver[T]:
 		r'''
 		Return a shallow copy of the sequence
 
 		:math:`O(1)`
 
 		>>> seq1 = psequence([1,2,3,4]).evolver()
 		>>> seq2 = seq1.copy()
@@ -831,40 +822,41 @@
 		>>> seq2
 		psequence([1, 0, 3, 4]).evolver()
 		>>> seq1
 		psequence([1, 2, 3, 4]).evolver()
 		'''
 
 	@abstractmethod
-	def clear(self) -> PSequenceEvolverBase[T]:
+	def clear(self) -> PSequenceEvolver[T]:
 		r'''
 		Remove all items from the sequence
 
 		:math:`O(1)`
 
 		>>> seq = psequence([1,2,3,4]).evolver()
 		>>> _ = seq.clear()
 		>>> seq
 		psequence([]).evolver()
 		'''
 
 	@abstractmethod
-	def persistent(self) -> PSequenceBase[T]:
+	def persistent(self) -> PSequence[T]:
 		r'''
 		Extract the sequence from the evolver
 
 		:math:`O(1)`
 
 		>>> seq = psequence([1,2,3,4])
 		>>> seq.evolver().persistent()
 		psequence([1, 2, 3, 4])
 		'''
 
 	@staticmethod
-	def _fromitems(iterable:Optional[Iterable[T]]=None) -> PSequenceBase[T]: ...
+	def _fromitems(iterable:Optional[Iterable[T]]=None) -> PSequence[T]:
+		raise TypeError('PSequenceEvolver does not support _fromitems')
 
 # for doctest
 def psequence(*args, **kwargs):
 	from pyrsistent_extras import psequence as pseq
 	return pseq(*args, **kwargs)
 
-__all__ = ('PSequenceBase', 'PSequencePSequenceEvolverBase')
+__all__ = ('PSequence', 'PSequencePSequenceEvolver')
```

### Comparing `pyrsistent-extras-0.1.0/pyrsistent_extras/_psequence/_c_ext.c` & `pyrsistent-extras-0.1.1/src/pyrsistent_extras/_psequence/_c_ext.c`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 // #define PYMALLOC_DEBUG 1
 
-#define PY_SSIZE_T_CLEAN
-#include <Python.h>
-#include <structmember.h>
-
-#include <stdarg.h>
-#include <stdbool.h>
-#include <assert.h>
+#include "_c_ext.h"
+
 
 /*
 Persistent/Immutable/Functional sequence and helper types.
 
 Please note that they are anything but immutable at this level since
 there is a whole lot of reference counting going on. That's the way
 CPython works though and the GIL makes them appear immutable.
@@ -21,257 +16,97 @@
 Naming conventions
 ------------------
 pyrsistent_* - Methods part of the interface
 <typename>_* - Instance methods of types. For examle FTree_extend(...)
 F<typename>  - FingerTree related types, considered private
 P<typename>  - PSequence related types, considered public
 
-All other methods are camel cased without prefix. All methods are static,
-none should require to be exposed outside of this module.
+All other methods are camel cased without prefix.
 */
 
-// {{{ typedef
-
-typedef struct FNode {
-	size_t refs;
-	size_t size;
-	union {
-		PyObject* value;
-		struct FNode* items[3];
-	};
-} FNode;
-
-typedef struct FDigit {
-	size_t refs;
-	size_t size;
-	int  count;
-	FNode* items[4];
-} FDigit;
-
-typedef struct FTree FTree;
-
-typedef struct FDeep {
-	size_t size;
-	FDigit* left;
-	FTree* middle;
-	FDigit* right;
-} FDeep;
-
-typedef enum FTreeT {
-	FEmptyT  = 0,
-	FSingleT = 1,
-	FDeepT   = 2
-} FTreeT ;
-
-typedef struct FTree {
-	size_t refs;
-	FTreeT type;
-	union {
-		void* empty;
-		FNode* single;
-		FDeep* deep;
-	};
-} FTree;
-
-typedef struct FView {
-	FNode* node;
-	FTree* tree;
-} FView;
-
-typedef struct FSplit {
-	FTree* left;
-	FNode* node;
-	FTree* right;
-} FSplit;
-
-typedef struct FIndex {
-	size_t index;
-	union {
-		FNode* node;
-		PyObject* value;
-	};
-} FIndex;
-
-typedef struct FIndex2 {
-	size_t index1;
-	size_t index2;
-	union {
-		FNode* node;
-		PyObject* value;
-	};
-} FIndex2;
-
-typedef struct FInsert {
-	FNode* extra;
-	union {
-		FNode* node;
-		FDigit* digit;
-	};
-} FInsert;
-
-typedef struct FMeld {
-	bool full;
-	union {
-		FNode* node;
-		FDigit* digit;
-		FTree* tree;
-	};
-} FMeld;
-
-typedef struct FMerge {
-	union {
-		FNode* left;
-		FNode* node;
-	};
-	union {
-		FNode* right;
-		void* extra;
-	};
-} FMerge;
-
-typedef enum FIterT {
-	FTreeI  = 0,
-	FDigitI = 1,
-	FNodeI  = 2
-} FIterT;
-
-typedef struct FIter {
-	FIterT type;
-	int index;
-	union {
-		FTree* tree;
-		FNode* node;
-		FDigit* digit;
-	};
-	struct FIter* next;
-} FIter;
-
-typedef struct FMset {
-	size_t index;
-	size_t count;
-	FIndex2* items;
-} FMset;
-
-typedef struct FSlice {
-	size_t modulo;
-	size_t count;
-	size_t step;
-	union {
-		PyObject** input;
-		FNode** output;
-	};
-} FSlice;
-
-typedef struct PSequence {
-	PyObject_HEAD
-	FTree* tree;
-	PyObject* weakrefs;
-} PSequence;
-
-typedef struct PSequenceIter {
-	PyObject_HEAD
-	Py_ssize_t index;
-	bool reverse;
-	PSequence* seq;
-	FIter* stack;
-} PSequenceIter;
-
-typedef struct PSequenceEvolver {
-	PyObject_HEAD
-	PSequence* seq;
-} PSequenceEvolver;
-
-static PyTypeObject PSequenceType;
-static PyTypeObject PSequenceIterType;
-static PyTypeObject PSequenceEvolverType;
-
-// }}}
-
 // {{{ misc
 
-#if defined(__GNUC__) || defined(__clang__)
-# define UNUSED __attribute__((unused))
-#else
-# define UNUSED
-#endif
+PyTypeObject PSequenceType;
+PyTypeObject PSequenceIterType;
+PyTypeObject PSequenceEvolverType;
 
-static PSequence* EMPTY_SEQUENCE = NULL;
-static FTree EMPTY_TREE = { .refs = 1, .type = FEmptyT, .empty = NULL };
+PSequence* EMPTY_SEQUENCE = NULL;
+FTree EMPTY_TREE = { .refs = 1, .type = FEmptyT, .empty = NULL };
 
-static void* PSequence_indexError(Py_ssize_t index) {
+void* PSequence_indexError(Py_ssize_t index) {
 	return PyErr_Format(PyExc_IndexError, "index out of range: %zd", index);
 }
 
-static int FNode_count(const FNode* node) {
+int FNode_count(const FNode* node) {
 	if(node->size == 1)
 		return 1;
 	if(node->items[2] == NULL)
 		return 2;
 	else
 		return 3;
 }
 
-UNUSED static size_t FNode_depth(const FNode* node) {
+size_t FNode_depth(const FNode* node) {
 	assert(node != NULL);
 	size_t n = 0;
 	while(node->size != 1) {
 		++n;
 		node = node->items[0];
 		assert(node != NULL);
 	}
 	return n;
 }
 
-static size_t FTree_size(const FTree* tree) {
+size_t FTree_size(const FTree* tree) {
 	switch(tree->type) {
 		case FEmptyT:  return 0;
 		case FSingleT: return tree->single->size;
 		case FDeepT:   return tree->deep->size;
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static Py_ssize_t FTree_ssize(const FTree* tree) {
+Py_ssize_t FTree_ssize(const FTree* tree) {
 	return (Py_ssize_t)FTree_size(tree);
 }
 
-static bool FTree_empty(const FTree* tree) {
+bool FTree_empty(const FTree* tree) {
 	return tree->type == FEmptyT;
 }
 
-static bool FTree_checkIndex(const FTree* tree, Py_ssize_t* index) {
+bool FTree_checkIndex(const FTree* tree, Py_ssize_t* index) {
 	Py_ssize_t size = FTree_size(tree);
 	Py_ssize_t idx = *index;
 	if(idx < 0) idx += size;
 	if(!(0 <= idx && idx < size))
 		return false;
 	*index = idx;
 	return true;
 }
 
-static int FIndex2_compare(const FIndex2* x, const FIndex2* y) {
+int FIndex2_compare(const FIndex2* x, const FIndex2* y) {
 	if(x->index1 == y->index1)
 		return x->index2 - y->index2;
 	return x->index1 - y->index1;
 }
 
 // }}}
 
 // {{{ print
 // for debugging tree structures
 
-#ifndef NDEBUG
+// LCOV_EXCL_START
 
-UNUSED static void FIndent_print(int indent) {
+UNUSED void FIndent_print(int indent) {
 	// printf("%d ", indent);
 	for(int i = 0; i < indent; ++i)
 		printf("  ");
 }
 
-UNUSED static void FNode_print(FNode* node, int indent) {
+UNUSED void FNode_print(FNode* node, int indent) {
 	FIndent_print(indent);
 	if(node->size == 1) {
 		printf("FElement(refs=%zu) ", node->refs);
 		PyObject_Print(node->value, stdout, 0);
 		// printf("%p(refs=%zd)", node->value, Py_REFCNT(node->items[0]));
 		printf("\n");
 	} else {
@@ -279,22 +114,22 @@
 		FNode_print((FNode*)node->items[0], indent + 1);
 		FNode_print((FNode*)node->items[1], indent + 1);
 		if(node->items[2] != NULL)
 			FNode_print((FNode*)node->items[2], indent + 1);
 	}
 }
 
-UNUSED static void FDigit_print(FDigit* digit, int indent) {
+UNUSED void FDigit_print(FDigit* digit, int indent) {
 	FIndent_print(indent);
 	printf("FDigit[size=%zu](refs=%zu)\n", digit->size, digit->refs);
 	for(int i = 0; i < digit->count; ++i)
 		FNode_print(digit->items[i], indent + 1);
 }
 
-UNUSED static void FTree_print(FTree* tree, int indent) {
+UNUSED void FTree_print(FTree* tree, int indent) {
 	FIndent_print(indent);
 	switch(tree->type) {
 		case FEmptyT:
 			printf("FEmpty(refs=%zu)\n", tree->refs);
 			break;
 		case FSingleT:
 			printf("FSingle(refs=%zu)\n", tree->refs);
@@ -303,138 +138,136 @@
 		case FDeepT:
 			printf("FDeep[size=%zu](refs=%zu)\n",
 				tree->deep->size, tree->refs);
 			FDigit_print(tree->deep->left, indent + 1);
 			FTree_print(tree->deep->middle, indent + 1);
 			FDigit_print(tree->deep->right, indent + 1);
 			break;
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-UNUSED static void FIter_print(FIter* iter) {
+UNUSED void FIter_print(FIter* iter) {
 	while(iter != NULL) {
 		switch(iter->type) {
 			case FTreeI: printf("Tree"); break;
 			case FNodeI: printf("Node"); break;
 			case FDigitI: printf("Digit"); break;
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		}
 		printf("%d ", iter->index);
 		iter = iter->next;
 	}
 	printf("(nil)\n");
 }
 
-#endif
+// LCOV_EXCL_STOP
 
 // }}}
 
 // {{{ debug
 
-typedef enum FRefs {
-	FTreeR = 0,
-	FDigitR = 1,
-	FNodeR = 2,
-} FRefs;
+// LCOV_EXCL_START
 
 #ifndef NDEBUG
-static long FRefs_count[3];
-static long FRefs_get(FRefs type) { return FRefs_count[type]; }
-static void FRefs_inc(FRefs type) { ++FRefs_count[type]; }
-static void FRefs_dec(FRefs type) { --FRefs_count[type]; }
+long FRefs_count[3];
+long FRefs_get(FRefs type) { return FRefs_count[type]; }
+void FRefs_inc(FRefs type) { ++FRefs_count[type]; }
+void FRefs_dec(FRefs type) { --FRefs_count[type]; }
 #else
-#define FRefs_get(type) 0
-#define FRefs_inc(type)
-#define FRefs_dec(type)
+inline long FRefs_get(FRefs type) { return 0; }
+inline void FRefs_inc(FRefs type) { }
+inline void FRefs_dec(FRefs type) { }
 #endif
 
+// LCOV_EXCL_STOP
+
 // }}}
 
 // {{{ ref count
 
-static void* PObj_IncRef(void* obj) {
+void* PObj_IncRef(void* obj) {
 	Py_INCREF(obj);
 	return obj;
 }
 
-static FNode* FNode_incRef(FNode* node) {
+FNode* FNode_incRef(FNode* node) {
 	assert(node != NULL);
 	++node->refs;
 	FRefs_inc(FNodeR);
 	return node;
 }
 
-static FNode* FNode_incRefM(FNode* node) {
+FNode* FNode_incRefM(FNode* node) {
 	if(node != NULL) {
 		++node->refs;
 		FRefs_inc(FNodeR);
 	}
 	return node;
 }
 
-static void FNode_decRef(FNode* node) {
+void FNode_decRef(FNode* node) {
 	assert(node != NULL);
 	assert(node->refs > 0);
 	FRefs_dec(FNodeR);
 	if(--node->refs == 0) {
 		if(node->size != 1) {
 			FNode_decRef(node->items[0]);
 			FNode_decRef(node->items[1]);
 			if(node->items[2] != NULL)
 				FNode_decRef(node->items[2]);
 		} else Py_DECREF(node->value);
 		PyMem_Free(node);
 	}
 }
 
-static void* FNode_decRefRet(FNode* node, void* ret) {
+void* FNode_decRefRet(FNode* node, void* ret) {
 	FNode_decRef(node);
 	return ret;
 }
 
-static FDigit* FDigit_incRef(FDigit* digit) {
+FDigit* FDigit_incRef(FDigit* digit) {
 	if(digit != NULL) {
 		++digit->refs;
 		FRefs_inc(FDigitR);
 	}
 	return digit;
 }
 
-static void FDigit_decRef(FDigit* digit) {
+void FDigit_decRef(FDigit* digit) {
 	assert(digit != NULL);
 	assert(digit->refs > 0);
 	FRefs_dec(FDigitR);
 	if(--digit->refs == 0) {
 		switch(digit->count) {
 			case 4: FNode_decRef(digit->items[3]);
 			case 3: FNode_decRef(digit->items[2]);
 			case 2: FNode_decRef(digit->items[1]);
 			case 1: FNode_decRef(digit->items[0]);
 				break;
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		}
 		PyMem_Free(digit);
 	}
 }
 
-// static void* FDigit_decRefRet(FDigit* digit, void* ret) {
+// void* FDigit_decRefRet(FDigit* digit, void* ret) {
 	// FDigit_decRef(digit);
 	// return ret;
 // }
 
-static FTree* FTree_incRef(FTree* tree) {
+FTree* FTree_incRef(FTree* tree) {
 	if(tree != NULL) {
 		++tree->refs;
 		FRefs_inc(FTreeR);
 	}
 	return tree;
 }
 
-static void FTree_decRef(FTree* tree) {
+void FTree_decRef(FTree* tree) {
 	assert(tree != NULL);
 	assert(tree->refs > 0);
 	FRefs_dec(FTreeR);
 	if(--tree->refs == 0) {
 		switch(tree->type) {
 			case FEmptyT:
 				break;
@@ -443,111 +276,111 @@
 				break;
 			case FDeepT:
 				FDigit_decRef(tree->deep->left);
 				FTree_decRef(tree->deep->middle);
 				FDigit_decRef(tree->deep->right);
 				PyMem_Free(tree->deep);
 				break;
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		}
 		PyMem_Free(tree);
 	}
 }
 
-static void* FTree_decRefRet(FTree* tree, void* ret) {
+void* FTree_decRefRet(FTree* tree, void* ret) {
 	FTree_decRef(tree);
 	return ret;
 }
 
-static FIter* FIter_incRef(FIter* iter) {
+FIter* FIter_incRef(FIter* iter) {
 	switch(iter->type) {
 		case FTreeI: FTree_incRef(iter->tree); break;
 		case FDigitI: FDigit_incRef(iter->digit); break;
 		case FNodeI: FNode_incRef(iter->node); break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	return iter;
 }
 
-static FIter* FIter_decRef(FIter* iter) {
+FIter* FIter_decRef(FIter* iter) {
 	switch(iter->type) {
 		case FTreeI: FTree_decRef(iter->tree); break;
 		case FDigitI: FDigit_decRef(iter->digit); break;
 		case FNodeI: FNode_decRef(iter->node); break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	return iter;
 }
 
 // }}}
 
 // {{{ constructor
 
 // {{{ FNode
 
-static FNode* FNode_alloc() {
-	FNode* node = PyMem_Malloc(sizeof(FNode));
+FNode* FNode_alloc() {
+	FNode* node = (FNode*)PyMem_Malloc(sizeof(FNode));
 	node->refs = 1;
 	FRefs_inc(FNodeR);
 	return node;
 }
 
-static FNode* FNode_make(
+FNode* FNode_make(
 	const size_t size,
 	const FNode* n0,
 	const FNode* n1,
 	const FNode* n2
 ) {
 	assert(size == 1 || size == n0->size + n1->size + (n2 ? n2->size : 0));
 	FNode* node = FNode_alloc();
 	node->size = size;
 	node->items[0] = (FNode*)n0; assert(size == 1 || n0 != NULL);
 	node->items[1] = (FNode*)n1; assert(size == 1 || n1 != NULL);
 	node->items[2] = (FNode*)n2;
 	return node;
 }
 
-static FNode* FNode_makeS(
+FNode* FNode_makeS(
 	const FNode* n0,
 	const FNode* n1,
 	const FNode* n2
 ) {
 	assert(n0 != NULL); assert(n1 != NULL);
 	size_t size = n0->size + n1->size + (n2 == NULL ? 0 : n2->size);
 	return FNode_make(size, n0, n1, n2);
 }
 
-static FNode* FNode_makeNS(const int count, FNode** nodes) {
+FNode* FNode_makeNS(const int count, FNode** nodes) {
 	switch(count) {
 		case 2: return FNode_make(
 			nodes[0]->size + nodes[1]->size,
 			nodes[0], nodes[1], NULL);
 		case 3: return FNode_make(
 			nodes[0]->size + nodes[1]->size + nodes[2]->size,
 			nodes[0], nodes[1], nodes[2]);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FNode* FNode_makeE(const PyObject* item) {
+FNode* FNode_makeE(const PyObject* item) {
 	return FNode_make(1, (FNode*)item, NULL, NULL);
 }
 
 // }}}
 
 // {{{ FDigit
 
-static FDigit* FDigit_alloc() {
-	FDigit* digit = PyMem_Malloc(sizeof(FDigit));
+FDigit* FDigit_alloc() {
+	FDigit* digit = (FDigit*)PyMem_Malloc(sizeof(FDigit));
 	digit->refs = 1;
 	FRefs_inc(FDigitR);
 	return digit;
 }
 
-static FDigit* FDigit_make(
+FDigit* FDigit_make(
 	const size_t size,
 	const int count,
 	const FNode* n0,
 	const FNode* n1,
 	const FNode* n2,
 	const FNode* n3
 ) {
@@ -558,33 +391,33 @@
 	digit->items[0] = (FNode*)n0; assert(n0 != NULL);
 	digit->items[1] = (FNode*)n1; assert((count < 2) == (n1 == NULL));
 	digit->items[2] = (FNode*)n2; assert((count < 3) == (n2 == NULL));
 	digit->items[3] = (FNode*)n3; assert((count < 4) == (n3 == NULL));
 	return digit;
 }
 
-static FDigit* FDigit_makeN(
+FDigit* FDigit_makeN(
 	const size_t size,
 	const int count,
 	FNode** nodes
 ) {
 	switch(count) {
 		case 1: return FDigit_make(size,
 			count, nodes[0], NULL, NULL, NULL);
 		case 2: return FDigit_make(size,
 			count, nodes[0], nodes[1], NULL, NULL);
 		case 3: return FDigit_make(size,
 			count, nodes[0], nodes[1], nodes[2], NULL);
 		case 4: return FDigit_make(size,
 			count, nodes[0], nodes[1], nodes[2], nodes[3]);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FDigit* FDigit_makeS(
+FDigit* FDigit_makeS(
 	const int count,
 	const FNode* n0,
 	const FNode* n1,
 	const FNode* n2,
 	const FNode* n3
 ) {
 	assert(1 <= count && count <= 4);
@@ -596,77 +429,77 @@
 	digit->items[3] = (FNode*)n3; assert((count < 4) == (n3 == NULL));
 	size_t size = n0->size;
 	switch(count) {
 		case 4: assert(n3 != NULL); size += n3->size;
 		case 3: assert(n2 != NULL); size += n2->size;
 		case 2: assert(n1 != NULL); size += n1->size;
 		case 1: break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	digit->size = size;
 	return digit;
 }
 
-static FDigit* FDigit_makeNS(const int count, FNode** nodes) {
+FDigit* FDigit_makeNS(const int count, FNode** nodes) {
 	assert(nodes[0] != NULL);
 	size_t size = nodes[0]->size;
 	switch(count) {
 		case 4: assert(nodes[3] != NULL); size += nodes[3]->size;
 		case 3: assert(nodes[2] != NULL); size += nodes[2]->size;
 		case 2: assert(nodes[1] != NULL); size += nodes[1]->size;
 		case 1: break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	return FDigit_makeN(size, count, nodes);
 }
 
-static FDigit* FDigit_fromNode(const FNode* node) {
+FDigit* FDigit_fromNode(const FNode* node) {
 	return FDigit_make(node->size, FNode_count(node),
 		FNode_incRef(node->items[0]),
 		FNode_incRef(node->items[1]),
 		FNode_incRefM(node->items[2]), NULL);
 }
 
-static FDigit* FDigit_fromMerge(FMerge merge) {
+FDigit* FDigit_fromMerge(FMerge merge) {
 	if(merge.extra == NULL)
 		return FDigit_make(merge.left->size, 1,
 			merge.left, NULL, NULL, NULL);
 	return FDigit_make(merge.left->size + merge.right->size, 2,
 		merge.left, merge.right, NULL, NULL);
 }
 
 // }}}
 
 // {{{ FTree
 
-static FTree* FTree_alloc() {
-	FTree* tree = PyMem_Malloc(sizeof(FTree));
+FTree* FTree_alloc() {
+	FTree* tree = (FTree*)PyMem_Malloc(sizeof(FTree));
 	tree->refs = 1;
 	FRefs_inc(FTreeR);
 	return tree;
 }
 
-static FTree* FEmpty_make() {
+FTree* FEmpty_make() {
 	FTree_incRef(&EMPTY_TREE);
 	return &EMPTY_TREE;
 }
 
-static FTree* FSingle_make(const FNode* node) {
+FTree* FSingle_make(const FNode* node) {
 	FTree* tree = FTree_alloc();
 	tree->type = FSingleT;
 	tree->single = (FNode*)node;
 	return tree;
 }
 
-static FDeep* FDeep_alloc() {
-	FDeep* deep = PyMem_Malloc(sizeof(FDeep));
+FDeep* FDeep_alloc() {
+	FDeep* deep = (FDeep*)PyMem_Malloc(sizeof(FDeep));
 	return deep;
 }
 
-static FTree* FDeep_make(
+FTree* FDeep_make(
 	const size_t size,
 	const FDigit* left,
 	const FTree* middle,
 	const FDigit* right
 ) {
 	assert(size == left->size + FTree_size(middle) + right->size);
 	FDeep* deep = FDeep_alloc();
@@ -676,24 +509,24 @@
 	deep->right = (FDigit*)right;
 	FTree* tree = FTree_alloc();
 	tree->type = FDeepT;
 	tree->deep = deep;
 	return tree;
 }
 
-static FTree* FDeep_makeS(
+FTree* FDeep_makeS(
 	const FDigit* left,
 	const FTree* middle,
 	const FDigit* right
 ) {
 	size_t size = left->size + FTree_size(middle) + right->size;
 	return FDeep_make(size, left, middle, right);
 }
 
-static FTree* FTree_fromDigit(const FDigit* digit) {
+FTree* FTree_fromDigit(const FDigit* digit) {
 	switch(digit->count) {
 		case 1: return FSingle_make(FNode_incRef(digit->items[0]));
 		case 2: return FDeep_make(digit->size,
 			FDigit_make(digit->items[0]->size, 1,
 				FNode_incRef(digit->items[0]), NULL, NULL, NULL),
 			FEmpty_make(),
 			FDigit_make(digit->items[1]->size, 1,
@@ -709,174 +542,116 @@
 			FDigit_make(digit->items[0]->size + digit->items[1]->size, 2,
 				FNode_incRef(digit->items[0]),
 				FNode_incRef(digit->items[1]), NULL, NULL),
 				FEmpty_make(),
 			FDigit_make(digit->items[2]->size + digit->items[3]->size, 2,
 				FNode_incRef(digit->items[2]),
 				FNode_incRef(digit->items[3]), NULL, NULL));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FTree* FTree_fromMerge(FMerge merge) {
+FTree* FTree_fromMerge(FMerge merge) {
 	if(merge.extra == NULL)
 		return FSingle_make(merge.left);
 	return FDeep_makeS(
 		FDigit_make(merge.left->size, 1, merge.left, NULL, NULL, NULL),
 		FEmpty_make(),
 		FDigit_make(merge.right->size, 1, merge.right, NULL, NULL, NULL));
 }
 
 // }}}
 
 // {{{ PSequence
 
-static PSequence* PSequence_make(const FTree* tree) {
+PSequence* PSequence_make(const FTree* tree) {
 	assert(tree != NULL);
 	PSequence* seq = PyObject_GC_New(PSequence, &PSequenceType);
 	seq->tree = (FTree*)tree;
 	seq->weakrefs = NULL;
 	PyObject_GC_Track(seq);
 	return seq;
 }
 
-static void PSequence_dealloc(PSequence* self) {
+void PSequence_dealloc(PSequence* self) {
 	if (self->weakrefs != NULL)
 		PyObject_ClearWeakRefs((PyObject*)self);
 	PyObject_GC_UnTrack(self);
 	Py_TRASHCAN_SAFE_BEGIN(self);
 	FTree_decRef(self->tree);
 	PyObject_GC_Del(self);
 	Py_TRASHCAN_SAFE_END(self);
 }
 
 // }}}
 
 // {{{ FIter
 
-static inline FIter* FIter_alloc() {
-	return PyMem_Malloc(sizeof(FIter));
-}
-
-static inline FIter* FIter_make(
-	FIterT type,
-	int index,
-	void* item,
-	FIter* next
-) {
-	FIter* iter = FIter_alloc();
-	iter->type = type;
-	iter->index = index;
-	iter->tree = item;
-	iter->next = next;
-	FIter_incRef(iter);
-	return iter;
-}
-
-static void FIter_dealloc(FIter* iter, bool all) {
+void FIter_dealloc(FIter* iter, bool all) {
 	if(iter == NULL) return;
 	FIter_decRef(iter);
 	FIter* next = iter->next;
 	PyMem_Free(iter);
 	if(all) FIter_dealloc(next, all);
 }
 
 // }}}
 
 // {{{ PSequenceIter
 
-static PSequenceIter* PSequenceIter_make(
+PSequenceIter* PSequenceIter_make(
 	Py_ssize_t index,
 	bool reverse,
 	PSequence* seq,
 	FIter* stack
 ) {
 	PSequenceIter* iter = PyObject_GC_New(PSequenceIter, &PSequenceIterType);
 	iter->index = index;
 	iter->reverse = reverse;
 	iter->seq = seq;
 	iter->stack = stack;
 	PyObject_GC_Track(iter);
 	return iter;
 }
 
-static void PSequenceIter_dealloc(PSequenceIter* self) {
+void PSequenceIter_dealloc(PSequenceIter* self) {
 	PyObject_GC_UnTrack(self);
 	Py_DECREF(self->seq);
 	FIter_dealloc(self->stack, true);
 	PyObject_GC_Del(self);
 }
 
 // }}}
 
 // {{{ PSequenceEvolver
 
-static PSequenceEvolver* PSequenceEvolver_make(PSequence* seq) {
+PSequenceEvolver* PSequenceEvolver_make(PSequence* seq) {
 	assert(seq != NULL);
 	PSequenceEvolver* evo = PyObject_GC_New(
 		PSequenceEvolver, &PSequenceEvolverType);
 	evo->seq = seq;
 	PyObject_GC_Track(evo);
 	return evo;
 }
 
-static void PSequenceEvolver_dealloc(PSequenceEvolver* self) {
+void PSequenceEvolver_dealloc(PSequenceEvolver* self) {
 	PyObject_GC_UnTrack(self);
 	Py_TRASHCAN_SAFE_BEGIN(self);
 	Py_DECREF(self->seq);
 	PyObject_GC_Del(self);
 	Py_TRASHCAN_SAFE_END(self);
 }
 
 // }}}
 
-// {{{ misc
-
-static inline FView FView_make(FNode* node, FTree* tree) {
-	FView view = { .node=node, .tree=tree };
-	return view;
-}
-
-static inline FSplit FSplit_make(FTree* left, FNode* node, FTree* right) {
-	FSplit split = { .left=left, .node=node, .right=right };
-	return split;
-}
-
-static inline FIndex FIndex_make(size_t idx, FNode* node) {
-	FIndex index = { .index=idx, .node=node };
-	return index;
-}
-
-static inline FIndex2 FIndex2_make(size_t idx1, size_t idx2, FNode* node) {
-	FIndex2 index = { .index1=idx1, .index2=idx2, .node=node };
-	return index;
-}
-
-static inline FInsert FInsert_make(FNode* extra, void* value) {
-	FInsert insert = { .extra=extra, .node=value };
-	return insert;
-}
-
-static inline FMeld FMeld_make(bool full, void* value) {
-	FMeld meld = { .full=full, .node=value };
-	return meld;
-}
-
-static inline FMerge FMerge_make(FNode* left, FNode* right) {
-	FMerge merge = { .left=left, .right=right };
-	return merge;
-}
-
-// }}}
-
 // }}}
 
 // {{{ toTree
 
-static PyObject* FNode_toTree(const FNode* node) {
+PyObject* FNode_toTree(const FNode* node) {
 	assert(node != NULL);
 	if(node->size == 1)
 		return Py_BuildValue("(slO)",
 			"Node", (long)node->size,  node->value);
 	if(FNode_count(node) == 2)
 		return Py_BuildValue("(slNN)",
 			"Node", (long)node->size,
@@ -885,15 +660,15 @@
 	return Py_BuildValue("(slNNN)",
 		"Node", (long)node->size,
 		FNode_toTree(node->items[0]),
 		FNode_toTree(node->items[1]),
 		FNode_toTree(node->items[2]));
 }
 
-static PyObject* FDigit_toTree(const FDigit* digit) {
+PyObject* FDigit_toTree(const FDigit* digit) {
 	assert(digit != NULL);
 	switch(digit->count) {
 		case 1:
 			return Py_BuildValue("(slN)",
 				"Digit", (long)digit->size,
 				FNode_toTree(digit->items[0]));
 		case 2:
@@ -910,56 +685,56 @@
 		case 4:
 			return Py_BuildValue("(slNNNN)",
 				"Digit", (long)digit->size,
 				FNode_toTree(digit->items[0]),
 				FNode_toTree(digit->items[1]),
 				FNode_toTree(digit->items[2]),
 				FNode_toTree(digit->items[3]));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* FTree_toTree(const FTree* tree) {
+PyObject* FTree_toTree(const FTree* tree) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return Py_BuildValue("(sl)", "Tree", 0);
 		case FSingleT: return Py_BuildValue("(slN)",
 			"Tree", (long)FTree_size(tree),
 			FNode_toTree(tree->single));
 		case FDeepT: return Py_BuildValue("(slNNN)",
 			"Tree", (long)FTree_size(tree),
 			FDigit_toTree(tree->deep->left),
 			FTree_toTree(tree->deep->middle),
 			FDigit_toTree(tree->deep->right));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_toTree(PSequence* self) {
+PyObject* PSequence_toTree(PSequence* self) {
 	return FTree_toTree(self->tree);
 }
 
 // }}}
 
 // {{{ fromTuple
 
-static bool FTuple_checkType(PyObject* arg, const char* name) {
+bool FTuple_checkType(PyObject* arg, const char* name) {
 	if(!PyTuple_Check(arg)) return PyErr_Format(
 		PyExc_TypeError, "expected tuple");
 	Py_ssize_t argc = PyTuple_GET_SIZE(arg);
 	if(argc < 2) return PyErr_Format(
 		PyExc_ValueError, "expected 2 or more items but got %zd", argc);
 	PyObject* arg0 = PyTuple_GET_ITEM(arg, 0);
 	int str = PyUnicode_CompareWithASCIIString(arg0, name);
 	if(str != 0) return PyErr_Format(
 		PyExc_AssertionError, "expected '%s' but got %R", name, arg0);
 	return true;
 }
 
-static FNode* FNode_fromTuple(PyObject* arg) {
+FNode* FNode_fromTuple(PyObject* arg) {
 	if(!FTuple_checkType(arg, "Node")) return NULL;
 	switch(PyTuple_GET_SIZE(arg)) {
 		case 3: return FNode_makeE(PObj_IncRef(PyTuple_GET_ITEM(arg, 2)));
 		case 4: case 5: {
 			int count = 0;
 			FNode* nodes[4];
 			for(int i = 2; i < PyTuple_GET_SIZE(arg); ++i, ++count) {
@@ -973,15 +748,15 @@
 			return FNode_makeNS(count, nodes);
 		} default: PyErr_Format(PyExc_ValueError,
 			"expected 3, 4, or 5 items but got %zd", PyTuple_GET_SIZE(arg));
 			return NULL;
 	}
 }
 
-static FDigit* FDigit_fromTuple(PyObject* arg) {
+FDigit* FDigit_fromTuple(PyObject* arg) {
 	if(!FTuple_checkType(arg, "Digit")) return NULL;
 	int argc = PyTuple_GET_SIZE(arg);
 	switch(argc) {
 		case 3: case 4: case 5: case 6: {
 			int count = 0;
 			FNode* nodes[4];
 			for(int i = 2; i < PyTuple_GET_SIZE(arg); ++i, ++count) {
@@ -995,15 +770,15 @@
 			return FDigit_makeNS(count, nodes);
 		} default: PyErr_Format(PyExc_ValueError,
 			"expected 3, 4, 5, or 6 items but got %zd", PyTuple_GET_SIZE(arg));
 			return NULL;
 	}
 }
 
-static FTree* FTree_fromTuple(PyObject* arg) {
+FTree* FTree_fromTuple(PyObject* arg) {
 	if(!FTuple_checkType(arg, "Tree")) return NULL;
 	switch(PyTuple_GET_SIZE(arg)) {
 		case 2: return FEmpty_make();
 		case 3: {
 			FNode* node = FNode_fromTuple(PyTuple_GET_ITEM(arg, 2));
 			if(node == NULL) return NULL;
 			return FSingle_make(node);
@@ -1018,41 +793,41 @@
 			return FDeep_makeS(left, middle, right);
 		} default: PyErr_Format(PyExc_ValueError,
 			"expected 2, 3, or 5 items but got %zd", PyTuple_GET_SIZE(arg));
 			return NULL;
 	}
 }
 
-static PSequence* PSequence_fromTuple(void* _, PyObject* arg) {
+PSequence* PSequence_fromTuple(void* _, PyObject* arg) {
 	FTree* tree = FTree_fromTuple(arg);
 	if(tree == NULL) return NULL;
 	return PSequence_make(tree);
 }
 
 // }}}
 
 // {{{ appendLeft
 
-static FDigit* FDigit_appendLeft(FDigit* digit, FNode* node) {
+FDigit* FDigit_appendLeft(FDigit* digit, FNode* node) {
 	assert(digit->count < 4);
 	switch(digit->count) {
 		case 3: return FDigit_make(digit->size + node->size, 4, node,
 			FNode_incRef(digit->items[0]),
 			FNode_incRef(digit->items[1]),
 			FNode_incRef(digit->items[2]));
 		case 2: return FDigit_make(digit->size + node->size, 3, node,
 			FNode_incRef(digit->items[0]),
 			FNode_incRef(digit->items[1]), NULL);
 		case 1: return FDigit_make(digit->size + node->size, 2, node,
 			FNode_incRef(digit->items[0]), NULL, NULL);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FTree* FTree_appendLeft(FTree* tree, FNode* node) {
+FTree* FTree_appendLeft(FTree* tree, FNode* node) {
 	switch(tree->type) {
 		case FEmptyT:
 			return FSingle_make(node);
 		case FSingleT:
 			return FDeep_make(tree->single->size + node->size,
 				FDigit_make(node->size, 1, node, NULL, NULL, NULL),
 				FEmpty_make(),
@@ -1069,47 +844,47 @@
 					node, FNode_incRef(tree->deep->left->items[0]), NULL, NULL),
 				FTree_appendLeft(tree->deep->middle, FNode_make(
 					tree->deep->left->size - tree->deep->left->items[0]->size,
 					FNode_incRef(tree->deep->left->items[1]),
 					FNode_incRef(tree->deep->left->items[2]),
 					FNode_incRef(tree->deep->left->items[3]))),
 				FDigit_incRef(tree->deep->right));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_appendLeft(PSequence* self, PyObject* value) {
+PSequence* PSequence_appendLeft(PSequence* self, PyObject* value) {
 	return PSequence_make(FTree_appendLeft(self->tree,
 		FNode_makeE(PObj_IncRef(value))));
 }
 
 // }}}
 
 // {{{ appendRight
 
-static FDigit* FDigit_appendRight(FDigit* digit, FNode* node) {
+FDigit* FDigit_appendRight(FDigit* digit, FNode* node) {
 	assert(digit->count < 4);
 	switch(digit->count) {
 		case 3: return FDigit_make(digit->size + node->size, 4,
 			FNode_incRef(digit->items[0]),
 			FNode_incRef(digit->items[1]),
 			FNode_incRef(digit->items[2]),
 			node);
 		case 2: return FDigit_make(digit->size + node->size, 3,
 			FNode_incRef(digit->items[0]),
 			FNode_incRef(digit->items[1]),
 			node, NULL);
 		case 1: return FDigit_make(digit->size + node->size, 2,
 			FNode_incRef(digit->items[0]),
 			node, NULL, NULL);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FTree* FTree_appendRight(FTree* tree, FNode* node) {
+FTree* FTree_appendRight(FTree* tree, FNode* node) {
 	switch(tree->type) {
 		case FEmptyT:
 			return FSingle_make(node);
 		case FSingleT:
 			return FDeep_make(tree->single->size + node->size,
 				FDigit_make(tree->single->size, 1,
 					FNode_incRef(tree->single), NULL, NULL, NULL),
@@ -1127,41 +902,39 @@
 					tree->deep->right->size - tree->deep->right->items[3]->size,
 					FNode_incRef(tree->deep->right->items[0]),
 					FNode_incRef(tree->deep->right->items[1]),
 					FNode_incRef(tree->deep->right->items[2]))),
 				FDigit_make(tree->deep->right->items[3]->size + node->size,
 					2, FNode_incRef(tree->deep->right->items[3]),
 					node, NULL, NULL));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_appendRight(PSequence* self, PyObject* value) {
+PSequence* PSequence_appendRight(PSequence* self, PyObject* value) {
 	return PSequence_make(
 		FTree_appendRight(self->tree,
 			FNode_makeE(PObj_IncRef(value))));
 }
 
 // }}}
 
 // {{{ viewLeft
 
-static FView FTree_viewLeft(FTree* tree);
-
-static FTree* FTree_pullLeft(FTree* middle, FDigit* right) {
+FTree* FTree_pullLeft(FTree* middle, FDigit* right) {
 	if(FTree_empty(middle))
 		return FTree_fromDigit(right);
 	FView view = FTree_viewLeft(middle);
 	FTree* tail = FDeep_make(FTree_size(middle) + right->size,
 		FDigit_fromNode(view.node), view.tree,
 		FDigit_incRef(right));
 	return tail;
 }
 
-static FView FTree_viewLeft(FTree* tree) {
+FView FTree_viewLeft(FTree* tree) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FSingleT: return FView_make(tree->single, FEmpty_make());
 		case FDeepT: {
 			FDigit* left = tree->deep->left;
 			FNode* head = left->items[0];
 			if(left->count == 1) return FView_make(head,
@@ -1171,44 +944,42 @@
 			FTree* tail = FDeep_make(tree->deep->size - head->size,
 				FDigit_makeN(left->size - head->size,
 					left->count - 1, left->items + 1),
 				FTree_incRef(tree->deep->middle),
 				FDigit_incRef(tree->deep->right));
 			return FView_make(head, tail);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_viewLeft(PSequence* self) {
+PyObject* PSequence_viewLeft(PSequence* self) {
 	if(FTree_empty(self->tree))
 		return PyErr_Format(PyExc_IndexError, "view from empty sequence");
 	FView view = FTree_viewLeft(self->tree);
 	assert(view.node->size == 1);
 	return Py_BuildValue("(ON)",
 		view.node->value, PSequence_make(view.tree));
 }
 
 // }}}
 
 // {{{ viewRight
 
-static FView FTree_viewRight(FTree* tree);
-
-static FTree* FTree_pullRight(FDigit* left, FTree* middle) {
+FTree* FTree_pullRight(FDigit* left, FTree* middle) {
 	if(FTree_empty(middle))
 		return FTree_fromDigit(left);
 	FView view = FTree_viewRight(middle);
 	FTree* init = FDeep_make(FTree_size(middle) + left->size,
 		FDigit_incRef(left), view.tree,
 		FDigit_fromNode(view.node));
 	return init;
 }
 
-static FView FTree_viewRight(FTree* tree) {
+FView FTree_viewRight(FTree* tree) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FSingleT: return FView_make(tree->single, FEmpty_make());
 		case FDeepT: {
 			FDigit* right = tree->deep->right;
 			FNode* last = right->items[right->count-1];
 			if(right->count == 1) return FView_make(last,
@@ -1218,74 +989,74 @@
 			FTree* init = FDeep_make(tree->deep->size - last->size,
 				FDigit_incRef(tree->deep->left),
 				FTree_incRef(tree->deep->middle),
 				FDigit_makeN(right->size - last->size,
 					right->count - 1, right->items));
 			return FView_make(last, init);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_viewRight(PSequence* self) {
+PyObject* PSequence_viewRight(PSequence* self) {
 	if(FTree_empty(self->tree))
 		return PyErr_Format(PyExc_IndexError, "view from empty sequence");
 	FView view = FTree_viewRight(self->tree);
 	assert(view.node->size == 1);
 	return Py_BuildValue("(NO)",
 		PSequence_make(view.tree), view.node->value);
 }
 
 // }}}
 
 // {{{ peek
 
-static PyObject* FTree_peekLeft(FTree* tree) {
+PyObject* FTree_peekLeft(FTree* tree) {
 	switch(tree->type) {
 		case FEmptyT: return PyErr_Format(
 			PyExc_IndexError, "peek from empty sequence");
 		case FSingleT:
 			assert(tree->single->size == 1);
 			return PObj_IncRef(tree->single->value);
 		case FDeepT:
 			assert(tree->deep->left->items[0]->size == 1);
 			return PObj_IncRef(tree->deep->left->items[0]->value);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_peekLeft(PSequence* self, void* UNUSED _ignore) {
+PyObject* PSequence_peekLeft(PSequence* self, void* UNUSED _ignore) {
 	return FTree_peekLeft(self->tree);
 }
 
-static PyObject* FTree_peekRight(FTree* tree) {
+PyObject* FTree_peekRight(FTree* tree) {
 	switch(tree->type) {
 		case FEmptyT: return PyErr_Format(
 			PyExc_IndexError, "peek from empty sequence");
 		case FSingleT:
 			assert(tree->single->size == 1);
 			return PObj_IncRef(tree->single->value);
 		case FDeepT: {
 			FDigit* right = tree->deep->right;
 			assert(right->items[right->count - 1]->size == 1);
 			return PObj_IncRef(right->items[right->count - 1]->value);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_peekRight(PSequence* self, void* UNUSED _ignore) {
+PyObject* PSequence_peekRight(PSequence* self, void* UNUSED _ignore) {
 	return FTree_peekRight(self->tree);
 }
 
 // }}}
 
 // {{{ fromIterable
 
-static FTree* FTree_fromNodes(size_t size, size_t count, FNode** nodes) {
+FTree* FTree_fromNodes(size_t size, size_t count, FNode** nodes) {
 	#ifndef NDEBUG
 		size_t sizeD = 0;
 		for(size_t i = 0; i < count; ++i)
 			sizeD += nodes[i]->size;
 		assert(size == sizeD);
 	#endif
 	if(count == 0) return FEmpty_make();
@@ -1318,249 +1089,249 @@
 			break;
 		case 2:
 			x = *input++; y = *input++; z = *input++;
 			*output++ = FNode_makeS(x, y, z);
 			x = *input++; y = *input++;
 			*output++ = FNode_makeS(x, y, NULL);
 			break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	size_t sizeN = size - left->size - right->size;
 	FTree* tree = FDeep_make(size, left,
 		FTree_fromNodes(sizeN, output - nodes, nodes), right);
 	return tree;
 }
 
-static PSequence* PSequence_fromIterable(PyObject* sequence) {
+PSequence* PSequence_fromIterable(PyObject* sequence) {
 	assert(sequence != NULL);
+	if(sequence == Py_None)
+		return PObj_IncRef(EMPTY_SEQUENCE);
 	if(Py_TYPE(sequence) == &PSequenceType)
 		return PObj_IncRef(sequence);
 	if(Py_TYPE(sequence) == &PSequenceEvolverType)
 		return PObj_IncRef(((PSequenceEvolver*)sequence)->seq);
 	PyObject* seq = PySequence_Fast(sequence, "expected a sequence");
 	if(seq == NULL) return NULL;
 	Py_ssize_t size = PySequence_Fast_GET_SIZE(seq);
-	FNode** nodes = PyMem_Malloc(size * sizeof(FNode*));
+	FNode** nodes = (FNode**)PyMem_Malloc(size * sizeof(FNode*));
 	PyObject** iter = PySequence_Fast_ITEMS(seq);
 	for(Py_ssize_t i = 0; i < size; ++i)
 		nodes[i] = FNode_makeE(PObj_IncRef(*iter++));
 	Py_DECREF(seq);
 	FTree* tree = FTree_fromNodes(size, size, nodes);
 	PyMem_Free(nodes);
 	return PSequence_make(tree);
 }
 
 // }}}
 
 // {{{ toTuple
 
-static size_t FNode_toTuple(FNode* node, PyObject* tuple, size_t index) {
+size_t FNode_toTuple(FNode* node, PyObject* tuple, size_t index) {
 	assert(node != NULL);
 	if(node->size == 1) {
 		PyTuple_SET_ITEM(tuple, index, PObj_IncRef(node->value));
 		return index + 1;
 	}
 	index = FNode_toTuple(node->items[0], tuple, index);
 	index = FNode_toTuple(node->items[1], tuple, index);
 	if(node->items[2] != NULL)
 		index = FNode_toTuple(node->items[2], tuple, index);
 	return index;
 }
 
-static size_t FDigit_toTuple(FDigit* digit, PyObject* tuple, size_t index) {
+size_t FDigit_toTuple(FDigit* digit, PyObject* tuple, size_t index) {
 	assert(digit != NULL);
 	for(int i = 0; i < digit->count; ++i)
 		index = FNode_toTuple(digit->items[i], tuple, index);
 	return index;
 }
 
-static size_t FTree_toTuple(FTree* tree, PyObject* tuple, size_t index) {
+size_t FTree_toTuple(FTree* tree, PyObject* tuple, size_t index) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return index;
 		case FSingleT: return FNode_toTuple(tree->single, tuple, index);
 		case FDeepT:
 			index = FDigit_toTuple(tree->deep->left, tuple, index);
 			index = FTree_toTuple(tree->deep->middle, tuple, index);
 			return FDigit_toTuple(tree->deep->right, tuple, index);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_toTuple(PSequence* self) {
+PyObject* PSequence_toTuple(PSequence* self) {
 	size_t size = FTree_size(self->tree);
 	PyObject* tuple = PyTuple_New(size);
 	if(tuple == NULL) return NULL;
 	size_t end UNUSED =
 		FTree_toTuple(self->tree, tuple, 0);
 	assert(end == size);
 	return tuple;
 }
 
 // }}}
 
 // {{{ toList
 
-static size_t FNode_toList(FNode* node, PyObject* list, size_t index) {
+size_t FNode_toList(FNode* node, PyObject* list, size_t index) {
 	assert(node != NULL);
 	if(node->size == 1) {
 		PyList_SET_ITEM(list, index, PObj_IncRef(node->value));
 		return index + 1;
 	}
 	index = FNode_toList(node->items[0], list, index);
 	index = FNode_toList(node->items[1], list, index);
 	if(node->items[2] != NULL)
 		index = FNode_toList(node->items[2], list, index);
 	return index;
 }
 
-static size_t FDigit_toList(FDigit* digit, PyObject* list, size_t index) {
+size_t FDigit_toList(FDigit* digit, PyObject* list, size_t index) {
 	assert(digit != NULL);
 	for(int i = 0; i < digit->count; ++i)
 		index = FNode_toList(digit->items[i], list, index);
 	return index;
 }
 
-static size_t FTree_toList(FTree* tree, PyObject* list, size_t index) {
+size_t FTree_toList(FTree* tree, PyObject* list, size_t index) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return index;
 		case FSingleT: return FNode_toList(tree->single, list, index);
 		case FDeepT:
 			index = FDigit_toList(tree->deep->left, list, index);
 			index = FTree_toList(tree->deep->middle, list, index);
 			return FDigit_toList(tree->deep->right, list, index);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_toList(PSequence* self) {
+PyObject* PSequence_toList(PSequence* self) {
 	size_t size = FTree_size(self->tree);
 	PyObject* list = PyList_New(size);
 	if(list == NULL) return NULL;
 	size_t end UNUSED =
 		FTree_toList(self->tree, list, 0);
 	assert(end == size);
 	return list;
 }
 
 // }}}
 
 // {{{ getItem
 
-static void* FNode_getItem(const FNode* node, size_t index) {
+void* FNode_getItem(const FNode* node, size_t index) {
 	assert(node != NULL);
 	assert(index < node->size);
 	if(node->size == 1)
 		return node->value;
 	size_t size;
 	if(index < (size = node->items[0]->size))
 		return FNode_getItem(node->items[0], index);
 	index -= size;
 	if(index < (size = node->items[1]->size))
 		return FNode_getItem(node->items[1], index);
 	index -= size;
 	return FNode_getItem(node->items[2], index);
 }
 
-static void* FDigit_getItem(const FDigit* digit, size_t index) {
+void* FDigit_getItem(const FDigit* digit, size_t index) {
 	assert(index < digit->size);
 	size_t size;
 	for(int i = 0; i < digit->count; ++i)
 		if(index < (size = digit->items[i]->size))
 			return FNode_getItem(digit->items[i], index);
 		else
 			index -= size;
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static void* FTree_getItem(const FTree* tree, size_t index) {
+void* FTree_getItem(const FTree* tree, size_t index) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: return FNode_getItem(tree->single, index);
 		case FDeepT: {
 			size_t size;
 			if(index < (size = tree->deep->left->size))
 				return FDigit_getItem(tree->deep->left, index);
 			index -= size;
 			if(index < (size = FTree_size(tree->deep->middle)))
 				return FTree_getItem(tree->deep->middle, index);
 			index -= size;
 			return FDigit_getItem(tree->deep->right, index);
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_getItem(const PSequence* self, Py_ssize_t index) {
+PyObject* PSequence_getItem(const PSequence* self, Py_ssize_t index) {
 	if(!(0 <= index && index < FTree_ssize(self->tree)))
 		return PSequence_indexError(index);
 	PyObject* value = FTree_getItem(self->tree, index);
 	assert(value != NULL);
 	return PObj_IncRef(value);
 }
 
-static PyObject* PSequence_getItemS(const PSequence* self, Py_ssize_t index) {
+PyObject* PSequence_getItemS(const PSequence* self, Py_ssize_t index) {
 	if(index < 0) index += FTree_ssize(self->tree);
 	return PSequence_getItem(self, index);
 }
 
 // }}}
 
 // {{{ traverse
 
-static int FNode_traverse(FNode* node, visitproc visit, void* arg) {
+int FNode_traverse(FNode* node, visitproc visit, void* arg) {
 	assert(node != NULL);
 	if(node->size == 1) {
 		Py_VISIT(node->value);
 		return 0;
 	}
 	int ret = FNode_traverse(node->items[0], visit, arg);
 	if(ret != 0) return ret;
 	ret = FNode_traverse(node->items[1], visit, arg);
 	if(ret != 0) return ret;
 	if(node->items[2] == NULL) return 0;
 	return FNode_traverse(node->items[2], visit, arg);
 }
 
-static int FDigit_traverse(FDigit* digit, visitproc visit, void* arg) {
+int FDigit_traverse(FDigit* digit, visitproc visit, void* arg) {
 	assert(digit != NULL);
 	for(int i = 0; i < digit->count; ++i) {
 		int ret = FNode_traverse(digit->items[i], visit, arg);
 		if(ret != 0) return ret;
 	}
 	return 0;
 }
 
-static int FTree_traverse(FTree* tree, visitproc visit, void* arg) {
+int FTree_traverse(FTree* tree, visitproc visit, void* arg) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return 0;
 		case FSingleT: return FNode_traverse(tree->single, visit, arg);
 		case FDeepT: {
 			int ret = FDigit_traverse(tree->deep->left, visit, arg);
 			if(ret != 0) return ret;
 			ret = FTree_traverse(tree->deep->middle, visit, arg);
 			if(ret != 0) return ret;
 			return FDigit_traverse(tree->deep->right, visit, arg);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static int PSequence_traverse(PSequence* self, visitproc visit, void* arg) {
+int PSequence_traverse(PSequence* self, visitproc visit, void* arg) {
 	return FTree_traverse(self->tree, visit, arg);
 }
 
 // }}}
 
 // {{{ concat
 
-static FTree* FTree_extend(FTree* xs, FTree* ys);
-
-static FTree* FDeep_extend(FDeep* xs, FDeep* ys) {
+FTree* FDeep_extend(FDeep* xs, FDeep* ys) {
 	size_t size = xs->size + ys->size;
 	FNode* mid[8]; int count = 0;
 	for(; count < xs->right->count; ++count)
 		mid[count] = FNode_incRef(xs->right->items[count]);
 	for(int i = 0; i < ys->left->count; ++i, ++count)
 		mid[count] = FNode_incRef(ys->left->items[i]);
 	FTree* right = FTree_incRef(ys->middle);
@@ -1582,57 +1353,57 @@
 			FNode_makeS(mid[4], mid[5], mid[6])));
 		case 4:
 			right = FTree_decRefRet(right, FTree_appendLeft(right,
 				FNode_makeS(mid[2], mid[3], NULL)));
 			right = FTree_decRefRet(right, FTree_appendLeft(right,
 				FNode_makeS(mid[0], mid[1], NULL)));
 		break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	return FTree_decRefRet(right, FDeep_make(size,
 		FDigit_incRef(xs->left),
 		FTree_extend(xs->middle, right),
 		FDigit_incRef(ys->right)));
 }
 
-static FTree* FTree_extend(FTree* xs, FTree* ys) {
+FTree* FTree_extend(FTree* xs, FTree* ys) {
 	switch(xs->type) {
 		case FEmptyT: return FTree_incRef(ys);
 		case FSingleT: return FTree_appendLeft(ys, FNode_incRef(xs->single));
 		case FDeepT: switch(ys->type) {
 			case FEmptyT: return FTree_incRef(xs);
 			case FSingleT: return FTree_appendRight(xs, FNode_incRef(ys->single));
 			case FDeepT: return FDeep_extend(xs->deep, ys->deep);
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_extendRight(PSequence* self, PyObject* arg) {
+PSequence* PSequence_extendRight(PSequence* self, PyObject* arg) {
 	PSequence* other = PSequence_fromIterable(arg);
 	if(other == NULL) return NULL;
 	PSequence* ret = PSequence_make(FTree_extend(self->tree, other->tree));
 	Py_DECREF(other);
 	return ret;
 }
 
-static PSequence* PSequence_extendLeft(PSequence* self, PyObject* arg) {
+PSequence* PSequence_extendLeft(PSequence* self, PyObject* arg) {
 	PSequence* other = PSequence_fromIterable(arg);
 	if(other == NULL) return NULL;
 	PSequence* ret = PSequence_make(FTree_extend(other->tree, self->tree));
 	Py_DECREF(other);
 	return ret;
 }
 
 // }}}
 
 // {{{ repeat
 
-static PSequence* PSequence_repeat(PSequence* self, Py_ssize_t count) {
+PSequence* PSequence_repeat(PSequence* self, Py_ssize_t count) {
 	if(count <= 0) return PObj_IncRef(EMPTY_SEQUENCE);
 	FTree* result = FEmpty_make();
 	FTree* tree = FTree_incRef(self->tree);
 	if(count & 1) result = FTree_decRefRet(result, FTree_extend(tree, result));
 	for(count >>= 1; count != 0; count >>= 1) {
 		tree = FTree_decRefRet(tree, FTree_extend(tree, tree));
 		if(count & 1) result = FTree_decRefRet(result, FTree_extend(tree, result));
@@ -1640,15 +1411,15 @@
 	return PSequence_make(FTree_decRefRet(tree, result));
 }
 
 // }}}
 
 // {{{ setItem
 
-static FNode* FNode_setItem(
+FNode* FNode_setItem(
 	const FNode* node,
 	size_t index,
 	const PyObject* value
 ) {
 	assert(node != NULL);
 	assert(index < node->size);
 	if(node->size == 1)
@@ -1668,15 +1439,15 @@
 	index -= size;
 	return FNode_make(node->size,
 		FNode_incRef(node->items[0]),
 		FNode_incRef(node->items[1]),
 		FNode_setItem(node->items[2], index, value));
 }
 
-static FDigit* FDigit_setItem(
+FDigit* FDigit_setItem(
 	const FDigit* digit,
 	size_t index,
 	const PyObject* value
 ) {
 	assert(index < digit->size);
 	FNode* nodes[4] = { NULL, NULL, NULL, NULL };
 	for(int i = 0; i < digit->count; ++i)
@@ -1685,18 +1456,18 @@
 	for(int i = 0; i < digit->count; ++i)
 		if(index < (size =digit->items[i]->size)) {
 			FNode_decRef(nodes[i]);
 			nodes[i] = FNode_setItem(nodes[i], index, value);
 			return FDigit_make(digit->size, digit->count,
 				nodes[0], nodes[1], nodes[2], nodes[3]);
 		} else index -= size;
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FTree* FTree_setItem(
+FTree* FTree_setItem(
 	const FTree* tree,
 	size_t index,
 	const PyObject* value
 ) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: return FSingle_make(
@@ -1715,30 +1486,30 @@
 					FTree_setItem(tree->deep->middle, index, value),
 					FDigit_incRef(tree->deep->right));
 			index -= size;
 			return FDeep_make(tree->deep->size,
 				FDigit_incRef(tree->deep->left),
 				FTree_incRef(tree->deep->middle),
 				FDigit_setItem(tree->deep->right, index, value));
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_setItem(
+PSequence* PSequence_setItem(
 	PSequence* self,
 	Py_ssize_t index,
 	PyObject* value
 ) {
 	if(!(0 <= index && index < FTree_ssize(self->tree)))
 		return PSequence_indexError(index);
 	return PSequence_make(FTree_setItem(
 		self->tree, index, PObj_IncRef(value)));
 }
 
-static PSequence* PSequence_setItemS(
+PSequence* PSequence_setItemS(
 	PSequence* self,
 	Py_ssize_t index,
 	PyObject* value
 ) {
 	if(!FTree_checkIndex(self->tree, &index))
 		return PSequence_indexError(index);
 	return PSequence_make(FTree_setItem(
@@ -1757,15 +1528,15 @@
 		// self->tree, index, PObj_IncRef(value)));
 // }
 
 // }}}
 
 // {{{ msetItem
 
-static FNode* FNode_msetItem(FNode* node, FMset* mset) {
+FNode* FNode_msetItem(FNode* node, FMset* mset) {
 	if(mset->count == 0)
 		return FNode_incRef(node);
 	if(mset->index + node->size <= mset->items->index1) {
 		mset->index += node->size;
 		return FNode_incRef(node);
 	}
 	if(node->size == 1) {
@@ -1778,28 +1549,28 @@
 	nodes[0] = FNode_msetItem(node->items[0], mset);
 	nodes[1] = FNode_msetItem(node->items[1], mset);
 	nodes[2] = node->items[2] == NULL ? NULL
 		: FNode_msetItem(node->items[2], mset);
 	return FNode_make(node->size, nodes[0], nodes[1], nodes[2]);
 }
 
-static FDigit* FDigit_msetItem(FDigit* digit, FMset* mset) {
+FDigit* FDigit_msetItem(FDigit* digit, FMset* mset) {
 	if(mset->count == 0)
 		return FDigit_incRef(digit);
 	if(mset->index + digit->size <= mset->items->index1) {
 		mset->index += digit->size;
 		return FDigit_incRef(digit);
 	}
 	FNode* nodes[4];
 	for(int i = 0; i < digit->count; ++i)
 		nodes[i] = FNode_msetItem(digit->items[i], mset);
 	return FDigit_makeN(digit->size, digit->count, nodes);
 }
 
-static FTree* FTree_msetItem(FTree* tree, FMset* mset) {
+FTree* FTree_msetItem(FTree* tree, FMset* mset) {
 	if(mset->count == 0)
 		return FTree_incRef(tree);
 	if(mset->index + FTree_size(tree) <= mset->items->index1) {
 		mset->index += FTree_size(tree);
 		return FTree_incRef(tree);
 	}
 	switch(tree->type) {
@@ -1807,23 +1578,23 @@
 			FNode_msetItem(tree->single, mset));
 		case FDeepT: {
 			FDigit* left = FDigit_msetItem(tree->deep->left, mset);
 			FTree* middle = FTree_msetItem(tree->deep->middle, mset);
 			FDigit* right = FDigit_msetItem(tree->deep->right, mset);
 			return FDeep_make(tree->deep->size, left, middle, right);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_msetItemN(PSequence* self, PyObject* args) {
+PSequence* PSequence_msetItemN(PSequence* self, PyObject* args) {
 	Py_ssize_t argc = PyTuple_GET_SIZE(args);
 	if(argc == 0) return PObj_IncRef(self);
 	FMset mset = { .index = 0, .count = 0, .items = NULL };
-	FIndex2* items = (mset.items = PyMem_Malloc(argc * sizeof(FIndex2)));
+	FIndex2* items = (mset.items = (FIndex2*)PyMem_Malloc(argc * sizeof(FIndex2)));
 	items = items;
 	for(Py_ssize_t i = 0; i < argc; ++i)
 		items[i].value = NULL;
 	for(Py_ssize_t index = 0; index < argc; ++index) {
 		Py_ssize_t sindex;
 		PyObject* arg = PyTuple_GET_ITEM(args, index);
 		if(PyIndex_Check(arg)) {
@@ -1867,15 +1638,15 @@
 		return NULL;
 }
 
 // }}}
 
 // {{{ insertItem
 
-static FInsert FNode_insertItem(FNode* node, size_t index, PyObject* item) {
+FInsert FNode_insertItem(FNode* node, size_t index, PyObject* item) {
 	assert(index < node->size);
 	if(node->size == 1) return FInsert_make(
 		FNode_incRef(node), FNode_makeE(PObj_IncRef(item)));
 	FNode* nodes[4] = { NULL, NULL, NULL, NULL };
 	do {
 		size_t size;
 		if(index < (size = node->items[0]->size)) {
@@ -1914,15 +1685,15 @@
 	if(nodes[3] == NULL) return FInsert_make(NULL,
 		FNode_make(node->size + 1, nodes[0], nodes[1], nodes[2]));
 	return FInsert_make(
 		FNode_makeS(nodes[2], nodes[3], NULL),
 		FNode_makeS(nodes[0], nodes[1], NULL));
 }
 
-static FInsert FDigit_insertLeft(FDigit* digit, size_t index, PyObject* item) {
+FInsert FDigit_insertLeft(FDigit* digit, size_t index, PyObject* item) {
 	assert(index < digit->size);
 	FNode* nodes[5] = { NULL, NULL, NULL, NULL, NULL };
 	int mid = 0, count;
 	for(; mid < digit->count; ++mid) {
 		if(index < digit->items[mid]->size) break;
 		nodes[mid] = FNode_incRef(digit->items[mid]);
 		index -= digit->items[mid]->size;
@@ -1946,15 +1717,15 @@
 	if(nodes[4] == NULL) return FInsert_make(NULL,
 		FDigit_makeN(digit->size + 1, count, nodes));
 	return FInsert_make(
 		FNode_makeS(nodes[2], nodes[3], nodes[4]),
 		FDigit_makeNS(2, nodes));
 }
 
-static FInsert FDigit_insertRight(FDigit* digit, size_t index, PyObject* item) {
+FInsert FDigit_insertRight(FDigit* digit, size_t index, PyObject* item) {
 	assert(index < digit->size);
 	FNode* nodes[5] = { NULL, NULL, NULL, NULL, NULL };
 	int mid = 0, count;
 	for(; mid < digit->count; ++mid) {
 		if(index < digit->items[mid]->size) break;
 		nodes[mid] = FNode_incRef(digit->items[mid]);
 		index -= digit->items[mid]->size;
@@ -1978,15 +1749,15 @@
 	if(nodes[4] == NULL) return FInsert_make(NULL,
 		FDigit_makeN(digit->size + 1, count, nodes));
 	return FInsert_make(
 		FNode_makeS(nodes[0], nodes[1], nodes[2]),
 		FDigit_makeNS(2, nodes + 3));
 }
 
-static FTree* FTree_insertItem(FTree* tree, size_t index, PyObject* item) {
+FTree* FTree_insertItem(FTree* tree, size_t index, PyObject* item) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: {
 			FInsert ins = FNode_insertItem(tree->single, index, item);
 			assert(tree->single->size + 1 ==
 				ins.digit->size + (ins.extra == NULL ? 0 : ins.extra->size));
 			if(ins.extra == NULL) return FSingle_make(ins.node);
@@ -2024,33 +1795,33 @@
 				FTree* middle = ins.extra == NULL
 					? FTree_incRef(tree->deep->middle)
 					: FTree_appendRight(tree->deep->middle, ins.extra);
 				return FDeep_make(tree->deep->size + 1,
 					FDigit_incRef(tree->deep->left), middle, ins.digit);
 			}
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_insertItemN(PSequence* self, PyObject* args) {
+PSequence* PSequence_insertItemN(PSequence* self, PyObject* args) {
 	Py_ssize_t index; PyObject* value;
 	if(!PyArg_ParseTuple(args, "nO", &index, &value)) return NULL;
 	if(!FTree_checkIndex(self->tree, &index)) {
 		if(index < 0) return PSequence_appendLeft(self, value);
 		return PSequence_appendRight(self, value);
 	}
 	return PSequence_make(FTree_insertItem(self->tree, index, value));
 }
 
 // }}}
 
 // {{{ merge/meld
 
-static FMerge FNode_mergeLeft(FNode* left, FNode* node) {
+FMerge FNode_mergeLeft(FNode* left, FNode* node) {
 	if(left == NULL)
 		return FMerge_make(FNode_incRef(node), NULL);
 	assert(FNode_depth(left) + 1 == FNode_depth(node));
 	if(node->items[2] == NULL)
 		return FMerge_make(FNode_makeS(
 			left,
 			FNode_incRef(node->items[0]),
@@ -2060,15 +1831,15 @@
 			left,
 			FNode_incRef(node->items[0]), NULL),
 		FNode_makeS(
 			FNode_incRef(node->items[1]),
 			FNode_incRef(node->items[2]), NULL));
 }
 
-static FMerge FNode_mergeRight(FNode* node, FNode* right) {
+FMerge FNode_mergeRight(FNode* node, FNode* right) {
 	if(right == NULL)
 		return FMerge_make(FNode_incRef(node), NULL);
 	assert(FNode_depth(node) == FNode_depth(right) + 1);
 	if(node->items[2] == NULL)
 		return FMerge_make(FNode_makeS(
 			FNode_incRef(node->items[0]),
 			FNode_incRef(node->items[1]),
@@ -2078,15 +1849,15 @@
 			FNode_incRef(node->items[0]),
 			FNode_incRef(node->items[1]), NULL),
 		FNode_makeS(
 			FNode_incRef(node->items[2]),
 			right, NULL));
 }
 
-static FDigit* FDigit_mergeLeft(FNode* left, FNode* node) {
+FDigit* FDigit_mergeLeft(FNode* left, FNode* node) {
 	if(left == NULL)
 		return FDigit_fromNode(node);
 	assert(FNode_depth(left) + 2 == FNode_depth(node));
 	FMerge merge = FNode_mergeLeft(left, node->items[0]);
 	if(merge.extra == NULL)
 		return FDigit_makeS(
 			FNode_count(node),
@@ -2097,15 +1868,15 @@
 		FNode_count(node) + 1,
 		merge.left,
 		merge.right,
 		FNode_incRef(node->items[1]),
 		FNode_incRefM(node->items[2]));
 }
 
-static FDigit* FDigit_mergeRight(FNode* node, FNode* right) {
+FDigit* FDigit_mergeRight(FNode* node, FNode* right) {
 	if(right == NULL)
 		return FDigit_fromNode(node);
 	assert(FNode_depth(right) + 2 == FNode_depth(node));
 	if(node->items[2] == NULL) {
 		FMerge merge = FNode_mergeRight(node->items[1], right);
 		return FDigit_makeS(merge.extra == NULL ? 2 : 3,
 			FNode_incRef(node->items[0]),
@@ -2115,44 +1886,42 @@
 		return FDigit_makeS(merge.extra == NULL ? 3 : 4,
 			FNode_incRef(node->items[0]),
 			FNode_incRef(node->items[1]),
 			merge.left, merge.right);
 	}
 }
 
-static FMeld FNode_meldLeft(FNode* extra, FMerge merge) {
+FMeld FNode_meldLeft(FNode* extra, FMerge merge) {
 	if(merge.extra != NULL) {
 		if(extra == NULL)
 			return FMeld_make(true, FNode_makeS(merge.left, merge.right, NULL));
 		return FMeld_make(true, FNode_makeS(
 			FNode_incRef(extra), merge.left, merge.right));
 	}
 	if(extra == NULL)
 		return FMeld_make(false, merge.node);
 	return FMeld_make(true, FNode_makeS(
 		FNode_incRef(extra), merge.node, NULL));
 }
 
-static FMeld FNode_meldRight(FMerge merge, FNode* extra) {
+FMeld FNode_meldRight(FMerge merge, FNode* extra) {
 	if(merge.extra != NULL) 
 		return FMeld_make(true, FNode_makeS(
 			merge.left, merge.right, FNode_incRefM(extra)));
 	if(extra == NULL)
 		return FMeld_make(false, merge.node);
 	return FMeld_make(true, FNode_makeS(
 		merge.node, FNode_incRefM(extra), NULL));
 }
 
 // }}}
 
 // {{{ deleteItem
 
-static FMeld FTree_deleteItem(FTree* tree, size_t index);
-
-static FMeld FNode_deleteItem(FNode* node, size_t index) {
+FMeld FNode_deleteItem(FNode* node, size_t index) {
 	assert(index < node->size);
 	if(node->size == 1) return FMeld_make(false, NULL);
 	size_t size;
 	if(index < (size = node->items[0]->size)) {
 		FMeld meld = FNode_deleteItem(node->items[0], index);
 		if(meld.full) return FMeld_make(true,
 			FNode_make(node->size - 1, meld.node,
@@ -2175,15 +1944,15 @@
 			FNode_make(node->size - 1, FNode_incRef(node->items[0]),
 				FNode_incRef(node->items[1]), meld.node));
 		return FNode_meldLeft(node->items[0],
 			FNode_mergeRight(node->items[1], meld.node));
 	}
 }
 
-static FMeld FDigit_deleteItem(FDigit* digit, size_t index) {
+FMeld FDigit_deleteItem(FDigit* digit, size_t index) {
 	assert(index < digit->size);
 	FNode* nodes[4] = { NULL, NULL, NULL, NULL };
 	int mid = 0, count;
 	for(; mid < digit->count; ++mid) {
 		if(index < digit->items[mid]->size) break;
 		nodes[mid] = FNode_incRef(digit->items[mid]);
 		index -= digit->items[mid]->size;
@@ -2224,15 +1993,15 @@
 				nodes[i] = FNode_incRef(digit->items[i]);
 			count = digit->count;
 		}
 	}
 	return FMeld_make(true, FDigit_makeNS(count, nodes));
 }
 
-static FMeld FTree_deleteItemLeft(FTree* tree, size_t index) {
+FMeld FTree_deleteItemLeft(FTree* tree, size_t index) {
 	FMeld meld = FDigit_deleteItem(tree->deep->left, index);
 	if(meld.full) return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		meld.digit,
 		FTree_incRef(tree->deep->middle),
 		FDigit_incRef(tree->deep->right)));
 	if(!FTree_empty(tree->deep->middle)) {
 		FView view = FTree_viewLeft(tree->deep->middle);
@@ -2249,15 +2018,15 @@
 	return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		FDigit_fromMerge(merge),
 		FEmpty_make(),
 		FDigit_makeNS(tree->deep->right->count - 1,
 			tree->deep->right->items + 1)));
 }
 
-static FMeld FTree_deleteItemRight(FTree* tree, size_t index) {
+FMeld FTree_deleteItemRight(FTree* tree, size_t index) {
 	FMeld meld = FDigit_deleteItem(tree->deep->right, index);
 	if(meld.full) return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		FDigit_incRef(tree->deep->left),
 		FTree_incRef(tree->deep->middle),
 		meld.digit));
 	if(!FTree_empty(tree->deep->middle)) {
 		FView view = FTree_viewRight(tree->deep->middle);
@@ -2275,15 +2044,15 @@
 	return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		FDigit_makeNS(tree->deep->left->count - 1,
 			tree->deep->left->items),
 		FEmpty_make(),
 		FDigit_fromMerge(merge)));
 }
 
-static FMeld FTree_deleteItemMiddle(FTree* tree, size_t index) {
+FMeld FTree_deleteItemMiddle(FTree* tree, size_t index) {
 	FMeld meld = FTree_deleteItem(tree->deep->middle, index);
 	if(meld.full) return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		FDigit_incRef(tree->deep->left),
 		meld.tree,
 		FDigit_incRef(tree->deep->right)));
 	FNode* nodes[4];
 	for(int i = 0; i < tree->deep->left->count; ++i)
@@ -2299,15 +2068,15 @@
 	}
 	return FMeld_make(true, FDeep_make(tree->deep->size - 1,
 		FDigit_makeNS(2, nodes),
 		FSingle_make(FNode_makeS(nodes[2], nodes[3], meld.node)),
 		FDigit_incRef(tree->deep->right)));
 }
 
-static FMeld FTree_deleteItem(FTree* tree, size_t index) {
+FMeld FTree_deleteItem(FTree* tree, size_t index) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: {
 			FMeld meld = FNode_deleteItem(tree->single, index);
 			if(meld.full) meld.tree = FSingle_make(meld.node);
 			return meld;
 		}
@@ -2318,133 +2087,130 @@
 			index -= size;
 			if(index < (size = FTree_size(tree->deep->middle)))
 				return FTree_deleteItemMiddle(tree, index);
 			index -= size;
 			assert(index < tree->deep->right->size);
 			return FTree_deleteItemRight(tree, index);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_deleteItem(PSequence* self, Py_ssize_t index) {
+PSequence* PSequence_deleteItem(PSequence* self, Py_ssize_t index) {
 	if(!(0 <= index && index < FTree_ssize(self->tree)))
 		return PSequence_indexError(index);
 	FMeld meld = FTree_deleteItem(self->tree, index);
 	assert((meld.node == NULL) == !meld.full);
 	if(!meld.full) return PObj_IncRef(EMPTY_SEQUENCE);
 	return PSequence_make(meld.tree);
 }
 
-static PSequence* PSequence_deleteItemS(PSequence* self, Py_ssize_t index) {
+PSequence* PSequence_deleteItemS(PSequence* self, Py_ssize_t index) {
 	if(!FTree_checkIndex(self->tree, &index))
 		return PSequence_indexError(index);
 	FMeld meld = FTree_deleteItem(self->tree, index);
 	assert((meld.node == NULL) == !meld.full);
 	if(!meld.full) return PObj_IncRef(EMPTY_SEQUENCE);
 	return PSequence_make(meld.tree);
 }
 
 // }}}
 
 // {{{ contains
 
-static int FNode_contains(FNode* node, PyObject* arg) {
+int FNode_contains(FNode* node, PyObject* arg) {
 	assert(node != NULL);
 	if(node->size == 1)
 		return PyObject_RichCompareBool(node->value, arg, Py_EQ);
 	int comp;
 	if((comp = FNode_contains(node->items[0], arg)) != 0) return comp;
 	if((comp = FNode_contains(node->items[1], arg)) != 0) return comp;
 	if(node->items[2] == NULL) return 0;
 	return FNode_contains(node->items[2], arg);
 }
 
-static int FDigit_contains(FDigit* digit, PyObject* arg) {
+int FDigit_contains(FDigit* digit, PyObject* arg) {
 	assert(digit != NULL);
 	for(int i = 0; i < digit->count; ++i) {
 		int comp = FNode_contains(digit->items[i], arg);
 		if(comp != 0) return comp;
 	}
 	return 0;
 }
 
-static int FTree_contains(FTree* tree, PyObject* arg) {
+int FTree_contains(FTree* tree, PyObject* arg) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return 0;
 		case FSingleT: return FNode_contains(tree->single, arg);
 		case FDeepT: {
 			int comp;
 			if((comp = FDigit_contains(tree->deep->left, arg)) != 0) return comp;
 			if((comp = FDigit_contains(tree->deep->right, arg)) != 0) return comp;
 			return FTree_contains(tree->deep->middle, arg);
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static int PSequence_contains(PSequence* self, PyObject* arg) {
+int PSequence_contains(PSequence* self, PyObject* arg) {
 	return FTree_contains(self->tree, arg);
 }
 
 // }}}
 
 // {{{ indexItem
 
-static PSequence* PSequence_takeLeft(PSequence* self, Py_ssize_t index);
-static PSequence* PSequence_takeRight(PSequence* self, Py_ssize_t index);
-
 #define check_and_return(index, offset) do { \
 	Py_ssize_t _idx = index; \
 	if(_idx < 0) return _idx; \
 	if(_idx > 0) return _idx + (offset); \
 	} while(0)
 
-static Py_ssize_t FNode_indexItem(FNode* node, PyObject* arg) {
+Py_ssize_t FNode_indexItem(FNode* node, PyObject* arg) {
 	assert(node != NULL);
 	if(node->size == 1) return (Py_ssize_t)
 		PyObject_RichCompareBool(node->value, arg, Py_EQ);
 	check_and_return(FNode_indexItem(node->items[0], arg), 0);
 	check_and_return(FNode_indexItem(node->items[1], arg),
 		node->items[0]->size);
 	if(node->items[2] == NULL) return 0;
 	check_and_return(FNode_indexItem(node->items[2], arg),
 		node->items[0]->size + node->items[1]->size);
 	return 0;
 }
 
-static Py_ssize_t FDigit_indexItem(FDigit* digit, PyObject* arg) {
+Py_ssize_t FDigit_indexItem(FDigit* digit, PyObject* arg) {
 	assert(digit != NULL);
 	int offset = 0;
 	for(int i = 0; i < digit->count; ++i) {
 		check_and_return(FNode_indexItem(digit->items[i], arg), offset);
 		offset += digit->items[i]->size;
 	}
 	return 0;
 }
 
-static Py_ssize_t FTree_indexItem(FTree* tree, PyObject* arg) {
+Py_ssize_t FTree_indexItem(FTree* tree, PyObject* arg) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return 0;
 		case FSingleT: return FNode_indexItem(tree->single, arg);
 		case FDeepT: {
 			check_and_return(FDigit_indexItem(tree->deep->left, arg), 0);
 			check_and_return(FTree_indexItem(tree->deep->middle, arg),
 				tree->deep->left->size);
 			check_and_return(FDigit_indexItem(tree->deep->right, arg),
 				tree->deep->left->size + FTree_size(tree->deep->middle));
 			return 0;
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
 #undef check_and_return
 
-static PyObject* PSequence_indexItem(PSequence* self, PyObject* args) {
+PyObject* PSequence_indexItem(PSequence* self, PyObject* args) {
 	PyObject* value; Py_ssize_t start = 0, stop = FTree_ssize(self->tree);
 	if(!PyArg_ParseTuple(args, "O|nn", &value, &start, &stop)) return NULL;
 	PSequence* seq1 = PSequence_takeRight(self, FTree_ssize(self->tree) - start);
 	PSequence* seq2 = PSequence_takeLeft(self, stop - start);
 	Py_DECREF(seq1);
 	Py_ssize_t index = FTree_indexItem(seq2->tree, value);
 	Py_DECREF(seq2);
@@ -2454,15 +2220,15 @@
 	return PyLong_FromSsize_t(index - 1 + (start >= 0 ? start : 0));
 }
 
 // }}}
 
 // {{{ removeItem
 
-static PSequence* PSequence_removeItemN(PSequence* self, PyObject* arg) {
+PSequence* PSequence_removeItemN(PSequence* self, PyObject* arg) {
 	Py_ssize_t index = FTree_indexItem(self->tree, arg);
 	if(index < 0) return NULL;
 	if(index == 0) return (void*)
 		PyErr_Format(PyExc_ValueError, "value not in sequence");
 	assert(0 < index && index <= FTree_ssize(self->tree));
 	FMeld meld = FTree_deleteItem(self->tree, (size_t)index - 1);
 	assert((meld.node == NULL) == !meld.full);
@@ -2470,67 +2236,65 @@
 	return PSequence_make(meld.tree);
 }
 
 // }}}
 
 // {{{ countItem
 
-static Py_ssize_t FNode_countItem(FNode* node, PyObject* arg) {
+Py_ssize_t FNode_countItem(FNode* node, PyObject* arg) {
 	assert(node != NULL);
 	if(node->size == 1)
 		return (Py_ssize_t)PyObject_RichCompareBool(node->value, arg, Py_EQ);
 	int comp, total;
 	if((comp = FNode_countItem(node->items[0], arg)) < 0) return comp;
 	total = comp;
 	if((comp = FNode_countItem(node->items[1], arg)) < 0) return comp;
 	total += comp;
 	if(node->items[2] == NULL) return total;
 	if((comp = FNode_countItem(node->items[2], arg)) < 0) return comp;
 	return total + comp;
 }
 
-static Py_ssize_t FDigit_countItem(FDigit* digit, PyObject* arg) {
+Py_ssize_t FDigit_countItem(FDigit* digit, PyObject* arg) {
 	assert(digit != NULL);
 	int total = 0;
 	for(int i = 0; i < digit->count; ++i) {
 		int comp = FNode_countItem(digit->items[i], arg);
 		if(comp < 0) return comp;
 		total += comp;
 	}
 	return total;
 }
 
-static Py_ssize_t FTree_countItem(FTree* tree, PyObject* arg) {
+Py_ssize_t FTree_countItem(FTree* tree, PyObject* arg) {
 	assert(tree != NULL);
 	switch(tree->type) {
 		case FEmptyT: return 0;
 		case FSingleT: return FNode_countItem(tree->single, arg);
 		case FDeepT: {
 			int comp, total;
 			if((comp = FDigit_countItem(tree->deep->left, arg)) < 0) return comp;
 			total = comp;
 			if((comp = FTree_countItem(tree->deep->middle, arg)) < 0) return comp;
 			total += comp;
 			if((comp = FDigit_countItem(tree->deep->right, arg)) < 0) return comp;
 			return total + comp;
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequence_countItem(PSequence* self, PyObject* arg) {
+PyObject* PSequence_countItem(PSequence* self, PyObject* arg) {
 	return PyLong_FromSsize_t(FTree_countItem(self->tree, arg));
 }
 
 // }}}
 
 // {{{ splitView
 
-static FSplit FTree_splitView(FTree* tree, size_t index);
-
-static FSplit FDeep_splitViewLeft(FDeep* deep, size_t index) {
+FSplit FDeep_splitViewLeft(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = 0; i < deep->left->count; ++i)
 		FNode_incRef(deep->left->items[i]);
 	for(int i = 0; i < deep->left->count; ++i)
 		if(index >= (size = deep->left->items[i]->size)) {
 			index -= size; dsize += size;
 		} else return FSplit_make(
@@ -2538,36 +2302,36 @@
 			FNode_decRefRet(deep->left->items[i], deep->left->items[i]),
 			i + 1 == deep->left->count
 				? FTree_pullLeft(deep->middle, deep->right)
 				: FDeep_make(deep->size - dsize - size,
 					FDigit_makeN(deep->left->size - dsize - size,
 						deep->left->count - i - 1, deep->left->items + i + 1),
 					FTree_incRef(deep->middle), FDigit_incRef(deep->right)));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FSplit FDeep_splitViewRight(FDeep* deep, size_t index) {
+FSplit FDeep_splitViewRight(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = 0; i < deep->right->count; ++i)
 		FNode_incRef(deep->right->items[i]);
 	for(int i = 0; i < deep->right->count; ++i)
 		if(index >= (size = deep->right->items[i]->size)) {
 			index -= size; dsize += size;
 		} else return FSplit_make(
 			i == 0 ? FTree_pullRight(deep->left, deep->middle)
 				: FDeep_make(deep->size - deep->right->size + dsize,
 					FDigit_incRef(deep->left), FTree_incRef(deep->middle),
 					FDigit_makeN(dsize, i, deep->right->items)),
 			FNode_decRefRet(deep->right->items[i], deep->right->items[i]),
 			FTree_fromNodes(deep->right->size - dsize - size,
 				deep->right->count - i - 1, deep->right->items + i + 1));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FSplit FDeep_splitViewMiddle(FDeep* deep, size_t index) {
+FSplit FDeep_splitViewMiddle(FDeep* deep, size_t index) {
 	FSplit split = FTree_splitView(deep->middle, index);
 	assert(split.node->size != 1);
 	index -= FTree_size(split.left);
 	size_t size, prefix = 0;
 	if(index < (size = split.node->items[0]->size)) {
 		FTree* left = FTree_decRefRet(split.left,
 			FTree_pullRight(deep->left, split.left));
@@ -2606,47 +2370,47 @@
 		FNode* middle = split.node->items[2];
 		FTree* right = FTree_decRefRet(split.right,
 			FTree_pullLeft(split.right, deep->right));
 		return FSplit_make(left, middle, right);
 	}
 }
 
-static FSplit FTree_splitView(FTree* tree, size_t index) {
+FSplit FTree_splitView(FTree* tree, size_t index) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: return FSplit_make(FEmpty_make(),
 			tree->single, FEmpty_make());
 		case FDeepT: {
 			size_t size;
 			if(index < (size = tree->deep->left->size))
 				return FDeep_splitViewLeft(tree->deep, index);
 			index -= size;
 			if(index < (size = FTree_size(tree->deep->middle)))
 				return FDeep_splitViewMiddle(tree->deep, index);
 			index -= size;
 			return FDeep_splitViewRight(tree->deep, index);
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
 // splitAt has to split nodes anyway, so just reuse splitView
-static PyObject* PSequence_splitAt(PSequence* self, PyObject* arg) {
+PyObject* PSequence_splitAt(PSequence* self, PyObject* arg) {
 	Py_ssize_t index = PyNumber_AsSsize_t(arg, PyExc_IndexError);
 	if(index == -1 && PyErr_Occurred()) return NULL;
 	if(!FTree_checkIndex(self->tree, &index) || index == 0) {
 		if(index <= 0) return Py_BuildValue("(OO)", EMPTY_SEQUENCE, self);
 		else return Py_BuildValue("(OO)", self, EMPTY_SEQUENCE);
 	}
 	FSplit split = FTree_splitView(self->tree, index);
 	return Py_BuildValue("(NN)", PSequence_make(split.left),
 		PSequence_make(FTree_decRefRet(split.right,
 			FTree_appendLeft(split.right, FNode_incRef(split.node)))));
 }
 
-static PyObject* PSequence_view(PSequence* self, PyObject* args) {
+PyObject* PSequence_view(PSequence* self, PyObject* args) {
 	Py_ssize_t argc = PyTuple_GET_SIZE(args);
 	if(argc == 1) {
 		Py_ssize_t index = PyNumber_AsSsize_t(
 			PyTuple_GET_ITEM(args, 0), PyExc_IndexError);
 		if(index == -1 && PyErr_Occurred()) return NULL;
 		if(!FTree_checkIndex(self->tree, &index))
 			return PSequence_indexError(index);
@@ -2689,15 +2453,15 @@
 		return NULL;
 }
 
 // }}}
 
 // {{{ chunksOf
 
-static PSequence* PSequence_chunksOf(PSequence* self, Py_ssize_t chunk) {
+PSequence* PSequence_chunksOf(PSequence* self, Py_ssize_t chunk) {
 	if(FTree_empty(self->tree)) return PObj_IncRef(self);
 	if(chunk <= 0) return (void*)PyErr_Format(
 		PyExc_ValueError, "chunk size must be positive");
 	FTree* left = FEmpty_make();
 	FTree* right = FTree_incRef(self->tree);
 	for(Py_ssize_t size = FTree_ssize(self->tree); size > chunk; size -= chunk) {
 		FSplit split = FTree_splitView(right, chunk);
@@ -2706,53 +2470,51 @@
 		right = FTree_decRefRet(right, FTree_decRefRet(split.right,
 			FTree_appendLeft(split.right, FNode_incRef(split.node))));
 	}
 	return FTree_decRefRet(left, PSequence_make(FTree_appendRight(left,
 		FNode_makeE((PyObject*)PSequence_make(right)))));
 }
 
-static PSequence* PSequence_chunksOfN(PSequence* self, PyObject* arg) {
+PSequence* PSequence_chunksOfN(PSequence* self, PyObject* arg) {
 	Py_ssize_t chunk = PyNumber_AsSsize_t(arg, PyExc_IndexError);
 	if(chunk == -1 && PyErr_Occurred()) return NULL;
 	return PSequence_chunksOf(self, chunk);
 }
 
 // }}}
 
 // {{{ takeLeft
 
-static FView FTree_takeLeft(FTree* tree, size_t index);
-
-static FView FDeep_takeLeftLeft(FDeep* deep, size_t index) {
+FView FDeep_takeLeftLeft(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = 0; i < deep->left->count; ++i)
 		if(index >= (size = deep->left->items[i]->size)) {
 			FNode_incRef(deep->left->items[i]);
 			index -= size; dsize += size;
 		} else return FView_make(deep->left->items[i],
 			FTree_fromNodes(dsize, i, deep->left->items));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FView FDeep_takeLeftRight(FDeep* deep, size_t index) {
+FView FDeep_takeLeftRight(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = 0; i < deep->right->count; ++i)
 		if(index >= (size = deep->right->items[i]->size)) {
 			FNode_incRef(deep->right->items[i]);
 			index -= size; dsize += size;
 		} else return FView_make(
 			deep->right->items[i],
 			i == 0 ? FTree_pullRight(deep->left, deep->middle)
 				: FDeep_make(deep->size - deep->right->size + dsize,
 					FDigit_incRef(deep->left), FTree_incRef(deep->middle),
 					FDigit_makeN(dsize, i, deep->right->items)));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FView FDeep_takeLeftMiddle(FDeep* deep, size_t index) {
+FView FDeep_takeLeftMiddle(FDeep* deep, size_t index) {
 	assert(index < deep->size);
 	FView view = FTree_takeLeft(deep->middle, index);
 	assert(view.node->size != 1);
 	assert(index >= FTree_size(view.tree));
 	index -= FTree_size(view.tree);
 	size_t size;
 	if(index < (size = view.node->items[0]->size))
@@ -2770,74 +2532,72 @@
 	return FView_make(view.node->items[2], FDeep_makeS(
 		FDigit_incRef(deep->left), view.tree,
 		FDigit_make(view.node->items[0]->size + view.node->items[1]->size, 2,
 			FNode_incRef(view.node->items[0]),
 			FNode_incRef(view.node->items[1]), NULL, NULL)));
 }
 
-static FView FTree_takeLeft(FTree* tree, size_t index) {
+FView FTree_takeLeft(FTree* tree, size_t index) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: return FView_make(tree->single, FEmpty_make());
 		case FDeepT: {
 			size_t size;
 			if(index < (size = tree->deep->left->size))
 				return FDeep_takeLeftLeft(tree->deep, index);
 			index -= size;
 			if(index < (size = FTree_size(tree->deep->middle)))
 				return FDeep_takeLeftMiddle(tree->deep, index);
 			index -= size;
 			return FDeep_takeLeftRight(tree->deep, index);
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_takeLeft(PSequence* self, Py_ssize_t index) {
+PSequence* PSequence_takeLeft(PSequence* self, Py_ssize_t index) {
 	if(index <= 0) return PObj_IncRef(EMPTY_SEQUENCE);
 	if((size_t)index >= FTree_size(self->tree)) return PObj_IncRef(self);
 	FView view = FTree_takeLeft(self->tree, index);
 	return PSequence_make(view.tree);
 }
 
 // }}}
 
 // {{{ takeRight
 
-static FView FTree_takeRight(FTree* tree, size_t index);
-
-static FView FDeep_takeRightLeft(FDeep* deep, size_t index) {
+FView FDeep_takeRightLeft(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = deep->left->count; i-- > 0;)
 		if(index >= (size = deep->left->items[i]->size)) {
 			FNode_incRef(deep->left->items[i]);
 			index -= size; dsize += size;
 		} else return FView_make(
 			deep->left->items[i],
 			i == deep->left->count - 1
 				? FTree_pullLeft(deep->middle, deep->right)
 				: FDeep_make(deep->size - deep->left->size + dsize,
 					FDigit_makeN(dsize, deep->left->count - i - 1,
 						deep->left->items + i + 1),
 					FTree_incRef(deep->middle), FDigit_incRef(deep->right)));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FView FDeep_takeRightRight(FDeep* deep, size_t index) {
+FView FDeep_takeRightRight(FDeep* deep, size_t index) {
 	size_t size, dsize = 0;
 	for(int i = deep->right->count; i-- > 0;)
 		if(index >= (size = deep->right->items[i]->size)) {
 			FNode_incRef(deep->right->items[i]);
 			index -= size; dsize += size;
 		} else return FView_make(deep->right->items[i],
 			FTree_fromNodes(dsize, deep->right->count - i - 1,
 				deep->right->items + i + 1));
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static FView FDeep_takeRightMiddle(FDeep* deep, size_t index) {
+FView FDeep_takeRightMiddle(FDeep* deep, size_t index) {
 	assert(index < deep->size);
 	FView view = FTree_takeRight(deep->middle, index);
 	assert(view.node->size != 1);
 	assert(index >= FTree_size(view.tree));
 	index -= FTree_size(view.tree);
 	size_t size;
 	if(view.node->items[2] != NULL) {
@@ -2861,79 +2621,79 @@
 		FDigit_make(view.node->size - view.node->items[0]->size,
 			FNode_count(view.node) - 1,
 			FNode_incRef(view.node->items[1]),
 			FNode_incRefM(view.node->items[2]), NULL, NULL),
 		view.tree, FDigit_incRef(deep->right)));
 }
 
-static FView FTree_takeRight(FTree* tree, size_t index) {
+FView FTree_takeRight(FTree* tree, size_t index) {
 	assert(index < FTree_size(tree));
 	switch(tree->type) {
 		case FSingleT: return FView_make(tree->single, FEmpty_make());
 		case FDeepT: {
 			size_t size;
 			if(index < (size = tree->deep->right->size))
 				return FDeep_takeRightRight(tree->deep, index);
 			index -= size;
 			if(index < (size = FTree_size(tree->deep->middle)))
 				return FDeep_takeRightMiddle(tree->deep, index);
 			index -= size;
 			return FDeep_takeRightLeft(tree->deep, index);
-		} default: Py_UNREACHABLE();
-	}
+		} default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_takeRight(PSequence* self, Py_ssize_t index) {
+PSequence* PSequence_takeRight(PSequence* self, Py_ssize_t index) {
 	if(index <= 0) return PObj_IncRef(EMPTY_SEQUENCE);
 	if((size_t)index >= FTree_size(self->tree)) return PObj_IncRef(self);
 	FView view = FTree_takeRight(self->tree, index);
 	return PSequence_make(view.tree);
 }
 
 // }}}
 
 // {{{ repr
 
-static PyObject* PSequence_repr(PSequence* self) {
+PyObject* PSequence_repr(PSequence* self) {
 	PyObject* list = PSequence_toList(self);
 	if(list == NULL) return NULL;
 	PyObject* repr = PyObject_Repr(list);
 	Py_DECREF(list);
 	if(repr == NULL) return NULL;
 	PyObject* form = PyUnicode_FromFormat("%s%U%s", "psequence(", repr, ")");
 	Py_DECREF(repr);
 	return form;
 }
 
 // }}}
 
 // {{{ compare
 
-static PyObject* PObj_compare(PyObject* x, PyObject* y, int op) {
+PyObject* PObj_compare(PyObject* x, PyObject* y, int op) {
 	if(x == NULL) {
 		if(y == NULL) switch(op) {
 			case Py_EQ: case Py_GE: case Py_LE:
 				return PObj_IncRef(Py_True);
 			case Py_NE: case Py_GT: case Py_LT:
 				return PObj_IncRef(Py_False);
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		} else switch(op) {
 			case Py_NE: case Py_LT: case Py_LE:
 				return PObj_IncRef(Py_True);
 			case Py_EQ: case Py_GT: case Py_GE:
 				return PObj_IncRef(Py_False);
-			default: Py_UNREACHABLE();
+			default: assert(false); // LCOV_EXCL_LINE
 		}
 	}
 	if(y == NULL) switch(op) {
 		case Py_NE: case Py_GT: case Py_GE:
 			return PObj_IncRef(Py_True);
 		case Py_EQ: case Py_LT: case Py_LE:
 			return PObj_IncRef(Py_False);
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	int eq = PyObject_RichCompareBool(x, y, Py_EQ);
 	if(eq != 0) return NULL;
 	switch(op) {
 		case Py_EQ: return PObj_IncRef(Py_False);
 		case Py_NE: return PObj_IncRef(Py_True);
 	}
@@ -2941,39 +2701,39 @@
 	if(gt == -1) return NULL;
 	switch(op) {
 		case Py_GT: case Py_GE:
 			return PObj_IncRef(gt == 0 ? Py_False : Py_True);
 		case Py_LT: case Py_LE:
 			return PObj_IncRef(gt == 0 ? Py_True : Py_False);
 	}
-	Py_UNREACHABLE();
+	assert(false); // LCOV_EXCL_LINE
 }
 
-static PyObject* PIter_compare(PyObject* xs, PyObject* ys, int op) {
+PyObject* PIter_compare(PyObject* xs, PyObject* ys, int op) {
 	PyObject* x = PyIter_Next(xs);
 	if(x == NULL && PyErr_Occurred()) return NULL;
 	PyObject* y = PyIter_Next(ys);
 	if(y == NULL && PyErr_Occurred()) {
 		if(x != NULL) Py_DECREF(x);
 		return NULL;
 	}
 	PyObject* cmp = PObj_compare(x, y, op);
 	if(x != NULL) Py_DECREF(x);
 	if(y != NULL) Py_DECREF(y);
 	if(cmp != NULL || PyErr_Occurred()) return cmp;
 	return PIter_compare(xs, ys, op);
 }
 
-static PyObject* PSequence_compare(PyObject* xs, PyObject* ys, int op) {
+PyObject* PSequence_compare(PyObject* xs, PyObject* ys, int op) {
 	if(xs == ys) switch(op) {
 		case Py_EQ: case Py_LE: case Py_GE:
 			return PObj_IncRef(Py_True);
 		case Py_NE: case Py_LT: case Py_GT:
 			return PObj_IncRef(Py_False);
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	PyObject* xi = PyObject_GetIter(xs);
 	if(xi == NULL) return NULL;
 	PyObject* yi = PyObject_GetIter(ys);
 	if(yi == NULL) {
 		Py_DECREF(xi);
 		return NULL;
@@ -2999,73 +2759,73 @@
 #else
 #define _PyHASH_XXPRIME_1 ((Py_uhash_t)2654435761UL)
 #define _PyHASH_XXPRIME_2 ((Py_uhash_t)2246822519UL)
 #define _PyHASH_XXPRIME_5 ((Py_uhash_t)374761393UL)
 #define _PyHASH_XXROTATE(x) ((x << 13) | (x >> 19))
 #endif
 
-static Py_uhash_t FNode_hash(FNode* node, Py_uhash_t acc) {
+Py_uhash_t FNode_hash(FNode* node, Py_uhash_t acc) {
 	if(node->size == 1) {
 		Py_uhash_t lane = PyObject_Hash(node->value);
 		if (lane == (Py_uhash_t)-1) return -1;
 		acc += lane * _PyHASH_XXPRIME_2;
 		acc = _PyHASH_XXROTATE(acc);
 		acc *= _PyHASH_XXPRIME_1;
 		return acc;
 	}
 	if((acc = FNode_hash(node->items[0], acc)) == (Py_uhash_t)-1) return -1;
 	if((acc = FNode_hash(node->items[1], acc)) == (Py_uhash_t)-1) return -1;
 	if(node->items[2] == NULL) return acc;
 	return FNode_hash(node->items[2], acc);
 }
 
-static Py_uhash_t FDigit_hash(FDigit* digit, Py_uhash_t acc) {
+Py_uhash_t FDigit_hash(FDigit* digit, Py_uhash_t acc) {
 	for(int i = 0; i < digit->count; ++i)
 		if((acc = FNode_hash(digit->items[i], acc)) == (Py_uhash_t)-1) return -1;
 	return acc;
 }
 
-static Py_uhash_t FTree_hash(FTree* tree, Py_uhash_t acc) {
+Py_uhash_t FTree_hash(FTree* tree, Py_uhash_t acc) {
 	switch(tree->type) {
 		case FEmptyT: return acc;
 		case FSingleT: return FNode_hash(tree->single, acc);
 		case FDeepT: {
 			if((acc = FDigit_hash(tree->deep->left, acc)) == (Py_uhash_t)-1) return -1;
 			if((acc = FTree_hash(tree->deep->middle, acc)) == (Py_uhash_t)-1) return -1;
 			return FDigit_hash(tree->deep->right, acc);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static Py_hash_t PSequence_hash(PSequence* self) {
+Py_hash_t PSequence_hash(PSequence* self) {
 	Py_uhash_t acc = FTree_hash(self->tree, _PyHASH_XXPRIME_5);
 	if(acc == (Py_uhash_t)-1) return -1;
 	acc += FTree_ssize(self->tree) ^ (_PyHASH_XXPRIME_5 ^ 3527539UL);
 	if (acc == (Py_uhash_t)-1) return 1546275796;
 	return acc;
 }
 
 // }}}
 
 // {{{ reverse
 
-static FNode* FNode_reverse(FNode* node) {
+FNode* FNode_reverse(FNode* node) {
 	if(node->size == 1) return FNode_incRef(node);
 	if(node->items[2] == NULL)
 		return FNode_make(node->size,
 			FNode_reverse(node->items[1]),
 			FNode_reverse(node->items[0]), NULL);
 	return FNode_make(node->size,
 	 	FNode_reverse(node->items[2]),
 	 	FNode_reverse(node->items[1]),
 		FNode_reverse(node->items[0]));
 }
 
-static FDigit* FDigit_reverse(FDigit* digit) {
+FDigit* FDigit_reverse(FDigit* digit) {
 	switch(digit->count) {
 		case 1: return FDigit_make(digit->size, digit->count,
 			FNode_reverse(digit->items[0]), NULL, NULL, NULL);
 		case 2: return FDigit_make(digit->size, digit->count,
 			FNode_reverse(digit->items[1]),
 			FNode_reverse(digit->items[0]), NULL, NULL);
 		case 3: return FDigit_make(digit->size, digit->count,
@@ -3073,40 +2833,40 @@
 			FNode_reverse(digit->items[1]),
 			FNode_reverse(digit->items[0]), NULL);
 		case 4: return FDigit_make(digit->size, digit->count,
 			FNode_reverse(digit->items[3]),
 			FNode_reverse(digit->items[2]),
 			FNode_reverse(digit->items[1]),
 			FNode_reverse(digit->items[0]));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FTree* FTree_reverse(FTree* tree) {
+FTree* FTree_reverse(FTree* tree) {
 	switch(tree->type) {
 		case FEmptyT: return FEmpty_make();
 		case FSingleT: return FSingle_make(
 			FNode_reverse(tree->single));
 		case FDeepT: return FDeep_make(tree->deep->size,
 			FDigit_reverse(tree->deep->right),
 			FTree_reverse(tree->deep->middle),
 			FDigit_reverse(tree->deep->left));
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_reverse(PSequence* self) {
+PSequence* PSequence_reverse(PSequence* self) {
 	return PSequence_make(FTree_reverse(self->tree));
 }
 
 // }}}
 
 // {{{ getSlice
 
-static bool FNode_getSlice(FNode* node, FSlice* slice) {
+bool FNode_getSlice(FNode* node, FSlice* slice) {
 	if(node->size <= slice->modulo) {
 		slice->modulo -= node->size;
 		return false;
 	}
 	if(node->size == 1) {
 		assert(slice->modulo == 0);
 		slice->modulo = slice->step;
@@ -3118,44 +2878,44 @@
 	if(FNode_getSlice(node->items[1], slice))
 		return true;
 	if(node->items[2] == NULL)
 		return false;
 	return FNode_getSlice(node->items[2], slice);
 }
 
-static bool FDigit_getSlice(FDigit* digit, FSlice* slice) {
+bool FDigit_getSlice(FDigit* digit, FSlice* slice) {
 	if(digit->size <= slice->modulo) {
 		slice->modulo -= digit->size;
 		return false;
 	}
 	for(int i = 0; i < digit->count; ++i)
 		if(FNode_getSlice(digit->items[i], slice))
 			return true;
 	return false;
 }
 
-static bool FTree_getSlice(FTree* tree, FSlice* slice) {
+bool FTree_getSlice(FTree* tree, FSlice* slice) {
 	if(FTree_size(tree) <= slice->modulo) {
 		slice->modulo -= FTree_size(tree);
 		return false;
 	}
 	switch(tree->type) {
 		case FSingleT:
 			return FNode_getSlice(tree->single, slice);
 		case FDeepT:
 			if(FDigit_getSlice(tree->deep->left, slice))
 				return true;
 			if(FTree_getSlice(tree->deep->middle, slice))
 				return true;
 			return FDigit_getSlice(tree->deep->right, slice);
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_getSlice(PSequence* self, PyObject* slice) {
+PSequence* PSequence_getSlice(PSequence* self, PyObject* slice) {
 	Py_ssize_t start, stop, step;
 	if(PySlice_Unpack(slice, &start, &stop, &step)) return NULL;
 	assert(step != 0);
 	Py_ssize_t count = PySlice_AdjustIndices(
 		FTree_ssize(self->tree), &start, &stop, step);
 	if(count == 0)
 		return PObj_IncRef(EMPTY_SEQUENCE);
@@ -3172,15 +2932,15 @@
 		if(stop < FTree_ssize(self->tree))
 			tree = FTree_decRefRet(tree,
 				FTree_takeLeft(tree, stop).tree);
 		if(start > 0)
 			tree = FTree_decRefRet(tree,
 				FTree_takeRight(tree, stop - start).tree);
 	} else {
-		FNode** nodes = PyMem_Malloc(count * sizeof(PyObject*));
+		FNode** nodes = (FNode**)PyMem_Malloc(count * sizeof(PyObject*));
 		FSlice slice = {
 			.modulo = start,
 			.count = count,
 			.step = absstep - 1,
 			.output = nodes,
 		};
 		bool sliced UNUSED = FTree_getSlice(self->tree, &slice);
@@ -3189,15 +2949,15 @@
 		PyMem_Free(nodes);
 	}
 	if(step < 0)
 		tree = FTree_decRefRet(tree, FTree_reverse(tree));
 	return PSequence_make(tree);
 }
 
-static PyObject* PSequence_subscr(PSequence* self, PyObject* arg) {
+PyObject* PSequence_subscr(PSequence* self, PyObject* arg) {
 	if(PyIndex_Check(arg)) {
 		Py_ssize_t index = PyNumber_AsSsize_t(arg, PyExc_IndexError);
 		if(index == -1 && PyErr_Occurred()) return NULL;
 		return PSequence_getItemS(self, index);
 	}
 	if(PySlice_Check(arg))
 		return (PyObject*)PSequence_getSlice(self, arg);
@@ -3205,15 +2965,15 @@
 		"psequence indices must be integers or slices");
 }
 
 // }}}
 
 // {{{ deleteSlice
 
-static PSequence* PSequence_deleteSlice(
+PSequence* PSequence_deleteSlice(
 	PSequence* self,
 	PyObject* slice
 ) {
 	Py_ssize_t start, stop, step;
 	if(PySlice_Unpack(slice, &start, &stop, &step)) return NULL;
 	assert(step != 0);
 	Py_ssize_t count = PySlice_AdjustIndices(
@@ -3251,15 +3011,15 @@
 	acc = FTree_decRefRet(acc, FTree_decRefRet(splitL.left,
 		FTree_extend(splitL.left, acc)));
 	acc = FTree_decRefRet(acc, FTree_decRefRet(splitR.right,
 		FTree_extend(acc, splitR.right)));
 	return PSequence_make(acc);
 }
 
-static PSequence* PSequence_deleteSubscr(PSequence* self, PyObject* index) {
+PSequence* PSequence_deleteSubscr(PSequence* self, PyObject* index) {
 	if(PyIndex_Check(index)) {
 		Py_ssize_t idx = PyNumber_AsSsize_t(index, PyExc_IndexError);
 		if(idx == -1 && PyErr_Occurred()) return NULL;
 		return PSequence_deleteItemS(self, idx);
 	}
 	if(PySlice_Check(index))
 		return PSequence_deleteSlice(self, index);
@@ -3267,15 +3027,15 @@
 		"psequence indices must be integers or slices");
 }
 
 // }}}
 
 // {{{ setSlice
 
-static FNode* FNode_setSlice(FNode* node, FSlice* slice) {
+FNode* FNode_setSlice(FNode* node, FSlice* slice) {
 	assert(node != NULL);
 	if(slice->count == 0)
 		return FNode_incRef(node);
 	if(node->size <= slice->modulo) {
 		slice->modulo -= node->size;
 		return FNode_incRef(node);
 	}
@@ -3290,28 +3050,28 @@
 	nodes[0] = FNode_setSlice(node->items[0], slice);
 	nodes[1] = FNode_setSlice(node->items[1], slice);
 	if(node->items[2] != NULL)
 		nodes[2] = FNode_setSlice(node->items[2], slice);
 	return FNode_make(node->size, nodes[0], nodes[1], nodes[2]);
 }
 
-static FDigit* FDigit_setSlice(FDigit* digit, FSlice* slice) {
+FDigit* FDigit_setSlice(FDigit* digit, FSlice* slice) {
 	if(slice->count == 0)
 		return FDigit_incRef(digit);
 	if(digit->size <= slice->modulo) {
 		slice->modulo -= digit->size;
 		return FDigit_incRef(digit);
 	}
 	FNode* nodes[4] = { NULL, NULL, NULL, NULL };
 	for(int i = 0; i < digit->count; ++i)
 		nodes[i] = FNode_setSlice(digit->items[i], slice);
 	return FDigit_makeN(digit->size, digit->count, nodes);
 }
 
-static FTree* FTree_setSlice(FTree* tree, FSlice* slice) {
+FTree* FTree_setSlice(FTree* tree, FSlice* slice) {
 	if(slice->count == 0)
 		return FTree_incRef(tree);
 	if(FTree_size(tree) <= slice->modulo) {
 		slice->modulo -= FTree_size(tree);
 		return FTree_incRef(tree);
 	}
 	switch(tree->type) {
@@ -3319,19 +3079,19 @@
 			return FSingle_make(FNode_setSlice(tree->single, slice));
 		case FDeepT: {
 			FDigit* left = FDigit_setSlice(tree->deep->left, slice);
 			FTree* middle = FTree_setSlice(tree->deep->middle, slice);
 			FDigit* right = FDigit_setSlice(tree->deep->right, slice);
 			return FDeep_make(tree->deep->size, left, middle, right);
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PSequence* PSequence_setSlice(
+PSequence* PSequence_setSlice(
 	PSequence* self,
 	PyObject* slice,
 	PyObject* value
 ) {
 	Py_ssize_t start, stop, step;
 	if(PySlice_Unpack(slice, &start, &stop, &step)) return NULL;
 	assert(step != 0);
@@ -3360,15 +3120,15 @@
 			" extended slice of size %zd", size, count);
 	}
 	PyObject** items = PySequence_Fast_ITEMS(itemsfast);
 	Py_ssize_t absstep = step > 0 ? step : -step;
 	if(step < 0) {
 		Py_ssize_t tstart = start + (count - 1) * step;
 		stop = start + 1; start = tstart;
-		PyObject** buf = PyMem_MALLOC(count * sizeof(PyObject*));
+		PyObject** buf = (PyObject**)PyMem_MALLOC(count * sizeof(PyObject*));
 		for(Py_ssize_t i = 0, j = count - 1; i < count; ++i, --j)
 			buf[i] = items[j];
 		items = buf;
 	}
 	assert(0 < stop && stop <= FTree_ssize(self->tree));
 	assert(0 <= start && start < stop);
 	FSlice fslice = {
@@ -3379,15 +3139,15 @@
 	};
 	FTree* tree = FTree_setSlice(self->tree, &fslice);
 	Py_DECREF(itemsfast);
 	if(step < 0) PyMem_FREE(items);
 	return PSequence_make(tree);
 }
 
-static PSequence* PSequence_setSubscr(
+PSequence* PSequence_setSubscr(
 	PSequence* self,
 	PyObject* index,
 	PyObject* value
 ) {
 	if(PyIndex_Check(index)) {
 		Py_ssize_t idx = PyNumber_AsSsize_t(index, PyExc_IndexError);
 		if(idx == -1 && PyErr_Occurred()) return NULL;
@@ -3395,38 +3155,38 @@
 	}
 	if(PySlice_Check(index))
 		return PSequence_setSlice(self, index, value);
 	return (void*)PyErr_Format(PyExc_TypeError,
 		"psequence indices must be integers or slices");
 }
 
-static PSequence* PSequence_setSubscrN(PSequence* self, PyObject* args) {
+PSequence* PSequence_setSubscrN(PSequence* self, PyObject* args) {
 	PyObject* index; PyObject* value;
 	if(!PyArg_ParseTuple(args, "OO", &index, &value)) return NULL;
 	return PSequence_setSubscr(self, index, value);
 }
 
 // }}}
 
 // {{{ reduce
 
-static PyObject* PSEQUENCE_FUNCTION = NULL;
+PyObject* PSEQUENCE_FUNCTION = NULL;
 
-static PyObject* PSequence_reduce(PSequence* self) {
+PyObject* PSequence_reduce(PSequence* self) {
 	assert(PSEQUENCE_FUNCTION != NULL);
 	return Py_BuildValue("(O(N))", PSEQUENCE_FUNCTION, PSequence_toList(self));
 }
 
 // }}}
 
 // {{{ transform
 
-static PyObject* TRANSFORM_FUNCTION = NULL;
+PyObject* TRANSFORM_FUNCTION = NULL;
 
-static PSequence* PSequence_transform(PSequence* self, PyObject* args) {
+PSequence* PSequence_transform(PSequence* self, PyObject* args) {
 	if(TRANSFORM_FUNCTION == NULL) {
 		PyObject* module = PyImport_ImportModule("pyrsistent._transformations");
 		if(module == NULL) return NULL;
 		TRANSFORM_FUNCTION = PyObject_GetAttrString(module, "transform");
 		Py_DECREF(module);
 		if(TRANSFORM_FUNCTION == NULL) return NULL;
 	}
@@ -3434,15 +3194,15 @@
 		TRANSFORM_FUNCTION, self, args, NULL);
 }
 
 // }}}
 
 // {{{ sort
 
-static PSequence* PSequence_sort(
+PSequence* PSequence_sort(
 	PSequence*  self,
 	PyObject* args,
 	PyObject* kwargs
 ) {
 	PSequence* retval = NULL;
 	PyObject* list = PSequence_toList(self);
 	if(list == NULL) goto err0;
@@ -3457,64 +3217,60 @@
 	err0: return retval;
 }
 
 // }}}
 
 // {{{ PSequence
 
-static Py_ssize_t PSequence_length(PSequence* self) {
+Py_ssize_t PSequence_length(PSequence* self) {
 	return FTree_ssize(self->tree);
 }
 
-static PyObject* PSequence_refcount(PyObject* self, PyObject* args) {
+PyObject* PSequence_refcount(PyObject* self, PyObject* args) {
 	return Py_BuildValue("(lll)",
 		FRefs_get(FTreeR), FRefs_get(FDigitR), FRefs_get(FNodeR));
 }
 
-static PSequence* PSequence_fromItems(PyObject* self, PyObject* args) {
+PSequence* PSequence_fromItems(PyObject* self, PyObject* args) {
 	PyObject* arg = NULL;
 	if(!PyArg_ParseTuple(args, "|O", &arg)) return NULL;
 	if(arg == NULL) return PObj_IncRef(EMPTY_SEQUENCE);
 	return PSequence_fromIterable(arg);
 }
 
-static PSequenceIter* PSequence_iter(PSequence* self);
-static PSequenceIter* PSequence_reversed(PSequence* self);
-static PSequenceEvolver* PSequence_evolver(PSequence* self);
-
-static PySequenceMethods PSequence_asSequence = {
+PySequenceMethods PSequence_asSequence = {
 	.sq_length         = (lenfunc)PSequence_length,
 	.sq_concat         = (binaryfunc)PSequence_extendRight,
 	.sq_repeat         = (ssizeargfunc)PSequence_repeat,
 	.sq_item           = (ssizeargfunc)PSequence_getItem,
 	.sq_ass_item       = (ssizeobjargproc)NULL,
 	.sq_contains       = (objobjproc)PSequence_contains,
 	.sq_inplace_concat = (binaryfunc)NULL,
 	.sq_inplace_repeat = (ssizeargfunc)NULL,
 };
 
-static PyMappingMethods PSequence_asMapping = {
+PyMappingMethods PSequence_asMapping = {
 	.mp_length        = (lenfunc)PSequence_length,
 	.mp_subscript     = (binaryfunc)PSequence_subscr,
 	.mp_ass_subscript = (objobjargproc)NULL,
 };
 
 #define define_getter(name, func) \
 	{ #name, (getter)PSequence_##func, NULL, NULL, NULL }
-static PyGetSetDef PSequence_getSet[] = {
+PyGetSetDef PSequence_getSet[] = {
 	// { (const char*)name, (getter)get, (setter)set, (const char*)doc, (void*)closure }
 	define_getter(left, peekLeft),
 	define_getter(right, peekRight),
 	{NULL}
 };
 #undef define_getter
 
 #define define_method(name, func, flags) \
 	{ #name, (PyCFunction)PSequence_##func, METH_##flags, NULL }
-static PyMethodDef PSequence_methods[] = {
+PyMethodDef PSequence_methods[] = {
 	define_method(append,       appendRight,  O),
 	define_method(appendright,  appendRight,  O),
 	define_method(appendleft,   appendLeft,   O),
 	define_method(view,         view,         VARARGS),
 	define_method(viewright,    viewRight,    NOARGS),
 	define_method(viewleft,     viewLeft,     NOARGS),
 	define_method(splitat,      splitAt,      O),
@@ -3541,15 +3297,15 @@
 	define_method(_fromtree,    fromTuple,    O       | METH_STATIC),
 	define_method(_refcount,    refcount,     NOARGS  | METH_STATIC),
 	define_method(_fromitems,   fromItems,    VARARGS | METH_STATIC),
 	{NULL}
 };
 #undef define_method
 
-static PyTypeObject PSequenceType = {
+PyTypeObject PSequenceType = {
 	PyVarObject_HEAD_INIT(NULL, 0)
 	.tp_name              = (const char*)"pyrsistent_extras._psequence._c_ext.PSequence",
 	.tp_basicsize         = (Py_ssize_t)sizeof(PSequence),
 	// .tp_itemsize          = (Py_ssize_t)0,
 	.tp_dealloc           = (destructor)PSequence_dealloc,
 	// .tp_vectorcall_offset = (Py_ssize_t)0,
 	// .tp_getattr           = (getattrfunc)NULL,
@@ -3597,45 +3353,45 @@
 	// .tp_vectorcall        = (vectorcallfunc)NULL,
 };
 
 // }}}
 
 // {{{ iter next
 
-static FIter* FIter_pushStack(
+FIter* FIter_pushStack(
 	FIter* iter,
 	FIterT type,
 	int index,
 	void* item
 ) {
 	return FIter_make(type, index, item, iter);
 }
 
-static FIter* FIter_swapStack(
+FIter* FIter_swapStack(
 	FIter* iter,
 	FIterT type,
 	int index,
 	void* item
 ) {
 	FIter_decRef(iter);
 	iter->type = type;
 	iter->index = index;
 	iter->tree = item;
 	FIter_incRef(iter);
 	return iter;
 }
 
-static FIter* FIter_popStack(FIter* iter) {
+FIter* FIter_popStack(FIter* iter) {
 	assert(iter != NULL);
 	FIter* next = iter->next;
 	FIter_dealloc(iter, false);
 	return next;
 }
 
-static FIter* FIter_nextStack(FIter* iter) {
+FIter* FIter_nextStack(FIter* iter) {
 	if(iter == NULL) return iter;
 	switch(iter->type) {
 		case FTreeI:
 			switch(iter->tree->type) {
 				case FEmptyT:
 					assert(iter->index == 0);
 					return FIter_nextStack(FIter_popStack(iter));
@@ -3647,17 +3403,17 @@
 					switch(iter->index++) {
 						case 0: return FIter_nextStack(FIter_pushStack(
 							iter, FDigitI, 0, iter->tree->deep->left));
 						case 1: return FIter_nextStack(FIter_pushStack(
 							iter, FTreeI, 0, iter->tree->deep->middle));
 						case 2: return FIter_nextStack(FIter_swapStack(
 							iter, FDigitI, 0, iter->tree->deep->right));
-						default: Py_UNREACHABLE();
+						default: assert(false); // LCOV_EXCL_LINE
 					}
-				default: Py_UNREACHABLE();
+				default: assert(false); // LCOV_EXCL_LINE
 			};
 		case FDigitI: {
 			assert(0 <= iter->index && iter->index <= 4);
 			FNode* node = iter->digit->items[iter->index];
 			if(++iter->index == iter->digit->count)
 				return FIter_nextStack(FIter_swapStack(iter, FNodeI, 0, node));
 			return FIter_nextStack(FIter_pushStack(iter, FNodeI, 0, node));
@@ -3670,19 +3426,19 @@
 			assert(0 <= iter->index &&
 				iter->index <= FNode_count(iter->node));
 			FNode* node = iter->node->items[iter->index];
 			if(++iter->index == FNode_count(iter->node))
 				return FIter_nextStack(FIter_swapStack(iter, FNodeI, 0, node));
 			return FIter_nextStack(FIter_pushStack(iter, FNodeI, 0, node));
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static FIter* FIter_prevStack(FIter* iter) {
+FIter* FIter_prevStack(FIter* iter) {
 	if(iter == NULL) return iter;
 	switch(iter->type) {
 		case FTreeI:
 			switch(iter->tree->type) {
 				case FEmptyT:
 					assert(iter->index == 0);
 					return FIter_prevStack(FIter_popStack(iter));
@@ -3704,25 +3460,25 @@
 							switch(tree->type) {
 								case FEmptyT: return FIter_prevStack(FIter_pushStack(
 									iter, FTreeI, 0, tree));
 								case FSingleT: return FIter_prevStack(FIter_pushStack(
 									iter, FTreeI, 1, tree));
 								case FDeepT: return FIter_prevStack(FIter_pushStack(
 									iter, FTreeI, 3, tree));
-								default: Py_UNREACHABLE();
+								default: assert(false); // LCOV_EXCL_LINE
 							}
 						}
 						case 3: {
 							FDigit* digit = iter->tree->deep->right;
 							return FIter_prevStack(FIter_pushStack(
 								iter, FDigitI, digit->count, digit));
 						}
-						default: Py_UNREACHABLE();
+						default: assert(false); // LCOV_EXCL_LINE
 					}
-				default: Py_UNREACHABLE();
+				default: assert(false); // LCOV_EXCL_LINE
 			};
 		case FDigitI: {
 			assert(1 <= iter->index && iter->index <= 4);
 			FNode* node = iter->digit->items[--iter->index];
 			if(iter->index == 0)
 				return FIter_prevStack(FIter_swapStack(
 					iter, FNodeI, FNode_count(node), node));
@@ -3739,19 +3495,19 @@
 			FNode* node = iter->node->items[--iter->index];
 			if(iter->index == 0)
 				return FIter_prevStack(FIter_swapStack(
 					iter, FNodeI, FNode_count(node), node));
 			return FIter_prevStack(FIter_pushStack(
 				iter, FNodeI, FNode_count(node), node));
 		}
-		default: Py_UNREACHABLE();
-	}
+		default: assert(false); // LCOV_EXCL_LINE
+	} // LCOV_EXCL_LINE
 }
 
-static PyObject* PSequenceIter_next(PSequenceIter* self) {
+PyObject* PSequenceIter_next(PSequenceIter* self) {
 	if(self->reverse)
 		self->stack = FIter_prevStack(self->stack);
 	else
 		self->stack = FIter_nextStack(self->stack);
 	if(self->stack == NULL) {
 		if(self->reverse)
 			assert(self->index == 0);
@@ -3772,55 +3528,55 @@
 	return value;
 }
 
 // }}}
 
 // {{{ PSequenceIter
 
-static PSequenceIter* PSequence_iter(PSequence* self) {
+PSequenceIter* PSequence_iter(PSequence* self) {
 	return PSequenceIter_make(
 		0, false, PObj_IncRef(self),
 		FIter_make(FTreeI, 0, self->tree, NULL));
 }
 
-static PSequenceIter* PSequence_reversed(PSequence* self) {
+PSequenceIter* PSequence_reversed(PSequence* self) {
 	int index;
 	switch(self->tree->type) {
 		case FEmptyT: index = 0; break;
 		case FSingleT: index = 1; break;
 		case FDeepT: index = 3; break;
-		default: Py_UNREACHABLE();
+		default: assert(false); // LCOV_EXCL_LINE
 	}
 	return PSequenceIter_make(
 		FTree_size(self->tree), true, PObj_IncRef(self),
 		FIter_make(FTreeI, index, self->tree, NULL));
 }
 
-static PyObject* PSequenceIter_lenHint(PSequenceIter* self) {
+PyObject* PSequenceIter_lenHint(PSequenceIter* self) {
 	return PyLong_FromSsize_t(self->reverse ? self->index
 		: FTree_ssize(self->seq->tree) - self->index);
 }
 
-static int PSequenceIter_traverse(
+int PSequenceIter_traverse(
 	PSequenceIter *self,
 	visitproc visit,
 	void* arg
 ) {
 	return PSequence_traverse(self->seq, visit, arg);
 }
 
 #define define_method(name, method, flags) \
 	{ #name, (PyCFunction)PSequenceIter_##method, METH_##flags, NULL }
-static PyMethodDef PSequenceIter_methods[] = {
+PyMethodDef PSequenceIter_methods[] = {
 	define_method(__length_hint__, lenHint, NOARGS),
 	{NULL}
 };
 #undef define_method
 
-static PyTypeObject PSequenceIterType = {
+PyTypeObject PSequenceIterType = {
 	PyVarObject_HEAD_INIT(NULL, 0)
 	.tp_name              = (const char*)"pyrsistent_extras._psequence._c_ext.Iterator",
 	.tp_basicsize         = (Py_ssize_t)sizeof(PSequenceIter),
 	// .tp_itemsize          = (Py_ssize_t)0,
 	.tp_dealloc           = (destructor)PSequenceIter_dealloc,
 	// .tp_vectorcall_offset = (Py_ssize_t)0,
 	// .tp_getattr           = (getattrfunc)NULL,
@@ -3869,53 +3625,53 @@
 };
 
 // }}}
 
 // {{{ evolver inherit
 
 #define inherit_query0(name, rettype) \
-	static rettype PSequenceEvolver_##name \
+	rettype PSequenceEvolver_##name \
 	(PSequenceEvolver* self) \
 	{ return PSequence_##name(self->seq); }
 #define inherit_query1(name, rettype, type1) \
-	static rettype PSequenceEvolver_##name \
+	rettype PSequenceEvolver_##name \
 	(PSequenceEvolver* self, type1 arg1) \
 	{ return PSequence_##name(self->seq, arg1); }
 #define inherit_query2(name, rettype, type1, type2) \
-	static rettype PSequenceEvolver_##name \
+	rettype PSequenceEvolver_##name \
 	(PSequenceEvolver* self, type1 arg1, type2 arg2) \
 	{ return PSequence_##name(self->seq, arg1, arg2); }
 
 #define inherit_method0(name) \
-	static PSequenceEvolver* PSequenceEvolver_##name \
+	PSequenceEvolver* PSequenceEvolver_##name \
 	(PSequenceEvolver* self) \
 	{ PSequence* seq = PSequence_##name(self->seq); \
 		if(seq == NULL) return NULL; \
 		Py_DECREF(self->seq); self->seq = seq; return PObj_IncRef(self); }
 #define inherit_method1(name, type1) \
-	static PSequenceEvolver* PSequenceEvolver_##name \
+	PSequenceEvolver* PSequenceEvolver_##name \
 	(PSequenceEvolver* self, type1 arg1) \
 	{ PSequence* seq = PSequence_##name(self->seq, arg1); \
 		if(seq == NULL) return NULL; \
 		Py_DECREF(self->seq); self->seq = seq; return PObj_IncRef(self); }
 #define inherit_method2(name, type1, type2) \
-	static PSequenceEvolver* PSequenceEvolver_##name \
+	PSequenceEvolver* PSequenceEvolver_##name \
 	(PSequenceEvolver* self, type1 arg1, type2 arg2) \
 	{ PSequence* seq = PSequence_##name(self->seq, arg1, arg2); \
 		if(seq == NULL) return NULL; \
 		Py_DECREF(self->seq); self->seq = seq; return PObj_IncRef(self); }
 #define inherit_methodN(name) \
-	static PSequenceEvolver* PSequenceEvolver_##name \
+	PSequenceEvolver* PSequenceEvolver_##name \
 	(PSequenceEvolver* self, PyObject* args) \
 	{ PSequence* seq = PSequence_##name(self->seq, args); \
 		if(seq == NULL) return NULL; \
 		Py_DECREF(self->seq); self->seq = seq; return PObj_IncRef(self); }
 
 #define inherit_new1(name, type1) \
-	static PSequenceEvolver* PSequenceEvolver_##name##New \
+	PSequenceEvolver* PSequenceEvolver_##name##New \
 	(PSequenceEvolver* self, type1 arg1) \
 	{ PSequence* seq = PSequence_##name(self->seq, arg1); \
 		if(seq == NULL) return NULL; \
 		return PSequenceEvolver_make(seq); }
 
 inherit_query0(length, Py_ssize_t)
 inherit_method1(repeat, Py_ssize_t)
@@ -3964,46 +3720,47 @@
 inherit_methodN(transform)
 
 #undef inherit_query0
 #undef inherit_query1
 #undef inherit_query2
 #undef inherit_method0
 #undef inherit_method1
+#undef inherit_method2
 #undef inherit_methodN
 #undef inherit_new1
 
 // }}}
 
 // {{{ pop
 
-static PyObject* PSequenceEvolver_popLeft(PSequenceEvolver* self) {
+PyObject* PSequenceEvolver_popLeft(PSequenceEvolver* self) {
 	if(FTree_empty(self->seq->tree))
 		return (void*)PyErr_Format(PyExc_IndexError,
 			"pop from empty sequence");
 	FView view = FTree_viewLeft(self->seq->tree);
 	assert(view.node->size == 1);
 	PyObject* value = PObj_IncRef(view.node->value);
 	Py_DECREF(self->seq);
 	self->seq = PSequence_make(view.tree);
 	return value;
 }
 
-static PyObject* PSequenceEvolver_popRight(PSequenceEvolver* self) {
+PyObject* PSequenceEvolver_popRight(PSequenceEvolver* self) {
 	if(FTree_empty(self->seq->tree))
 		return (void*)PyErr_Format(PyExc_IndexError,
 			"pop from empty sequence");
 	FView view = FTree_viewRight(self->seq->tree);
 	assert(view.node->size == 1);
 	PyObject* value = PObj_IncRef(view.node->value);
 	Py_DECREF(self->seq);
 	self->seq = PSequence_make(view.tree);
 	return value;
 }
 
-static PyObject* PSequenceEvolver_pop(PSequenceEvolver* self, PyObject* args) {
+PyObject* PSequenceEvolver_pop(PSequenceEvolver* self, PyObject* args) {
 	PyObject* arg = NULL;
 	if(!PyArg_ParseTuple(args, "|O", &arg)) return NULL;
 	if(arg == NULL) return PSequenceEvolver_popRight(self);
 	PyObject* value = PSequenceEvolver_subscr(self, arg);
 	if(value == NULL) return NULL;
 	PSequenceEvolver* del = PSequenceEvolver_deleteSubscr(self, arg);
 	if(del == NULL) { Py_DECREF(value); return NULL; }
@@ -4011,45 +3768,45 @@
 	return value;
 }
 
 // }}}
 
 // {{{ PSequenceEvolver
 
-static PSequenceEvolver* PSequence_evolver(PSequence* self) {
+PSequenceEvolver* PSequence_evolver(PSequence* self) {
 	return PSequenceEvolver_make(PObj_IncRef(self));
 }
 
-static PyObject* PSequenceEvolver_repr(PSequenceEvolver* self) {
+PyObject* PSequenceEvolver_repr(PSequenceEvolver* self) {
 	PyObject* list = PSequence_toList(self->seq);
 	if(list == NULL) return NULL;
 	PyObject* repr = PyObject_Repr(list);
 	Py_DECREF(list);
 	if(repr == NULL) return NULL;
 	PyObject* form = PyUnicode_FromFormat("%s%U%s",
 		"psequence(", repr, ").evolver()");
 	Py_DECREF(repr);
 	return form;
 }
 
-static PSequence* PSequenceEvolver_persistent(PSequenceEvolver* self) {
+PSequence* PSequenceEvolver_persistent(PSequenceEvolver* self) {
 	return PObj_IncRef(self->seq);
 }
 
-static PSequenceEvolver* PSequenceEvolver_copy(PSequenceEvolver* self) {
+PSequenceEvolver* PSequenceEvolver_copy(PSequenceEvolver* self) {
 	return PSequenceEvolver_make(PObj_IncRef(self->seq));
 }
 
-static PSequenceEvolver* PSequenceEvolver_clear(PSequenceEvolver* self) {
+PSequenceEvolver* PSequenceEvolver_clear(PSequenceEvolver* self) {
 	Py_DECREF(self->seq);
 	self->seq = PObj_IncRef(EMPTY_SEQUENCE);
 	return PObj_IncRef(Py_None);
 }
 
-static int PSequenceEvolver_assItem(
+int PSequenceEvolver_assItem(
 	PSequenceEvolver* self,
 	Py_ssize_t index,
 	PyObject* value
 ) {
 	PSequence* seq;
 	if(value == NULL)
 		seq = PSequence_deleteItem(self->seq, index);
@@ -4057,15 +3814,15 @@
 		seq = PSequence_setItem(self->seq, index, value);
 	if(seq == NULL) return -1;
 	Py_DECREF(self->seq);
 	self->seq = seq;
 	return 0;
 }
 
-static int PSequenceEvolver_assSubscr(
+int PSequenceEvolver_assSubscr(
 	PSequenceEvolver* self,
 	PyObject* index,
 	PyObject* value
 ) {
 	PSequence* seq;
 	if(value == NULL)
 		seq = PSequence_deleteSubscr(self->seq, index);
@@ -4075,25 +3832,25 @@
 	Py_DECREF(self->seq);
 	self->seq = seq;
 	return 0;
 }
 
 #define define_getter(name, func) \
 	{ #name, (getter)PSequenceEvolver_##func, NULL, NULL, NULL }
-static PyGetSetDef PSequenceEvolver_getSet[] = {
+PyGetSetDef PSequenceEvolver_getSet[] = {
 	// { (const char*)name, (getter)get, (setter)set, (const char*)doc, (void*)closure }
 	define_getter(left, peekLeft),
 	define_getter(right, peekRight),
 	{NULL}
 };
 #undef define_getter
 
 #define define_method(name, method, flags) \
 	{ #name, (PyCFunction)PSequenceEvolver_##method, METH_##flags, NULL }
-static PyMethodDef PSequenceEvolver_methods[] = {
+PyMethodDef PSequenceEvolver_methods[] = {
 	define_method(append,       appendRight,  O),
 	define_method(appendright,  appendRight,  O),
 	define_method(appendleft,   appendLeft,   O),
 	define_method(view,         view,         VARARGS),
 	define_method(viewright,    viewRight,    NOARGS),
 	define_method(viewleft,     viewLeft,     NOARGS),
 	define_method(pop,          pop,          VARARGS),
@@ -4122,32 +3879,32 @@
 	define_method(copy,         copy,         NOARGS),
 	define_method(clear,        clear,        NOARGS),
 	define_method(sort,         sort,         VARARGS | METH_KEYWORDS),
 	{NULL}
 };
 #undef define_method
 
-static PySequenceMethods PSequenceEvolver_asSequence = {
+PySequenceMethods PSequenceEvolver_asSequence = {
 	.sq_length         = (lenfunc)PSequenceEvolver_length,
 	.sq_concat         = (binaryfunc)PSequenceEvolver_extendRightNew,
 	.sq_repeat         = (ssizeargfunc)PSequenceEvolver_repeatNew,
 	.sq_item           = (ssizeargfunc)PSequenceEvolver_getItem,
 	.sq_ass_item       = (ssizeobjargproc)PSequenceEvolver_assItem,
 	.sq_contains       = (objobjproc)PSequenceEvolver_contains,
 	.sq_inplace_concat = (binaryfunc)PSequenceEvolver_extendRight,
 	.sq_inplace_repeat = (ssizeargfunc)PSequenceEvolver_repeat,
 };
 
-static PyMappingMethods PSequenceEvolver_asMapping = {
+PyMappingMethods PSequenceEvolver_asMapping = {
 	.mp_length        = (lenfunc)PSequenceEvolver_length,
 	.mp_subscript     = (binaryfunc)PSequenceEvolver_subscr,
 	.mp_ass_subscript = (objobjargproc)PSequenceEvolver_assSubscr,
 };
 
-static PyTypeObject PSequenceEvolverType = {
+PyTypeObject PSequenceEvolverType = {
 	PyVarObject_HEAD_INIT(NULL, 0)
 	.tp_name              = (const char*)"pyrsistent_extras._psequence._c_ext.Iterator",
 	.tp_basicsize         = (Py_ssize_t)sizeof(PSequenceEvolver),
 	// .tp_itemsize          = (Py_ssize_t)0,
 	.tp_dealloc           = (destructor)PSequenceEvolver_dealloc,
 	// .tp_vectorcall_offset = (Py_ssize_t)0,
 	// .tp_getattr           = (getattrfunc)NULL,
@@ -4195,15 +3952,15 @@
 	// .tp_vectorcall        = (vectorcallfunc)NULL,
 };
 
 // }}}
 
 // {{{ module def
 
-static struct PyModuleDef moduleDef = {
+struct PyModuleDef moduleDef = {
 	PyModuleDef_HEAD_INIT,
 	.m_name     = (const char*)"pyrsistent_extras._psequence._c_ext",
 	.m_doc      = (const char*)"persistent sequence c implementation",
 	.m_size     = (Py_ssize_t)-1,
 	// .m_methods  = (PyMethodDef*)NULL,
 	// .m_slots    = (struct PyModuleDef_Slot*)NULL,
 	// .m_traverse = (traverseproc)NULL,
@@ -4230,18 +3987,18 @@
 
 bool pyrsistent_psequence_inheritDocs() {
 	bool okay = false;
 
 	PyObject* module = PyImport_ImportModule("pyrsistent_extras._psequence._base");
 	if(module == NULL) goto err0;
 
-	PyObject* seqbase = PyObject_GetAttrString(module, "PSequenceBase");
+	PyObject* seqbase = PyObject_GetAttrString(module, "PSequence");
 	if(seqbase == NULL) goto err1;
 	if(PSequenceType.tp_doc == NULL)
-		PSequenceType.tp_doc = PObj_getDoc("PSequenceBase", module);
+		PSequenceType.tp_doc = PObj_getDoc("PSequence", module);
 	if(PSequenceType.tp_doc == NULL) goto err1;
 
 	for(struct PyMethodDef* methdef = PSequenceType.tp_methods;
 			methdef->ml_name != NULL; ++methdef) {
 		if(methdef->ml_doc != NULL || methdef->ml_name[0] == '_') continue;
 		methdef->ml_doc = PObj_getDoc(methdef->ml_name, seqbase);
 		if(methdef->ml_doc == NULL) goto err2;
@@ -4250,18 +4007,18 @@
 	for(struct PyGetSetDef* methdef = PSequenceType.tp_getset;
 			methdef->name != NULL; ++methdef) {
 		if(methdef->doc != NULL || methdef->name[0] == '_') continue;
 		methdef->doc = PObj_getDoc(methdef->name, seqbase);
 		if(methdef->doc == NULL) goto err2;
 	}
 
-	PyObject* evobase = PyObject_GetAttrString(module, "PSequenceEvolverBase");
+	PyObject* evobase = PyObject_GetAttrString(module, "PSequenceEvolver");
 	if(evobase == NULL) goto err2;
 	if(PSequenceType.tp_doc == NULL)
-		PSequenceType.tp_doc = PObj_getDoc("PSequenceEvolverBase", module);
+		PSequenceType.tp_doc = PObj_getDoc("PSequenceEvolver", module);
 	if(PSequenceType.tp_doc == NULL) goto err1;
 
 	for(struct PyMethodDef* methdef = PSequenceEvolverType.tp_methods;
 			methdef->ml_name != NULL; ++methdef) {
 		if(methdef->ml_doc != NULL || methdef->ml_name[0] == '_') continue;
 		methdef->ml_doc = PObj_getDoc(methdef->ml_name, evobase);
 		if(methdef->ml_doc == NULL) goto err3;
```

### Comparing `pyrsistent-extras-0.1.0/pyrsistent_extras/_util.py` & `pyrsistent-extras-0.1.1/src/pyrsistent_extras/_utility.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from abc import abstractmethod
-from typing import Any, Iterator, TypeVar, Optional, Union, Tuple, Callable
+from typing import Any, Iterator, TypeVar, Optional, Union, Tuple, Callable, \
+	MappingView, KeysView, ValuesView, ItemsView, Generic, cast
 from typing_extensions import Protocol
 
 import builtins
 import platform
 import os
 
+NOTHING = cast(Any, object())
+
 class Comparable(Protocol):
 	@abstractmethod
 	def __lt__(self, other: Any) -> bool: ...
 	@abstractmethod
 	def __eq__(self, other: Any) -> bool: ...
 
 K = TypeVar('K', bound=Comparable)
+V = TypeVar('V')
 
 def compare_single(x:K, y:K, equality:bool) -> int:
 	if x == y: return 0
 	if equality or x < y: return -1
 	return 1
 
 def compare_next(xs:Iterator[Any], ys:Iterator[Any]) -> Union[int,Tuple[Any,Any]]:
@@ -36,17 +40,18 @@
 	return x, y
 
 def compare_iter(xs:Any, ys:Any, equality:bool) -> int:
 	if equality:
 		if xs is ys: return 0
 		try:
 			xl, yl = len(xs), len(ys)
-			if xl != yl: return 1
 		except TypeError:
 			pass
+		else:
+			if xl != yl: return 1
 	try:
 		xs, ys = iter(xs), iter(ys)
 	except TypeError:
 		return NotImplemented
 	while True:
 		n = compare_next(xs, ys)
 		if isinstance(n, int): return n
@@ -57,13 +62,26 @@
 	idx = index
 	if idx < 0:
 		idx += length
 	if not (0 <= idx < length):
 		raise IndexError('index out of range: ' + str(index))
 	return idx
 
+def trace(*args, **kwargs):
+	print(*args, **kwargs)
+	return args[-1]
+
 sphinx_build: bool = getattr(builtins, '__sphinx_build__', False)
 
 try_c_ext: bool = not sphinx_build \
-	and platform.python_implementation() == 'CPython' \
 	and not os.environ.get('PYRSISTENT_NO_C_EXTENSION')
 
+def keys_from_items(self):
+	for k, v in self._items():
+		yield k
+
+def values_from_items(self):
+	for k, v in self._items():
+		yield v
+
+def items_from_items(self):
+	return self._items()
```

