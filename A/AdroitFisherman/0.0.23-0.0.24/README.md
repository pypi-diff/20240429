# Comparing `tmp/AdroitFisherman-0.0.23.tar.gz` & `tmp/AdroitFisherman-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.23.tar", last modified: Thu Apr 25 11:26:51 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.24.tar", last modified: Mon Apr 29 14:12:20 2024, max compression
```

## Comparing `AdroitFisherman-0.0.23.tar` & `AdroitFisherman-0.0.24.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 11:26:51.169818 AdroitFisherman-0.0.23/
-drwxrwxrwx   0        0        0        0 2024-04-25 11:26:51.160843 AdroitFisherman-0.0.23/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-04-25 11:26:51.168820 AdroitFisherman-0.0.23/AdroitFisherman/SequentialList/
--rw-rw-rw-   0        0        0      695 2024-04-25 11:15:25.000000 AdroitFisherman-0.0.23/AdroitFisherman/SequentialList/ListObject.py
--rw-rw-rw-   0        0        0       24 2024-04-25 07:29:17.000000 AdroitFisherman-0.0.23/AdroitFisherman/SequentialList/__init__.py
--rw-rw-rw-   0        0        0       28 2024-04-25 09:21:48.000000 AdroitFisherman-0.0.23/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 11:26:51.168820 AdroitFisherman-0.0.23/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      710 2024-04-25 10:46:39.000000 AdroitFisherman-0.0.23/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5224 2024-04-25 11:26:39.000000 AdroitFisherman-0.0.23/AdroitFisherman/includes/SeqList.h
-drwxrwxrwx   0        0        0        0 2024-04-25 11:26:51.166825 AdroitFisherman-0.0.23/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     3049 2024-04-25 11:26:51.000000 AdroitFisherman-0.0.23/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-04-25 11:26:51.000000 AdroitFisherman-0.0.23/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 11:26:51.000000 AdroitFisherman-0.0.23/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 11:26:51.000000 AdroitFisherman-0.0.23/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.23/MANIFEST.in
--rw-rw-rw-   0        0        0     3049 2024-04-25 11:26:51.169818 AdroitFisherman-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.23/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 11:26:51.170815 AdroitFisherman-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-04-25 11:09:16.000000 AdroitFisherman-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.817307 AdroitFisherman-0.0.24/
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.795366 AdroitFisherman-0.0.24/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.812321 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0      701 2024-04-29 14:10:00.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0      843 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.813321 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0      161 2024-04-29 13:36:19.000000 AdroitFisherman-0.0.24/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.24/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.814317 AdroitFisherman-0.0.24/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.24/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.816311 AdroitFisherman-0.0.24/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5163 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8070 2024-04-29 04:10:03.000000 AdroitFisherman-0.0.24/AdroitFisherman/includes/SingleLinkedList.h
+drwxrwxrwx   0        0        0        0 2024-04-29 14:12:20.807336 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     3089 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 14:12:20.000000 AdroitFisherman-0.0.24/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     3089 2024-04-29 14:12:20.817307 AdroitFisherman-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.24/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 14:12:20.818306 AdroitFisherman-0.0.24/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-04-29 14:12:17.000000 AdroitFisherman-0.0.24/setup.py
```

### Comparing `AdroitFisherman-0.0.23/AdroitFisherman/SequentialList/ListObject.py` & `AdroitFisherman-0.0.24/AdroitFisherman/Utilities/SequentialList.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from AdroitFisherman.Utilities import SeqList
+from AdroitFisherman.SequentialList import SeqList
 
 
-class listobject:
+class ListObject:
     def __init__(self, size):
-        self.__list =SeqList()
+        self.__list = SeqList()
         self.__list.init_list(size)
 
     def destroy(self):
         self.__list.destroy_list()
 
     def clear_list(self):
         self.__list.clear_list()
```

### Comparing `AdroitFisherman-0.0.23/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #define PY_SIZE_T_CLEAN
 #include <python.h>
 #include <structmember.h>
 #include "SeqList.h"
 static PyModuleDef module = {
     PyModuleDef_HEAD_INIT,
-    .m_name="Utilities",
+    .m_name="SequentialList",
     .m_size = -1
 };
-PyMODINIT_FUNC PyInit_Utilities()
+PyMODINIT_FUNC PyInit_SequentialList()
 {
     PyObject* m;
     if (PyType_Ready(&SeqListObject)<0)
     {
         return NULL;
     }
     m = PyModule_Create(&module);
```

### Comparing `AdroitFisherman-0.0.23/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.24/AdroitFisherman/includes/SeqList.h`

 * *Files 4% similar despite different names*

```diff
@@ -38,24 +38,24 @@
 }
 static PyMemberDef SeqList_members[] = {
     {"elem",T_OBJECT,offsetof(SeqList,elem),0,""},
     {"length",T_INT,offsetof(SeqList,length),0,""},
     {"size",T_INT,offsetof(SeqList,size),0,""},
     {NULL}
 };
