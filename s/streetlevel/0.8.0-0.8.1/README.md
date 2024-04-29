# Comparing `tmp/streetlevel-0.8.0.tar.gz` & `tmp/streetlevel-0.8.1.tar.gz`

## Comparing `streetlevel-0.8.0.tar` & `streetlevel-0.8.1.tar`

### file list

```diff
@@ -1,108 +1,116 @@
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 streetlevel-0.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 streetlevel-0.8.0/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streetlevel-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 streetlevel-0.8.0/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/Makefile
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/conf.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/dataclasses.rst
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/geo.rst
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/make.bat
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.ja.rst
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.kakao.rst
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.lookaround.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.mapy.rst
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.naver.rst
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.streetside.rst
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.streetview.rst
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/streetlevel.yandex.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/util.rst
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 streetlevel-0.8.0/docs/_static/css/additional.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/__init__.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/dataclasses.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/geo.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/util.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/ja/__init__.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/ja/api.py
--rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/ja/ja.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/ja/panorama.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/ja/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/kakao/__init__.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/kakao/api.py
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/kakao/kakao.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/kakao/panorama.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/kakao/util.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/api.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/auth.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/geo.py
--rw-r--r--   0        0        0     8156 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/lookaround.py
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/panorama.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/reproject.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/util.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/proto/GroundMetadataTile.proto
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/proto/GroundMetadataTile_pb2.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/proto/MuninViewState.proto
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/proto/MuninViewState_pb2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/lookaround/proto/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/mapy/__init__.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/mapy/api.py
--rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/mapy/mapy.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/mapy/panorama.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/mapy/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/naver/__init__.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/naver/api.py
--rw-r--r--   0        0        0    16511 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/naver/naver.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/naver/panorama.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/naver/util.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetside/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetside/api.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetside/panorama.py
--rw-r--r--   0        0        0    11091 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetside/streetside.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetside/util.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/__init__.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/api.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/depth.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/panorama.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/protobuf.py
--rw-r--r--   0        0        0    19203 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/streetview.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/streetview/util.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/yandex/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/yandex/api.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/yandex/panorama.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/yandex/util.py
--rw-r--r--   0        0        0    10412 2020-02-02 00:00:00.000000 streetlevel-0.8.0/streetlevel/yandex/yandex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/geo_test.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/lookaround/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/lookaround/geo_test.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/lookaround/lookaround_test.py
--rw-r--r--   0        0        0    26834 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/lookaround/data/metadata_tile.pb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/mapy/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/mapy/mapy_test.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/mapy/data/getbest.pkl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetside/__init__.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetside/streetside_test.py
--rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetside/data/find.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/__init__.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/streetview_test.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/coverage_tile.json
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/find.json
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/find_by_id.json
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/missing_date.json
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/missing_historical_date.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/missing_level_name.json
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/missing_link_direction.json
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/nepal_links.json
--rw-r--r--   0        0        0    10441 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/places.json
--rw-r--r--   0        0        0    25482 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/streetview/data/street_names.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/yandex/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/yandex/yandex_test.py
--rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 streetlevel-0.8.0/tests/yandex/data/find.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 streetlevel-0.8.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 streetlevel-0.8.0/LICENSE
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 streetlevel-0.8.0/README.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 streetlevel-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 streetlevel-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 streetlevel-0.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 streetlevel-0.8.1/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streetlevel-0.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 streetlevel-0.8.1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/dataclasses.rst
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/geo.rst
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/index.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/make.bat
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.ja.rst
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.kakao.rst
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.lookaround.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.mapy.rst
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.naver.rst
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.streetside.rst
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.streetview.rst
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/streetlevel.yandex.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/util.rst
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 streetlevel-0.8.1/docs/_static/css/additional.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/dataclasses.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/geo.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/util.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/__init__.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/api.py
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/ja.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/panorama.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/parse.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/ja/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/__init__.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/api.py
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/kakao.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/panorama.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/parse.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/kakao/util.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/api.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/auth.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/geo.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/lookaround.py
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/panorama.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/parse.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/reproject.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/util.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/proto/GroundMetadataTile.proto
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/proto/GroundMetadataTile_pb2.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/proto/MuninViewState.proto
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/proto/MuninViewState_pb2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/lookaround/proto/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/__init__.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/api.py
+-rw-r--r--   0        0        0     8722 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/mapy.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/panorama.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/parse.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/mapy/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/__init__.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/api.py
+-rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/naver.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/panorama.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/parse.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/naver/util.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/api.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/panorama.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/parse.py
+-rw-r--r--   0        0        0     9806 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/streetside.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetside/util.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/__init__.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/api.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/depth.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/panorama.py
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/parse.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/protobuf.py
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/streetview.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/streetview/util.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/api.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/panorama.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/parse.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/util.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 streetlevel-0.8.1/streetlevel/yandex/yandex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/geo_test.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/pytest.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/lookaround/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/lookaround/geo_test.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/lookaround/lookaround_test.py
+-rw-r--r--   0        0        0    26834 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/lookaround/data/metadata_tile.pb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/mapy/__init__.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/mapy/mapy_test.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/mapy/data/getbest.pkl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetside/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetside/streetside_test.py
+-rw-r--r--   0        0        0    10506 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetside/data/find.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/__init__.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/streetview_test.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/coverage_tile.json
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/find.json
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/find_by_id.json
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/missing_date.json
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/missing_historical_date.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/missing_level_name.json
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/missing_link_direction.json
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/nepal_links.json
+-rw-r--r--   0        0        0    10441 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/places.json
+-rw-r--r--   0        0        0    25482 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/streetview/data/street_names.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/yandex/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/yandex/yandex_test.py
+-rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 streetlevel-0.8.1/tests/yandex/data/find.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 streetlevel-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 streetlevel-0.8.1/LICENSE
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 streetlevel-0.8.1/README.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 streetlevel-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 streetlevel-0.8.1/PKG-INFO
```

### Comparing `streetlevel-0.8.0/.readthedocs.yaml` & `streetlevel-0.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/.github/workflows/python-publish.yml` & `streetlevel-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/.github/workflows/python-test.yml` & `streetlevel-0.8.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/Makefile` & `streetlevel-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/conf.py` & `streetlevel-0.8.1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'streetlevel'
 copyright = '2024, skzk'
 author = 'skzk'
-release = '0.8.0'
+release = '0.8.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `streetlevel-0.8.0/docs/index.rst` & `streetlevel-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/make.bat` & `streetlevel-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.ja.rst` & `streetlevel-0.8.1/docs/streetlevel.ja.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.kakao.rst` & `streetlevel-0.8.1/docs/streetlevel.kakao.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.lookaround.rst` & `streetlevel-0.8.1/docs/streetlevel.lookaround.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.mapy.rst` & `streetlevel-0.8.1/docs/streetlevel.mapy.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.naver.rst` & `streetlevel-0.8.1/docs/streetlevel.naver.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.streetside.rst` & `streetlevel-0.8.1/docs/streetlevel.streetside.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.streetview.rst` & `streetlevel-0.8.1/docs/streetlevel.streetview.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/streetlevel.yandex.rst` & `streetlevel-0.8.1/docs/streetlevel.yandex.rst`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/docs/_static/css/additional.css` & `streetlevel-0.8.1/docs/_static/css/additional.css`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/geo.py` & `streetlevel-0.8.1/streetlevel/geo.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/util.py` & `streetlevel-0.8.1/streetlevel/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/ja/api.py` & `streetlevel-0.8.1/streetlevel/ja/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/ja/ja.py` & `streetlevel-0.8.1/streetlevel/streetside/streetside.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,247 @@
-import math
-from typing import Optional, List, Tuple, Union
+import asyncio
+from io import BytesIO
+from typing import List, Union, Optional
 
 from PIL import Image
 from aiohttp import ClientSession
 from requests import Session
 
+from streetlevel.geo import *
 from . import api
-from .panorama import JaPanorama, CaptureDate, Address, StreetLabel
-from ..dataclasses import Tile
-from ..util import download_tiles, download_tiles_async, CubemapStitchingMethod, stitch_cubemap_faces, \
-    save_cubemap_panorama, stitch_cubemap_face, try_get
+from .panorama import StreetsidePanorama
+from .parse import parse_panoramas, parse_panorama, parse_panoramas_id_response
+from .util import to_base4
+from ..util import download_files_async, stitch_cubemap_faces, CubemapStitchingMethod, save_cubemap_panorama
 
+TILE_SIZE = 256
 
-def find_panorama(lat: float, lon: float, radius: int = 100, session: Session = None) -> Optional[JaPanorama]:
+
+def find_panorama_by_id(panoid: int, session: Session = None) -> Optional[StreetsidePanorama]:
     """
-    Searches for a panorama within a radius around a point.
+    Fetches metadata for a specific panorama.
 
-    :param lat: Latitude of the center point.
-    :param lon: Longitude of the center point.
-    :param radius: *(optional)* Search radius in meters, max. 5000(?). Defaults to 100.
+    :param panoid: The pano ID.
     :param session: *(optional)* A requests session.
-    :return: A JaPanorama if a panorama was found, or None.
+    :return: A StreetsidePanorama object if a panorama was found, or None.
     """
-    response = api.find_panorama(lat, lon, radius, session)
-
-    if "message" in response:
-        return None
-
-    return _parse_panorama(response)
-
-
-async def find_panorama_async(lat: float, lon: float, session: ClientSession,
-                               radius: int = 100) -> Optional[JaPanorama]:
-    response = await api.find_panorama_async(lat, lon, session, radius)
+    response = api.find_panorama_by_id(panoid, session)
+    return parse_panoramas_id_response(response)
 
-    if "message" in response:
-        return None
 
