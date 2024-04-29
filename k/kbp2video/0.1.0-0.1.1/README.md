# Comparing `tmp/kbp2video-0.1.0.tar.gz` & `tmp/kbp2video-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbp2video-0.1.0.tar", last modified: Thu Apr 25 01:32:08 2024, max compression
+gzip compressed data, was "kbp2video-0.1.1.tar", last modified: Mon Apr 29 21:58:17 2024, max compression
```

## Comparing `kbp2video-0.1.0.tar` & `kbp2video-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-25 01:32:08.282324 kbp2video-0.1.0/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.0/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      151 2024-04-25 01:32:08.282324 kbp2video-0.1.0/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.0/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-25 01:32:08.278991 kbp2video-0.1.0/kbp2video/
--rw-r--r--   0 matt      (1000) matt      (1000)      290 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/__main__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/_ffmpegcolor.py
--rw-r--r--   0 matt      (1000) matt      (1000)    70343 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/_gui.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/advanced_editor.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.0/kbp2video/utils.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-25 01:32:08.278991 kbp2video-0.1.0/kbp2video.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      151 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       31 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-04-25 01:32:08.000000 kbp2video-0.1.0/kbp2video.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      305 2024-04-25 01:31:39.000000 kbp2video-0.1.0/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-25 01:32:08.282324 kbp2video-0.1.0/setup.cfg
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.264047 kbp2video-0.1.1/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2024-04-25 01:31:39.000000 kbp2video-0.1.1/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)      166 2024-04-29 21:58:17.264047 kbp2video-0.1.1/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      471 2024-04-25 01:31:39.000000 kbp2video-0.1.1/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.260714 kbp2video-0.1.1/kbp2video/
+-rw-r--r--   0 matt      (1000) matt      (1000)      290 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)       28 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/__main__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      923 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/_ffmpegcolor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    74002 2024-04-29 21:56:59.000000 kbp2video-0.1.1/kbp2video/_gui.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14259 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/advanced_editor.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2024-04-25 01:31:39.000000 kbp2video-0.1.1/kbp2video/utils.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 21:58:17.260714 kbp2video-0.1.1/kbp2video.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      166 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      368 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       49 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       46 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       10 2024-04-29 21:58:17.000000 kbp2video-0.1.1/kbp2video.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      322 2024-04-29 21:56:59.000000 kbp2video-0.1.1/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-29 21:58:17.264047 kbp2video-0.1.1/setup.cfg
```

### Comparing `kbp2video-0.1.0/LICENSE` & `kbp2video-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.0/kbp2video/_ffmpegcolor.py` & `kbp2video-0.1.1/kbp2video/_ffmpegcolor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.0/kbp2video/_gui.py` & `kbp2video-0.1.1/kbp2video/_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,46 +22,62 @@
 from ._ffmpegcolor import ffmpeg_color
 import enum
 import kbputils
 import io
 import shutil
 
 class TrackTableColumn(enum.Enum):
-    KBP = 0
+    KBP_ASS = 0
     Audio = 1
     Background = 2
     Advanced = 3
 
-# TODO: Allow this to be at either the .kbp or .ass stage
-# Possibly pull PlayRes? from .ass to letterbox
+# TODO: Possibly pull PlayRes? from .ass to letterbox
 class KBPASSWrapper:
-    def __init__(self, kbppath):
-        self.kbp_path = kbppath
-        self.kbp_obj = kbputils.KBPFile(kbppath)
+    def __init__(self, path):
+        if path.endswith(".ass"):
+            self.ass_path = path
+        else:
+            self.kbp_path = path
+            self.kbp_obj = kbputils.KBPFile(path)
     def ass_data(self, **kwargs):
-        tmp = io.StringIO()
-        kbputils.AssConverter(self.kbp_obj,**kwargs).ass_document().dump_file(tmp)
-        return tmp.getvalue()
+        if hasattr(self,"kbp_path"):
+            # Re-read file in case it changed on disk
+            self.kbp_obj = kbputils.KBPFile(self.kbp_path)
+
+            tmp = io.StringIO()
+            kbputils.AssConverter(self.kbp_obj,**kwargs).ass_document().dump_file(tmp)
+            return tmp.getvalue()
+        else:
+            # Added for symmetry or something, but...
+            print("Probably shouldn't reach this code")
+            f = QFile(self.ass_path)
+            if not f.open(QIODevice.ReadOnly | QIODevice.Text):                                                                                  
+                raise IOError(f"Unable to open {self.ass_path}")
+            res = QTextStream(f).readAll()
+            f.close()
+            return res
+
     def __str__(self):