-static PyObject* InitList(SeqList* self,PyObject* args,PyObject* kwds)
+static PyObject* InitList(SeqList* self, PyObject* args, PyObject* kwds)
 {
     int size;
-    if (PyArg_ParseTuple(args,"i",&size) < 0)
+    if (PyArg_ParseTuple(args, "i", &size) < 0)
     {
         Py_RETURN_FALSE;
     }
     else
     {
-        self->elem = (ElemType*)PyMem_Calloc(size,sizeof(ElemType));
+        self->elem = (ElemType*)PyMem_Calloc(size, sizeof(ElemType));
         if (self->elem == NULL)
         {
             Py_RETURN_FALSE;
         }
         else
         {
             self->size = size;
@@ -81,71 +81,74 @@
         self->elem[i] = NULL;
     }
     self->length = 0;
     Py_RETURN_TRUE;
 }
 static PyObject* ListEmpty(SeqList* self, PyObject* args)
 {
-    if (self->length==0)
+    if (self->length == 0)
     {
         Py_RETURN_TRUE;
     }
     else
     {
         Py_RETURN_FALSE;
     }
 }
 static PyObject* ListLength(SeqList* self, PyObject* args)
 {
-    PyObject* obj = Py_BuildValue("i",self->length);
+    PyObject* obj = Py_BuildValue("i", self->length);
     Py_INCREF(obj);
     return obj;
 }
 static PyObject* GetElem(SeqList* self, PyObject* args)
 {
     int index;
+    PyObject* result;
     if (PyArg_ParseTuple(args, "i", &index) < 0)
     {
         PyErr_SetString(PyExc_Exception, "Args parsed failure!");
         Py_RETURN_NONE;
     }
     else
     {
         if (index<0 || index>self->length)
         {
             Py_RETURN_NONE;
         }
         else
         {
-            Py_INCREF(self->elem[index]);
-            return self->elem[index];
+            result = self->elem[index];
+            Py_XINCREF(result);
+            return result;
         }
     }
 }
 static PyObject* ListInsert(SeqList* self, PyObject* args)
 {
     int index;
     PyObject* elem;
-    if (PyArg_ParseTuple(args,"iO",&index,&elem)<0)
+    if (PyArg_ParseTuple(args, "iO", &index, &elem) < 0)
     {
-        PyErr_SetString(PyExc_Exception,"Args parsed failure!");
+        PyErr_SetString(PyExc_Exception, "Args parsed failure!");
         Py_RETURN_FALSE;
     }
     else
     {
-        if (index<0||index>self->length)
+        if (index<0 || index>self->length)
         {
             Py_RETURN_FALSE;
         }
         else
         {
             for (int i = self->length; i >= index; i--)
             {
                 self->elem[i + 1] = self->elem[i];
             }
+            Py_XINCREF(elem);
             self->elem[index] = elem;
             self->length++;
             Py_RETURN_TRUE;
         }
     }
 }
 static PyObject* ListDelete(SeqList* self, PyObject* args)
@@ -154,36 +157,29 @@
     if (PyArg_ParseTuple(args, "i", &index) < 0)
     {
         PyErr_SetString(PyExc_Exception, "Args parsed failure!");
         Py_RETURN_FALSE;
     }
     else
     {
-        if (index<0||index>self->length)
-        {
-            Py_RETURN_FALSE;
-        }
-        else
+        for (int i = index; i < self->length; i++)
         {
-            for (int i = index; i < self->length; i++)
-            {
-                self->elem[i] = self->elem[i + 1];
-            }
-            self->elem[self->length] = NULL;
-            self->length--;
-            Py_RETURN_TRUE;
+            self->elem[i] = self->elem[i + 1];
         }
+        self->elem[self->length] = NULL;
+        self->length--;
+        Py_RETURN_TRUE;
     }
 }
 static PyObject* TraverseList(SeqList* self, PyObject* args)
 {
     int i = 0;
     while (i < self->length)
     {
-        PyObject_Print(self->elem[i],stdout,0);
+        PyObject_Print(self->elem[i], stdout, 0);
         i++;
     }
     printf("\n");
 }
 static PyMethodDef SeqList_methods[] = {
     {"init_list",InitList,METH_VARARGS,""},
     {"destroy_list",DestroyList,METH_VARARGS,""},
@@ -194,15 +190,15 @@
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
     {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 static PyTypeObject SeqListObject = {
     PyVarObject_HEAD_INIT(NULL,0)
-    .tp_name = "Utilities.SeqList",
+    .tp_name = "SequentialList.SeqList",
     .tp_new = SeqList_new,
     .tp_init = (initproc)SeqList_init,
     .tp_dealloc = (destructor)SeqList_destroy,
     .tp_basicsize = sizeof(SeqList),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
     .tp_members = SeqList_members,
```

### Comparing `AdroitFisherman-0.0.23/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.24/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.23
+Version: 0.0.24
 Summary: This is a simple package about Data Structure packed by C/C++ language.
+Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
+License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3.10
@@ -112,7 +114,8 @@
     {"get_elem",GetElem,METH_VARARGS,""},
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
     {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 ```
+
```

### Comparing `AdroitFisherman-0.0.23/PKG-INFO` & `AdroitFisherman-0.0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.23
+Version: 0.0.24
 Summary: This is a simple package about Data Structure packed by C/C++ language.
+Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
+License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3.10
@@ -112,7 +114,8 @@
     {"get_elem",GetElem,METH_VARARGS,""},
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
     {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 ```
+
```

### Comparing `AdroitFisherman-0.0.23/README.md` & `AdroitFisherman-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.23/setup.py` & `AdroitFisherman-0.0.24/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup,Extension
-import os
-SeqList=Extension("AdroitFisherman.Utilities",sources=['AdroitFisherman/includes/SeqList.c'])
-
+SeqList=Extension("AdroitFisherman.SequentialList",sources=['AdroitFisherman/includes/SeqList.c'])
+SingleLinkedList=Extension("AdroitFisherman.SingleLinkedList",sources=['AdroitFisherman/includes/SingleLinkedList.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.23",
+    version="0.0.24",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
@@ -18,11 +17,11 @@
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3.10",
         "Topic :: Utilities"
     ],
     include_package_data=True,
-    packages=['AdroitFisherman.SequentialList'],
-    ext_modules=[SeqList]
+    packages=['AdroitFisherman.Utilities'],
+    ext_modules=[SeqList,SingleLinkedList]
 )
 read_me.close()
```

