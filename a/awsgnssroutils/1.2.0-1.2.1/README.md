# Comparing `tmp/awsgnssroutils-1.2.0.tar.gz` & `tmp/awsgnssroutils-1.2.1.tar.gz`

## Comparing `awsgnssroutils-1.2.0.tar` & `awsgnssroutils-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/__init__.py
--rw-r--r--   0        0        0    50883 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/database.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/__init__.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/rotcol.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/awsro.py
--rwxr-xr-x   0        0        0     8082 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/brute_force.py
--rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/celestrak.py
--rwxr-xr-x   0        0        0    23003 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/collocation.py
--rwxr-xr-x   0        0        0     6273 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/constants_and_utils.py
--rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/eumetsat.py
--rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nadir_satellite.py
--rw-r--r--   0        0        0    15639 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nasa_earthdata.py
--rwxr-xr-x   0        0        0    10076 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/rotation_collocation.py
--rw-r--r--   0        0        0    18531 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/spacetrack.py
--rw-r--r--   0        0        0    27555 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/timestandards.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/__init__.py
--rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/amsua.py
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/atms.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/LICENSE
--rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/__init__.py
+-rw-r--r--   0        0        0    51140 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/database.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/__init__.py
+-rw-r--r--   0        0        0    19330 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/rotcol.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/awsro.py
+-rwxr-xr-x   0        0        0     8082 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/brute_force.py
+-rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/celestrak.py
+-rwxr-xr-x   0        0        0    23003 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/collocation.py
+-rwxr-xr-x   0        0        0     6273 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/constants_and_utils.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/eumetsat.py
+-rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/nadir_satellite.py
+-rw-r--r--   0        0        0    16053 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/nasa_earthdata.py
+-rwxr-xr-x   0        0        0    10076 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/rotation_collocation.py
+-rw-r--r--   0        0        0    18854 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/spacetrack.py
+-rw-r--r--   0        0        0    27555 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/timestandards.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/__init__.py
+-rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/amsua.py
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/atms.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/LICENSE
+-rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/README.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    18302 2020-02-02 00:00:00.000000 awsgnssroutils-1.2.1/PKG-INFO
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/database.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,16 @@
                         when the method OccList.download is called. "data_root" 
                         must be an absolute path.
 
     version             The default RO format version. The available versions 
                         can be found in s3://gnss-ro-data/dynamo. 
     """
 
-    # defaults = { 'metadata_root': "", 'data_root': "", 'version': "" }
+    ret = { 'status': None, 'messages': [], 'comments': [], 'data': None }
+
     new_defaults = {}
 
     #  Check for existence of defaults file. Get existing defaults. 
 
     HOME = os.path.expanduser( "~" )
     defaults_file_path = os.path.join( HOME, defaults_filename )
 
@@ -261,51 +262,67 @@
     else: 
         defaults = {}
 
     #  Be sure the paths are absolute paths. Also, create paths if they 
     #  don't already exist. 
 
     if metadata_root is not None: 
-        if metadata_root != os.path.abspath( metadata_root ): 
-            raise AWSgnssroutilsError( "BadPathName", 
-                    f'Path to metadata_root ({metadata_root}) must be an absolute path' )
-        else: 
-            defaults.update( { 'metadata_root': metadata_root } )
+
+        try: 
             os.makedirs( metadata_root, exist_ok=True )
 
+        except: 
+            ret['status'] = "fail"
+            ret['messages'].append( "BadPathName" )
+            ret['comments'].append( f'Unable to create metadata_root ("{metadata_root}") as a directory.' )
+            return ret
+
+        defaults.update( { 'metadata_root': os.path.abspath( metadata_root ) } )
+
+
     if data_root is not None: 
-        if data_root != os.path.abspath( data_root ): 
-            raise AWSgnssroutilsError( "BadPathName", 
-                    f'Path to data_root ({data_root}) must be an absolute path' )
-        else: 
-            defaults.update( { 'data_root': data_root } )
+
+        try: 
             os.makedirs( data_root, exist_ok=True )
 
+        except: 
+            ret['status'] = "fail"
+            ret['messages'].append( "BadPathName" )
+            ret['comments'].append( f'Unable to create data_root ("{data_root}") as a directory.' )
+            return ret
+
+        defaults.update( { 'data_root': os.path.abspath( data_root ) } )
 
     #  Check for a valid version. 
 
     if version is not None: 
 
         if version not in valid_versions: 
-            raise AWSgnssroutilsError( "InvalidVersion", f'Version "{version}" is invalid; ' + \
+            ret['status'] = "fail"
+            ret['messages'].append( "InvalidVersion" )
+            ret['comments'].append( f'Version "{version}" is invalid; ' + \
                     'valid versions are ' + ", ".join( valid_versions ) )
+            return ret
 
         defaults.update( { 'version': version } )
 
         if metadata_root is not None: 
             os.makedirs( os.path.join( metadata_root, version ), exist_ok=True )
 
     #  Record new set of defaults. 
 
     with open( defaults_file_path, 'w' ) as fp: 
-        json.dump( defaults, fp )
+        json.dump( defaults, fp, indent="  " )
 
     #  Done. 
 
-    return defaults
+    ret['data'] = defaults
+    ret['status'] = "success"
+
+    return ret
 
 
 def populate() -> subprocess.CompletedProcess : 
     """Populate the metadata database in the path established by 
     setdefaults. 
 
     This function will synchronize the default metadata_root path
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/rotcol.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/rotcol.py`

 * *Files 12% similar despite different names*

```diff
@@ -329,80 +329,105 @@
 
             from awsgnssroutils.database import setdefaults
 
             kwargs = { 'version': "v1.1" }
             if args.dataroot is not None: 
                 kwargs.update( { 'data_root': args.dataroot } )
             if args.metadataroot is not None: 
