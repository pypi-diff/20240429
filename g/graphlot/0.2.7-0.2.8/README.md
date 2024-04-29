# Comparing `tmp/graphlot-0.2.7-py3-none-any.whl.zip` & `tmp/graphlot-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18058 bytes, number of entries: 7
+Zip file size: 18159 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx      140 b- defN 23-May-05 11:08 graphlot/__init__.py
--rwxrwxrwx  2.0 unx    18241 b- defN 24-Mar-21 18:27 graphlot/graphlot.py
--rwxrwxrwx  2.0 unx    34523 b- defN 24-Mar-21 18:28 graphlot-0.2.7.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx     2138 b- defN 24-Mar-21 18:28 graphlot-0.2.7.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 24-Mar-21 18:28 graphlot-0.2.7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        9 b- defN 24-Mar-21 18:28 graphlot-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      549 b- defN 24-Mar-21 18:28 graphlot-0.2.7.dist-info/RECORD
-7 files, 55692 bytes uncompressed, 17088 bytes compressed:  69.3%
+-rwxrwxrwx  2.0 unx    18519 b- defN 24-Apr-29 15:35 graphlot/graphlot.py
+-rwxrwxrwx  2.0 unx    34523 b- defN 24-Apr-29 15:37 graphlot-0.2.8.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx     2138 b- defN 24-Apr-29 15:37 graphlot-0.2.8.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 24-Apr-29 15:37 graphlot-0.2.8.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        9 b- defN 24-Apr-29 15:37 graphlot-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      549 b- defN 24-Apr-29 15:37 graphlot-0.2.8.dist-info/RECORD
+7 files, 55970 bytes uncompressed, 17189 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: graphlot/__init__.py
 Comment: 
 
 Filename: graphlot/graphlot.py
 Comment: 
 
-Filename: graphlot-0.2.7.dist-info/LICENSE.txt
+Filename: graphlot-0.2.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: graphlot-0.2.7.dist-info/METADATA
+Filename: graphlot-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: graphlot-0.2.7.dist-info/WHEEL
+Filename: graphlot-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: graphlot-0.2.7.dist-info/top_level.txt
+Filename: graphlot-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: graphlot-0.2.7.dist-info/RECORD
+Filename: graphlot-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## graphlot/graphlot.py

```diff
@@ -101,20 +101,27 @@
     if node_color_attribute:
         NodeClasses = []
         for n in G.nodes(data = True):
             try:
                 NodeClasses.append(n[1][node_color_attribute])
             except:
                 NodeClasses.append('unknown')
-        N = len(set(NodeClasses))
-        Cdict=dict(zip(set(NodeClasses),[n for n in range(N)]))
-        NodeColors = list(map(Cdict.get,NodeClasses))
+        
+        if all([isinstance(classe,str) for classe in NodeClasses]):
+            # Here we will detect automatically if we need to use a categorical color type or continuous one
+        
+            N = len(set(NodeClasses))
+            Cdict=dict(zip(set(NodeClasses),[n for n in range(N)]))
+            NodeColors = list(map(Cdict.get,NodeClasses))
 
-        colors  = [f"C{i}" for i in np.arange(1, max(NodeColors)+1)]
-#             cmap, norm = matplotlib.colors.from_levels_and_colors(np.arange(1, max(NodeColors)+2), colors)
+            colors  = [f"C{i}" for i in np.arange(1, max(NodeColors)+1)]
+    #             cmap, norm = matplotlib.colors.from_levels_and_colors(np.arange(1, max(NodeColors)+2), colors)
+        else:
+            
+            NodeColors = NodeColors
 
     else:
         N = len(G.nodes)
         NodeColors = [0 for n in range(N)]
         colors  = [f"C{i}" for i in np.arange(1, max(NodeColors)+1)]
 #             cmap, norm = None,None
```

## Comparing `graphlot-0.2.7.dist-info/LICENSE.txt` & `graphlot-0.2.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `graphlot-0.2.7.dist-info/METADATA` & `graphlot-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlot
-Version: 0.2.7
+Version: 0.2.8
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: networkx
 Requires-Dist: igraph
 Requires-Dist: pygraphviz
```

## Comparing `graphlot-0.2.7.dist-info/RECORD` & `graphlot-0.2.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 graphlot/__init__.py,sha256=rRv-JGgzhLgHGhpCJP34Ihavp-U2-yso6Iw7RQFCaqM,140
-graphlot/graphlot.py,sha256=YHqeV8Sl6aOGdiWAxt0rQ_xcVK9y7LnuodamEbfzNq8,18241
-graphlot-0.2.7.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-graphlot-0.2.7.dist-info/METADATA,sha256=N_wo2JdOISs__9dDn0mDYAToQmOifEH8OCiWkRzET5w,2138
-graphlot-0.2.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-graphlot-0.2.7.dist-info/top_level.txt,sha256=DCHVg4MpdSH08h3dxhncRR01bL_mfqfkKpAK0xpkeWM,9
-graphlot-0.2.7.dist-info/RECORD,,
+graphlot/graphlot.py,sha256=fKiMnAGEfuLjmLKySoSw6xBaciskQaHvMN2JOpKJ8kE,18519
+graphlot-0.2.8.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+graphlot-0.2.8.dist-info/METADATA,sha256=eomD-1Lu9PuSCyXRdMj_erg_151qZEs_GbTwdXf3i7E,2138
+graphlot-0.2.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+graphlot-0.2.8.dist-info/top_level.txt,sha256=DCHVg4MpdSH08h3dxhncRR01bL_mfqfkKpAK0xpkeWM,9
+graphlot-0.2.8.dist-info/RECORD,,
```