-        return self.kbp_path
+        return self.kbp_path if hasattr(self,"kbp_path") else self.ass_path
 
 
 # This should *probably* be redone as a QTableView with a proxy to better
 # manage the data and separate it from display
 class TrackTable(QTableWidget):
 
     def __init__(self, **kwargs):
         super().__init__(0, 4, **kwargs)
         self.setObjectName("tableWidget")
         self.setAcceptDrops(True)
         # If this is enabled, user gets stuck in the widget. Arrow keys can still be used to navigate within it
         self.setTabKeyNavigation(False)
         # TODO: update when support for both is included
         # self.setHorizontalHeaderLabels(["KBP/ASS", "Audio", "Background"])
-        self.setHorizontalHeaderLabels(list(TrackTableColumn.__members__.keys()))
+        self.setHorizontalHeaderLabels([x.replace("_", "/") for x in TrackTableColumn.__members__.keys()])
         self.hideColumn(TrackTableColumn.Advanced.value)
         self.horizontalHeader().setSectionResizeMode(QHeaderView.Stretch)
         self.setDragEnabled(False)
         self.setSortingEnabled(True)
         self.setDragDropMode(QAbstractItemView.DropOnly)
         self.setDefaultDropAction(Qt.CopyAction)
         self.setSelectionMode(QAbstractItemView.ExtendedSelection)
@@ -94,18 +110,20 @@
         else:
             return item.text()
 
     def handle_selection_change(self):
         mainWindow = self.parentWidget().parentWidget().parentWidget()
         if self.selectedRanges() == []:
             mainWindow.removeButton.setEnabled(False)
+            mainWindow.editButton.setEnabled(False)
             mainWindow.advancedButton.setEnabled(False)
             mainWindow.colorApplyButton.setEnabled(False)
         else:
             mainWindow.removeButton.setEnabled(True)
+            mainWindow.editButton.setEnabled(True)
             mainWindow.advancedButton.setEnabled(True)
             mainWindow.colorApplyButton.setEnabled(True)
 
     # TODO: Make user entered and imported work the same way
 
     def key(self, row, column):
         item = self.item(row, column)
@@ -165,14 +183,22 @@
     def add(self, category, file):
         data = getattr(self, category)
         key = FileResultSet.normalize(file)
         if not key in data:
             data[key] = set()
         data[key].add(file)
 
+    # Include both kbp and ass results. If there is any key with both kbp and
+    # ass results, keep only the kbp ones (assuming previous work of kbp2video
+    # that needs redone)
+    def merged_kbp_ass_data(self):
+        data = self.ass.copy()
+        data.update(self.kbp)
+        return data
+
     def normalize(path):
         path = os.path.splitext(os.path.basename(path))[0]
         path = FileResultSet.PATH_REGEX.sub('', path)
         return path.casefold().translate(str.maketrans(
             "", "", string.punctuation + string.whitespace))
 
     def search(self, category, file, fuzziness=0.6):
@@ -263,39 +289,36 @@
                     dir_expand=True,
                     identified=identified)
         return identified
 
     def importFiles(self, data, drop=True):
         mainWindow = self.parentWidget().parentWidget().parentWidget()
         if data and (result := self.generateFileList(data)):
-            # for key, files in list(getattr(result, 'kbp').items()) + list(getattr(result, 'ass').items()):
-            # For now, will assume files will be taken through the whole
-            # process from kbp to video. Will later support going from .ass
-            # file
-            for key, files in result.kbp.items():
+            for key, files in result.merged_kbp_ass_data().items():
+            #for key, files in result.kbp.items():
                 # TODO: handle multiple kbp files under one key
