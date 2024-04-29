# Comparing `tmp/librus_apix-0.7.2.tar.gz` & `tmp/librus_apix-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.2.tar", last modified: Sat Apr 27 12:51:02 2024, max compression
+gzip compressed data, was "librus_apix-0.7.3.tar", last modified: Mon Apr 29 07:53:49 2024, max compression
```

## Comparing `librus_apix-0.7.2.tar` & `librus_apix-0.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.499705 librus_apix-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-27 12:50:55.000000 librus_apix-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 12:51:02.499705 librus_apix-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-27 12:50:55.000000 librus_apix-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.495705 librus_apix-0.7.2/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-27 12:50:55.000000 librus_apix-0.7.2/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:51:02.495705 librus_apix-0.7.2/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 12:51:02.000000 librus_apix-0.7.2/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 12:50:55.000000 librus_apix-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-27 12:51:02.499705 librus_apix-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 12:50:55.000000 librus_apix-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.473608 librus_apix-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:53:47.000000 librus_apix-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 07:53:49.473608 librus_apix-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-29 07:53:47.000000 librus_apix-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.469608 librus_apix-0.7.3/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.473608 librus_apix-0.7.3/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 07:53:47.000000 librus_apix-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 07:53:49.473608 librus_apix-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:53:47.000000 librus_apix-0.7.3/setup.py
```

### Comparing `librus_apix-0.7.2/LICENSE` & `librus_apix-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.2/README.md` & `librus_apix-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.2/librus_apix/announcements.py` & `librus_apix-0.7.3/librus_apix/announcements.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,20 @@
         BeautifulSoup(token.get(token.ANNOUNCEMENTS_URL).text, "lxml")
     )
     announcements = []
     announcement_tables = soup.select("table.decorated.big.center.printable.margin-top")
     if len(announcement_tables) < 1:
         raise ParseError("Error in parsing announcements")
     for table in announcement_tables:
-        title = table.select_one("thead > tr > td").text
-        author, date, desc = [
+        title = table.select_one("thead > tr > td")
+        title = title.text if title is not None else ""
+
+        data = [
             line.select_one("td").text.strip()
+            if line.select_one("td") is not None
+            else ""
             for line in table.find_all("tr", attrs={"class": ["line0", "line1"]})
         ]
+        author, date, desc = data
         a = Announcement(title, author, desc, date)
         announcements.append(a)
     return announcements
```

### Comparing `librus_apix-0.7.2/librus_apix/attendance.py` & `librus_apix-0.7.3/librus_apix/attendance.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,64 +21,70 @@
 
 
 def get_detail(token: Token, detail_url: str) -> Dict[str, str]:
     details = {}
     div = no_access_check(
         BeautifulSoup(token.get(token.ATTENDANCE_DETAILS_URL + detail_url).text, "lxml")
     ).find("div", attrs={"class": "container-background"})
+    if div is None:
+        raise ParseError("Error in parsing attendance")
     line = div.find_all("tr", attrs={"class": ["line0", "line1"]})
     if len(line) < 1:
         raise ParseError("Error in parsing attendance.")
     for l in line:
-        if not l.find("th"):
+        if l.find("th") is None or l.find("td") is None:
             continue
-        details[l.find("th").text] = l.find("td").text
+        if th_elem is not None and td_elem is not None:
+            details[l.find("th").text] = l.find("td").text
     return details
 
+
 def get_gateway_attendance(token: Token):
     # The gateway api seems to be only updated every 3 hours
     # The api.librus.pl seems to require a private key to access
     types = {
-            "1": {"short": "nb" ,"name": "Nieobecność"},
-            "2": {"short": "sp" ,"name": "Spóźnienie"},
-            "3": {"short": "u" ,"name": "Nieobecność uspr."},
-            "4": {"short": "zw" ,"name": "Zwolnienie"},
-            "100": {"short": "ob" ,"name": "Obecność"},
-            "1266": {"short": "wy" ,"name": "Wycieczka"},
-            "2022": {"short": "k" ,"name": "Konkurs szkolny"},
-            "2829": {"short": "sz" ,"name": "Szkolenie"},
-            }
+        "1": {"short": "nb", "name": "Nieobecność"},
+        "2": {"short": "sp", "name": "Spóźnienie"},
+        "3": {"short": "u", "name": "Nieobecność uspr."},
+        "4": {"short": "zw", "name": "Zwolnienie"},
+        "100": {"short": "ob", "name": "Obecność"},
+        "1266": {"short": "wy", "name": "Wycieczka"},
+        "2022": {"short": "k", "name": "Konkurs szkolny"},
+        "2829": {"short": "sz", "name": "Szkolenie"},
+    }
     if token.oauth == "":
         token.refresh_oauth()
     token.cookies["oauth_token"] = token.oauth
     response = token.get(token.GATEWAY_API_ATTENDANCE)
 
     attendances = response.json()["Attendances"]
 
