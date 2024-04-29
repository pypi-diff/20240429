# Comparing `tmp/txdir-2.0.0-py3-none-any.whl.zip` & `tmp/txdir-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 16415 bytes, number of entries: 8
--rw-r--r--  2.0 unx    30915 b- defN 19-Nov-20 20:39 txdir.py
--rw-r--r--  2.0 unx     9395 b- defN 19-Nov-20 21:35 txdir-2.0.0.data/data/man/man1/txdir.1
--rw-r--r--  2.0 unx     1059 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     9497 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      633 b- defN 19-Nov-20 21:35 txdir-2.0.0.dist-info/RECORD
-8 files, 51654 bytes uncompressed, 15311 bytes compressed:  70.4%
+Zip file size: 16392 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    31299 b- defN 24-Apr-29 15:40 txdir.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Apr-29 16:02 txdir-2.0.2.data/data/man/man1/txdir.1
+-rw-r--r--  2.0 unx     1059 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     9503 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      633 b- defN 24-Apr-29 16:02 txdir-2.0.2.dist-info/RECORD
+8 files, 51327 bytes uncompressed, 15288 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: txdir.py
 Comment: 
 
-Filename: txdir-2.0.0.data/data/man/man1/txdir.1
+Filename: txdir-2.0.2.data/data/man/man1/txdir.1
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/LICENSE.txt
+Filename: txdir-2.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/METADATA
+Filename: txdir-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/WHEEL
+Filename: txdir-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/entry_points.txt
+Filename: txdir-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/top_level.txt
+Filename: txdir-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: txdir-2.0.0.dist-info/RECORD
+Filename: txdir-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## txdir.py

