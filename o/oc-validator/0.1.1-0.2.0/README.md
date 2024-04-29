# Comparing `tmp/oc_validator-0.1.1.tar.gz` & `tmp/oc_validator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_validator-0.1.1.tar", max compression
+gzip compressed data, was "oc_validator-0.2.0.tar", max compression
```

## Comparing `oc_validator-0.1.1.tar` & `oc_validator-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      797 2023-03-11 16:50:32.462808 oc_validator-0.1.1/oc_validator/__init__.py
--rw-r--r--   0        0        0    22216 2023-03-11 16:12:45.708000 oc_validator-0.1.1/oc_validator/csv_wellformedness.py
--rw-r--r--   0        0        0     6435 2023-03-10 23:16:12.229000 oc_validator-0.1.1/oc_validator/helper.py
--rw-r--r--   0        0        0     2974 2023-03-10 23:16:12.216000 oc_validator-0.1.1/oc_validator/id_existence.py
--rw-r--r--   0        0        0     2545 2023-03-10 23:16:12.234000 oc_validator-0.1.1/oc_validator/id_syntax.py
--rw-r--r--   0        0        0     1837 2023-02-01 23:52:18.462000 oc_validator-0.1.1/oc_validator/id_type_alignment.json
--rw-r--r--   0        0        0    38800 2023-03-11 16:12:45.768000 oc_validator-0.1.1/oc_validator/main.py
--rw-r--r--   0        0        0     5797 2023-03-11 15:09:21.793000 oc_validator-0.1.1/oc_validator/messages.yaml
--rw-r--r--   0        0        0     1906 2023-03-10 23:18:13.073000 oc_validator-0.1.1/oc_validator/semantics.py
--rw-r--r--   0        0        0      623 2023-03-12 10:38:57.765957 oc_validator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1856 2023-03-12 09:47:48.977956 oc_validator-0.1.1/README.md
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 oc_validator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-01-23 18:11:55.346907 oc_validator-0.2.0/oc_validator/__init__.py
+-rw-r--r--   0        0        0    21222 2024-04-09 16:12:58.831239 oc_validator-0.2.0/oc_validator/csv_wellformedness.py
+-rw-r--r--   0        0        0     6435 2024-01-23 18:11:55.351908 oc_validator-0.2.0/oc_validator/helper.py
+-rw-r--r--   0        0        0     5654 2024-04-03 14:45:13.962545 oc_validator-0.2.0/oc_validator/id_existence.py
+-rw-r--r--   0        0        0     2975 2024-04-03 14:45:13.962545 oc_validator-0.2.0/oc_validator/id_syntax.py
+-rw-r--r--   0        0        0     5259 2024-03-18 13:57:31.276651 oc_validator-0.2.0/oc_validator/id_type_alignment.json
+-rw-r--r--   0        0        0    45376 2024-03-28 14:09:28.851098 oc_validator-0.2.0/oc_validator/main.py
+-rw-r--r--   0        0        0     5823 2024-03-06 17:05:18.324799 oc_validator-0.2.0/oc_validator/messages.yaml
+-rw-r--r--   0        0        0     1906 2024-01-23 18:11:55.353911 oc_validator-0.2.0/oc_validator/semantics.py
+-rw-r--r--   0        0        0      624 2024-04-24 16:32:09.756696 oc_validator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1856 2024-01-23 18:11:55.345908 oc_validator-0.2.0/README.md
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 oc_validator-0.2.0/PKG-INFO
```

### Comparing `oc_validator-0.1.1/oc_validator/__init__.py` & `oc_validator-0.2.0/oc_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_validator-0.1.1/oc_validator/csv_wellformedness.py` & `oc_validator-0.2.0/oc_validator/csv_wellformedness.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 
 from re import match, search, sub
 from roman import fromRoman, InvalidRomanNumeralError
 from oc_validator.helper import Helper
+from json import load
 
 
 class Wellformedness:
     def __init__(self):
-        self.descr = 'This class groups the function for validating the well-formedness of the document.'  # todo: remove descr?
         self.helper = Helper()