-
     return [
-            (tuple(
-                types[
-                    str(a["Type"]["Id"])].values()),
-            a["LessonNo"],
-            a["Semester"]
-            ) for a in attendances]
+        (tuple(types[str(a["Type"]["Id"])].values()), a["LessonNo"], a["Semester"])
+        for a in attendances
+    ]
+
 
 def get_attendance_frequency(token: Token):
     attendance = get_gateway_attendance(token)
     first_semester = [a for a in attendance if a[2] == 1]
     second_semester = [a for a in attendance if a[2] == 2]
     f_attended = len([a for a in first_semester if a[0][0] in ["wy", "ob", "sp"]])
     s_attended = len([a for a in second_semester if a[0][0] in ["wy", "ob", "sp"]])
     f_freq = f_attended / len(first_semester) if len(second_semester) != 0 else 1
     s_freq = s_attended / len(second_semester) if len(second_semester) != 0 else 1
-    overall_freq = len([a for a in attendance if a[0][0] in ["wy", "ob", "sp"]]) / len(attendance) if len(attendance) != 0 else 1
+    overall_freq = (
+        len([a for a in attendance if a[0][0] in ["wy", "ob", "sp"]]) / len(attendance)
+        if len(attendance) != 0
+        else 1
+    )
     return f_freq, s_freq, overall_freq
     # ADD Lesson frequency
 
+
 def get_attendance(token: Token, sort_by: str = "all") -> List[List[Attendance]]:
     SORT = {
         "all": {"zmiany_logowanie_wszystkie": ""},
         "week": {"zmiany_logowanie_tydzien": "zmiany_logowanie_tydzien"},
         "last_login": {"zmiany_logowanie": "zmiany_logowanie"},
     }
     if sort_by not in SORT.keys():
@@ -97,36 +103,44 @@
         raise ParseError("Error parsing attendance.")
     days = table.find_all("tr", attrs={"class": ["line0", "line1"]})
     att = [[], []]
     semester = -1
     for day in days:
         if day.find("td", attrs={"class": "center bolded"}):
             semester += 1
-        date = day.find("td", attrs={"class": None})
         attendance = day.find_all("td", attrs={"class": "center"})
         for attend in attendance:
             at = attend.find_all("a")
             for single in at:
                 if not single:
                     continue
