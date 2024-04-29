# Comparing `tmp/pydruid-0.6.6.tar.gz` & `tmp/pydruid-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydruid-0.6.6.tar", last modified: Fri Dec  1 18:19:21 2023, max compression
+gzip compressed data, was "pydruid-0.6.7.tar", last modified: Mon Apr 29 19:34:54 2024, max compression
```

## Comparing `pydruid-0.6.6.tar` & `pydruid-0.6.7.tar`

### file list

```diff
@@ -1,41 +1,67 @@
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.217408 pydruid-0.6.6/
--rw-r--r--   0 gian       (501) staff       (20)    35132 2023-12-01 18:17:31.000000 pydruid-0.6.6/CHANGELOG.md
--rw-r--r--   0 gian       (501) staff       (20)      563 2022-09-19 22:49:20.000000 pydruid-0.6.6/LICENSE
--rw-r--r--   0 gian       (501) staff       (20)      127 2022-09-19 22:49:20.000000 pydruid-0.6.6/MANIFEST.in
--rw-r--r--   0 gian       (501) staff       (20)    10998 2023-12-01 18:19:21.217321 pydruid-0.6.6/PKG-INFO
--rw-r--r--   0 gian       (501) staff       (20)     9821 2022-09-19 22:49:20.000000 pydruid-0.6.6/README.md
--rw-r--r--   0 gian       (501) staff       (20)      570 2022-09-19 22:49:20.000000 pydruid-0.6.6/RELEASE.md
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.214640 pydruid-0.6.6/pydruid/
--rw-r--r--   0 gian       (501) staff       (20)        0 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/__init__.py
--rw-r--r--   0 gian       (501) staff       (20)     5875 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/async_client.py
--rwxr-xr-x   0 gian       (501) staff       (20)    22963 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/client.py
--rw-r--r--   0 gian       (501) staff       (20)     4461 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/console.py
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.215746 pydruid-0.6.6/pydruid/db/
--rw-r--r--   0 gian       (501) staff       (20)      652 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/db/__init__.py
--rw-r--r--   0 gian       (501) staff       (20)    12010 2023-12-01 18:17:31.000000 pydruid-0.6.6/pydruid/db/api.py
--rw-r--r--   0 gian       (501) staff       (20)      479 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/db/exceptions.py
--rw-r--r--   0 gian       (501) staff       (20)     7162 2023-12-01 18:17:31.000000 pydruid-0.6.6/pydruid/db/sqlalchemy.py
--rw-r--r--   0 gian       (501) staff       (20)    17347 2023-12-01 18:17:31.000000 pydruid-0.6.6/pydruid/query.py
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.216492 pydruid-0.6.6/pydruid/utils/
--rw-r--r--   0 gian       (501) staff       (20)        0 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/utils/__init__.py
--rw-r--r--   0 gian       (501) staff       (20)     3069 2023-12-01 18:17:31.000000 pydruid-0.6.6/pydruid/utils/aggregators.py
--rw-r--r--   0 gian       (501) staff       (20)     5541 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/utils/dimensions.py
--rw-r--r--   0 gian       (501) staff       (20)    10600 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/utils/filters.py
--rw-r--r--   0 gian       (501) staff       (20)     3544 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/utils/having.py
--rw-r--r--   0 gian       (501) staff       (20)     7007 2023-12-01 18:17:31.000000 pydruid-0.6.6/pydruid/utils/postaggregator.py
--rw-r--r--   0 gian       (501) staff       (20)     1359 2022-09-19 22:49:20.000000 pydruid-0.6.6/pydruid/utils/query_utils.py
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.215309 pydruid-0.6.6/pydruid.egg-info/
--rw-r--r--   0 gian       (501) staff       (20)    10998 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/PKG-INFO
--rw-r--r--   0 gian       (501) staff       (20)      748 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/SOURCES.txt
--rw-r--r--   0 gian       (501) staff       (20)        1 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/dependency_links.txt
--rw-r--r--   0 gian       (501) staff       (20)      225 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/entry_points.txt
--rw-r--r--   0 gian       (501) staff       (20)      115 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/requires.txt
--rw-r--r--   0 gian       (501) staff       (20)        8 2023-12-01 18:19:21.000000 pydruid-0.6.6/pydruid.egg-info/top_level.txt
--rw-r--r--   0 gian       (501) staff       (20)     2714 2022-09-19 22:49:20.000000 pydruid-0.6.6/requirements-dev.txt
--rw-r--r--   0 gian       (501) staff       (20)      757 2022-09-19 22:49:20.000000 pydruid-0.6.6/requirements.txt
--rw-r--r--   0 gian       (501) staff       (20)      451 2023-12-01 18:19:21.217651 pydruid-0.6.6/setup.cfg
--rw-r--r--   0 gian       (501) staff       (20)     1734 2023-12-01 18:18:01.000000 pydruid-0.6.6/setup.py
-drwxr-xr-x   0 gian       (501) staff       (20)        0 2023-12-01 18:19:21.216822 pydruid-0.6.6/tests/
--rw-r--r--   0 gian       (501) staff       (20)     5627 2022-09-19 22:49:20.000000 pydruid-0.6.6/tests/test_async_client.py
--rw-r--r--   0 gian       (501) staff       (20)     6305 2022-09-19 22:49:20.000000 pydruid-0.6.6/tests/test_client.py
--rw-r--r--   0 gian       (501) staff       (20)    11554 2023-12-01 18:17:31.000000 pydruid-0.6.6/tests/test_query.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.466992 pydruid-0.6.7/
+-rw-r--r--   0 beto       (501) staff       (20)      150 2020-12-09 19:07:01.000000 pydruid-0.6.7/.flake8
+-rw-r--r--   0 beto       (501) staff       (20)      137 2020-12-09 19:07:01.000000 pydruid-0.6.7/.gitignore
+-rw-r--r--   0 beto       (501) staff       (20)      668 2024-04-29 19:31:26.000000 pydruid-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 beto       (501) staff       (20)      360 2020-12-09 19:07:01.000000 pydruid-0.6.7/.travis.yml
+-rw-r--r--   0 beto       (501) staff       (20)    35132 2024-04-29 19:31:26.000000 pydruid-0.6.7/CHANGELOG.md
+-rw-r--r--   0 beto       (501) staff       (20)      563 2020-12-09 19:07:01.000000 pydruid-0.6.7/LICENSE
+-rw-r--r--   0 beto       (501) staff       (20)      127 2020-12-09 19:07:01.000000 pydruid-0.6.7/MANIFEST.in
+-rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 19:34:54.467316 pydruid-0.6.7/PKG-INFO
+-rw-r--r--   0 beto       (501) staff       (20)     9821 2020-12-09 19:07:01.000000 pydruid-0.6.7/README.md
+-rw-r--r--   0 beto       (501) staff       (20)      570 2022-07-25 16:17:08.000000 pydruid-0.6.7/RELEASE.md
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.454954 pydruid-0.6.7/docs/
+-rw-r--r--   0 beto       (501) staff       (20)     6775 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/Makefile
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.455669 pydruid-0.6.7/docs/figures/
+-rw-r--r--   0 beto       (501) staff       (20)    26636 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/figures/avg_tweet_length.png
+-rw-r--r--   0 beto       (501) staff       (20)    46319 2020-12-09 19:07:01.000000 pydruid-0.6.7/docs/figures/twitter_graph.png
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.456384 pydruid-0.6.7/docs/source/
+-rw-r--r--   0 beto       (501) staff       (20)     8401 2020-12-09 20:36:52.000000 pydruid-0.6.7/docs/source/conf.py
+-rw-r--r--   0 beto       (501) staff       (20)     1339 2020-12-09 20:36:52.000000 pydruid-0.6.7/docs/source/index.rst
+-rwxr-xr-x   0 beto       (501) staff       (20)      299 2022-11-02 22:28:56.000000 pydruid-0.6.7/gen_changelog.sh
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.457909 pydruid-0.6.7/pydruid/
+-rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)     5875 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/async_client.py
+-rwxr-xr-x   0 beto       (501) staff       (20)    22963 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/client.py
+-rw-r--r--   0 beto       (501) staff       (20)     4461 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/console.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.461089 pydruid-0.6.7/pydruid/db/
+-rw-r--r--   0 beto       (501) staff       (20)      652 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/db/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)    12015 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/api.py
+-rw-r--r--   0 beto       (501) staff       (20)      475 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/exceptions.py
+-rw-r--r--   0 beto       (501) staff       (20)     7187 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/db/sqlalchemy.py
+-rw-r--r--   0 beto       (501) staff       (20)    17347 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/query.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.463387 pydruid-0.6.7/pydruid/utils/
+-rw-r--r--   0 beto       (501) staff       (20)        0 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/__init__.py
+-rw-r--r--   0 beto       (501) staff       (20)     3069 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/utils/aggregators.py
+-rw-r--r--   0 beto       (501) staff       (20)     5541 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/dimensions.py
+-rw-r--r--   0 beto       (501) staff       (20)    10600 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/filters.py
+-rw-r--r--   0 beto       (501) staff       (20)     3544 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/having.py
+-rw-r--r--   0 beto       (501) staff       (20)     7007 2024-04-29 19:31:26.000000 pydruid-0.6.7/pydruid/utils/postaggregator.py
+-rw-r--r--   0 beto       (501) staff       (20)     1359 2020-12-09 19:07:01.000000 pydruid-0.6.7/pydruid/utils/query_utils.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.459819 pydruid-0.6.7/pydruid.egg-info/
+-rw-r--r--   0 beto       (501) staff       (20)    12943 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/PKG-INFO
+-rw-r--r--   0 beto       (501) staff       (20)     1206 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/SOURCES.txt
+-rw-r--r--   0 beto       (501) staff       (20)        1 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/dependency_links.txt
+-rw-r--r--   0 beto       (501) staff       (20)      226 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/entry_points.txt
+-rw-r--r--   0 beto       (501) staff       (20)      115 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/requires.txt
+-rw-r--r--   0 beto       (501) staff       (20)        8 2024-04-29 19:34:54.000000 pydruid-0.6.7/pydruid.egg-info/top_level.txt
+-rwxr-xr-x   0 beto       (501) staff       (20)       77 2020-12-09 19:07:01.000000 pydruid-0.6.7/pypi_push.sh
+-rw-r--r--   0 beto       (501) staff       (20)       75 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements-dev.in
+-rw-r--r--   0 beto       (501) staff       (20)     2714 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements-dev.txt
+-rw-r--r--   0 beto       (501) staff       (20)       34 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements.in
+-rw-r--r--   0 beto       (501) staff       (20)      757 2020-12-09 19:07:01.000000 pydruid-0.6.7/requirements.txt
+-rw-r--r--   0 beto       (501) staff       (20)      451 2024-04-29 19:34:54.468439 pydruid-0.6.7/setup.cfg
+-rw-r--r--   0 beto       (501) staff       (20)     1734 2024-04-29 19:31:55.000000 pydruid-0.6.7/setup.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.464360 pydruid-0.6.7/tests/
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.465042 pydruid-0.6.7/tests/db/
+-rw-r--r--   0 beto       (501) staff       (20)     5061 2024-04-29 19:31:26.000000 pydruid-0.6.7/tests/db/test_cursor.py
+-rw-r--r--   0 beto       (501) staff       (20)     1492 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/db/test_rows_from_chunks.py
+-rw-r--r--   0 beto       (501) staff       (20)     5627 2020-12-09 20:36:52.000000 pydruid-0.6.7/tests/test_async_client.py
+-rw-r--r--   0 beto       (501) staff       (20)     6305 2020-12-09 20:36:52.000000 pydruid-0.6.7/tests/test_client.py
+-rw-r--r--   0 beto       (501) staff       (20)    11554 2024-04-29 19:31:26.000000 pydruid-0.6.7/tests/test_query.py
+drwxr-xr-x   0 beto       (501) staff       (20)        0 2024-04-29 19:34:54.466700 pydruid-0.6.7/tests/utils/
+-rw-r--r--   0 beto       (501) staff       (20)     8582 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_aggregators.py
+-rw-r--r--   0 beto       (501) staff       (20)    11885 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_dimensions.py
+-rw-r--r--   0 beto       (501) staff       (20)    16142 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_filters.py
+-rw-r--r--   0 beto       (501) staff       (20)     3840 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_having.py
+-rw-r--r--   0 beto       (501) staff       (20)      896 2020-12-09 19:07:01.000000 pydruid-0.6.7/tests/utils/test_query_utils.py
+-rw-r--r--   0 beto       (501) staff       (20)      459 2020-12-09 19:07:01.000000 pydruid-0.6.7/tox.ini
```

### Comparing `pydruid-0.6.6/CHANGELOG.md` & `pydruid-0.6.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/LICENSE` & `pydruid-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/PKG-INFO` & `pydruid-0.6.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,309 +1,302 @@
 Metadata-Version: 2.1
 Name: pydruid
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Python connector for Druid.
 Home-page: https://druid.apache.org
 Author: Druid Developers
 Author-email: druid-development@googlegroups.com
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/druid-io/pydruid/issues
 Project-URL: Documentation, https://pythonhosted.org/pydruid/
 Project-URL: Source Code, https://github.com/druid-io/pydruid