-    return _parse_panorama(response)
+async def find_panorama_by_id_async(panoid: int, session: ClientSession) -> Optional[StreetsidePanorama]:
+    response = await api.find_panorama_by_id_async(panoid, session)
+    return parse_panoramas_id_response(response)
 
 
-def find_panorama_by_id(panoid: int, session: Session = None) -> Optional[JaPanorama]:
+def find_panoramas_in_bbox(north: float, west: float, south: float, east: float,
+                           limit: int = 50, session: Session = None) -> List[StreetsidePanorama]:
     """
-    Fetches metadata of a specific panorama.
+    Retrieves panoramas within a bounding box.
 
-    :param panoid: The pano ID.
+    :param north: lat1.
+    :param west: lon1.
+    :param south: lat2.
+    :param east: lon2.
+    :param limit: *(optional)* Maximum number of results to return. Defaults to 50.
     :param session: *(optional)* A requests session.
-    :return: A JaPanorama object if a panorama with this ID was found, or None.
+    :return: A list of StreetsidePanorama objects.
     """
-    response = api.find_panorama_by_id(panoid, session)
-    return _parse_panorama_by_id(response)
+    response = api.find_panoramas(north, west, south, east, limit, session)
+    return parse_panoramas(response)
 
 
-async def find_panorama_by_id_async(panoid: int, session: ClientSession) -> Optional[JaPanorama]:
-    response = await api.find_panorama_by_id_async(panoid, session)
-    return _parse_panorama_by_id(response)
+async def find_panoramas_in_bbox_async(north: float, west: float, south: float, east: float,
+                                       session: ClientSession, limit: int = 50) -> List[StreetsidePanorama]:
+    response = await api.find_panoramas_async(north, west, south, east, session, limit)
+    return parse_panoramas(response)
 
 
-def get_panorama(pano: JaPanorama, zoom: int = 0,
-                 stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW) \
-        -> Union[List[Image.Image], Image.Image]:
+def find_panoramas(lat: float, lon: float, radius: float = 25,
+                   limit: int = 50, session: Session = None) -> List[StreetsidePanorama]:
     """
-    Downloads a panorama and returns it as PIL image.
+    Retrieves panoramas within a square around a point.
 
-    :param pano: The panorama.
-    :param zoom: *(optional)* Image size; 0 is high, 1 is low. Defaults to 0.
-    :param stitching_method: *(optional)* Whether and how the faces of the cubemap are stitched into one
-        image. Defaults to ``ROW``.
-    :return: A PIL image or a list of six PIL images depending on ``stitching_method``.
+    :param lat: Latitude of the center point.
+    :param lon: Longitude of the center point.
+    :param radius: *(optional)* Radius of the square in meters. (Not sure if that's the correct mathematical
+      term, but you get the idea.) Defaults to 25.
+    :param limit: *(optional)* Maximum number of results to return. Defaults to 50.
+    :param session: *(optional)* A requests session.
+    :return: A list of StreetsidePanorama objects.
     """