-                kbpFile = next(iter(files))
+                kbpassFile = next(iter(files))
                 table = self.parentWidget().widget(0)
                 current = table.rowCount()
                 table.setRowCount(current + 1)
-                item = QTableWidgetItem(os.path.basename(kbpFile))
-                item.setData(Qt.UserRole, KBPASSWrapper(kbpFile))
-                item.setToolTip(kbpFile)
+                item = QTableWidgetItem(os.path.basename(kbpassFile))
+                item.setData(Qt.UserRole, KBPASSWrapper(kbpassFile))
+                item.setToolTip(kbpassFile)
                 item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
                 table.setItem(current, 0, item)
                 #if not (outputdir := mainWindow.outputDir).text():
                 #    outputdir.setText(os.path.dirname(kbpFile) + "/kbp2video")
-                mainWindow.lastinputdir = os.path.dirname(kbpFile)
+                mainWindow.lastinputdir = os.path.dirname(kbpassFile)
 
                 for filetype, column in (('audio', 1), ('background', 2)):
                     if column == 2 and drop and mainWindow.skipBackgrounds.checkState() == Qt.Checked:
                         continue
                     # Update current in case sort moved it. Needs to be done each time in case one of these columns is the sort field
                     current = table.row(item)
-                    match = result.search(filetype, kbpFile)
+                    match = result.search(filetype, kbpassFile)
 
                     # If there happens to be only one kbp, assume all selected audio/backgrounds were intended for it
                     # Also, if there happens to be only one background, assume
                     # it's for all the KBPs
                     if not match and (len(result.all_files('kbp')) == 1 or (
                             filetype == 'background' and len(getattr(result, 'background')) == 1)):
                         match = result.all_files(filetype)
@@ -304,53 +327,54 @@
                         continue
 
                     print(f"Match found: {match}")
 
                     if len(match) > 1:
                         choice, ok = QInputDialog.getItem(
                             self.parentWidget(), f"Select {filetype} file to use",
-                            f"Multiple potential {filetype} files were found for {kbpFile}. Please select one, or enter a different path.",
+                            f"Multiple potential {filetype} files were found for {kbpassFile}. Please select one, or enter a different path.",
                             match)
                         if ok:
                             match = [choice]
                         else:
                             continue
 
                     match_item = QTableWidgetItem(os.path.basename(match[0]))
                     match_item.setData(Qt.UserRole, match[0])
                     match_item.setToolTip(match[0])
                     match_item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
                     table.setItem(current, column, match_item)
 
                 # Process audio/background options from KBP file
                 current = table.row(item)
-                if isinstance((k := item.data(Qt.UserRole)), KBPASSWrapper):
+                if hasattr((k := item.data(Qt.UserRole)), "kbp_obj"):
                     if not table.item(current, TrackTableColumn.Audio.value).text() and (audio := k.kbp_obj.trackinfo["audio"]):
                         # Audio is either absolute path or relative to kbp
                         audio_path = os.path.join(os.path.dirname(str(k)), audio)
                         audio_item = QTableWidgetItem(os.path.basename(audio_path))
                         audio_item.setData(Qt.UserRole, audio_path)
                         audio_item.setToolTip(audio_path)
                         audio_item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
                         table.setItem(current, TrackTableColumn.Audio.value, audio_item)
                     if not table.item(current, TrackTableColumn.Background.value).text():
                         bg_color = k.kbp_obj.colors.as_rgb24()[0]
                         bg_item = QTableWidgetItem(f"color: #{bg_color}")
                         table.setItem(current, TrackTableColumn.Background.value, bg_item)
 
-        if result.kbp:
+        if result.kbp or result.ass:
             # Ui_MainWindow > QWidget > QStackedWidget > DropLabel
             # TODO: Seems like there should be a better way - maybe pass convertButton to constructor
             mainWindow.convertButton.setEnabled(True)
+            mainWindow.convertAssButton.setEnabled(True)
 
         elif result and (table := self.parentWidget().widget(0)).rowCount() > 0:
             # Try to fill in gaps
             # Need the item itself instead of the row due to potential reordering with sorting
             # TODO: figure out what to do if a kbp file is in the list twice - currently it just updates the last one