+        self.br_id_schemes = ['doi', 'issn', 'isbn', 'pmid', 'pmcid', 'url', 'wikidata', 'wikipedia', 'openalex']
+        self.ra_id_schemes = ['crossref', 'orcid', 'viaf', 'wikidata', 'ror']
+        self.id_type_dict: dict = load(open('oc_validator/id_type_alignment.json', 'r', encoding='utf-8'))
 
     def wellformedness_br_id(self, id_element):
         """
         Validates the well-formedness of a single element inside the 'citing_id', 'cited_id' or 'id' field of a row,
         checking its compliance with CITS-csv/META-CSV syntax.
         :param id_element: str
         :return: bool
         """
-        id_pattern = r'^(doi|issn|isbn|pmid|pmcid|url|wikidata|wikipedia):\S+$'
+        id_pattern = fr'^({"|".join(self.br_id_schemes)}):\S+$'
         if match(id_pattern, id_element):
             return True
         else:
             return False
 
     def wellformedness_people_item(self, ra_item: str):
         """
@@ -41,32 +44,32 @@
         checking its compliance with META-CSV syntax.
         :param ra_item: str
         :return: bool
         """
         #  todo: create stricter regex for not allowing characters that are likely to be illegal in a person's name/surname
         #   (e.g. digits, apostrophe, underscore, full-stop, etc.)
         outside_brackets = r'(?:[^\s,;\[\]]+(?:\s[^\s,;\[\]]+)*),?(?:\s[^\s,;\[\]]+)*'
-        inside_brackets = r'\[(crossref|orcid|viaf|wikidata|ror):\S+(?:\s(crossref|orcid|viaf|wikidata|ror):\S+)*\]'
-        ra_item_pattern = f'^(?:({outside_brackets}\\s{inside_brackets})|({outside_brackets}\\s?)|({inside_brackets}))$'
+        inside_brackets = fr'\[({"|".join(self.ra_id_schemes)}):\S+(?:\s({"|".join(self.ra_id_schemes)}):\S+)*\]'
+        ra_item_pattern = fr'^(?:({outside_brackets}\s{inside_brackets})|({outside_brackets}\s?)|({inside_brackets}))$'
 
         if match(ra_item_pattern, ra_item):
             return True
         else:
             return False
 
     def wellformedness_publisher_item(self, ra_item: str):
         """
         Validates the well-formedness of an item inside the 'publisher' field of a row,
         checking its compliance with META-CSV syntax.
         :param ra_item: str
         :return: bool
         """
         outside_brackets_pub = r'(?:[^\s\[\]]+(?:\s[^\s\[\]]+)*)'
-        inside_brackets = r'\[(crossref|orcid|viaf|wikidata|ror):\S+(?:\s(crossref|orcid|viaf|wikidata|ror):\S+)*\]'
-        ra_item_pattern = f'^(?:({outside_brackets_pub}\\s{inside_brackets})|({outside_brackets_pub}\\s?)|({inside_brackets}))$'
+        inside_brackets = fr'\[({"|".join(self.ra_id_schemes)}):\S+(?:\s({"|".join(self.ra_id_schemes)}):\S+)*\]'
+        ra_item_pattern = fr'^(?:({outside_brackets_pub}\s{inside_brackets})|({outside_brackets_pub}\s?)|({inside_brackets}))$'
 
         if match(ra_item_pattern, ra_item):
             return True
         else:
             return False
 
     def orphan_ra_id(self, ra_item: str):
@@ -74,15 +77,15 @@
         Looks for possible ID of responsible agents ('author', 'publisher' or 'editor') that are NOT enclosed in
         brackets, as they should be. Returns True if the input string is likely to contain one or more R.A. ID outside
         square brackets.
         :param ra_item: the item inside a R.A. field, as it is split by the '; ' separator.
         :return:
         bool, True if a match is found (the string is likely NOT well-formed), False if NO match is found.
         """
-        if search(r'(crossref|orcid|viaf|wikidata|ror):', sub(r'\[.*\]', '', ra_item)):
+        if search(fr'({"|".join(self.ra_id_schemes)}):', sub(r'\[.*\]', '', ra_item)):
             return True
         else:
             return False
 
     def wellformedness_date(self, date_field):
         """
         Validates the well-formedness of the content of the 'citing_publication_date', 'cited_publication_date'