-                kwargs.update( { 'metadata_root': args.dataroot } )
+                kwargs.update( { 'metadata_root': args.metadataroot } )
 
             print( "Updating AWS RO defaults: " + json.dumps( kwargs ) )
-            setdefaults( **kwargs )
+
+            ret = setdefaults( **kwargs )
+
+            if ret['status'] == "success": 
+                print( "Successful." )
+                print( ret['data'] )
+            else: 
+                print( "Failed.\n{:}: {:}".format( ret['messages'][-1], ret['comments'][-1] ) )
 
         elif args.service == "eumetsat": 
 
             from awsgnssroutils.collocation.core.eumetsat import setdefaults
 
             kwargs = {}
             if args.dataroot is not None: 
                 kwargs.update( { 'root_path': args.dataroot } )
             if args.consumer_key is not None and args.consumer_secret is not None: 
                 kwargs.update( { 'eumetsattokens': ( args.consumer_key, args.consumer_secret ) } )
 
             print( "Updating EUMETSAT defaults: " + json.dumps( kwargs ) )
+
             ret = setdefaults( **kwargs )
-            if ret['status'] == "fail": 
-                print( "Error: \n" + "\n".join( ret['comments'] ) )
+
+            if ret['status'] == "success": 
+                print( "Successful." )
+                odata = { key: value for key, value in ret['data'].items() if "password" not in key }
+                print( odata )
+            else: 
+                print( "Failed.\n{:}: {:}".format( ret['messages'][-1], ret['comments'][-1] ) )
 
         elif args.service == "earthdata": 
 
             from awsgnssroutils.collocation.core.nasa_earthdata import setdefaults
 
             kwargs = {}
             if args.dataroot is not None: 
                 kwargs.update( { 'root_path': args.dataroot } )
             if args.username is not None: 
                 password = getpass()
                 kwargs.update( { 'earthdatalogin': ( args.username, password ) } )
 
             print( "Updating NASA Earthdata defaults: " + json.dumps( kwargs ) )
+
             ret = setdefaults( **kwargs )
-            if ret['status'] == "fail": 
-                print( "Error: \n" + "\n".join( ret['comments'] ) )
+
+            if ret['status'] == "success": 
+                print( "Successful." )
+                odata = { key: value for key, value in ret['data'].items() if "password" not in key }
+                print( odata )
+            else: 
+                print( "Failed.\n{:}: {:}".format( ret['messages'][-1], ret['comments'][-1] ) )
 
         elif args.service == "spacetrack": 
 
             from awsgnssroutils.collocation.core.spacetrack import setdefaults
 
             kwargs = {}
             if args.dataroot is not None: 
                 kwargs.update( { 'root_path': args.dataroot } )
             if args.username is not None: 
                 password = getpass()
                 kwargs.update( { 'spacetracklogin': ( args.username, password ) } )
 
             print( "Updating Space-Track defaults: " + json.dumps( kwargs ) )