-                attributes = {
-                    i.split(": ")[0].strip(): i.split(": ")[1].strip()
-                    for i in single.attrs["title"]
+                attributes = {}
+                pairs = [
+                    pair.split(":", 1)
+                    for pair in single.attrs["title"]
                     .replace("</b>", "<br>")
                     .replace("<br/>", "")
                     .strip()
                     .split("<br>")
-                }
-                date = attributes["Data"].split(" ")[0]
-                _type = attributes["Rodzaj"]
-                school_subject = attributes["Lekcja"]
-                topic = attributes.get("Temat zajęć")  # optional
-                period = int(attributes["Godzina lekcyjna"])
-                excursion = True if attributes["Czy wycieczka"] == "Tak" else False
-                teacher = attributes["Nauczyciel"]
+                ]
+                for pair in pairs:
+                    if len(pair) != 2:
+                        attributes[pair[0].strip()] = "unknown"
+                        continue
+                    key, val = pair
+                    attributes[key.strip()] = val.strip()
+                date = attributes.get("Data", "").split(" ")[0]
+                _type = attributes.get("Rodzaj", "")
+                school_subject = attributes.get("Lekcja", "")
+                topic = attributes.get("Temat zajęć", "")
+                period = int(attributes.get("Godzina lekcyjna", "0"))
+                excursion = (
+                    True if attributes.get("Czy wycieczka", "") == "Tak" else False
+                )
+                teacher = attributes.get("Nauczyciel", "")
 
                 href = (
                     single.attrs["onclick"]
                     .replace("otworz_w_nowym_oknie(", "")
                     .split(",")[0]
                     .replace("'", "")
                     .split("/")[3]
```

### Comparing `librus_apix-0.7.2/librus_apix/completed_lessons.py` & `librus_apix-0.7.3/librus_apix/completed_lessons.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,23 +68,29 @@
     completed_lessons = []
     soup = no_access_check(
         BeautifulSoup(token.post(token.COMPLETED_LESSONS_URL, data=data).text, "lxml")
     )
 
     lines = soup.select('table[class="decorated"] > tbody > tr')
     for line in lines:
-        date = line.select_one('td[class="center small"]').text
-        weekday = line.select_one("td.tiny").text
-        lesson_number, subject_and_teacher, topic, z_value, attendance = [
-            td.text.strip() for td in line.find_all("td", attrs={"class": None})
-        ]
+        date = line.select_one('td[class="center small"]')
+        date = date.text if date is not None else "01-01-2000"
+        weekday = line.select_one("td.tiny")
+        weekday = weekday.text if weekday is not None else ""
+        data = [td.text.strip() for td in line.find_all("td", attrs={"class": None})]
+        if len(data) < 5:
+            continue
+        lesson_number, subject_and_teacher, topic, z_value, attendance = data
         subject, teacher = subject_and_teacher.split(", ")
         attendance_href = ""
         if attendance != "":
-            attendance_href = line.select_one("td > p.box > a").text
+            attendance_href = line.select_one("td > p.box > a")
+            attendance_href = (
+                attendance_href.text if attendance_href is not None else ""
+            )
         lesson = Lesson(
             subject,
             teacher,
             topic,
             z_value,
             attendance,
             attendance_href,
```

### Comparing `librus_apix-0.7.2/librus_apix/get_token.py` & `librus_apix-0.7.3/librus_apix/get_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         schedule_url: Optional[str] = urls.SCHEDULE_URL,
         homework_url: Optional[str] = urls.HOMEWORK_URL,
         homework_details_url: Optional[str] = urls.HOMEWORK_DETAILS_URL,
         info_url: Optional[str] = urls.INFO_URL,
         recipients_url: Optional[str] = urls.RECIPIENTS_URL,
         completed_lessons_url: Optional[str] = urls.COMPLETED_LESSONS_URL,
         gateway_api_attendance: Optional[str] = urls.GATEWAY_API_ATTENDANCE,
-        proxy: Optional[dict[str, str]] = {}
-        ):
+        proxy: Optional[dict[str, str]] = {},
+    ):
         self._session = Session()
         if not API_Key:
             self.cookies = {}
             self.csrf_token = ""
             return
         self.API_Key = API_Key
         cookies = {"DZIENNIKSID": API_Key.split(":")[0]}
@@ -56,20 +56,24 @@
         self.GATEWAY_API_ATTENDANCE = gateway_api_attendance
         self.RECIPIENTS_URL = recipients_url
 
     def refresh_oauth(self) -> str:
         with self._session as s:
             s.headers = urls.HEADERS
             s.cookies = cookiejar_from_dict(self.cookies)
-            response: Response = s.get("https://synergia.librus.pl/refreshToken", proxies=self.proxy)
+            response: Response = s.get(
+                "https://synergia.librus.pl/refreshToken", proxies=self.proxy
+            )
             if response.status_code == 200:
                 oauth = response.cookies.get("oauth_token")
                 self.oauth = oauth
                 return oauth