@@ -101,31 +104,31 @@
         Validates the well-formedness of the string inside the 'venue' field of a row,
         checking its compliance with META-CSV syntax.
         :param venue_value: str
         :return: bool
         """
         outside_brackets_venue = r'(?:[^\s\[\]]+(?:\s[^\s\[\]]+)*)'
         # pmcids are not valid identifiers for 'venues'!
-        inside_brackets_venue = r'\[(doi|pmid|issn|isbn|url|wikidata|wikipedia):\S+(?:\s(doi|pmid|issn|isbn|url|wikidata|wikipedia):\S+)*\]'
-        venue_pattern = f'^(?:({outside_brackets_venue}\\s{inside_brackets_venue})|({outside_brackets_venue}\\s?)|({inside_brackets_venue}))$'
+        inside_brackets_venue = fr'\[({"|".join(self.br_id_schemes)}):\S+(?:\s({"|".join(self.br_id_schemes)}):\S+)*\]'
+        venue_pattern = fr'^(?:({outside_brackets_venue}\s{inside_brackets_venue})|({outside_brackets_venue}\s?)|({inside_brackets_venue}))$'
 
         if match(venue_pattern, venue_value):
             return True
         else:
             return False
 
     def orphan_venue_id(self, venue_value: str):
         """
         Looks for IDs of BRs that might be a venue but are NOT enclosed in brackets, as they should be. Returns True if the
         input string is likely to contain one or more BR ID outside square brackets.
         :param venue_value: the value of the 'venue' field of a row.
         :return:
         bool, True if a match is found (the string is likely NOT well-formed), False if NO match is found.
         """
-        if search(r'(doi|pmid|issn|isbn|url|wikidata|wikipedia):', sub(r'\[.*\]', '', venue_value)):
+        if search(fr'({"|".join(self.br_id_schemes)}):', sub(r'\[.*\]', '', venue_value)):
             return True
         else:
             return False
 
     def wellformedness_volume_issue(self, vi_value: str):
         """
         Validates the well-formedness of the string inside the 'volume' or 'issue' field of a row,
@@ -189,21 +192,16 @@
     def wellformedness_type(self, type_value: str):
         """
         Validates the well-formedness of the string inside the 'type' field of a row,
         checking its compliance with META-CSV syntax.
         :param type_value: str
         :return: bool
         """
-        valid_types = ['book', 'book chapter', 'book part', 'book section', 'book series', 'book set', 'book track',
-                       'component', 'dataset', 'data file', 'dissertation', 'edited book', 'journal', 'journal article',
-                       'journal issue', 'journal volume', 'monograph', 'other', 'peer review', 'posted content',
-                       'web content', 'proceedings', 'proceedings article', 'proceedings series', 'reference book',
-                       'reference entry', 'report', 'report series', 'series' 'standard', 'standard series']
 
-        if type_value in valid_types:
+        if type_value in self.id_type_dict.keys():
             return True
         else:
             return False
 
     def get_missing_values(self, row: dict) -> dict:
         """
         Checks whether a row has all required fields, depending on the specified 'type' of the resource, in case the
@@ -219,15 +217,15 @@
         #  of accepted types might change/be extended frequently!
 
         missing = {}
         if not row['id']:  # ID value is missing
 
             if row['type']:  # ID is missing and 'type' is specified
 
-                if row['type'] in ['book', 'dataset', 'data file', 'dissertation', 'edited book', 'journal',
+                if row['type'] in ['book', 'dataset', 'data file', 'dissertation', 'edited book',
                                    'journal article', 'monograph', 'other', 'peer review', 'posted content',
                                    'web content', 'proceedings article', 'reference book', 'report']:
                     if not row['title']:
                         missing['type'] = [0]
                         missing['title'] = None
                     if not row['pub_date']:
                         missing['type'] = [0]
@@ -287,36 +285,25 @@
                 if not row['author'] and not row['editor']:
                     missing['type'] = None
                     if not row['author']:
                         missing['author'] = None
                     if not row['editor']:
                         missing['editor'] = None
 
-        if row['id']:
-            if row['volume']:
-                if not row['venue']:
-                    missing['volume'] = [0]
-                    missing['venue'] = None
-                if row['type'] not in ['journal article', 'journal volume', 'journal issue']:
-                    missing['volume'] = [0]
-                    if not row['type']:
-                        missing['type'] = None
-                    else:
-                        missing['type'] = [0]
+        # the 2 conditions below apply to any type of BR and regardless of an ID being specified
+        # cfr. also docs/mandatory_fields.csv
+
+        if row['volume'] and not row['venue']:
+            missing['volume'] = [0]
+            missing['venue'] = None
+
+        if row['issue'] and not row['venue']:
+            missing['issue'] = [0]
+            missing['venue'] = None
 
-            if row['issue']:
-                if not row['venue']:
-                    missing['issue'] = [0]
-                    missing['venue'] = None
-                if row['type'] not in ['journal article', 'journal volume', 'journal issue']:
-                    missing['issue'] = [0]
-                    if not row['type']:
-                        missing['type'] = None
-                    else:
-                        missing['type'] = [0]
 
         return missing
 
     def get_duplicates_cits(self, entities: list, data_dict: list, messages) -> list:
         """
         Creates a list of dictionaries containing the duplication error in the whole document, either within a row
         (self-citation) or between two or more rows (duplicate citations).