```diff
@@ -10,15 +10,15 @@
 from threading import RLock
 from urllib import request
 from tempfile import NamedTemporaryFile
 from base64 import b64encode, b64decode
 import pathspec
 
 #also in README.rst
-__version__ = "2.0.0"
+__version__ = "2.0.2"
 
 #see test_txdir.py to see how to change
 MID = '├'
 END = '└'
 HOR = '─'
 VER = '│'
 LNKL = '<-'
@@ -68,20 +68,20 @@
     )
 
 def set_utf8():
     set_tree_chars()
 
 
 #OS
-cwd = lambda: os.getcwd().replace('\\', '/')
+def cwd(): return os.getcwd().replace('\\', '/')
 cd = os.chdir
 mkdir = partial(os.makedirs, exist_ok=True)
-relpath = lambda x, start: os.path.relpath(x, start=start).replace('\\', '/')
-dirname = lambda x: os.path.dirname(x).replace('\\', '/')
-normjoin = lambda *x: os.path.normpath(os.path.join(*x)).replace("\\", "/")
+def relpath(x, start): return os.path.relpath(x, start=start).replace('\\', '/')
+def dirname(x): return os.path.dirname(x).replace('\\', '/')
+def normjoin(*x): return os.path.normpath(os.path.join(*x)).replace("\\", "/")
 basename = os.path.basename
 exists = os.path.exists
 isfile = os.path.isfile
 isdir = os.path.isdir
 islink = os.path.islink
 listdir = os.listdir
 readlink = os.readlink
@@ -184,15 +184,15 @@
     parent = up(start)
     if start == parent:
         try:
             rootres = start.replace('\\','/').strip('/').strip(':')
             if len(rootres)==1 and 'win' in sys.platform: # pragma: no cover
                 rootres = ''
             return rootres
-        except:
+        except Exception:
             return None
     if not parent:
         return parent
     return up_dir(match,start=parent,listdir=listdir,up=up)
 class GitIgnore:
     def __init__(self
                  ,start
@@ -259,15 +259,15 @@
             dn = name(d)
             if not with_dot and dn.startswith('.'):
                 continue
             padding = prefix + MID_END[i==lends-1]
             if islink(pd):
                 try:
                     rlink = readlink(pd)
-                except: # pragma: no cover
+                except Exception: # pragma: no cover
                     rlink = ''
                 yield padding + dn + ' ' + LNKR + ' ' + rlink
             elif isdir(pd):
                 yield padding + dn + '/'
                 yield from _tree(pd, prefix + SUB_MID_END[i==lends-1])
             elif with_files:
                 yield padding + dn
@@ -286,16 +286,16 @@
             yield i
 def intervals(nms):
     return list(zip(nms[:], nms[1:]))
 def _rex():
     dwn = re.escape(DWN)
     lnkr = re.escape(LNKR)
     return argparse.Namespace(
-    _re_pth_plus = re.compile(r'^(\w[^ </\\]*)(\s*'+dwn+r'\s*|\s*[\\/]\s*|\s*'+lnkr+r'\s*)*([\w\.].*)*')
-    ,_re_lnk_pth_plus = re.compile(r'^(/?\w[^ </\\]*)(\s*'+dwn+r'\s*|\s*[\\/]\s*|\s*'+lnkr+r'\s*)*([\w\.].*)*') #for symlink
+    _re_pth_plus = re.compile(r'^([\w\.][^ </\\]*)(\s*'+dwn+r'\s*|\s*[\\/]\s*|\s*'+lnkr+r'\s*)*([\w\.].*)*')
+    ,_re_lnk_pth_plus = re.compile(r'^(/?[\w\.][^ </\\]*)(\s*'+dwn+r'\s*|\s*[\\/]\s*|\s*'+lnkr+r'\s*)*([\w\.].*)*') #for symlink
     ,_re_skip = re.compile(r'[^\s'+re.escape(MID+VER+END+HOR)+']')
     ,_re_skip_middle = re.compile(r'[^\s'+re.escape(VER)+']')
     ,_re_to_file = re.compile(r'['+re.escape(MID+END)+']')
     ,_re_space = re.compile(r'[^ ]')
     )
 def view_to_tree(view_str_list
          ,fullpthroot=None
@@ -331,69 +331,72 @@
     pwd = cwd()
     if not fullpthroot:
         fullpthroot = pwd
     for treestart, t in enumerate(view_str_list):
         try:
             ct = _r._re_skip.search(t).span()[0]
             break
-        except:
+        except Exception:
             continue
     sublst = [t[ct:].rstrip() for t in view_str_list[treestart:]]
     isublst = list(rindices(_r._re_lnk_pth_plus, sublst))
     isublst.append(len(sublst))
     for strt, last in intervals(isublst):
         file_entry = sublst[strt]
         try:
             efile, delim, url = _r._re_pth_plus.match(file_entry).groups()
-        except: #/symlink/rel/to/root <- name
+        except Exception: #/symlink/rel/to/root <- name
             lnk = fullpthroot+file_entry
             lndst = basename(lnk)
             try:
                 _,lndst = lndst.split(LNKL)
                 lnk,_ = lnk.split(LNKL)
-            except: pass
+            except Exception:
+                pass
             try:
                 lnk = relpath(lnk.strip().strip('/'),pwd.strip('/'))
                 symlink(lnk,lndst.strip())
-            except: pass
+            except Exception:
+                pass
             continue
         if efile:
             if strt < last - 1:
                 nxtline = sublst[strt + 1]
                 try:
-                    ix = _r._re_to_file.search(nxtline).span()[0]
+                    _ = _r._re_to_file.search(nxtline).span()[0]
                     # file name starter found
                     mkdir(efile)
                     with withcwd(efile):
                         view_str_list = sublst[strt + 1:last]
                         view_to_tree(view_str_list,fullpthroot
                                      ,cwd=cwd
                                      ,mkdir=mkdir
                                      ,symlink=symlink
                                      ,withcwd=withcwd
                                      ,filewrite=filewrite
                                      ,eprint=eprint
                                      )
-                except:# .. else file content
+                except Exception:# .. else file content
                     cntent = sublst[strt + 1:last]
                     ct = 0
                     try:
                         ct = _r._re_skip_middle.search(cntent[0]).span()[0]
-                    except:
+                    except Exception:
                         eprint(strt, last, '\n'.join(cntent[:10]))
                         eprint("FIRST LINE OF FILE CONTENT MUST NOT BE EMPTY!")
                     cntlns = [t[ct:] + '\n' for t in cntent]
                     fileput(efile,cntlns,filewrite=filewrite)
             elif delim:
                 if '\\' in delim or '/' in delim:
                     mkdir(efile)
                 elif LNKR in delim and url and efile: #name -> ../rel/to/here
                     try:
                         symlink(url,efile)
-                    except: pass
+                    except Exception:
+                        pass
                 elif DWN in delim:
                     urlretrieve(url, efile,filewrite=filewrite,eprint=eprint)
             else:
                 if not exists(efile):
                     filewrite(efile,'')
 
 def tree_to_flat(rootpath = None
@@ -443,15 +446,15 @@
             if not with_dot and dn.startswith('.'):
                 continue
             nprefix = prefix+[dn]
             thispth = '/'.join(nprefix)
             if islink(pd):
                 try:
                     rlink = readlink(pd)
-                except: # pragma: no cover
+                except Exception: # pragma: no cover
                     rlink = ''
                 yield thispth + ' ' + LNKR + ' ' + rlink
             elif isdir(pd):
                 entries = list(_tree(pd, nprefix))
                 if entries:
                     yield from entries
                 else:
@@ -502,39 +505,43 @@
         usplit = e.split(DWN)
         if len(esplit) == 2: #islink
             fnm = esplit[0].strip()
             tgt = esplit[1].strip()
             if tgt.startswith('/'):
                 tgt = '../'*(len(fnm.split('/'))-1)+tgt[1:]
             dfnm = dirname(fnm)
-            if dfnm: mkdir(dfnm)
+            if dfnm:
+                mkdir(dfnm)
             try:
                 symlink(tgt,fnm)
-            except: pass
+            except Exception:
+                pass
         elif len(usplit) == 2:
             urlretrieve(usplit[1], usplit[0], filewrite=filewrite,eprint=eprint)
         elif e.endswith('/'):
             mkdir(e)
         else:
             de = dirname(e)
-            if de: mkdir(de)
+            if de:
+                mkdir(de)
             indent,fllns = 0,[]
             try:
                 j = i
                 while j<leni:
                     x = flat_str_list[j]
                     if not x or x.startswith(' '):
                         fllns.append(x)
                     else: # pragma: no cover (it is covered, but coverage says not)
                         break
                     j = j+1
                 ln0 = fllns[0]
                 indent = _r._re_space.search(ln0).span()[0]
                 i = j
-            except: pass
+            except Exception:
+                pass
             flcntlns = [x[indent:]+'\n' for x in fllns]
             if flcntlns or not exists(e):
                 fileput(e,flcntlns,filewrite=filewrite)
 
 def to_tree(view_or_flat):
     """Check whether a flat listing or indented view,
     then create the directory accordingly"""
@@ -608,24 +615,24 @@
     def mkdir(self,apath,content=None):
         return self.cd(apath,[] if content is None else content)
 
     def cd(self,apath,content=None):#content != None == make
         c = self
         try:
             apath = [x for x in apath.split('/') if x]
-        except:
+        except Exception:
             pass
         maxi = len(apath)-1
         for i,an in enumerate(apath):
             if c.isdir():
                 try:
                     c = next(x for x in c.content if x.name==an)
                     continue
-                except:
-                    if an == '.': 
+                except Exception:
+                    if an == '.':
                         continue
                     elif an == '..':
                         c = c.parent
                         continue
             if content is None:
                 raise FileNotFoundError(f"{an} in {c.path()} while cd to {apath}")
             else:
@@ -688,15 +695,15 @@
                 elif token == "/":
                     if current.isdir() and current.content:
                         current = current.content[-1]
                 elif token == ".":
                     if current.parent:
                         current = current.parent
                 else:
-                    node = TxDir(token, parent=current)
+                    _ = TxDir(token, parent=current)
         return root
 
     @staticmethod
     def fromview(viewstr,eprint=eprint):
         """Builds the directory from an indented view.
 
         viewstr:
@@ -813,15 +820,16 @@
         """Create directory in file system"""
         lastdir = None
         for e in self:
             if e.islink():
                 mkdir(dirname(e.path()))
                 try:
                     symlink(e.content,e.path())
-                except: pass
+                except Exception:
+                    pass
             elif e.isdir():
                 lastdir = e.path()
                 mkdir(lastdir)
             else:
                 mkdir(dirname(e.path()))
                 fileput(e.path(),e.content)
         return lastdir
@@ -837,29 +845,29 @@
         args.setdefault('infile','-')
         args.setdefault('outdir','-')
         args=argparse.Namespace(**args)
     else:
         parser = argparse.ArgumentParser(add_help=False,description='''\
         Files/dirs are ignored via .gitignore.
         If the directory contains unignored binary files,
-        exclude files with '-f' or ignoring content with '-n'.
+        exclude files with '-f'. Ignore content with '-n'.
         Text file content must not have an empty first line.
         '''
         )
         parser.add_argument("-h", action="help", help="Print help information.")
         parser.add_argument(
             "-v",
             action="version",
             version=f"%(prog)s {__version__}",
             help="Print version information.",
         )
         parser.add_argument(
             "-a",
             action="store_true",
-            help="Use ASCII instead of unicode when printint the indented view.",
+            help="Use ASCII instead of unicode when printing the indented view.",
         )
         parser.add_argument(
             "-b",
             action="store_true",
             help="Include content of binary files as base64 encoded.",
         )
         parser.add_argument(
@@ -937,15 +945,15 @@
     if trees:
         tx = TxDir.fromcmds(trees)
 
     try:
         sys.stdin = codecs.getreader("utf-8")(sys.stdin.detach())
         sys.stdout = codecs.getwriter("utf-8")(sys.stdout.detach())
         sys.stderr = codecs.getreader("utf-8")(sys.stderr.detach())
-    except:
+    except Exception:
         pass
     fview = []
     inf = isfile(infile)
     if not inf and infile == '-':
         if not trees:
             fview = [x.rstrip() for x in sys.stdin.readlines()]
     elif inf:
@@ -967,21 +975,25 @@
                              ,with_content=with_content
                              ,with_binary=with_binary
                              ,maxdepth=maxdepth
                                   ))
     outf = isfile(outdir)
     if not outf:
         if outdir == '-':
-            if tx: print(tx.flat()) if args.l else print(tx.view())
-            if fview: print('\n'.join(fview))
+            if tx:
+                print(tx.flat()) if args.l else print(tx.view())
+            if fview:
+                print('\n'.join(fview))
         else: #dir
             mkdir(outdir)
             with with_cwd(outdir):
-                if tx: tx.tree()
-                if fview: to_tree(fview)
+                if tx:
+                    tx.tree()
+                if fview:
+                    to_tree(fview)
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 
 # vim: ts=4 sw=4 sts=4 et noai nocin nosi inde=
```

## Comparing `txdir-2.0.0.dist-info/LICENSE.txt` & `txdir-2.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `txdir-2.0.0.dist-info/METADATA` & `txdir-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: txdir
-Version: 2.0.0
+Version: 2.0.2
 Summary: Creating file tree from text tree and vice versa
 Home-page: https://github.com/rpuntaie/txdir
 Author: Roland Puntaier
 Author-email: roland.puntaier@gmail.com
 License: MIT
 Keywords: text tree directory file content template
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,18 +18,19 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 Requires-Dist: pathspec
 
 =================================
-txdir(1) Version 2.0.0 \| txdir
+txdir(1) Version 2.0.2 \| txdir
 =================================
 
 NAME
 ====
 
 **txdir** — text tree from or to file tree
 
@@ -354,9 +354,7 @@
 
 
 License
 -------
 
 MIT
 
-
-
```