-            data = dict((table.key(row, TrackTableColumn.KBP.value), table.item(row, TrackTableColumn.KBP.value)) for row in range(table.rowCount()))
+            data = dict((table.key(row, TrackTableColumn.KBP_ASS.value), table.item(row, TrackTableColumn.KBP_ASS.value)) for row in range(table.rowCount()))
             for filetype, column in (('audio', TrackTableColumn.Audio.value), ('background', TrackTableColumn.Background.value)):
                 if column == TrackTableColumn.Background.value and drop and mainWindow.skipBackgrounds.checkState() == Qt.Checked:
                     continue
                 for key in getattr(result, filetype):
                     if len(filenames := list(getattr(result, filetype)[key])) > 1:
                         choice, ok = QInputDialog.getItem(
                             self.parentWidget(), f"Select {filetype} file to use",
@@ -364,15 +388,15 @@
 
                     search_results = difflib.get_close_matches(key, data, n=3, cutoff=0.6)
 
                     # If just one file was dropped, assume it was intentional and prompt with all the kbps
                     if not search_results and len(result.all_files(filetype)) == 1:
                         search_results = data
 
-                    if match := dict((table.filename(table.indexFromItem(data[key]).row(), TrackTableColumn.KBP.value), data[key]) for key in search_results):
+                    if match := dict((table.filename(table.indexFromItem(data[key]).row(), TrackTableColumn.KBP_ASS.value), data[key]) for key in search_results):
                         if len(match) > 1:
                             choice, ok = QInputDialog.getItem(
                                 self.parentWidget(), "Select KBP file to use",
                                 f"Multiple potential KBP files were found for {filenames[0]}. Please select one or hit cancel to skip.",
                                 match.keys(),
                                 editable=False)
                             if ok:
@@ -388,15 +412,15 @@
                                     "Replace file?",
                                     f"Replace {filetype} file\n{table.item_filename(current)} for\n{fname}\nwith\n{filenames[0]}?",
                                     QMessageBox.StandardButtons(
                                         QMessageBox.Yes | QMessageBox.No))
                                 if answer != QMessageBox.Yes:
                                     continue
                             match_item = QTableWidgetItem(os.path.basename(filenames[0]))
-                            match_item.setData(Qt.UserRole, KBPASSWrapper(filenames[0]) if column == TrackTableColumn.KBP.value else filenames[0])
+                            match_item.setData(Qt.UserRole, KBPASSWrapper(filenames[0]) if column == TrackTableColumn.KBP_ASS.value else filenames[0])
                             match_item.setToolTip(filenames[0])
                             match_item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
                             table.setItem(table.indexFromItem(kbp).row(), column, match_item)
 
         else:
             QMessageBox.information(
                 self.parentWidget(), "No Files Found",
@@ -551,14 +575,20 @@
         self.leftPaneButtons.addWidget(
             self.bind(
                 "addRowButton", QPushButton(
                     clicked=self.add_row_button)))
 
         self.leftPaneButtons.addWidget(
             self.bind(
+                "editButton", QPushButton(
+                    clicked=self.edit_button,
+                    enabled=False))) 
+
+        self.leftPaneButtons.addWidget(
+            self.bind(
                 "advancedButton", QPushButton(
                     clicked=self.advanced_button,
                     enabled=False))) 
 
         self.horizontalLayout.addItem(QSpacerItem(
             20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding))
 
@@ -801,15 +831,17 @@
 
         gridRow += 1
         self.gridLayout.addItem(QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding), gridRow, 0, 1, 3)
         self.gridLayout.setRowStretch(gridRow, 30)
 
         gridRow += 1
         self.gridLayout.addWidget(
-            self.bind("convertButton", QPushButton(enabled=False, clicked=self.runConversion)), gridRow, 0, 1, 3)
+            self.bind("convertAssButton", QPushButton(enabled=False, clicked=self.runAssConversion)), gridRow, 0, 1, 1)
+        self.gridLayout.addWidget(
+            self.bind("convertButton", QPushButton(enabled=False, clicked=self.runConversion)), gridRow, 1, 1, 2)
 
         self.horizontalLayout.addItem(QSpacerItem(
             20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding))
 
         self.loadSettings()
 
         self.retranslateUi()