-        raise AuthorizationError(f"Error while refreshing oauth token {response.content}")
+        raise AuthorizationError(
+            f"Error while refreshing oauth token {response.content}"
+        )
 
     def post(self, url: str, data: Dict[str, Union[str, int]]) -> Response:
         with self._session as s:
             s.headers = urls.HEADERS
             s.cookies = cookiejar_from_dict(self.cookies)
             response: Response = s.post(url, data=data, proxies=self.proxy)
             return response
@@ -110,19 +114,21 @@
             message_list = maint_check.json().get("Message")
             if not message_list:
                 # during recent maintenance there were no messages (empty list)
                 raise MaintananceError("maintenance")
             raise MaintananceError(message_list[0]["description"])
         s.get(
             api_url
-            + "/OAuth/Authorization?client_id=46&response_type=code&scope=mydata", proxies=proxy
+            + "/OAuth/Authorization?client_id=46&response_type=code&scope=mydata",
+            proxies=proxy,
         )
         response = s.post(
             api_url + "/OAuth/Authorization?client_id=46",
-            data={"action": "login", "login": username, "pass": password}, proxies=proxy
+            data={"action": "login", "login": username, "pass": password},
+            proxies=proxy,
         )
         if response.json()["status"] == "error":
             raise AuthorizationError(response.json()["errors"][0]["message"])
 
         s.get(api_url + response.json().get("goTo"), proxies=proxy)
 
         cookies = dict_from_cookiejar(s.cookies)
@@ -140,11 +146,11 @@
             schedule_url,
             homework_url,
             homework_details_url,
             info_url,
             recipients_url,
             completed_lessons_url,
             gateway_api_attendance,
-            proxy=proxy
+            proxy=proxy,
         )
 
         return token
```

### Comparing `librus_apix-0.7.2/librus_apix/grades.py` & `librus_apix-0.7.3/librus_apix/grades.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,25 +99,26 @@
     if gpacount and gpacount[0].split(": ")[1] == "tak":
         counts = True
     return desc, counts
 
 
 def _extract_grade_info(a, subject):
     date = re.search("Data:.{11}", a.attrs["title"])
+    if date is None:
+        raise ParseError("Error in getting grade's date.")
+
     attr_dict = {}
     for attr in a.attrs["title"].replace("<br/>", "<br>").split("<br>"):
         if len(attr.strip()) > 2:
             key, value = attr.split(": ", 1)
             attr_dict[key] = value
     category = attr_dict.get("Kategoria", "")
     teacher = attr_dict.get("Nauczyciel", "")
     weight = attr_dict.get("Waga", 0)
 