```

### Comparing `oc_validator-0.1.1/oc_validator/helper.py` & `oc_validator-0.2.0/oc_validator/helper.py`

 * *Files identical despite different names*

### Comparing `oc_validator-0.1.1/oc_validator/main.py` & `oc_validator-0.2.0/oc_validator/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,43 +23,44 @@
 from oc_validator.id_syntax import IdSyntax
 from oc_validator.id_existence import IdExistence
 from oc_validator.semantics import Semantics
 from argparse import ArgumentParser
 
 
 class Validator:
-    def __init__(self, csv_doc: str, output_dir: str):
+    def __init__(self, csv_doc: str, output_dir: str, use_meta_endpoint=False):
         self.data = self.read_csv(csv_doc)
         self.table_to_process = self.process_selector(self.data)
         self.helper = Helper()
         self.wellformed = Wellformedness()
         self.syntax = IdSyntax()
-        self.existence = IdExistence()
+        self.existence = IdExistence(use_meta_endpoint=use_meta_endpoint)
         self.semantics = Semantics()
         self.messages = full_load(open('oc_validator/messages.yaml', 'r', encoding='utf-8'))
         # self.messages = full_load(open(join(dirname(__file__), 'messages.yaml'), 'r', encoding='utf-8'))
         self.id_type_dict = load(
             open('oc_validator/id_type_alignment.json', 'r', encoding='utf-8'))  # for ID-type alignment (semantics)
         self.output_dir = output_dir
         if not exists(self.output_dir):
             makedirs(self.output_dir)
+        self.visited_ids = dict()
 
     def read_csv(self, csv_doc):
         with open(csv_doc, 'r', encoding='utf-8') as f:
             data_dict = list(DictReader(f))
             return data_dict
 
     def process_selector(self, data: list):
         process_type = None
         try:
-            if all(list(row.keys()) == ["id", "title", "author", "pub_date", "venue", "volume", "issue", "page", "type",
-                                        "publisher", "editor"] for row in data):
+            if all(set(row.keys()) == {"id", "title", "author", "pub_date", "venue", "volume", "issue", "page", "type",
+                                        "publisher", "editor"} for row in data):
                 process_type = 'meta_csv'
                 return process_type
-            elif all(list(row.keys()) == ['citing_id', 'citing_publication_date', 'cited_id', 'cited_publication_date']
+            elif all(set(row.keys()) == {'citing_id', 'citing_publication_date', 'cited_id', 'cited_publication_date'}
                      for row in
                      data):
                 process_type = 'cits_csv'
                 return process_type
             else:
                 return process_type
         except KeyError:
@@ -160,24 +161,37 @@
                                         self.helper.create_error_dict(validation_level='external_syntax',
                                                                       error_type='error',
                                                                       message=message,
                                                                       error_label='br_id_syntax',
                                                                       located_in='item',
                                                                       table=table))
                                 #  3rd validation level: EXISTENCE OF ID (BIBLIOGRAPHIC RESOURCE)
-                                elif not self.existence.check_id_existence(item):
+                                else:
                                     message = messages['m20']
                                     table = {row_idx: {field: [item_idx]}}