@@ -879,32 +911,40 @@
                 reverse=True):
             self.tableWidget.setItem(row, TrackTableColumn.Background.value, QTableWidgetItem(
                 f"color: {self.colorText.text()}"))
 
     def advanced_button(self):
         AdvancedEditor.showAdvancedEditor(self.tableWidget)
 
+    def edit_button(self):
+        rows = set(x.row() for x in self.tableWidget.selectedIndexes())
+        if len(rows) == 1 or QMessageBox.question(self, f"Open {len(rows)} files?", f"Are you sure you want to open {len(rows)} files at the same time?") == QMessageBox.Yes:
+            for row in rows:
+                QDesktopServices.openUrl(QUrl.fromLocalFile(self.tableWidget.filename(row, TrackTableColumn.KBP_ASS.value)))
+
     def color_choose_button(self):
         result = QColorDialog.getColor(
             initial=QColor.fromString(self.colorText.text()))
         if result.isValid():
             self.colorText.setText(result.name())
 
     def remove_files_button(self):
         # remove from the end to avoid re-order
         for row in sorted(
                 set(x.row() for x in self.tableWidget.selectedIndexes()),
                 reverse=True):
             self.tableWidget.removeRow(row)
         if self.tableWidget.rowCount() == 0:
             self.convertButton.setEnabled(False)
+            self.convertAssButton.setEnabled(False)
 
     def add_row_button(self):
         self.tableWidget.setRowCount(self.tableWidget.rowCount() + 1)
         self.convertButton.setEnabled(True)
+        self.convertAssButton.setEnabled(True)
 
     def updateColor(self, *_ignored, setColor=None):
         if setColor != None:
             self.colorText.setText(setColor)
         bgcolor = QColor.fromString(self.colorText.text())
         textcolor = "#000000"
         if bgcolor.lightness() <= 128:
@@ -993,26 +1033,38 @@
         self.acodecBox.setCurrentIndex(self.settings.value("video/audio_codec_index", type=int, defaultValue=0))
         self.abitrateBox.setText(self.settings.value("video/audio_bitrate", type=str, defaultValue=""))
         self.relative.setCheckState(bool2check(self.settings.value("kbp2video/relative_path", type=bool, defaultValue=True)))
         self.outputDir.setText(self.settings.value("kbp2video/output_dir", type=str, defaultValue="kbp2video"))
         self.skipBackgrounds.setCheckState(bool2check(self.settings.value("kbp2video/ignore_bg_files_drag_drop", type=bool, defaultValue=False)))
         self.saveSettings()  # Save to disk any new defaults that were used
 
+    def runAssConversion(self):
+        self.saveSettings()
+        converter = Converter(self.conversion_runner, assOnly = True)
+        # worker.signals.finished.connect
+        self.threadpool.start(converter)
+
     def runConversion(self):
         self.saveSettings()
         converter = Converter(self.conversion_runner)
         # worker.signals.finished.connect
         self.threadpool.start(converter)
 
     def resolved_output_dir(self, kbp):
         if check2bool(self.relative):
-            # TODO: check if self.outputDir starts with a slash? Otherwise it behaves like an absolute path
-            return os.path.join(os.path.dirname(kbp), self.outputDir.text())
+
+            # If relative is set, assume .ass dir is the output dir because we
+            # no longer know the project file
+            if kbp.endswith(".ass"):
+                return os.path.dirname(kbp)
+            else:
+                # TODO: check if self.outputDir starts with a slash? Otherwise it behaves like an absolute path
+                return os.path.join(os.path.dirname(kbp), self.outputDir.text())
         else:
-            return self.output_dir()
+            return self.outputDir.text()
     
     def assFile(self, kbp):
         filename = os.path.basename(kbp)
         # This REALLY needs to be set...
         while not check2bool(self.relative) and not self.outputDir.text():
             self.output_dir()
         return self.resolved_output_dir(kbp) + "/" + filename[:-4].translate(str.maketrans("","",":;,'=\"")) + ".ass"