-    if date is None:
-        raise ParseError("Error in getting grade's date.")
     grade = a.text.replace("\xa0", "").replace("\n", "")
     desc, counts = get_desc_and_counts(a, grade, subject)
 
     return (
         grade,
         date.group().split(" ")[1],
         a.attrs["href"],
@@ -147,16 +148,21 @@
         average_grades = list(map(lambda x: x.text, box.select("td.right")))
         semesters = [semester_grades[1:4], semester_grades[4:7]]
         subject = _handle_subject(semester_grades)
         for sem, semester in enumerate(semesters):
             if subject not in sem_grades[sem]:
                 sem_grades[sem][subject] = []
             for sg in semester:
-                grade_a_improved = sg.select("td[class!='center'] > span > span.grade-box > a")
-                grade_a = sg.select("td[class!='center'] > span.grade-box > a") + grade_a_improved
+                grade_a_improved = sg.select(
+                    "td[class!='center'] > span > span.grade-box > a"
+                )
+                grade_a = (
+                    sg.select("td[class!='center'] > span.grade-box > a")
+                    + grade_a_improved
+                )
                 for a in grade_a:
                     (
                         _grade,
                         date,
                         href,
                         desc,
                         counts,
@@ -174,20 +180,20 @@
                         sem + 1,
                         category,
                         teacher,
                         weight,
                     )
                     sem_grades[sem][subject].append(g)
             avg_gr = (
-                average_grades[sem] if len(average_grades) > sem else 0.0
+                average_grades[sem] if len(average_grades) >= sem else 0.0
             )  # might happen that the list is empty
             gpa = Gpa(sem + 1, avg_gr, subject)
             avg_grades[subject].append(gpa)
         avg_gr = (
-            average_grades[-1] if average_grades else 0.0
+            average_grades[-1] if len(average_grades) > 0 else 0.0
         )  # might happen that the list is empty
         avg_grades[subject].append(Gpa(0, avg_gr, subject))
 
     return sem_grades, avg_grades
 
 
 def _extract_grades_descriptive(table_rows):
@@ -246,35 +252,42 @@
     summary_teacher = ""
 
     parse_next_row = False
     for box in table_rows:
         if parse_next_row:
             parse_next_row = False
             paragraphs = box.find_all("p")
-            text_list = [ par.text.strip() for par in paragraphs ]
+            text_list = [par.text.strip() for par in paragraphs]
             summary_desc = "\n".join(text_list).strip()
             found_grade = True
             # description found - break
             # There is no more grades for now (for first semester). Maybe there will be grade for
             # second semester, but the format (structure) of web page is unknown for the moment.
             # #TODO: implement the case for second semester (in future)
             break
 
         header = box.select_one("th")
-        if header:
+        if header and header.select_one("strong") is not None:
             # header row found - next row will contain the description
             parse_next_row = True
             title_tag = header.select_one("strong")
             info = title_tag.next_sibling
             summary_title = title_tag.text.strip()
-            summary_date = re.findall(r"opublikowano: (.+?) ", info)[0]     # get date only
+            summary_date = re.findall(r"opublikowano: (.+?) ", info)[0]  # get date only
             summary_teacher = re.findall(r"nauczyciel: (.+?)\)", info)[0]
 
     if found_grade:
         sem_index = 0
-        semester_summary = GradeDescriptive(summary_title, "", summary_date, "",
-                                            summary_desc, sem_index + 1, summary_teacher)
+        semester_summary = GradeDescriptive(
+            summary_title,
+            "",
+            summary_date,
+            "",
+            summary_desc,
+            sem_index + 1,
+            summary_teacher,
+        )
         if summary_title not in sem_grades_desc[sem_index]:
             sem_grades_desc[sem_index][summary_title] = []
         sem_grades_desc[sem_index][summary_title].append(semester_summary)
 
     return sem_grades_desc
```

### Comparing `librus_apix-0.7.2/librus_apix/homework.py` & `librus_apix-0.7.3/librus_apix/homework.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,15 +57,22 @@
             return []
         # parsing error
         raise ParseError("Error in parsing homework.")
     hw = []
     lines = soup.find_all("tr", attrs={"class": ["line0", "line1"]})
     for line in lines:
         hw_list = [txt.text.replace("\n", "") for txt in line.find_all("td")]
-        href = line.find("input").attrs["onclick"].split("'")[1].split("/")[3]
+        if len(hw_list) < 8:
+            raise ParseError("Error while parsing homework data")
+        href = line.find("input")
+        href = (
+            href.attrs["onclick"].split("'")[1].split("/")[3]
+            if line is not None
+            else ""
+        )
         h = Homework(
             hw_list[0],
             hw_list[1],
             hw_list[2],
             hw_list[3],
             str(hw_list[4] + " " + hw_list[5]),
             str(hw_list[6] + " " + str(hw_list[7])),
```

### Comparing `librus_apix-0.7.2/librus_apix/messages.py` & `librus_apix-0.7.3/librus_apix/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,68 +12,89 @@
     author: str
     title: str
     date: str
     href: str
     unread: bool
     has_attachment: bool
 
+
 def recipient_groups():
-    return  {
-            "teachers": "nauczyciel",
-            "tutors": "wychowawca",
-            "parent_council": "szkolna_rada_rodzicow",
-            "pedagogue": "pedagog",
-            "admin": "admin",
-            "secretary": "sekretariat",
-            }
+    return {
+        "teachers": "nauczyciel",
+        "tutors": "wychowawca",
+        "parent_council": "szkolna_rada_rodzicow",
+        "pedagogue": "pedagog",
+        "admin": "admin",
+        "secretary": "sekretariat",
+    }
 
 
 def get_recipients(token: Token, group: str = "teachers"):
     groups = recipient_groups()
     if group not in groups:
-        raise ValueError(f"{group} group is not available. Available groups: {' | '.join(groups.keys())}")
+        raise ValueError(
+            f"{group} group is not available. Available groups: {' | '.join(groups.keys())}"
+        )
     group = groups[group]
-    payload = {"typAdresata": group, "poprzednia": 5, "tabZaznaczonych": "", "czyWirtualneKlasy": False, "idGrupy": 0}
+    payload = {
+        "typAdresata": group,
+        "poprzednia": 5,
+        "tabZaznaczonych": "",
+        "czyWirtualneKlasy": False,
+        "idGrupy": 0,
+    }
     soup = no_access_check(
         BeautifulSoup(token.post(token.RECIPIENTS_URL, data=payload).text, "lxml")
     )
     labels = soup.select("label")
     teachers = {}
     for label in labels:
-        teachers[label.text.replace("\xa0", "")] = label.attrs.get("for", "").split("_")[-1]
+        teachers[label.text.replace("\xa0", "")] = label.attrs.get("for", "").split(
+            "_"
+        )[-1]
     return teachers
 
-def send_message(token: Token, title: str, content: str, recipient_group: str, recipient_ids: list[str]):
+
+def send_message(
+    token: Token,
+    title: str,
+    content: str,
+    recipient_group: str,
+    recipient_ids: list[str],
+):
     """
     librus' amazing requests include all possible teacher ids for the group inside the payload.
     The recipients are differentiated by lack of '_hid' in the key.
     It might not be needed but I would rather not send a test message to everyone in school accidentally.
     if anyone is willing to give it a test, good luck.
     """
     all_recipients_ids = list(get_recipients(token, recipient_group).values())
     payload = {
-            "filtrUzytkownikow": 0,
-            "idPojemnika": "",
-            "adresat": recipient_groups().get(recipient_group, ""),
-            "DoKogo_hid": list(filter(lambda id: id not in recipient_ids, all_recipients_ids)),
-            "DoKogo": list(filter(lambda id: id in recipient_ids, all_recipients_ids)),
-            "Rodzaj": 0,
-            "temat": title,
-            "tresc": content,
-            "poprzednia": 5,
-            "fileStorageIdentifier": "",
-            "wyslij": "Wyślij"
-            }
+        "filtrUzytkownikow": 0,
+        "idPojemnika": "",
+        "adresat": recipient_groups().get(recipient_group, ""),
+        "DoKogo_hid": list(
+            filter(lambda id: id not in recipient_ids, all_recipients_ids)
+        ),
+        "DoKogo": list(filter(lambda id: id in recipient_ids, all_recipients_ids)),
+        "Rodzaj": 0,
+        "temat": title,
+        "tresc": content,
+        "poprzednia": 5,
+        "fileStorageIdentifier": "",
+        "wyslij": "Wyślij",
+    }
     sent_message = token.post(token.SEND_MESSAGE_URL, data=payload)
 
     if sent_message.status_code == 200:
         return True
 
     return False
 
+
 def message_content(token: Token, content_url: str) -> str:
     soup = no_access_check(
         BeautifulSoup(token.get(token.MESSAGE_URL + "/" + content_url).text, "lxml")
     )
     content = soup.find("div", attrs={"class": "container-message-content"})
     if content is None:
         raise ParseError("Error in parsing message content.")
@@ -82,27 +103,31 @@
 
 def parse(message_soup: BeautifulSoup) -> List[Message]:
     msgs: List[Message] = []
     hasAttachment = False
     soup = message_soup.find("table", attrs={"class": "decorated stretch"})
     if soup is None:
         raise ParseError("Error in parsing messages.")
-    tds = soup.find("tbody").find_all("tr", attrs={"class": ["line0", "line1"]})
+    tbody = soup.find("tbody")
+    if tbody is None:
+        raise ParseError("Error in parsing messages (tbody).")
+    tds = tbody.find_all("tr", attrs={"class": ["line0", "line1"]})
     if tds[0].text.strip() == "Brak wiadomości":
         return []
     for td in tds:
         unread = False
         hasAttachment = False
         _tick, attachment, author, title, date, _trash = td.find_all("td")
         if attachment.find("img"):
             hasAttachment = True
         if title.get("style") and "font-weight: bold" in title.get("style"):
             unread = True
 
-        href = author.find("a").attrs["href"].split("/")[4]
+        href = author.find("a")
+        href = href.attrs["href"].split("/")[4] if href is not None else ""
         author = str(author.text)
         title = str(title.text)
         date = str(date.text)
         m = Message(author, title, date, href, unread, hasAttachment)
         msgs.append(m)
     return msgs
```

### Comparing `librus_apix-0.7.2/librus_apix/schedule.py` & `librus_apix-0.7.3/librus_apix/schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,39 +30,46 @@
         raise ParseError("Error in parsing schedule details.")
     tr = div.find_all("tr", attrs={"class": ["line0", "line1"]})
     for s in tr:
         schedule[s.find("th").text.strip()] = s.find("td").text.strip()
     return schedule
 
 
-def get_schedule(token: Token, month: str, year: str, include_empty: bool = False) -> Dict[int, List[Event]]:
+def get_schedule(
+    token: Token, month: str, year: str, include_empty: bool = False
+) -> Dict[int, List[Event]]:
     schedule = defaultdict(list)
     soup = no_access_check(
         BeautifulSoup(
             token.post(token.SCHEDULE_URL, data={"rok": year, "miesiac": month}).text,
             "lxml",
         )
     )
     days = soup.find_all("div", attrs={"class": "kalendarz-dzien"})
     if len(days) < 1:
         raise ParseError("Error in parsing days of the schedule.")
     for day in days:
-        d = day.find("div", attrs={"class": "kalendarz-numer-dnia"}).text
+        try:
+            d = day.find("div", attrs={"class": "kalendarz-numer-dnia"}).text
+        except:
+            raise ParseError("Error while parsing day number")
         if include_empty == True:
             schedule[int(d)] = []
         tr = day.find_all("tr")
         if tr:
             for event in tr:
                 td = event.find("td")
+                if td is None:
+                    continue
                 title = td.attrs.get("title", "Nauczyciel: unknown<br />Opis: unknown")
                 additional_data = {}
                 pairs = [pair.split(":", 1) for pair in title.split("<br />")]
                 for pair in pairs:
                     if len(pair) != 2:
-                        additional_data[key.strip()] = "unknown"
+                        additional_data[pair[0].strip()] = "unknown"
                         continue
                     key, val = pair
                     additional_data[key.strip()] = val.strip()
                 subject = "unspecified"
                 span = td.find("span")
                 if span:
                     subject = span.text
@@ -100,11 +107,13 @@
                 except IndexError:
                     pass
                 try:
                     onclick = event.find("td").attrs["onclick"]
                     href = "/".join(onclick.split("'")[1].split("/")[2:])
                 except KeyError:
                     href = ""
+                except IndexError:
+                    href = ""
 
                 event = Event(title, subject, additional_data, d, number, hour, href)
                 schedule[int(d)].append(event)
     return schedule
```

### Comparing `librus_apix-0.7.2/librus_apix/timetable.py` & `librus_apix-0.7.3/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.2/librus_apix/urls.py` & `librus_apix-0.7.3/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.2/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.3/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.2/setup.cfg` & `librus_apix-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.7.2
+version = 0.7.3
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