-                                    error_final_report.append(
-                                        self.helper.create_error_dict(validation_level='existence',
-                                                                      error_type='warning',
-                                                                      message=message,
-                                                                      error_label='br_id_existence',
-                                                                      located_in='item',
-                                                                      table=table, valid=True))
+                                    if item not in self.visited_ids:
+                                        if not self.existence.check_id_existence(item):
+                                            error_final_report.append(
+                                                self.helper.create_error_dict(validation_level='existence',
+                                                                              error_type='warning',
+                                                                              message=message,
+                                                                              error_label='br_id_existence',
+                                                                              located_in='item',
+                                                                              table=table, valid=True))
+                                            self.visited_ids[item] = False
+                                        else:
+                                            self.visited_ids[item] = True
+                                    elif self.visited_ids[item] is False:
+                                        error_final_report.append(
+                                            self.helper.create_error_dict(validation_level='existence',
+                                                                          error_type='warning',
+                                                                          message=message,
+                                                                          error_label='br_id_existence',
+                                                                          located_in='item',
+                                                                          table=table, valid=True))
 
                         if len(br_ids_set) >= 1:
                             br_id_groups.append(br_ids_set)
 
                         if len(br_ids_set) != len(items):  # --> some well-formedness error occurred in the id field
                             id_ok = False
 
@@ -237,25 +251,39 @@
                                             self.helper.create_error_dict(validation_level='external_syntax',
                                                                           error_type='error',
                                                                           message=message,
                                                                           error_label='ra_id_syntax',
                                                                           located_in='item',
                                                                           table=table))
                                     #  3rd validation level: EXISTENCE OF ID (RESPONSIBLE AGENT)
-                                    elif not self.existence.check_id_existence(id):
+                                    else:
                                         message = messages['m22']
                                         table = {row_idx: {field: [item_idx]}}
-                                        error_final_report.append(
-                                            self.helper.create_error_dict(validation_level='existence',
-                                                                          error_type='warning',
-                                                                          message=message,
-                                                                          error_label='ra_id_existence',
-                                                                          located_in='item',
-                                                                          table=table,
-                                                                          valid=True))
+                                        if id not in self.visited_ids:
+                                            if not self.existence.check_id_existence(id):
+                                                error_final_report.append(
+                                                    self.helper.create_error_dict(validation_level='existence',
+                                                                                  error_type='warning',
+                                                                                  message=message,
+                                                                                  error_label='ra_id_existence',
+                                                                                  located_in='item',
+                                                                                  table=table,
+                                                                                  valid=True))
+                                                self.visited_ids[id] = False
+                                            else:
+                                                self.visited_ids[id] = True
+                                        elif self.visited_ids[id] is False:
+                                            error_final_report.append(
+                                                self.helper.create_error_dict(validation_level='existence',
+                                                                              error_type='warning',
+                                                                              message=message,
+                                                                              error_label='ra_id_existence',
+                                                                              located_in='item',
+                                                                              table=table,
+                                                                              valid=True))
                 if field == 'pub_date':
                     if value:
                         if not self.wellformed.wellformedness_date(value):
                             message = messages['m3']
                             table = {row_idx: {field: [0]}}
                             error_final_report.append(
                                 self.helper.create_error_dict(validation_level='csv_wellformedness',
@@ -289,15 +317,15 @@
                                                               message=message,
                                                               error_label='venue_format',
                                                               located_in='item',
                                                               table=table))
 
                         else:
                             ids = [m.group() for m in
-                                   finditer(r'((?:doi|issn|isbn|url|wikidata|wikipedia):\S+)(?=\s|\])', value)]
+                                   finditer(r'((?:doi|issn|isbn|url|wikidata|wikipedia|openalex):\S+)(?=\s|\])', value)]
 
                             for id in ids:
 
                                 #  2nd validation level: EXTERNAL SYNTAX OF ID (BIBLIOGRAPHIC RESOURCE)
                                 if not self.syntax.check_id_syntax(id):
                                     message = messages['m19']
                                     table = {row_idx: {field: [0]}}
@@ -305,25 +333,40 @@
                                         self.helper.create_error_dict(validation_level='external_syntax',
                                                                       error_type='error',
                                                                       message=message,
                                                                       error_label='br_id_syntax',
                                                                       located_in='item',
                                                                       table=table))
                                 #  3rd validation level: EXISTENCE OF ID (BIBLIOGRAPHIC RESOURCE)
-                                elif not self.existence.check_id_existence(id):
+                                else:
                                     message = messages['m20']
                                     table = {row_idx: {field: [0]}}
