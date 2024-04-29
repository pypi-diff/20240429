# Comparing `tmp/mkv_episode_matcher-0.1.0.tar.gz` & `tmp/mkv_episode_matcher-0.1.1.tar.gz`

## Comparing `mkv_episode_matcher-0.1.0.tar` & `mkv_episode_matcher-0.1.1.tar`

### file list

```diff
@@ -1,132 +1,4 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.coverage.DESKTOP-NTJ52LL.19040.XkHNEbEx
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.coverage.DESKTOP-NTJ52LL.24340.XjsBEKWx
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.gitattributes
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.gitmodules
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/mkv_episode_matcher.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0    59241 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0   131054 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/doctrees/mkv_episode_matcher.doctree
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/.nojekyll
--rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/index.html
--rw-r--r--   0        0        0    45080 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/mkv_episode_matcher.html
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/modules.html
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/search.html
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/index.html
--rw-r--r--   0        0        0    12903 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/mkv_episode_matcher/config.html
--rw-r--r--   0        0        0    41533 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/mkv_episode_matcher/episode_matcher.html
--rw-r--r--   0        0        0    31320 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/mkv_episode_matcher/mkv_to_srt.html
--rw-r--r--   0        0        0    20905 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/mkv_episode_matcher/tmdb_client.html
--rw-r--r--   0        0        0    39686 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_modules/mkv_episode_matcher/utils.html
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_sources/mkv_episode_matcher.rst.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0    15555 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0   287630 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0    89476 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/jquery.js
--rw-r--r--   0        0        0    11151 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    16578 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/underscore.js
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   123687 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   109948 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0        0        0    96964 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0        0        0    63184 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Inconsolata.ttf
--rw-r--r--   0        0        0   656544 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   656568 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0   170616 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0        0        0   169064 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   256056 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bold.eot
--rw-r--r--   0        0        0   600856 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bold.ttf
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bold.woff2
--rw-r--r--   0        0        0   266158 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bolditalic.eot
--rw-r--r--   0        0        0   622572 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bolditalic.ttf
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff2
--rw-r--r--   0        0        0   268604 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-italic.eot
--rw-r--r--   0        0        0   639388 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-italic.ttf
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-italic.woff2
--rw-r--r--   0        0        0   253461 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-regular.eot
--rw-r--r--   0        0        0   607720 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-regular.ttf
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-regular.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/Lato/lato-regular.woff2
--rw-r--r--   0        0        0    79520 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-r--r--   0        0        0   170616 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-r--r--   0        0        0    78331 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-r--r--   0        0        0   169064 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/js/modernizr.min.js
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/.git
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/.gitignore
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/__init__.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/imagemaker.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/pgs2srt.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/pgsreader.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/requirements.txt
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/Libraries/SubZero/SubZero.py
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/Libraries/SubZero/post_processing.py
--rw-r--r--   0        0        0   676829 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/.gitattributes
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/__init__.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/__main__.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/config.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/episode_matcher.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/mkv_to_srt.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/requirements.txt
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/tmdb_client.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/mkv_episode_matcher/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/.gitignore
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/README.md
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/README.md
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/PKG-INFO
```

### Comparing `mkv_episode_matcher-0.1.0/README.md` & `mkv_episode_matcher-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.0/pyproject.toml` & `mkv_episode_matcher-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.sdist]
+include = [
+  "libraries/pgs2srtkg/**/*.py",
+]
 [project]
 name = "mkv-episode-matcher"
 dynamic = ["version"]
 description = "The MKV Episode Matcher is a tool for identifying TV series episodes from MKV files and renaming the files accordingly."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
```

### Comparing `mkv_episode_matcher-0.1.0/PKG-INFO` & `mkv_episode_matcher-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mkv-episode-matcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: The MKV Episode Matcher is a tool for identifying TV series episodes from MKV files and renaming the files accordingly.
 Project-URL: Documentation, https://github.com/Jsakkos/mkv-episode-matcher#readme
 Project-URL: Issues, https://github.com/Jsakkos/mkv-episode-matcher/issues
 Project-URL: Source, https://github.com/Jsakkos/mkv-episode-matcher
 Author-email: Jsakkos <jonathansakkos@protonmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