+Description: # pydruid
+        
+        pydruid exposes a simple API to create, execute, and analyze [Druid](http://druid.io/) queries. pydruid can parse query results into [Pandas](http://pandas.pydata.org/) DataFrame objects for subsequent data analysis -- this offers a tight integration between [Druid](http://druid.io/), the [SciPy](http://www.scipy.org/stackspec.html) stack (for scientific computing) and [scikit-learn](http://scikit-learn.org/stable/) (for machine learning). pydruid can export query results into TSV or JSON for further processing with your favorite tool, e.g., R, Julia, Matlab, Excel. It provides both synchronous and asynchronous clients.
+        
+        Additionally, pydruid implements the [Python DB API 2.0](https://www.python.org/dev/peps/pep-0249/), a [SQLAlchemy dialect](http://docs.sqlalchemy.org/en/latest/dialects/), and a provides a command line interface to interact with Druid.
+        
+        To install:
+        ```python
+        pip install pydruid
+        # or, if you intend to use asynchronous client
+        pip install pydruid[async]
+        # or, if you intend to export query results into pandas
+        pip install pydruid[pandas]
+        # or, if you intend to do both
+        pip install pydruid[async, pandas]
+        # or, if you want to use the SQLAlchemy engine
+        pip install pydruid[sqlalchemy]
+        # or, if you want to use the CLI
+        pip install pydruid[cli]
+        ```
+        Documentation: https://pythonhosted.org/pydruid/.
+        
+        # examples
+        
+        The following exampes show how to execute and analyze the results of three types of queries: timeseries, topN, and groupby. We will use these queries to ask simple questions about twitter's public data set.
+        
+        ## timeseries
+        
+        What was the average tweet length, per day, surrounding the 2014 Sochi olympics?
+        
+        ```python
+        from pydruid.client import *
+        from pylab import plt
+        
+        query = PyDruid(druid_url_goes_here, 'druid/v2')
+        
+        ts = query.timeseries(
+            datasource='twitterstream',
+            granularity='day',
+            intervals='2014-02-02/p4w',
+            aggregations={'length': doublesum('tweet_length'), 'count': doublesum('count')},
+            post_aggregations={'avg_tweet_length': (Field('length') / Field('count'))},
+            filter=Dimension('first_hashtag') == 'sochi2014'
+        )
+        df = query.export_pandas()
+        df['timestamp'] = df['timestamp'].map(lambda x: x.split('T')[0])
+        df.plot(x='timestamp', y='avg_tweet_length', ylim=(80, 140), rot=20,
+                title='Sochi 2014')
+        plt.ylabel('avg tweet length (chars)')
+        plt.show()
+        ```
+        
+        ![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/avg_tweet_length.png "Avg. tweet length")
+        
+        ## topN
+        
+        Who were the top ten mentions (@user_name) during the 2014 Oscars?
+        
+        ```python
+        top = query.topn(
+            datasource='twitterstream',
+            granularity='all',
+            intervals='2014-03-03/p1d',  # utc time of 2014 oscars
+            aggregations={'count': doublesum('count')},
+            dimension='user_mention_name',
+            filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
+                   (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
+                   ~(Dimension('user_mention_name') == 'No Mention'),
+            metric='count',
+            threshold=10
+        )
+        
+        df = query.export_pandas()
+        print df
+        
+           count                 timestamp user_mention_name
+        0   1303  2014-03-03T00:00:00.000Z      TheEllenShow
+        1     44  2014-03-03T00:00:00.000Z        TheAcademy
+        2     21  2014-03-03T00:00:00.000Z               MTV
+        3     21  2014-03-03T00:00:00.000Z         peoplemag
+        4     17  2014-03-03T00:00:00.000Z               THR
+        5     16  2014-03-03T00:00:00.000Z      ItsQueenElsa
+        6     16  2014-03-03T00:00:00.000Z           eonline
+        7     15  2014-03-03T00:00:00.000Z       PerezHilton
+        8     14  2014-03-03T00:00:00.000Z     realjohngreen
+        9     12  2014-03-03T00:00:00.000Z       KevinSpacey
+        
+        ```
+        
+        ## groupby
+        
+        What does the social network of users replying to other users look like?
+        
+        ```python
+        from igraph import *
+        from cairo import *
+        from pandas import concat
+        
+        group = query.groupby(
+            datasource='twitterstream',
+            granularity='hour',
+            intervals='2013-10-04/pt12h',
+            dimensions=["user_name", "reply_to_name"],
+            filter=(~(Dimension("reply_to_name") == "Not A Reply")) &
+                   (Dimension("user_location") == "California"),
+            aggregations={"count": doublesum("count")}
+        )
+        
+        df = query.export_pandas()
+        
+        # map names to categorical variables with a lookup table
+        names = concat([df['user_name'], df['reply_to_name']]).unique()
+        nameLookup = dict([pair[::-1] for pair in enumerate(names)])
+        df['user_name_lookup'] = df['user_name'].map(nameLookup.get)
+        df['reply_to_name_lookup'] = df['reply_to_name'].map(nameLookup.get)
+        
+        # create the graph with igraph
+        g = Graph(len(names), directed=False)
+        vertices = zip(df['user_name_lookup'], df['reply_to_name_lookup'])
+        g.vs["name"] = names
+        g.add_edges(vertices)
+        layout = g.layout_fruchterman_reingold()
+        plot(g, "tweets.png", layout=layout, vertex_size=2, bbox=(400, 400), margin=25, edge_width=1, vertex_color="blue")
+        ```
+        
+        ![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/twitter_graph.png "Social Network")
+        
+        # asynchronous client
+        ```pydruid.async_client.AsyncPyDruid``` implements an asynchronous client. To achieve that, it utilizes an asynchronous
+        HTTP client from ```Tornado``` framework. The asynchronous client is suitable for use with async frameworks such as Tornado
+        and provides much better performance at scale. It lets you serve multiple requests at the same time, without blocking on
+        Druid executing your queries.
+        
+        ## example
+        ```python
+        from tornado import gen
+        from pydruid.async_client import AsyncPyDruid
+        from pydruid.utils.aggregators import longsum
+        from pydruid.utils.filters import Dimension
+        
+        client = AsyncPyDruid(url_to_druid_broker, 'druid/v2')
+        
+        @gen.coroutine
+        def your_asynchronous_method_serving_top10_mentions_for_day(day
+            top_mentions = yield client.topn(
+                datasource='twitterstream',
+                granularity='all',
+                intervals="%s/p1d" % (day, ),
+                aggregations={'count': doublesum('count')},
+                dimension='user_mention_name',
+                filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
+                       (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
+                       ~(Dimension('user_mention_name') == 'No Mention'),
+                metric='count',
+                threshold=10)
+        
+            # asynchronously return results
+            # can be simply ```return top_mentions``` in python 3.x
+            raise gen.Return(top_mentions)
+        ```
+        
+        
+        # thetaSketches
+        Theta sketch Post aggregators are built slightly differently to normal Post Aggregators, as they have different operators.
+        Note: you must have the ```druid-datasketches``` extension loaded into your Druid cluster in order to use these.
+        See the [Druid datasketches](http://druid.io/docs/latest/development/extensions-core/datasketches-aggregators.html) documentation for details.
+        
+        ```python
+        from pydruid.client import *
+        from pydruid.utils import aggregators
+        from pydruid.utils import filters
+        from pydruid.utils import postaggregator
+        
+        query = PyDruid(url_to_druid_broker, 'druid/v2')
+        ts = query.groupby(
+            datasource='test_datasource',
+            granularity='all',
+            intervals='2016-09-01/P1M',
+            filter = ( filters.Dimension('product').in_(['product_A', 'product_B'])),
+            aggregations={
+                'product_A_users': aggregators.filtered(
+                    filters.Dimension('product') == 'product_A',
+                    aggregators.thetasketch('user_id')
+                    ),
+                'product_B_users': aggregators.filtered(
+                    filters.Dimension('product') == 'product_B',
+                    aggregators.thetasketch('user_id')
+                    )
+            },
+            post_aggregations={
+                'both_A_and_B': postaggregator.ThetaSketchEstimate(
+                    postaggregator.ThetaSketch('product_A_users') & postaggregator.ThetaSketch('product_B_users')
+                    )
+            }
+        )
+        ```
+        
+        # DB API
+        
+        ```python
+        from pydruid.db import connect
+        
+        conn = connect(host='localhost', port=8082, path='/druid/v2/sql/', scheme='http')
+        curs = conn.cursor()
+        curs.execute("""
+            SELECT place,
+                   CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
+                   CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
+              FROM places
+             LIMIT 10
+        """)
+        for row in curs:
+            print(row)
+        ```
+        
+        # SQLAlchemy
+        
+        ```python
+        from sqlalchemy import *
+        from sqlalchemy.engine import create_engine
+        from sqlalchemy.schema import *
+        
+        engine = create_engine('druid://localhost:8082/druid/v2/sql/')  # uses HTTP by default :(
+        # engine = create_engine('druid+http://localhost:8082/druid/v2/sql/')
+        # engine = create_engine('druid+https://localhost:8082/druid/v2/sql/')
+        
+        places = Table('places', MetaData(bind=engine), autoload=True)
+        print(select([func.count('*')], from_obj=places).scalar())
+        ```
+        
+        
+        ## Column headers
+        
+        In version 0.13.0 Druid SQL added support for including the column names in the
+        response which can be requested via the "header" field in the request. This
+        helps to ensure that the cursor description is defined (which is a requirement
+        for SQLAlchemy query statements) regardless on whether the result set contains
+        any rows. Historically this was problematic for result sets which contained no
+        rows at one could not infer the expected column names.
+        
+        Enabling the header can be configured via the SQLAlchemy URI by using the query
+        parameter, i.e.,
+        
+        ```python
+        engine = create_engine('druid://localhost:8082/druid/v2/sql?header=true')
+        ```
+        
+        Note the current default is `false` to ensure backwards compatibility but should
+        be set to `true` for Druid versions >= 0.13.0.
+        
+        
+        # Command line
+        
+        ```bash
+        $ pydruid http://localhost:8082/druid/v2/sql/
+        > SELECT COUNT(*) AS cnt FROM places
+          cnt
+        -----
+        12345
+        > SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES;
+        TABLE_NAME
+        ----------
+        test_table
+        COLUMNS
+        SCHEMATA
+        TABLES
+        > BYE;
+        GoodBye!
+        ```
+        
+        # Contributing
+        
+        Contributions are welcomed of course. We like to use `black` and `flake8`.
+        
+        ```bash
+        pip install -r requirements-dev.txt  # installs useful dev deps
+        pre-commit install  # installs useful commit hooks
+        ```
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
 Provides-Extra: pandas
-Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: async
-Requires-Dist: tornado; extra == "async"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy; extra == "sqlalchemy"
 Provides-Extra: cli
-Requires-Dist: pygments; extra == "cli"
-Requires-Dist: prompt_toolkit>=2.0.0; extra == "cli"
-Requires-Dist: tabulate; extra == "cli"
-
-# pydruid
-
-pydruid exposes a simple API to create, execute, and analyze [Druid](http://druid.io/) queries. pydruid can parse query results into [Pandas](http://pandas.pydata.org/) DataFrame objects for subsequent data analysis -- this offers a tight integration between [Druid](http://druid.io/), the [SciPy](http://www.scipy.org/stackspec.html) stack (for scientific computing) and [scikit-learn](http://scikit-learn.org/stable/) (for machine learning). pydruid can export query results into TSV or JSON for further processing with your favorite tool, e.g., R, Julia, Matlab, Excel. It provides both synchronous and asynchronous clients.
-
-Additionally, pydruid implements the [Python DB API 2.0](https://www.python.org/dev/peps/pep-0249/), a [SQLAlchemy dialect](http://docs.sqlalchemy.org/en/latest/dialects/), and a provides a command line interface to interact with Druid.
-
-To install:
-```python
-pip install pydruid
-# or, if you intend to use asynchronous client
-pip install pydruid[async]
-# or, if you intend to export query results into pandas
-pip install pydruid[pandas]
-# or, if you intend to do both
-pip install pydruid[async, pandas]
-# or, if you want to use the SQLAlchemy engine
-pip install pydruid[sqlalchemy]
-# or, if you want to use the CLI
-pip install pydruid[cli]
-```
-Documentation: https://pythonhosted.org/pydruid/.
-
-# examples
-
-The following exampes show how to execute and analyze the results of three types of queries: timeseries, topN, and groupby. We will use these queries to ask simple questions about twitter's public data set.
-
-## timeseries
-
-What was the average tweet length, per day, surrounding the 2014 Sochi olympics?
-
-```python
-from pydruid.client import *
-from pylab import plt
-
-query = PyDruid(druid_url_goes_here, 'druid/v2')
-
-ts = query.timeseries(
-    datasource='twitterstream',
-    granularity='day',
-    intervals='2014-02-02/p4w',
-    aggregations={'length': doublesum('tweet_length'), 'count': doublesum('count')},
-    post_aggregations={'avg_tweet_length': (Field('length') / Field('count'))},
-    filter=Dimension('first_hashtag') == 'sochi2014'
-)
-df = query.export_pandas()
-df['timestamp'] = df['timestamp'].map(lambda x: x.split('T')[0])
-df.plot(x='timestamp', y='avg_tweet_length', ylim=(80, 140), rot=20,
-        title='Sochi 2014')
-plt.ylabel('avg tweet length (chars)')
-plt.show()
-```
-
-![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/avg_tweet_length.png "Avg. tweet length")
-
-## topN
-
-Who were the top ten mentions (@user_name) during the 2014 Oscars?
-
-```python
-top = query.topn(
-    datasource='twitterstream',
-    granularity='all',
-    intervals='2014-03-03/p1d',  # utc time of 2014 oscars
-    aggregations={'count': doublesum('count')},
-    dimension='user_mention_name',
-    filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
-           (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
-           ~(Dimension('user_mention_name') == 'No Mention'),
-    metric='count',
-    threshold=10
-)
-
-df = query.export_pandas()
-print df
-
-   count                 timestamp user_mention_name
-0   1303  2014-03-03T00:00:00.000Z      TheEllenShow
-1     44  2014-03-03T00:00:00.000Z        TheAcademy
-2     21  2014-03-03T00:00:00.000Z               MTV
-3     21  2014-03-03T00:00:00.000Z         peoplemag
-4     17  2014-03-03T00:00:00.000Z               THR
-5     16  2014-03-03T00:00:00.000Z      ItsQueenElsa
-6     16  2014-03-03T00:00:00.000Z           eonline
-7     15  2014-03-03T00:00:00.000Z       PerezHilton
-8     14  2014-03-03T00:00:00.000Z     realjohngreen
-9     12  2014-03-03T00:00:00.000Z       KevinSpacey
-
-```
-
-## groupby
-
-What does the social network of users replying to other users look like?
-
-```python
-from igraph import *
-from cairo import *
-from pandas import concat
-
-group = query.groupby(
-    datasource='twitterstream',
-    granularity='hour',
-    intervals='2013-10-04/pt12h',
-    dimensions=["user_name", "reply_to_name"],
-    filter=(~(Dimension("reply_to_name") == "Not A Reply")) &
-           (Dimension("user_location") == "California"),
-    aggregations={"count": doublesum("count")}
-)
-
-df = query.export_pandas()
-
-# map names to categorical variables with a lookup table
-names = concat([df['user_name'], df['reply_to_name']]).unique()
-nameLookup = dict([pair[::-1] for pair in enumerate(names)])
-df['user_name_lookup'] = df['user_name'].map(nameLookup.get)
-df['reply_to_name_lookup'] = df['reply_to_name'].map(nameLookup.get)
-
-# create the graph with igraph
-g = Graph(len(names), directed=False)
-vertices = zip(df['user_name_lookup'], df['reply_to_name_lookup'])
-g.vs["name"] = names
-g.add_edges(vertices)
-layout = g.layout_fruchterman_reingold()
-plot(g, "tweets.png", layout=layout, vertex_size=2, bbox=(400, 400), margin=25, edge_width=1, vertex_color="blue")
-```
-
-![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/twitter_graph.png "Social Network")
-
-# asynchronous client
-```pydruid.async_client.AsyncPyDruid``` implements an asynchronous client. To achieve that, it utilizes an asynchronous
-HTTP client from ```Tornado``` framework. The asynchronous client is suitable for use with async frameworks such as Tornado
-and provides much better performance at scale. It lets you serve multiple requests at the same time, without blocking on
-Druid executing your queries.
-
-## example
-```python
-from tornado import gen
-from pydruid.async_client import AsyncPyDruid
-from pydruid.utils.aggregators import longsum
-from pydruid.utils.filters import Dimension
-
-client = AsyncPyDruid(url_to_druid_broker, 'druid/v2')
-
-@gen.coroutine
-def your_asynchronous_method_serving_top10_mentions_for_day(day
-    top_mentions = yield client.topn(
-        datasource='twitterstream',
-        granularity='all',
-        intervals="%s/p1d" % (day, ),
-        aggregations={'count': doublesum('count')},
-        dimension='user_mention_name',
-        filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
-               (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
-               ~(Dimension('user_mention_name') == 'No Mention'),
-        metric='count',
-        threshold=10)
-
-    # asynchronously return results
-    # can be simply ```return top_mentions``` in python 3.x
-    raise gen.Return(top_mentions)
-```
-
-
-# thetaSketches
-Theta sketch Post aggregators are built slightly differently to normal Post Aggregators, as they have different operators.
-Note: you must have the ```druid-datasketches``` extension loaded into your Druid cluster in order to use these.
-See the [Druid datasketches](http://druid.io/docs/latest/development/extensions-core/datasketches-aggregators.html) documentation for details.
-
-```python
-from pydruid.client import *
-from pydruid.utils import aggregators
-from pydruid.utils import filters
-from pydruid.utils import postaggregator
-
-query = PyDruid(url_to_druid_broker, 'druid/v2')
-ts = query.groupby(
-    datasource='test_datasource',
-    granularity='all',
-    intervals='2016-09-01/P1M',
-    filter = ( filters.Dimension('product').in_(['product_A', 'product_B'])),
-    aggregations={
-        'product_A_users': aggregators.filtered(
-            filters.Dimension('product') == 'product_A',
-            aggregators.thetasketch('user_id')
-            ),
-        'product_B_users': aggregators.filtered(
-            filters.Dimension('product') == 'product_B',
-            aggregators.thetasketch('user_id')
-            )
-    },
-    post_aggregations={
-        'both_A_and_B': postaggregator.ThetaSketchEstimate(
-            postaggregator.ThetaSketch('product_A_users') & postaggregator.ThetaSketch('product_B_users')
-            )
-    }
-)
-```
-
-# DB API
-
-```python
-from pydruid.db import connect
-
-conn = connect(host='localhost', port=8082, path='/druid/v2/sql/', scheme='http')
-curs = conn.cursor()
-curs.execute("""
-    SELECT place,
-           CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
-           CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
-      FROM places
-     LIMIT 10
-""")
-for row in curs:
-    print(row)
-```
-
-# SQLAlchemy
-
-```python
-from sqlalchemy import *
-from sqlalchemy.engine import create_engine
-from sqlalchemy.schema import *
-
-engine = create_engine('druid://localhost:8082/druid/v2/sql/')  # uses HTTP by default :(
-# engine = create_engine('druid+http://localhost:8082/druid/v2/sql/')
-# engine = create_engine('druid+https://localhost:8082/druid/v2/sql/')
-
-places = Table('places', MetaData(bind=engine), autoload=True)
-print(select([func.count('*')], from_obj=places).scalar())
-```
-
-
-## Column headers
-
-In version 0.13.0 Druid SQL added support for including the column names in the
-response which can be requested via the "header" field in the request. This
-helps to ensure that the cursor description is defined (which is a requirement
-for SQLAlchemy query statements) regardless on whether the result set contains
-any rows. Historically this was problematic for result sets which contained no
-rows at one could not infer the expected column names.
-
-Enabling the header can be configured via the SQLAlchemy URI by using the query
-parameter, i.e.,
-
-```python
-engine = create_engine('druid://localhost:8082/druid/v2/sql?header=true')
-```
-
-Note the current default is `false` to ensure backwards compatibility but should
-be set to `true` for Druid versions >= 0.13.0.
-
-
-# Command line
-
-```bash
-$ pydruid http://localhost:8082/druid/v2/sql/
-> SELECT COUNT(*) AS cnt FROM places
-  cnt
------
-12345
-> SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES;
-TABLE_NAME
-----------
-test_table
-COLUMNS
-SCHEMATA
-TABLES
-> BYE;
-GoodBye!
-```
-
-# Contributing
-
-Contributions are welcomed of course. We like to use `black` and `flake8`.
-
-```bash
-pip install -r requirements-dev.txt  # installs useful dev deps
-pre-commit install  # installs useful commit hooks
-```
```

### Comparing `pydruid-0.6.6/README.md` & `pydruid-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/RELEASE.md` & `pydruid-0.6.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/async_client.py` & `pydruid-0.6.7/pydruid/async_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/client.py` & `pydruid-0.6.7/pydruid/client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/console.py` & `pydruid-0.6.7/pydruid/console.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/db/__init__.py` & `pydruid-0.6.7/pydruid/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/db/api.py` & `pydruid-0.6.7/pydruid/db/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,16 +200,16 @@
         self,
         url,
         user=None,
         password=None,
         context=None,
         header=False,
         ssl_verify_cert=True,
-        proxies=None,
         ssl_client_cert=None,
+        proxies=None,
     ):
         self.url = url
         self.context = context or {}
         self.header = header
         self.user = user
         self.password = password
         self.ssl_verify_cert = ssl_verify_cert
@@ -425,15 +425,15 @@
             "[{rows}]".format(rows=rows), object_pairs_hook=OrderedDict
         ):
             yield row
 
 
 def apply_parameters(operation, parameters):
     if not parameters:
-        return operation
+        return operation % ()
 
     escaped_parameters = {key: escape(value) for key, value in parameters.items()}
     return operation % escaped_parameters
 
 
 def escape(value):
     """
```

### Comparing `pydruid-0.6.6/pydruid/db/sqlalchemy.py` & `pydruid-0.6.7/pydruid/db/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 
     @classmethod
     def dbapi(cls):
         return pydruid.db
 
     def create_connect_args(self, url):
         kwargs = {
+            **url.query,
             "host": url.host,
             "port": url.port or 8082,
             "user": url.username or None,
             "password": url.password or None,
             "path": url.database,
             "scheme": self.scheme,
             "context": self.context,
```

### Comparing `pydruid-0.6.6/pydruid/query.py` & `pydruid-0.6.7/pydruid/query.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/aggregators.py` & `pydruid-0.6.7/pydruid/utils/aggregators.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/dimensions.py` & `pydruid-0.6.7/pydruid/utils/dimensions.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/filters.py` & `pydruid-0.6.7/pydruid/utils/filters.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/having.py` & `pydruid-0.6.7/pydruid/utils/having.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/postaggregator.py` & `pydruid-0.6.7/pydruid/utils/postaggregator.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid/utils/query_utils.py` & `pydruid-0.6.7/pydruid/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/pydruid.egg-info/PKG-INFO` & `pydruid-0.6.7/pydruid.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,309 +1,302 @@
 Metadata-Version: 2.1
 Name: pydruid
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Python connector for Druid.
 Home-page: https://druid.apache.org
 Author: Druid Developers
 Author-email: druid-development@googlegroups.com
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/druid-io/pydruid/issues
 Project-URL: Documentation, https://pythonhosted.org/pydruid/
 Project-URL: Source Code, https://github.com/druid-io/pydruid
+Description: # pydruid
+        
+        pydruid exposes a simple API to create, execute, and analyze [Druid](http://druid.io/) queries. pydruid can parse query results into [Pandas](http://pandas.pydata.org/) DataFrame objects for subsequent data analysis -- this offers a tight integration between [Druid](http://druid.io/), the [SciPy](http://www.scipy.org/stackspec.html) stack (for scientific computing) and [scikit-learn](http://scikit-learn.org/stable/) (for machine learning). pydruid can export query results into TSV or JSON for further processing with your favorite tool, e.g., R, Julia, Matlab, Excel. It provides both synchronous and asynchronous clients.
+        
+        Additionally, pydruid implements the [Python DB API 2.0](https://www.python.org/dev/peps/pep-0249/), a [SQLAlchemy dialect](http://docs.sqlalchemy.org/en/latest/dialects/), and a provides a command line interface to interact with Druid.
+        
+        To install:
+        ```python
+        pip install pydruid
+        # or, if you intend to use asynchronous client
+        pip install pydruid[async]
+        # or, if you intend to export query results into pandas
+        pip install pydruid[pandas]
+        # or, if you intend to do both
+        pip install pydruid[async, pandas]
+        # or, if you want to use the SQLAlchemy engine
+        pip install pydruid[sqlalchemy]
+        # or, if you want to use the CLI
+        pip install pydruid[cli]
+        ```
+        Documentation: https://pythonhosted.org/pydruid/.
+        
+        # examples
+        
+        The following exampes show how to execute and analyze the results of three types of queries: timeseries, topN, and groupby. We will use these queries to ask simple questions about twitter's public data set.
+        
+        ## timeseries
+        
+        What was the average tweet length, per day, surrounding the 2014 Sochi olympics?
+        
+        ```python
+        from pydruid.client import *
+        from pylab import plt
+        
+        query = PyDruid(druid_url_goes_here, 'druid/v2')
+        
+        ts = query.timeseries(
+            datasource='twitterstream',
+            granularity='day',
+            intervals='2014-02-02/p4w',
+            aggregations={'length': doublesum('tweet_length'), 'count': doublesum('count')},
+            post_aggregations={'avg_tweet_length': (Field('length') / Field('count'))},
+            filter=Dimension('first_hashtag') == 'sochi2014'
+        )
+        df = query.export_pandas()
+        df['timestamp'] = df['timestamp'].map(lambda x: x.split('T')[0])
+        df.plot(x='timestamp', y='avg_tweet_length', ylim=(80, 140), rot=20,
+                title='Sochi 2014')
+        plt.ylabel('avg tweet length (chars)')
+        plt.show()
+        ```
+        
+        ![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/avg_tweet_length.png "Avg. tweet length")
+        
+        ## topN
+        
+        Who were the top ten mentions (@user_name) during the 2014 Oscars?
+        
+        ```python
+        top = query.topn(
+            datasource='twitterstream',
+            granularity='all',
+            intervals='2014-03-03/p1d',  # utc time of 2014 oscars
+            aggregations={'count': doublesum('count')},
+            dimension='user_mention_name',
+            filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
+                   (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
+                   ~(Dimension('user_mention_name') == 'No Mention'),
+            metric='count',
+            threshold=10
+        )
+        
+        df = query.export_pandas()
+        print df
+        
+           count                 timestamp user_mention_name
+        0   1303  2014-03-03T00:00:00.000Z      TheEllenShow
+        1     44  2014-03-03T00:00:00.000Z        TheAcademy
+        2     21  2014-03-03T00:00:00.000Z               MTV
+        3     21  2014-03-03T00:00:00.000Z         peoplemag
+        4     17  2014-03-03T00:00:00.000Z               THR
+        5     16  2014-03-03T00:00:00.000Z      ItsQueenElsa
+        6     16  2014-03-03T00:00:00.000Z           eonline
+        7     15  2014-03-03T00:00:00.000Z       PerezHilton
+        8     14  2014-03-03T00:00:00.000Z     realjohngreen
+        9     12  2014-03-03T00:00:00.000Z       KevinSpacey
+        
+        ```
+        
+        ## groupby
+        
+        What does the social network of users replying to other users look like?
+        
+        ```python
+        from igraph import *
+        from cairo import *
+        from pandas import concat
+        
+        group = query.groupby(
+            datasource='twitterstream',
+            granularity='hour',
+            intervals='2013-10-04/pt12h',
+            dimensions=["user_name", "reply_to_name"],
+            filter=(~(Dimension("reply_to_name") == "Not A Reply")) &
+                   (Dimension("user_location") == "California"),
+            aggregations={"count": doublesum("count")}
+        )
+        
+        df = query.export_pandas()
+        
+        # map names to categorical variables with a lookup table
+        names = concat([df['user_name'], df['reply_to_name']]).unique()
+        nameLookup = dict([pair[::-1] for pair in enumerate(names)])
+        df['user_name_lookup'] = df['user_name'].map(nameLookup.get)
+        df['reply_to_name_lookup'] = df['reply_to_name'].map(nameLookup.get)
+        
+        # create the graph with igraph
+        g = Graph(len(names), directed=False)
+        vertices = zip(df['user_name_lookup'], df['reply_to_name_lookup'])
+        g.vs["name"] = names
+        g.add_edges(vertices)
+        layout = g.layout_fruchterman_reingold()
+        plot(g, "tweets.png", layout=layout, vertex_size=2, bbox=(400, 400), margin=25, edge_width=1, vertex_color="blue")
+        ```
+        
+        ![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/twitter_graph.png "Social Network")
+        
+        # asynchronous client
+        ```pydruid.async_client.AsyncPyDruid``` implements an asynchronous client. To achieve that, it utilizes an asynchronous
+        HTTP client from ```Tornado``` framework. The asynchronous client is suitable for use with async frameworks such as Tornado
+        and provides much better performance at scale. It lets you serve multiple requests at the same time, without blocking on
+        Druid executing your queries.
+        
+        ## example
+        ```python
+        from tornado import gen
+        from pydruid.async_client import AsyncPyDruid
+        from pydruid.utils.aggregators import longsum
+        from pydruid.utils.filters import Dimension
+        
+        client = AsyncPyDruid(url_to_druid_broker, 'druid/v2')
+        
+        @gen.coroutine
+        def your_asynchronous_method_serving_top10_mentions_for_day(day
+            top_mentions = yield client.topn(
+                datasource='twitterstream',
+                granularity='all',
+                intervals="%s/p1d" % (day, ),
+                aggregations={'count': doublesum('count')},
+                dimension='user_mention_name',
+                filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
+                       (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
+                       ~(Dimension('user_mention_name') == 'No Mention'),
+                metric='count',
+                threshold=10)
+        
+            # asynchronously return results
+            # can be simply ```return top_mentions``` in python 3.x
+            raise gen.Return(top_mentions)
+        ```
+        
+        
+        # thetaSketches
+        Theta sketch Post aggregators are built slightly differently to normal Post Aggregators, as they have different operators.
+        Note: you must have the ```druid-datasketches``` extension loaded into your Druid cluster in order to use these.
+        See the [Druid datasketches](http://druid.io/docs/latest/development/extensions-core/datasketches-aggregators.html) documentation for details.
+        
+        ```python
+        from pydruid.client import *
+        from pydruid.utils import aggregators
+        from pydruid.utils import filters
+        from pydruid.utils import postaggregator
+        
+        query = PyDruid(url_to_druid_broker, 'druid/v2')
+        ts = query.groupby(
+            datasource='test_datasource',
+            granularity='all',
+            intervals='2016-09-01/P1M',
+            filter = ( filters.Dimension('product').in_(['product_A', 'product_B'])),
+            aggregations={
+                'product_A_users': aggregators.filtered(
+                    filters.Dimension('product') == 'product_A',
+                    aggregators.thetasketch('user_id')
+                    ),
+                'product_B_users': aggregators.filtered(
+                    filters.Dimension('product') == 'product_B',
+                    aggregators.thetasketch('user_id')
+                    )
+            },
+            post_aggregations={
+                'both_A_and_B': postaggregator.ThetaSketchEstimate(
+                    postaggregator.ThetaSketch('product_A_users') & postaggregator.ThetaSketch('product_B_users')
+                    )
+            }
+        )
+        ```
+        
+        # DB API
+        
+        ```python
+        from pydruid.db import connect
+        
+        conn = connect(host='localhost', port=8082, path='/druid/v2/sql/', scheme='http')
+        curs = conn.cursor()
+        curs.execute("""
+            SELECT place,
+                   CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
+                   CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
+              FROM places
+             LIMIT 10
+        """)
+        for row in curs:
+            print(row)
+        ```
+        
+        # SQLAlchemy
+        
+        ```python
+        from sqlalchemy import *
+        from sqlalchemy.engine import create_engine
+        from sqlalchemy.schema import *
+        
+        engine = create_engine('druid://localhost:8082/druid/v2/sql/')  # uses HTTP by default :(
+        # engine = create_engine('druid+http://localhost:8082/druid/v2/sql/')
+        # engine = create_engine('druid+https://localhost:8082/druid/v2/sql/')
+        
+        places = Table('places', MetaData(bind=engine), autoload=True)
+        print(select([func.count('*')], from_obj=places).scalar())
+        ```
+        
+        
+        ## Column headers
+        
+        In version 0.13.0 Druid SQL added support for including the column names in the
+        response which can be requested via the "header" field in the request. This
+        helps to ensure that the cursor description is defined (which is a requirement
+        for SQLAlchemy query statements) regardless on whether the result set contains
+        any rows. Historically this was problematic for result sets which contained no
+        rows at one could not infer the expected column names.
+        
+        Enabling the header can be configured via the SQLAlchemy URI by using the query
+        parameter, i.e.,
+        
+        ```python
+        engine = create_engine('druid://localhost:8082/druid/v2/sql?header=true')
+        ```
+        
+        Note the current default is `false` to ensure backwards compatibility but should
+        be set to `true` for Druid versions >= 0.13.0.
+        
+        
+        # Command line
+        
+        ```bash
+        $ pydruid http://localhost:8082/druid/v2/sql/
+        > SELECT COUNT(*) AS cnt FROM places
+          cnt
+        -----
+        12345
+        > SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES;
+        TABLE_NAME
+        ----------
+        test_table
+        COLUMNS
+        SCHEMATA
+        TABLES
+        > BYE;
+        GoodBye!
+        ```
+        
+        # Contributing
+        
+        Contributions are welcomed of course. We like to use `black` and `flake8`.
+        
+        ```bash
+        pip install -r requirements-dev.txt  # installs useful dev deps
+        pre-commit install  # installs useful commit hooks
+        ```
+        
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
 Provides-Extra: pandas
-Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: async
-Requires-Dist: tornado; extra == "async"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy; extra == "sqlalchemy"
 Provides-Extra: cli
-Requires-Dist: pygments; extra == "cli"
-Requires-Dist: prompt_toolkit>=2.0.0; extra == "cli"
-Requires-Dist: tabulate; extra == "cli"
-
-# pydruid
-
-pydruid exposes a simple API to create, execute, and analyze [Druid](http://druid.io/) queries. pydruid can parse query results into [Pandas](http://pandas.pydata.org/) DataFrame objects for subsequent data analysis -- this offers a tight integration between [Druid](http://druid.io/), the [SciPy](http://www.scipy.org/stackspec.html) stack (for scientific computing) and [scikit-learn](http://scikit-learn.org/stable/) (for machine learning). pydruid can export query results into TSV or JSON for further processing with your favorite tool, e.g., R, Julia, Matlab, Excel. It provides both synchronous and asynchronous clients.
-
-Additionally, pydruid implements the [Python DB API 2.0](https://www.python.org/dev/peps/pep-0249/), a [SQLAlchemy dialect](http://docs.sqlalchemy.org/en/latest/dialects/), and a provides a command line interface to interact with Druid.
-
-To install:
-```python
-pip install pydruid
-# or, if you intend to use asynchronous client
-pip install pydruid[async]
-# or, if you intend to export query results into pandas
-pip install pydruid[pandas]
-# or, if you intend to do both
-pip install pydruid[async, pandas]
-# or, if you want to use the SQLAlchemy engine
-pip install pydruid[sqlalchemy]
-# or, if you want to use the CLI
-pip install pydruid[cli]
-```
-Documentation: https://pythonhosted.org/pydruid/.
-
-# examples
-
-The following exampes show how to execute and analyze the results of three types of queries: timeseries, topN, and groupby. We will use these queries to ask simple questions about twitter's public data set.
-
-## timeseries
-
-What was the average tweet length, per day, surrounding the 2014 Sochi olympics?
-
-```python
-from pydruid.client import *
-from pylab import plt
-
-query = PyDruid(druid_url_goes_here, 'druid/v2')
-
-ts = query.timeseries(
-    datasource='twitterstream',
-    granularity='day',
-    intervals='2014-02-02/p4w',
-    aggregations={'length': doublesum('tweet_length'), 'count': doublesum('count')},
-    post_aggregations={'avg_tweet_length': (Field('length') / Field('count'))},
-    filter=Dimension('first_hashtag') == 'sochi2014'
-)
-df = query.export_pandas()
-df['timestamp'] = df['timestamp'].map(lambda x: x.split('T')[0])
-df.plot(x='timestamp', y='avg_tweet_length', ylim=(80, 140), rot=20,
-        title='Sochi 2014')
-plt.ylabel('avg tweet length (chars)')
-plt.show()
-```
-
-![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/avg_tweet_length.png "Avg. tweet length")
-
-## topN
-
-Who were the top ten mentions (@user_name) during the 2014 Oscars?
-
-```python
-top = query.topn(
-    datasource='twitterstream',
-    granularity='all',
-    intervals='2014-03-03/p1d',  # utc time of 2014 oscars
-    aggregations={'count': doublesum('count')},
-    dimension='user_mention_name',
-    filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
-           (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
-           ~(Dimension('user_mention_name') == 'No Mention'),
-    metric='count',
-    threshold=10
-)
-
-df = query.export_pandas()
-print df
-
-   count                 timestamp user_mention_name
-0   1303  2014-03-03T00:00:00.000Z      TheEllenShow
-1     44  2014-03-03T00:00:00.000Z        TheAcademy
-2     21  2014-03-03T00:00:00.000Z               MTV
-3     21  2014-03-03T00:00:00.000Z         peoplemag
-4     17  2014-03-03T00:00:00.000Z               THR
-5     16  2014-03-03T00:00:00.000Z      ItsQueenElsa
-6     16  2014-03-03T00:00:00.000Z           eonline
-7     15  2014-03-03T00:00:00.000Z       PerezHilton
-8     14  2014-03-03T00:00:00.000Z     realjohngreen
-9     12  2014-03-03T00:00:00.000Z       KevinSpacey
-
-```
-
-## groupby
-
-What does the social network of users replying to other users look like?
-
-```python
-from igraph import *
-from cairo import *
-from pandas import concat
-
-group = query.groupby(
-    datasource='twitterstream',
-    granularity='hour',
-    intervals='2013-10-04/pt12h',
-    dimensions=["user_name", "reply_to_name"],
-    filter=(~(Dimension("reply_to_name") == "Not A Reply")) &
-           (Dimension("user_location") == "California"),
-    aggregations={"count": doublesum("count")}
-)
-
-df = query.export_pandas()
-
-# map names to categorical variables with a lookup table
-names = concat([df['user_name'], df['reply_to_name']]).unique()
-nameLookup = dict([pair[::-1] for pair in enumerate(names)])
-df['user_name_lookup'] = df['user_name'].map(nameLookup.get)
-df['reply_to_name_lookup'] = df['reply_to_name'].map(nameLookup.get)
-
-# create the graph with igraph
-g = Graph(len(names), directed=False)
-vertices = zip(df['user_name_lookup'], df['reply_to_name_lookup'])
-g.vs["name"] = names
-g.add_edges(vertices)
-layout = g.layout_fruchterman_reingold()
-plot(g, "tweets.png", layout=layout, vertex_size=2, bbox=(400, 400), margin=25, edge_width=1, vertex_color="blue")
-```
-
-![alt text](https://github.com/metamx/pydruid/raw/master/docs/figures/twitter_graph.png "Social Network")
-
-# asynchronous client
-```pydruid.async_client.AsyncPyDruid``` implements an asynchronous client. To achieve that, it utilizes an asynchronous
-HTTP client from ```Tornado``` framework. The asynchronous client is suitable for use with async frameworks such as Tornado
-and provides much better performance at scale. It lets you serve multiple requests at the same time, without blocking on
-Druid executing your queries.
-
-## example
-```python
-from tornado import gen
-from pydruid.async_client import AsyncPyDruid
-from pydruid.utils.aggregators import longsum
-from pydruid.utils.filters import Dimension
-
-client = AsyncPyDruid(url_to_druid_broker, 'druid/v2')
-
-@gen.coroutine
-def your_asynchronous_method_serving_top10_mentions_for_day(day
-    top_mentions = yield client.topn(
-        datasource='twitterstream',
-        granularity='all',
-        intervals="%s/p1d" % (day, ),
-        aggregations={'count': doublesum('count')},
-        dimension='user_mention_name',
-        filter=(Dimension('user_lang') == 'en') & (Dimension('first_hashtag') == 'oscars') &
-               (Dimension('user_time_zone') == 'Pacific Time (US & Canada)') &
-               ~(Dimension('user_mention_name') == 'No Mention'),
-        metric='count',
-        threshold=10)
-
-    # asynchronously return results
-    # can be simply ```return top_mentions``` in python 3.x
-    raise gen.Return(top_mentions)
-```
-
-
-# thetaSketches
-Theta sketch Post aggregators are built slightly differently to normal Post Aggregators, as they have different operators.
-Note: you must have the ```druid-datasketches``` extension loaded into your Druid cluster in order to use these.
-See the [Druid datasketches](http://druid.io/docs/latest/development/extensions-core/datasketches-aggregators.html) documentation for details.
-
-```python
-from pydruid.client import *
-from pydruid.utils import aggregators
-from pydruid.utils import filters
-from pydruid.utils import postaggregator
-
-query = PyDruid(url_to_druid_broker, 'druid/v2')
-ts = query.groupby(
-    datasource='test_datasource',
-    granularity='all',
-    intervals='2016-09-01/P1M',
-    filter = ( filters.Dimension('product').in_(['product_A', 'product_B'])),
-    aggregations={
-        'product_A_users': aggregators.filtered(
-            filters.Dimension('product') == 'product_A',
-            aggregators.thetasketch('user_id')
-            ),
-        'product_B_users': aggregators.filtered(
-            filters.Dimension('product') == 'product_B',
-            aggregators.thetasketch('user_id')
-            )
-    },
-    post_aggregations={
-        'both_A_and_B': postaggregator.ThetaSketchEstimate(
-            postaggregator.ThetaSketch('product_A_users') & postaggregator.ThetaSketch('product_B_users')
-            )
-    }
-)
-```
-
-# DB API
-
-```python
-from pydruid.db import connect
-
-conn = connect(host='localhost', port=8082, path='/druid/v2/sql/', scheme='http')
-curs = conn.cursor()
-curs.execute("""
-    SELECT place,
-           CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
-           CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
-      FROM places
-     LIMIT 10
-""")
-for row in curs:
-    print(row)
-```
-
-# SQLAlchemy
-
-```python
-from sqlalchemy import *
-from sqlalchemy.engine import create_engine
-from sqlalchemy.schema import *
-
-engine = create_engine('druid://localhost:8082/druid/v2/sql/')  # uses HTTP by default :(
-# engine = create_engine('druid+http://localhost:8082/druid/v2/sql/')
-# engine = create_engine('druid+https://localhost:8082/druid/v2/sql/')
-
-places = Table('places', MetaData(bind=engine), autoload=True)
-print(select([func.count('*')], from_obj=places).scalar())
-```
-
-
-## Column headers
-
-In version 0.13.0 Druid SQL added support for including the column names in the
-response which can be requested via the "header" field in the request. This
-helps to ensure that the cursor description is defined (which is a requirement
-for SQLAlchemy query statements) regardless on whether the result set contains
-any rows. Historically this was problematic for result sets which contained no
-rows at one could not infer the expected column names.
-
-Enabling the header can be configured via the SQLAlchemy URI by using the query
-parameter, i.e.,
-
-```python
-engine = create_engine('druid://localhost:8082/druid/v2/sql?header=true')
-```
-
-Note the current default is `false` to ensure backwards compatibility but should
-be set to `true` for Druid versions >= 0.13.0.
-
-
-# Command line
-
-```bash
-$ pydruid http://localhost:8082/druid/v2/sql/
-> SELECT COUNT(*) AS cnt FROM places
-  cnt
------
-12345
-> SELECT TABLE_NAME FROM INFORMATION_SCHEMA.TABLES;
-TABLE_NAME
-----------
-test_table
-COLUMNS
-SCHEMATA
-TABLES
-> BYE;
-GoodBye!
-```
-
-# Contributing
-
-Contributions are welcomed of course. We like to use `black` and `flake8`.
-
-```bash
-pip install -r requirements-dev.txt  # installs useful dev deps
-pre-commit install  # installs useful commit hooks
-```
```

### Comparing `pydruid-0.6.6/requirements-dev.txt` & `pydruid-0.6.7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/requirements.txt` & `pydruid-0.6.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/setup.py` & `pydruid-0.6.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 }
 
 with io.open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pydruid",
-    version="0.6.6",
+    version="0.6.7",
     author="Druid Developers",
     author_email="druid-development@googlegroups.com",
     packages=find_packages(),
     url="https://druid.apache.org",
     project_urls={
         "Bug Tracker": "https://github.com/druid-io/pydruid/issues",
         "Documentation": "https://pythonhosted.org/pydruid/",
```

### Comparing `pydruid-0.6.6/tests/test_async_client.py` & `pydruid-0.6.7/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/tests/test_client.py` & `pydruid-0.6.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydruid-0.6.6/tests/test_query.py` & `pydruid-0.6.7/tests/test_query.py`

 * *Files identical despite different names*