-                                    error_final_report.append(
-                                        self.helper.create_error_dict(validation_level='existence',
-                                                                      error_type='warning',
-                                                                      message=message,
-                                                                      error_label='br_id_existence',
-                                                                      located_in='item',
-                                                                      table=table,
-                                                                      valid=True))
+                                    if id not in self.visited_ids:
+                                        if not self.existence.check_id_existence(id):
+                                            error_final_report.append(
+                                                self.helper.create_error_dict(validation_level='existence',
+                                                                              error_type='warning',
+                                                                              message=message,
+                                                                              error_label='br_id_existence',
+                                                                              located_in='item',
+                                                                              table=table,
+                                                                              valid=True))
+                                            self.visited_ids[id] = False
+                                        else:
+                                            self.visited_ids[id] = True
+                                    elif self.visited_ids[id] is False:
+                                        error_final_report.append(
+                                            self.helper.create_error_dict(validation_level='existence',
+                                                                          error_type='warning',
+                                                                          message=message,
+                                                                          error_label='br_id_existence',
+                                                                          located_in='item',
+                                                                          table=table,
+                                                                          valid=True))
+
                 if field == 'volume':
                     if value:
                         if not self.wellformed.wellformedness_volume_issue(value):
                             message = messages['m13']
                             table = {row_idx: {field: [0]}}
                             error_final_report.append(
                                 self.helper.create_error_dict(validation_level='csv_wellformedness',
@@ -384,65 +427,82 @@
                                                               located_in='item',
                                                               table=table))
 
                             type_ok = False
 
                 if field == 'publisher':
                     if value:
-                        if self.wellformed.orphan_ra_id(value):
-                            message = messages['m10']
-                            table = {row_idx: {field: [0]}}
-                            error_final_report.append(
-                                self.helper.create_error_dict(validation_level='csv_wellformedness',
-                                                              error_type='warning',
-                                                              message=message,
-                                                              error_label='orphan_ra_id',
-                                                              located_in='item',
-                                                              table=table,
-                                                              valid=True))
+                        items = value.split('; ')
+                        for item_idx, item in enumerate(items):
+                            if self.wellformed.orphan_ra_id(value):
+                                message = messages['m10']
+                                table = {row_idx: {field: [item_idx]}}
+                                error_final_report.append(
+                                    self.helper.create_error_dict(validation_level='csv_wellformedness',
+                                                                  error_type='warning',
+                                                                  message=message,
+                                                                  error_label='orphan_ra_id',
+                                                                  located_in='item',
+                                                                  table=table,
+                                                                  valid=True))
 
-                        if not self.wellformed.wellformedness_publisher_item(value):
-                            message = messages['m9']
-                            table = {row_idx: {field: [0]}}
-                            error_final_report.append(
-                                self.helper.create_error_dict(validation_level='csv_wellformedness',
-                                                              error_type='error',
-                                                              message=message,
-                                                              error_label='publisher_format',
-                                                              located_in='item',
-                                                              table=table))
+                            if not self.wellformed.wellformedness_publisher_item(value):
+                                message = messages['m9']
+                                table = {row_idx: {field: [item_idx]}}
+                                error_final_report.append(
+                                    self.helper.create_error_dict(validation_level='csv_wellformedness',
+                                                                  error_type='error',
+                                                                  message=message,
+                                                                  error_label='publisher_format',
+                                                                  located_in='item',
+                                                                  table=table))
 
-                        else:
-                            ids = [m.group() for m in
-                                   finditer(r'((?:crossref|orcid|viaf|wikidata|ror):\S+)(?=\s|\])', value)]
+                            else:
+                                ids = [m.group() for m in
+                                       finditer(r'((?:crossref|orcid|viaf|wikidata|ror):\S+)(?=\s|\])', value)]
 
-                            for id in ids:
+                                for id in ids:
 
