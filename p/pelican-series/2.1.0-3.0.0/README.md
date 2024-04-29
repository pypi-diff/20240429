# Comparing `tmp/pelican-series-2.1.0.tar.gz` & `tmp/pelican_series-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-series-2.1.0.tar", max compression
+gzip compressed data, was "pelican_series-3.0.0.tar", max compression
```

## Comparing `pelican-series-2.1.0.tar` & `pelican_series-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     4170 2021-05-04 11:12:02.186372 pelican-series-2.1.0/README.md
--rw-r--r--   0        0        0       30 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/__init__.py
--rw-r--r--   0        0        0     1335 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/conftest.py
--rw-r--r--   0        0        0     2218 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/series.py
--rw-r--r--   0        0        0     1715 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_articles_no_index.py
--rw-r--r--   0        0        0     1438 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_articles_with_index.py
--rw-r--r--   0        0        0      670 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_articles_with_index_over_10.py
--rw-r--r--   0        0        0      146 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_no_index/series_article_1.md
--rw-r--r--   0        0        0      146 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_no_index/series_article_2.md
--rw-r--r--   0        0        0      146 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_no_index/series_article_3.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index/series_article_1.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index/series_article_2.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index/series_article_3.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_1.md
--rw-r--r--   0        0        0      165 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_10.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_2.md
--rw-r--r--   0        0        0      162 2021-05-04 11:12:02.186372 pelican-series-2.1.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_3.md
--rw-r--r--   0        0        0     2003 2021-05-04 11:12:14.658472 pelican-series-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5292 2021-05-04 11:12:16.578561 pelican-series-2.1.0/setup.py
--rw-r--r--   0        0        0     5573 2021-05-04 11:12:16.578999 pelican-series-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5631 2024-04-29 10:40:19.727527 pelican_series-3.0.0/README.md
+-rw-r--r--   0        0        0       30 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/__init__.py
+-rw-r--r--   0        0        0     1335 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/conftest.py
+-rw-r--r--   0        0        0     3306 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/series.py
+-rw-r--r--   0        0        0     1715 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_articles_no_index.py
+-rw-r--r--   0        0        0     1438 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_articles_with_index.py
+-rw-r--r--   0        0        0      670 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_articles_with_index_over_10.py
+-rw-r--r--   0        0        0      146 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_no_index/series_article_1.md
+-rw-r--r--   0        0        0      146 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_no_index/series_article_2.md
+-rw-r--r--   0        0        0      146 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_no_index/series_article_3.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index/series_article_1.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index/series_article_2.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index/series_article_3.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_1.md
+-rw-r--r--   0        0        0      165 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_10.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_2.md
+-rw-r--r--   0        0        0      162 2024-04-29 10:40:19.731527 pelican_series-3.0.0/pelican/plugins/series/test_data/articles_with_index_over_10/series_article_3.md
+-rw-r--r--   0        0        0     2089 2024-04-29 10:40:35.915552 pelican_series-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 pelican_series-3.0.0/PKG-INFO
```

### Comparing `pelican-series-2.1.0/README.md` & `pelican_series-3.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Series: A Plugin for Pelican
 ============================
 