-    zoom = min(1, max(zoom, 0))
-    face_tiles, cols, rows = _generate_tile_list(pano, zoom)
-    tile_images = _download_tiles(face_tiles)
-    return _stitch_panorama(tile_images, cols, rows, stitching_method=stitching_method)
+    top_left, bottom_right = create_bounding_box_around_point(lat, lon, radius)
+    return find_panoramas_in_bbox(
+        top_left[0], top_left[1],
+        bottom_right[0], bottom_right[1],
+        limit=limit, session=session)
 
 
-async def get_panorama_async(pano: JaPanorama, session: ClientSession, zoom: int = 0,
-                             stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW) \
-        -> Union[List[Image.Image], Image.Image]:
-    zoom = min(1, max(zoom, 0))
-    face_tiles, cols, rows = _generate_tile_list(pano, zoom)
-    tile_images = await _download_tiles_async(face_tiles, session)
-    return _stitch_panorama(tile_images, cols, rows, stitching_method=stitching_method)
+async def find_panoramas_async(lat: float, lon: float, session: ClientSession,
+                               radius: float = 25, limit: int = 50) -> List[StreetsidePanorama]:
+
+    top_left, bottom_right = create_bounding_box_around_point(lat, lon, radius)
+    return await find_panoramas_in_bbox_async(
+        top_left[0], top_left[1],
+        bottom_right[0], bottom_right[1],
+        session, limit=limit)
 
 
-def download_panorama(pano: JaPanorama, path: str, zoom: int = 0,
+def download_panorama(pano: StreetsidePanorama, path: str, zoom: int = 4,
                       stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW,
                       pil_args: dict = None) -> None:
     """
     Downloads a panorama to a file.
 
     :param pano: The panorama.
     :param path: Output path.
-    :param zoom: *(optional)* Image size; 0 is high, 1 is low. Defaults to 0.
+    :param zoom: *(optional)* Image size; 0 is lowest, 4 is highest. Defaults to 4. If 4 is not available, 3 will be
+      downloaded.
+      (Note that only the old Microsoft panoramas go up to 4; the TomTom-provided panoramas stop at 3.)
     :param stitching_method: *(optional)* Whether and how the faces of the cubemap are stitched into one
         image. Defaults to ``ROW``.
     :param pil_args: *(optional)* Additional arguments for PIL's
         `Image.save <https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.save>`_
         method, e.g. ``{"quality":100}``. Defaults to ``{}``.
     """
     if pil_args is None:
         pil_args = {}
 
     output = get_panorama(pano, zoom=zoom, stitching_method=stitching_method)
     save_cubemap_panorama(output, path, pil_args)
 
 
-async def download_panorama_async(pano: JaPanorama, path: str, session: ClientSession, zoom: int = 0,
+async def download_panorama_async(pano: StreetsidePanorama, path: str, session: ClientSession, zoom: int = 4,
                                   stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW,
                                   pil_args: dict = None) -> None:
     if pil_args is None:
         pil_args = {}
 
     output = await get_panorama_async(pano, session, zoom=zoom, stitching_method=stitching_method)
     save_cubemap_panorama(output, path, pil_args)
 
 
-def _parse_panorama_by_id(pano_dict: dict) -> JaPanorama:
-    address = try_get(lambda: pano_dict["streets"]["nearestAddress"])
-    if address:
-        address = Address(*address.values())
-
-    return JaPanorama(
-        id=pano_dict["image"]["id"],
-        lat=pano_dict["image"]["lat"],
-        lon=pano_dict["image"]["lng"],
-        heading=math.radians(pano_dict["image"]["heading"]),
-        date=_parse_date(pano_dict["image"]["month"]),
-        pano_url="https:" + pano_dict["image"]["pano_url"],
-        blur_key=pano_dict["image"]["blur_key"],
-        street_names=_parse_streets(pano_dict["streets"]),
-        address=address,
-        neighbors=_parse_hotspots(pano_dict["hotspots"]),
-    )
-
-
-def _parse_streets(streets: dict) -> List[StreetLabel]:
-    main = StreetLabel(name=streets["street"]["name"],
-                       angles=[math.radians(a) for a in streets["street"]["azimuths"]])
-    connections = []
-    for connection_dict in streets["connections"]:
-        connection = StreetLabel(name=connection_dict["name"],
-                                 angles=[math.radians(connection_dict["angle"])],
-                                 distance=connection_dict["distance"])
-        connections.append(connection)
-
-    return [main] + connections
-
-
-def _parse_hotspots(hotspots: list) -> List[JaPanorama]:
-    neighbors = []
-    for hotspot in hotspots:
-        neighbors.append(JaPanorama(
-            id=hotspot["image"]["id"],
-            lat=hotspot["image"]["lat"],
-            lon=hotspot["image"]["lng"],
-            heading=math.radians(hotspot["image"]["heading"]),
-            date=_parse_date(hotspot["image"]["month"]),
-            pano_url="https:" + hotspot["image"]["pano_url"],
-            blur_key=hotspot["image"]["blur_key"],
-        ))
-    return neighbors
-
-
-def _parse_date(date_str: str) -> CaptureDate:
-    year, month = date_str.split("-")
-    date = CaptureDate(int(year), int(month))
-    return date
-
-
-def _parse_panorama(pano_dict: dict) -> JaPanorama:
-    return JaPanorama(
-        id=pano_dict["id"],
-        lat=pano_dict["lat"],
-        lon=pano_dict["lng"],
-        heading=math.radians(pano_dict["image_heading"]),
-    )
-
-
-def _generate_tile_list(pano: JaPanorama, zoom: int) -> Tuple[List[List[Tile]], int, int]:
-    if not (zoom == 0 or zoom == 1):
-        raise ValueError("Unsupported zoom level")
-
-    cols = 2 if zoom == 1 else 4
-    rows = 2 if zoom == 1 else 4
+def get_panorama(pano: StreetsidePanorama, zoom: int = 4,
+                 stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW) \
+        -> Union[List[Image.Image], Image.Image]:
+    """
+    Downloads a panorama and returns it as PIL image.
 
-    tiles = []
-    for face_url_name in ["f", "r", "b", "l", "u", "d"]:
+    :param pano: The panorama.
+    :param zoom: *(optional)* Image size; 0 is lowest, 4 is highest. Defaults to 4. If 4 is not available, 3 will be
+      downloaded.
+      (Note that only the old Microsoft panoramas go up to 4; the TomTom-provided panoramas stop at 3.)
+    :param stitching_method: *(optional)* Whether and how the faces of the cubemap are stitched into one
+        image. Defaults to ``ROW``.
+    :return: A PIL image or a list of six PIL images depending on ``stitching_method``.
+    """
+    zoom = max(0, min(zoom, pano.max_zoom))
+    faces = _generate_tile_list(pano.id, zoom)
+    _download_tiles(faces)
+    return _stitch_panorama(faces, stitching_method=stitching_method)
+
+
+async def get_panorama_async(pano: StreetsidePanorama, session: ClientSession, zoom: int = 4,
+                             stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW
+                             ) -> Union[List[Image.Image], Image.Image]:
+    zoom = max(0, min(zoom, pano.max_zoom))
+    faces = _generate_tile_list(pano.id, zoom)
+    await _download_tiles_async(faces, session)
+    return _stitch_panorama(faces, stitching_method=stitching_method)
+
+
+def _generate_tile_list(panoid, zoom):
+    """
+    Generates a list of a panorama's tiles.
+    Returns a list of faces and its tiles.
+    """
+    if zoom > 4:
+        raise ValueError("Zoom can't be greater than 4")
+    panoid_base4 = to_base4(panoid).rjust(16, "0")
+    subdivs = pow(4, zoom)
+    faces = {}
+    for face_id in range(0, 6):
+        face_id_base4 = to_base4(face_id + 1).rjust(2, "0")
         face_tiles = []
-        for row_idx in range(0, rows):
-            for col_idx in range(0, cols):
-                blur_key_str = f".{pano.blur_key}" if pano.blur_key else ""
-                face_tiles.append(Tile(col_idx, row_idx,
-                                       f"{pano.pano_url}/mres_{face_url_name}/l{zoom+1}/"
-                                       f"l{zoom+1}_{face_url_name}_{row_idx+1}_{col_idx+1}{blur_key_str}.jpg"))
-        tiles.append(face_tiles)
-    return tiles, cols, rows
+        for subdiv in range(0, subdivs):
+            if zoom < 1:
+                subdiv_base4 = ""
+            else:
+                subdiv_base4 = to_base4(subdiv).rjust(zoom, "0")
+            tile_key = f"{face_id_base4}{subdiv_base4}"
+            url = f"https://t.ssl.ak.tiles.virtualearth.net/tiles/hs{panoid_base4}{tile_key}.jpg?" \
+                  f"g=13716"
+            face_tiles.append({"face": face_id_base4, "subdiv": subdiv, "url": url})
+        faces[face_id] = face_tiles
+    return faces
 
 
-def _download_tiles(face_tiles: List[List[Tile]]) -> List[dict]:
-    faces = []
-    for face in face_tiles:
-        faces.append(download_tiles(face))
-    return faces
+def _download_tiles(faces):
+    """
+    Downloads the tiles of a panorama.
+    """
+    for face_id, face in faces.items():
+        tiles = asyncio.run(download_files_async([tile["url"] for tile in face]))
+        for idx, tile in enumerate(face):
+            tile["image"] = tiles[idx]
 
 
-async def _download_tiles_async(face_tiles: List[List[Tile]], session: ClientSession) -> List[dict]:
-    faces = []
-    for face in face_tiles:
-        faces.append(await download_tiles_async(face, session))
-    return faces
+async def _download_tiles_async(faces, session: ClientSession):
+    """
+    Downloads the tiles of a panorama.
+    """
+    for face_id, face in faces.items():
+        tiles = await download_files_async([tile["url"] for tile in face], session)
+        for idx, tile in enumerate(face):
+            tile["image"] = tiles[idx]
 
 
-def _stitch_panorama(tile_images: List[dict], cols: int, rows: int,
-                     stitching_method: CubemapStitchingMethod) -> Union[List[Image.Image], Image.Image]:
+def _stitch_four(face):
+    """
+    Stitches four consecutive individual tiles.
+    """
+    sub_tile = Image.new('RGB', (TILE_SIZE * 2, TILE_SIZE * 2))
+    for idx, tile in enumerate(face[0:4]):
+        tile_img = Image.open(BytesIO(tile["image"]))
+        x = idx % 2
+        y = idx // 2
+        sub_tile.paste(im=tile_img, box=(x * TILE_SIZE, y * TILE_SIZE))
+    return sub_tile
+
+
+def _split_list(list_, size):
+    return [list_[i:i + size] for i in range(0, len(list_), size)]
+
+
+def _stitch_face(face):
+    """
+    Stitches one face of a panorama.
+    """
+    if len(face) <= 4:
+        return _stitch_four(face)
+    else:
+        grid_size = int(math.sqrt(len(face)))
+        stitched_tile_size = (grid_size // 2) * TILE_SIZE
+        tile = Image.new('RGB', (stitched_tile_size * 2, stitched_tile_size * 2))
+        split = _split_list(face, len(face) // 4)
+        tile.paste(im=_stitch_face(split[0]), box=(0, 0))
+        tile.paste(im=_stitch_face(split[1]), box=(stitched_tile_size, 0))
+        tile.paste(im=_stitch_face(split[2]), box=(0, stitched_tile_size))
+        tile.paste(im=_stitch_face(split[3]), box=(stitched_tile_size, stitched_tile_size))
+        return tile
+
+
+def _stitch_panorama(faces, stitching_method: CubemapStitchingMethod) -> Union[List[Image.Image], Image.Image]:
+    """
+    Stitches downloaded tiles into full faces or one full image.
+    """
+    full_tile_size = int(math.sqrt(len(faces[1]))) * TILE_SIZE
+
     stitched_faces = []
-    for tiles in tile_images:
-        stitched_face = stitch_cubemap_face(tiles, 512, cols, rows)
-        stitched_faces.append(stitched_face)
-    return stitch_cubemap_faces(stitched_faces, stitched_faces[0].size[0], stitching_method)
+    if len(faces[1]) == 1:
+        for i in range(0, 6):
+            stitched_faces.append(Image.open(BytesIO(faces[i][0]["image"])))
+    else:
+        for i in range(0, 6):
+            stitched_faces.append(_stitch_face(faces[i]))
+
+    return stitch_cubemap_faces(stitched_faces, full_tile_size, stitching_method=stitching_method)
```

### Comparing `streetlevel-0.8.0/streetlevel/ja/panorama.py` & `streetlevel-0.8.1/streetlevel/ja/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/ja/util.py` & `streetlevel-0.8.1/streetlevel/ja/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/kakao/api.py` & `streetlevel-0.8.1/streetlevel/kakao/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/kakao/kakao.py` & `streetlevel-0.8.1/streetlevel/kakao/kakao.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import itertools
-import math
 from typing import List, Optional
-from datetime import datetime
 
 import requests
 from PIL import Image
 from aiohttp import ClientSession
 from requests import Session
 
 from . import api
-from .panorama import KakaoPanorama, PanoramaType
-from ..dataclasses import Tile, Size, Link
-from ..util import try_get, get_equirectangular_panorama, get_equirectangular_panorama_async, get_image, \
+from .panorama import KakaoPanorama
+from .parse import parse_panoramas, parse_panorama
+from ..dataclasses import Tile, Size
+from ..util import get_equirectangular_panorama, get_equirectangular_panorama_async, get_image, \
     get_image_async, download_file, download_file_async
 
 PANO_COLS = [1, 8, 16]
 PANO_ROWS = [1, 4, 8]
 PANO_TILE_SIZE = Size(512, 512)
 PANO_TILE_URL_TEMPLATE = [
     "https://map.daumcdn.net/map_roadview{0}.jpg",
@@ -39,25 +38,25 @@
     :return: A list of KakaoPanorama objects.
     """
     response = api.find_panoramas(lat, lon, radius, limit, session)
 
     if response["street_view"]["cnt"] == 0:
         return []
 
-    return _parse_panoramas(response)
+    return parse_panoramas(response)
 
 
 async def find_panoramas_async(lat: float, lon: float, session: ClientSession,
                                radius: int = 35, limit: int = 50) -> List[KakaoPanorama]:
     response = await api.find_panoramas_async(lat, lon, session, radius, limit)
 
     if response["street_view"]["cnt"] == 0:
         return []
 
-    return _parse_panoramas(response)
+    return parse_panoramas(response)
 
 
 def find_panorama_by_id(panoid: int, neighbors: bool = True, session: Session = None) -> Optional[KakaoPanorama]:
     """
     Fetches metadata of a specific panorama.
 
     This call only appears to work for the most recent coverage at a location. IDs of older panoramas will return
@@ -70,28 +69,28 @@
     :return: A KakaoPanorama object if a panorama with this ID was found, or None.
     """
     response = api.find_panorama_by_id(panoid, session)
 
     if response["street_view"]["cnt"] == 0:
         return None
 
-    pano = _parse_panorama(response["street_view"]["street"])
+    pano = parse_panorama(response["street_view"]["street"])
     if neighbors:
         pano.neighbors = find_panoramas(pano.lat, pano.lon, session=session)
     return pano
 
 
 async def find_panorama_by_id_async(panoid: int, session: ClientSession,
                                     neighbors: bool = True) -> Optional[KakaoPanorama]:
     response = await api.find_panorama_by_id_async(panoid, session)
 
     if response["street_view"]["cnt"] == 0:
         return None
 
-    pano = _parse_panorama(response["street_view"]["street"])
+    pano = parse_panorama(response["street_view"]["street"])
     if neighbors:
         pano.neighbors = await find_panoramas_async(pano.lat, pano.lon, session)
     return pano
 
 
 def get_panorama(pano: KakaoPanorama, zoom: int = 2) -> Image.Image:
     """
@@ -183,58 +182,14 @@
 
 
 def _build_depthmap_url(pano):
     return f"https://map.daumcdn.net/map_roadview/depthmap_meerkat" \
            f"{pano.image_path}_W.png"
 
 
-def _parse_panoramas(response):
-    return [_parse_panorama(pano) for pano in response["street_view"]["streetList"]]
-
-
-def _parse_panorama(pano_json: dict) -> KakaoPanorama:
-    pano = KakaoPanorama(
-        id=pano_json["id"],
-        lat=pano_json["wgsy"],
-        lon=pano_json["wgsx"],
-        wcongx=pano_json["wcongx"],
-        wcongy=pano_json["wcongy"],
-        heading=math.radians(float(pano_json["angle"])),
-        image_path=pano_json["img_path"],
-        # shot_date sometimes returns the time as 00:00:00, but the image url is always correct
-        date=datetime.strptime(pano_json["img_path"].split("_")[-1], "%Y%m%d%H%M%S"),
-        street_name=try_get(lambda: pano_json["st_name"]),
-        address=try_get(lambda: pano_json["addr"]),
-        street_type=try_get(lambda: pano_json["st_type"]),
-        panorama_type=PanoramaType(int(pano_json["shot_tool"]))
-    )
-
-    if "past" in pano_json and pano_json["past"] is not None:
-        pano.historical = [_parse_panorama(past) for past in pano_json["past"]]
-
-    if "spot" in pano_json and pano_json["past"] is not None:
-        pano.links = _parse_links(pano_json["spot"])
-
-    return pano
-
-
-def _parse_links(links_json: List[dict]) -> List[Link]:
-    links = []
-    for linked_json in links_json:
-        linked = KakaoPanorama(
-            id=linked_json["id"],
-            lat=linked_json["wgsy"],
-            lon=linked_json["wgsx"],
-            street_name=try_get(lambda: linked_json["st_name"]),
-        )
-        angle = math.radians(float(linked_json["pan"]))
-        links.append(Link(linked, angle))
-    return links
-
-
 def _generate_tile_list(pano: KakaoPanorama, zoom: int) -> List[Tile]:
     """
     Generates a list of a panorama's tiles and the URLs pointing to them.
     """
     if not (zoom == 1 or zoom == 2):
         raise ValueError("Call _get_thumbnail")
```

### Comparing `streetlevel-0.8.0/streetlevel/kakao/panorama.py` & `streetlevel-0.8.1/streetlevel/kakao/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/kakao/util.py` & `streetlevel-0.8.1/streetlevel/kakao/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/api.py` & `streetlevel-0.8.1/streetlevel/lookaround/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/auth.py` & `streetlevel-0.8.1/streetlevel/lookaround/auth.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/geo.py` & `streetlevel-0.8.1/streetlevel/lookaround/geo.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/panorama.py` & `streetlevel-0.8.1/streetlevel/lookaround/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/reproject.py` & `streetlevel-0.8.1/streetlevel/lookaround/reproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from PIL import Image
 from equilib import Equi2Equi
 import torch
 from torchvision import transforms
 
-from streetlevel.lookaround import CameraMetadata
+from streetlevel.lookaround.panorama import CameraMetadata
 
 _equi2equi = Equi2Equi(mode="bilinear", z_down=True)
 _device = torch.device("cuda")
 _to_tensor = transforms.Compose([transforms.ToTensor()])
 _to_pil = transforms.Compose([transforms.ToPILImage()])
```

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/util.py` & `streetlevel-0.8.1/streetlevel/lookaround/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/proto/GroundMetadataTile.proto` & `streetlevel-0.8.1/streetlevel/lookaround/proto/GroundMetadataTile.proto`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/proto/GroundMetadataTile_pb2.py` & `streetlevel-0.8.1/streetlevel/lookaround/proto/GroundMetadataTile_pb2.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/lookaround/proto/MuninViewState_pb2.py` & `streetlevel-0.8.1/streetlevel/lookaround/proto/MuninViewState_pb2.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/mapy/api.py` & `streetlevel-0.8.1/streetlevel/mapy/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/mapy/mapy.py` & `streetlevel-0.8.1/streetlevel/mapy/mapy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import itertools
-import math
 from typing import List, Optional
 
-from PIL import Image
 from aiohttp import ClientSession
+from PIL import Image
+from requests import Session
 
-from .panorama import MapyPanorama
 from . import api
-from requests import Session
-from ..dataclasses import Size, Tile, Link
-from ..geo import opk_to_rotation
+from .panorama import MapyPanorama
+from .parse import parse_pan_info_dict, parse_neighbors_response, parse_getbest_response
+from ..dataclasses import Tile, Link
 from ..util import get_equirectangular_panorama, get_equirectangular_panorama_async, get_image, get_image_async
 
 
 def find_panorama(lat: float, lon: float,
                   radius: float = 100.0,
                   year: Optional[int] = None,
                   links: bool = True,
@@ -27,58 +26,39 @@
     :param year: *(optional)* If given, searches for a specific year. Otherwise, the most recent panorama is returned.
     :param links: *(optional)* Whether an additional network request is made to fetch linked panoramas.
         Defaults to True.
     :param historical: *(optional)* Whether additional network requests are made to fetch metadata of
         panoramas from other years. Defaults to True.
     :return: A MapyPanorama object if a panorama was found, or None.
     """
-    radius = float(radius)
-    if year is None:
-        options = None
-    else:
-        options = {'year': year, 'nopenalties': True}
+    options, radius = _validate_find_panorama_params(radius, year)
     response = api.getbest(lat, lon, radius, options=options)
-
-    if response["status"] != 200:
-        return None
-
-    pan_info = response["result"]["panInfo"]
-    pano = _parse_pan_info_dict(pan_info)
+    pano = parse_getbest_response(response)
 
     if links:
         pano.links = get_links(pano.id, year=pano.date.year)
     if historical:
-        _append_historical(lat, lon, pan_info, pano)
+        _append_historical(pano, response["result"]["panInfo"], lat, lon)
 
     return pano
 
 
 async def find_panorama_async(lat: float, lon: float,
                               radius: float = 100.0,
                               year: Optional[int] = None,
                               links: bool = True,
                               historical: bool = True) -> Optional[MapyPanorama]:
-    # TODO reduce duplication
-    radius = float(radius)
-    if year is None:
-        options = None
-    else:
-        options = {'year': year, 'nopenalties': True}
+    options, radius = _validate_find_panorama_params(radius, year)
     response = await api.getbest_async(lat, lon, radius, options=options)
-
-    if response["status"] != 200:
-        return None
-
-    pan_info = response["result"]["panInfo"]
-    pano = _parse_pan_info_dict(pan_info)
+    pano = parse_getbest_response(response)
 
     if links:
         pano.links = await get_links_async(pano.id, year=pano.date.year)
     if historical:
-        await _append_historical_async(lat, lon, pan_info, pano)
+        await _append_historical_async(pano, response["result"]["panInfo"], lat, lon)
 
     return pano
 
 
 def find_panorama_by_id(panoid: int,
                         links: bool = True,
                         historical: bool = True) -> Optional[MapyPanorama]:
@@ -94,39 +74,39 @@
     """
     response = api.detail(panoid)
 
     if response["status"] != 200:
         return None
 
     pan_info = response["result"]
-    pano = _parse_pan_info_dict(pan_info)
+    pano = parse_pan_info_dict(pan_info)
 
     if links:
         pano.links = get_links(pano.id, year=pano.date.year)
     if historical:
-        _append_historical(pano.lat, pano.lon, pan_info, pano)
+        _append_historical(pano, pan_info, pano.lat, pano.lon)
 
     return pano
 
 
 async def find_panorama_by_id_async(panoid: int,
                                     links: bool = True,
                                     historical: bool = True) -> Optional[MapyPanorama]:
     response = await api.detail_async(panoid)
 
     if response["status"] != 200:
         return None
 
     pan_info = response["result"]
-    pano = _parse_pan_info_dict(pan_info)
+    pano = parse_pan_info_dict(pan_info)
 
     if links:
         pano.links = await get_links_async(pano.id, year=pano.date.year)
     if historical:
-        await _append_historical_async(pano.lat, pano.lon, pan_info, pano)
+        await _append_historical_async(pano, pan_info, pano.lat, pano.lon)
 
     return pano
 
 
 def get_links(panoid: int, year: Optional[int] = None) -> List[Link]:
     """
     Fetches linked panoramas.
@@ -138,33 +118,25 @@
     """
     if year is None:
         options = None
     else:
         options = {"year": year}
 
     response = api.getneighbours(panoid, options)
-
-    if response["status"] != 200:
-        return []
-
-    return _neighbors_response_to_links(response)
+    return parse_neighbors_response(response)
 
 
 async def get_links_async(panoid: int, year: Optional[int] = None) -> List[Link]:
     if year is None:
         options = None
     else:
         options = {"year": year}
 
     response = await api.getneighbours_async(panoid, options)
-
-    if response["status"] != 200:
-        return []
-
-    return _neighbors_response_to_links(response)
+    return parse_neighbors_response(response)
 
 
 def get_panorama(pano: MapyPanorama, zoom: int = 2) -> Image.Image:
     """
     Downloads a panorama and returns it as PIL image.
 
     :param pano: The panorama.
@@ -218,91 +190,41 @@
                                   zoom: int = 2, pil_args: dict = None) -> None:
     if pil_args is None:
         pil_args = {}
     image = await get_panorama_async(pano, session, zoom=zoom)
     image.save(path, **pil_args)
 
 
-def _append_historical(lat, lon, pan_info, pano):
+def _validate_find_panorama_params(radius, year):
+    radius = float(radius)
+    if year is None:
+        options = None
+    else:
+        options = {'year': year, 'nopenalties': True}
+    return options, radius
+
+
+def _append_historical(pano, pan_info, lat, lon):
     for year in pan_info["timeline"]:
         if pano.date.year == year:
             continue
         historical_pano = find_panorama(lat, lon, 50.0, year=year,
                                         historical=False, links=False)
         pano.historical.append(historical_pano)
 
 
-async def _append_historical_async(lat, lon, pan_info, pano):
+async def _append_historical_async(pano, pan_info, lat, lon):
     for year in pan_info["timeline"]:
         if pano.date.year == year:
             continue
         historical_pano = await find_panorama_async(lat, lon, 50.0, year=year,
                                                     historical=False, links=False)
         pano.historical.append(historical_pano)
 
 
-def _neighbors_response_to_links(response: dict) -> List[Link]:
-    panos = []
-    for pan_info in response["result"]["neighbours"]:
-        pano = _parse_pan_info_dict(pan_info["near"])
-        angle = math.radians(float(pan_info["angle"]))
-        panos.append(Link(pano, angle))
-    return panos
-
-
-def _parse_pan_info_dict(pan_info: dict) -> MapyPanorama:
-    pano = MapyPanorama(
-        id=pan_info["pid"],
-        lat=pan_info["mark"]["lat"],
-        lon=pan_info["mark"]["lon"],
-        tile_size=Size(pan_info["tileWidth"], pan_info["tileHeight"]),
-        domain_prefix=pan_info["domainPrefix"],
-        uri_path=pan_info["uriPath"],
-        file_mask=pan_info["fileMask"],
-        max_zoom=pan_info["maxZoom"],
-        date=pan_info["createdAt"],
-        elevation=pan_info["mark"]["alt"],
-        provider=pan_info["provider"],
-    )
-
-    _parse_angles(pan_info, pano)
-    pano.num_tiles = _parse_num_tiles(pan_info)
-
-    return pano
-
-
-def _parse_num_tiles(pan_info: dict) -> List[Size]:
-    # zoom level 0
-    num_tiles = [Size(1, 1)]
-    # zoom levels 1 and 2 for cyclomedia
-    if "extra" in pan_info and "tileNumX" in pan_info["extra"]:
-        for i in range(0, len(pan_info["extra"]["tileNumX"])):
-            num = Size(int(pan_info["extra"]["tileNumX"][i]),
-                       int(pan_info["extra"]["tileNumY"][i]))
-            num_tiles.append(num)
-    # zoom level 1 for other providers
-    else:
-        num_tiles.append(Size(pan_info["tileNumX"], pan_info["tileNumY"]))
-    return num_tiles
-
-
-def _parse_angles(pan_info: dict, pano: MapyPanorama) -> None:
-    if "extra" in pan_info and "carDirection" in pan_info["extra"]:
-        pano.heading = math.radians(pan_info["extra"]["carDirection"])
-
-    pano.omega = math.radians(pan_info["omega"])
-    pano.phi = math.radians(pan_info["phi"])
-    pano.kappa = math.radians(pan_info["kappa"])
-    heading, pitch, roll = opk_to_rotation(pano.omega, pano.phi, pano.kappa).as_euler('yxz')
-    if not pano.heading:
-        pano.heading = heading
-    pano.pitch = pitch
-    pano.roll = roll
-
-
 def _get_zoom_0(pano: MapyPanorama, session: Session = None) -> Image.Image:
     return get_image(_generate_tile_list(pano, 0)[0].url, session=session)
 
 
 async def _get_zoom_0_async(pano: MapyPanorama, session: ClientSession) -> Image.Image:
     return await get_image_async(_generate_tile_list(pano, 0)[0].url, session)
```

### Comparing `streetlevel-0.8.0/streetlevel/mapy/panorama.py` & `streetlevel-0.8.1/streetlevel/mapy/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/mapy/util.py` & `streetlevel-0.8.1/streetlevel/mapy/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/naver/api.py` & `streetlevel-0.8.1/streetlevel/naver/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/naver/naver.py` & `streetlevel-0.8.1/streetlevel/naver/naver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import math
-from datetime import datetime
 from typing import Optional, List, Union, Tuple
 
 import numpy as np
 from aiohttp import ClientSession
 from PIL import Image
 from requests import Session
 
 from . import api
-from .panorama import NaverPanorama, PanoramaType, Overlay, Neighbors
-from ..dataclasses import Tile, Link
+from .panorama import NaverPanorama, Neighbors
+from .parse import parse_panorama, parse_nearby, parse_historical, parse_neighbors
+from ..dataclasses import Tile
 from ..util import download_tiles, CubemapStitchingMethod, stitch_cubemap_faces, download_tiles_async, \
     save_cubemap_panorama, get_image, get_image_async, stitch_cubemap_face
 
 
 def find_panorama_by_id(panoid: str, language: str = "en",
                         neighbors: bool = True, historical: bool = True, depth: bool = False,
                         session: Session = None) -> Optional[NaverPanorama]:
@@ -33,15 +32,15 @@
     :return: A NaverPanorama object if a panorama with this ID exists, or None.
     """
     response = api.find_panorama_by_id(panoid, language, session)
 
     if "errors" in response:
         return None
 
-    pano = _parse_panorama(response)
+    pano = parse_panorama(response)
     if neighbors:
         pano.neighbors = get_neighbors(pano.id, session=session)
     if historical:
         pano.historical = get_historical(pano.timeline_id, session=session)
     if depth:
         pano.depth = get_depth(pano.id, session=session)
     return pano
@@ -50,15 +49,15 @@
 async def find_panorama_by_id_async(panoid: str, session: ClientSession, language: str = "en", neighbors: bool = True,
                                     historical: bool = True, depth: bool = False) -> Optional[NaverPanorama]:
     response = await api.find_panorama_by_id_async(panoid, language, session)
 
     if "errors" in response:
         return None
 
-    pano = _parse_panorama(response)
+    pano = parse_panorama(response)
     if neighbors:
         pano.neighbors = await get_neighbors_async(pano.id, session)
     if historical:
         pano.historical = await get_historical_async(pano.timeline_id, session)
     if depth:
         pano.depth = await get_depth_async(pano.id, session)
     return pano
@@ -83,15 +82,15 @@
     :return: A NaverPanorama object if a panorama was found, or None.
     """
     response = api.find_panorama(lat, lon, session)
 
     if "error" in response or len(response["features"]) == 0:
         return None
 
-    pano = _parse_nearby(response)
+    pano = parse_nearby(response)
     if neighbors:
         pano.neighbors = get_neighbors(pano.id, session=session)
     if historical:
         pano.historical = get_historical(pano.id, session=session)
     if depth:
         pano.depth = get_depth(pano.id, session=session)
     return pano
@@ -100,15 +99,15 @@
 async def find_panorama_async(lat: float, lon: float, session: ClientSession, neighbors: bool = True,
                               historical: bool = True, depth: bool = False) -> Optional[NaverPanorama]:
     response = await api.find_panorama_async(lat, lon, session)
 
     if "error" in response or len(response["features"]) == 0:
         return None
 
-    pano = _parse_nearby(response)
+    pano = parse_nearby(response)
     if neighbors:
         pano.neighbors = await get_neighbors_async(pano.id, session)
     if historical:
         pano.historical = await get_historical_async(pano.id, session)
     if depth:
         pano.depth = await get_depth_async(pano.id, session)
     return pano
@@ -125,24 +124,24 @@
     :return: A list of NaverPanorama objects.
     """
     response = api.get_historical(panoid, session=session)
 
     if "errors" in response:
         return []
 
-    return _parse_historical(response, panoid)
+    return parse_historical(response, panoid)
 
 
 async def get_historical_async(panoid: str, session: ClientSession) -> List[NaverPanorama]:
     response = await api.get_historical_async(panoid, session)
 
     if "errors" in response:
         return []
 
-    return _parse_historical(response, panoid)
+    return parse_historical(response, panoid)
 
 
 def get_neighbors(panoid: str, session: Session = None) -> Neighbors:
     """
     Fetches neighbors of a panorama.
 
     :param panoid: The pano ID.
@@ -150,24 +149,24 @@
     :return: A Neighbors object.
     """
     response = api.get_neighbors(panoid, session=session)
 
     if "errors" in response:
         return Neighbors([], [])
 
-    return _parse_neighbors(response, panoid)
+    return parse_neighbors(response, panoid)
 
 
 async def get_neighbors_async(panoid: str, session: ClientSession) -> Neighbors:
     response = await api.get_neighbors_async(panoid, session)
 
     if "errors" in response:
         return Neighbors([], [])
 
-    return _parse_neighbors(response, panoid)
+    return parse_neighbors(response, panoid)
 
 
 def get_panorama(pano: NaverPanorama, zoom: int = 2,
                  stitching_method: CubemapStitchingMethod = CubemapStitchingMethod.ROW) \
         -> Union[List[Image.Image], Image.Image]:
     """
     Downloads a panorama and returns it as PIL image.
@@ -319,106 +318,7 @@
 def _stitch_panorama(tile_images: List[dict], cols: int, rows: int,
                      stitching_method: CubemapStitchingMethod) -> Union[List[Image.Image], Image.Image]:
     stitched_faces = []
     for tiles in tile_images:
         stitched_face = stitch_cubemap_face(tiles, 512, cols, rows)
         stitched_faces.append(stitched_face)
     return stitch_cubemap_faces(stitched_faces, stitched_faces[0].size[0], stitching_method)
-
-
-def _parse_neighbors(response: dict, parent_id: str) -> Neighbors:
-    street = _parse_neighbor_section(response, "street", parent_id)
-    other = _parse_neighbor_section(response, "air", parent_id)
-    return Neighbors(street, other)
-
-
-def _parse_neighbor_section(response: dict, section: str, parent_id: str) -> List[NaverPanorama]:
-    panos = []
-    if section in response["around"]["panoramas"]:
-        for raw_pano in response["around"]["panoramas"][section][1:]:
-            if raw_pano[0] == parent_id:
-                continue
-            elevation = raw_pano[4] * 0.01
-            pano = NaverPanorama(
-                id=raw_pano[0],
-                lat=raw_pano[2],
-                lon=raw_pano[1],
-                elevation=elevation,
-                camera_height=(raw_pano[3] * 0.01) - elevation)
-            panos.append(pano)
-    return panos
-
-
-def _parse_historical(response: dict, parent_id: str) -> List[NaverPanorama]:
-    panos = response["timeline"]["panoramas"][1:]
-    return [NaverPanorama(
-        id=pano[0],
-        lat=pano[2],
-        lon=pano[1],
-        date=datetime.strptime(pano[3], "%Y-%m-%d %H:%M:%S.0")
-    ) for pano in panos if pano[0] != parent_id]
-
-
-def _parse_nearby(response: dict) -> NaverPanorama:
-    feature = response["features"][0]
-    elevation = feature["properties"]["land_altitude"] * 0.01
-    return NaverPanorama(
-        id=feature["properties"]["id"],
-        lat=feature["geometry"]["coordinates"][1],
-        lon=feature["geometry"]["coordinates"][0],
-        heading=math.radians(feature["properties"]["camera_angle"][1]),
-        date=_parse_date(feature["properties"]["photodate"]),
-        description=feature["properties"]["description"],
-        title=feature["properties"]["title"],
-        elevation=elevation,
-        camera_height=(feature["properties"]["camera_altitude"] * 0.01) - elevation
-    )
-
-
-def _parse_date(date_str: str) -> datetime:
-    return datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")
-
-
-def _parse_panorama(response: dict) -> NaverPanorama:
-    basic = response["basic"]
-    elevation = basic["land_altitude"] * 0.01
-    pano = NaverPanorama(
-        id=basic["id"],
-        lat=basic["latitude"],
-        lon=basic["longitude"],
-        heading=math.radians(basic["camera_angle"][1]),
-        max_zoom=int(basic["image"]["segment"]) // 2,
-        timeline_id=basic["timeline_id"],
-        date=_parse_date(basic["photodate"]),
-        is_latest=basic["latest"],
-        description=basic["description"],
-        title=basic["title"],
-        panorama_type=PanoramaType(int(basic["dtl_type"])),
-        elevation=elevation,
-        camera_height=(basic["camera_altitude"] * 0.01) - elevation
-    )
-
-    if len(basic["image"]["overlays"]) > 1:
-        pano.overlay = Overlay(
-            "https://panorama.map.naver.com" + basic["image"]["overlays"][1][0],
-            "https://panorama.map.naver.com" + basic["image"]["overlays"][1][1])
-
-    pano.links = _parse_links(basic["links"])
-
-    return pano
-
-
-def _parse_links(links_json: List) -> Optional[List[Link]]:
-    if len(links_json) < 2:
-        return None
-
-    links = []
-    for linked_json in links_json[1:]:
-        linked = NaverPanorama(
-            id=linked_json[0],
-            title=linked_json[1],
-            lat=linked_json[5],
-            lon=linked_json[4],
-        )
-        angle = math.radians(float(linked_json[2]))
-        links.append(Link(linked, angle))
-    return links
```

### Comparing `streetlevel-0.8.0/streetlevel/naver/panorama.py` & `streetlevel-0.8.1/streetlevel/naver/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/naver/util.py` & `streetlevel-0.8.1/streetlevel/naver/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetside/api.py` & `streetlevel-0.8.1/streetlevel/streetside/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetside/panorama.py` & `streetlevel-0.8.1/streetlevel/streetside/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetside/util.py` & `streetlevel-0.8.1/streetlevel/streetside/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetview/api.py` & `streetlevel-0.8.1/streetlevel/streetview/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetview/depth.py` & `streetlevel-0.8.1/streetlevel/streetview/depth.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetview/panorama.py` & `streetlevel-0.8.1/streetlevel/streetview/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/streetview/protobuf.py` & `streetlevel-0.8.1/streetlevel/streetview/protobuf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Some code to deal with the URL-encoded protobuf Google uses in Maps.
 from enum import Enum
-
+from decimal import Decimal
 
 class ProtobufType(Enum):
     """
     Data types found in protobuf and their identifier in the URL encoded version.
     """
     # There are more data types in protobuf,
     # these are just the ones I've encountered in this project
@@ -84,12 +84,14 @@
         datatype = ProtobufType.BOOL
     elif isinstance(value, ProtobufEnum):
         datatype = ProtobufType.ENUM
     elif isinstance(value, int):
         datatype = ProtobufType.INT
     elif isinstance(value, float):
         datatype = ProtobufType.DOUBLE
+    elif isinstance(value, Decimal):
+        datatype = ProtobufType.DOUBLE
     elif isinstance(value, dict):
         datatype = ProtobufType.MESSAGE
     else:
         raise NotImplementedError(value)
     return datatype
```

### Comparing `streetlevel-0.8.0/streetlevel/streetview/util.py` & `streetlevel-0.8.1/streetlevel/streetview/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/yandex/api.py` & `streetlevel-0.8.1/streetlevel/yandex/api.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/yandex/panorama.py` & `streetlevel-0.8.1/streetlevel/yandex/panorama.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/yandex/util.py` & `streetlevel-0.8.1/streetlevel/yandex/util.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/streetlevel/yandex/yandex.py` & `streetlevel-0.8.1/streetlevel/streetview/streetview.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,298 +1,201 @@
+from aiohttp import ClientSession
 import itertools
 import math
-from datetime import datetime
-from typing import List, Optional, Tuple
-import re
-
 from PIL import Image
-from aiohttp import ClientSession
 from requests import Session
+from typing import List, Optional
 
 from . import api
-from .panorama import YandexPanorama, Place, Address, Marker
-from ..dataclasses import Size, Tile, Link
-from ..util import try_get, get_equirectangular_panorama, get_equirectangular_panorama_async
-
-
-def find_panorama(lat: float, lon: float, session: Session = None) -> Optional[YandexPanorama]:
-    """
-    Searches for a panorama near the given point.
-
-    Aerial panoramas are ignored by this API call.
-
-    :param lat: Latitude of the point.
-    :param lon: Longitude of the point.
+from .panorama import StreetViewPanorama
+from .parse import parse_coverage_tile_response, parse_panorama_id_response, \
+    parse_panorama_radius_response
+from .util import is_third_party_panoid
+from ..dataclasses import Tile
+from ..geo import wgs84_to_tile_coord
+from ..util import get_equirectangular_panorama, get_equirectangular_panorama_async
+
+
+def find_panorama(lat: float, lon: float, radius: int = 50, locale: str = "en",
+                  search_third_party: bool = False, session: Session = None) -> Optional[StreetViewPanorama]:
+    """
+    Searches for a panorama within a radius around a point.
+
+    :param lat: Latitude of the center point.
+    :param lon: Longitude of the center point.
+    :param radius: *(optional)* Search radius in meters. Defaults to 50.
+    :param locale: *(optional)* Desired language of the location's address as IETF code.
+      Defaults to ``en``.
+    :param search_third_party: *(optional)* Whether to search for third-party panoramas
+      rather than official ones. Defaults to false.
     :param session: *(optional)* A requests session.
-    :return: A YandexPanorama object if a panorama was found, or None.
+    :return: A StreetViewPanorama object if a panorama was found, or None.
     """
 
-    resp = api.find_panorama(lat, lon, session)
+    # TODO
+    # the `SingleImageSearch` call returns a different kind of depth data
+    # than `photometa`; need to deal with that at some point
 
-    if resp["status"] == "error":
-        return None
+    response = api.find_panorama(lat, lon, radius=radius, download_depth=False,
+                                 locale=locale, search_third_party=search_third_party, session=session)
+    return parse_panorama_radius_response(response)
 
-    pano = _parse_panorama(resp["data"])
-    return pano
 
+async def find_panorama_async(lat: float, lon: float, session: ClientSession, radius: int = 50,
+                              locale: str = "en", search_third_party: bool = False) -> Optional[StreetViewPanorama]:
+    # TODO
+    # the `SingleImageSearch` call returns a different kind of depth data
+    # than `photometa`; need to deal with that at some point
+    response = await api.find_panorama_async(lat, lon, session, radius=radius, download_depth=False,
+                                             locale=locale, search_third_party=search_third_party)
+    return parse_panorama_radius_response(response)
 
-async def find_panorama_async(lat: float, lon: float, session: ClientSession) -> Optional[YandexPanorama]:
-    resp = await api.find_panorama_async(lat, lon, session)
 
-    if resp["status"] == "error":
-        return None
-
-    pano = _parse_panorama(resp["data"])
-    return pano
-
-
-def find_panorama_by_id(panoid: str, session: Session = None) -> Optional[YandexPanorama]:
+def find_panorama_by_id(panoid: str, download_depth: bool = False, locale: str = "en",
+                        session: Session = None) -> Optional[StreetViewPanorama]:
     """
     Fetches metadata of a specific panorama.
 
+    Unfortunately, `as mentioned on this page
+    <https://developers.google.com/maps/documentation/tile/streetview#panoid_response>`_,
+    pano IDs are not stable, so a request that works today may return nothing a few months into the future.
+
     :param panoid: The pano ID.
+    :param download_depth: Whether to download and parse the depth map.
+    :param locale: Desired language of the location's address as IETF code.
     :param session: *(optional)* A requests session.
-    :return: A YandexPanorama object if a panorama with this ID exists, or None.
+    :return: A StreetViewPanorama object if a panorama with this ID exists, or None.
     """
-    resp = api.find_panorama_by_id(panoid, session)
-
-    if resp["status"] == "error":
-        return None
+    response = api.find_panorama_by_id(panoid, download_depth=download_depth,
+                                       locale=locale, session=session)
+    return parse_panorama_id_response(response)
 
-    pano = _parse_panorama(resp["data"])
-    return pano
 
+async def find_panorama_by_id_async(panoid: str, session: ClientSession, download_depth: bool = False,
+                                    locale: str = "en") -> Optional[StreetViewPanorama]:
+    response = await api.find_panorama_by_id_async(panoid, session,
+                                                   download_depth=download_depth, locale=locale)
+    return parse_panorama_id_response(response)
 
-async def find_panorama_by_id_async(panoid: str, session: ClientSession) -> Optional[YandexPanorama]:
-    resp = await api.find_panorama_by_id_async(panoid, session)
 
-    if resp["status"] == "error":
-        return None
+def get_coverage_tile(tile_x: int, tile_y: int, session: Session = None) -> List[StreetViewPanorama]:
+    """
+    Fetches Street View coverage on a specific map tile. Coordinates are in Slippy Map aka XYZ format
+    at zoom level 17.
 
-    pano = _parse_panorama(resp["data"])
-    return pano
+    When viewing Google Maps with satellite imagery in globe view and zooming into a spot,
+    it makes this API call. This is useful because 1) it allows for fetching coverage for a whole area, and
+    2) there are various hidden/removed locations which cannot be found by any other method
+    (unless you access them by pano ID directly).
 
+    This function returns ID, position, elevation, orientation, and links within the tile of the most recent coverage.
+    The rest of the metadata, such as historical panoramas or links across tiles, must be fetched manually one by one.
 
-def get_panorama(pano: YandexPanorama, zoom: int = 0) -> Image.Image:
+    :param tile_x: X coordinate of the tile.
+    :param tile_y: Y coordinate of the tile.
+    :param session: *(optional)* A requests session.
+    :return: A list of StreetViewPanoramas. If no coverage was returned by the API, the list is empty.
     """
-    Downloads a panorama and returns it as PIL image.
+    response = api.get_coverage_tile(tile_x, tile_y, session)
+    return parse_coverage_tile_response(response)
 
-    Note that most official car coverage has its bottom part cropped out.
 
-    :param pano: The panorama to download.
-    :param zoom: *(optional)* Image size; 0 is highest, 4 is lowest. The dimensions of a zoom level of a
-        specific panorama depend on the camera used. If the requested zoom level does not exist,
-        the highest available level will be downloaded. Defaults to 0.
-    :return: A PIL image containing the panorama.
+async def get_coverage_tile_async(tile_x: int, tile_y: int, session: ClientSession) -> List[StreetViewPanorama]:
+    response = await api.get_coverage_tile_async(tile_x, tile_y, session)
+    return parse_coverage_tile_response(response)
+
+
+def get_coverage_tile_by_latlon(lat: float, lon: float, session: Session = None) -> List[StreetViewPanorama]:
     """
-    zoom = _validate_get_panorama_params(pano, zoom)
-    return get_equirectangular_panorama(
-        pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
-        pano.tile_size, _generate_tile_list(pano, zoom))
+    Same as :func:`get_coverage_tile <get_coverage_tile>`, but for fetching the tile on which a point is located.
+
+    :param lat: Latitude of the point.
+    :param lon: Longitude of the point.
+    :param session: *(optional)* A requests session.
+    :return: A list of StreetViewPanoramas. If no coverage was returned by the API, the list is empty.
+    """
+    tile_coord = wgs84_to_tile_coord(lat, lon, 17)
+    return get_coverage_tile(tile_coord[0], tile_coord[1], session=session)
 
 
-async def get_panorama_async(pano: YandexPanorama, session: ClientSession, zoom: int = 0) -> Image.Image:
-    zoom = _validate_get_panorama_params(pano, zoom)
-    return await get_equirectangular_panorama_async(
-        pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
-        pano.tile_size, _generate_tile_list(pano, zoom),
-        session)
+async def get_coverage_tile_by_latlon_async(lat: float, lon: float, session: ClientSession) \
+        -> List[StreetViewPanorama]:
+    tile_coord = wgs84_to_tile_coord(lat, lon, 17)
+    return await get_coverage_tile_async(tile_coord[0], tile_coord[1], session)
 
 
-def download_panorama(pano: YandexPanorama, path: str, zoom: int = 0, pil_args: dict = None) -> None:
+def download_panorama(pano: StreetViewPanorama, path: str, zoom: int = 5, pil_args: dict = None) -> None:
     """
     Downloads a panorama to a file.
 
-    Note that most official car coverage has its bottom part cropped out.
-
     :param pano: The panorama to download.
     :param path: Output path.
-    :param zoom: *(optional)* Image size; 0 is highest, 4 is lowest. The dimensions of a zoom level of a
+    :param zoom: *(optional)* Image size; 0 is lowest, 5 is highest. The dimensions of a zoom level of a
         specific panorama depend on the camera used. If the requested zoom level does not exist,
-        the highest available level will be downloaded. Defaults to 0.
+        the highest available level will be downloaded. Defaults to 5.
     :param pil_args: *(optional)* Additional arguments for PIL's
         `Image.save <https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.save>`_
         method, e.g. ``{"quality":100}``. Defaults to ``{}``.
     """
     if pil_args is None:
         pil_args = {}
     image = get_panorama(pano, zoom=zoom)
     image.save(path, **pil_args)
 
 
-async def download_panorama_async(pano: YandexPanorama, path: str, session: ClientSession,
-                                  zoom: int = 0, pil_args: dict = None) -> None:
+async def download_panorama_async(pano: StreetViewPanorama, path: str, session: ClientSession,
+                                  zoom: int = 5, pil_args: dict = None) -> None:
     if pil_args is None:
         pil_args = {}
     image = await get_panorama_async(pano, session, zoom=zoom)
     image.save(path, **pil_args)
 
 
-def _generate_tile_list(pano: YandexPanorama, zoom: int) -> List[Tile]:
+def get_panorama(pano: StreetViewPanorama, zoom: int = 5) -> Image.Image:
     """
-    Generates a list of a panorama's tiles and the URLs pointing to them.
+    Downloads a panorama and returns it as PIL image.
+
+    :param pano: The panorama to download.
+    :param zoom: *(optional)* Image size; 0 is lowest, 5 is highest. The dimensions of a zoom level of a
+        specific panorama depend on the camera used. If the requested zoom level does not exist,
+        the highest available level will be downloaded. Defaults to 5.
+    :return: A PIL image containing the panorama.
     """
-    img_size = pano.image_sizes[zoom]
-    tile_width = pano.tile_size.x
-    tile_height = pano.tile_size.y
-    cols = math.ceil(img_size.x / tile_width)
-    rows = math.ceil(img_size.y / tile_height)
+    zoom = _validate_get_panorama_params(pano, zoom)
+    return get_equirectangular_panorama(
+        pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
+        pano.tile_size, _generate_tile_list(pano, zoom))
 
-    IMAGE_URL = "https://pano.maps.yandex.net/{0:}/{1:}.{2:}.{3:}"
 
-    coords = list(itertools.product(range(cols), range(rows)))
-    tiles = [Tile(x, y, IMAGE_URL.format(pano.image_id, zoom, x, y)) for x, y in coords]
-    return tiles
+async def get_panorama_async(pano: StreetViewPanorama, session: ClientSession, zoom: int = 5) -> Image.Image:
+    zoom = _validate_get_panorama_params(pano, zoom)
+    return await get_equirectangular_panorama_async(
+        pano.image_sizes[zoom].x, pano.image_sizes[zoom].y,
+        pano.tile_size, _generate_tile_list(pano, zoom),
+        session)
 
 
-def _validate_get_panorama_params(pano: YandexPanorama, zoom: int) -> int:
+def _validate_get_panorama_params(pano: StreetViewPanorama, zoom: int) -> int:
     if not pano.image_sizes:
         raise ValueError("pano.image_sizes is None.")
     zoom = max(0, min(zoom, len(pano.image_sizes) - 1))
     return zoom
 
 
-def _parse_panorama(pano_dict: dict) -> YandexPanorama:
-    data = pano_dict["Data"]
-    annotation = pano_dict["Annotation"]
-    panoid = data["panoramaId"]
-
-    addresses, other_markers = _parse_markers(annotation["Markers"])
-
-    return YandexPanorama(
-        id=panoid,
-        lat=float(data["Point"]["coordinates"][1]),
-        lon=float(data["Point"]["coordinates"][0]),
-
-        heading=math.radians(float(data["EquirectangularProjection"]["Origin"][0])),
-
-        image_id=data["Images"]["imageId"],
-        tile_size=Size(int(data["Images"]["Tiles"]["width"]),
-                       int(data["Images"]["Tiles"]["height"])),
-        image_sizes=_parse_image_sizes(data["Images"]["Zooms"]),
-
-        neighbors=_parse_neighbors(annotation["Graph"]["Nodes"],
-                                   annotation["Connections"],
-                                   panoid),
-        links=_parse_links(annotation["Thoroughfares"]),
-        historical=_parse_historical(annotation["HistoricalPanoramas"], panoid),
-
-        date=_get_date_from_panoid(panoid),
-        height=int(data["Point"]["coordinates"][2]),
-        street_name=data["Point"]["name"],
-
-        places=_parse_companies(annotation["Companies"]),
-        addresses=addresses,
-        other_markers=other_markers,
-
-        author=try_get(lambda: pano_dict["Author"]["name"]),
-        author_avatar_url=try_get(lambda: pano_dict["Author"]["avatarUrlTemplate"]),
-    )
-
-
-def _parse_companies(companies_json: list) -> List[Place]:
-    companies = []
-    for company in companies_json:
-        companies.append(Place(
-            id=int(company["properties"]["id"]),
-            lat=company["geometry"]["coordinates"][1],
-            lon=company["geometry"]["coordinates"][0],
-            name=company["properties"]["name"],
-            tags=company["properties"]["tags"],
-        ))
-    return companies
-
-
-def _parse_markers(markers_json: list) -> Tuple[List[Address], List[Marker]]:
-    addresses = []
-    other_markers = []
-    for marker in markers_json:
-        # Address markers are displayed at a height of 7 m;
-        # all others, like metro icons, have a height of 2 m.
-        if marker["geometry"]["coordinates"][2] == 7:
-            addresses.append(Address(
-                lat=marker["geometry"]["coordinates"][1],
-                lon=marker["geometry"]["coordinates"][0],
-                house_number=marker["properties"]["name"],
-                street_name_and_house_number=marker["properties"]["description"],
-            ))
-        else:
-            other_markers.append(Marker(
-                lat=marker["geometry"]["coordinates"][1],
-                lon=marker["geometry"]["coordinates"][0],
-                name=marker["properties"]["name"],
-                description=marker["properties"]["description"],
-                style=marker["properties"]["style"],
-            ))
-
-    return addresses, other_markers
-
-
-def _parse_links(links_json):
-    links = []
-    for link_json in links_json:
-        panoid = _get_panoid_from_url(link_json["Connection"]["href"])
-        angle = math.radians(float(link_json["Direction"][0]))
-        links.append(Link(panoid, angle))
-    return links
-
-
-def _get_panoid_from_url(url: str) -> str:
-    return re.findall(r"oid=(.*?)&", url)[0]
-
-
-def _get_date_from_panoid(panoid: str) -> datetime:
-    return datetime.utcfromtimestamp(int(panoid.split("_")[-1]))
-
-
-def _parse_image_sizes(zooms: dict) -> List[Size]:
-    sizes = [None] * len(zooms)
-    for zoom in zooms:
-        idx = int(zoom["level"])
-        sizes[idx] = Size(int(zoom["width"]), int(zoom["height"]))
-    return sizes
-
-
-def _parse_neighbors(nodes: List[dict], connections: List[dict], parent_id: str) -> List[YandexPanorama]:
-    panos = []
-    for node in nodes:
-        panoid = node["panoid"]
-        if panoid == parent_id:
-            continue
-        pano = YandexPanorama(
-            id=panoid,
-            lat=float(node["lat"]),
-            lon=float(node["lon"]),
-            date=_get_date_from_panoid(panoid),
-        )
-        panos.append(pano)
-
-    for connection in connections:
-        panoid = _get_panoid_from_url(connection["href"])
-        pano = YandexPanorama(
-            id=panoid,
-            lat=connection["Point"]["coordinates"][1],
-            lon=connection["Point"]["coordinates"][0],
-            height=connection["Point"]["coordinates"][2],
-            date=_get_date_from_panoid(panoid),
-        )
-        panos.append(pano)
-
-    return panos
-
-
-def _parse_historical(historical: List[dict], parent_id: str) -> List[YandexPanorama]:
-    panos = []
-    for raw_pano in historical:
-        panoid = raw_pano["Connection"]["oid"]
-        if panoid == parent_id:
-            continue
-        pano = YandexPanorama(
-            id=panoid,
-            lat=float(raw_pano["Connection"]["Point"]["coordinates"][1]),
-            lon=float(raw_pano["Connection"]["Point"]["coordinates"][0]),
-            height=int(raw_pano["Connection"]["Point"]["coordinates"][2]),
-            date=_get_date_from_panoid(panoid)
-        )
-        panos.append(pano)
-    panos = sorted(panos, key=lambda x: x.date, reverse=True)
-    return panos
+def _generate_tile_list(pano: StreetViewPanorama, zoom: int) -> List[Tile]:
+    """
+    Generates a list of a panorama's tiles and the URLs pointing to them.
+    """
+    img_size = pano.image_sizes[zoom]
+    tile_width = pano.tile_size.x
+    tile_height = pano.tile_size.y
+    cols = math.ceil(img_size.x / tile_width)
+    rows = math.ceil(img_size.y / tile_height)
+
+    IMAGE_URL = "https://cbk0.google.com/cbk?output=tile&panoid={0:}&zoom={3:}&x={1:}&y={2:}"
+    THIRD_PARTY_IMAGE_URL = "https://lh3.ggpht.com/p/{0:}=x{1:}-y{2:}-z{3:}"
+
+    url_to_use = THIRD_PARTY_IMAGE_URL if is_third_party_panoid(pano.id) else IMAGE_URL
+
+    coords = list(itertools.product(range(cols), range(rows)))
+    tiles = [Tile(x, y, url_to_use.format(pano.id, x, y, zoom)) for x, y in coords]
+    return tiles
```

### Comparing `streetlevel-0.8.0/tests/geo_test.py` & `streetlevel-0.8.1/tests/geo_test.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/lookaround/geo_test.py` & `streetlevel-0.8.1/tests/lookaround/geo_test.py`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/lookaround/data/metadata_tile.pb` & `streetlevel-0.8.1/tests/lookaround/data/metadata_tile.pb`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/mapy/mapy_test.py` & `streetlevel-0.8.1/tests/mapy/mapy_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import pytest
 from pytest import approx
 import pickle
+
 from streetlevel import mapy
+import streetlevel.mapy.parse
 from streetlevel.dataclasses import Size
 
 
-def mocked_getbest(lat, lon, radius, options=None):
+def test_parse_getbest_response():
     with open("mapy/data/getbest.pkl", "rb") as f:
-        return pickle.load(f)
-
-
-mapy.api.getbest = mocked_getbest
-
+        response = pickle.load(f)
 
-def test_find_panorama():
-    pano = mapy.find_panorama(50.1265193, 17.3762701, 100.0, historical=False, links=False)
+    pano = mapy.parse.parse_getbest_response(response)
     assert pano.id == 59418543
     assert pano.lat == approx(50.1265193, 0.001)
     assert pano.lon == approx(17.3762701, 0.001)
     assert pano.provider == "stavinvex"
     assert pano.num_tiles == [Size(x=1, y=1), Size(x=16, y=8)]
     assert pano.pitch == approx(0.01970877694733808, 0.001)
     assert pano.roll == approx(0.019988022665593075, 0.001)
```

### Comparing `streetlevel-0.8.0/tests/mapy/data/getbest.pkl` & `streetlevel-0.8.1/tests/mapy/data/getbest.pkl`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetside/streetside_test.py` & `streetlevel-0.8.1/tests/streetside/streetside_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from pytest import approx
 import json
+
 from streetlevel import streetside
+import streetlevel.streetside.parse
 
 
-def mocked_api_find_panoramas(north, west, south, east, limit=50, session=None):
+def test_parse_panoramas():
     with open("streetside/data/find.json", "r") as f:
-        return json.load(f)
-
-
-streetside.api.find_panoramas = mocked_api_find_panoramas
-
+        response = json.load(f)
 
-def test_find_panoramas_in_bbox():
-    panos = streetside.find_panoramas_in_bbox(-23.860792, 35.343169, -23.863089, 35.347470)
+    panos = streetside.parse.parse_panoramas(response)
     assert len(panos) != 0
     assert panos[0].id == 362530254
     assert panos[0].lat == approx(-23.862083, 0.001)
     assert panos[0].lon == approx(35.34479, 0.001)
 
 
 def test_to_base4():
```

### Comparing `streetlevel-0.8.0/tests/streetside/data/find.json` & `streetlevel-0.8.1/tests/streetside/data/find.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/coverage_tile.json` & `streetlevel-0.8.1/tests/streetview/data/coverage_tile.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/find.json` & `streetlevel-0.8.1/tests/streetview/data/find.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/find_by_id.json` & `streetlevel-0.8.1/tests/streetview/data/find_by_id.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/missing_date.json` & `streetlevel-0.8.1/tests/streetview/data/missing_date.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/missing_historical_date.json` & `streetlevel-0.8.1/tests/streetview/data/missing_historical_date.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/missing_level_name.json` & `streetlevel-0.8.1/tests/streetview/data/missing_level_name.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/missing_link_direction.json` & `streetlevel-0.8.1/tests/streetview/data/missing_link_direction.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/nepal_links.json` & `streetlevel-0.8.1/tests/streetview/data/nepal_links.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/places.json` & `streetlevel-0.8.1/tests/streetview/data/places.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/streetview/data/street_names.json` & `streetlevel-0.8.1/tests/streetview/data/street_names.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/tests/yandex/yandex_test.py` & `streetlevel-0.8.1/tests/yandex/yandex_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from datetime import datetime
-
-from pytest import approx
 import json
 
-from requests import Session
+from pytest import approx
 
 from streetlevel import yandex
+import streetlevel.yandex.parse
 
 
-def mocked_api_find_panorama(lat: float, lon: float, session: Session = None) -> dict:
+def test_parse_panorama_response():
     with open("yandex/data/find.json", "r") as f:
-        return json.load(f)
-
-
-yandex.api.find_panorama = mocked_api_find_panorama
-
+        response = json.load(f)
 
-def test_find_panorama():
-    pano = yandex.find_panorama(53.917633, 27.548128)
+    pano = yandex.parse.parse_panorama_response(response)
     assert pano.id == "1238072810_692204477_23_1688105969"
     assert pano.lat == approx(53.917633, 0.001)
     assert pano.lon == approx(27.548128, 0.001)
     assert pano.date == datetime.utcfromtimestamp(1688105969)
     assert pano.image_id == "WhpeuZGm2FIL"
     assert pano.image_sizes[0].x == 17664
     assert pano.image_sizes[0].y == 6145
```

### Comparing `streetlevel-0.8.0/tests/yandex/data/find.json` & `streetlevel-0.8.1/tests/yandex/data/find.json`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/.gitignore` & `streetlevel-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/LICENSE` & `streetlevel-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streetlevel-0.8.0/README.md` & `streetlevel-0.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # streetlevel
-**streetlevel** is a library for downloading panoramas and metadata from street-level imagery services including Google Street View, Apple Look Around, and several others.
+**streetlevel** is a library for downloading panoramas and metadata from street-level imagery services
+such as Google Street View, Apple Look Around, and several others. It provides a high-level abstraction
+over the internal APIs of the supported services &ndash; this means that no API keys are required, but the
+library may break unexpectedly. 
 
-Since it relies on calls to internal APIs, it may break unexpectedly.
-
-(Nearly) all functions are available as both a sync function using `requests` or an async function using `aiohttp`, requiring a `ClientSession`.
+(Nearly) all functions are available as either a sync function using `requests` or an async function
+using `aiohttp`, requiring a `ClientSession`.
 
 ## Installation
 ```sh
 pip install streetlevel
 ```
 
 ## Example
```

### Comparing `streetlevel-0.8.0/pyproject.toml` & `streetlevel-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "streetlevel"
-version = "0.8.0"
+version = "0.8.1"
 license = "MIT"
 authors = [
   { name="sk-zk", email="sk-zk@users.noreply.github.com" },
 ]
 description = "Download panoramas and metadata from Street View and others"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -18,14 +18,15 @@
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
     "Pillow",
     "aiohttp",
+    "cython",
     "numpy",
     "protobuf > 4",
     "pycryptodome",
     "pyequilib",
     "pyfrpc",
     "pyproj",
     "pytest",
```

### Comparing `streetlevel-0.8.0/PKG-INFO` & `streetlevel-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: streetlevel
-Version: 0.8.0
+Version: 0.8.1
 Summary: Download panoramas and metadata from Street View and others
 Project-URL: Homepage, https://github.com/sk-zk/streetlevel
 Project-URL: Bug Tracker, https://github.com/sk-zk/streetlevel/issues
 Author-email: sk-zk <sk-zk@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
+Requires-Dist: cython
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: protobuf>4
 Requires-Dist: pycryptodome
 Requires-Dist: pyequilib
 Requires-Dist: pyfrpc
 Requires-Dist: pyproj
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: requests
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # streetlevel
-**streetlevel** is a library for downloading panoramas and metadata from street-level imagery services including Google Street View, Apple Look Around, and several others.
+**streetlevel** is a library for downloading panoramas and metadata from street-level imagery services
+such as Google Street View, Apple Look Around, and several others. It provides a high-level abstraction
+over the internal APIs of the supported services &ndash; this means that no API keys are required, but the
+library may break unexpectedly. 
 
-Since it relies on calls to internal APIs, it may break unexpectedly.
-
-(Nearly) all functions are available as both a sync function using `requests` or an async function using `aiohttp`, requiring a `ClientSession`.
+(Nearly) all functions are available as either a sync function using `requests` or an async function
+using `aiohttp`, requiring a `ClientSession`.
 
 ## Installation
 ```sh
 pip install streetlevel
 ```
 
 ## Example
```