-                                #  2nd validation level: EXTERNAL SYNTAX OF ID (RESPONSIBLE AGENT)
-                                if not self.syntax.check_id_syntax(id):
-                                    message = messages['m21']
-                                    table = {row_idx: {field: [0]}}
-                                    error_final_report.append(
-                                        self.helper.create_error_dict(validation_level='external_syntax',
-                                                                      error_type='error',
-                                                                      message=message,
-                                                                      error_label='ra_id_syntax',
-                                                                      located_in='item',
-                                                                      table=table))
-                                #  3rd validation level: EXISTENCE OF ID (RESPONSIBLE AGENT)
-                                elif not self.existence.check_id_existence(id):
-                                    message = messages['m22']
-                                    table = {row_idx: {field: [0]}}
-                                    error_final_report.append(
-                                        self.helper.create_error_dict(validation_level='existence',
-                                                                      error_type='warning',
-                                                                      message=message,
-                                                                      error_label='ra_id_existence',
-                                                                      located_in='item',
-                                                                      table=table, valid=True))
+                                    #  2nd validation level: EXTERNAL SYNTAX OF ID (RESPONSIBLE AGENT)
+                                    if not self.syntax.check_id_syntax(id):
+                                        message = messages['m21']
+                                        table = {row_idx: {field: [item_idx]}}
+                                        error_final_report.append(
+                                            self.helper.create_error_dict(validation_level='external_syntax',
+                                                                          error_type='error',
+                                                                          message=message,
+                                                                          error_label='ra_id_syntax',
+                                                                          located_in='item',
+                                                                          table=table))
+                                    #  3rd validation level: EXISTENCE OF ID (RESPONSIBLE AGENT)
+                                    else:
+                                        message = messages['m22']
+                                        table = {row_idx: {field: [item_idx]}}
+                                        if id not in self.visited_ids:
+                                            if not self.existence.check_id_existence(id):
+                                                error_final_report.append(
+                                                    self.helper.create_error_dict(validation_level='existence',
+                                                                                  error_type='warning',
+                                                                                  message=message,
+                                                                                  error_label='ra_id_existence',
+                                                                                  located_in='item',
+                                                                                  table=table,
+                                                                                  valid=True))
+                                                self.visited_ids[id] = False
+                                            else:
+                                                self.visited_ids[id] = True
+                                        elif self.visited_ids[id] is False:
+                                            error_final_report.append(
+                                                self.helper.create_error_dict(validation_level='existence',
+                                                                              error_type='warning',
+                                                                              message=message,
+                                                                              error_label='ra_id_existence',
+                                                                              located_in='item',
+                                                                              table=table,
+                                                                              valid=True))
 
             if row_ok and id_ok and type_ok:  # row semantics is checked only when the involved parts are well-formed
 
                 invalid_semantics = self.semantics.check_semantics(row, id_type_dict)
                 if invalid_semantics:
                     message = messages['m23']
                     table = {row_idx: invalid_semantics}
@@ -552,25 +612,37 @@
                                         self.helper.create_error_dict(validation_level='external_syntax',
                                                                       error_type='error',
                                                                       message=message,
                                                                       error_label='br_id_syntax',
                                                                       located_in='item',
                                                                       table=table))
                                 #  3rd validation level: EXISTENCE OF ID (BIBLIOGRAPHIC RESOURCE)
-                                elif not self.existence.check_id_existence(item):
+                                else:
                                     message = messages['m20']
                                     table = {row_idx: {field: [item_idx]}}
-                                    error_final_report.append(
-                                        self.helper.create_error_dict(validation_level='existence',
-                                                                      error_type='warning',
-                                                                      message=message,
-                                                                      error_label='br_id_existence',
-                                                                      located_in='item',
-                                                                      table=table,
-                                                                      valid=True))
+                                    if item not in self.visited_ids:
+                                        if not self.existence.check_id_existence(item):
+                                            error_final_report.append(
+                                                self.helper.create_error_dict(validation_level='existence',
+                                                                              error_type='warning',
+                                                                              message=message,
+                                                                              error_label='br_id_existence',
+                                                                              located_in='item',
+                                                                              table=table, valid=True))
+                                            self.visited_ids[item] = False
+                                        else:
+                                            self.visited_ids[item] = True
+                                    elif self.visited_ids[item] is False:
+                                        error_final_report.append(
+                                            self.helper.create_error_dict(validation_level='existence',
+                                                                          error_type='warning',
+                                                                          message=message,
+                                                                          error_label='br_id_existence',
+                                                                          located_in='item',
+                                                                          table=table, valid=True))
 
                         if len(ids_set) >= 1:
                             id_fields_instances.append(ids_set)
 
                 if field == 'citing_publication_date' or field == 'cited_publication_date':
                     if value:
                         if not self.wellformed.wellformedness_date(value):
@@ -607,18 +679,20 @@
 
 if __name__ == '__main__':
     parser = ArgumentParser()
     parser.add_argument('-i', '--input', dest='input_csv', required=True,
                         help='The path to the CSV document to validate.', type=str)
     parser.add_argument('-o', '--output', dest='output_dir', required=True,
                         help='The path to the directory where to store the output JSON file.', type=str)