+
             ret = setdefaults( **kwargs )
-            if ret['status'] == "fail": 
-                print( "Error: \n" + "\n".join( ret['comments'] ) )
+
+            if ret['status'] == "success": 
+                print( "Successful." )
+                odata = { key: value for key, value in ret['data'].items() if "password" not in key }
+                print( odata )
+            else: 
+                print( "Failed.\n{:}: {:}".format( ret['messages'][-1], ret['comments'][-1] ) )
 
         else: 
 
-            print( f'Invalid service: "{args.service}"' )
+            print( f'Invalid service: "{args.service}". Get help by "rotcol setdefaults -h".' )
 
     elif args.command == "execute": 
 
         #  Execute rotation-collocation algorithm for collocation finding. 
 
         #  Get arguments for rotation-collocation: missions, timerange, nadir_satellite, 
         #  nadir_instrument, ro_processing_center. 
 
-        missions = re.split( "\s+", args.missions )
+        missions = re.split( r"\s+", args.missions )
 
-        ss = re.split( "\s+", args.timerange )
+        ss = re.split( r"\s+", args.timerange )
         timerange = ( datetime.fromisoformat( ss[0] ), datetime.fromisoformat( ss[1] ) )
 
         nadir_satellite = str( args.nadir_satellite )
         nadir_instrument = str( args.nadir_instrument )
         ro_processing_center = str( args.ro_processing_center )
         output_file = str( args.output )
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/awsro.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/awsro.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/brute_force.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/brute_force.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/celestrak.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/celestrak.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/collocation.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/collocation.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/constants_and_utils.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/constants_and_utils.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/eumetsat.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/eumetsat.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,33 +41,29 @@
     """This method sets the default root path for EUMETSAT Data Store downloads.
     It also can set the consumer key and consumer secret as created on the 
     EUMETSAT Data Store website/account. If the keyword eumetsattokens is given, 
     it must be a 2-element tuple/list containing the user's consumer key and 
     consumer secret as provided for the user's account on the EUMETSAT Data 
     Store."""
 
-    ret = { 'status': None, 'messages': [], 'comments': [] }
-
-    if isinstance(root_path,str): 
+    ret = { 'status': None, 'messages': [], 'comments': [], 'data': None }
+    new_defaults = {}
 
-        if os.path.exists( defaults_file ): 
-            with open( defaults_file, 'r' ) as f: 
-                defaults = json.load( f )
-        else: 
-            defaults = {}
+    if root_path is not None:
 
-        path = os.path.abspath( os.path.expanduser( root_path ) ) 
-        defaults.update( { root_path_variable: path } )
-        os.makedirs( path, exist_ok=True )
+        try:
+            os.makedirs( root_path, exist_ok=True )
 
-        #  Write to defaults file. 
+        except:
+            ret['status'] = "fail"
+            ret['messages'].append( "BadPathName" )
+            ret['comments'].append( f'Unable to create root_path ("{root_path}") as a directory.' )
+            return ret
 
-        with open( defaults_file, 'w' ) as f: 
-            json.dump( defaults, f, indent="  " )
-        os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
+        new_defaults.update( { root_path_variable: os.path.abspath( root_path ) } )
 
     #  Define consumer key, consumer secret. 
 
     if eumetsattokens is not None: 
         if isinstance(eumetsattokens,tuple) or isinstance(eumetsattokens,list): 
             if len(eumetsattokens) == 2: 
                 command = [ "eumdac", "set-credentials", eumetsattokens[0], eumetsattokens[1] ]
@@ -81,14 +77,36 @@
 
         else:
             ret['status'] = "fail"
             ret['messages'].append( "InvalidArgument" )
             ret['comments'].append( "eumetsattokens must be a tuple or a list" )
             return ret
 
+    if len( new_defaults ) > 0: 
+
+        #  Get old defaults.
+
+        if os.path.exists( defaults_file ):
+            with open( defaults_file, 'r' ) as f:
+                defaults = json.load( f )
+        else:
+            defaults = {}
+
+        #  Update with new defaults.
+
+        defaults.update( new_defaults )
+
+        #  Write to defaults file.
+
+        with open( defaults_file, 'w' ) as f:
+            json.dump( defaults, f, indent="  " )
+        os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
+
+        ret['data'] = defaults
+
     #  Done. 
 
     ret['status'] = "success"
 
     return
 
 