@@ -1060,15 +1112,15 @@
             QMessageBox.StandardButtons(
                 QMessageBox.Yes | QMessageBox.No))
 
     @Slot(str, str)
     def info(self, title, text):
         QMessageBox.information(self, title, text)
 
-    def conversion_runner(self, signals):
+    def conversion_runner(self, signals, assOnly = False):
         unsupported_message = False
         assOptions = ["-f"]
         kbputils_options = {}
         ratio, border = self.get_aspect_ratio()
         if ratio[0] is None or border is None:
             QMetaObject.invokeMethod(
                 self,
@@ -1108,15 +1160,16 @@
         if self.overrideOffset.checkState() == Qt.Checked:
             assOptions += ["-o", f"{self.offset.value()}"]
             kbputils_options['offset'] = self.offset.value()
         if self.transparencyBox.checkState() != Qt.Checked:
             assOptions += ["--no-t"]
             kbputils_options['transparency'] = False
         for row in range(self.tableWidget.rowCount()):
-            kbp_obj = self.tableWidget.item(row, TrackTableColumn.KBP.value).data(Qt.UserRole)
+            kbp_table_item = self.tableWidget.item(row, TrackTableColumn.KBP_ASS.value)
+            kbp_obj = kbp_table_item.data(Qt.UserRole) or kbp_table_item.text()
             kbp = str(kbp_obj)
             audio = self.tableWidget.filename(row, TrackTableColumn.Audio.value)
             background = self.tableWidget.filename(row, TrackTableColumn.Background.value)
             advanced = self.tableWidget.item(row, TrackTableColumn.Advanced.value).data(Qt.UserRole) or {}
             print(f"Retrieved Advanced settings for {kbp}:")
             print(advanced)
             if not kbp:
@@ -1132,69 +1185,86 @@
                 background_type = 1
             elif mimename.startswith('video/'):
                 background_type = 2
             # bad mime type (not image/video or nonexistant file), or no background specified
             if background_type == None:
                 background_type = 0
                 background = default_bg
-            print("kbp2ass " + " ".join(assOptions) + " " + kbp)
-            if isinstance(kbp_obj, KBPASSWrapper):
+
+            assfile = self.assFile(kbp)
+
+            if hasattr(kbp_obj, "kbp_path"):
                 print("Converting the new way")
                 print(kbputils_options)
                 try:
                     data = kbp_obj.ass_data(**kbputils_options)
                 except:
                     QMetaObject.invokeMethod(
                         self,
                         'info', 
                         Qt.AutoConnection,
                         Q_ARG(str, "Failed to process kbp"),
                         Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{' '.join(sys.exc_info())}"))
                     continue
+            elif kbp.endswith(".ass"): # kbp_obj is either a KBPASSWrapper with a .ass file, or a manually entered string with .ass
+                if any(x in kbp for x in ":;,'=\""):
+                    print("Already .ass file, but needs new filename for ffmpeg")
+                    QFile(kbp).copy(assfile)
+                else:
+                    print("Using existing .ass file")
+                    assfile = kbp
                     
             else:
                 print("Falling back to kbp2ass")
+                print("kbp2ass " + " ".join(assOptions) + " " + kbp)
                 q = QProcess(program="kbp2ass", arguments=assOptions+[kbp])
                 q.start()
                 q.waitForFinished(-1)
                 data = q.readAllStandardOutput()
                 if q.exitStatus() != QProcess.NormalExit or data.isEmpty():
                     QMetaObject.invokeMethod(
                         self,
                         'info', 
                         Qt.AutoConnection,
                         Q_ARG(str, "Failed to process kbp"),
                         Q_ARG(str, f"Failed to process .kbp file\n{kbp}\n\nError Output:\n{q.readAllStandardError().toStdString()}"))
                     continue
 
-            assfile = self.assFile(kbp)
-
             # QDir is inconsistent. Needs to be static to check existence, and
             # mkdir needs to be run from an instantiated instance in the parent
             # directory, not worth the hassle
-            if not os.path.isdir(outdir := os.path.dirname(assfile)):
+            if not os.path.isdir(outdir := self.resolved_output_dir(kbp)):
                 os.mkdir(outdir)
 
-            f = QFile(assfile)
-            if f.exists():
-                answer = QMessageBox.StandardButton(QMetaObject.invokeMethod(
-                    self,
-                    'yesno',
-                    Qt.BlockingQueuedConnection,
-                    Q_RETURN_ARG(int),
-                    Q_ARG(str, "Replace file?"),
-                    Q_ARG(str, f"Overwrite {assfile}?")))
-                if answer != QMessageBox.Yes:
+            # File was converted and .ass file needs to be written
+            if kbp.endswith(".kbp"):
+                f = QFile(assfile)
+                if f.exists():
+                    answer = QMessageBox.StandardButton(QMetaObject.invokeMethod(
+                        self,
+                        'yesno',
+                        Qt.BlockingQueuedConnection,
+                        Q_RETURN_ARG(int),
+                        Q_ARG(str, "Replace file?"),
+                        Q_ARG(str, f"Overwrite {assfile}?")))
+                    if answer != QMessageBox.Yes:
+                        continue
+                if not f.open(QIODevice.WriteOnly | QIODevice.Text):
                     continue
-            if not f.open(QIODevice.WriteOnly | QIODevice.Text):
-                continue
-            out = QTextStream(f)
-            out << data
-            f.close()
+                out = QTextStream(f)
+                out << data
+                f.close()
+                if assOnly:
+                    kbp_table_item.setData(Qt.UserRole, KBPASSWrapper(assfile))
+                    kbp_table_item.setText(os.path.basename(assfile))
+                    kbp_table_item.setToolTip(assfile)
+                    kbp_table_item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsEnabled | Qt.ItemNeverHasChildren)
 
+            if assOnly:
+                continue
 
             #ffmpeg_options = ["-y"]
             output_options = {}
             base_assfile = os.path.basename(assfile)
             if background_type == 0:
                 #ffmpeg_options += f"-f lavfi -i color=color={background}:r=60:s={resolution}".split()
                 background_video = ffmpeg.input(f"color=color={background}:r=60:s={resolution}", f="lavfi")
@@ -1332,14 +1402,16 @@
         signals.finished.emit()
 
     def retranslateUi(self):
         self.setWindowTitle(QCoreApplication.translate(
             "MainWindow", "KBP to Video", None))
         self.addButton.setText(QCoreApplication.translate(
             "MainWindow", "&Add Files...", None))
+        self.editButton.setText(QCoreApplication.translate(
+            "MainWindow", "Edit files...", None))
         self.advancedButton.setText(QCoreApplication.translate(
             "MainWindow", "Set Intro&/Outro...", None))
         self.colorChooseButton.setText(QCoreApplication.translate(
             "MainWindow", "C&hoose...", None))
         self.colorChooseButton.setToolTip(QCoreApplication.translate(
             "MainWindow", "Choose a background color with a color picker", None))
         self.colorApplyButton.setText(QCoreApplication.translate(
@@ -1415,15 +1487,17 @@
         self.relativeLabel.setToolTip(QCoreApplication.translate(
             "MainWindow", "Interpret Output Folder as a relative path from your .kbp file.\nE.g. leave it blank to have it in the same folder as your .kbp.", None))
         self.outputDirButton.setText(QCoreApplication.translate(
             "MainWindow", "Bro&wse...", None))
         self.resetButton.setText(QCoreApplication.translate(
             "MainWindow", "Reset Settings&...", None))
         self.convertButton.setText(QCoreApplication.translate(
-            "MainWindow", "&Convert", None))
+            "MainWindow", "&Convert to Video", None))
+        self.convertAssButton.setText(QCoreApplication.translate(
+            "MainWindow", "Subtitle onl&y", None))
     # retranslateUi
 
 
 def run(argv=sys.argv, ffmpeg_path=None):
     # Look better on Windows
     QApplication.setStyle("Fusion")
     app = QApplication(argv)
```

### Comparing `kbp2video-0.1.0/kbp2video/advanced_editor.py` & `kbp2video-0.1.1/kbp2video/advanced_editor.py`

 * *Files identical despite different names*

### Comparing `kbp2video-0.1.0/kbp2video/utils.py` & `kbp2video-0.1.1/kbp2video/utils.py`

 * *Files identical despite different names*