+    parser.add_argument('-m', '--use-meta', dest='use_meta_endpoint', action='store_true',
+                        help='Use the OC Meta endpoint to check if an ID exists.', required=False)
     args = parser.parse_args()
-    v = Validator(args.input_csv, args.output_dir)
+    v = Validator(args.input_csv, args.output_dir, args.use_meta_endpoint)
     v.validate()
 
 # to instantiate the class, write:
-# v = Validator('path/to/csv/file', 'output/dir/path')
+# v = Validator('path/to/csv/file', 'output/dir/path') # optionally set use_meta_endpoint to True
 # v.validate() --> validates, returns the output, and saves files
 
 
 # FROM THE COMMAND LINE:
-# python -m oc_validator.main -i <input csv file path> -o <output dir path>
+# python -m oc_validator.main -i <input csv file path> -o <output dir path> [-m]
```

### Comparing `oc_validator-0.1.1/oc_validator/messages.yaml` & `oc_validator-0.2.0/oc_validator/messages.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
   by one single space character (Unicode Character “SPACE”, U+0020). Each ID must not have spaces within 
   itself, and must be of the following form: <ID abbreviation> + “:” + <ID value>.
 
 m2: >
   The value in this field is not expressed in compliance with the syntax of OpenCitations CITS-CSV. 
   Each identifier in 'citing_id' and/or 'cited_id' must have the following form: ID abbreviation + “:” + ID value.
   No spaces are admitted within the ID. Example: doi:10.48550/arXiv.2206.03971. The accepted prefixes 
-  (ID abbreviations) are the following: 'doi', 'issn', 'isbn', 'pmid', 'pmcid', 'url', 'wikidata', 'wikipedia'.
+  (ID abbreviations) are the following: 'doi', 'issn', 'isbn', 'pmid', 'pmcid', 'url', 'wikidata', 'wikipedia', 
+  'openalex'.
 
 m3: >
   The value in this field is not expressed in compliance with the syntax of OpenCitations CITS-CSV. 
   The content of 'citing_publication_date' and/or 'cited_publication_date' must be of one of the following 
   forms (according to standard ISO 86014): YYYY-MM-DD, YYYY-MM, YYYY. If year is required, month and day 
   are optional. If the day is expressed, the day must also be expressed. Examples: '2000'; '2000-04'; '2000-04-27'.
 
@@ -50,15 +51,15 @@
   The same bibliographic resource is being represented in more than one row. Please check all the rows involved in 
   the representation of this publication and unify them or remove the extra ones.
 
 m12: >
   The value representing the bibliographic resource entity is not well-formed. The entity for a bibliographic resource
   is represented by the name of the publication, followed by a single whitespace and one or 
   more associated identifiers, always enclosed in square brackets (among the following schemes: doi, wikipedia, 
-  wikidata, pmid, pmcid, url, issn and isbn). Common mistakes: two or more consecutive whitespace characters; 
+  wikidata, pmid, pmcid, url, issn, isbn and openalex). Common mistakes: two or more consecutive whitespace characters; 
   unsupported ID schemes; whitespace character separating the prefix and the ID value.
 
 m13: >
   The value for 'issue'/'volume' is not well-formed. Likely cause of error might be the presence of (an) extra 
   whitespace character(s).
 
 m14: >
```

### Comparing `oc_validator-0.1.1/oc_validator/semantics.py` & `oc_validator-0.2.0/oc_validator/semantics.py`

 * *Files identical despite different names*

### Comparing `oc_validator-0.1.1/README.md` & `oc_validator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oc_validator-0.1.1/PKG-INFO` & `oc_validator-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: oc-validator
-Version: 0.1.1
+Version: 0.2.0
 Summary: A software to validate CSV documents storing citation data and bibliographic metadata according to the OpenCitations Data Model.
 Author: Elia Rizzetto
 Author-email: elia.rizzetto@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: oc-idmanager (>=0.2.6,<0.3.0)
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: roman (>=4.0,<5.0)
+Requires-Dist: sparqlwrapper (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # oc_validator
 
 **oc_validator** is a Python (≥3.9) library to validate CSV documents storing citation data and bibliographic metadata.
 To be processed by the validator, the tables must be built as either CITS-CSV or META-CSV tables, defined in two
 specification documents[^1][^2].
```