@@ -176,30 +194,30 @@
     def inventory_metop_amsua( self ): 
         """Create an inventory of the files available on the local file system, 
         keeping information on the absolute path and the time range of data."""
 
         #  Get list of satellites. 
 
         data_root = os.path.join( self.data_root, "amsua" )
-        satellites = [ p for p in os.listdir( data_root ) if re.search( "^Metop-", p ) \
+        satellites = [ p for p in os.listdir( data_root ) if re.search( r"^Metop-", p ) \
                 and os.path.isdir( os.path.join( data_root, p ) ) ]
 
         #  Initialize inventory. 
 
         self.inventory = { sat: [] for sat in satellites }
 
         #  Loop over satellites. 
 
         for sat in satellites: 
 
             for root, subdirs, files in os.walk( os.path.join( data_root, sat ) ): 
                 subdirs.sort()
                 files.sort()
 
-                ss = "^" + sat + "_AMSAL1_(\d{8}T\d{6})Z_(\d{8}T\d{6})Z\.nc$"
+                ss = "^" + sat + r"_AMSAL1_(\d{8}T\d{6})Z_(\d{8}T\d{6})Z\.nc$"
                 st = "%Y%m%dT%H%M%S" 
 
                 for file in files: 
                     m = re.search( ss, file )
                     if m is None: 
                         continue
                     t1 = Time( **{ eumetsat_time_convention: datetime.strptime( m.group(1), st ) } ) 
@@ -280,15 +298,15 @@
         #  repository directory. 
 
         download = False
         matched_files = [] 
 
         for item in inventory: 
 
-            m = re.search( "(\d{14})Z_(\d{14})Z", item )
+            m = re.search( r"(\d{14})Z_(\d{14})Z", item )
             if not m: continue
 
             #  Start time and end time of inventory item. 
 
             dt1 = datetime.strptime( m.group(1), "%Y%m%d%H%M%S" )
             dt2 = datetime.strptime( m.group(2), "%Y%m%d%H%M%S" )
 
@@ -358,15 +376,15 @@
                 #  time of the first sounding in each file, and transfer them into the 
                 #  repository. 
 
                 files = os.listdir( "tmp" )
 
                 for file in files:
                     inpath = os.path.join( "tmp", file )
-                    m = re.search( "^AMSAL1_(\d{8}T\d{6})Z_(\d{8}T\d{6})Z_epct_.*\.nc$", file )
+                    m = re.search( r"^AMSAL1_(\d{8}T\d{6})Z_(\d{8}T\d{6})Z_epct_.*\.nc$", file )
                     t = datetime.strptime( m.group(1), "%Y%m%dT%H%M%S" )
                     outpath = os.path.join( self.data_root, "amsua", satellite, 
                             f'{t.year:4d}', f'{t.month:02d}', f'{t.day:02d}',
                             f'{satellite}_AMSAL1_{m.group(1)}Z_{m.group(2)}Z.nc' )
                     if not os.path.exists( outpath ):
                         os.makedirs( os.path.dirname(outpath), exist_ok=True )
                         os.link( inpath, outpath )
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nadir_satellite.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/nadir_satellite.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/nasa_earthdata.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/nasa_earthdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 HOME = os.path.expanduser( "~" )
 root_path_variable = "nasa_earthdata_root"
 earthdata_machine = "urs.earthdata.nasa.gov"
 time_limit = timedelta( seconds=3600 )
 
 #  String parsing. 
 
-file_search_string = "^SNDR\..*(\d{8}T\d{4})\.m.*\.nc$"
+file_search_string = r"^SNDR\..*(\d{8}T\d{4})\.m.*\.nc$"
 time_parse_string = "%Y%m%dT%H%M" 
 
 #  Establist the netrc file name. 
 
 if system() == "Windows": 
     netrc_file = os.path.join( HOME, "_netrc" )
 else: 
@@ -80,35 +80,31 @@
     """This method sets the default root path for NASA GDAAC downloads.
     Optionally, it also allows you to register your Earthdata username and 
     password in your home .netrc (if you haven't done so already).
 
     The Earthdata username and password can be given as a 2-tuple 
     (username,password) in optional argument earthdatalogin."""
 
-    ret = { 'status': None, 'messages': [], 'comments': [] }
+    ret = { 'status': None, 'messages': [], 'comments': [], 'data': None }
+    new_defaults = {}
 
     #  Set root data path. Create the directory. 
 
-    if isinstance(root_path,str): 
-
-        if os.path.exists( defaults_file ): 
-            with open( defaults_file, 'r' ) as f: 
-                defaults = json.load( f )
-        else: 
-            defaults = {}
+    if root_path is not None:
 
-        path = os.path.abspath( os.path.expanduser( root_path ) ) 
-        defaults.update( { root_path_variable: path } )
-        os.makedirs( path, exist_ok=True )
+        try:
+            os.makedirs( root_path, exist_ok=True )
 
-        #  Write to defaults file. 
+        except:
+            ret['status'] = "fail"
+            ret['messages'].append( "BadPathName" )
+            ret['comments'].append( f'Unable to create root_path ("{root_path}") as a directory.' )
+            return ret
 
-        with open( defaults_file, 'w' ) as f: 
-            json.dump( defaults, f, indent="  " )
-        os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
+        new_defaults.update( { root_path_variable: os.path.abspath( root_path ) } )
 
     #  Write Earthdata login username and password to .netrc file if 
     #  provided. 
 
     if earthdatalogin is not None: 
         if isinstance(earthdatalogin,tuple) or isinstance(earthdatalogin,list): 
             if len(earthdatalogin) == 2: 
@@ -119,15 +115,15 @@
                 else: 
                     lines = []
                 
                 #  Catalog lines according to machine. 
 
                 catalog = {}
                 for line in lines: 
-                    m = re.search( "^machine\s+(\S+)", line )
+                    m = re.search( r"^machine\s+(\S+)", line )
                     if m: 
                         catalog.update( { m.group(1): line.strip() } )
 
                 #  Update catalog to include earthdata. 
 
                 catalog.update( { earthdata_machine: \
                         "machine {:} login {:} password {:}".format( earthdata_machine, *earthdatalogin ) 
@@ -151,14 +147,36 @@
         else: 
 
             ret['status'] = "fail"
             ret['messages'].append( "InvalidArgument" )
             ret['comments'].append( "earthdatalogin must be a tuple or a list" )
             return ret
 
+    if len( new_defaults ) > 0:
+
+        #  Get old defaults.
+
+        if os.path.exists( defaults_file ):
+            with open( defaults_file, 'r' ) as f:
+                defaults = json.load( f )
+        else:
+            defaults = {}
+
+        #  Update with new defaults.
+
+        defaults.update( new_defaults )
+
+        #  Write to defaults file.
+
+        with open( defaults_file, 'w' ) as f:
+            json.dump( defaults, f, indent="  " )
+        os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
+
+        ret['data'] = defaults
+
     #  Done. 
 
     ret['status'] = "success" 
 
     return ret
 
 
@@ -178,15 +196,15 @@
 
     #  Check to see that the earthdata_machine entry exists in the netrc file. 
 
     with open( netrc_file, 'r' ) as f: 
         lines = f.readlines()
 
     for line in lines: 
-        m = re.search( "^machine\s+(\S+)", line )
+        m = re.search( r"^machine\s+(\S+)", line )
         if m: 
             machine = m.group(1)
             if machine == earthdata_machine: 
                 break
         else: 
             machine = None
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/rotation_collocation.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/rotation_collocation.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/spacetrack.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/spacetrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,31 @@
 
 def setdefaults( root_path=None, spacetracklogin=None ):
     """This method sets the default root path for Spacetrack TLE data. If the 
     keyword spacetracklogin is given, it must be a 2-element tuple/list 
     containing the user's username and password for the user's Space-Track 
     account."""
 
-    ret = { 'status': None, 'messages': [], 'comments': [] }
-
+    ret = { 'status': None, 'messages': [], 'comments': [], 'data': None }
     new_defaults = {}
 
     #  Update data root path and create the directory. 
 
-    if isinstance(root_path,str): 
-        path = os.path.abspath( os.path.expanduser( root_path ) ) 
-        new_defaults.update( { root_path_variable: path } )
-        os.makedirs( path, exist_ok=True )
+    if root_path is not None:
+
+        try:
+            os.makedirs( root_path, exist_ok=True )
+
+        except:
+            ret['status'] = "fail"
+            ret['messages'].append( "BadPathName" )
+            ret['comments'].append( f'Unable to create root_path ("{root_path}") as a directory.' )
+            return ret
+
+        new_defaults.update( { root_path_variable: os.path.abspath( root_path ) } )
 
     #  Update username and password. 
 
     if spacetracklogin is not None: 
 
         if isinstance(spacetracklogin,tuple) or isinstance(spacetracklogin,list): 
             if len(spacetracklogin) == 2: 
@@ -89,31 +96,35 @@
 
         else:
             ret['status'] = "fail"
             ret['messages'].append( "InvalidArgument" )
             ret['comments'].append( "spacetracklogin must be a tuple or a list" )
             return ret
 
-    #  Get old defaults. 
+    if len( new_defaults ) > 0:
 
-    if os.path.exists( defaults_file ):
-        with open( defaults_file, 'r' ) as f:
-            defaults = json.load( f )
-    else: 
-        defaults = {}
+        #  Get old defaults.
+
+        if os.path.exists( defaults_file ):
+            with open( defaults_file, 'r' ) as f:
+                defaults = json.load( f )
+        else:
+            defaults = {}
+
+        #  Update with new defaults.
 
-    #  Update with new defaults. 
+        defaults.update( new_defaults )
 
-    defaults.update( new_defaults )
+        #  Write to defaults file.
 
-    #  Write to defaults file. 
+        with open( defaults_file, 'w' ) as f:
+            json.dump( defaults, f, indent="  " )
+        os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
 
-    with open( defaults_file, 'w' ) as f:  
-        json.dump( defaults, f, indent="  " ) 
-    os.chmod( defaults_file, stat.S_IRUSR | stat.S_IWUSR )
+        ret['data'] = defaults
 
     #  Done. 
 
     ret['status'] = "success"
 
     return ret
 
@@ -396,15 +407,15 @@
 
         for root, dirs, files in os.walk( self.data_root ): 
 
             files.sort()
             dirs.sort()
 
             for file in files: 
-                m = re.search( "^sat(\d{5}).*\.txt$", file )
+                m = re.search( r"^sat(\d{5}).*\.txt$", file )
                 if not m: continue
 
                 #  Read first line of the file to get the satellite NORAD number. 
 
                 file_path = os.path.join( root, file )
                 f = open( file_path, 'r' )
                 line = f.readline()
```

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/core/timestandards.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/core/timestandards.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/__init__.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/amsua.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/amsua.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/src/awsgnssroutils/collocation/instruments/atms.py` & `awsgnssroutils-1.2.1/src/awsgnssroutils/collocation/instruments/atms.py`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/LICENSE` & `awsgnssroutils-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/README.md` & `awsgnssroutils-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.2.0/pyproject.toml` & `awsgnssroutils-1.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # requires = [ "hatchling", "s3fs", "numpy", "tqdm" ]
 requires = [ "hatchling>=1.22.2" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awsgnssroutils"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
 	{ name="Stephen Leroy", email="sleroy@aer.com" },
 	{ name="Amy McVey", email="amcvey@aer.com" }
 	]
 description = "Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -19,13 +19,13 @@
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: BSD License",
 	"Operating System :: OS Independent"
 	]
 
 [project.urls]
-"Homepage" = "https://github.com/gnss-ro/aws-opendata/awsgnssroutils"
+"Homepage" = "https://github.com/gnss-ro/aws-opendata/tree/master/awsgnssroutils"
 "Bug Tracker" = "https://github.com/gnss-ro/aws-opendata/issues"
 
 [project.scripts]
 rotcol = "awsgnssroutils.collocation.rotcol:main"
```

### Comparing `awsgnssroutils-1.2.0/PKG-INFO` & `awsgnssroutils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: awsgnssroutils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data
-Project-URL: Homepage, https://github.com/gnss-ro/aws-opendata/awsgnssroutils
+Project-URL: Homepage, https://github.com/gnss-ro/aws-opendata/tree/master/awsgnssroutils
 Project-URL: Bug Tracker, https://github.com/gnss-ro/aws-opendata/issues
 Author-email: Stephen Leroy <sleroy@aer.com>, Amy McVey <amcvey@aer.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