-[![Build Status](https://img.shields.io/github/workflow/status/pelican-plugins/series/build)](https://github.com/pelican-plugins/series/actions)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/series/main.yml?branch=main)](https://github.com/pelican-plugins/series/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-series)](https://pypi.org/project/pelican-series/)
 ![License](https://img.shields.io/pypi/l/pelican-series?color=blue)
 
 Series is a Pelican plugin that joins multiple posts into a series. Globally, it provides a list of all the series, and for each article it provides a list of all articles in the same series and links to the next and previous articles in the series.
 
 Installation
 ------------
 
 This plugin can be installed via:
 
     python -m pip install pelican-series
 
+As long as you have not explicitly added a `PLUGINS` setting to your Pelican settings file, then the newly-installed plugin should be automatically detected and enabled. Otherwise, you must add `series` to your existing `PLUGINS` list. For more information, please see the [How to Use Plugins](https://docs.getpelican.com/en/latest/plugins.html#how-to-use-plugins) documentation.
+
 Usage
 -----
 
 In order to mark reStructuredText-formatted posts as part of a series, use the `:series:` metadata:
 
     :series:  NAME_OF_THIS_SERIES
 
 Or, for Markdown-formatted content:
 
     Series: NAME_OF_THIS_SERIES
 
-The plugin collects all articles belonging to the same series and provides series-related variables that you can use in your template.
+The plugin collects all articles or pages belonging to the same series and provides series-related variables that you can use in your template.
+
+Articles and pages
+------------------
+
+This plugin works both with articles and pages. As Pelican uses the specific variable `article` for article templates and `page` for page templates it is complicated to give examples that work for both cases. In the following documentation all example will mention `article.` (e.g. `article.series`, `article.title`) but the code works in the same way with `page` (e.g. `page.series`, `page.title`).
+
+Article series and page series are created separately, so even if an article and a page have the same series they won't appear together.
 
 Indexing
 --------
 
-By default, articles in a series are ordered by date and then automatically numbered.
+By default, articles in a series are ordered by date and then automatically numbered. Pages in a series are ordered by title and automatically numbered.
 
-If you want to force a given order, specify `:series_index:` (reST) or `series_index:` (Markdown) in the article metadata, starting from 1. All articles with this enforced index are put at the beginning of the series and ordered according to the index itself. All the remaining articles come after them, ordered by date.
+If you want to force a given order, specify `:series_index:` (reST) or `series_index:` (Markdown) in the article metadata, starting from 1. All articles with this enforced index are put at the beginning of the series and ordered according to the index itself. All the remaining articles come after them, ordered with the default ordering (date for articles and title for pages).
 
 The plugin provides the following variables to your templates:
 
 * `article.series.name` is the name of the series as specified in the article metadata
 * `article.series.index` is the index of the current article inside the series
 * `article.series.all` is an ordered list of all articles in the series (including the current one)
 * `article.series.all_previous` is an ordered list of the articles published before the current one
@@ -58,15 +67,17 @@
     </ol>
 {% endif %}
 ```
 
 Global Context
 --------------
 
-The plugin also adds the key `series` to the global context, which is a dictionary of all series names (as keys) and articles (as values). You can use that to list all the series of articles in your site, for example
+**Warning**: in version 3 the global key `series` has been renamed to `article_series` to differentiate it from the new global key `page_series`.
+
+The plugin also adds the keys `article_series` and `page_series` to the global context. They are dictionaries of all series names (as keys) and items (as values). You can use that to list all the series in your site, for example
 
 ```html+jinja
 {% for series_name, series_articles in series.items() %}
 {% set article = series_articles[0] %}
 <article class="card">
 	<a href="{{ article.url }}" class="image">
 		<img src="/images/{{ article.image }}.jpg" alt="{{ article.image }}" />
@@ -77,14 +88,16 @@
      		<li><a href="{{ article.url }}" class="button">Start</a></li>
      	</ul>
 	</div>
 </article>
 {% endfor %}
 ```
 
+As it is not possible to create pages from plugins you can leverage it to create a page for a specific series, even though you have to hard code the name of the series in the template.
+
 Contributing
 ------------
 
 Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
 
 To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
```

#### html2text {}

```diff
@@ -1,54 +1,73 @@
 Series: A Plugin for Pelican ============================ [![Build Status]
-(https://img.shields.io/github/workflow/status/pelican-plugins/series/build)]
-(https://github.com/pelican-plugins/series/actions) [![PyPI Version](https://
-img.shields.io/pypi/v/pelican-series)](https://pypi.org/project/pelican-series/
-) ![License](https://img.shields.io/pypi/l/pelican-series?color=blue) Series is
-a Pelican plugin that joins multiple posts into a series. Globally, it provides
-a list of all the series, and for each article it provides a list of all
-articles in the same series and links to the next and previous articles in the
-series. Installation ------------ This plugin can be installed via: python -
-m pip install pelican-series Usage ----- In order to mark reStructuredText-
-formatted posts as part of a series, use the `:series:` metadata: :series:
-NAME_OF_THIS_SERIES Or, for Markdown-formatted content: Series:
-NAME_OF_THIS_SERIES The plugin collects all articles belonging to the same
-series and provides series-related variables that you can use in your template.
-Indexing -------- By default, articles in a series are ordered by date and then
-automatically numbered. If you want to force a given order, specify `:
-series_index:` (reST) or `series_index:` (Markdown) in the article metadata,
-starting from 1. All articles with this enforced index are put at the beginning
-of the series and ordered according to the index itself. All the remaining
-articles come after them, ordered by date. The plugin provides the following
-variables to your templates: * `article.series.name` is the name of the series
-as specified in the article metadata * `article.series.index` is the index of
-the current article inside the series * `article.series.all` is an ordered list
-of all articles in the series (including the current one) *
+(https://img.shields.io/github/actions/workflow/status/pelican-plugins/series/
+main.yml?branch=main)](https://github.com/pelican-plugins/series/actions) [!
+[PyPI Version](https://img.shields.io/pypi/v/pelican-series)](https://pypi.org/
+project/pelican-series/) ![License](https://img.shields.io/pypi/l/pelican-
+series?color=blue) Series is a Pelican plugin that joins multiple posts into a
+series. Globally, it provides a list of all the series, and for each article it
+provides a list of all articles in the same series and links to the next and
+previous articles in the series. Installation ------------ This plugin can be
+installed via: python -m pip install pelican-series As long as you have not
+explicitly added a `PLUGINS` setting to your Pelican settings file, then the
+newly-installed plugin should be automatically detected and enabled. Otherwise,
+you must add `series` to your existing `PLUGINS` list. For more information,
+please see the [How to Use Plugins](https://docs.getpelican.com/en/latest/
+plugins.html#how-to-use-plugins) documentation. Usage ----- In order to mark
+reStructuredText-formatted posts as part of a series, use the `:series:
+` metadata: :series: NAME_OF_THIS_SERIES Or, for Markdown-formatted content:
+Series: NAME_OF_THIS_SERIES The plugin collects all articles or pages belonging
+to the same series and provides series-related variables that you can use in
+your template. Articles and pages ------------------ This plugin works both
+with articles and pages. As Pelican uses the specific variable `article` for
+article templates and `page` for page templates it is complicated to give
+examples that work for both cases. In the following documentation all example
+will mention `article.` (e.g. `article.series`, `article.title`) but the code
+works in the same way with `page` (e.g. `page.series`, `page.title`). Article
+series and page series are created separately, so even if an article and a page
+have the same series they won't appear together. Indexing -------- By default,
+articles in a series are ordered by date and then automatically numbered. Pages
+in a series are ordered by title and automatically numbered. If you want to
+force a given order, specify `:series_index:` (reST) or `series_index:`
+(Markdown) in the article metadata, starting from 1. All articles with this
+enforced index are put at the beginning of the series and ordered according to
+the index itself. All the remaining articles come after them, ordered with the
+default ordering (date for articles and title for pages). The plugin provides
+the following variables to your templates: * `article.series.name` is the name
+of the series as specified in the article metadata * `article.series.index` is
+the index of the current article inside the series * `article.series.all` is an
+ordered list of all articles in the series (including the current one) *
 `article.series.all_previous` is an ordered list of the articles published
 before the current one * `article.series.all_next` is an ordered list of the
 articles published after the current one * `article.series.previous` is the
 previous article in the series (a shortcut to `article.series.all_previous[-
 1]`) or `None` for the first article * `article.series.next` is the next
 article in the series (a shortcut to `article.series.all_next[0]`) or `None`
 for the last one For example: ```html+jinja {% if article.series %}
 This post is part {{ article.series.index }} of the "{{ article.series.name }}"
 series:
    1. {% for part_article in article.series.all %}
    2. % if part_article == article %}class="active"{% endif %}> _{
       _{_ _p_a_r_t___a_r_t_i_c_l_e_._t_i_t_l_e_ _}_}
    3. {% endfor %}
-{% endif %} ``` Global Context -------------- The plugin also adds the key
-`series` to the global context, which is a dictionary of all series names (as
-keys) and articles (as values). You can use that to list all the series of
-articles in your site, for example ```html+jinja {% for series_name,
+{% endif %} ``` Global Context -------------- **Warning**: in version 3 the
+global key `series` has been renamed to `article_series` to differentiate it
+from the new global key `page_series`. The plugin also adds the keys
+`article_series` and `page_series` to the global context. They are dictionaries
+of all series names (as keys) and items (as values). You can use that to list
+all the series in your site, for example ```html+jinja {% for series_name,
 series_articles in series.items() %} {% set article = series_articles[0] %}_[_{
 _{_ _a_r_t_i_c_l_e_._i_m_a_g_e_ _}_}_]
 _**_**_**_**_ _{{_{{_ _ss_ee_rr_ii_ee_ss____nn_aa_mm_ee_ _}}_}}_ _**_**_**_**
     * _S_t_a_r_t
-{% endfor %} ``` Contributing ------------ Contributions are welcome and much
-appreciated. Every little bit helps. You can contribute by improving the
-documentation, adding missing features, and fixing bugs. You can also help out
-by reviewing and commenting on [existing issues][]. To start contributing to
-this plugin, review the [Contributing to Pelican][] documentation, beginning
-with the **Contributing Code** section. [existing issues]: https://github.com/
-pelican-plugins/series/issues [Contributing to Pelican]: https://
-docs.getpelican.com/en/latest/contribute.html License ------- This project is
-licensed under the AGPL 3.0 license.
+{% endfor %} ``` As it is not possible to create pages from plugins you can
+leverage it to create a page for a specific series, even though you have to
+hard code the name of the series in the template. Contributing -----------
+- Contributions are welcome and much appreciated. Every little bit helps. You
+can contribute by improving the documentation, adding missing features, and
+fixing bugs. You can also help out by reviewing and commenting on [existing
+issues][]. To start contributing to this plugin, review the [Contributing to
+Pelican][] documentation, beginning with the **Contributing Code** section.
+[existing issues]: https://github.com/pelican-plugins/series/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/
+contribute.html License ------- This project is licensed under the AGPL 3.0
+license.
```

### Comparing `pelican-series-2.1.0/pelican/plugins/series/conftest.py` & `pelican_series-3.0.0/pelican/plugins/series/conftest.py`

 * *Files identical despite different names*

### Comparing `pelican-series-2.1.0/pelican/plugins/series/test_articles_no_index.py` & `pelican_series-3.0.0/pelican/plugins/series/test_articles_no_index.py`

 * *Files identical despite different names*

### Comparing `pelican-series-2.1.0/pelican/plugins/series/test_articles_with_index.py` & `pelican_series-3.0.0/pelican/plugins/series/test_articles_with_index.py`

 * *Files identical despite different names*

### Comparing `pelican-series-2.1.0/pelican/plugins/series/test_articles_with_index_over_10.py` & `pelican_series-3.0.0/pelican/plugins/series/test_articles_with_index_over_10.py`

 * *Files identical despite different names*

### Comparing `pelican-series-2.1.0/pyproject.toml` & `pelican_series-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-series"
-version = "2.1.0"
+version = "3.0.0"
 description = "Series is a Pelican plugin that joins multiple posts into a series"
 authors = ["Leonardo Giordani <giordani.leonardo@gmail.com>", "Justin Mayer <entroP@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "series", "multiple"]
 repository = "https://github.com/pelican-plugins/series"
 documentation = "https://docs.getpelican.com"
@@ -24,39 +24,41 @@
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/pelican-plugins/series/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.8.1,<4.0"
 pelican = ">=4.5"
 markdown = {version = ">=3.2", optional = true}
+# Avoid PyPI/Poetry problem: https://github.com/python-poetry/poetry/issues/9293
+docutils = "!=0.21.post1"
 
 [tool.poetry.dev-dependencies]
-black = {version = "^21.4b2", allow-prereleases = true}
-flake8 = "^3.9"
-flake8-black = "^0.2.0"
-invoke = "^1.3"
-isort = "^5.4"
+black = "^23.0"
+flake8 = "^6.0"
+flake8-black = "^0.3"
+invoke = "^2.0"
+isort = "^5.12"
 livereload = "^2.6"
 markdown = "^3.2"
 pytest = "^6.0"
 pytest-cov = "^2.8"
-pytest-pythonpath = "^0.7.3"
-pytest-sugar = "^0.9.4"
+pytest-pythonpath = "^0.7.4"
+pytest-sugar = "^0.9.6"
 Werkzeug = "^1.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
 project-name = "Series"
 git-username = "botpub"
-git-email = "botpub@autopub.rocks"
+git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.isort]
 # Maintain compatibility with Black
 profile = "black"
 multi_line_output = 3
```

### Comparing `pelican-series-2.1.0/setup.py` & `pelican_series-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,331 +1,446 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2770 656c 6963 616e 272c 2027   \.['pelican', '
-00000050: 7065 6c69 6361 6e2e 706c 7567 696e 732e  pelican.plugins.
-00000060: 7365 7269 6573 275d 0a0a 7061 636b 6167  series']..packag
-00000070: 655f 6461 7461 203d 205c 0a7b 2727 3a20  e_data = \.{'': 
-00000080: 5b27 2a27 5d2c 0a20 2770 656c 6963 616e  ['*'],. 'pelican
-00000090: 2e70 6c75 6769 6e73 2e73 6572 6965 7327  .plugins.series'
-000000a0: 3a20 5b27 7465 7374 5f64 6174 612f 6172  : ['test_data/ar
-000000b0: 7469 636c 6573 5f6e 6f5f 696e 6465 782f  ticles_no_index/
-000000c0: 2a27 2c0a 2020 2020 2020 2020 2020 2020  *',.            
-000000d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000e0: 2774 6573 745f 6461 7461 2f61 7274 6963  'test_data/artic
-000000f0: 6c65 735f 7769 7468 5f69 6e64 6578 2f2a  les_with_index/*
-00000100: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00000110: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000120: 7465 7374 5f64 6174 612f 6172 7469 636c  test_data/articl
-00000130: 6573 5f77 6974 685f 696e 6465 785f 6f76  es_with_index_ov
-00000140: 6572 5f31 302f 2a27 5d7d 0a0a 696e 7374  er_10/*']}..inst
-00000150: 616c 6c5f 7265 7175 6972 6573 203d 205c  all_requires = \
-00000160: 0a5b 2770 656c 6963 616e 3e3d 342e 3527  .['pelican>=4.5'
-00000170: 5d0a 0a65 7874 7261 735f 7265 7175 6972  ]..extras_requir
-00000180: 6520 3d20 5c0a 7b27 6d61 726b 646f 776e  e = \.{'markdown
-00000190: 273a 205b 276d 6172 6b64 6f77 6e3e 3d33  ': ['markdown>=3
-000001a0: 2e32 275d 7d0a 0a73 6574 7570 5f6b 7761  .2']}..setup_kwa
-000001b0: 7267 7320 3d20 7b0a 2020 2020 276e 616d  rgs = {.    'nam
-000001c0: 6527 3a20 2770 656c 6963 616e 2d73 6572  e': 'pelican-ser
-000001d0: 6965 7327 2c0a 2020 2020 2776 6572 7369  ies',.    'versi
-000001e0: 6f6e 273a 2027 322e 312e 3027 2c0a 2020  on': '2.1.0',.  
-000001f0: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-00000200: 2027 5365 7269 6573 2069 7320 6120 5065   'Series is a Pe
-00000210: 6c69 6361 6e20 706c 7567 696e 2074 6861  lican plugin tha
-00000220: 7420 6a6f 696e 7320 6d75 6c74 6970 6c65  t joins multiple
-00000230: 2070 6f73 7473 2069 6e74 6f20 6120 7365   posts into a se
-00000240: 7269 6573 272c 0a20 2020 2027 6c6f 6e67  ries',.    'long
-00000250: 5f64 6573 6372 6970 7469 6f6e 273a 2027  _description': '
-00000260: 5365 7269 6573 3a20 4120 506c 7567 696e  Series: A Plugin
-00000270: 2066 6f72 2050 656c 6963 616e 5c6e 3d3d   for Pelican\n==
-00000280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000290: 3d3d 3d3d 3d3d 3d3d 3d3d 5c6e 5c6e 5b21  ==========\n\n[!
-000002a0: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
-000002b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000002c0: 6473 2e69 6f2f 6769 7468 7562 2f77 6f72  ds.io/github/wor
-000002d0: 6b66 6c6f 772f 7374 6174 7573 2f70 656c  kflow/status/pel
-000002e0: 6963 616e 2d70 6c75 6769 6e73 2f73 6572  ican-plugins/ser
-000002f0: 6965 732f 6275 696c 6429 5d28 6874 7470  ies/build)](http
-00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000310: 656c 6963 616e 2d70 6c75 6769 6e73 2f73  elican-plugins/s
-00000320: 6572 6965 732f 6163 7469 6f6e 7329 5c6e  eries/actions)\n
-00000330: 5b21 5b50 7950 4920 5665 7273 696f 6e5d  [![PyPI Version]
-00000340: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000350: 656c 6473 2e69 6f2f 7079 7069 2f76 2f70  elds.io/pypi/v/p
-00000360: 656c 6963 616e 2d73 6572 6965 7329 5d28  elican-series)](
-00000370: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000380: 2f70 726f 6a65 6374 2f70 656c 6963 616e  /project/pelican
-00000390: 2d73 6572 6965 732f 295c 6e21 5b4c 6963  -series/)\n![Lic
-000003a0: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
-000003b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000003c0: 692f 6c2f 7065 6c69 6361 6e2d 7365 7269  i/l/pelican-seri
-000003d0: 6573 3f63 6f6c 6f72 3d62 6c75 6529 5c6e  es?color=blue)\n
-000003e0: 5c6e 5365 7269 6573 2069 7320 6120 5065  \nSeries is a Pe
-000003f0: 6c69 6361 6e20 706c 7567 696e 2074 6861  lican plugin tha
-00000400: 7420 6a6f 696e 7320 6d75 6c74 6970 6c65  t joins multiple
-00000410: 2070 6f73 7473 2069 6e74 6f20 6120 7365   posts into a se
-00000420: 7269 6573 2e20 476c 6f62 616c 6c79 2c20  ries. Globally, 
-00000430: 6974 2070 726f 7669 6465 7320 6120 6c69  it provides a li
-00000440: 7374 206f 6620 616c 6c20 7468 6520 7365  st of all the se
-00000450: 7269 6573 2c20 616e 6420 666f 7220 6561  ries, and for ea
-00000460: 6368 2061 7274 6963 6c65 2069 7420 7072  ch article it pr
-00000470: 6f76 6964 6573 2061 206c 6973 7420 6f66  ovides a list of
-00000480: 2061 6c6c 2061 7274 6963 6c65 7320 696e   all articles in
-00000490: 2074 6865 2073 616d 6520 7365 7269 6573   the same series
-000004a0: 2061 6e64 206c 696e 6b73 2074 6f20 7468   and links to th
-000004b0: 6520 6e65 7874 2061 6e64 2070 7265 7669  e next and previ
-000004c0: 6f75 7320 6172 7469 636c 6573 2069 6e20  ous articles in 
-000004d0: 7468 6520 7365 7269 6573 2e5c 6e5c 6e49  the series.\n\nI
-000004e0: 6e73 7461 6c6c 6174 696f 6e5c 6e2d 2d2d  nstallation\n---
-000004f0: 2d2d 2d2d 2d2d 2d2d 2d5c 6e5c 6e54 6869  ---------\n\nThi
-00000500: 7320 706c 7567 696e 2063 616e 2062 6520  s plugin can be 
-00000510: 696e 7374 616c 6c65 6420 7669 613a 5c6e  installed via:\n
-00000520: 5c6e 2020 2020 7079 7468 6f6e 202d 6d20  \n    python -m 
-00000530: 7069 7020 696e 7374 616c 6c20 7065 6c69  pip install peli
-00000540: 6361 6e2d 7365 7269 6573 5c6e 5c6e 5573  can-series\n\nUs
-00000550: 6167 655c 6e2d 2d2d 2d2d 5c6e 5c6e 496e  age\n-----\n\nIn
-00000560: 206f 7264 6572 2074 6f20 6d61 726b 2072   order to mark r
-00000570: 6553 7472 7563 7475 7265 6454 6578 742d  eStructuredText-
-00000580: 666f 726d 6174 7465 6420 706f 7374 7320  formatted posts 
-00000590: 6173 2070 6172 7420 6f66 2061 2073 6572  as part of a ser
-000005a0: 6965 732c 2075 7365 2074 6865 2060 3a73  ies, use the `:s
-000005b0: 6572 6965 733a 6020 6d65 7461 6461 7461  eries:` metadata
-000005c0: 3a5c 6e5c 6e20 2020 203a 7365 7269 6573  :\n\n    :series
-000005d0: 3a20 204e 414d 455f 4f46 5f54 4849 535f  :  NAME_OF_THIS_
-000005e0: 5345 5249 4553 5c6e 5c6e 4f72 2c20 666f  SERIES\n\nOr, fo
-000005f0: 7220 4d61 726b 646f 776e 2d66 6f72 6d61  r Markdown-forma
-00000600: 7474 6564 2063 6f6e 7465 6e74 3a5c 6e5c  tted content:\n\
-00000610: 6e20 2020 2053 6572 6965 733a 204e 414d  n    Series: NAM
-00000620: 455f 4f46 5f54 4849 535f 5345 5249 4553  E_OF_THIS_SERIES
-00000630: 5c6e 5c6e 5468 6520 706c 7567 696e 2063  \n\nThe plugin c
-00000640: 6f6c 6c65 6374 7320 616c 6c20 6172 7469  ollects all arti
-00000650: 636c 6573 2062 656c 6f6e 6769 6e67 2074  cles belonging t
-00000660: 6f20 7468 6520 7361 6d65 2073 6572 6965  o the same serie
-00000670: 7320 616e 6420 7072 6f76 6964 6573 2073  s and provides s
-00000680: 6572 6965 732d 7265 6c61 7465 6420 7661  eries-related va
-00000690: 7269 6162 6c65 7320 7468 6174 2079 6f75  riables that you
-000006a0: 2063 616e 2075 7365 2069 6e20 796f 7572   can use in your
-000006b0: 2074 656d 706c 6174 652e 5c6e 5c6e 496e   template.\n\nIn
-000006c0: 6465 7869 6e67 5c6e 2d2d 2d2d 2d2d 2d2d  dexing\n--------
-000006d0: 5c6e 5c6e 4279 2064 6566 6175 6c74 2c20  \n\nBy default, 
-000006e0: 6172 7469 636c 6573 2069 6e20 6120 7365  articles in a se
-000006f0: 7269 6573 2061 7265 206f 7264 6572 6564  ries are ordered
-00000700: 2062 7920 6461 7465 2061 6e64 2074 6865   by date and the
-00000710: 6e20 6175 746f 6d61 7469 6361 6c6c 7920  n automatically 
-00000720: 6e75 6d62 6572 6564 2e5c 6e5c 6e49 6620  numbered.\n\nIf 
-00000730: 796f 7520 7761 6e74 2074 6f20 666f 7263  you want to forc
-00000740: 6520 6120 6769 7665 6e20 6f72 6465 722c  e a given order,
-00000750: 2073 7065 6369 6679 2060 3a73 6572 6965   specify `:serie
-00000760: 735f 696e 6465 783a 6020 2872 6553 5429  s_index:` (reST)
-00000770: 206f 7220 6073 6572 6965 735f 696e 6465   or `series_inde
-00000780: 783a 6020 284d 6172 6b64 6f77 6e29 2069  x:` (Markdown) i
-00000790: 6e20 7468 6520 6172 7469 636c 6520 6d65  n the article me
-000007a0: 7461 6461 7461 2c20 7374 6172 7469 6e67  tadata, starting
-000007b0: 2066 726f 6d20 312e 2041 6c6c 2061 7274   from 1. All art
-000007c0: 6963 6c65 7320 7769 7468 2074 6869 7320  icles with this 
-000007d0: 656e 666f 7263 6564 2069 6e64 6578 2061  enforced index a
-000007e0: 7265 2070 7574 2061 7420 7468 6520 6265  re put at the be
-000007f0: 6769 6e6e 696e 6720 6f66 2074 6865 2073  ginning of the s
-00000800: 6572 6965 7320 616e 6420 6f72 6465 7265  eries and ordere
-00000810: 6420 6163 636f 7264 696e 6720 746f 2074  d according to t
-00000820: 6865 2069 6e64 6578 2069 7473 656c 662e  he index itself.
-00000830: 2041 6c6c 2074 6865 2072 656d 6169 6e69   All the remaini
-00000840: 6e67 2061 7274 6963 6c65 7320 636f 6d65  ng articles come
-00000850: 2061 6674 6572 2074 6865 6d2c 206f 7264   after them, ord
-00000860: 6572 6564 2062 7920 6461 7465 2e5c 6e5c  ered by date.\n\
-00000870: 6e54 6865 2070 6c75 6769 6e20 7072 6f76  nThe plugin prov
-00000880: 6964 6573 2074 6865 2066 6f6c 6c6f 7769  ides the followi
-00000890: 6e67 2076 6172 6961 626c 6573 2074 6f20  ng variables to 
-000008a0: 796f 7572 2074 656d 706c 6174 6573 3a5c  your templates:\
-000008b0: 6e5c 6e2a 2060 6172 7469 636c 652e 7365  n\n* `article.se
-000008c0: 7269 6573 2e6e 616d 6560 2069 7320 7468  ries.name` is th
-000008d0: 6520 6e61 6d65 206f 6620 7468 6520 7365  e name of the se
-000008e0: 7269 6573 2061 7320 7370 6563 6966 6965  ries as specifie
-000008f0: 6420 696e 2074 6865 2061 7274 6963 6c65  d in the article
-00000900: 206d 6574 6164 6174 615c 6e2a 2060 6172   metadata\n* `ar
-00000910: 7469 636c 652e 7365 7269 6573 2e69 6e64  ticle.series.ind
-00000920: 6578 6020 6973 2074 6865 2069 6e64 6578  ex` is the index
-00000930: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
-00000940: 6172 7469 636c 6520 696e 7369 6465 2074  article inside t
-00000950: 6865 2073 6572 6965 735c 6e2a 2060 6172  he series\n* `ar
-00000960: 7469 636c 652e 7365 7269 6573 2e61 6c6c  ticle.series.all
-00000970: 6020 6973 2061 6e20 6f72 6465 7265 6420  ` is an ordered 
-00000980: 6c69 7374 206f 6620 616c 6c20 6172 7469  list of all arti
-00000990: 636c 6573 2069 6e20 7468 6520 7365 7269  cles in the seri
-000009a0: 6573 2028 696e 636c 7564 696e 6720 7468  es (including th
-000009b0: 6520 6375 7272 656e 7420 6f6e 6529 5c6e  e current one)\n
-000009c0: 2a20 6061 7274 6963 6c65 2e73 6572 6965  * `article.serie
-000009d0: 732e 616c 6c5f 7072 6576 696f 7573 6020  s.all_previous` 
-000009e0: 6973 2061 6e20 6f72 6465 7265 6420 6c69  is an ordered li
-000009f0: 7374 206f 6620 7468 6520 6172 7469 636c  st of the articl
-00000a00: 6573 2070 7562 6c69 7368 6564 2062 6566  es published bef
-00000a10: 6f72 6520 7468 6520 6375 7272 656e 7420  ore the current 
-00000a20: 6f6e 655c 6e2a 2060 6172 7469 636c 652e  one\n* `article.
-00000a30: 7365 7269 6573 2e61 6c6c 5f6e 6578 7460  series.all_next`
-00000a40: 2069 7320 616e 206f 7264 6572 6564 206c   is an ordered l
-00000a50: 6973 7420 6f66 2074 6865 2061 7274 6963  ist of the artic
-00000a60: 6c65 7320 7075 626c 6973 6865 6420 6166  les published af
-00000a70: 7465 7220 7468 6520 6375 7272 656e 7420  ter the current 
-00000a80: 6f6e 655c 6e2a 2060 6172 7469 636c 652e  one\n* `article.
-00000a90: 7365 7269 6573 2e70 7265 7669 6f75 7360  series.previous`
-00000aa0: 2069 7320 7468 6520 7072 6576 696f 7573   is the previous
-00000ab0: 2061 7274 6963 6c65 2069 6e20 7468 6520   article in the 
-00000ac0: 7365 7269 6573 2028 6120 7368 6f72 7463  series (a shortc
-00000ad0: 7574 2074 6f20 6061 7274 6963 6c65 2e73  ut to `article.s
-00000ae0: 6572 6965 732e 616c 6c5f 7072 6576 696f  eries.all_previo
-00000af0: 7573 5b2d 315d 6029 206f 7220 604e 6f6e  us[-1]`) or `Non
-00000b00: 6560 2066 6f72 2074 6865 2066 6972 7374  e` for the first
-00000b10: 2061 7274 6963 6c65 5c6e 2a20 6061 7274   article\n* `art
-00000b20: 6963 6c65 2e73 6572 6965 732e 6e65 7874  icle.series.next
-00000b30: 6020 6973 2074 6865 206e 6578 7420 6172  ` is the next ar
-00000b40: 7469 636c 6520 696e 2074 6865 2073 6572  ticle in the ser
-00000b50: 6965 7320 2861 2073 686f 7274 6375 7420  ies (a shortcut 
-00000b60: 746f 2060 6172 7469 636c 652e 7365 7269  to `article.seri
-00000b70: 6573 2e61 6c6c 5f6e 6578 745b 305d 6029  es.all_next[0]`)
-00000b80: 206f 7220 604e 6f6e 6560 2066 6f72 2074   or `None` for t
-00000b90: 6865 206c 6173 7420 6f6e 655c 6e5c 6e46  he last one\n\nF
-00000ba0: 6f72 2065 7861 6d70 6c65 3a5c 6e5c 6e60  or example:\n\n`
-00000bb0: 6060 6874 6d6c 2b6a 696e 6a61 5c6e 7b25  ``html+jinja\n{%
-00000bc0: 2069 6620 6172 7469 636c 652e 7365 7269   if article.seri
-00000bd0: 6573 2025 7d5c 6e20 2020 203c 703e 5468  es %}\n    <p>Th
-00000be0: 6973 2070 6f73 7420 6973 2070 6172 7420  is post is part 
-00000bf0: 7b7b 2061 7274 6963 6c65 2e73 6572 6965  {{ article.serie
-00000c00: 732e 696e 6465 7820 7d7d 206f 6620 7468  s.index }} of th
-00000c10: 6520 227b 7b20 6172 7469 636c 652e 7365  e "{{ article.se
-00000c20: 7269 6573 2e6e 616d 6520 7d7d 2220 7365  ries.name }}" se
-00000c30: 7269 6573 3a3c 2f70 3e5c 6e20 2020 203c  ries:</p>\n    <
-00000c40: 6f6c 2063 6c61 7373 3d22 7061 7274 7322  ol class="parts"
-00000c50: 3e5c 6e20 2020 2020 2020 207b 2520 666f  >\n        {% fo
-00000c60: 7220 7061 7274 5f61 7274 6963 6c65 2069  r part_article i
-00000c70: 6e20 6172 7469 636c 652e 7365 7269 6573  n article.series
-00000c80: 2e61 6c6c 2025 7d5c 6e20 2020 2020 2020  .all %}\n       
-00000c90: 2020 2020 203c 6c69 207b 2520 6966 2070       <li {% if p
-00000ca0: 6172 745f 6172 7469 636c 6520 3d3d 2061  art_article == a
-00000cb0: 7274 6963 6c65 2025 7d63 6c61 7373 3d22  rticle %}class="
-00000cc0: 6163 7469 7665 227b 2520 656e 6469 6620  active"{% endif 
-00000cd0: 257d 3e5c 6e20 2020 2020 2020 2020 2020  %}>\n           
-00000ce0: 2020 2020 203c 6120 6872 6566 3d5c 277b       <a href=\'{
-00000cf0: 7b20 5349 5445 5552 4c20 7d7d 2f7b 7b20  { SITEURL }}/{{ 
-00000d00: 7061 7274 5f61 7274 6963 6c65 2e75 726c  part_article.url
-00000d10: 207d 7d5c 273e 7b7b 2070 6172 745f 6172   }}\'>{{ part_ar
-00000d20: 7469 636c 652e 7469 746c 6520 7d7d 3c2f  ticle.title }}</
-00000d30: 613e 5c6e 2020 2020 2020 2020 2020 2020  a>\n            
-00000d40: 3c2f 6c69 3e5c 6e20 2020 2020 2020 207b  </li>\n        {
-00000d50: 2520 656e 6466 6f72 2025 7d5c 6e20 2020  % endfor %}\n   
-00000d60: 203c 2f6f 6c3e 5c6e 7b25 2065 6e64 6966   </ol>\n{% endif
-00000d70: 2025 7d5c 6e60 6060 5c6e 5c6e 476c 6f62   %}\n```\n\nGlob
-00000d80: 616c 2043 6f6e 7465 7874 5c6e 2d2d 2d2d  al Context\n----
-00000d90: 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e 5c6e 5468  ----------\n\nTh
-00000da0: 6520 706c 7567 696e 2061 6c73 6f20 6164  e plugin also ad
-00000db0: 6473 2074 6865 206b 6579 2060 7365 7269  ds the key `seri
-00000dc0: 6573 6020 746f 2074 6865 2067 6c6f 6261  es` to the globa
-00000dd0: 6c20 636f 6e74 6578 742c 2077 6869 6368  l context, which
-00000de0: 2069 7320 6120 6469 6374 696f 6e61 7279   is a dictionary
-00000df0: 206f 6620 616c 6c20 7365 7269 6573 206e   of all series n
-00000e00: 616d 6573 2028 6173 206b 6579 7329 2061  ames (as keys) a
-00000e10: 6e64 2061 7274 6963 6c65 7320 2861 7320  nd articles (as 
-00000e20: 7661 6c75 6573 292e 2059 6f75 2063 616e  values). You can
-00000e30: 2075 7365 2074 6861 7420 746f 206c 6973   use that to lis
-00000e40: 7420 616c 6c20 7468 6520 7365 7269 6573  t all the series
-00000e50: 206f 6620 6172 7469 636c 6573 2069 6e20   of articles in 
-00000e60: 796f 7572 2073 6974 652c 2066 6f72 2065  your site, for e
-00000e70: 7861 6d70 6c65 5c6e 5c6e 6060 6068 746d  xample\n\n```htm
-00000e80: 6c2b 6a69 6e6a 615c 6e7b 2520 666f 7220  l+jinja\n{% for 
-00000e90: 7365 7269 6573 5f6e 616d 652c 2073 6572  series_name, ser
-00000ea0: 6965 735f 6172 7469 636c 6573 2069 6e20  ies_articles in 
-00000eb0: 7365 7269 6573 2e69 7465 6d73 2829 2025  series.items() %
-00000ec0: 7d5c 6e7b 2520 7365 7420 6172 7469 636c  }\n{% set articl
-00000ed0: 6520 3d20 7365 7269 6573 5f61 7274 6963  e = series_artic
-00000ee0: 6c65 735b 305d 2025 7d5c 6e3c 6172 7469  les[0] %}\n<arti
-00000ef0: 636c 6520 636c 6173 733d 2263 6172 6422  cle class="card"
-00000f00: 3e5c 6e5c 743c 6120 6872 6566 3d22 7b7b  >\n\t<a href="{{
-00000f10: 2061 7274 6963 6c65 2e75 726c 207d 7d22   article.url }}"
-00000f20: 2063 6c61 7373 3d22 696d 6167 6522 3e5c   class="image">\
-00000f30: 6e5c 745c 743c 696d 6720 7372 633d 222f  n\t\t<img src="/
-00000f40: 696d 6167 6573 2f7b 7b20 6172 7469 636c  images/{{ articl
-00000f50: 652e 696d 6167 6520 7d7d 2e6a 7067 2220  e.image }}.jpg" 
-00000f60: 616c 743d 227b 7b20 6172 7469 636c 652e  alt="{{ article.
-00000f70: 696d 6167 6520 7d7d 2220 2f3e 5c6e 5c74  image }}" />\n\t
-00000f80: 3c2f 613e 5c6e 5c74 3c64 6976 2063 6c61  </a>\n\t<div cla
-00000f90: 7373 3d22 6361 7264 2d62 6f64 7922 3e5c  ss="card-body">\
-00000fa0: 6e20 2020 205c 743c 6120 6872 6566 3d22  n    \t<a href="
-00000fb0: 7b7b 2061 7274 6963 6c65 2e75 726c 207d  {{ article.url }
-00000fc0: 7d22 3e3c 6833 2063 6c61 7373 3d22 6361  }"><h3 class="ca
-00000fd0: 7264 2d74 6974 6c65 223e 7b7b 2073 6572  rd-title">{{ ser
-00000fe0: 6965 735f 6e61 6d65 207d 7d3c 2f68 333e  ies_name }}</h3>
-00000ff0: 3c2f 613e 5c6e 2020 2020 205c 743c 756c  </a>\n     \t<ul
-00001000: 2063 6c61 7373 3d22 6163 7469 6f6e 7322   class="actions"
-00001010: 3e5c 6e20 2020 2020 5c74 5c74 3c6c 693e  >\n     \t\t<li>
-00001020: 3c61 2068 7265 663d 227b 7b20 6172 7469  <a href="{{ arti
-00001030: 636c 652e 7572 6c20 7d7d 2220 636c 6173  cle.url }}" clas
-00001040: 733d 2262 7574 746f 6e22 3e53 7461 7274  s="button">Start
-00001050: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
-00001060: 5c74 3c2f 756c 3e5c 6e5c 743c 2f64 6976  \t</ul>\n\t</div
-00001070: 3e5c 6e3c 2f61 7274 6963 6c65 3e5c 6e7b  >\n</article>\n{
-00001080: 2520 656e 6466 6f72 2025 7d5c 6e60 6060  % endfor %}\n```
-00001090: 5c6e 5c6e 436f 6e74 7269 6275 7469 6e67  \n\nContributing
-000010a0: 5c6e 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e  \n------------\n
-000010b0: 5c6e 436f 6e74 7269 6275 7469 6f6e 7320  \nContributions 
-000010c0: 6172 6520 7765 6c63 6f6d 6520 616e 6420  are welcome and 
-000010d0: 6d75 6368 2061 7070 7265 6369 6174 6564  much appreciated
-000010e0: 2e20 4576 6572 7920 6c69 7474 6c65 2062  . Every little b
-000010f0: 6974 2068 656c 7073 2e20 596f 7520 6361  it helps. You ca
-00001100: 6e20 636f 6e74 7269 6275 7465 2062 7920  n contribute by 
-00001110: 696d 7072 6f76 696e 6720 7468 6520 646f  improving the do
-00001120: 6375 6d65 6e74 6174 696f 6e2c 2061 6464  cumentation, add
-00001130: 696e 6720 6d69 7373 696e 6720 6665 6174  ing missing feat
-00001140: 7572 6573 2c20 616e 6420 6669 7869 6e67  ures, and fixing
-00001150: 2062 7567 732e 2059 6f75 2063 616e 2061   bugs. You can a
-00001160: 6c73 6f20 6865 6c70 206f 7574 2062 7920  lso help out by 
-00001170: 7265 7669 6577 696e 6720 616e 6420 636f  reviewing and co
-00001180: 6d6d 656e 7469 6e67 206f 6e20 5b65 7869  mmenting on [exi
-00001190: 7374 696e 6720 6973 7375 6573 5d5b 5d2e  sting issues][].
-000011a0: 5c6e 5c6e 546f 2073 7461 7274 2063 6f6e  \n\nTo start con
-000011b0: 7472 6962 7574 696e 6720 746f 2074 6869  tributing to thi
-000011c0: 7320 706c 7567 696e 2c20 7265 7669 6577  s plugin, review
-000011d0: 2074 6865 205b 436f 6e74 7269 6275 7469   the [Contributi
-000011e0: 6e67 2074 6f20 5065 6c69 6361 6e5d 5b5d  ng to Pelican][]
-000011f0: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
-00001200: 6265 6769 6e6e 696e 6720 7769 7468 2074  beginning with t
-00001210: 6865 202a 2a43 6f6e 7472 6962 7574 696e  he **Contributin
-00001220: 6720 436f 6465 2a2a 2073 6563 7469 6f6e  g Code** section
-00001230: 2e5c 6e5c 6e5b 6578 6973 7469 6e67 2069  .\n\n[existing i
-00001240: 7373 7565 735d 3a20 6874 7470 733a 2f2f  ssues]: https://
-00001250: 6769 7468 7562 2e63 6f6d 2f70 656c 6963  github.com/pelic
-00001260: 616e 2d70 6c75 6769 6e73 2f73 6572 6965  an-plugins/serie
-00001270: 732f 6973 7375 6573 5c6e 5b43 6f6e 7472  s/issues\n[Contr
-00001280: 6962 7574 696e 6720 746f 2050 656c 6963  ibuting to Pelic
-00001290: 616e 5d3a 2068 7474 7073 3a2f 2f64 6f63  an]: https://doc
-000012a0: 732e 6765 7470 656c 6963 616e 2e63 6f6d  s.getpelican.com
-000012b0: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 7472  /en/latest/contr
-000012c0: 6962 7574 652e 6874 6d6c 5c6e 5c6e 4c69  ibute.html\n\nLi
-000012d0: 6365 6e73 655c 6e2d 2d2d 2d2d 2d2d 5c6e  cense\n-------\n
-000012e0: 5c6e 5468 6973 2070 726f 6a65 6374 2069  \nThis project i
-000012f0: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-00001300: 2074 6865 2041 4750 4c20 332e 3020 6c69   the AGPL 3.0 li
-00001310: 6365 6e73 652e 5c6e 272c 0a20 2020 2027  cense.\n',.    '
-00001320: 6175 7468 6f72 273a 2027 4c65 6f6e 6172  author': 'Leonar
-00001330: 646f 2047 696f 7264 616e 6927 2c0a 2020  do Giordani',.  
-00001340: 2020 2761 7574 686f 725f 656d 6169 6c27    'author_email'
-00001350: 3a20 2767 696f 7264 616e 692e 6c65 6f6e  : 'giordani.leon
-00001360: 6172 646f 4067 6d61 696c 2e63 6f6d 272c  ardo@gmail.com',
-00001370: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00001380: 273a 204e 6f6e 652c 0a20 2020 2027 6d61  ': None,.    'ma
-00001390: 696e 7461 696e 6572 5f65 6d61 696c 273a  intainer_email':
-000013a0: 204e 6f6e 652c 0a20 2020 2027 7572 6c27   None,.    'url'
-000013b0: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-000013c0: 622e 636f 6d2f 7065 6c69 6361 6e2d 706c  b.com/pelican-pl
-000013d0: 7567 696e 732f 7365 7269 6573 272c 0a20  ugins/series',. 
-000013e0: 2020 2027 7061 636b 6167 6573 273a 2070     'packages': p
-000013f0: 6163 6b61 6765 732c 0a20 2020 2027 7061  ackages,.    'pa
-00001400: 636b 6167 655f 6461 7461 273a 2070 6163  ckage_data': pac
-00001410: 6b61 6765 5f64 6174 612c 0a20 2020 2027  kage_data,.    '
-00001420: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00001430: 273a 2069 6e73 7461 6c6c 5f72 6571 7569  ': install_requi
-00001440: 7265 732c 0a20 2020 2027 6578 7472 6173  res,.    'extras
-00001450: 5f72 6571 7569 7265 273a 2065 7874 7261  _require': extra
-00001460: 735f 7265 7175 6972 652c 0a20 2020 2027  s_require,.    '
-00001470: 7079 7468 6f6e 5f72 6571 7569 7265 7327  python_requires'
-00001480: 3a20 273e 3d33 2e36 2e32 2c3c 342e 3027  : '>=3.6.2,<4.0'
-00001490: 2c0a 7d0a 0a0a 7365 7475 7028 2a2a 7365  ,.}...setup(**se
-000014a0: 7475 705f 6b77 6172 6773 290a            tup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7065 6c69  : 2.1.Name: peli
+00000020: 6361 6e2d 7365 7269 6573 0a56 6572 7369  can-series.Versi
+00000030: 6f6e 3a20 332e 302e 300a 5375 6d6d 6172  on: 3.0.0.Summar
+00000040: 793a 2053 6572 6965 7320 6973 2061 2050  y: Series is a P
+00000050: 656c 6963 616e 2070 6c75 6769 6e20 7468  elican plugin th
+00000060: 6174 206a 6f69 6e73 206d 756c 7469 706c  at joins multipl
+00000070: 6520 706f 7374 7320 696e 746f 2061 2073  e posts into a s
+00000080: 6572 6965 730a 486f 6d65 2d70 6167 653a  eries.Home-page:
+00000090: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000a0: 636f 6d2f 7065 6c69 6361 6e2d 706c 7567  com/pelican-plug
+000000b0: 696e 732f 7365 7269 6573 0a4c 6963 656e  ins/series.Licen
+000000c0: 7365 3a20 4147 504c 2d33 2e30 0a4b 6579  se: AGPL-3.0.Key
+000000d0: 776f 7264 733a 2070 656c 6963 616e 2c70  words: pelican,p
+000000e0: 6c75 6769 6e2c 7365 7269 6573 2c6d 756c  lugin,series,mul
+000000f0: 7469 706c 650a 4175 7468 6f72 3a20 4c65  tiple.Author: Le
+00000100: 6f6e 6172 646f 2047 696f 7264 616e 690a  onardo Giordani.
+00000110: 4175 7468 6f72 2d65 6d61 696c 3a20 6769  Author-email: gi
+00000120: 6f72 6461 6e69 2e6c 656f 6e61 7264 6f40  ordani.leonardo@
+00000130: 676d 6169 6c2e 636f 6d0a 5265 7175 6972  gmail.com.Requir
+00000140: 6573 2d50 7974 686f 6e3a 203e 3d33 2e38  es-Python: >=3.8
+00000150: 2e31 2c3c 342e 300a 436c 6173 7369 6669  .1,<4.0.Classifi
+00000160: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+00000170: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
+00000180: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
+00000190: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
+000001a0: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
+000001b0: 6c65 0a43 6c61 7373 6966 6965 723a 2046  le.Classifier: F
+000001c0: 7261 6d65 776f 726b 203a 3a20 5065 6c69  ramework :: Peli
+000001d0: 6361 6e0a 436c 6173 7369 6669 6572 3a20  can.Classifier: 
+000001e0: 4672 616d 6577 6f72 6b20 3a3a 2050 656c  Framework :: Pel
+000001f0: 6963 616e 203a 3a20 506c 7567 696e 730a  ican :: Plugins.
+00000200: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000210: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000220: 2045 6e64 2055 7365 7273 2f44 6573 6b74   End Users/Deskt
+00000230: 6f70 0a43 6c61 7373 6966 6965 723a 204c  op.Classifier: L
+00000240: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000250: 7072 6f76 6564 203a 3a20 474e 5520 4166  proved :: GNU Af
+00000260: 6665 726f 2047 656e 6572 616c 2050 7562  fero General Pub
+00000270: 6c69 6320 4c69 6365 6e73 6520 7633 0a43  lic License v3.C
+00000280: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00000290: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000002a0: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
+000002b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002d0: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+000002e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000002f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000300: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+00000310: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000340: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000350: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000360: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000370: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+00000380: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000390: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003a0: 203a 3a20 332e 3132 0a43 6c61 7373 6966   :: 3.12.Classif
+000003b0: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
+000003c0: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
+000003d0: 5450 0a43 6c61 7373 6966 6965 723a 2054  TP.Classifier: T
+000003e0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000003f0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000400: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
+00000410: 686f 6e20 4d6f 6475 6c65 730a 5072 6f76  hon Modules.Prov
+00000420: 6964 6573 2d45 7874 7261 3a20 6d61 726b  ides-Extra: mark
+00000430: 646f 776e 0a52 6571 7569 7265 732d 4469  down.Requires-Di
+00000440: 7374 3a20 646f 6375 7469 6c73 2028 213d  st: docutils (!=
+00000450: 302e 3231 2e70 6f73 7431 290a 5265 7175  0.21.post1).Requ
+00000460: 6972 6573 2d44 6973 743a 206d 6172 6b64  ires-Dist: markd
+00000470: 6f77 6e20 283e 3d33 2e32 2920 3b20 6578  own (>=3.2) ; ex
+00000480: 7472 6120 3d3d 2022 6d61 726b 646f 776e  tra == "markdown
+00000490: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000004a0: 2070 656c 6963 616e 2028 3e3d 342e 3529   pelican (>=4.5)
+000004b0: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+000004c0: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+000004d0: 7073 3a2f 2f64 6f63 732e 6765 7470 656c  ps://docs.getpel
+000004e0: 6963 616e 2e63 6f6d 0a50 726f 6a65 6374  ican.com.Project
+000004f0: 2d55 524c 3a20 4675 6e64 696e 672c 2068  -URL: Funding, h
+00000500: 7474 7073 3a2f 2f64 6f6e 6174 652e 6765  ttps://donate.ge
+00000510: 7470 656c 6963 616e 2e63 6f6d 2f0a 5072  tpelican.com/.Pr
+00000520: 6f6a 6563 742d 5552 4c3a 2049 7373 7565  oject-URL: Issue
+00000530: 2054 7261 636b 6572 2c20 6874 7470 733a   Tracker, https:
+00000540: 2f2f 6769 7468 7562 2e63 6f6d 2f70 656c  //github.com/pel
+00000550: 6963 616e 2d70 6c75 6769 6e73 2f73 6572  ican-plugins/ser
+00000560: 6965 732f 6973 7375 6573 0a50 726f 6a65  ies/issues.Proje
+00000570: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
+00000580: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
+00000590: 7562 2e63 6f6d 2f70 656c 6963 616e 2d70  ub.com/pelican-p
+000005a0: 6c75 6769 6e73 2f73 6572 6965 730a 4465  lugins/series.De
+000005b0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000005c0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000005d0: 6b64 6f77 6e0a 0a53 6572 6965 733a 2041  kdown..Series: A
+000005e0: 2050 6c75 6769 6e20 666f 7220 5065 6c69   Plugin for Peli
+000005f0: 6361 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  can.============
+00000600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000610: 0a0a 5b21 5b42 7569 6c64 2053 7461 7475  ..[![Build Statu
+00000620: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+00000630: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000640: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000650: 772f 7374 6174 7573 2f70 656c 6963 616e  w/status/pelican
+00000660: 2d70 6c75 6769 6e73 2f73 6572 6965 732f  -plugins/series/
+00000670: 6d61 696e 2e79 6d6c 3f62 7261 6e63 683d  main.yml?branch=
+00000680: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
+00000690: 6974 6875 622e 636f 6d2f 7065 6c69 6361  ithub.com/pelica
+000006a0: 6e2d 706c 7567 696e 732f 7365 7269 6573  n-plugins/series
+000006b0: 2f61 6374 696f 6e73 290a 5b21 5b50 7950  /actions).[![PyP
+000006c0: 4920 5665 7273 696f 6e5d 2868 7474 7073  I Version](https
+000006d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000006e0: 6f2f 7079 7069 2f76 2f70 656c 6963 616e  o/pypi/v/pelican
+000006f0: 2d73 6572 6965 7329 5d28 6874 7470 733a  -series)](https:
+00000700: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000710: 6374 2f70 656c 6963 616e 2d73 6572 6965  ct/pelican-serie
+00000720: 732f 290a 215b 4c69 6365 6e73 655d 2868  s/).![License](h
+00000730: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000740: 6473 2e69 6f2f 7079 7069 2f6c 2f70 656c  ds.io/pypi/l/pel
+00000750: 6963 616e 2d73 6572 6965 733f 636f 6c6f  ican-series?colo
+00000760: 723d 626c 7565 290a 0a53 6572 6965 7320  r=blue)..Series 
+00000770: 6973 2061 2050 656c 6963 616e 2070 6c75  is a Pelican plu
+00000780: 6769 6e20 7468 6174 206a 6f69 6e73 206d  gin that joins m
+00000790: 756c 7469 706c 6520 706f 7374 7320 696e  ultiple posts in
+000007a0: 746f 2061 2073 6572 6965 732e 2047 6c6f  to a series. Glo
+000007b0: 6261 6c6c 792c 2069 7420 7072 6f76 6964  bally, it provid
+000007c0: 6573 2061 206c 6973 7420 6f66 2061 6c6c  es a list of all
+000007d0: 2074 6865 2073 6572 6965 732c 2061 6e64   the series, and
+000007e0: 2066 6f72 2065 6163 6820 6172 7469 636c   for each articl
+000007f0: 6520 6974 2070 726f 7669 6465 7320 6120  e it provides a 
+00000800: 6c69 7374 206f 6620 616c 6c20 6172 7469  list of all arti
+00000810: 636c 6573 2069 6e20 7468 6520 7361 6d65  cles in the same
+00000820: 2073 6572 6965 7320 616e 6420 6c69 6e6b   series and link
+00000830: 7320 746f 2074 6865 206e 6578 7420 616e  s to the next an
+00000840: 6420 7072 6576 696f 7573 2061 7274 6963  d previous artic
+00000850: 6c65 7320 696e 2074 6865 2073 6572 6965  les in the serie
+00000860: 732e 0a0a 496e 7374 616c 6c61 7469 6f6e  s...Installation
+00000870: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54  .------------..T
+00000880: 6869 7320 706c 7567 696e 2063 616e 2062  his plugin can b
+00000890: 6520 696e 7374 616c 6c65 6420 7669 613a  e installed via:
+000008a0: 0a0a 2020 2020 7079 7468 6f6e 202d 6d20  ..    python -m 
+000008b0: 7069 7020 696e 7374 616c 6c20 7065 6c69  pip install peli
+000008c0: 6361 6e2d 7365 7269 6573 0a0a 4173 206c  can-series..As l
+000008d0: 6f6e 6720 6173 2079 6f75 2068 6176 6520  ong as you have 
+000008e0: 6e6f 7420 6578 706c 6963 6974 6c79 2061  not explicitly a
+000008f0: 6464 6564 2061 2060 504c 5547 494e 5360  dded a `PLUGINS`
+00000900: 2073 6574 7469 6e67 2074 6f20 796f 7572   setting to your
+00000910: 2050 656c 6963 616e 2073 6574 7469 6e67   Pelican setting
+00000920: 7320 6669 6c65 2c20 7468 656e 2074 6865  s file, then the
+00000930: 206e 6577 6c79 2d69 6e73 7461 6c6c 6564   newly-installed
+00000940: 2070 6c75 6769 6e20 7368 6f75 6c64 2062   plugin should b
+00000950: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+00000960: 6465 7465 6374 6564 2061 6e64 2065 6e61  detected and ena
+00000970: 626c 6564 2e20 4f74 6865 7277 6973 652c  bled. Otherwise,
+00000980: 2079 6f75 206d 7573 7420 6164 6420 6073   you must add `s
+00000990: 6572 6965 7360 2074 6f20 796f 7572 2065  eries` to your e
+000009a0: 7869 7374 696e 6720 6050 4c55 4749 4e53  xisting `PLUGINS
+000009b0: 6020 6c69 7374 2e20 466f 7220 6d6f 7265  ` list. For more
+000009c0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 706c   information, pl
+000009d0: 6561 7365 2073 6565 2074 6865 205b 486f  ease see the [Ho
+000009e0: 7720 746f 2055 7365 2050 6c75 6769 6e73  w to Use Plugins
+000009f0: 5d28 6874 7470 733a 2f2f 646f 6373 2e67  ](https://docs.g
+00000a00: 6574 7065 6c69 6361 6e2e 636f 6d2f 656e  etpelican.com/en
+00000a10: 2f6c 6174 6573 742f 706c 7567 696e 732e  /latest/plugins.
+00000a20: 6874 6d6c 2368 6f77 2d74 6f2d 7573 652d  html#how-to-use-
+00000a30: 706c 7567 696e 7329 2064 6f63 756d 656e  plugins) documen
+00000a40: 7461 7469 6f6e 2e0a 0a55 7361 6765 0a2d  tation...Usage.-
+00000a50: 2d2d 2d2d 0a0a 496e 206f 7264 6572 2074  ----..In order t
+00000a60: 6f20 6d61 726b 2072 6553 7472 7563 7475  o mark reStructu
+00000a70: 7265 6454 6578 742d 666f 726d 6174 7465  redText-formatte
+00000a80: 6420 706f 7374 7320 6173 2070 6172 7420  d posts as part 
+00000a90: 6f66 2061 2073 6572 6965 732c 2075 7365  of a series, use
+00000aa0: 2074 6865 2060 3a73 6572 6965 733a 6020   the `:series:` 
+00000ab0: 6d65 7461 6461 7461 3a0a 0a20 2020 203a  metadata:..    :
+00000ac0: 7365 7269 6573 3a20 204e 414d 455f 4f46  series:  NAME_OF
+00000ad0: 5f54 4849 535f 5345 5249 4553 0a0a 4f72  _THIS_SERIES..Or
+00000ae0: 2c20 666f 7220 4d61 726b 646f 776e 2d66  , for Markdown-f
+00000af0: 6f72 6d61 7474 6564 2063 6f6e 7465 6e74  ormatted content
+00000b00: 3a0a 0a20 2020 2053 6572 6965 733a 204e  :..    Series: N
+00000b10: 414d 455f 4f46 5f54 4849 535f 5345 5249  AME_OF_THIS_SERI
+00000b20: 4553 0a0a 5468 6520 706c 7567 696e 2063  ES..The plugin c
+00000b30: 6f6c 6c65 6374 7320 616c 6c20 6172 7469  ollects all arti
+00000b40: 636c 6573 206f 7220 7061 6765 7320 6265  cles or pages be
+00000b50: 6c6f 6e67 696e 6720 746f 2074 6865 2073  longing to the s
+00000b60: 616d 6520 7365 7269 6573 2061 6e64 2070  ame series and p
+00000b70: 726f 7669 6465 7320 7365 7269 6573 2d72  rovides series-r
+00000b80: 656c 6174 6564 2076 6172 6961 626c 6573  elated variables
+00000b90: 2074 6861 7420 796f 7520 6361 6e20 7573   that you can us
+00000ba0: 6520 696e 2079 6f75 7220 7465 6d70 6c61  e in your templa
+00000bb0: 7465 2e0a 0a41 7274 6963 6c65 7320 616e  te...Articles an
+00000bc0: 6420 7061 6765 730a 2d2d 2d2d 2d2d 2d2d  d pages.--------
+00000bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6973  ----------..This
+00000be0: 2070 6c75 6769 6e20 776f 726b 7320 626f   plugin works bo
+00000bf0: 7468 2077 6974 6820 6172 7469 636c 6573  th with articles
+00000c00: 2061 6e64 2070 6167 6573 2e20 4173 2050   and pages. As P
+00000c10: 656c 6963 616e 2075 7365 7320 7468 6520  elican uses the 
+00000c20: 7370 6563 6966 6963 2076 6172 6961 626c  specific variabl
+00000c30: 6520 6061 7274 6963 6c65 6020 666f 7220  e `article` for 
+00000c40: 6172 7469 636c 6520 7465 6d70 6c61 7465  article template
+00000c50: 7320 616e 6420 6070 6167 6560 2066 6f72  s and `page` for
+00000c60: 2070 6167 6520 7465 6d70 6c61 7465 7320   page templates 
+00000c70: 6974 2069 7320 636f 6d70 6c69 6361 7465  it is complicate
+00000c80: 6420 746f 2067 6976 6520 6578 616d 706c  d to give exampl
+00000c90: 6573 2074 6861 7420 776f 726b 2066 6f72  es that work for
+00000ca0: 2062 6f74 6820 6361 7365 732e 2049 6e20   both cases. In 
+00000cb0: 7468 6520 666f 6c6c 6f77 696e 6720 646f  the following do
+00000cc0: 6375 6d65 6e74 6174 696f 6e20 616c 6c20  cumentation all 
+00000cd0: 6578 616d 706c 6520 7769 6c6c 206d 656e  example will men
+00000ce0: 7469 6f6e 2060 6172 7469 636c 652e 6020  tion `article.` 
+00000cf0: 2865 2e67 2e20 6061 7274 6963 6c65 2e73  (e.g. `article.s
+00000d00: 6572 6965 7360 2c20 6061 7274 6963 6c65  eries`, `article
+00000d10: 2e74 6974 6c65 6029 2062 7574 2074 6865  .title`) but the
+00000d20: 2063 6f64 6520 776f 726b 7320 696e 2074   code works in t
+00000d30: 6865 2073 616d 6520 7761 7920 7769 7468  he same way with
+00000d40: 2060 7061 6765 6020 2865 2e67 2e20 6070   `page` (e.g. `p
+00000d50: 6167 652e 7365 7269 6573 602c 2060 7061  age.series`, `pa
+00000d60: 6765 2e74 6974 6c65 6029 2e0a 0a41 7274  ge.title`)...Art
+00000d70: 6963 6c65 2073 6572 6965 7320 616e 6420  icle series and 
+00000d80: 7061 6765 2073 6572 6965 7320 6172 6520  page series are 
+00000d90: 6372 6561 7465 6420 7365 7061 7261 7465  created separate
+00000da0: 6c79 2c20 736f 2065 7665 6e20 6966 2061  ly, so even if a
+00000db0: 6e20 6172 7469 636c 6520 616e 6420 6120  n article and a 
+00000dc0: 7061 6765 2068 6176 6520 7468 6520 7361  page have the sa
+00000dd0: 6d65 2073 6572 6965 7320 7468 6579 2077  me series they w
+00000de0: 6f6e 2774 2061 7070 6561 7220 746f 6765  on't appear toge
+00000df0: 7468 6572 2e0a 0a49 6e64 6578 696e 670a  ther...Indexing.
+00000e00: 2d2d 2d2d 2d2d 2d2d 0a0a 4279 2064 6566  --------..By def
+00000e10: 6175 6c74 2c20 6172 7469 636c 6573 2069  ault, articles i
+00000e20: 6e20 6120 7365 7269 6573 2061 7265 206f  n a series are o
+00000e30: 7264 6572 6564 2062 7920 6461 7465 2061  rdered by date a
+00000e40: 6e64 2074 6865 6e20 6175 746f 6d61 7469  nd then automati
+00000e50: 6361 6c6c 7920 6e75 6d62 6572 6564 2e20  cally numbered. 
+00000e60: 5061 6765 7320 696e 2061 2073 6572 6965  Pages in a serie
+00000e70: 7320 6172 6520 6f72 6465 7265 6420 6279  s are ordered by
+00000e80: 2074 6974 6c65 2061 6e64 2061 7574 6f6d   title and autom
+00000e90: 6174 6963 616c 6c79 206e 756d 6265 7265  atically numbere
+00000ea0: 642e 0a0a 4966 2079 6f75 2077 616e 7420  d...If you want 
+00000eb0: 746f 2066 6f72 6365 2061 2067 6976 656e  to force a given
+00000ec0: 206f 7264 6572 2c20 7370 6563 6966 7920   order, specify 
+00000ed0: 603a 7365 7269 6573 5f69 6e64 6578 3a60  `:series_index:`
+00000ee0: 2028 7265 5354 2920 6f72 2060 7365 7269   (reST) or `seri
+00000ef0: 6573 5f69 6e64 6578 3a60 2028 4d61 726b  es_index:` (Mark
+00000f00: 646f 776e 2920 696e 2074 6865 2061 7274  down) in the art
+00000f10: 6963 6c65 206d 6574 6164 6174 612c 2073  icle metadata, s
+00000f20: 7461 7274 696e 6720 6672 6f6d 2031 2e20  tarting from 1. 
+00000f30: 416c 6c20 6172 7469 636c 6573 2077 6974  All articles wit
+00000f40: 6820 7468 6973 2065 6e66 6f72 6365 6420  h this enforced 
+00000f50: 696e 6465 7820 6172 6520 7075 7420 6174  index are put at
+00000f60: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
+00000f70: 6620 7468 6520 7365 7269 6573 2061 6e64  f the series and
+00000f80: 206f 7264 6572 6564 2061 6363 6f72 6469   ordered accordi
+00000f90: 6e67 2074 6f20 7468 6520 696e 6465 7820  ng to the index 
+00000fa0: 6974 7365 6c66 2e20 416c 6c20 7468 6520  itself. All the 
+00000fb0: 7265 6d61 696e 696e 6720 6172 7469 636c  remaining articl
+00000fc0: 6573 2063 6f6d 6520 6166 7465 7220 7468  es come after th
+00000fd0: 656d 2c20 6f72 6465 7265 6420 7769 7468  em, ordered with
+00000fe0: 2074 6865 2064 6566 6175 6c74 206f 7264   the default ord
+00000ff0: 6572 696e 6720 2864 6174 6520 666f 7220  ering (date for 
+00001000: 6172 7469 636c 6573 2061 6e64 2074 6974  articles and tit
+00001010: 6c65 2066 6f72 2070 6167 6573 292e 0a0a  le for pages)...
+00001020: 5468 6520 706c 7567 696e 2070 726f 7669  The plugin provi
+00001030: 6465 7320 7468 6520 666f 6c6c 6f77 696e  des the followin
+00001040: 6720 7661 7269 6162 6c65 7320 746f 2079  g variables to y
+00001050: 6f75 7220 7465 6d70 6c61 7465 733a 0a0a  our templates:..
+00001060: 2a20 6061 7274 6963 6c65 2e73 6572 6965  * `article.serie
+00001070: 732e 6e61 6d65 6020 6973 2074 6865 206e  s.name` is the n
+00001080: 616d 6520 6f66 2074 6865 2073 6572 6965  ame of the serie
+00001090: 7320 6173 2073 7065 6369 6669 6564 2069  s as specified i
+000010a0: 6e20 7468 6520 6172 7469 636c 6520 6d65  n the article me
+000010b0: 7461 6461 7461 0a2a 2060 6172 7469 636c  tadata.* `articl
+000010c0: 652e 7365 7269 6573 2e69 6e64 6578 6020  e.series.index` 
+000010d0: 6973 2074 6865 2069 6e64 6578 206f 6620  is the index of 
+000010e0: 7468 6520 6375 7272 656e 7420 6172 7469  the current arti
+000010f0: 636c 6520 696e 7369 6465 2074 6865 2073  cle inside the s
+00001100: 6572 6965 730a 2a20 6061 7274 6963 6c65  eries.* `article
+00001110: 2e73 6572 6965 732e 616c 6c60 2069 7320  .series.all` is 
+00001120: 616e 206f 7264 6572 6564 206c 6973 7420  an ordered list 
+00001130: 6f66 2061 6c6c 2061 7274 6963 6c65 7320  of all articles 
+00001140: 696e 2074 6865 2073 6572 6965 7320 2869  in the series (i
+00001150: 6e63 6c75 6469 6e67 2074 6865 2063 7572  ncluding the cur
+00001160: 7265 6e74 206f 6e65 290a 2a20 6061 7274  rent one).* `art
+00001170: 6963 6c65 2e73 6572 6965 732e 616c 6c5f  icle.series.all_
+00001180: 7072 6576 696f 7573 6020 6973 2061 6e20  previous` is an 
+00001190: 6f72 6465 7265 6420 6c69 7374 206f 6620  ordered list of 
+000011a0: 7468 6520 6172 7469 636c 6573 2070 7562  the articles pub
+000011b0: 6c69 7368 6564 2062 6566 6f72 6520 7468  lished before th
+000011c0: 6520 6375 7272 656e 7420 6f6e 650a 2a20  e current one.* 
+000011d0: 6061 7274 6963 6c65 2e73 6572 6965 732e  `article.series.
+000011e0: 616c 6c5f 6e65 7874 6020 6973 2061 6e20  all_next` is an 
+000011f0: 6f72 6465 7265 6420 6c69 7374 206f 6620  ordered list of 
+00001200: 7468 6520 6172 7469 636c 6573 2070 7562  the articles pub
+00001210: 6c69 7368 6564 2061 6674 6572 2074 6865  lished after the
+00001220: 2063 7572 7265 6e74 206f 6e65 0a2a 2060   current one.* `
+00001230: 6172 7469 636c 652e 7365 7269 6573 2e70  article.series.p
+00001240: 7265 7669 6f75 7360 2069 7320 7468 6520  revious` is the 
+00001250: 7072 6576 696f 7573 2061 7274 6963 6c65  previous article
+00001260: 2069 6e20 7468 6520 7365 7269 6573 2028   in the series (
+00001270: 6120 7368 6f72 7463 7574 2074 6f20 6061  a shortcut to `a
+00001280: 7274 6963 6c65 2e73 6572 6965 732e 616c  rticle.series.al
+00001290: 6c5f 7072 6576 696f 7573 5b2d 315d 6029  l_previous[-1]`)
+000012a0: 206f 7220 604e 6f6e 6560 2066 6f72 2074   or `None` for t
+000012b0: 6865 2066 6972 7374 2061 7274 6963 6c65  he first article
+000012c0: 0a2a 2060 6172 7469 636c 652e 7365 7269  .* `article.seri
+000012d0: 6573 2e6e 6578 7460 2069 7320 7468 6520  es.next` is the 
+000012e0: 6e65 7874 2061 7274 6963 6c65 2069 6e20  next article in 
+000012f0: 7468 6520 7365 7269 6573 2028 6120 7368  the series (a sh
+00001300: 6f72 7463 7574 2074 6f20 6061 7274 6963  ortcut to `artic
+00001310: 6c65 2e73 6572 6965 732e 616c 6c5f 6e65  le.series.all_ne
+00001320: 7874 5b30 5d60 2920 6f72 2060 4e6f 6e65  xt[0]`) or `None
+00001330: 6020 666f 7220 7468 6520 6c61 7374 206f  ` for the last o
+00001340: 6e65 0a0a 466f 7220 6578 616d 706c 653a  ne..For example:
+00001350: 0a0a 6060 6068 746d 6c2b 6a69 6e6a 610a  ..```html+jinja.
+00001360: 7b25 2069 6620 6172 7469 636c 652e 7365  {% if article.se
+00001370: 7269 6573 2025 7d0a 2020 2020 3c70 3e54  ries %}.    <p>T
+00001380: 6869 7320 706f 7374 2069 7320 7061 7274  his post is part
+00001390: 207b 7b20 6172 7469 636c 652e 7365 7269   {{ article.seri
+000013a0: 6573 2e69 6e64 6578 207d 7d20 6f66 2074  es.index }} of t
+000013b0: 6865 2022 7b7b 2061 7274 6963 6c65 2e73  he "{{ article.s
+000013c0: 6572 6965 732e 6e61 6d65 207d 7d22 2073  eries.name }}" s
+000013d0: 6572 6965 733a 3c2f 703e 0a20 2020 203c  eries:</p>.    <
+000013e0: 6f6c 2063 6c61 7373 3d22 7061 7274 7322  ol class="parts"
+000013f0: 3e0a 2020 2020 2020 2020 7b25 2066 6f72  >.        {% for
+00001400: 2070 6172 745f 6172 7469 636c 6520 696e   part_article in
+00001410: 2061 7274 6963 6c65 2e73 6572 6965 732e   article.series.
+00001420: 616c 6c20 257d 0a20 2020 2020 2020 2020  all %}.         
+00001430: 2020 203c 6c69 207b 2520 6966 2070 6172     <li {% if par
+00001440: 745f 6172 7469 636c 6520 3d3d 2061 7274  t_article == art
+00001450: 6963 6c65 2025 7d63 6c61 7373 3d22 6163  icle %}class="ac
+00001460: 7469 7665 227b 2520 656e 6469 6620 257d  tive"{% endif %}
+00001470: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001480: 2020 3c61 2068 7265 663d 277b 7b20 5349    <a href='{{ SI
+00001490: 5445 5552 4c20 7d7d 2f7b 7b20 7061 7274  TEURL }}/{{ part
+000014a0: 5f61 7274 6963 6c65 2e75 726c 207d 7d27  _article.url }}'
+000014b0: 3e7b 7b20 7061 7274 5f61 7274 6963 6c65  >{{ part_article
+000014c0: 2e74 6974 6c65 207d 7d3c 2f61 3e0a 2020  .title }}</a>.  
+000014d0: 2020 2020 2020 2020 2020 3c2f 6c69 3e0a            </li>.
+000014e0: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+000014f0: 7220 257d 0a20 2020 203c 2f6f 6c3e 0a7b  r %}.    </ol>.{
+00001500: 2520 656e 6469 6620 257d 0a60 6060 0a0a  % endif %}.```..
+00001510: 476c 6f62 616c 2043 6f6e 7465 7874 0a2d  Global Context.-
+00001520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2a  -------------..*
+00001530: 2a57 6172 6e69 6e67 2a2a 3a20 696e 2076  *Warning**: in v
+00001540: 6572 7369 6f6e 2033 2074 6865 2067 6c6f  ersion 3 the glo
+00001550: 6261 6c20 6b65 7920 6073 6572 6965 7360  bal key `series`
+00001560: 2068 6173 2062 6565 6e20 7265 6e61 6d65   has been rename
+00001570: 6420 746f 2060 6172 7469 636c 655f 7365  d to `article_se
+00001580: 7269 6573 6020 746f 2064 6966 6665 7265  ries` to differe
+00001590: 6e74 6961 7465 2069 7420 6672 6f6d 2074  ntiate it from t
+000015a0: 6865 206e 6577 2067 6c6f 6261 6c20 6b65  he new global ke
+000015b0: 7920 6070 6167 655f 7365 7269 6573 602e  y `page_series`.
+000015c0: 0a0a 5468 6520 706c 7567 696e 2061 6c73  ..The plugin als
+000015d0: 6f20 6164 6473 2074 6865 206b 6579 7320  o adds the keys 
+000015e0: 6061 7274 6963 6c65 5f73 6572 6965 7360  `article_series`
+000015f0: 2061 6e64 2060 7061 6765 5f73 6572 6965   and `page_serie
+00001600: 7360 2074 6f20 7468 6520 676c 6f62 616c  s` to the global
+00001610: 2063 6f6e 7465 7874 2e20 5468 6579 2061   context. They a
+00001620: 7265 2064 6963 7469 6f6e 6172 6965 7320  re dictionaries 
+00001630: 6f66 2061 6c6c 2073 6572 6965 7320 6e61  of all series na
+00001640: 6d65 7320 2861 7320 6b65 7973 2920 616e  mes (as keys) an
+00001650: 6420 6974 656d 7320 2861 7320 7661 6c75  d items (as valu
+00001660: 6573 292e 2059 6f75 2063 616e 2075 7365  es). You can use
+00001670: 2074 6861 7420 746f 206c 6973 7420 616c   that to list al
+00001680: 6c20 7468 6520 7365 7269 6573 2069 6e20  l the series in 
+00001690: 796f 7572 2073 6974 652c 2066 6f72 2065  your site, for e
+000016a0: 7861 6d70 6c65 0a0a 6060 6068 746d 6c2b  xample..```html+
+000016b0: 6a69 6e6a 610a 7b25 2066 6f72 2073 6572  jinja.{% for ser
+000016c0: 6965 735f 6e61 6d65 2c20 7365 7269 6573  ies_name, series
+000016d0: 5f61 7274 6963 6c65 7320 696e 2073 6572  _articles in ser
+000016e0: 6965 732e 6974 656d 7328 2920 257d 0a7b  ies.items() %}.{
+000016f0: 2520 7365 7420 6172 7469 636c 6520 3d20  % set article = 
+00001700: 7365 7269 6573 5f61 7274 6963 6c65 735b  series_articles[
+00001710: 305d 2025 7d0a 3c61 7274 6963 6c65 2063  0] %}.<article c
+00001720: 6c61 7373 3d22 6361 7264 223e 0a09 3c61  lass="card">..<a
+00001730: 2068 7265 663d 227b 7b20 6172 7469 636c   href="{{ articl
+00001740: 652e 7572 6c20 7d7d 2220 636c 6173 733d  e.url }}" class=
+00001750: 2269 6d61 6765 223e 0a09 093c 696d 6720  "image">...<img 
+00001760: 7372 633d 222f 696d 6167 6573 2f7b 7b20  src="/images/{{ 
+00001770: 6172 7469 636c 652e 696d 6167 6520 7d7d  article.image }}
+00001780: 2e6a 7067 2220 616c 743d 227b 7b20 6172  .jpg" alt="{{ ar
+00001790: 7469 636c 652e 696d 6167 6520 7d7d 2220  ticle.image }}" 
+000017a0: 2f3e 0a09 3c2f 613e 0a09 3c64 6976 2063  />..</a>..<div c
+000017b0: 6c61 7373 3d22 6361 7264 2d62 6f64 7922  lass="card-body"
+000017c0: 3e0a 2020 2020 093c 6120 6872 6566 3d22  >.    .<a href="
+000017d0: 7b7b 2061 7274 6963 6c65 2e75 726c 207d  {{ article.url }
+000017e0: 7d22 3e3c 6833 2063 6c61 7373 3d22 6361  }"><h3 class="ca
+000017f0: 7264 2d74 6974 6c65 223e 7b7b 2073 6572  rd-title">{{ ser
+00001800: 6965 735f 6e61 6d65 207d 7d3c 2f68 333e  ies_name }}</h3>
+00001810: 3c2f 613e 0a20 2020 2020 093c 756c 2063  </a>.     .<ul c
+00001820: 6c61 7373 3d22 6163 7469 6f6e 7322 3e0a  lass="actions">.
+00001830: 2020 2020 2009 093c 6c69 3e3c 6120 6872       ..<li><a hr
+00001840: 6566 3d22 7b7b 2061 7274 6963 6c65 2e75  ef="{{ article.u
+00001850: 726c 207d 7d22 2063 6c61 7373 3d22 6275  rl }}" class="bu
+00001860: 7474 6f6e 223e 5374 6172 743c 2f61 3e3c  tton">Start</a><
+00001870: 2f6c 693e 0a20 2020 2020 093c 2f75 6c3e  /li>.     .</ul>
+00001880: 0a09 3c2f 6469 763e 0a3c 2f61 7274 6963  ..</div>.</artic
+00001890: 6c65 3e0a 7b25 2065 6e64 666f 7220 257d  le>.{% endfor %}
+000018a0: 0a60 6060 0a0a 4173 2069 7420 6973 206e  .```..As it is n
+000018b0: 6f74 2070 6f73 7369 626c 6520 746f 2063  ot possible to c
+000018c0: 7265 6174 6520 7061 6765 7320 6672 6f6d  reate pages from
+000018d0: 2070 6c75 6769 6e73 2079 6f75 2063 616e   plugins you can
+000018e0: 206c 6576 6572 6167 6520 6974 2074 6f20   leverage it to 
+000018f0: 6372 6561 7465 2061 2070 6167 6520 666f  create a page fo
+00001900: 7220 6120 7370 6563 6966 6963 2073 6572  r a specific ser
+00001910: 6965 732c 2065 7665 6e20 7468 6f75 6768  ies, even though
+00001920: 2079 6f75 2068 6176 6520 746f 2068 6172   you have to har
+00001930: 6420 636f 6465 2074 6865 206e 616d 6520  d code the name 
+00001940: 6f66 2074 6865 2073 6572 6965 7320 696e  of the series in
+00001950: 2074 6865 2074 656d 706c 6174 652e 0a0a   the template...
+00001960: 436f 6e74 7269 6275 7469 6e67 0a2d 2d2d  Contributing.---
+00001970: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6f6e 7472  ---------..Contr
+00001980: 6962 7574 696f 6e73 2061 7265 2077 656c  ibutions are wel
+00001990: 636f 6d65 2061 6e64 206d 7563 6820 6170  come and much ap
+000019a0: 7072 6563 6961 7465 642e 2045 7665 7279  preciated. Every
+000019b0: 206c 6974 746c 6520 6269 7420 6865 6c70   little bit help
+000019c0: 732e 2059 6f75 2063 616e 2063 6f6e 7472  s. You can contr
+000019d0: 6962 7574 6520 6279 2069 6d70 726f 7669  ibute by improvi
+000019e0: 6e67 2074 6865 2064 6f63 756d 656e 7461  ng the documenta
+000019f0: 7469 6f6e 2c20 6164 6469 6e67 206d 6973  tion, adding mis
+00001a00: 7369 6e67 2066 6561 7475 7265 732c 2061  sing features, a
+00001a10: 6e64 2066 6978 696e 6720 6275 6773 2e20  nd fixing bugs. 
+00001a20: 596f 7520 6361 6e20 616c 736f 2068 656c  You can also hel
+00001a30: 7020 6f75 7420 6279 2072 6576 6965 7769  p out by reviewi
+00001a40: 6e67 2061 6e64 2063 6f6d 6d65 6e74 696e  ng and commentin
+00001a50: 6720 6f6e 205b 6578 6973 7469 6e67 2069  g on [existing i
+00001a60: 7373 7565 735d 5b5d 2e0a 0a54 6f20 7374  ssues][]...To st
+00001a70: 6172 7420 636f 6e74 7269 6275 7469 6e67  art contributing
+00001a80: 2074 6f20 7468 6973 2070 6c75 6769 6e2c   to this plugin,
+00001a90: 2072 6576 6965 7720 7468 6520 5b43 6f6e   review the [Con
+00001aa0: 7472 6962 7574 696e 6720 746f 2050 656c  tributing to Pel
+00001ab0: 6963 616e 5d5b 5d20 646f 6375 6d65 6e74  ican][] document
+00001ac0: 6174 696f 6e2c 2062 6567 696e 6e69 6e67  ation, beginning
+00001ad0: 2077 6974 6820 7468 6520 2a2a 436f 6e74   with the **Cont
+00001ae0: 7269 6275 7469 6e67 2043 6f64 652a 2a20  ributing Code** 
+00001af0: 7365 6374 696f 6e2e 0a0a 5b65 7869 7374  section...[exist
+00001b00: 696e 6720 6973 7375 6573 5d3a 2068 7474  ing issues]: htt
+00001b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001b20: 7065 6c69 6361 6e2d 706c 7567 696e 732f  pelican-plugins/
+00001b30: 7365 7269 6573 2f69 7373 7565 730a 5b43  series/issues.[C
+00001b40: 6f6e 7472 6962 7574 696e 6720 746f 2050  ontributing to P
+00001b50: 656c 6963 616e 5d3a 2068 7474 7073 3a2f  elican]: https:/
+00001b60: 2f64 6f63 732e 6765 7470 656c 6963 616e  /docs.getpelican
+00001b70: 2e63 6f6d 2f65 6e2f 6c61 7465 7374 2f63  .com/en/latest/c
+00001b80: 6f6e 7472 6962 7574 652e 6874 6d6c 0a0a  ontribute.html..
+00001b90: 4c69 6365 6e73 650a 2d2d 2d2d 2d2d 2d0a  License.-------.
+00001ba0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001bb0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001bc0: 7468 6520 4147 504c 2033 2e30 206c 6963  the AGPL 3.0 lic
+00001bd0: 656e 7365 2e0a 0a                        ense...
```

