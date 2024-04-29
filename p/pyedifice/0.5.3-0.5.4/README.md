# Comparing `tmp/pyedifice-0.5.3.tar.gz` & `tmp/pyedifice-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedifice-0.5.3.tar", max compression
+gzip compressed data, was "pyedifice-0.5.4.tar", max compression
```

## Comparing `pyedifice-0.5.3.tar` & `pyedifice-0.5.4.tar`

### file list

```diff
@@ -1,1182 +1,1182 @@
--rw-r--r--   0        0        0     1063 2023-08-29 11:20:58.178933 pyedifice-0.5.3/LICENSE
--rw-r--r--   0        0        0     8222 2024-03-10 09:51:30.834464 pyedifice-0.5.3/README.md
--rw-r--r--   0        0        0     6089 2024-04-01 12:22:39.745576 pyedifice-0.5.3/edifice/__init__.py
--rw-r--r--   0        0        0       72 2024-04-11 04:19:58.677589 pyedifice-0.5.3/edifice/__main__.py
--rw-r--r--   0        0        0    15881 2024-04-11 04:19:58.677589 pyedifice-0.5.3/edifice/app.py
--rw-r--r--   0        0        0     2927 2024-04-11 04:19:58.677589 pyedifice-0.5.3/edifice/base_components/__init__.py
--rw-r--r--   0        0        0    69110 2024-04-22 14:03:28.066900 pyedifice-0.5.3/edifice/base_components/base_components.py
--rw-r--r--   0        0        0     4585 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/base_components/button_view.py
--rw-r--r--   0        0        0     6925 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/base_components/flow_view.py
--rw-r--r--   0        0        0     4238 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/base_components/image_aspect.py
--rw-r--r--   0        0        0     6159 2024-04-22 14:03:38.263066 pyedifice-0.5.3/edifice/base_components/spin_input.py
--rw-r--r--   0        0        0    10386 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/base_components/table_grid_view.py
--rw-r--r--   0        0        0    86040 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/engine.py
--rw-r--r--   0        0        0      129 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/extra/__init__.py
--rw-r--r--   0        0        0     3783 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/extra/matplotlib_figure.py
--rw-r--r--   0        0        0     3491 2024-04-11 04:19:58.678589 pyedifice-0.5.3/edifice/extra/pyqtgraph_plot.py
--rw-r--r--   0        0        0    16146 2024-04-11 04:19:58.679589 pyedifice-0.5.3/edifice/hooks.py
--rw-r--r--   0        0        0        0 2023-11-09 12:56:14.685839 pyedifice-0.5.3/edifice/icons/__init__.py
--rw-r--r--   0        0        0     1548 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/LICENSE.txt
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/address-book.svg
--rw-r--r--   0        0        0      895 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/address-card.svg
--rw-r--r--   0        0        0      996 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/angry.svg
--rw-r--r--   0        0        0      565 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-down.svg
--rw-r--r--   0        0        0      559 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-left.svg
--rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-right.svg
--rw-r--r--   0        0        0      565 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-up.svg
--rw-r--r--   0        0        0      971 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/bell-slash.svg
--rw-r--r--   0        0        0      829 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/bell.svg
--rw-r--r--   0        0        0      414 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/bookmark.svg
--rw-r--r--   0        0        0     1057 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/building.svg
--rw-r--r--   0        0        0     1115 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-alt.svg
--rw-r--r--   0        0        0      835 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-check.svg
--rw-r--r--   0        0        0      626 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-minus.svg
--rw-r--r--   0        0        0      730 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-plus.svg
--rw-r--r--   0        0        0      825 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-times.svg
--rw-r--r--   0        0        0      529 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar.svg
--rw-r--r--   0        0        0      570 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-down.svg
--rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-left.svg
--rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-right.svg
--rw-r--r--   0        0        0      567 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-up.svg
--rw-r--r--   0        0        0      928 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/chart-bar.svg
--rw-r--r--   0        0        0      761 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/check-circle.svg
--rw-r--r--   0        0        0      680 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/check-square.svg
--rw-r--r--   0        0        0      412 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/circle.svg
--rw-r--r--   0        0        0      615 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/clipboard.svg
--rw-r--r--   0        0        0      584 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/clock.svg
--rw-r--r--   0        0        0      608 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/clone.svg
--rw-r--r--   0        0        0      920 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/closed-captioning.svg
--rw-r--r--   0        0        0      542 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment-alt.svg
--rw-r--r--   0        0        0      913 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment-dots.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment.svg
--rw-r--r--   0        0        0     1151 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/comments.svg
--rw-r--r--   0        0        0      773 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/compass.svg
--rw-r--r--   0        0        0      768 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/copy.svg
--rw-r--r--   0        0        0      964 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/copyright.svg
--rw-r--r--   0        0        0      699 2023-08-29 11:20:58.179933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/credit-card.svg
--rw-r--r--   0        0        0     1059 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/dizzy.svg
--rw-r--r--   0        0        0      552 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/dot-circle.svg
--rw-r--r--   0        0        0      778 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/edit.svg
--rw-r--r--   0        0        0     1323 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/envelope-open.svg
--rw-r--r--   0        0        0      754 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/envelope.svg
--rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/eye-slash.svg
--rw-r--r--   0        0        0      689 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/eye.svg
--rw-r--r--   0        0        0      690 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-alt.svg
--rw-r--r--   0        0        0      790 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-archive.svg
--rw-r--r--   0        0        0      864 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-audio.svg
--rw-r--r--   0        0        0     1030 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-code.svg
--rw-r--r--   0        0        0      852 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-excel.svg
--rw-r--r--   0        0        0      657 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-image.svg
--rw-r--r--   0        0        0     1058 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-pdf.svg
--rw-r--r--   0        0        0      710 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-powerpoint.svg
--rw-r--r--   0        0        0      764 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-video.svg
--rw-r--r--   0        0        0     1035 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-word.svg
--rw-r--r--   0        0        0      484 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/file.svg
--rw-r--r--   0        0        0      972 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/flag.svg
--rw-r--r--   0        0        0      929 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/flushed.svg
--rw-r--r--   0        0        0      548 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/folder-open.svg
--rw-r--r--   0        0        0      487 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/folder.svg
--rw-r--r--   0        0        0     3174 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/font-awesome-logo-full.svg
--rw-r--r--   0        0        0      721 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/frown-open.svg
--rw-r--r--   0        0        0      778 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/frown.svg
--rw-r--r--   0        0        0      905 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/futbol.svg
--rw-r--r--   0        0        0      626 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/gem.svg
--rw-r--r--   0        0        0      902 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grimace.svg
--rw-r--r--   0        0        0      900 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-alt.svg
--rw-r--r--   0        0        0     1280 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-beam-sweat.svg
--rw-r--r--   0        0        0     1000 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-beam.svg
--rw-r--r--   0        0        0      942 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-hearts.svg
--rw-r--r--   0        0        0     1566 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-squint-tears.svg
--rw-r--r--   0        0        0      950 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-squint.svg
--rw-r--r--   0        0        0     1019 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-stars.svg
--rw-r--r--   0        0        0     1503 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tears.svg
--rw-r--r--   0        0        0     1213 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue-squint.svg
--rw-r--r--   0        0        0     1256 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue-wink.svg
--rw-r--r--   0        0        0      986 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue.svg
--rw-r--r--   0        0        0      901 2023-08-29 11:20:58.180933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-wink.svg
--rw-r--r--   0        0        0      722 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin.svg
--rw-r--r--   0        0        0      955 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-lizard.svg
--rw-r--r--   0        0        0     1167 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-paper.svg
--rw-r--r--   0        0        0     1300 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-peace.svg
--rw-r--r--   0        0        0     1315 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-down.svg
--rw-r--r--   0        0        0     1319 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-left.svg
--rw-r--r--   0        0        0     1326 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-right.svg
--rw-r--r--   0        0        0     1320 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-up.svg
--rw-r--r--   0        0        0     1578 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-pointer.svg
--rw-r--r--   0        0        0     1311 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-rock.svg
--rw-r--r--   0        0        0     1301 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-scissors.svg
--rw-r--r--   0        0        0     1667 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-spock.svg
--rw-r--r--   0        0        0     1313 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/handshake.svg
--rw-r--r--   0        0        0      722 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hdd.svg
--rw-r--r--   0        0        0      670 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/heart.svg
--rw-r--r--   0        0        0     1245 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hospital.svg
--rw-r--r--   0        0        0      727 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/hourglass.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/id-badge.svg
--rw-r--r--   0        0        0      863 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/id-card.svg
--rw-r--r--   0        0        0      671 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/image.svg
--rw-r--r--   0        0        0      824 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/images.svg
--rw-r--r--   0        0        0     1846 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/keyboard.svg
--rw-r--r--   0        0        0     1193 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss-beam.svg
--rw-r--r--   0        0        0     1362 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss-wink-heart.svg
--rw-r--r--   0        0        0      912 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss.svg
--rw-r--r--   0        0        0      975 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-beam.svg
--rw-r--r--   0        0        0      872 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-squint.svg
--rw-r--r--   0        0        0      895 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-wink.svg
--rw-r--r--   0        0        0      775 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh.svg
--rw-r--r--   0        0        0     1144 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/lemon.svg
--rw-r--r--   0        0        0      917 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/life-ring.svg
--rw-r--r--   0        0        0     1036 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/lightbulb.svg
--rw-r--r--   0        0        0     1038 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/list-alt.svg
--rw-r--r--   0        0        0      759 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/map.svg
--rw-r--r--   0        0        0      556 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh-blank.svg
--rw-r--r--   0        0        0     1006 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh-rolling-eyes.svg
--rw-r--r--   0        0        0      644 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh.svg
--rw-r--r--   0        0        0      556 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/minus-square.svg
--rw-r--r--   0        0        0      845 2023-08-29 11:20:58.181933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/money-bill-alt.svg
--rw-r--r--   0        0        0      779 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/moon.svg
--rw-r--r--   0        0        0     1126 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/newspaper.svg
--rw-r--r--   0        0        0     1096 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/object-group.svg
--rw-r--r--   0        0        0     1290 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/object-ungroup.svg
--rw-r--r--   0        0        0      621 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/paper-plane.svg
--rw-r--r--   0        0        0      612 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/pause-circle.svg
--rw-r--r--   0        0        0      524 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/play-circle.svg
--rw-r--r--   0        0        0      660 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/plus-square.svg
--rw-r--r--   0        0        0     1009 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/question-circle.svg
--rw-r--r--   0        0        0      914 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/registered.svg
--rw-r--r--   0        0        0     1043 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/sad-cry.svg
--rw-r--r--   0        0        0      841 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/sad-tear.svg
--rw-r--r--   0        0        0      779 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/save.svg
--rw-r--r--   0        0        0     1181 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/share-square.svg
--rw-r--r--   0        0        0     1055 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile-beam.svg
--rw-r--r--   0        0        0      861 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile-wink.svg
--rw-r--r--   0        0        0      769 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile.svg
--rw-r--r--   0        0        0     1782 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/snowflake.svg
--rw-r--r--   0        0        0      452 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/square.svg
--rw-r--r--   0        0        0      462 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/star-half.svg
--rw-r--r--   0        0        0      628 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/star.svg
--rw-r--r--   0        0        0      523 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/sticky-note.svg
--rw-r--r--   0        0        0      517 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/stop-circle.svg
--rw-r--r--   0        0        0     1132 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/sun.svg
--rw-r--r--   0        0        0      627 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/surprise.svg
--rw-r--r--   0        0        0     1231 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/thumbs-down.svg
--rw-r--r--   0        0        0     1224 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/thumbs-up.svg
--rw-r--r--   0        0        0      728 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/times-circle.svg
--rw-r--r--   0        0        0      950 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/tired.svg
--rw-r--r--   0        0        0      761 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/trash-alt.svg
--rw-r--r--   0        0        0      845 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/user-circle.svg
--rw-r--r--   0        0        0      701 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/user.svg
--rw-r--r--   0        0        0      783 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/window-close.svg
--rw-r--r--   0        0        0      420 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/window-maximize.svg
--rw-r--r--   0        0        0      348 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/window-minimize.svg
--rw-r--r--   0        0        0      498 2023-08-29 11:20:58.182933 pyedifice-0.5.3/edifice/icons/font-awesome/regular/window-restore.svg
--rw-r--r--   0        0        0      960 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ad.svg
--rw-r--r--   0        0        0      773 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/address-book.svg
--rw-r--r--   0        0        0      873 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/address-card.svg
--rw-r--r--   0        0        0      419 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/adjust.svg
--rw-r--r--   0        0        0      823 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/air-freshener.svg
--rw-r--r--   0        0        0      731 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-center.svg
--rw-r--r--   0        0        0      632 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-justify.svg
--rw-r--r--   0        0        0      739 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-left.svg
--rw-r--r--   0        0        0      747 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-right.svg
--rw-r--r--   0        0        0     1185 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/allergies.svg
--rw-r--r--   0        0        0      887 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ambulance.svg
--rw-r--r--   0        0        0     2349 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/american-sign-language-interpreting.svg
--rw-r--r--   0        0        0     1085 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/anchor.svg
--rw-r--r--   0        0        0      634 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-down.svg
--rw-r--r--   0        0        0      636 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-left.svg
--rw-r--r--   0        0        0      638 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-right.svg
--rw-r--r--   0        0        0      637 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-up.svg
--rw-r--r--   0        0        0      450 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-down.svg
--rw-r--r--   0        0        0      448 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-left.svg
--rw-r--r--   0        0        0      449 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-right.svg
--rw-r--r--   0        0        0      449 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-up.svg
--rw-r--r--   0        0        0      947 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/angry.svg
--rw-r--r--   0        0        0      661 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ankh.svg
--rw-r--r--   0        0        0     1056 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/apple-alt.svg
--rw-r--r--   0        0        0      524 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/archive.svg
--rw-r--r--   0        0        0      586 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/archway.svg
--rw-r--r--   0        0        0      500 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-alt-circle-down.svg
--rw-r--r--   0        0        0      501 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-alt-circle-left.svg
--rw-r--r--   0        0        0      495 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-alt-circle-right.svg
--rw-r--r--   0        0        0      495 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-alt-circle-up.svg
--rw-r--r--   0        0        0      584 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-down.svg
--rw-r--r--   0        0        0      581 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-left.svg
--rw-r--r--   0        0        0      582 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-right.svg
--rw-r--r--   0        0        0      577 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-up.svg
--rw-r--r--   0        0        0      508 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-down.svg
--rw-r--r--   0        0        0      508 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-left.svg
--rw-r--r--   0        0        0      513 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-right.svg
--rw-r--r--   0        0        0      511 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-up.svg
--rw-r--r--   0        0        0      595 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt-h.svg
--rw-r--r--   0        0        0      593 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt-v.svg
--rw-r--r--   0        0        0      939 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt.svg
--rw-r--r--   0        0        0     1285 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/assistive-listening-systems.svg
--rw-r--r--   0        0        0      959 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/asterisk.svg
--rw-r--r--   0        0        0     1157 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/at.svg
--rw-r--r--   0        0        0     1117 2023-08-29 11:20:58.183933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/atlas.svg
--rw-r--r--   0        0        0     2056 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/atom.svg
--rw-r--r--   0        0        0     1042 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/audio-description.svg
--rw-r--r--   0        0        0     1702 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/award.svg
--rw-r--r--   0        0        0      835 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/baby-carriage.svg
--rw-r--r--   0        0        0      886 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/baby.svg
--rw-r--r--   0        0        0      835 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/backspace.svg
--rw-r--r--   0        0        0      487 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/backward.svg
--rw-r--r--   0        0        0     1080 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacon.svg
--rw-r--r--   0        0        0     3069 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacteria.svg
--rw-r--r--   0        0        0     1680 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacterium.svg
--rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bahai.svg
--rw-r--r--   0        0        0     1088 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale-left.svg
--rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale-right.svg
--rw-r--r--   0        0        0      984 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale.svg
--rw-r--r--   0        0        0      583 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ban.svg
--rw-r--r--   0        0        0      697 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/band-aid.svg
--rw-r--r--   0        0        0      749 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/barcode.svg
--rw-r--r--   0        0        0      601 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bars.svg
--rw-r--r--   0        0        0      931 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/baseball-ball.svg
--rw-r--r--   0        0        0      950 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/basketball-ball.svg
--rw-r--r--   0        0        0      812 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bath.svg
--rw-r--r--   0        0        0      473 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/battery-empty.svg
--rw-r--r--   0        0        0      496 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/battery-full.svg
--rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/battery-half.svg
--rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/battery-quarter.svg
--rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/battery-three-quarters.svg
--rw-r--r--   0        0        0      563 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bed.svg
--rw-r--r--   0        0        0      769 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/beer.svg
--rw-r--r--   0        0        0      875 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bell-slash.svg
--rw-r--r--   0        0        0      657 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bell.svg
--rw-r--r--   0        0        0     1056 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bezier-curve.svg
--rw-r--r--   0        0        0      733 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bible.svg
--rw-r--r--   0        0        0     1602 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bicycle.svg
--rw-r--r--   0        0        0      702 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/biking.svg
--rw-r--r--   0        0        0      707 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/binoculars.svg
--rw-r--r--   0        0        0     1701 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/biohazard.svg
--rw-r--r--   0        0        0      958 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/birthday-cake.svg
--rw-r--r--   0        0        0     1005 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/blender-phone.svg
--rw-r--r--   0        0        0      751 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/blender.svg
--rw-r--r--   0        0        0     1073 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/blind.svg
--rw-r--r--   0        0        0      879 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/blog.svg
--rw-r--r--   0        0        0      579 2023-08-29 11:20:58.184933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bold.svg
--rw-r--r--   0        0        0      469 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bolt.svg
--rw-r--r--   0        0        0     1102 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bomb.svg
--rw-r--r--   0        0        0      875 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bone.svg
--rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bong.svg
--rw-r--r--   0        0        0     1128 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-dead.svg
--rw-r--r--   0        0        0      652 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-medical.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-open.svg
--rw-r--r--   0        0        0      798 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-reader.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/book.svg
--rw-r--r--   0        0        0      336 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bookmark.svg
--rw-r--r--   0        0        0      429 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/border-all.svg
--rw-r--r--   0        0        0     2202 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/border-none.svg
--rw-r--r--   0        0        0     1027 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/border-style.svg
--rw-r--r--   0        0        0      544 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bowling-ball.svg
--rw-r--r--   0        0        0      761 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/box-open.svg
--rw-r--r--   0        0        0      560 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/box-tissue.svg
--rw-r--r--   0        0        0      486 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/box.svg
--rw-r--r--   0        0        0      642 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/boxes.svg
--rw-r--r--   0        0        0     1238 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/braille.svg
--rw-r--r--   0        0        0      925 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/brain.svg
--rw-r--r--   0        0        0      420 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bread-slice.svg
--rw-r--r--   0        0        0      629 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/briefcase-medical.svg
--rw-r--r--   0        0        0      528 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/briefcase.svg
--rw-r--r--   0        0        0     1660 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/broadcast-tower.svg
--rw-r--r--   0        0        0      727 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/broom.svg
--rw-r--r--   0        0        0      532 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/brush.svg
--rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bug.svg
--rw-r--r--   0        0        0     1144 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/building.svg
--rw-r--r--   0        0        0      916 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bullhorn.svg
--rw-r--r--   0        0        0      624 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bullseye.svg
--rw-r--r--   0        0        0      467 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/burn.svg
--rw-r--r--   0        0        0      987 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bus-alt.svg
--rw-r--r--   0        0        0      870 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/bus.svg
--rw-r--r--   0        0        0      866 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/business-time.svg
--rw-r--r--   0        0        0     1149 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calculator.svg
--rw-r--r--   0        0        0     1084 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-alt.svg
--rw-r--r--   0        0        0      894 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-check.svg
--rw-r--r--   0        0        0      591 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-day.svg
--rw-r--r--   0        0        0      669 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-minus.svg
--rw-r--r--   0        0        0      773 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-plus.svg
--rw-r--r--   0        0        0      882 2023-08-29 11:20:58.185933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-times.svg
--rw-r--r--   0        0        0      592 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-week.svg
--rw-r--r--   0        0        0      572 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar.svg
--rw-r--r--   0        0        0      855 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/camera-retro.svg
--rw-r--r--   0        0        0      602 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/camera.svg
--rw-r--r--   0        0        0      631 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/campground.svg
--rw-r--r--   0        0        0     1093 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/candy-cane.svg
--rw-r--r--   0        0        0     1334 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cannabis.svg
--rw-r--r--   0        0        0      788 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/capsules.svg
--rw-r--r--   0        0        0      918 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-alt.svg
--rw-r--r--   0        0        0      781 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-battery.svg
--rw-r--r--   0        0        0     2160 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-crash.svg
--rw-r--r--   0        0        0      764 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-side.svg
--rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/car.svg
--rw-r--r--   0        0        0      653 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caravan.svg
--rw-r--r--   0        0        0      379 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-down.svg
--rw-r--r--   0        0        0      420 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-left.svg
--rw-r--r--   0        0        0      412 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-right.svg
--rw-r--r--   0        0        0      474 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-down.svg
--rw-r--r--   0        0        0      542 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-left.svg
--rw-r--r--   0        0        0      538 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-right.svg
--rw-r--r--   0        0        0      537 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-up.svg
--rw-r--r--   0        0        0      420 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-up.svg
--rw-r--r--   0        0        0      730 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/carrot.svg
--rw-r--r--   0        0        0     1093 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cart-arrow-down.svg
--rw-r--r--   0        0        0     1110 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cart-plus.svg
--rw-r--r--   0        0        0     1354 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cash-register.svg
--rw-r--r--   0        0        0      818 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cat.svg
--rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/certificate.svg
--rw-r--r--   0        0        0      658 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chair.svg
--rw-r--r--   0        0        0      779 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chalkboard-teacher.svg
--rw-r--r--   0        0        0      463 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chalkboard.svg
--rw-r--r--   0        0        0     1088 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/charging-station.svg
--rw-r--r--   0        0        0      497 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-area.svg
--rw-r--r--   0        0        0      922 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-bar.svg
--rw-r--r--   0        0        0      726 2023-08-29 11:20:58.186933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-line.svg
--rw-r--r--   0        0        0      695 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-pie.svg
--rw-r--r--   0        0        0      616 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-circle.svg
--rw-r--r--   0        0        0      643 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-double.svg
--rw-r--r--   0        0        0      639 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-square.svg
--rw-r--r--   0        0        0      534 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/check.svg
--rw-r--r--   0        0        0      385 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cheese.svg
--rw-r--r--   0        0        0      699 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-bishop.svg
--rw-r--r--   0        0        0      920 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-board.svg
--rw-r--r--   0        0        0      564 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-king.svg
--rw-r--r--   0        0        0      732 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-knight.svg
--rw-r--r--   0        0        0      609 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-pawn.svg
--rw-r--r--   0        0        0      840 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-queen.svg
--rw-r--r--   0        0        0      618 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-rook.svg
--rw-r--r--   0        0        0     1235 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess.svg
--rw-r--r--   0        0        0      521 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-down.svg
--rw-r--r--   0        0        0      521 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-left.svg
--rw-r--r--   0        0        0      518 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-right.svg
--rw-r--r--   0        0        0      516 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-up.svg
--rw-r--r--   0        0        0      539 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-down.svg
--rw-r--r--   0        0        0      498 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-left.svg
--rw-r--r--   0        0        0      541 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-right.svg
--rw-r--r--   0        0        0      544 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-up.svg
--rw-r--r--   0        0        0      705 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/child.svg
--rw-r--r--   0        0        0      762 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/church.svg
--rw-r--r--   0        0        0      728 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/circle-notch.svg
--rw-r--r--   0        0        0      329 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/circle.svg
--rw-r--r--   0        0        0     1713 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/city.svg
--rw-r--r--   0        0        0      770 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clinic-medical.svg
--rw-r--r--   0        0        0      667 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard-check.svg
--rw-r--r--   0        0        0      952 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard-list.svg
--rw-r--r--   0        0        0      577 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard.svg
--rw-r--r--   0        0        0      482 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clock.svg
--rw-r--r--   0        0        0      502 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/clone.svg
--rw-r--r--   0        0        0      834 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/closed-captioning.svg
--rw-r--r--   0        0        0      691 2023-08-29 11:20:58.187933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-download-alt.svg
--rw-r--r--   0        0        0     1255 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-meatball.svg
--rw-r--r--   0        0        0     1350 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-moon-rain.svg
--rw-r--r--   0        0        0      856 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-moon.svg
--rw-r--r--   0        0        0      874 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-rain.svg
--rw-r--r--   0        0        0     1231 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-showers-heavy.svg
--rw-r--r--   0        0        0     1630 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-sun-rain.svg
--rw-r--r--   0        0        0     1045 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-sun.svg
--rw-r--r--   0        0        0      691 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-upload-alt.svg
--rw-r--r--   0        0        0      514 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud.svg
--rw-r--r--   0        0        0      704 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cocktail.svg
--rw-r--r--   0        0        0      935 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/code-branch.svg
--rw-r--r--   0        0        0      800 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/code.svg
--rw-r--r--   0        0        0      496 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/coffee.svg
--rw-r--r--   0        0        0     1070 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cog.svg
--rw-r--r--   0        0        0     2645 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cogs.svg
--rw-r--r--   0        0        0      791 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/coins.svg
--rw-r--r--   0        0        0      420 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/columns.svg
--rw-r--r--   0        0        0      402 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-alt.svg
--rw-r--r--   0        0        0     1187 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-dollar.svg
--rw-r--r--   0        0        0      695 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-dots.svg
--rw-r--r--   0        0        0      628 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-medical.svg
--rw-r--r--   0        0        0      730 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-slash.svg
--rw-r--r--   0        0        0      480 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment.svg
--rw-r--r--   0        0        0     1498 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comments-dollar.svg
--rw-r--r--   0        0        0      759 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/comments.svg
--rw-r--r--   0        0        0      526 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/compact-disc.svg
--rw-r--r--   0        0        0      675 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/compass.svg
--rw-r--r--   0        0        0      775 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress-alt.svg
--rw-r--r--   0        0        0      982 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress-arrows-alt.svg
--rw-r--r--   0        0        0      765 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress.svg
--rw-r--r--   0        0        0      559 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/concierge-bell.svg
--rw-r--r--   0        0        0      931 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cookie-bite.svg
--rw-r--r--   0        0        0      964 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cookie.svg
--rw-r--r--   0        0        0      611 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/copy.svg
--rw-r--r--   0        0        0      833 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/copyright.svg
--rw-r--r--   0        0        0      627 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/couch.svg
--rw-r--r--   0        0        0      583 2023-08-29 11:20:58.188933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/credit-card.svg
--rw-r--r--   0        0        0      576 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crop-alt.svg
--rw-r--r--   0        0        0      670 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crop.svg
--rw-r--r--   0        0        0      496 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cross.svg
--rw-r--r--   0        0        0     1210 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crosshairs.svg
--rw-r--r--   0        0        0      807 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crow.svg
--rw-r--r--   0        0        0      763 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crown.svg
--rw-r--r--   0        0        0      749 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/crutch.svg
--rw-r--r--   0        0        0      554 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cube.svg
--rw-r--r--   0        0        0      867 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cubes.svg
--rw-r--r--   0        0        0      866 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/cut.svg
--rw-r--r--   0        0        0      657 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/database.svg
--rw-r--r--   0        0        0     1179 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/deaf.svg
--rw-r--r--   0        0        0     1493 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/democrat.svg
--rw-r--r--   0        0        0      488 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/desktop.svg
--rw-r--r--   0        0        0     2218 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dharmachakra.svg
--rw-r--r--   0        0        0     1087 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/diagnoses.svg
--rw-r--r--   0        0        0     1186 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-d20.svg
--rw-r--r--   0        0        0      707 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-d6.svg
--rw-r--r--   0        0        0      755 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-five.svg
--rw-r--r--   0        0        0      681 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-four.svg
--rw-r--r--   0        0        0      451 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-one.svg
--rw-r--r--   0        0        0      829 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-six.svg
--rw-r--r--   0        0        0      603 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-three.svg
--rw-r--r--   0        0        0      529 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-two.svg
--rw-r--r--   0        0        0     1151 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice.svg
--rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/digital-tachograph.svg
--rw-r--r--   0        0        0      675 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/directions.svg
--rw-r--r--   0        0        0      846 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/disease.svg
--rw-r--r--   0        0        0      529 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/divide.svg
--rw-r--r--   0        0        0      808 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dizzy.svg
--rw-r--r--   0        0        0     1025 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dna.svg
--rw-r--r--   0        0        0      666 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dog.svg
--rw-r--r--   0        0        0      861 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dollar-sign.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dolly-flatbed.svg
--rw-r--r--   0        0        0      844 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dolly.svg
--rw-r--r--   0        0        0     1195 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/donate.svg
--rw-r--r--   0        0        0      530 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/door-closed.svg
--rw-r--r--   0        0        0      598 2023-08-29 11:20:58.189933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/door-open.svg
--rw-r--r--   0        0        0      431 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dot-circle.svg
--rw-r--r--   0        0        0      778 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dove.svg
--rw-r--r--   0        0        0      702 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/download.svg
--rw-r--r--   0        0        0     1143 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/drafting-compass.svg
--rw-r--r--   0        0        0     1100 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dragon.svg
--rw-r--r--   0        0        0     1273 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/draw-polygon.svg
--rw-r--r--   0        0        0      911 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/drum-steelpan.svg
--rw-r--r--   0        0        0      904 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/drum.svg
--rw-r--r--   0        0        0      680 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/drumstick-bite.svg
--rw-r--r--   0        0        0      790 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumbbell.svg
--rw-r--r--   0        0        0     1164 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumpster-fire.svg
--rw-r--r--   0        0        0      719 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumpster.svg
--rw-r--r--   0        0        0     2102 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/dungeon.svg
--rw-r--r--   0        0        0      767 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/edit.svg
--rw-r--r--   0        0        0      326 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/egg.svg
--rw-r--r--   0        0        0      545 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/eject.svg
--rw-r--r--   0        0        0      477 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ellipsis-h.svg
--rw-r--r--   0        0        0      471 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ellipsis-v.svg
--rw-r--r--   0        0        0     1016 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-open-text.svg
--rw-r--r--   0        0        0     1051 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-open.svg
--rw-r--r--   0        0        0      859 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-square.svg
--rw-r--r--   0        0        0      724 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope.svg
--rw-r--r--   0        0        0      490 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/equals.svg
--rw-r--r--   0        0        0      596 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/eraser.svg
--rw-r--r--   0        0        0      522 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ethernet.svg
--rw-r--r--   0        0        0     1138 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/euro-sign.svg
--rw-r--r--   0        0        0      655 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/exchange-alt.svg
--rw-r--r--   0        0        0      642 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation-circle.svg
--rw-r--r--   0        0        0      708 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation-triangle.svg
--rw-r--r--   0        0        0      527 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation.svg
--rw-r--r--   0        0        0      769 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand-alt.svg
--rw-r--r--   0        0        0      763 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand-arrows-alt.svg
--rw-r--r--   0        0        0      768 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand.svg
--rw-r--r--   0        0        0      603 2023-08-29 11:20:58.190933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/external-link-alt.svg
--rw-r--r--   0        0        0      639 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/external-link-square-alt.svg
--rw-r--r--   0        0        0      681 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye-dropper.svg
--rw-r--r--   0        0        0      995 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye-slash.svg
--rw-r--r--   0        0        0      590 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye.svg
--rw-r--r--   0        0        0      762 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fan.svg
--rw-r--r--   0        0        0      526 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fast-backward.svg
--rw-r--r--   0        0        0      529 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fast-forward.svg
--rw-r--r--   0        0        0      791 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/faucet.svg
--rw-r--r--   0        0        0      919 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fax.svg
--rw-r--r--   0        0        0      659 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/feather-alt.svg
--rw-r--r--   0        0        0      678 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/feather.svg
--rw-r--r--   0        0        0      610 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/female.svg
--rw-r--r--   0        0        0      631 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fighter-jet.svg
--rw-r--r--   0        0        0      737 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-alt.svg
--rw-r--r--   0        0        0      767 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-archive.svg
--rw-r--r--   0        0        0      826 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-audio.svg
--rw-r--r--   0        0        0     1120 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-code.svg
--rw-r--r--   0        0        0     1142 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-contract.svg
--rw-r--r--   0        0        0     1296 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-csv.svg
--rw-r--r--   0        0        0      644 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-download.svg
--rw-r--r--   0        0        0      822 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-excel.svg
--rw-r--r--   0        0        0      626 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-export.svg
--rw-r--r--   0        0        0      718 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-image.svg
--rw-r--r--   0        0        0      630 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-import.svg
--rw-r--r--   0        0        0     1293 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-invoice-dollar.svg
--rw-r--r--   0        0        0      858 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-invoice.svg
--rw-r--r--   0        0        0      677 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-medical-alt.svg
--rw-r--r--   0        0        0      630 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-medical.svg
--rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-pdf.svg
--rw-r--r--   0        0        0      693 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-powerpoint.svg
--rw-r--r--   0        0        0      954 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-prescription.svg
--rw-r--r--   0        0        0     1076 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-signature.svg
--rw-r--r--   0        0        0      647 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-upload.svg
--rw-r--r--   0        0        0      738 2023-08-29 11:20:58.191933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-video.svg
--rw-r--r--   0        0        0      924 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-word.svg
--rw-r--r--   0        0        0      447 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/file.svg
--rw-r--r--   0        0        0      882 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fill-drip.svg
--rw-r--r--   0        0        0      820 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fill.svg
--rw-r--r--   0        0        0     1352 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/film.svg
--rw-r--r--   0        0        0      465 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/filter.svg
--rw-r--r--   0        0        0     2123 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fingerprint.svg
--rw-r--r--   0        0        0      686 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire-alt.svg
--rw-r--r--   0        0        0      888 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire-extinguisher.svg
--rw-r--r--   0        0        0      531 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire.svg
--rw-r--r--   0        0        0      588 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/first-aid.svg
--rw-r--r--   0        0        0      603 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fish.svg
--rw-r--r--   0        0        0     1290 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/fist-raised.svg
--rw-r--r--   0        0        0     1194 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag-checkered.svg
--rw-r--r--   0        0        0     1284 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag-usa.svg
--rw-r--r--   0        0        0      787 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag.svg
--rw-r--r--   0        0        0      558 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/flask.svg
--rw-r--r--   0        0        0      675 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/flushed.svg
--rw-r--r--   0        0        0      496 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder-minus.svg
--rw-r--r--   0        0        0      582 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder-open.svg
--rw-r--r--   0        0        0      563 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder-plus.svg
--rw-r--r--   0        0        0      387 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder.svg
--rw-r--r--   0        0        0     3174 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/font-awesome-logo-full.svg
--rw-r--r--   0        0        0      588 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/font.svg
--rw-r--r--   0        0        0     1247 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/football-ball.svg
--rw-r--r--   0        0        0      480 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/forward.svg
--rw-r--r--   0        0        0      979 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/frog.svg
--rw-r--r--   0        0        0      637 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/frown-open.svg
--rw-r--r--   0        0        0      646 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/frown.svg
--rw-r--r--   0        0        0     1254 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/funnel-dollar.svg
--rw-r--r--   0        0        0      923 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/futbol.svg
--rw-r--r--   0        0        0      608 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gamepad.svg
--rw-r--r--   0        0        0      738 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gas-pump.svg
--rw-r--r--   0        0        0      976 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gavel.svg
--rw-r--r--   0        0        0      532 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gem.svg
--rw-r--r--   0        0        0      412 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/genderless.svg
--rw-r--r--   0        0        0      777 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ghost.svg
--rw-r--r--   0        0        0      758 2023-08-29 11:20:58.192933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gift.svg
--rw-r--r--   0        0        0     1337 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gifts.svg
--rw-r--r--   0        0        0      962 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/glass-cheers.svg
--rw-r--r--   0        0        0      503 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/glass-martini-alt.svg
--rw-r--r--   0        0        0      464 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/glass-martini.svg
--rw-r--r--   0        0        0      439 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/glass-whiskey.svg
--rw-r--r--   0        0        0     1510 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/glasses.svg
--rw-r--r--   0        0        0     1493 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-africa.svg
--rw-r--r--   0        0        0     1652 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-americas.svg
--rw-r--r--   0        0        0     1531 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-asia.svg
--rw-r--r--   0        0        0     1638 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-europe.svg
--rw-r--r--   0        0        0      998 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe.svg
--rw-r--r--   0        0        0      879 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/golf-ball.svg
--rw-r--r--   0        0        0      890 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/gopuram.svg
--rw-r--r--   0        0        0      874 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/graduation-cap.svg
--rw-r--r--   0        0        0      669 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/greater-than-equal.svg
--rw-r--r--   0        0        0      554 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/greater-than.svg
--rw-r--r--   0        0        0      758 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grimace.svg
--rw-r--r--   0        0        0      848 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-alt.svg
--rw-r--r--   0        0        0     1071 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-beam-sweat.svg
--rw-r--r--   0        0        0      849 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-beam.svg
--rw-r--r--   0        0        0      865 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-hearts.svg
--rw-r--r--   0        0        0     1291 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-squint-tears.svg
--rw-r--r--   0        0        0      736 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-squint.svg
--rw-r--r--   0        0        0      931 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-stars.svg
--rw-r--r--   0        0        0     1367 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tears.svg
--rw-r--r--   0        0        0     1027 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue-squint.svg
--rw-r--r--   0        0        0     1082 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue-wink.svg
--rw-r--r--   0        0        0      931 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-wink.svg
--rw-r--r--   0        0        0      641 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin.svg
--rw-r--r--   0        0        0      943 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-horizontal.svg
--rw-r--r--   0        0        0      456 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-lines-vertical.svg
--rw-r--r--   0        0        0      458 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-lines.svg
--rw-r--r--   0        0        0      938 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-vertical.svg
--rw-r--r--   0        0        0      867 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/guitar.svg
--rw-r--r--   0        0        0      614 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/h-square.svg
--rw-r--r--   0        0        0      677 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hamburger.svg
--rw-r--r--   0        0        0      826 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hammer.svg
--rw-r--r--   0        0        0      846 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hamsa.svg
--rw-r--r--   0        0        0      773 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-heart.svg
--rw-r--r--   0        0        0      789 2023-08-29 11:20:58.193933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-medical.svg
--rw-r--r--   0        0        0     1257 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-usd.svg
--rw-r--r--   0        0        0      701 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-water.svg
--rw-r--r--   0        0        0      577 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding.svg
--rw-r--r--   0        0        0      640 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-lizard.svg
--rw-r--r--   0        0        0      717 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-middle-finger.svg
--rw-r--r--   0        0        0      839 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-paper.svg
--rw-r--r--   0        0        0      706 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-peace.svg
--rw-r--r--   0        0        0      988 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-down.svg
--rw-r--r--   0        0        0      992 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-left.svg
--rw-r--r--   0        0        0      995 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-right.svg
--rw-r--r--   0        0        0      990 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-up.svg
--rw-r--r--   0        0        0      737 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-pointer.svg
--rw-r--r--   0        0        0      774 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-rock.svg
--rw-r--r--   0        0        0      711 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-scissors.svg
--rw-r--r--   0        0        0     1461 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-sparkles.svg
--rw-r--r--   0        0        0      968 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-spock.svg
--rw-r--r--   0        0        0      779 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands-helping.svg
--rw-r--r--   0        0        0     1481 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands-wash.svg
--rw-r--r--   0        0        0      958 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands.svg
--rw-r--r--   0        0        0      865 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake-alt-slash.svg
--rw-r--r--   0        0        0      960 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake-slash.svg
--rw-r--r--   0        0        0     1083 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake.svg
--rw-r--r--   0        0        0     1760 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hanukiah.svg
--rw-r--r--   0        0        0      502 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hard-hat.svg
--rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hashtag.svg
--rw-r--r--   0        0        0      681 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-cowboy-side.svg
--rw-r--r--   0        0        0      662 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-cowboy.svg
--rw-r--r--   0        0        0      597 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-wizard.svg
--rw-r--r--   0        0        0      705 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hdd.svg
--rw-r--r--   0        0        0      954 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-cough-slash.svg
--rw-r--r--   0        0        0      803 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-cough.svg
--rw-r--r--   0        0        0      697 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-mask.svg
--rw-r--r--   0        0        0     1111 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-virus.svg
--rw-r--r--   0        0        0      650 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/heading.svg
--rw-r--r--   0        0        0      773 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/headphones-alt.svg
--rw-r--r--   0        0        0      728 2023-08-29 11:20:58.194933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/headphones.svg
--rw-r--r--   0        0        0      832 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/headset.svg
--rw-r--r--   0        0        0      497 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/heart-broken.svg
--rw-r--r--   0        0        0      467 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/heart.svg
--rw-r--r--   0        0        0      666 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/heartbeat.svg
--rw-r--r--   0        0        0      839 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/helicopter.svg
--rw-r--r--   0        0        0      626 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/highlighter.svg
--rw-r--r--   0        0        0     1086 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hiking.svg
--rw-r--r--   0        0        0      831 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hippo.svg
--rw-r--r--   0        0        0      981 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/history.svg
--rw-r--r--   0        0        0      412 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hockey-puck.svg
--rw-r--r--   0        0        0     1392 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/holly-berry.svg
--rw-r--r--   0        0        0      745 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/home.svg
--rw-r--r--   0        0        0      782 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/horse-head.svg
--rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/horse.svg
--rw-r--r--   0        0        0     1194 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-alt.svg
--rw-r--r--   0        0        0      521 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-symbol.svg
--rw-r--r--   0        0        0     1253 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-user.svg
--rw-r--r--   0        0        0     1145 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital.svg
--rw-r--r--   0        0        0     1438 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hot-tub.svg
--rw-r--r--   0        0        0     1229 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hotdog.svg
--rw-r--r--   0        0        0     1373 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hotel.svg
--rw-r--r--   0        0        0      696 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-end.svg
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-half.svg
--rw-r--r--   0        0        0      694 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-start.svg
--rw-r--r--   0        0        0      627 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass.svg
--rw-r--r--   0        0        0      843 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/house-damage.svg
--rw-r--r--   0        0        0      855 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/house-user.svg
--rw-r--r--   0        0        0     1139 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/hryvnia.svg
--rw-r--r--   0        0        0      995 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/i-cursor.svg
--rw-r--r--   0        0        0      390 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ice-cream.svg
--rw-r--r--   0        0        0      502 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/icicles.svg
--rw-r--r--   0        0        0     1308 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/icons.svg
--rw-r--r--   0        0        0      691 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-badge.svg
--rw-r--r--   0        0        0      691 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-card-alt.svg
--rw-r--r--   0        0        0      891 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-card.svg
--rw-r--r--   0        0        0      732 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/igloo.svg
--rw-r--r--   0        0        0      594 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/image.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/images.svg
--rw-r--r--   0        0        0      567 2023-08-29 11:20:58.195933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/inbox.svg
--rw-r--r--   0        0        0      858 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/indent.svg
--rw-r--r--   0        0        0      503 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/industry.svg
--rw-r--r--   0        0        0      671 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/infinity.svg
--rw-r--r--   0        0        0      659 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/info-circle.svg
--rw-r--r--   0        0        0      568 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/info.svg
--rw-r--r--   0        0        0      468 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/italic.svg
--rw-r--r--   0        0        0     2071 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/jedi.svg
--rw-r--r--   0        0        0     1136 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/joint.svg
--rw-r--r--   0        0        0     2235 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/journal-whills.svg
--rw-r--r--   0        0        0     1276 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/kaaba.svg
--rw-r--r--   0        0        0      718 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/key.svg
--rw-r--r--   0        0        0     1742 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/keyboard.svg
--rw-r--r--   0        0        0     1857 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/khanda.svg
--rw-r--r--   0        0        0      977 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss-beam.svg
--rw-r--r--   0        0        0     1184 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss-wink-heart.svg
--rw-r--r--   0        0        0      781 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss.svg
--rw-r--r--   0        0        0     1001 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiwi-bird.svg
--rw-r--r--   0        0        0      662 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/landmark.svg
--rw-r--r--   0        0        0     1246 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/language.svg
--rw-r--r--   0        0        0      992 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-code.svg
--rw-r--r--   0        0        0      966 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-house.svg
--rw-r--r--   0        0        0      684 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-medical.svg
--rw-r--r--   0        0        0      523 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop.svg
--rw-r--r--   0        0        0      789 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-beam.svg
--rw-r--r--   0        0        0      683 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-squint.svg
--rw-r--r--   0        0        0      675 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-wink.svg
--rw-r--r--   0        0        0      586 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh.svg
--rw-r--r--   0        0        0      899 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/layer-group.svg
--rw-r--r--   0        0        0      634 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/leaf.svg
--rw-r--r--   0        0        0      863 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lemon.svg
--rw-r--r--   0        0        0      669 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/less-than-equal.svg
--rw-r--r--   0        0        0      547 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/less-than.svg
--rw-r--r--   0        0        0      543 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/level-down-alt.svg
--rw-r--r--   0        0        0      547 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/level-up-alt.svg
--rw-r--r--   0        0        0      923 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/life-ring.svg
--rw-r--r--   0        0        0      824 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lightbulb.svg
--rw-r--r--   0        0        0     1507 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/link.svg
--rw-r--r--   0        0        0      898 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lira-sign.svg
--rw-r--r--   0        0        0      964 2023-08-29 11:20:58.196933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-alt.svg
--rw-r--r--   0        0        0     1496 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-ol.svg
--rw-r--r--   0        0        0      671 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-ul.svg
--rw-r--r--   0        0        0      818 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/list.svg
--rw-r--r--   0        0        0      418 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/location-arrow.svg
--rw-r--r--   0        0        0      537 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lock-open.svg
--rw-r--r--   0        0        0      472 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lock.svg
--rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/long-arrow-alt-down.svg
--rw-r--r--   0        0        0      487 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/long-arrow-alt-left.svg
--rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/long-arrow-alt-right.svg
--rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/long-arrow-alt-up.svg
--rw-r--r--   0        0        0     1304 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/low-vision.svg
--rw-r--r--   0        0        0      852 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/luggage-cart.svg
--rw-r--r--   0        0        0     1659 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lungs-virus.svg
--rw-r--r--   0        0        0     1050 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/lungs.svg
--rw-r--r--   0        0        0      793 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/magic.svg
--rw-r--r--   0        0        0      690 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/magnet.svg
--rw-r--r--   0        0        0      866 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mail-bulk.svg
--rw-r--r--   0        0        0      563 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/male.svg
--rw-r--r--   0        0        0      905 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marked-alt.svg
--rw-r--r--   0        0        0      834 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marked.svg
--rw-r--r--   0        0        0      504 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marker-alt.svg
--rw-r--r--   0        0        0      421 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marker.svg
--rw-r--r--   0        0        0      592 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-pin.svg
--rw-r--r--   0        0        0      756 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-signs.svg
--rw-r--r--   0        0        0      498 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/map.svg
--rw-r--r--   0        0        0      699 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/marker.svg
--rw-r--r--   0        0        0      994 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-double.svg
--rw-r--r--   0        0        0      767 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke-h.svg
--rw-r--r--   0        0        0      766 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke-v.svg
--rw-r--r--   0        0        0      736 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke.svg
--rw-r--r--   0        0        0      570 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars.svg
--rw-r--r--   0        0        0      846 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mask.svg
--rw-r--r--   0        0        0      947 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/medal.svg
--rw-r--r--   0        0        0      741 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/medkit.svg
--rw-r--r--   0        0        0      473 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/meh-blank.svg
--rw-r--r--   0        0        0      738 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/meh-rolling-eyes.svg
--rw-r--r--   0        0        0      533 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/meh.svg
--rw-r--r--   0        0        0      728 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/memory.svg
--rw-r--r--   0        0        0     1417 2023-08-29 11:20:58.197933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/menorah.svg
--rw-r--r--   0        0        0      910 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mercury.svg
--rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/meteor.svg
--rw-r--r--   0        0        0     1070 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microchip.svg
--rw-r--r--   0        0        0     1100 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-alt-slash.svg
--rw-r--r--   0        0        0      920 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-alt.svg
--rw-r--r--   0        0        0      948 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-slash.svg
--rw-r--r--   0        0        0      723 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone.svg
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/microscope.svg
--rw-r--r--   0        0        0      430 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/minus-circle.svg
--rw-r--r--   0        0        0      464 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/minus-square.svg
--rw-r--r--   0        0        0      376 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/minus.svg
--rw-r--r--   0        0        0      526 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mitten.svg
--rw-r--r--   0        0        0      536 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mobile-alt.svg
--rw-r--r--   0        0        0      436 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mobile.svg
--rw-r--r--   0        0        0      871 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-alt.svg
--rw-r--r--   0        0        0      763 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-wave-alt.svg
--rw-r--r--   0        0        0     1097 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-wave.svg
--rw-r--r--   0        0        0      617 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill.svg
--rw-r--r--   0        0        0     1317 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-check-alt.svg
--rw-r--r--   0        0        0      781 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-check.svg
--rw-r--r--   0        0        0      654 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/monument.svg
--rw-r--r--   0        0        0      563 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/moon.svg
--rw-r--r--   0        0        0      686 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mortar-pestle.svg
--rw-r--r--   0        0        0      867 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mosque.svg
--rw-r--r--   0        0        0     1271 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/motorcycle.svg
--rw-r--r--   0        0        0      521 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mountain.svg
--rw-r--r--   0        0        0      546 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mouse-pointer.svg
--rw-r--r--   0        0        0      400 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mouse.svg
--rw-r--r--   0        0        0      889 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/mug-hot.svg
--rw-r--r--   0        0        0      504 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/music.svg
--rw-r--r--   0        0        0      802 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/network-wired.svg
--rw-r--r--   0        0        0      487 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/neuter.svg
--rw-r--r--   0        0        0     1028 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/newspaper.svg
--rw-r--r--   0        0        0      726 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/not-equal.svg
--rw-r--r--   0        0        0      746 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/notes-medical.svg
--rw-r--r--   0        0        0      859 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/object-group.svg
--rw-r--r--   0        0        0      790 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/object-ungroup.svg
--rw-r--r--   0        0        0      847 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/oil-can.svg
--rw-r--r--   0        0        0     1600 2023-08-29 11:20:58.198933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/om.svg
--rw-r--r--   0        0        0      934 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/otter.svg
--rw-r--r--   0        0        0      857 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/outdent.svg
--rw-r--r--   0        0        0      557 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pager.svg
--rw-r--r--   0        0        0      705 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paint-brush.svg
--rw-r--r--   0        0        0      599 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paint-roller.svg
--rw-r--r--   0        0        0      741 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/palette.svg
--rw-r--r--   0        0        0      634 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pallet.svg
--rw-r--r--   0        0        0      473 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paper-plane.svg
--rw-r--r--   0        0        0     1046 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paperclip.svg
--rw-r--r--   0        0        0      694 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/parachute-box.svg
--rw-r--r--   0        0        0      438 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paragraph.svg
--rw-r--r--   0        0        0      539 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/parking.svg
--rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/passport.svg
--rw-r--r--   0        0        0     2295 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pastafarianism.svg
--rw-r--r--   0        0        0      762 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paste.svg
--rw-r--r--   0        0        0      529 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pause-circle.svg
--rw-r--r--   0        0        0      474 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pause.svg
--rw-r--r--   0        0        0     1047 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/paw.svg
--rw-r--r--   0        0        0      654 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/peace.svg
--rw-r--r--   0        0        0      705 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-alt.svg
--rw-r--r--   0        0        0      635 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-fancy.svg
--rw-r--r--   0        0        0      673 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-nib.svg
--rw-r--r--   0        0        0      649 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-square.svg
--rw-r--r--   0        0        0      504 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen.svg
--rw-r--r--   0        0        0      725 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pencil-alt.svg
--rw-r--r--   0        0        0      960 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pencil-ruler.svg
--rw-r--r--   0        0        0     1020 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/people-arrows.svg
--rw-r--r--   0        0        0     1408 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/people-carry.svg
--rw-r--r--   0        0        0      682 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pepper-hot.svg
--rw-r--r--   0        0        0      718 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/percent.svg
--rw-r--r--   0        0        0      714 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/percentage.svg
--rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/person-booth.svg
--rw-r--r--   0        0        0      524 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-alt.svg
--rw-r--r--   0        0        0      774 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-slash.svg
--rw-r--r--   0        0        0      720 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-square-alt.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-square.svg
--rw-r--r--   0        0        0     1425 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-volume.svg
--rw-r--r--   0        0        0      541 2023-08-29 11:20:58.199933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone.svg
--rw-r--r--   0        0        0      830 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/photo-video.svg
--rw-r--r--   0        0        0      940 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/piggy-bank.svg
--rw-r--r--   0        0        0      682 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pills.svg
--rw-r--r--   0        0        0      672 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pizza-slice.svg
--rw-r--r--   0        0        0      702 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/place-of-worship.svg
--rw-r--r--   0        0        0      825 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-arrival.svg
--rw-r--r--   0        0        0      833 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-departure.svg
--rw-r--r--   0        0        0      770 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-slash.svg
--rw-r--r--   0        0        0      673 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane.svg
--rw-r--r--   0        0        0      437 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/play-circle.svg
--rw-r--r--   0        0        0      371 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/play.svg
--rw-r--r--   0        0        0      498 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plug.svg
--rw-r--r--   0        0        0      534 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plus-circle.svg
--rw-r--r--   0        0        0      569 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plus-square.svg
--rw-r--r--   0        0        0      499 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/plus.svg
--rw-r--r--   0        0        0     1573 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/podcast.svg
--rw-r--r--   0        0        0      686 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/poll-h.svg
--rw-r--r--   0        0        0      685 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/poll.svg
--rw-r--r--   0        0        0      947 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/poo-storm.svg
--rw-r--r--   0        0        0      939 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/poo.svg
--rw-r--r--   0        0        0      759 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/poop.svg
--rw-r--r--   0        0        0      611 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/portrait.svg
--rw-r--r--   0        0        0      784 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pound-sign.svg
--rw-r--r--   0        0        0      723 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/power-off.svg
--rw-r--r--   0        0        0      730 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pray.svg
--rw-r--r--   0        0        0     1121 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/praying-hands.svg
--rw-r--r--   0        0        0      607 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription-bottle-alt.svg
--rw-r--r--   0        0        0      561 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription-bottle.svg
--rw-r--r--   0        0        0      768 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription.svg
--rw-r--r--   0        0        0      697 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/print.svg
--rw-r--r--   0        0        0      776 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/procedures.svg
--rw-r--r--   0        0        0      659 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/project-diagram.svg
--rw-r--r--   0        0        0      883 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pump-medical.svg
--rw-r--r--   0        0        0      709 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/pump-soap.svg
--rw-r--r--   0        0        0      904 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/puzzle-piece.svg
--rw-r--r--   0        0        0      479 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/qrcode.svg
--rw-r--r--   0        0        0      882 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/question-circle.svg
--rw-r--r--   0        0        0      840 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/question.svg
--rw-r--r--   0        0        0      763 2023-08-29 11:20:58.200933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/quidditch.svg
--rw-r--r--   0        0        0      631 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/quote-left.svg
--rw-r--r--   0        0        0      627 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/quote-right.svg
--rw-r--r--   0        0        0     1185 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/quran.svg
--rw-r--r--   0        0        0      925 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/radiation-alt.svg
--rw-r--r--   0        0        0      804 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/radiation.svg
--rw-r--r--   0        0        0      917 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/rainbow.svg
--rw-r--r--   0        0        0      932 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/random.svg
--rw-r--r--   0        0        0      824 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/receipt.svg
--rw-r--r--   0        0        0      476 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/record-vinyl.svg
--rw-r--r--   0        0        0     1390 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/recycle.svg
--rw-r--r--   0        0        0      805 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/redo-alt.svg
--rw-r--r--   0        0        0      602 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/redo.svg
--rw-r--r--   0        0        0      802 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/registered.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/remove-format.svg
--rw-r--r--   0        0        0      848 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/reply-all.svg
--rw-r--r--   0        0        0      581 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/reply.svg
--rw-r--r--   0        0        0     1257 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/republican.svg
--rw-r--r--   0        0        0      987 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/restroom.svg
--rw-r--r--   0        0        0     1075 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/retweet.svg
--rw-r--r--   0        0        0      718 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ribbon.svg
--rw-r--r--   0        0        0      687 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ring.svg
--rw-r--r--   0        0        0      949 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/road.svg
--rw-r--r--   0        0        0      756 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/robot.svg
--rw-r--r--   0        0        0     1033 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/rocket.svg
--rw-r--r--   0        0        0      735 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/route.svg
--rw-r--r--   0        0        0      968 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/rss-square.svg
--rw-r--r--   0        0        0      903 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/rss.svg
--rw-r--r--   0        0        0      711 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruble-sign.svg
--rw-r--r--   0        0        0      776 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-combined.svg
--rw-r--r--   0        0        0      636 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-horizontal.svg
--rw-r--r--   0        0        0      581 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-vertical.svg
--rw-r--r--   0        0        0      864 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler.svg
--rw-r--r--   0        0        0     1067 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/running.svg
--rw-r--r--   0        0        0      832 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/rupee-sign.svg
--rw-r--r--   0        0        0      955 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sad-cry.svg
--rw-r--r--   0        0        0      719 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sad-tear.svg
--rw-r--r--   0        0        0     1281 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/satellite-dish.svg
--rw-r--r--   0        0        0     1245 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/satellite.svg
--rw-r--r--   0        0        0      701 2023-08-29 11:20:58.201933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/save.svg
--rw-r--r--   0        0        0      787 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/school.svg
--rw-r--r--   0        0        0      550 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/screwdriver.svg
--rw-r--r--   0        0        0      581 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/scroll.svg
--rw-r--r--   0        0        0      411 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sd-card.svg
--rw-r--r--   0        0        0     1349 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-dollar.svg
--rw-r--r--   0        0        0      943 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-location.svg
--rw-r--r--   0        0        0      685 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-minus.svg
--rw-r--r--   0        0        0      789 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-plus.svg
--rw-r--r--   0        0        0      605 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/search.svg
--rw-r--r--   0        0        0      468 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/seedling.svg
--rw-r--r--   0        0        0     1120 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/server.svg
--rw-r--r--   0        0        0      552 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shapes.svg
--rw-r--r--   0        0        0      851 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-alt-square.svg
--rw-r--r--   0        0        0      716 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-alt.svg
--rw-r--r--   0        0        0      919 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-square.svg
--rw-r--r--   0        0        0      577 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/share.svg
--rw-r--r--   0        0        0      650 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shekel-sign.svg
--rw-r--r--   0        0        0      519 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shield-alt.svg
--rw-r--r--   0        0        0     1145 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shield-virus.svg
--rw-r--r--   0        0        0      957 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ship.svg
--rw-r--r--   0        0        0      921 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shipping-fast.svg
--rw-r--r--   0        0        0      799 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shoe-prints.svg
--rw-r--r--   0        0        0      618 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-bag.svg
--rw-r--r--   0        0        0     1022 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-basket.svg
--rw-r--r--   0        0        0      796 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-cart.svg
--rw-r--r--   0        0        0     1396 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shower.svg
--rw-r--r--   0        0        0      739 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/shuttle-van.svg
--rw-r--r--   0        0        0      596 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-in-alt.svg
--rw-r--r--   0        0        0     1687 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-language.svg
--rw-r--r--   0        0        0      600 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-out-alt.svg
--rw-r--r--   0        0        0      486 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign.svg
--rw-r--r--   0        0        0      798 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/signal.svg
--rw-r--r--   0        0        0      822 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/signature.svg
--rw-r--r--   0        0        0      579 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sim-card.svg
--rw-r--r--   0        0        0      698 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sink.svg
--rw-r--r--   0        0        0      842 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sitemap.svg
--rw-r--r--   0        0        0     1066 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/skating.svg
--rw-r--r--   0        0        0     1019 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/skiing-nordic.svg
--rw-r--r--   0        0        0     1010 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/skiing.svg
--rw-r--r--   0        0        0     1034 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/skull-crossbones.svg
--rw-r--r--   0        0        0      738 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/skull.svg
--rw-r--r--   0        0        0      451 2023-08-29 11:20:58.202933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/slash.svg
--rw-r--r--   0        0        0      747 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sleigh.svg
--rw-r--r--   0        0        0      869 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sliders-h.svg
--rw-r--r--   0        0        0      846 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile-beam.svg
--rw-r--r--   0        0        0      729 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile-wink.svg
--rw-r--r--   0        0        0      646 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile.svg
--rw-r--r--   0        0        0      793 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smog.svg
--rw-r--r--   0        0        0      918 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smoking-ban.svg
--rw-r--r--   0        0        0      988 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/smoking.svg
--rw-r--r--   0        0        0     1379 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sms.svg
--rw-r--r--   0        0        0     1183 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowboarding.svg
--rw-r--r--   0        0        0     1737 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowflake.svg
--rw-r--r--   0        0        0     1383 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowman.svg
--rw-r--r--   0        0        0     1209 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowplow.svg
--rw-r--r--   0        0        0      649 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/soap.svg
--rw-r--r--   0        0        0      800 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/socks.svg
--rw-r--r--   0        0        0      934 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/solar-panel.svg
--rw-r--r--   0        0        0      882 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-down-alt.svg
--rw-r--r--   0        0        0      879 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-down.svg
--rw-r--r--   0        0        0      877 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-up-alt.svg
--rw-r--r--   0        0        0      876 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-up.svg
--rw-r--r--   0        0        0      797 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-down-alt.svg
--rw-r--r--   0        0        0      801 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-down.svg
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-up-alt.svg
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-up.svg
--rw-r--r--   0        0        0      359 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-down.svg
--rw-r--r--   0        0        0      889 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-down-alt.svg
--rw-r--r--   0        0        0      886 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-down.svg
--rw-r--r--   0        0        0      885 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-up-alt.svg
--rw-r--r--   0        0        0      883 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-up.svg
--rw-r--r--   0        0        0      360 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-up.svg
--rw-r--r--   0        0        0      458 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort.svg
--rw-r--r--   0        0        0      844 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/spa.svg
--rw-r--r--   0        0        0      840 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/space-shuttle.svg
--rw-r--r--   0        0        0      928 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/spell-check.svg
--rw-r--r--   0        0        0     1718 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/spider.svg
--rw-r--r--   0        0        0      838 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/spinner.svg
--rw-r--r--   0        0        0      745 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/splotch.svg
--rw-r--r--   0        0        0      984 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/spray-can.svg
--rw-r--r--   0        0        0      281 2023-08-29 11:20:58.203933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/square-full.svg
--rw-r--r--   0        0        0      953 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/square-root-alt.svg
--rw-r--r--   0        0        0      365 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/square.svg
--rw-r--r--   0        0        0      672 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stamp.svg
--rw-r--r--   0        0        0      973 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-and-crescent.svg
--rw-r--r--   0        0        0      802 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-half-alt.svg
--rw-r--r--   0        0        0      402 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-half.svg
--rw-r--r--   0        0        0      912 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-of-david.svg
--rw-r--r--   0        0        0      820 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-of-life.svg
--rw-r--r--   0        0        0      516 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/star.svg
--rw-r--r--   0        0        0      442 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/step-backward.svg
--rw-r--r--   0        0        0      443 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/step-forward.svg
--rw-r--r--   0        0        0      888 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stethoscope.svg
--rw-r--r--   0        0        0      447 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sticky-note.svg
--rw-r--r--   0        0        0      430 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stop-circle.svg
--rw-r--r--   0        0        0      365 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stop.svg
--rw-r--r--   0        0        0     1328 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stopwatch-20.svg
--rw-r--r--   0        0        0      682 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stopwatch.svg
--rw-r--r--   0        0        0      705 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-alt-slash.svg
--rw-r--r--   0        0        0      554 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-alt.svg
--rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-slash.svg
--rw-r--r--   0        0        0      825 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/store.svg
--rw-r--r--   0        0        0      580 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stream.svg
--rw-r--r--   0        0        0      852 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/street-view.svg
--rw-r--r--   0        0        0      848 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/strikethrough.svg
--rw-r--r--   0        0        0     2664 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/stroopwafel.svg
--rw-r--r--   0        0        0      800 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/subscript.svg
--rw-r--r--   0        0        0      880 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/subway.svg
--rw-r--r--   0        0        0      756 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/suitcase-rolling.svg
--rw-r--r--   0        0        0      479 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/suitcase.svg
--rw-r--r--   0        0        0      847 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sun.svg
--rw-r--r--   0        0        0      798 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/superscript.svg
--rw-r--r--   0        0        0      546 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/surprise.svg
--rw-r--r--   0        0        0      631 2023-08-29 11:20:58.204933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/swatchbook.svg
--rw-r--r--   0        0        0     1494 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/swimmer.svg
--rw-r--r--   0        0        0     1345 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/swimming-pool.svg
--rw-r--r--   0        0        0      966 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/synagogue.svg
--rw-r--r--   0        0        0     1022 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sync-alt.svg
--rw-r--r--   0        0        0      887 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/sync.svg
--rw-r--r--   0        0        0      970 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/syringe.svg
--rw-r--r--   0        0        0      674 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/table-tennis.svg
--rw-r--r--   0        0        0      463 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/table.svg
--rw-r--r--   0        0        0      536 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tablet-alt.svg
--rw-r--r--   0        0        0      436 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tablet.svg
--rw-r--r--   0        0        0      746 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tablets.svg
--rw-r--r--   0        0        0     1197 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tachometer-alt.svg
--rw-r--r--   0        0        0      550 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tag.svg
--rw-r--r--   0        0        0      810 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tags.svg
--rw-r--r--   0        0        0      544 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tape.svg
--rw-r--r--   0        0        0      966 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tasks.svg
--rw-r--r--   0        0        0      923 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/taxi.svg
--rw-r--r--   0        0        0     1275 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/teeth-open.svg
--rw-r--r--   0        0        0     1166 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/teeth.svg
--rw-r--r--   0        0        0      833 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/temperature-high.svg
--rw-r--r--   0        0        0      832 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/temperature-low.svg
--rw-r--r--   0        0        0      509 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tenge.svg
--rw-r--r--   0        0        0      661 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/terminal.svg
--rw-r--r--   0        0        0      723 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/text-height.svg
--rw-r--r--   0        0        0      723 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/text-width.svg
--rw-r--r--   0        0        0      753 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/th-large.svg
--rw-r--r--   0        0        0     1030 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/th-list.svg
--rw-r--r--   0        0        0     1455 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/th.svg
--rw-r--r--   0        0        0     1803 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/theater-masks.svg
--rw-r--r--   0        0        0      786 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-empty.svg
--rw-r--r--   0        0        0      860 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-full.svg
--rw-r--r--   0        0        0      865 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-half.svg
--rw-r--r--   0        0        0      864 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-quarter.svg
--rw-r--r--   0        0        0      873 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-three-quarters.svg
--rw-r--r--   0        0        0      688 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer.svg
--rw-r--r--   0        0        0     1059 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbs-down.svg
--rw-r--r--   0        0        0     1066 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbs-up.svg
--rw-r--r--   0        0        0      666 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbtack.svg
--rw-r--r--   0        0        0      619 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/ticket-alt.svg
--rw-r--r--   0        0        0      635 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/times-circle.svg
--rw-r--r--   0        0        0      675 2023-08-29 11:20:58.205933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/times.svg
--rw-r--r--   0        0        0      720 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tint-slash.svg
--rw-r--r--   0        0        0      552 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tint.svg
--rw-r--r--   0        0        0      740 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tired.svg
--rw-r--r--   0        0        0      598 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toggle-off.svg
--rw-r--r--   0        0        0      448 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toggle-on.svg
--rw-r--r--   0        0        0      851 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet-paper-slash.svg
--rw-r--r--   0        0        0      907 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet-paper.svg
--rw-r--r--   0        0        0      730 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet.svg
--rw-r--r--   0        0        0      813 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/toolbox.svg
--rw-r--r--   0        0        0      951 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tools.svg
--rw-r--r--   0        0        0      971 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tooth.svg
--rw-r--r--   0        0        0     1122 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/torah.svg
--rw-r--r--   0        0        0      656 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/torii-gate.svg
--rw-r--r--   0        0        0     1466 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tractor.svg
--rw-r--r--   0        0        0      914 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trademark.svg
--rw-r--r--   0        0        0      829 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/traffic-light.svg
--rw-r--r--   0        0        0      863 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trailer.svg
--rw-r--r--   0        0        0      685 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/train.svg
--rw-r--r--   0        0        0      752 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tram.svg
--rw-r--r--   0        0        0     1055 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/transgender-alt.svg
--rw-r--r--   0        0        0      745 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/transgender.svg
--rw-r--r--   0        0        0      619 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-alt.svg
--rw-r--r--   0        0        0      668 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-restore-alt.svg
--rw-r--r--   0        0        0      680 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-restore.svg
--rw-r--r--   0        0        0      494 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash.svg
--rw-r--r--   0        0        0      885 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tree.svg
--rw-r--r--   0        0        0      840 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/trophy.svg
--rw-r--r--   0        0        0      714 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-loading.svg
--rw-r--r--   0        0        0     2510 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-monster.svg
--rw-r--r--   0        0        0      892 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-moving.svg
--rw-r--r--   0        0        0      899 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-pickup.svg
--rw-r--r--   0        0        0      704 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck.svg
--rw-r--r--   0        0        0      580 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tshirt.svg
--rw-r--r--   0        0        0     2005 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tty.svg
--rw-r--r--   0        0        0      473 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/tv.svg
--rw-r--r--   0        0        0      849 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/umbrella-beach.svg
--rw-r--r--   0        0        0      819 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/umbrella.svg
--rw-r--r--   0        0        0      613 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/underline.svg
--rw-r--r--   0        0        0      804 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/undo-alt.svg
--rw-r--r--   0        0        0      799 2023-08-29 11:20:58.206933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/undo.svg
--rw-r--r--   0        0        0     1249 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/universal-access.svg
--rw-r--r--   0        0        0      666 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/university.svg
--rw-r--r--   0        0        0     1254 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlink.svg
--rw-r--r--   0        0        0      622 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlock-alt.svg
--rw-r--r--   0        0        0      535 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlock.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/upload.svg
--rw-r--r--   0        0        0      584 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-alt-slash.svg
--rw-r--r--   0        0        0      504 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-alt.svg
--rw-r--r--   0        0        0      967 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-astronaut.svg
--rw-r--r--   0        0        0      718 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-check.svg
--rw-r--r--   0        0        0      614 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-circle.svg
--rw-r--r--   0        0        0      778 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-clock.svg
--rw-r--r--   0        0        0     1562 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-cog.svg
--rw-r--r--   0        0        0      752 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-edit.svg
--rw-r--r--   0        0        0      763 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-friends.svg
--rw-r--r--   0        0        0      799 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-graduate.svg
--rw-r--r--   0        0        0      938 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-injured.svg
--rw-r--r--   0        0        0      695 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-lock.svg
--rw-r--r--   0        0        0     1037 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-md.svg
--rw-r--r--   0        0        0      617 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-minus.svg
--rw-r--r--   0        0        0      665 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-ninja.svg
--rw-r--r--   0        0        0      785 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-nurse.svg
--rw-r--r--   0        0        0      721 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-plus.svg
--rw-r--r--   0        0        0     1094 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-secret.svg
--rw-r--r--   0        0        0      800 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-shield.svg
--rw-r--r--   0        0        0      583 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-slash.svg
--rw-r--r--   0        0        0      848 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-tag.svg
--rw-r--r--   0        0        0      511 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-tie.svg
--rw-r--r--   0        0        0      846 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-times.svg
--rw-r--r--   0        0        0      516 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/user.svg
--rw-r--r--   0        0        0     1816 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/users-cog.svg
--rw-r--r--   0        0        0     1042 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/users-slash.svg
--rw-r--r--   0        0        0      904 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/users.svg
--rw-r--r--   0        0        0      477 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/utensil-spoon.svg
--rw-r--r--   0        0        0      764 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/utensils.svg
--rw-r--r--   0        0        0      812 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vector-square.svg
--rw-r--r--   0        0        0     1005 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus-double.svg
--rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus-mars.svg
--rw-r--r--   0        0        0      589 2023-08-29 11:20:58.207933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus.svg
--rw-r--r--   0        0        0     1201 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vest-patches.svg
--rw-r--r--   0        0        0      908 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vest.svg
--rw-r--r--   0        0        0      556 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vial.svg
--rw-r--r--   0        0        0      656 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vials.svg
--rw-r--r--   0        0        0      635 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/video-slash.svg
--rw-r--r--   0        0        0      496 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/video.svg
--rw-r--r--   0        0        0      861 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vihara.svg
--rw-r--r--   0        0        0     1234 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/virus-slash.svg
--rw-r--r--   0        0        0      982 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/virus.svg
--rw-r--r--   0        0        0     1608 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/viruses.svg
--rw-r--r--   0        0        0      435 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/voicemail.svg
--rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/volleyball-ball.svg
--rw-r--r--   0        0        0      697 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-down.svg
--rw-r--r--   0        0        0      799 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-mute.svg
--rw-r--r--   0        0        0      376 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-off.svg
--rw-r--r--   0        0        0     1238 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-up.svg
--rw-r--r--   0        0        0      743 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vote-yea.svg
--rw-r--r--   0        0        0      682 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/vr-cardboard.svg
--rw-r--r--   0        0        0     1041 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/walking.svg
--rw-r--r--   0        0        0      550 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wallet.svg
--rw-r--r--   0        0        0      789 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/warehouse.svg
--rw-r--r--   0        0        0     1517 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/water.svg
--rw-r--r--   0        0        0      508 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wave-square.svg
--rw-r--r--   0        0        0      627 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/weight-hanging.svg
--rw-r--r--   0        0        0      769 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/weight.svg
--rw-r--r--   0        0        0     1033 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wheelchair.svg
--rw-r--r--   0        0        0      795 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wifi.svg
--rw-r--r--   0        0        0     1086 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wind.svg
--rw-r--r--   0        0        0      697 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-close.svg
--rw-r--r--   0        0        0      426 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-maximize.svg
--rw-r--r--   0        0        0      368 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-minimize.svg
--rw-r--r--   0        0        0      545 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-restore.svg
--rw-r--r--   0        0        0      702 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-bottle.svg
--rw-r--r--   0        0        0      575 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-glass-alt.svg
--rw-r--r--   0        0        0      537 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-glass.svg
--rw-r--r--   0        0        0     1152 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/won-sign.svg
--rw-r--r--   0        0        0      713 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/wrench.svg
--rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/x-ray.svg
--rw-r--r--   0        0        0      762 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/yen-sign.svg
--rw-r--r--   0        0        0      626 2023-08-29 11:20:58.208933 pyedifice-0.5.3/edifice/icons/font-awesome/solid/yin-yang.svg
--rw-r--r--   0        0        0        0 2023-08-29 11:20:58.209933 pyedifice-0.5.3/edifice/inspector/__init__.py
--rw-r--r--   0        0        0     2304 2023-08-29 11:20:58.209933 pyedifice-0.5.3/edifice/inspector/icon.png
--rw-r--r--   0        0        0     7234 2024-04-11 04:19:58.679589 pyedifice-0.5.3/edifice/inspector/inspector.py
--rw-r--r--   0        0        0     1743 2024-04-11 04:19:58.679589 pyedifice-0.5.3/edifice/logger.py
--rw-r--r--   0        0        0       72 2023-09-12 12:13:41.458375 pyedifice-0.5.3/edifice/qt/__init__.py
--rw-r--r--   0        0        0     6806 2024-04-11 04:19:58.679589 pyedifice-0.5.3/edifice/runner.py
--rw-r--r--   0        0        0     2565 2024-04-11 04:19:58.679589 pyedifice-0.5.3/edifice/utilities.py
--rw-r--r--   0        0        0     1593 2024-04-22 14:06:35.876965 pyedifice-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     8863 1970-01-01 00:00:00.000000 pyedifice-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-29 11:20:58.178933 pyedifice-0.5.4/LICENSE
+-rw-r--r--   0        0        0     8222 2024-03-10 09:51:30.834464 pyedifice-0.5.4/README.md
+-rw-r--r--   0        0        0     6089 2024-04-01 12:22:39.745576 pyedifice-0.5.4/edifice/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-11 04:19:58.677589 pyedifice-0.5.4/edifice/__main__.py
+-rw-r--r--   0        0        0    15881 2024-04-11 04:19:58.677589 pyedifice-0.5.4/edifice/app.py
+-rw-r--r--   0        0        0     2927 2024-04-11 04:19:58.677589 pyedifice-0.5.4/edifice/base_components/__init__.py
+-rw-r--r--   0        0        0    69408 2024-04-29 06:57:52.107400 pyedifice-0.5.4/edifice/base_components/base_components.py
+-rw-r--r--   0        0        0     4582 2024-04-25 14:52:26.045029 pyedifice-0.5.4/edifice/base_components/button_view.py
+-rw-r--r--   0        0        0     6925 2024-04-11 04:19:58.678589 pyedifice-0.5.4/edifice/base_components/flow_view.py
+-rw-r--r--   0        0        0     4235 2024-04-25 14:52:26.046029 pyedifice-0.5.4/edifice/base_components/image_aspect.py
+-rw-r--r--   0        0        0     6153 2024-04-25 14:52:26.046029 pyedifice-0.5.4/edifice/base_components/spin_input.py
+-rw-r--r--   0        0        0    10376 2024-04-25 14:52:26.046029 pyedifice-0.5.4/edifice/base_components/table_grid_view.py
+-rw-r--r--   0        0        0    87174 2024-04-25 14:52:26.047029 pyedifice-0.5.4/edifice/engine.py
+-rw-r--r--   0        0        0      129 2024-04-11 04:19:58.678589 pyedifice-0.5.4/edifice/extra/__init__.py
+-rw-r--r--   0        0        0     3780 2024-04-25 14:52:26.047029 pyedifice-0.5.4/edifice/extra/matplotlib_figure.py
+-rw-r--r--   0        0        0     3489 2024-04-25 14:52:26.047029 pyedifice-0.5.4/edifice/extra/pyqtgraph_plot.py
+-rw-r--r--   0        0        0    16146 2024-04-11 04:19:58.679589 pyedifice-0.5.4/edifice/hooks.py
+-rw-r--r--   0        0        0        0 2023-11-09 12:56:14.685839 pyedifice-0.5.4/edifice/icons/__init__.py
+-rw-r--r--   0        0        0     1548 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/LICENSE.txt
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/address-book.svg
+-rw-r--r--   0        0        0      895 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/address-card.svg
+-rw-r--r--   0        0        0      996 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/angry.svg
+-rw-r--r--   0        0        0      565 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-down.svg
+-rw-r--r--   0        0        0      559 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-left.svg
+-rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-right.svg
+-rw-r--r--   0        0        0      565 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-up.svg
+-rw-r--r--   0        0        0      971 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/bell-slash.svg
+-rw-r--r--   0        0        0      829 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/bell.svg
+-rw-r--r--   0        0        0      414 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/bookmark.svg
+-rw-r--r--   0        0        0     1057 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/building.svg
+-rw-r--r--   0        0        0     1115 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-alt.svg
+-rw-r--r--   0        0        0      835 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-check.svg
+-rw-r--r--   0        0        0      626 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-minus.svg
+-rw-r--r--   0        0        0      730 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-plus.svg
+-rw-r--r--   0        0        0      825 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-times.svg
+-rw-r--r--   0        0        0      529 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar.svg
+-rw-r--r--   0        0        0      570 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-down.svg
+-rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-left.svg
+-rw-r--r--   0        0        0      568 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-right.svg
+-rw-r--r--   0        0        0      567 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-up.svg
+-rw-r--r--   0        0        0      928 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/chart-bar.svg
+-rw-r--r--   0        0        0      761 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/check-circle.svg
+-rw-r--r--   0        0        0      680 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/check-square.svg
+-rw-r--r--   0        0        0      412 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/circle.svg
+-rw-r--r--   0        0        0      615 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/clipboard.svg
+-rw-r--r--   0        0        0      584 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/clock.svg
+-rw-r--r--   0        0        0      608 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/clone.svg
+-rw-r--r--   0        0        0      920 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/closed-captioning.svg
+-rw-r--r--   0        0        0      542 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment-alt.svg
+-rw-r--r--   0        0        0      913 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment-dots.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment.svg
+-rw-r--r--   0        0        0     1151 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/comments.svg
+-rw-r--r--   0        0        0      773 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/compass.svg
+-rw-r--r--   0        0        0      768 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/copy.svg
+-rw-r--r--   0        0        0      964 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/copyright.svg
+-rw-r--r--   0        0        0      699 2023-08-29 11:20:58.179933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/credit-card.svg
+-rw-r--r--   0        0        0     1059 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/dizzy.svg
+-rw-r--r--   0        0        0      552 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/dot-circle.svg
+-rw-r--r--   0        0        0      778 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/edit.svg
+-rw-r--r--   0        0        0     1323 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/envelope-open.svg
+-rw-r--r--   0        0        0      754 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/envelope.svg
+-rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/eye-slash.svg
+-rw-r--r--   0        0        0      689 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/eye.svg
+-rw-r--r--   0        0        0      690 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-alt.svg
+-rw-r--r--   0        0        0      790 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-archive.svg
+-rw-r--r--   0        0        0      864 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-audio.svg
+-rw-r--r--   0        0        0     1030 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-code.svg
+-rw-r--r--   0        0        0      852 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-excel.svg
+-rw-r--r--   0        0        0      657 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-image.svg
+-rw-r--r--   0        0        0     1058 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-pdf.svg
+-rw-r--r--   0        0        0      710 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-powerpoint.svg
+-rw-r--r--   0        0        0      764 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-video.svg
+-rw-r--r--   0        0        0     1035 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-word.svg
+-rw-r--r--   0        0        0      484 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/file.svg
+-rw-r--r--   0        0        0      972 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/flag.svg
+-rw-r--r--   0        0        0      929 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/flushed.svg
+-rw-r--r--   0        0        0      548 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/folder-open.svg
+-rw-r--r--   0        0        0      487 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/folder.svg
+-rw-r--r--   0        0        0     3174 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/font-awesome-logo-full.svg
+-rw-r--r--   0        0        0      721 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/frown-open.svg
+-rw-r--r--   0        0        0      778 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/frown.svg
+-rw-r--r--   0        0        0      905 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/futbol.svg
+-rw-r--r--   0        0        0      626 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/gem.svg
+-rw-r--r--   0        0        0      902 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grimace.svg
+-rw-r--r--   0        0        0      900 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-alt.svg
+-rw-r--r--   0        0        0     1280 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-beam-sweat.svg
+-rw-r--r--   0        0        0     1000 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-beam.svg
+-rw-r--r--   0        0        0      942 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-hearts.svg
+-rw-r--r--   0        0        0     1566 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-squint-tears.svg
+-rw-r--r--   0        0        0      950 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-squint.svg
+-rw-r--r--   0        0        0     1019 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-stars.svg
+-rw-r--r--   0        0        0     1503 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tears.svg
+-rw-r--r--   0        0        0     1213 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue-squint.svg
+-rw-r--r--   0        0        0     1256 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue-wink.svg
+-rw-r--r--   0        0        0      986 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue.svg
+-rw-r--r--   0        0        0      901 2023-08-29 11:20:58.180933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-wink.svg
+-rw-r--r--   0        0        0      722 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin.svg
+-rw-r--r--   0        0        0      955 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-lizard.svg
+-rw-r--r--   0        0        0     1167 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-paper.svg
+-rw-r--r--   0        0        0     1300 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-peace.svg
+-rw-r--r--   0        0        0     1315 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-down.svg
+-rw-r--r--   0        0        0     1319 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-left.svg
+-rw-r--r--   0        0        0     1326 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-right.svg
+-rw-r--r--   0        0        0     1320 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-up.svg
+-rw-r--r--   0        0        0     1578 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-pointer.svg
+-rw-r--r--   0        0        0     1311 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-rock.svg
+-rw-r--r--   0        0        0     1301 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-scissors.svg
+-rw-r--r--   0        0        0     1667 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-spock.svg
+-rw-r--r--   0        0        0     1313 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/handshake.svg
+-rw-r--r--   0        0        0      722 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hdd.svg
+-rw-r--r--   0        0        0      670 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/heart.svg
+-rw-r--r--   0        0        0     1245 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hospital.svg
+-rw-r--r--   0        0        0      727 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/hourglass.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/id-badge.svg
+-rw-r--r--   0        0        0      863 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/id-card.svg
+-rw-r--r--   0        0        0      671 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/image.svg
+-rw-r--r--   0        0        0      824 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/images.svg
+-rw-r--r--   0        0        0     1846 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/keyboard.svg
+-rw-r--r--   0        0        0     1193 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss-beam.svg
+-rw-r--r--   0        0        0     1362 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss-wink-heart.svg
+-rw-r--r--   0        0        0      912 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss.svg
+-rw-r--r--   0        0        0      975 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-beam.svg
+-rw-r--r--   0        0        0      872 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-squint.svg
+-rw-r--r--   0        0        0      895 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-wink.svg
+-rw-r--r--   0        0        0      775 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh.svg
+-rw-r--r--   0        0        0     1144 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/lemon.svg
+-rw-r--r--   0        0        0      917 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/life-ring.svg
+-rw-r--r--   0        0        0     1036 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/lightbulb.svg
+-rw-r--r--   0        0        0     1038 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/list-alt.svg
+-rw-r--r--   0        0        0      759 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/map.svg
+-rw-r--r--   0        0        0      556 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh-blank.svg
+-rw-r--r--   0        0        0     1006 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh-rolling-eyes.svg
+-rw-r--r--   0        0        0      644 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh.svg
+-rw-r--r--   0        0        0      556 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/minus-square.svg
+-rw-r--r--   0        0        0      845 2023-08-29 11:20:58.181933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/money-bill-alt.svg
+-rw-r--r--   0        0        0      779 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/moon.svg
+-rw-r--r--   0        0        0     1126 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/newspaper.svg
+-rw-r--r--   0        0        0     1096 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/object-group.svg
+-rw-r--r--   0        0        0     1290 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/object-ungroup.svg
+-rw-r--r--   0        0        0      621 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/paper-plane.svg
+-rw-r--r--   0        0        0      612 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/pause-circle.svg
+-rw-r--r--   0        0        0      524 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/play-circle.svg
+-rw-r--r--   0        0        0      660 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/plus-square.svg
+-rw-r--r--   0        0        0     1009 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/question-circle.svg
+-rw-r--r--   0        0        0      914 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/registered.svg
+-rw-r--r--   0        0        0     1043 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/sad-cry.svg
+-rw-r--r--   0        0        0      841 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/sad-tear.svg
+-rw-r--r--   0        0        0      779 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/save.svg
+-rw-r--r--   0        0        0     1181 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/share-square.svg
+-rw-r--r--   0        0        0     1055 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile-beam.svg
+-rw-r--r--   0        0        0      861 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile-wink.svg
+-rw-r--r--   0        0        0      769 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile.svg
+-rw-r--r--   0        0        0     1782 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/snowflake.svg
+-rw-r--r--   0        0        0      452 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/square.svg
+-rw-r--r--   0        0        0      462 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/star-half.svg
+-rw-r--r--   0        0        0      628 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/star.svg
+-rw-r--r--   0        0        0      523 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/sticky-note.svg
+-rw-r--r--   0        0        0      517 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/stop-circle.svg
+-rw-r--r--   0        0        0     1132 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/sun.svg
+-rw-r--r--   0        0        0      627 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/surprise.svg
+-rw-r--r--   0        0        0     1231 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/thumbs-down.svg
+-rw-r--r--   0        0        0     1224 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/thumbs-up.svg
+-rw-r--r--   0        0        0      728 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/times-circle.svg
+-rw-r--r--   0        0        0      950 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/tired.svg
+-rw-r--r--   0        0        0      761 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/trash-alt.svg
+-rw-r--r--   0        0        0      845 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/user-circle.svg
+-rw-r--r--   0        0        0      701 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/user.svg
+-rw-r--r--   0        0        0      783 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/window-close.svg
+-rw-r--r--   0        0        0      420 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/window-maximize.svg
+-rw-r--r--   0        0        0      348 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/window-minimize.svg
+-rw-r--r--   0        0        0      498 2023-08-29 11:20:58.182933 pyedifice-0.5.4/edifice/icons/font-awesome/regular/window-restore.svg
+-rw-r--r--   0        0        0      960 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ad.svg
+-rw-r--r--   0        0        0      773 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/address-book.svg
+-rw-r--r--   0        0        0      873 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/address-card.svg
+-rw-r--r--   0        0        0      419 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/adjust.svg
+-rw-r--r--   0        0        0      823 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/air-freshener.svg
+-rw-r--r--   0        0        0      731 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-center.svg
+-rw-r--r--   0        0        0      632 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-justify.svg
+-rw-r--r--   0        0        0      739 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-left.svg
+-rw-r--r--   0        0        0      747 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-right.svg
+-rw-r--r--   0        0        0     1185 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/allergies.svg
+-rw-r--r--   0        0        0      887 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ambulance.svg
+-rw-r--r--   0        0        0     2349 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/american-sign-language-interpreting.svg
+-rw-r--r--   0        0        0     1085 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/anchor.svg
+-rw-r--r--   0        0        0      634 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-down.svg
+-rw-r--r--   0        0        0      636 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-left.svg
+-rw-r--r--   0        0        0      638 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-right.svg
+-rw-r--r--   0        0        0      637 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-up.svg
+-rw-r--r--   0        0        0      450 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-down.svg
+-rw-r--r--   0        0        0      448 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-left.svg
+-rw-r--r--   0        0        0      449 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-right.svg
+-rw-r--r--   0        0        0      449 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-up.svg
+-rw-r--r--   0        0        0      947 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/angry.svg
+-rw-r--r--   0        0        0      661 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ankh.svg
+-rw-r--r--   0        0        0     1056 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/apple-alt.svg
+-rw-r--r--   0        0        0      524 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/archive.svg
+-rw-r--r--   0        0        0      586 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/archway.svg
+-rw-r--r--   0        0        0      500 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-alt-circle-down.svg
+-rw-r--r--   0        0        0      501 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-alt-circle-left.svg
+-rw-r--r--   0        0        0      495 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-alt-circle-right.svg
+-rw-r--r--   0        0        0      495 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-alt-circle-up.svg
+-rw-r--r--   0        0        0      584 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-down.svg
+-rw-r--r--   0        0        0      581 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-left.svg
+-rw-r--r--   0        0        0      582 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-right.svg
+-rw-r--r--   0        0        0      577 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-up.svg
+-rw-r--r--   0        0        0      508 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-down.svg
+-rw-r--r--   0        0        0      508 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-left.svg
+-rw-r--r--   0        0        0      513 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-right.svg
+-rw-r--r--   0        0        0      511 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-up.svg
+-rw-r--r--   0        0        0      595 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt-h.svg
+-rw-r--r--   0        0        0      593 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt-v.svg
+-rw-r--r--   0        0        0      939 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt.svg
+-rw-r--r--   0        0        0     1285 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/assistive-listening-systems.svg
+-rw-r--r--   0        0        0      959 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/asterisk.svg
+-rw-r--r--   0        0        0     1157 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/at.svg
+-rw-r--r--   0        0        0     1117 2023-08-29 11:20:58.183933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/atlas.svg
+-rw-r--r--   0        0        0     2056 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/atom.svg
+-rw-r--r--   0        0        0     1042 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/audio-description.svg
+-rw-r--r--   0        0        0     1702 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/award.svg
+-rw-r--r--   0        0        0      835 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/baby-carriage.svg
+-rw-r--r--   0        0        0      886 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/baby.svg
+-rw-r--r--   0        0        0      835 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/backspace.svg
+-rw-r--r--   0        0        0      487 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/backward.svg
+-rw-r--r--   0        0        0     1080 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacon.svg
+-rw-r--r--   0        0        0     3069 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacteria.svg
+-rw-r--r--   0        0        0     1680 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacterium.svg
+-rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bahai.svg
+-rw-r--r--   0        0        0     1088 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale-left.svg
+-rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale-right.svg
+-rw-r--r--   0        0        0      984 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale.svg
+-rw-r--r--   0        0        0      583 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ban.svg
+-rw-r--r--   0        0        0      697 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/band-aid.svg
+-rw-r--r--   0        0        0      749 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/barcode.svg
+-rw-r--r--   0        0        0      601 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bars.svg
+-rw-r--r--   0        0        0      931 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/baseball-ball.svg
+-rw-r--r--   0        0        0      950 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/basketball-ball.svg
+-rw-r--r--   0        0        0      812 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bath.svg
+-rw-r--r--   0        0        0      473 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/battery-empty.svg
+-rw-r--r--   0        0        0      496 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/battery-full.svg
+-rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/battery-half.svg
+-rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/battery-quarter.svg
+-rw-r--r--   0        0        0      497 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/battery-three-quarters.svg
+-rw-r--r--   0        0        0      563 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bed.svg
+-rw-r--r--   0        0        0      769 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/beer.svg
+-rw-r--r--   0        0        0      875 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bell-slash.svg
+-rw-r--r--   0        0        0      657 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bell.svg
+-rw-r--r--   0        0        0     1056 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bezier-curve.svg
+-rw-r--r--   0        0        0      733 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bible.svg
+-rw-r--r--   0        0        0     1602 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bicycle.svg
+-rw-r--r--   0        0        0      702 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/biking.svg
+-rw-r--r--   0        0        0      707 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/binoculars.svg
+-rw-r--r--   0        0        0     1701 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/biohazard.svg
+-rw-r--r--   0        0        0      958 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/birthday-cake.svg
+-rw-r--r--   0        0        0     1005 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/blender-phone.svg
+-rw-r--r--   0        0        0      751 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/blender.svg
+-rw-r--r--   0        0        0     1073 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/blind.svg
+-rw-r--r--   0        0        0      879 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/blog.svg
+-rw-r--r--   0        0        0      579 2023-08-29 11:20:58.184933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bold.svg
+-rw-r--r--   0        0        0      469 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bolt.svg
+-rw-r--r--   0        0        0     1102 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bomb.svg
+-rw-r--r--   0        0        0      875 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bone.svg
+-rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bong.svg
+-rw-r--r--   0        0        0     1128 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-dead.svg
+-rw-r--r--   0        0        0      652 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-medical.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-open.svg
+-rw-r--r--   0        0        0      798 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-reader.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/book.svg
+-rw-r--r--   0        0        0      336 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bookmark.svg
+-rw-r--r--   0        0        0      429 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/border-all.svg
+-rw-r--r--   0        0        0     2202 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/border-none.svg
+-rw-r--r--   0        0        0     1027 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/border-style.svg
+-rw-r--r--   0        0        0      544 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bowling-ball.svg
+-rw-r--r--   0        0        0      761 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/box-open.svg
+-rw-r--r--   0        0        0      560 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/box-tissue.svg
+-rw-r--r--   0        0        0      486 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/box.svg
+-rw-r--r--   0        0        0      642 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/boxes.svg
+-rw-r--r--   0        0        0     1238 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/braille.svg
+-rw-r--r--   0        0        0      925 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/brain.svg
+-rw-r--r--   0        0        0      420 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bread-slice.svg
+-rw-r--r--   0        0        0      629 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/briefcase-medical.svg
+-rw-r--r--   0        0        0      528 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/briefcase.svg
+-rw-r--r--   0        0        0     1660 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/broadcast-tower.svg
+-rw-r--r--   0        0        0      727 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/broom.svg
+-rw-r--r--   0        0        0      532 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/brush.svg
+-rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bug.svg
+-rw-r--r--   0        0        0     1144 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/building.svg
+-rw-r--r--   0        0        0      916 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bullhorn.svg
+-rw-r--r--   0        0        0      624 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bullseye.svg
+-rw-r--r--   0        0        0      467 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/burn.svg
+-rw-r--r--   0        0        0      987 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bus-alt.svg
+-rw-r--r--   0        0        0      870 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/bus.svg
+-rw-r--r--   0        0        0      866 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/business-time.svg
+-rw-r--r--   0        0        0     1149 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calculator.svg
+-rw-r--r--   0        0        0     1084 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-alt.svg
+-rw-r--r--   0        0        0      894 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-check.svg
+-rw-r--r--   0        0        0      591 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-day.svg
+-rw-r--r--   0        0        0      669 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-minus.svg
+-rw-r--r--   0        0        0      773 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-plus.svg
+-rw-r--r--   0        0        0      882 2023-08-29 11:20:58.185933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-times.svg
+-rw-r--r--   0        0        0      592 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-week.svg
+-rw-r--r--   0        0        0      572 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar.svg
+-rw-r--r--   0        0        0      855 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/camera-retro.svg
+-rw-r--r--   0        0        0      602 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/camera.svg
+-rw-r--r--   0        0        0      631 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/campground.svg
+-rw-r--r--   0        0        0     1093 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/candy-cane.svg
+-rw-r--r--   0        0        0     1334 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cannabis.svg
+-rw-r--r--   0        0        0      788 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/capsules.svg
+-rw-r--r--   0        0        0      918 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-alt.svg
+-rw-r--r--   0        0        0      781 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-battery.svg
+-rw-r--r--   0        0        0     2160 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-crash.svg
+-rw-r--r--   0        0        0      764 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-side.svg
+-rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/car.svg
+-rw-r--r--   0        0        0      653 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caravan.svg
+-rw-r--r--   0        0        0      379 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-down.svg
+-rw-r--r--   0        0        0      420 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-left.svg
+-rw-r--r--   0        0        0      412 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-right.svg
+-rw-r--r--   0        0        0      474 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-down.svg
+-rw-r--r--   0        0        0      542 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-left.svg
+-rw-r--r--   0        0        0      538 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-right.svg
+-rw-r--r--   0        0        0      537 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-up.svg
+-rw-r--r--   0        0        0      420 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-up.svg
+-rw-r--r--   0        0        0      730 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/carrot.svg
+-rw-r--r--   0        0        0     1093 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cart-arrow-down.svg
+-rw-r--r--   0        0        0     1110 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cart-plus.svg
+-rw-r--r--   0        0        0     1354 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cash-register.svg
+-rw-r--r--   0        0        0      818 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cat.svg
+-rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/certificate.svg
+-rw-r--r--   0        0        0      658 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chair.svg
+-rw-r--r--   0        0        0      779 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chalkboard-teacher.svg
+-rw-r--r--   0        0        0      463 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chalkboard.svg
+-rw-r--r--   0        0        0     1088 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/charging-station.svg
+-rw-r--r--   0        0        0      497 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-area.svg
+-rw-r--r--   0        0        0      922 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-bar.svg
+-rw-r--r--   0        0        0      726 2023-08-29 11:20:58.186933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-line.svg
+-rw-r--r--   0        0        0      695 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-pie.svg
+-rw-r--r--   0        0        0      616 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-circle.svg
+-rw-r--r--   0        0        0      643 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-double.svg
+-rw-r--r--   0        0        0      639 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-square.svg
+-rw-r--r--   0        0        0      534 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/check.svg
+-rw-r--r--   0        0        0      385 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cheese.svg
+-rw-r--r--   0        0        0      699 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-bishop.svg
+-rw-r--r--   0        0        0      920 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-board.svg
+-rw-r--r--   0        0        0      564 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-king.svg
+-rw-r--r--   0        0        0      732 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-knight.svg
+-rw-r--r--   0        0        0      609 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-pawn.svg
+-rw-r--r--   0        0        0      840 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-queen.svg
+-rw-r--r--   0        0        0      618 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-rook.svg
+-rw-r--r--   0        0        0     1235 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess.svg
+-rw-r--r--   0        0        0      521 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-down.svg
+-rw-r--r--   0        0        0      521 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-left.svg
+-rw-r--r--   0        0        0      518 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-right.svg
+-rw-r--r--   0        0        0      516 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-up.svg
+-rw-r--r--   0        0        0      539 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-down.svg
+-rw-r--r--   0        0        0      498 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-left.svg
+-rw-r--r--   0        0        0      541 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-right.svg
+-rw-r--r--   0        0        0      544 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-up.svg
+-rw-r--r--   0        0        0      705 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/child.svg
+-rw-r--r--   0        0        0      762 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/church.svg
+-rw-r--r--   0        0        0      728 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/circle-notch.svg
+-rw-r--r--   0        0        0      329 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/circle.svg
+-rw-r--r--   0        0        0     1713 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/city.svg
+-rw-r--r--   0        0        0      770 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clinic-medical.svg
+-rw-r--r--   0        0        0      667 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard-check.svg
+-rw-r--r--   0        0        0      952 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard-list.svg
+-rw-r--r--   0        0        0      577 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard.svg
+-rw-r--r--   0        0        0      482 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clock.svg
+-rw-r--r--   0        0        0      502 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/clone.svg
+-rw-r--r--   0        0        0      834 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/closed-captioning.svg
+-rw-r--r--   0        0        0      691 2023-08-29 11:20:58.187933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-download-alt.svg
+-rw-r--r--   0        0        0     1255 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-meatball.svg
+-rw-r--r--   0        0        0     1350 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-moon-rain.svg
+-rw-r--r--   0        0        0      856 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-moon.svg
+-rw-r--r--   0        0        0      874 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-rain.svg
+-rw-r--r--   0        0        0     1231 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-showers-heavy.svg
+-rw-r--r--   0        0        0     1630 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-sun-rain.svg
+-rw-r--r--   0        0        0     1045 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-sun.svg
+-rw-r--r--   0        0        0      691 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-upload-alt.svg
+-rw-r--r--   0        0        0      514 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud.svg
+-rw-r--r--   0        0        0      704 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cocktail.svg
+-rw-r--r--   0        0        0      935 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/code-branch.svg
+-rw-r--r--   0        0        0      800 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/code.svg
+-rw-r--r--   0        0        0      496 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/coffee.svg
+-rw-r--r--   0        0        0     1070 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cog.svg
+-rw-r--r--   0        0        0     2645 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cogs.svg
+-rw-r--r--   0        0        0      791 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/coins.svg
+-rw-r--r--   0        0        0      420 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/columns.svg
+-rw-r--r--   0        0        0      402 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-alt.svg
+-rw-r--r--   0        0        0     1187 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-dollar.svg
+-rw-r--r--   0        0        0      695 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-dots.svg
+-rw-r--r--   0        0        0      628 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-medical.svg
+-rw-r--r--   0        0        0      730 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-slash.svg
+-rw-r--r--   0        0        0      480 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment.svg
+-rw-r--r--   0        0        0     1498 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comments-dollar.svg
+-rw-r--r--   0        0        0      759 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/comments.svg
+-rw-r--r--   0        0        0      526 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/compact-disc.svg
+-rw-r--r--   0        0        0      675 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/compass.svg
+-rw-r--r--   0        0        0      775 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress-alt.svg
+-rw-r--r--   0        0        0      982 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress-arrows-alt.svg
+-rw-r--r--   0        0        0      765 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress.svg
+-rw-r--r--   0        0        0      559 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/concierge-bell.svg
+-rw-r--r--   0        0        0      931 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cookie-bite.svg
+-rw-r--r--   0        0        0      964 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cookie.svg
+-rw-r--r--   0        0        0      611 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/copy.svg
+-rw-r--r--   0        0        0      833 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/copyright.svg
+-rw-r--r--   0        0        0      627 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/couch.svg
+-rw-r--r--   0        0        0      583 2023-08-29 11:20:58.188933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/credit-card.svg
+-rw-r--r--   0        0        0      576 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crop-alt.svg
+-rw-r--r--   0        0        0      670 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crop.svg
+-rw-r--r--   0        0        0      496 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cross.svg
+-rw-r--r--   0        0        0     1210 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crosshairs.svg
+-rw-r--r--   0        0        0      807 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crow.svg
+-rw-r--r--   0        0        0      763 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crown.svg
+-rw-r--r--   0        0        0      749 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/crutch.svg
+-rw-r--r--   0        0        0      554 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cube.svg
+-rw-r--r--   0        0        0      867 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cubes.svg
+-rw-r--r--   0        0        0      866 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/cut.svg
+-rw-r--r--   0        0        0      657 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/database.svg
+-rw-r--r--   0        0        0     1179 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/deaf.svg
+-rw-r--r--   0        0        0     1493 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/democrat.svg
+-rw-r--r--   0        0        0      488 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/desktop.svg
+-rw-r--r--   0        0        0     2218 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dharmachakra.svg
+-rw-r--r--   0        0        0     1087 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/diagnoses.svg
+-rw-r--r--   0        0        0     1186 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-d20.svg
+-rw-r--r--   0        0        0      707 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-d6.svg
+-rw-r--r--   0        0        0      755 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-five.svg
+-rw-r--r--   0        0        0      681 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-four.svg
+-rw-r--r--   0        0        0      451 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-one.svg
+-rw-r--r--   0        0        0      829 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-six.svg
+-rw-r--r--   0        0        0      603 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-three.svg
+-rw-r--r--   0        0        0      529 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-two.svg
+-rw-r--r--   0        0        0     1151 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice.svg
+-rw-r--r--   0        0        0     1044 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/digital-tachograph.svg
+-rw-r--r--   0        0        0      675 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/directions.svg
+-rw-r--r--   0        0        0      846 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/disease.svg
+-rw-r--r--   0        0        0      529 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/divide.svg
+-rw-r--r--   0        0        0      808 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dizzy.svg
+-rw-r--r--   0        0        0     1025 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dna.svg
+-rw-r--r--   0        0        0      666 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dog.svg
+-rw-r--r--   0        0        0      861 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dollar-sign.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dolly-flatbed.svg
+-rw-r--r--   0        0        0      844 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dolly.svg
+-rw-r--r--   0        0        0     1195 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/donate.svg
+-rw-r--r--   0        0        0      530 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/door-closed.svg
+-rw-r--r--   0        0        0      598 2023-08-29 11:20:58.189933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/door-open.svg
+-rw-r--r--   0        0        0      431 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dot-circle.svg
+-rw-r--r--   0        0        0      778 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dove.svg
+-rw-r--r--   0        0        0      702 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/download.svg
+-rw-r--r--   0        0        0     1143 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/drafting-compass.svg
+-rw-r--r--   0        0        0     1100 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dragon.svg
+-rw-r--r--   0        0        0     1273 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/draw-polygon.svg
+-rw-r--r--   0        0        0      911 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/drum-steelpan.svg
+-rw-r--r--   0        0        0      904 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/drum.svg
+-rw-r--r--   0        0        0      680 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/drumstick-bite.svg
+-rw-r--r--   0        0        0      790 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumbbell.svg
+-rw-r--r--   0        0        0     1164 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumpster-fire.svg
+-rw-r--r--   0        0        0      719 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumpster.svg
+-rw-r--r--   0        0        0     2102 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/dungeon.svg
+-rw-r--r--   0        0        0      767 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/edit.svg
+-rw-r--r--   0        0        0      326 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/egg.svg
+-rw-r--r--   0        0        0      545 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/eject.svg
+-rw-r--r--   0        0        0      477 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ellipsis-h.svg
+-rw-r--r--   0        0        0      471 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ellipsis-v.svg
+-rw-r--r--   0        0        0     1016 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-open-text.svg
+-rw-r--r--   0        0        0     1051 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-open.svg
+-rw-r--r--   0        0        0      859 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-square.svg
+-rw-r--r--   0        0        0      724 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope.svg
+-rw-r--r--   0        0        0      490 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/equals.svg
+-rw-r--r--   0        0        0      596 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/eraser.svg
+-rw-r--r--   0        0        0      522 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ethernet.svg
+-rw-r--r--   0        0        0     1138 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/euro-sign.svg
+-rw-r--r--   0        0        0      655 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/exchange-alt.svg
+-rw-r--r--   0        0        0      642 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation-circle.svg
+-rw-r--r--   0        0        0      708 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation-triangle.svg
+-rw-r--r--   0        0        0      527 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation.svg
+-rw-r--r--   0        0        0      769 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand-alt.svg
+-rw-r--r--   0        0        0      763 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand-arrows-alt.svg
+-rw-r--r--   0        0        0      768 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand.svg
+-rw-r--r--   0        0        0      603 2023-08-29 11:20:58.190933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/external-link-alt.svg
+-rw-r--r--   0        0        0      639 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/external-link-square-alt.svg
+-rw-r--r--   0        0        0      681 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye-dropper.svg
+-rw-r--r--   0        0        0      995 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye-slash.svg
+-rw-r--r--   0        0        0      590 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye.svg
+-rw-r--r--   0        0        0      762 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fan.svg
+-rw-r--r--   0        0        0      526 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fast-backward.svg
+-rw-r--r--   0        0        0      529 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fast-forward.svg
+-rw-r--r--   0        0        0      791 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/faucet.svg
+-rw-r--r--   0        0        0      919 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fax.svg
+-rw-r--r--   0        0        0      659 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/feather-alt.svg
+-rw-r--r--   0        0        0      678 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/feather.svg
+-rw-r--r--   0        0        0      610 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/female.svg
+-rw-r--r--   0        0        0      631 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fighter-jet.svg
+-rw-r--r--   0        0        0      737 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-alt.svg
+-rw-r--r--   0        0        0      767 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-archive.svg
+-rw-r--r--   0        0        0      826 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-audio.svg
+-rw-r--r--   0        0        0     1120 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-code.svg
+-rw-r--r--   0        0        0     1142 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-contract.svg
+-rw-r--r--   0        0        0     1296 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-csv.svg
+-rw-r--r--   0        0        0      644 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-download.svg
+-rw-r--r--   0        0        0      822 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-excel.svg
+-rw-r--r--   0        0        0      626 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-export.svg
+-rw-r--r--   0        0        0      718 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-image.svg
+-rw-r--r--   0        0        0      630 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-import.svg
+-rw-r--r--   0        0        0     1293 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-invoice-dollar.svg
+-rw-r--r--   0        0        0      858 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-invoice.svg
+-rw-r--r--   0        0        0      677 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-medical-alt.svg
+-rw-r--r--   0        0        0      630 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-medical.svg
+-rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-pdf.svg
+-rw-r--r--   0        0        0      693 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-powerpoint.svg
+-rw-r--r--   0        0        0      954 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-prescription.svg
+-rw-r--r--   0        0        0     1076 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-signature.svg
+-rw-r--r--   0        0        0      647 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-upload.svg
+-rw-r--r--   0        0        0      738 2023-08-29 11:20:58.191933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-video.svg
+-rw-r--r--   0        0        0      924 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-word.svg
+-rw-r--r--   0        0        0      447 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/file.svg
+-rw-r--r--   0        0        0      882 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fill-drip.svg
+-rw-r--r--   0        0        0      820 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fill.svg
+-rw-r--r--   0        0        0     1352 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/film.svg
+-rw-r--r--   0        0        0      465 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/filter.svg
+-rw-r--r--   0        0        0     2123 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fingerprint.svg
+-rw-r--r--   0        0        0      686 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire-alt.svg
+-rw-r--r--   0        0        0      888 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire-extinguisher.svg
+-rw-r--r--   0        0        0      531 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire.svg
+-rw-r--r--   0        0        0      588 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/first-aid.svg
+-rw-r--r--   0        0        0      603 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fish.svg
+-rw-r--r--   0        0        0     1290 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/fist-raised.svg
+-rw-r--r--   0        0        0     1194 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag-checkered.svg
+-rw-r--r--   0        0        0     1284 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag-usa.svg
+-rw-r--r--   0        0        0      787 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag.svg
+-rw-r--r--   0        0        0      558 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/flask.svg
+-rw-r--r--   0        0        0      675 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/flushed.svg
+-rw-r--r--   0        0        0      496 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder-minus.svg
+-rw-r--r--   0        0        0      582 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder-open.svg
+-rw-r--r--   0        0        0      563 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder-plus.svg
+-rw-r--r--   0        0        0      387 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder.svg
+-rw-r--r--   0        0        0     3174 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/font-awesome-logo-full.svg
+-rw-r--r--   0        0        0      588 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/font.svg
+-rw-r--r--   0        0        0     1247 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/football-ball.svg
+-rw-r--r--   0        0        0      480 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/forward.svg
+-rw-r--r--   0        0        0      979 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/frog.svg
+-rw-r--r--   0        0        0      637 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/frown-open.svg
+-rw-r--r--   0        0        0      646 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/frown.svg
+-rw-r--r--   0        0        0     1254 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/funnel-dollar.svg
+-rw-r--r--   0        0        0      923 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/futbol.svg
+-rw-r--r--   0        0        0      608 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gamepad.svg
+-rw-r--r--   0        0        0      738 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gas-pump.svg
+-rw-r--r--   0        0        0      976 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gavel.svg
+-rw-r--r--   0        0        0      532 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gem.svg
+-rw-r--r--   0        0        0      412 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/genderless.svg
+-rw-r--r--   0        0        0      777 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ghost.svg
+-rw-r--r--   0        0        0      758 2023-08-29 11:20:58.192933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gift.svg
+-rw-r--r--   0        0        0     1337 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gifts.svg
+-rw-r--r--   0        0        0      962 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/glass-cheers.svg
+-rw-r--r--   0        0        0      503 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/glass-martini-alt.svg
+-rw-r--r--   0        0        0      464 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/glass-martini.svg
+-rw-r--r--   0        0        0      439 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/glass-whiskey.svg
+-rw-r--r--   0        0        0     1510 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/glasses.svg
+-rw-r--r--   0        0        0     1493 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-africa.svg
+-rw-r--r--   0        0        0     1652 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-americas.svg
+-rw-r--r--   0        0        0     1531 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-asia.svg
+-rw-r--r--   0        0        0     1638 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-europe.svg
+-rw-r--r--   0        0        0      998 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe.svg
+-rw-r--r--   0        0        0      879 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/golf-ball.svg
+-rw-r--r--   0        0        0      890 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/gopuram.svg
+-rw-r--r--   0        0        0      874 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/graduation-cap.svg
+-rw-r--r--   0        0        0      669 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/greater-than-equal.svg
+-rw-r--r--   0        0        0      554 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/greater-than.svg
+-rw-r--r--   0        0        0      758 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grimace.svg
+-rw-r--r--   0        0        0      848 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-alt.svg
+-rw-r--r--   0        0        0     1071 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-beam-sweat.svg
+-rw-r--r--   0        0        0      849 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-beam.svg
+-rw-r--r--   0        0        0      865 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-hearts.svg
+-rw-r--r--   0        0        0     1291 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-squint-tears.svg
+-rw-r--r--   0        0        0      736 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-squint.svg
+-rw-r--r--   0        0        0      931 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-stars.svg
+-rw-r--r--   0        0        0     1367 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tears.svg
+-rw-r--r--   0        0        0     1027 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue-squint.svg
+-rw-r--r--   0        0        0     1082 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue-wink.svg
+-rw-r--r--   0        0        0      931 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-wink.svg
+-rw-r--r--   0        0        0      641 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin.svg
+-rw-r--r--   0        0        0      943 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-horizontal.svg
+-rw-r--r--   0        0        0      456 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-lines-vertical.svg
+-rw-r--r--   0        0        0      458 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-lines.svg
+-rw-r--r--   0        0        0      938 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-vertical.svg
+-rw-r--r--   0        0        0      867 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/guitar.svg
+-rw-r--r--   0        0        0      614 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/h-square.svg
+-rw-r--r--   0        0        0      677 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hamburger.svg
+-rw-r--r--   0        0        0      826 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hammer.svg
+-rw-r--r--   0        0        0      846 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hamsa.svg
+-rw-r--r--   0        0        0      773 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-heart.svg
+-rw-r--r--   0        0        0      789 2023-08-29 11:20:58.193933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-medical.svg
+-rw-r--r--   0        0        0     1257 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-usd.svg
+-rw-r--r--   0        0        0      701 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-water.svg
+-rw-r--r--   0        0        0      577 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding.svg
+-rw-r--r--   0        0        0      640 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-lizard.svg
+-rw-r--r--   0        0        0      717 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-middle-finger.svg
+-rw-r--r--   0        0        0      839 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-paper.svg
+-rw-r--r--   0        0        0      706 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-peace.svg
+-rw-r--r--   0        0        0      988 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-down.svg
+-rw-r--r--   0        0        0      992 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-left.svg
+-rw-r--r--   0        0        0      995 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-right.svg
+-rw-r--r--   0        0        0      990 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-up.svg
+-rw-r--r--   0        0        0      737 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-pointer.svg
+-rw-r--r--   0        0        0      774 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-rock.svg
+-rw-r--r--   0        0        0      711 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-scissors.svg
+-rw-r--r--   0        0        0     1461 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-sparkles.svg
+-rw-r--r--   0        0        0      968 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-spock.svg
+-rw-r--r--   0        0        0      779 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands-helping.svg
+-rw-r--r--   0        0        0     1481 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands-wash.svg
+-rw-r--r--   0        0        0      958 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands.svg
+-rw-r--r--   0        0        0      865 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake-alt-slash.svg
+-rw-r--r--   0        0        0      960 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake-slash.svg
+-rw-r--r--   0        0        0     1083 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake.svg
+-rw-r--r--   0        0        0     1760 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hanukiah.svg
+-rw-r--r--   0        0        0      502 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hard-hat.svg
+-rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hashtag.svg
+-rw-r--r--   0        0        0      681 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-cowboy-side.svg
+-rw-r--r--   0        0        0      662 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-cowboy.svg
+-rw-r--r--   0        0        0      597 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-wizard.svg
+-rw-r--r--   0        0        0      705 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hdd.svg
+-rw-r--r--   0        0        0      954 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-cough-slash.svg
+-rw-r--r--   0        0        0      803 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-cough.svg
+-rw-r--r--   0        0        0      697 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-mask.svg
+-rw-r--r--   0        0        0     1111 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-virus.svg
+-rw-r--r--   0        0        0      650 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/heading.svg
+-rw-r--r--   0        0        0      773 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/headphones-alt.svg
+-rw-r--r--   0        0        0      728 2023-08-29 11:20:58.194933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/headphones.svg
+-rw-r--r--   0        0        0      832 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/headset.svg
+-rw-r--r--   0        0        0      497 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/heart-broken.svg
+-rw-r--r--   0        0        0      467 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/heart.svg
+-rw-r--r--   0        0        0      666 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/heartbeat.svg
+-rw-r--r--   0        0        0      839 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/helicopter.svg
+-rw-r--r--   0        0        0      626 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/highlighter.svg
+-rw-r--r--   0        0        0     1086 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hiking.svg
+-rw-r--r--   0        0        0      831 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hippo.svg
+-rw-r--r--   0        0        0      981 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/history.svg
+-rw-r--r--   0        0        0      412 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hockey-puck.svg
+-rw-r--r--   0        0        0     1392 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/holly-berry.svg
+-rw-r--r--   0        0        0      745 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/home.svg
+-rw-r--r--   0        0        0      782 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/horse-head.svg
+-rw-r--r--   0        0        0     1091 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/horse.svg
+-rw-r--r--   0        0        0     1194 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-alt.svg
+-rw-r--r--   0        0        0      521 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-symbol.svg
+-rw-r--r--   0        0        0     1253 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-user.svg
+-rw-r--r--   0        0        0     1145 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital.svg
+-rw-r--r--   0        0        0     1438 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hot-tub.svg
+-rw-r--r--   0        0        0     1229 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hotdog.svg
+-rw-r--r--   0        0        0     1373 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hotel.svg
+-rw-r--r--   0        0        0      696 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-end.svg
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-half.svg
+-rw-r--r--   0        0        0      694 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-start.svg
+-rw-r--r--   0        0        0      627 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass.svg
+-rw-r--r--   0        0        0      843 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/house-damage.svg
+-rw-r--r--   0        0        0      855 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/house-user.svg
+-rw-r--r--   0        0        0     1139 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/hryvnia.svg
+-rw-r--r--   0        0        0      995 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/i-cursor.svg
+-rw-r--r--   0        0        0      390 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ice-cream.svg
+-rw-r--r--   0        0        0      502 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/icicles.svg
+-rw-r--r--   0        0        0     1308 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/icons.svg
+-rw-r--r--   0        0        0      691 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-badge.svg
+-rw-r--r--   0        0        0      691 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-card-alt.svg
+-rw-r--r--   0        0        0      891 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-card.svg
+-rw-r--r--   0        0        0      732 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/igloo.svg
+-rw-r--r--   0        0        0      594 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/image.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/images.svg
+-rw-r--r--   0        0        0      567 2023-08-29 11:20:58.195933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/inbox.svg
+-rw-r--r--   0        0        0      858 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/indent.svg
+-rw-r--r--   0        0        0      503 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/industry.svg
+-rw-r--r--   0        0        0      671 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/infinity.svg
+-rw-r--r--   0        0        0      659 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/info-circle.svg
+-rw-r--r--   0        0        0      568 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/info.svg
+-rw-r--r--   0        0        0      468 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/italic.svg
+-rw-r--r--   0        0        0     2071 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/jedi.svg
+-rw-r--r--   0        0        0     1136 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/joint.svg
+-rw-r--r--   0        0        0     2235 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/journal-whills.svg
+-rw-r--r--   0        0        0     1276 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/kaaba.svg
+-rw-r--r--   0        0        0      718 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/key.svg
+-rw-r--r--   0        0        0     1742 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/keyboard.svg
+-rw-r--r--   0        0        0     1857 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/khanda.svg
+-rw-r--r--   0        0        0      977 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss-beam.svg
+-rw-r--r--   0        0        0     1184 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss-wink-heart.svg
+-rw-r--r--   0        0        0      781 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss.svg
+-rw-r--r--   0        0        0     1001 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiwi-bird.svg
+-rw-r--r--   0        0        0      662 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/landmark.svg
+-rw-r--r--   0        0        0     1246 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/language.svg
+-rw-r--r--   0        0        0      992 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-code.svg
+-rw-r--r--   0        0        0      966 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-house.svg
+-rw-r--r--   0        0        0      684 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-medical.svg
+-rw-r--r--   0        0        0      523 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop.svg
+-rw-r--r--   0        0        0      789 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-beam.svg
+-rw-r--r--   0        0        0      683 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-squint.svg
+-rw-r--r--   0        0        0      675 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-wink.svg
+-rw-r--r--   0        0        0      586 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh.svg
+-rw-r--r--   0        0        0      899 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/layer-group.svg
+-rw-r--r--   0        0        0      634 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/leaf.svg
+-rw-r--r--   0        0        0      863 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lemon.svg
+-rw-r--r--   0        0        0      669 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/less-than-equal.svg
+-rw-r--r--   0        0        0      547 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/less-than.svg
+-rw-r--r--   0        0        0      543 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/level-down-alt.svg
+-rw-r--r--   0        0        0      547 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/level-up-alt.svg
+-rw-r--r--   0        0        0      923 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/life-ring.svg
+-rw-r--r--   0        0        0      824 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lightbulb.svg
+-rw-r--r--   0        0        0     1507 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/link.svg
+-rw-r--r--   0        0        0      898 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lira-sign.svg
+-rw-r--r--   0        0        0      964 2023-08-29 11:20:58.196933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-alt.svg
+-rw-r--r--   0        0        0     1496 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-ol.svg
+-rw-r--r--   0        0        0      671 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-ul.svg
+-rw-r--r--   0        0        0      818 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/list.svg
+-rw-r--r--   0        0        0      418 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/location-arrow.svg
+-rw-r--r--   0        0        0      537 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lock-open.svg
+-rw-r--r--   0        0        0      472 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lock.svg
+-rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/long-arrow-alt-down.svg
+-rw-r--r--   0        0        0      487 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/long-arrow-alt-left.svg
+-rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/long-arrow-alt-right.svg
+-rw-r--r--   0        0        0      486 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/long-arrow-alt-up.svg
+-rw-r--r--   0        0        0     1304 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/low-vision.svg
+-rw-r--r--   0        0        0      852 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/luggage-cart.svg
+-rw-r--r--   0        0        0     1659 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lungs-virus.svg
+-rw-r--r--   0        0        0     1050 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/lungs.svg
+-rw-r--r--   0        0        0      793 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/magic.svg
+-rw-r--r--   0        0        0      690 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/magnet.svg
+-rw-r--r--   0        0        0      866 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mail-bulk.svg
+-rw-r--r--   0        0        0      563 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/male.svg
+-rw-r--r--   0        0        0      905 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marked-alt.svg
+-rw-r--r--   0        0        0      834 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marked.svg
+-rw-r--r--   0        0        0      504 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marker-alt.svg
+-rw-r--r--   0        0        0      421 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marker.svg
+-rw-r--r--   0        0        0      592 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-pin.svg
+-rw-r--r--   0        0        0      756 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-signs.svg
+-rw-r--r--   0        0        0      498 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/map.svg
+-rw-r--r--   0        0        0      699 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/marker.svg
+-rw-r--r--   0        0        0      994 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-double.svg
+-rw-r--r--   0        0        0      767 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke-h.svg
+-rw-r--r--   0        0        0      766 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke-v.svg
+-rw-r--r--   0        0        0      736 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke.svg
+-rw-r--r--   0        0        0      570 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars.svg
+-rw-r--r--   0        0        0      846 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mask.svg
+-rw-r--r--   0        0        0      947 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/medal.svg
+-rw-r--r--   0        0        0      741 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/medkit.svg
+-rw-r--r--   0        0        0      473 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/meh-blank.svg
+-rw-r--r--   0        0        0      738 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/meh-rolling-eyes.svg
+-rw-r--r--   0        0        0      533 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/meh.svg
+-rw-r--r--   0        0        0      728 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/memory.svg
+-rw-r--r--   0        0        0     1417 2023-08-29 11:20:58.197933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/menorah.svg
+-rw-r--r--   0        0        0      910 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mercury.svg
+-rw-r--r--   0        0        0     1129 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/meteor.svg
+-rw-r--r--   0        0        0     1070 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microchip.svg
+-rw-r--r--   0        0        0     1100 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-alt-slash.svg
+-rw-r--r--   0        0        0      920 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-alt.svg
+-rw-r--r--   0        0        0      948 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-slash.svg
+-rw-r--r--   0        0        0      723 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone.svg
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/microscope.svg
+-rw-r--r--   0        0        0      430 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/minus-circle.svg
+-rw-r--r--   0        0        0      464 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/minus-square.svg
+-rw-r--r--   0        0        0      376 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/minus.svg
+-rw-r--r--   0        0        0      526 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mitten.svg
+-rw-r--r--   0        0        0      536 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mobile-alt.svg
+-rw-r--r--   0        0        0      436 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mobile.svg
+-rw-r--r--   0        0        0      871 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-alt.svg
+-rw-r--r--   0        0        0      763 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-wave-alt.svg
+-rw-r--r--   0        0        0     1097 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-wave.svg
+-rw-r--r--   0        0        0      617 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill.svg
+-rw-r--r--   0        0        0     1317 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-check-alt.svg
+-rw-r--r--   0        0        0      781 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-check.svg
+-rw-r--r--   0        0        0      654 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/monument.svg
+-rw-r--r--   0        0        0      563 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/moon.svg
+-rw-r--r--   0        0        0      686 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mortar-pestle.svg
+-rw-r--r--   0        0        0      867 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mosque.svg
+-rw-r--r--   0        0        0     1271 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/motorcycle.svg
+-rw-r--r--   0        0        0      521 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mountain.svg
+-rw-r--r--   0        0        0      546 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mouse-pointer.svg
+-rw-r--r--   0        0        0      400 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mouse.svg
+-rw-r--r--   0        0        0      889 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/mug-hot.svg
+-rw-r--r--   0        0        0      504 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/music.svg
+-rw-r--r--   0        0        0      802 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/network-wired.svg
+-rw-r--r--   0        0        0      487 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/neuter.svg
+-rw-r--r--   0        0        0     1028 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/newspaper.svg
+-rw-r--r--   0        0        0      726 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/not-equal.svg
+-rw-r--r--   0        0        0      746 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/notes-medical.svg
+-rw-r--r--   0        0        0      859 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/object-group.svg
+-rw-r--r--   0        0        0      790 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/object-ungroup.svg
+-rw-r--r--   0        0        0      847 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/oil-can.svg
+-rw-r--r--   0        0        0     1600 2023-08-29 11:20:58.198933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/om.svg
+-rw-r--r--   0        0        0      934 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/otter.svg
+-rw-r--r--   0        0        0      857 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/outdent.svg
+-rw-r--r--   0        0        0      557 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pager.svg
+-rw-r--r--   0        0        0      705 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paint-brush.svg
+-rw-r--r--   0        0        0      599 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paint-roller.svg
+-rw-r--r--   0        0        0      741 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/palette.svg
+-rw-r--r--   0        0        0      634 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pallet.svg
+-rw-r--r--   0        0        0      473 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paper-plane.svg
+-rw-r--r--   0        0        0     1046 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paperclip.svg
+-rw-r--r--   0        0        0      694 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/parachute-box.svg
+-rw-r--r--   0        0        0      438 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paragraph.svg
+-rw-r--r--   0        0        0      539 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/parking.svg
+-rw-r--r--   0        0        0     1068 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/passport.svg
+-rw-r--r--   0        0        0     2295 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pastafarianism.svg
+-rw-r--r--   0        0        0      762 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paste.svg
+-rw-r--r--   0        0        0      529 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pause-circle.svg
+-rw-r--r--   0        0        0      474 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pause.svg
+-rw-r--r--   0        0        0     1047 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/paw.svg
+-rw-r--r--   0        0        0      654 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/peace.svg
+-rw-r--r--   0        0        0      705 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-alt.svg
+-rw-r--r--   0        0        0      635 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-fancy.svg
+-rw-r--r--   0        0        0      673 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-nib.svg
+-rw-r--r--   0        0        0      649 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-square.svg
+-rw-r--r--   0        0        0      504 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen.svg
+-rw-r--r--   0        0        0      725 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pencil-alt.svg
+-rw-r--r--   0        0        0      960 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pencil-ruler.svg
+-rw-r--r--   0        0        0     1020 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/people-arrows.svg
+-rw-r--r--   0        0        0     1408 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/people-carry.svg
+-rw-r--r--   0        0        0      682 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pepper-hot.svg
+-rw-r--r--   0        0        0      718 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/percent.svg
+-rw-r--r--   0        0        0      714 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/percentage.svg
+-rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/person-booth.svg
+-rw-r--r--   0        0        0      524 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-alt.svg
+-rw-r--r--   0        0        0      774 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-slash.svg
+-rw-r--r--   0        0        0      720 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-square-alt.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-square.svg
+-rw-r--r--   0        0        0     1425 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-volume.svg
+-rw-r--r--   0        0        0      541 2023-08-29 11:20:58.199933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone.svg
+-rw-r--r--   0        0        0      830 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/photo-video.svg
+-rw-r--r--   0        0        0      940 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/piggy-bank.svg
+-rw-r--r--   0        0        0      682 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pills.svg
+-rw-r--r--   0        0        0      672 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pizza-slice.svg
+-rw-r--r--   0        0        0      702 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/place-of-worship.svg
+-rw-r--r--   0        0        0      825 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-arrival.svg
+-rw-r--r--   0        0        0      833 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-departure.svg
+-rw-r--r--   0        0        0      770 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-slash.svg
+-rw-r--r--   0        0        0      673 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane.svg
+-rw-r--r--   0        0        0      437 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/play-circle.svg
+-rw-r--r--   0        0        0      371 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/play.svg
+-rw-r--r--   0        0        0      498 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plug.svg
+-rw-r--r--   0        0        0      534 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plus-circle.svg
+-rw-r--r--   0        0        0      569 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plus-square.svg
+-rw-r--r--   0        0        0      499 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/plus.svg
+-rw-r--r--   0        0        0     1573 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/podcast.svg
+-rw-r--r--   0        0        0      686 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/poll-h.svg
+-rw-r--r--   0        0        0      685 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/poll.svg
+-rw-r--r--   0        0        0      947 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/poo-storm.svg
+-rw-r--r--   0        0        0      939 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/poo.svg
+-rw-r--r--   0        0        0      759 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/poop.svg
+-rw-r--r--   0        0        0      611 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/portrait.svg
+-rw-r--r--   0        0        0      784 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pound-sign.svg
+-rw-r--r--   0        0        0      723 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/power-off.svg
+-rw-r--r--   0        0        0      730 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pray.svg
+-rw-r--r--   0        0        0     1121 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/praying-hands.svg
+-rw-r--r--   0        0        0      607 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription-bottle-alt.svg
+-rw-r--r--   0        0        0      561 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription-bottle.svg
+-rw-r--r--   0        0        0      768 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription.svg
+-rw-r--r--   0        0        0      697 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/print.svg
+-rw-r--r--   0        0        0      776 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/procedures.svg
+-rw-r--r--   0        0        0      659 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/project-diagram.svg
+-rw-r--r--   0        0        0      883 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pump-medical.svg
+-rw-r--r--   0        0        0      709 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/pump-soap.svg
+-rw-r--r--   0        0        0      904 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/puzzle-piece.svg
+-rw-r--r--   0        0        0      479 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/qrcode.svg
+-rw-r--r--   0        0        0      882 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/question-circle.svg
+-rw-r--r--   0        0        0      840 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/question.svg
+-rw-r--r--   0        0        0      763 2023-08-29 11:20:58.200933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/quidditch.svg
+-rw-r--r--   0        0        0      631 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/quote-left.svg
+-rw-r--r--   0        0        0      627 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/quote-right.svg
+-rw-r--r--   0        0        0     1185 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/quran.svg
+-rw-r--r--   0        0        0      925 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/radiation-alt.svg
+-rw-r--r--   0        0        0      804 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/radiation.svg
+-rw-r--r--   0        0        0      917 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/rainbow.svg
+-rw-r--r--   0        0        0      932 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/random.svg
+-rw-r--r--   0        0        0      824 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/receipt.svg
+-rw-r--r--   0        0        0      476 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/record-vinyl.svg
+-rw-r--r--   0        0        0     1390 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/recycle.svg
+-rw-r--r--   0        0        0      805 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/redo-alt.svg
+-rw-r--r--   0        0        0      602 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/redo.svg
+-rw-r--r--   0        0        0      802 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/registered.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/remove-format.svg
+-rw-r--r--   0        0        0      848 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/reply-all.svg
+-rw-r--r--   0        0        0      581 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/reply.svg
+-rw-r--r--   0        0        0     1257 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/republican.svg
+-rw-r--r--   0        0        0      987 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/restroom.svg
+-rw-r--r--   0        0        0     1075 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/retweet.svg
+-rw-r--r--   0        0        0      718 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ribbon.svg
+-rw-r--r--   0        0        0      687 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ring.svg
+-rw-r--r--   0        0        0      949 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/road.svg
+-rw-r--r--   0        0        0      756 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/robot.svg
+-rw-r--r--   0        0        0     1033 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/rocket.svg
+-rw-r--r--   0        0        0      735 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/route.svg
+-rw-r--r--   0        0        0      968 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/rss-square.svg
+-rw-r--r--   0        0        0      903 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/rss.svg
+-rw-r--r--   0        0        0      711 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruble-sign.svg
+-rw-r--r--   0        0        0      776 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-combined.svg
+-rw-r--r--   0        0        0      636 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-horizontal.svg
+-rw-r--r--   0        0        0      581 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-vertical.svg
+-rw-r--r--   0        0        0      864 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler.svg
+-rw-r--r--   0        0        0     1067 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/running.svg
+-rw-r--r--   0        0        0      832 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/rupee-sign.svg
+-rw-r--r--   0        0        0      955 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sad-cry.svg
+-rw-r--r--   0        0        0      719 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sad-tear.svg
+-rw-r--r--   0        0        0     1281 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/satellite-dish.svg
+-rw-r--r--   0        0        0     1245 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/satellite.svg
+-rw-r--r--   0        0        0      701 2023-08-29 11:20:58.201933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/save.svg
+-rw-r--r--   0        0        0      787 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/school.svg
+-rw-r--r--   0        0        0      550 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/screwdriver.svg
+-rw-r--r--   0        0        0      581 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/scroll.svg
+-rw-r--r--   0        0        0      411 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sd-card.svg
+-rw-r--r--   0        0        0     1349 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-dollar.svg
+-rw-r--r--   0        0        0      943 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-location.svg
+-rw-r--r--   0        0        0      685 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-minus.svg
+-rw-r--r--   0        0        0      789 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-plus.svg
+-rw-r--r--   0        0        0      605 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/search.svg
+-rw-r--r--   0        0        0      468 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/seedling.svg
+-rw-r--r--   0        0        0     1120 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/server.svg
+-rw-r--r--   0        0        0      552 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shapes.svg
+-rw-r--r--   0        0        0      851 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-alt-square.svg
+-rw-r--r--   0        0        0      716 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-alt.svg
+-rw-r--r--   0        0        0      919 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-square.svg
+-rw-r--r--   0        0        0      577 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/share.svg
+-rw-r--r--   0        0        0      650 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shekel-sign.svg
+-rw-r--r--   0        0        0      519 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shield-alt.svg
+-rw-r--r--   0        0        0     1145 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shield-virus.svg
+-rw-r--r--   0        0        0      957 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ship.svg
+-rw-r--r--   0        0        0      921 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shipping-fast.svg
+-rw-r--r--   0        0        0      799 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shoe-prints.svg
+-rw-r--r--   0        0        0      618 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-bag.svg
+-rw-r--r--   0        0        0     1022 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-basket.svg
+-rw-r--r--   0        0        0      796 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-cart.svg
+-rw-r--r--   0        0        0     1396 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shower.svg
+-rw-r--r--   0        0        0      739 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/shuttle-van.svg
+-rw-r--r--   0        0        0      596 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-in-alt.svg
+-rw-r--r--   0        0        0     1687 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-language.svg
+-rw-r--r--   0        0        0      600 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-out-alt.svg
+-rw-r--r--   0        0        0      486 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign.svg
+-rw-r--r--   0        0        0      798 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/signal.svg
+-rw-r--r--   0        0        0      822 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/signature.svg
+-rw-r--r--   0        0        0      579 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sim-card.svg
+-rw-r--r--   0        0        0      698 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sink.svg
+-rw-r--r--   0        0        0      842 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sitemap.svg
+-rw-r--r--   0        0        0     1066 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/skating.svg
+-rw-r--r--   0        0        0     1019 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/skiing-nordic.svg
+-rw-r--r--   0        0        0     1010 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/skiing.svg
+-rw-r--r--   0        0        0     1034 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/skull-crossbones.svg
+-rw-r--r--   0        0        0      738 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/skull.svg
+-rw-r--r--   0        0        0      451 2023-08-29 11:20:58.202933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/slash.svg
+-rw-r--r--   0        0        0      747 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sleigh.svg
+-rw-r--r--   0        0        0      869 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sliders-h.svg
+-rw-r--r--   0        0        0      846 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile-beam.svg
+-rw-r--r--   0        0        0      729 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile-wink.svg
+-rw-r--r--   0        0        0      646 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile.svg
+-rw-r--r--   0        0        0      793 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smog.svg
+-rw-r--r--   0        0        0      918 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smoking-ban.svg
+-rw-r--r--   0        0        0      988 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/smoking.svg
+-rw-r--r--   0        0        0     1379 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sms.svg
+-rw-r--r--   0        0        0     1183 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowboarding.svg
+-rw-r--r--   0        0        0     1737 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowflake.svg
+-rw-r--r--   0        0        0     1383 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowman.svg
+-rw-r--r--   0        0        0     1209 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowplow.svg
+-rw-r--r--   0        0        0      649 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/soap.svg
+-rw-r--r--   0        0        0      800 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/socks.svg
+-rw-r--r--   0        0        0      934 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/solar-panel.svg
+-rw-r--r--   0        0        0      882 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-down-alt.svg
+-rw-r--r--   0        0        0      879 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-down.svg
+-rw-r--r--   0        0        0      877 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-up-alt.svg
+-rw-r--r--   0        0        0      876 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-up.svg
+-rw-r--r--   0        0        0      797 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-down-alt.svg
+-rw-r--r--   0        0        0      801 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-down.svg
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-up-alt.svg
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-up.svg
+-rw-r--r--   0        0        0      359 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-down.svg
+-rw-r--r--   0        0        0      889 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-down-alt.svg
+-rw-r--r--   0        0        0      886 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-down.svg
+-rw-r--r--   0        0        0      885 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-up-alt.svg
+-rw-r--r--   0        0        0      883 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-up.svg
+-rw-r--r--   0        0        0      360 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-up.svg
+-rw-r--r--   0        0        0      458 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort.svg
+-rw-r--r--   0        0        0      844 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/spa.svg
+-rw-r--r--   0        0        0      840 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/space-shuttle.svg
+-rw-r--r--   0        0        0      928 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/spell-check.svg
+-rw-r--r--   0        0        0     1718 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/spider.svg
+-rw-r--r--   0        0        0      838 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/spinner.svg
+-rw-r--r--   0        0        0      745 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/splotch.svg
+-rw-r--r--   0        0        0      984 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/spray-can.svg
+-rw-r--r--   0        0        0      281 2023-08-29 11:20:58.203933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/square-full.svg
+-rw-r--r--   0        0        0      953 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/square-root-alt.svg
+-rw-r--r--   0        0        0      365 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/square.svg
+-rw-r--r--   0        0        0      672 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stamp.svg
+-rw-r--r--   0        0        0      973 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-and-crescent.svg
+-rw-r--r--   0        0        0      802 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-half-alt.svg
+-rw-r--r--   0        0        0      402 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-half.svg
+-rw-r--r--   0        0        0      912 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-of-david.svg
+-rw-r--r--   0        0        0      820 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-of-life.svg
+-rw-r--r--   0        0        0      516 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/star.svg
+-rw-r--r--   0        0        0      442 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/step-backward.svg
+-rw-r--r--   0        0        0      443 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/step-forward.svg
+-rw-r--r--   0        0        0      888 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stethoscope.svg
+-rw-r--r--   0        0        0      447 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sticky-note.svg
+-rw-r--r--   0        0        0      430 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stop-circle.svg
+-rw-r--r--   0        0        0      365 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stop.svg
+-rw-r--r--   0        0        0     1328 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stopwatch-20.svg
+-rw-r--r--   0        0        0      682 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stopwatch.svg
+-rw-r--r--   0        0        0      705 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-alt-slash.svg
+-rw-r--r--   0        0        0      554 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-alt.svg
+-rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-slash.svg
+-rw-r--r--   0        0        0      825 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/store.svg
+-rw-r--r--   0        0        0      580 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stream.svg
+-rw-r--r--   0        0        0      852 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/street-view.svg
+-rw-r--r--   0        0        0      848 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/strikethrough.svg
+-rw-r--r--   0        0        0     2664 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/stroopwafel.svg
+-rw-r--r--   0        0        0      800 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/subscript.svg
+-rw-r--r--   0        0        0      880 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/subway.svg
+-rw-r--r--   0        0        0      756 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/suitcase-rolling.svg
+-rw-r--r--   0        0        0      479 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/suitcase.svg
+-rw-r--r--   0        0        0      847 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sun.svg
+-rw-r--r--   0        0        0      798 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/superscript.svg
+-rw-r--r--   0        0        0      546 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/surprise.svg
+-rw-r--r--   0        0        0      631 2023-08-29 11:20:58.204933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/swatchbook.svg
+-rw-r--r--   0        0        0     1494 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/swimmer.svg
+-rw-r--r--   0        0        0     1345 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/swimming-pool.svg
+-rw-r--r--   0        0        0      966 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/synagogue.svg
+-rw-r--r--   0        0        0     1022 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sync-alt.svg
+-rw-r--r--   0        0        0      887 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/sync.svg
+-rw-r--r--   0        0        0      970 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/syringe.svg
+-rw-r--r--   0        0        0      674 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/table-tennis.svg
+-rw-r--r--   0        0        0      463 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/table.svg
+-rw-r--r--   0        0        0      536 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tablet-alt.svg
+-rw-r--r--   0        0        0      436 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tablet.svg
+-rw-r--r--   0        0        0      746 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tablets.svg
+-rw-r--r--   0        0        0     1197 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tachometer-alt.svg
+-rw-r--r--   0        0        0      550 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tag.svg
+-rw-r--r--   0        0        0      810 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tags.svg
+-rw-r--r--   0        0        0      544 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tape.svg
+-rw-r--r--   0        0        0      966 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tasks.svg
+-rw-r--r--   0        0        0      923 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/taxi.svg
+-rw-r--r--   0        0        0     1275 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/teeth-open.svg
+-rw-r--r--   0        0        0     1166 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/teeth.svg
+-rw-r--r--   0        0        0      833 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/temperature-high.svg
+-rw-r--r--   0        0        0      832 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/temperature-low.svg
+-rw-r--r--   0        0        0      509 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tenge.svg
+-rw-r--r--   0        0        0      661 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/terminal.svg
+-rw-r--r--   0        0        0      723 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/text-height.svg
+-rw-r--r--   0        0        0      723 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/text-width.svg
+-rw-r--r--   0        0        0      753 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/th-large.svg
+-rw-r--r--   0        0        0     1030 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/th-list.svg
+-rw-r--r--   0        0        0     1455 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/th.svg
+-rw-r--r--   0        0        0     1803 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/theater-masks.svg
+-rw-r--r--   0        0        0      786 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-empty.svg
+-rw-r--r--   0        0        0      860 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-full.svg
+-rw-r--r--   0        0        0      865 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-half.svg
+-rw-r--r--   0        0        0      864 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-quarter.svg
+-rw-r--r--   0        0        0      873 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-three-quarters.svg
+-rw-r--r--   0        0        0      688 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer.svg
+-rw-r--r--   0        0        0     1059 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbs-down.svg
+-rw-r--r--   0        0        0     1066 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbs-up.svg
+-rw-r--r--   0        0        0      666 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbtack.svg
+-rw-r--r--   0        0        0      619 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/ticket-alt.svg
+-rw-r--r--   0        0        0      635 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/times-circle.svg
+-rw-r--r--   0        0        0      675 2023-08-29 11:20:58.205933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/times.svg
+-rw-r--r--   0        0        0      720 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tint-slash.svg
+-rw-r--r--   0        0        0      552 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tint.svg
+-rw-r--r--   0        0        0      740 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tired.svg
+-rw-r--r--   0        0        0      598 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toggle-off.svg
+-rw-r--r--   0        0        0      448 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toggle-on.svg
+-rw-r--r--   0        0        0      851 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet-paper-slash.svg
+-rw-r--r--   0        0        0      907 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet-paper.svg
+-rw-r--r--   0        0        0      730 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet.svg
+-rw-r--r--   0        0        0      813 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/toolbox.svg
+-rw-r--r--   0        0        0      951 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tools.svg
+-rw-r--r--   0        0        0      971 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tooth.svg
+-rw-r--r--   0        0        0     1122 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/torah.svg
+-rw-r--r--   0        0        0      656 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/torii-gate.svg
+-rw-r--r--   0        0        0     1466 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tractor.svg
+-rw-r--r--   0        0        0      914 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trademark.svg
+-rw-r--r--   0        0        0      829 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/traffic-light.svg
+-rw-r--r--   0        0        0      863 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trailer.svg
+-rw-r--r--   0        0        0      685 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/train.svg
+-rw-r--r--   0        0        0      752 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tram.svg
+-rw-r--r--   0        0        0     1055 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/transgender-alt.svg
+-rw-r--r--   0        0        0      745 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/transgender.svg
+-rw-r--r--   0        0        0      619 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-alt.svg
+-rw-r--r--   0        0        0      668 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-restore-alt.svg
+-rw-r--r--   0        0        0      680 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-restore.svg
+-rw-r--r--   0        0        0      494 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash.svg
+-rw-r--r--   0        0        0      885 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tree.svg
+-rw-r--r--   0        0        0      840 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/trophy.svg
+-rw-r--r--   0        0        0      714 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-loading.svg
+-rw-r--r--   0        0        0     2510 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-monster.svg
+-rw-r--r--   0        0        0      892 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-moving.svg
+-rw-r--r--   0        0        0      899 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-pickup.svg
+-rw-r--r--   0        0        0      704 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck.svg
+-rw-r--r--   0        0        0      580 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tshirt.svg
+-rw-r--r--   0        0        0     2005 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tty.svg
+-rw-r--r--   0        0        0      473 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/tv.svg
+-rw-r--r--   0        0        0      849 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/umbrella-beach.svg
+-rw-r--r--   0        0        0      819 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/umbrella.svg
+-rw-r--r--   0        0        0      613 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/underline.svg
+-rw-r--r--   0        0        0      804 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/undo-alt.svg
+-rw-r--r--   0        0        0      799 2023-08-29 11:20:58.206933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/undo.svg
+-rw-r--r--   0        0        0     1249 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/universal-access.svg
+-rw-r--r--   0        0        0      666 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/university.svg
+-rw-r--r--   0        0        0     1254 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlink.svg
+-rw-r--r--   0        0        0      622 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlock-alt.svg
+-rw-r--r--   0        0        0      535 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlock.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/upload.svg
+-rw-r--r--   0        0        0      584 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-alt-slash.svg
+-rw-r--r--   0        0        0      504 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-alt.svg
+-rw-r--r--   0        0        0      967 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-astronaut.svg
+-rw-r--r--   0        0        0      718 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-check.svg
+-rw-r--r--   0        0        0      614 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-circle.svg
+-rw-r--r--   0        0        0      778 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-clock.svg
+-rw-r--r--   0        0        0     1562 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-cog.svg
+-rw-r--r--   0        0        0      752 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-edit.svg
+-rw-r--r--   0        0        0      763 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-friends.svg
+-rw-r--r--   0        0        0      799 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-graduate.svg
+-rw-r--r--   0        0        0      938 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-injured.svg
+-rw-r--r--   0        0        0      695 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-lock.svg
+-rw-r--r--   0        0        0     1037 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-md.svg
+-rw-r--r--   0        0        0      617 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-minus.svg
+-rw-r--r--   0        0        0      665 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-ninja.svg
+-rw-r--r--   0        0        0      785 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-nurse.svg
+-rw-r--r--   0        0        0      721 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-plus.svg
+-rw-r--r--   0        0        0     1094 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-secret.svg
+-rw-r--r--   0        0        0      800 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-shield.svg
+-rw-r--r--   0        0        0      583 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-slash.svg
+-rw-r--r--   0        0        0      848 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-tag.svg
+-rw-r--r--   0        0        0      511 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-tie.svg
+-rw-r--r--   0        0        0      846 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-times.svg
+-rw-r--r--   0        0        0      516 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/user.svg
+-rw-r--r--   0        0        0     1816 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/users-cog.svg
+-rw-r--r--   0        0        0     1042 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/users-slash.svg
+-rw-r--r--   0        0        0      904 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/users.svg
+-rw-r--r--   0        0        0      477 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/utensil-spoon.svg
+-rw-r--r--   0        0        0      764 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/utensils.svg
+-rw-r--r--   0        0        0      812 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vector-square.svg
+-rw-r--r--   0        0        0     1005 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus-double.svg
+-rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus-mars.svg
+-rw-r--r--   0        0        0      589 2023-08-29 11:20:58.207933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus.svg
+-rw-r--r--   0        0        0     1201 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vest-patches.svg
+-rw-r--r--   0        0        0      908 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vest.svg
+-rw-r--r--   0        0        0      556 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vial.svg
+-rw-r--r--   0        0        0      656 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vials.svg
+-rw-r--r--   0        0        0      635 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/video-slash.svg
+-rw-r--r--   0        0        0      496 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/video.svg
+-rw-r--r--   0        0        0      861 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vihara.svg
+-rw-r--r--   0        0        0     1234 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/virus-slash.svg
+-rw-r--r--   0        0        0      982 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/virus.svg
+-rw-r--r--   0        0        0     1608 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/viruses.svg
+-rw-r--r--   0        0        0      435 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/voicemail.svg
+-rw-r--r--   0        0        0     1015 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/volleyball-ball.svg
+-rw-r--r--   0        0        0      697 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-down.svg
+-rw-r--r--   0        0        0      799 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-mute.svg
+-rw-r--r--   0        0        0      376 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-off.svg
+-rw-r--r--   0        0        0     1238 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-up.svg
+-rw-r--r--   0        0        0      743 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vote-yea.svg
+-rw-r--r--   0        0        0      682 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/vr-cardboard.svg
+-rw-r--r--   0        0        0     1041 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/walking.svg
+-rw-r--r--   0        0        0      550 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wallet.svg
+-rw-r--r--   0        0        0      789 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/warehouse.svg
+-rw-r--r--   0        0        0     1517 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/water.svg
+-rw-r--r--   0        0        0      508 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wave-square.svg
+-rw-r--r--   0        0        0      627 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/weight-hanging.svg
+-rw-r--r--   0        0        0      769 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/weight.svg
+-rw-r--r--   0        0        0     1033 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wheelchair.svg
+-rw-r--r--   0        0        0      795 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wifi.svg
+-rw-r--r--   0        0        0     1086 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wind.svg
+-rw-r--r--   0        0        0      697 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-close.svg
+-rw-r--r--   0        0        0      426 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-maximize.svg
+-rw-r--r--   0        0        0      368 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-minimize.svg
+-rw-r--r--   0        0        0      545 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-restore.svg
+-rw-r--r--   0        0        0      702 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-bottle.svg
+-rw-r--r--   0        0        0      575 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-glass-alt.svg
+-rw-r--r--   0        0        0      537 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-glass.svg
+-rw-r--r--   0        0        0     1152 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/won-sign.svg
+-rw-r--r--   0        0        0      713 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/wrench.svg
+-rw-r--r--   0        0        0     1054 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/x-ray.svg
+-rw-r--r--   0        0        0      762 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/yen-sign.svg
+-rw-r--r--   0        0        0      626 2023-08-29 11:20:58.208933 pyedifice-0.5.4/edifice/icons/font-awesome/solid/yin-yang.svg
+-rw-r--r--   0        0        0        0 2023-08-29 11:20:58.209933 pyedifice-0.5.4/edifice/inspector/__init__.py
+-rw-r--r--   0        0        0     2304 2023-08-29 11:20:58.209933 pyedifice-0.5.4/edifice/inspector/icon.png
+-rw-r--r--   0        0        0     7234 2024-04-11 04:19:58.679589 pyedifice-0.5.4/edifice/inspector/inspector.py
+-rw-r--r--   0        0        0     1743 2024-04-11 04:19:58.679589 pyedifice-0.5.4/edifice/logger.py
+-rw-r--r--   0        0        0       72 2023-09-12 12:13:41.458375 pyedifice-0.5.4/edifice/qt/__init__.py
+-rw-r--r--   0        0        0     6806 2024-04-11 04:19:58.679589 pyedifice-0.5.4/edifice/runner.py
+-rw-r--r--   0        0        0     2565 2024-04-11 04:19:58.679589 pyedifice-0.5.4/edifice/utilities.py
+-rw-r--r--   0        0        0     1592 2024-04-29 07:01:10.676758 pyedifice-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     8924 1970-01-01 00:00:00.000000 pyedifice-0.5.4/PKG-INFO
```

### Comparing `pyedifice-0.5.3/LICENSE` & `pyedifice-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/README.md` & `pyedifice-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/__init__.py` & `pyedifice-0.5.4/edifice/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/app.py` & `pyedifice-0.5.4/edifice/app.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/base_components/__init__.py` & `pyedifice-0.5.4/edifice/base_components/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/base_components/base_components.py` & `pyedifice-0.5.4/edifice/base_components/base_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import importlib.resources
 import logging
 import re
 import typing as tp
 from ..engine import (
     _WidgetTree,
     _get_widget_children,
-    _CommandType,
+    CommandType,
     PropsDict,
     Element,
     QtWidgetElement,
     _create_qmenu,
     _CURSORS,
     _ensure_future,
 )
@@ -104,16 +104,16 @@
         assert self.underlying is not None
         if len(children) != 1:
             raise ValueError("GroupBox expects exactly 1 child, got %s" % len(children))
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         child_underlying = children[0].underlying
         assert child_underlying is not None
         widget = tp.cast(QtWidgets.QGroupBox, self.underlying)
-        commands.append(_CommandType(child_underlying.setParent, self.underlying))
-        commands.append(_CommandType(widget.setTitle, self.props.title))
+        commands.append(CommandType(child_underlying.setParent, self.underlying))
+        commands.append(CommandType(widget.setTitle, self.props.title))
         return commands
 
 
 class Icon(QtWidgetElement):
     """Display an Icon.
 
     * Underlying Qt Widget
@@ -203,15 +203,15 @@
             or "size" in newprops
             or "collection" in newprops
             or "sub_collection" in newprops
             or "color" in newprops
             or "rotation" in newprops
         ):
             commands.append(
-                _CommandType(self._render_image, icon_path, self.props.size, self.props.color, self.props.rotation)
+                CommandType(self._render_image, icon_path, self.props.size, self.props.color, self.props.rotation)
             )
 
         return commands
 
 
 class Button(QtWidgetElement):
     """Basic button widget.
@@ -253,15 +253,15 @@
         assert self.underlying is not None
         size = self.underlying.font().pointSize()
         self._set_size(size * len(self.props.title), size, lambda size: (size * len(self.props.title), size))
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         widget = tp.cast(QtWidgets.QPushButton, self.underlying)
         for prop in newprops:
             if prop == "title":
-                commands.append(_CommandType(widget.setText, str(newprops.title)))
+                commands.append(CommandType(widget.setText, str(newprops.title)))
 
         return commands
 
 
 class IconButton(Button):
     """Display an Icon Button.
 
@@ -346,15 +346,15 @@
             or "size" in newprops
             or "collection" in newprops
             or "sub_collection" in newprops
             or "color" in newprops
             or "rotation" in newprops
         ):
             commands.append(
-                _CommandType(render_image, icon_path, self.props.size, self.props.color, self.props.rotation)
+                CommandType(render_image, icon_path, self.props.size, self.props.color, self.props.rotation)
             )
 
         return commands
 
 
 class Label(QtWidgetElement):
     """Basic widget for displaying text.
@@ -417,19 +417,19 @@
         # https://github.com/pyedifice/pyedifice/issues/41
         # https://stackoverflow.com/questions/48665788/qlabels-getting-clipped-off-at-the-end/48665900#48665900
 
         widget = tp.cast(QtWidgets.QLabel, self.underlying)
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying, None)
         for prop in newprops:
             if prop == "text":
-                commands.append(_CommandType(widget.setText, str(newprops[prop])))
+                commands.append(CommandType(widget.setText, str(newprops[prop])))
             elif prop == "word_wrap":
-                commands.append(_CommandType(widget.setWordWrap, self.props.word_wrap))
+                commands.append(CommandType(widget.setWordWrap, self.props.word_wrap))
             elif prop == "link_open":
-                commands.append(_CommandType(widget.setOpenExternalLinks, self.props.link_open))
+                commands.append(CommandType(widget.setOpenExternalLinks, self.props.link_open))
             elif prop == "selectable" or prop == "editable":
                 interaction_flags = 0
                 change_cursor = False
                 if self.props.selectable:
                     change_cursor = True
                     interaction_flags = (
                         QtCore.Qt.TextInteractionFlag.TextSelectableByMouse
@@ -440,17 +440,17 @@
                     # PyQt5 doesn't support bitwise or with ints
                     # TODO What about PyQt6?
                     if interaction_flags:
                         interaction_flags |= QtCore.Qt.TextInteractionFlag.TextEditable
                     else:
                         interaction_flags = QtCore.Qt.TextInteractionFlag.TextEditable
                 if change_cursor and self.props.cursor is None:
-                    commands.append(_CommandType(widget.setCursor, _CURSORS["text"]))
+                    commands.append(CommandType(widget.setCursor, _CURSORS["text"]))
                 if interaction_flags:
-                    commands.append(_CommandType(widget.setTextInteractionFlags, interaction_flags))
+                    commands.append(CommandType(widget.setTextInteractionFlags, interaction_flags))
         return commands
 
 
 class ImageSvg(QtWidgetElement):
     """An SVG Image container.
 
     * Underlying Qt Widget
@@ -483,15 +483,15 @@
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(QtSvgWidgets.QSvgWidget, self.underlying)
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying, None)
         for prop in newprops:
             if prop == "src":
-                commands.append(_CommandType(widget.load, self.props.src))
+                commands.append(CommandType(widget.load, self.props.src))
         return commands
 
 
 # TODO
 # It seems to me that the type for Completer should be
 #
 #     Callable[[str], str]
@@ -609,20 +609,20 @@
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QLineEdit, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         if "text" in newprops:
-            commands.append(_CommandType(widget.setText, str(newprops.text)))
+            commands.append(CommandType(widget.setText, str(newprops.text)))
             # This setCursorPosition is needed because otherwise the cursor will
             # jump to the end of the text after the setText.
-            commands.append(_CommandType(widget.setCursorPosition, widget.cursorPosition()))
+            commands.append(CommandType(widget.setCursorPosition, widget.cursorPosition()))
         if "placeholder_text" in newprops:
-            commands.append(_CommandType(widget.setPlaceholderText, newprops.placeholder_text))
+            commands.append(CommandType(widget.setPlaceholderText, newprops.placeholder_text))
         return commands
 
 
 class Dropdown(QtWidgetElement):
     """Basic widget for a dropdown menu.
 
     * Underlying Qt Widget
@@ -646,46 +646,52 @@
             Callback for the value of the text input changes.
             The callback is passed the changed
             value of the text.
             This event is only raised when :code:`editable=True`.
         on_select:
             Callback for when the selection changes.
             The callback is passed the new value of the text.
+        enable_mouse_scroll:
+            Whether mouse scroll events should be able to change the value.
     """
 
     def __init__(
         self,
         selection: tp.Text = "",
         text: tp.Text = "",
         options: tp.Optional[tp.Sequence[tp.Text]] = None,
         editable: bool = False,
         # TODO
         # completer: tp.Optional[Completer] = None,
         on_change: tp.Optional[tp.Callable[[tp.Text], None | tp.Awaitable[None]]] = None,
         on_select: tp.Optional[tp.Callable[[tp.Text], None | tp.Awaitable[None]]] = None,
+        enable_mouse_scroll: bool = True,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self._register_props(
             {
                 "selection": selection,
                 "text": text,
                 "options": options,
                 "editable": editable,
                 "on_change": on_change,
                 "on_select": on_select,
+                "enable_mouse_scroll": enable_mouse_scroll,
             }
         )
         self._register_props(kwargs)
 
     def _initialize(self):
         self.underlying = QtWidgets.QComboBox()
         self.underlying.setObjectName(str(id(self)))
         self.underlying.editTextChanged.connect(self._on_change)
         self.underlying.textActivated.connect(self._on_select)
+        if "enable_mouse_scroll" in self.props and not self.props.enable_mouse_scroll:
+            self.underlying.wheelEvent = lambda e: e.ignore()
 
     # TODO
     # def _set_completer(self, completer):
     #     if completer:
     #         qt_completer = QtWidgets.QCompleter(completer.options)
     #         qt_completer.setCompletionMode(completer.mode)
     #         self.underlying.setCompleter(qt_completer)
@@ -719,28 +725,28 @@
     ):
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QComboBox, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
-        commands.append(_CommandType(widget.setEditable, self.props.editable))
+        commands.append(CommandType(widget.setEditable, self.props.editable))
         if "options" in newprops:
             commands.extend(
                 [
-                    _CommandType(widget.clear),
-                    _CommandType(widget.addItems, newprops.options),
+                    CommandType(widget.clear),
+                    CommandType(widget.addItems, newprops.options),
                 ]
             )
         if "text" in newprops:
-            commands.append(_CommandType(self._set_edit_text, newprops.text))
+            commands.append(CommandType(self._set_edit_text, newprops.text))
         if "selection" in newprops:
-            commands.append(_CommandType(self._set_current_text, newprops.selection))
+            commands.append(CommandType(self._set_current_text, newprops.selection))
         # elif prop == "completer":
-        #     commands.append(_CommandType(self._set_completer, newprops[prop]))
+        #     commands.append(CommandType(self._set_completer, newprops[prop]))
         return commands
 
 
 class RadioButton(QtWidgetElement):
     """Radio buttons.
 
     * Underlying Qt Widget
@@ -808,17 +814,17 @@
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QRadioButton, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         if "checked" in newprops:
-            commands.append(_CommandType(self._set_checked, newprops.checked))
+            commands.append(CommandType(self._set_checked, newprops.checked))
         if "text" in newprops:
-            commands.append(_CommandType(widget.setText, str(newprops.text)))
+            commands.append(CommandType(widget.setText, str(newprops.text)))
         return commands
 
 
 class CheckBox(QtWidgetElement):
     """Checkbox widget.
 
     * Underlying Qt Widget
@@ -889,17 +895,17 @@
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QCheckBox, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         if "text" in newprops:
-            commands.append(_CommandType(widget.setText, str(newprops.text)))
+            commands.append(CommandType(widget.setText, str(newprops.text)))
         if "checked" in newprops:
-            commands.append(_CommandType(self._set_checked, newprops.checked))
+            commands.append(CommandType(self._set_checked, newprops.checked))
         return commands
 
 
 class Slider(QtWidgetElement):
     """Slider bar widget.
 
     * Underlying Qt Widget
@@ -997,21 +1003,21 @@
         if self.underlying is None:
             self._initialize(newprops.orientation)
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QSlider, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         if "min_value" in newprops:
-            commands.append(_CommandType(widget.setMinimum, newprops.min_value))
+            commands.append(CommandType(widget.setMinimum, newprops.min_value))
         if "max_value" in newprops:
-            commands.append(_CommandType(widget.setMaximum, newprops.max_value))
+            commands.append(CommandType(widget.setMaximum, newprops.max_value))
         if "value" in newprops:
-            commands.append(_CommandType(self._set_value, newprops.value))
+            commands.append(CommandType(self._set_value, newprops.value))
         if "on_change" in newprops:
-            commands.append(_CommandType(self._set_on_change, newprops.on_change))
+            commands.append(CommandType(self._set_on_change, newprops.on_change))
         return commands
 
 
 class _LinearView(QtWidgetElement):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._widget_children: list[QtWidgetElement] = []
@@ -1024,15 +1030,15 @@
         Diffing and reconciliation of QtWidgetElements.
         Compute the sequence of commands to transform self._widget_children
         into the new children.
         """
 
         children_new = children
 
-        commands: list[_CommandType] = []
+        commands: list[CommandType] = []
 
         children_old_positioned_reverse: list[QtWidgetElement] = []
         # old children in the same position as new children.
         # In reverse order for speed because popping from the end of a list is
         # faster than popping from the beginning of a list?
 
         # First we delete old children that are not in the right position.
@@ -1054,18 +1060,18 @@
                     # old child is in the same position as new child
                     children_old_positioned_reverse.append(child_old)
                     i_old += 1
                 else:
                     # old child is out of position
                     if child_old in children_new:
                         # child will be added back in later
-                        commands.append(_CommandType(self._soft_delete_child, i_old, child_old))
+                        commands.append(CommandType(self._soft_delete_child, i_old, child_old))
                     else:
                         # child will be deleted
-                        commands.append(_CommandType(self._delete_child, i_old, child_old))
+                        commands.append(CommandType(self._delete_child, i_old, child_old))
                 i_new += 1
 
             r = list(reversed(children_old_positioned_reverse))
             children_old_positioned_reverse = r
 
         # Case 2:
         # Then we iterate backwards pairwise and hope that we get a lot of
@@ -1079,30 +1085,30 @@
                 if i_new > 0 and child_old is children_new[i_new]:
                     # old child is in the same position as new child
                     children_old_positioned_reverse.append(child_old)
                 else:
                     # old child is out of position
                     if child_old in children_new:
                         # child will be added back in later
-                        commands.append(_CommandType(self._soft_delete_child, i_old, child_old))
+                        commands.append(CommandType(self._soft_delete_child, i_old, child_old))
                     else:
                         # child will be deleted
-                        commands.append(_CommandType(self._delete_child, i_old, child_old))
+                        commands.append(CommandType(self._delete_child, i_old, child_old))
                 i_new -= 1
 
         # Now we have deleted all the old children that are not in the right position.
         # Add in the missing new children.
         for i, child_new in enumerate(children_new):
             if len(children_old_positioned_reverse) > 0 and child_new is children_old_positioned_reverse[-1]:
                 # if child is already in the right position
                 del children_old_positioned_reverse[-1]
             else:
                 assert isinstance(child_new, QtWidgetElement)
                 assert child_new.underlying is not None
-                commands.append(_CommandType(self._add_child, i, child_new.underlying))
+                commands.append(CommandType(self._add_child, i, child_new.underlying))
 
         # assert sanity check that we used all the old children.
         assert len(children_old_positioned_reverse) == 0
         self._widget_children = children_new
         return commands
 
     def _add_child(self, i, child_component: QtWidgets.QWidget):
@@ -1311,28 +1317,28 @@
     ):
         if self.underlying is None:
             super()._initialize()
             assert isinstance(self.underlying, QtWidgets.QWidget)
             self.underlying.closeEvent = self._handle_close
             self.underlying.show()
 
-        commands: list[_CommandType] = super()._qt_update_commands(widget_trees, newprops)
+        commands: list[CommandType] = super()._qt_update_commands(widget_trees, newprops)
 
         if "title" in newprops:
-            commands.append(_CommandType(self.underlying.setWindowTitle, newprops.title))
+            commands.append(CommandType(self.underlying.setWindowTitle, newprops.title))
         if "on_close" in newprops:
-            commands.append(_CommandType(self._set_on_close, newprops.on_close))
+            commands.append(CommandType(self._set_on_close, newprops.on_close))
         if "icon" in newprops and newprops.icon:
             pixmap = _image_descriptor_to_pixmap(newprops.icon)
-            commands.append(_CommandType(self.underlying.setWindowIcon, QtGui.QIcon(pixmap)))
+            commands.append(CommandType(self.underlying.setWindowIcon, QtGui.QIcon(pixmap)))
         if "menu" in newprops and newprops.menu:
             if self._menu_bar is not None:
                 self._menu_bar.setParent(None)
             self._menu_bar = QtWidgets.QMenuBar()
-            commands.append(_CommandType(self._attach_menubar, self._menu_bar, newprops.menu))
+            commands.append(CommandType(self._attach_menubar, self._menu_bar, newprops.menu))
 
         return commands
 
 
 class ScrollView(_LinearView):
     """Scrollable layout widget for grouping children together.
 
@@ -1579,19 +1585,19 @@
         assert self.underlying is not None
         rows, columns, grid_spec = _layout_str_to_grid_spec(self.props.layout)
         if self.props.key_to_code is None:
             code_to_child = {c._key[0]: c for c in children}
         else:
             code_to_child = {self.props.key_to_code[c._key]: c for c in children}
         grid_spec = [(code_to_child[cell[0]],) + cell[1:] for cell in grid_spec if cell[0] not in " _"]
-        commands: list[_CommandType] = []
+        commands: list[CommandType] = []
         if grid_spec != self._previously_rendered:
-            commands.append(_CommandType(self._clear))
+            commands.append(CommandType(self._clear))
             for child, y, x, dy, dx in grid_spec:
-                commands.append(_CommandType(self.underlying_layout.addWidget, child.underlying, y, x, dy, dx))
+                commands.append(CommandType(self.underlying_layout.addWidget, child.underlying, y, x, dy, dx))
             self._previously_rendered = grid_spec
         commands.extend(super()._qt_update_commands_super(widget_trees, newprops, self.underlying, None))
         return commands
 
 
 class TabView(_LinearView):
     """Widget with multiple tabs.
@@ -1693,15 +1699,15 @@
         self,
         widget_trees: dict[Element, _WidgetTree],
         newprops: PropsDict,
     ):
         if self.underlying is None:
             self.underlying = self.create_widget()
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying, None)
-        commands.append(_CommandType(self.paint, self.underlying, newprops))
+        commands.append(CommandType(self.paint, self.underlying, newprops))
         return commands
 
 
 class ExportList(QtWidgetElement):
     """
     The root element for an App which does :func:`App.export_widgets`.
     """
@@ -1745,49 +1751,49 @@
 #     def _qt_update_commands(self, children, newprops, newstate):
 #         assert self.underlying is not None
 #         commands = super()._qt_update_commands(children, newprops, newstate, self.underlying, None)
 #         widget = tp.cast(QtWidgets.QTableWidget, self.underlying)
 #
 #         for prop in newprops:
 #             if prop == "rows":
-#                 commands.append(_CommandType(widget.setRowCount, newprops[prop]))
+#                 commands.append(CommandType(widget.setRowCount, newprops[prop]))
 #             elif prop == "columns":
-#                 commands.append(_CommandType(widget.setColumnCount, newprops[prop]))
+#                 commands.append(CommandType(widget.setColumnCount, newprops[prop]))
 #             elif prop == "alternating_row_colors":
-#                 commands.append(_CommandType(widget.setAlternatingRowColors, newprops[prop]))
+#                 commands.append(CommandType(widget.setAlternatingRowColors, newprops[prop]))
 #             elif prop == "row_headers":
 #                 if newprops[prop] is not None:
-#                     commands.append(_CommandType(widget.setVerticalHeaderLabels, list(map(str, newprops[prop]))))
+#                     commands.append(CommandType(widget.setVerticalHeaderLabels, list(map(str, newprops[prop]))))
 #                 else:
-#                     commands.append(_CommandType(widget.setVerticalHeaderLabels, list(map(str, range(newprops.rows)))))
+#                     commands.append(CommandType(widget.setVerticalHeaderLabels, list(map(str, range(newprops.rows)))))
 #             elif prop == "column_headers":
 #                 if newprops[prop] is not None:
-#                     commands.append(_CommandType(widget.setHorizontalHeaderLabels, list(map(str, newprops[prop]))))
+#                     commands.append(CommandType(widget.setHorizontalHeaderLabels, list(map(str, newprops[prop]))))
 #                 else:
-#                     commands.append(_CommandType(widget.setHorizontalHeaderLabels, list(map(str, range(newprops.columns)))))
+#                     commands.append(CommandType(widget.setHorizontalHeaderLabels, list(map(str, range(newprops.columns)))))
 #
 #         new_children = set()
 #         for child in children:
 #             new_children.add(child.component)
 #
 #         for child in list(self._already_rendered.keys()):
 #             if child not in new_children:
 #                 del self._already_rendered[child]
 #
 #         for i, old_child in reversed(list(enumerate(self._widget_children))):
 #             if old_child not in new_children:
 #                 for j, el in enumerate(old_child.children):
 #                     if el:
-#                         commands.append(_CommandType(widget.setCellWidget, i, j, QtWidgets.QWidget()))
+#                         commands.append(CommandType(widget.setCellWidget, i, j, QtWidgets.QWidget()))
 #
 #         self._widget_children = [child.component for child in children]
 #         for i, child in enumerate(children):
 #             if child.component not in self._already_rendered:
 #                 for j, el in enumerate(child.children):
-#                     commands.append(_CommandType(widget.setCellWidget, i, j, el.component.underlying))
+#                     commands.append(CommandType(widget.setCellWidget, i, j, el.component.underlying))
 #             self._already_rendered[child.component] = True
 #         return commands
 
 
 class ProgressBar(QtWidgetElement):
     """Progress bar widget.
 
@@ -1853,17 +1859,17 @@
         if self.underlying is None:
             self._initialize(newprops.orientation)
         assert self.underlying is not None
         widget = tp.cast(QtWidgets.QProgressBar, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
         if "orientation" in newprops:
-            commands.append(_CommandType(widget.setOrientation, newprops.orientation))
+            commands.append(CommandType(widget.setOrientation, newprops.orientation))
         if "min_value" in newprops:
-            commands.append(_CommandType(widget.setMinimum, newprops.min_value))
+            commands.append(CommandType(widget.setMinimum, newprops.min_value))
         if "max_value" in newprops:
-            commands.append(_CommandType(widget.setMaximum, newprops.max_value))
+            commands.append(CommandType(widget.setMaximum, newprops.max_value))
         if "format" in newprops:
-            commands.append(_CommandType(widget.setFormat, newprops.format))
+            commands.append(CommandType(widget.setFormat, newprops.format))
         if "value" in newprops:
-            commands.append(_CommandType(widget.setValue, newprops.value))
+            commands.append(CommandType(widget.setValue, newprops.value))
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/base_components/button_view.py` & `pyedifice-0.5.4/edifice/base_components/button_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         from PyQt6.QtGui import QKeyEvent, QMouseEvent
         from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QHBoxLayout
     else:
         from PySide6.QtCore import QSize, Qt
         from PySide6.QtGui import QKeyEvent, QMouseEvent
         from PySide6.QtWidgets import QPushButton, QVBoxLayout, QHBoxLayout
 
-from .base_components import View, _CommandType, QtWidgetElement, Element, _WidgetTree
+from .base_components import View, CommandType, QtWidgetElement, Element, _WidgetTree
 
 
 class _PushButton(QPushButton):
     def __init__(self):
         super().__init__()
 
     # https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QLayout.html#detailed-description
@@ -124,10 +124,10 @@
     ):
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
         commands = super()._qt_update_commands(widget_trees, newprops)
         for prop in newprops:
             if prop == "on_trigger":
-                commands.append(_CommandType(self._set_on_trigger, self.underlying, newprops.on_trigger))
-            commands.append(_CommandType(self.underlying.setCursor, Qt.CursorShape.PointingHandCursor))
+                commands.append(CommandType(self._set_on_trigger, self.underlying, newprops.on_trigger))
+            commands.append(CommandType(self.underlying.setCursor, Qt.CursorShape.PointingHandCursor))
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/base_components/flow_view.py` & `pyedifice-0.5.4/edifice/base_components/flow_view.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/base_components/image_aspect.py` & `pyedifice-0.5.4/edifice/base_components/image_aspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import PyQt6.QtGui as QtGui
     import PyQt6.QtWidgets as QtWidgets
 else:
     import PySide6.QtCore as QtCore
     import PySide6.QtGui as QtGui
     import PySide6.QtWidgets as QtWidgets
 
-from .base_components import QtWidgetElement, _image_descriptor_to_pixmap, _CommandType, Element, _WidgetTree
+from .base_components import QtWidgetElement, _image_descriptor_to_pixmap, CommandType, Element, _WidgetTree
 
 
 class _ScaledLabel(QtWidgets.QLabel):
     """
     https://stackoverflow.com/questions/72188903/pyside6-how-do-i-resize-a-qlabel-without-loosing-the-size-aspect-ratio
     """
 
@@ -116,11 +116,11 @@
     ):
         if self.underlying is None:
             self._initialize()
         assert self.underlying is not None
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying, None)
         if "src" in newprops:
-            commands.append(_CommandType(self.underlying._setPixmap, _image_descriptor_to_pixmap(newprops.src)))
+            commands.append(CommandType(self.underlying._setPixmap, _image_descriptor_to_pixmap(newprops.src)))
         if "aspect_ratio_mode" in newprops:
-            commands.append(_CommandType(self.underlying._setAspectRatioMode, newprops.aspect_ratio_mode))
+            commands.append(CommandType(self.underlying._setAspectRatioMode, newprops.aspect_ratio_mode))
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/base_components/spin_input.py` & `pyedifice-0.5.4/edifice/base_components/spin_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if QT_VERSION == "PyQt6" and not tp.TYPE_CHECKING:
     from PyQt6.QtGui import QValidator
     from PyQt6.QtWidgets import QSpinBox
 else:
     from PySide6.QtGui import QValidator
     from PySide6.QtWidgets import QSpinBox
 
-from .base_components import QtWidgetElement, _CommandType, _ensure_future, Element, _WidgetTree
+from .base_components import QtWidgetElement, CommandType, _ensure_future, Element, _WidgetTree
 
 
 class _SpinBox(QSpinBox):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._textFromValue: tp.Callable[[int], str] | None = None
         self._valueFromText: tp.Callable[
@@ -146,17 +146,17 @@
             self._initialize()
         assert self.underlying is not None
         widget = tp.cast(_SpinBox, self.underlying)
 
         commands = super()._qt_update_commands_super(widget_trees, newprops, self.underlying)
 
         if "value_to_text" in newprops:
-            commands.append(_CommandType(setattr, widget, "_textFromValue", newprops.value_to_text))
+            commands.append(CommandType(setattr, widget, "_textFromValue", newprops.value_to_text))
         if "text_to_value" in newprops:
-            commands.append(_CommandType(setattr, widget, "_valueFromText", newprops.text_to_value))
+            commands.append(CommandType(setattr, widget, "_valueFromText", newprops.text_to_value))
         if "min_value" in newprops:
-            commands.append(_CommandType(widget.setMinimum, newprops.min_value))
+            commands.append(CommandType(widget.setMinimum, newprops.min_value))
         if "max_value" in newprops:
-            commands.append(_CommandType(widget.setMaximum, newprops.max_value))
+            commands.append(CommandType(widget.setMaximum, newprops.max_value))
         if "value" in newprops:
-            commands.append(_CommandType(self._set_value, newprops.value))
+            commands.append(CommandType(self._set_value, newprops.value))
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/base_components/table_grid_view.py` & `pyedifice-0.5.4/edifice/base_components/table_grid_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..qt import QT_VERSION
 
 if QT_VERSION == "PyQt6" and not TYPE_CHECKING:
     from PyQt6.QtWidgets import QGridLayout, QWidget
 else:
     from PySide6.QtWidgets import QGridLayout, QWidget
 
-from .base_components import _CommandType, PropsDict, Element, _get_widget_children, _WidgetTree, QtWidgetElement
+from .base_components import CommandType, PropsDict, Element, _get_widget_children, _WidgetTree, QtWidgetElement
 
 logger = logging.getLogger("Edifice")
 
 
 class _TableGridViewRow(QtWidgetElement):
     """
     Row Element of a :class:`TableGridView`.
@@ -23,15 +23,15 @@
     def __init__(self, tgv: "TableGridView"):
         super().__init__()
 
     def _qt_update_commands(
         self,
         children: list[_WidgetTree],
         newprops: PropsDict,
-    ) -> list[_CommandType]:
+    ) -> list[CommandType]:
         # This element has no Qt underlying so it has nothing to do except store
         # the children of the row.
         # The _qt_update_commands for TableGridView will render the children.
         return []
 
 
 class TableGridView(QtWidgetElement):
@@ -185,35 +185,35 @@
             children_of_rows.extend(children_of_row)
             for col, child in enumerate(children_of_row):
                 new_children[child] = (row, col)
 
         old_deletions = self._old_children.items() - new_children.items()
         new_additions = new_children.items() - self._old_children.items()
 
-        commands: list[_CommandType] = []
+        commands: list[CommandType] = []
 
         for w, (row, column) in old_deletions:
             if w in new_children:
-                commands.append(_CommandType(self._soft_delete_child, w, row, column))
+                commands.append(CommandType(self._soft_delete_child, w, row, column))
             else:
-                commands.append(_CommandType(self._delete_child, w, row, column))
+                commands.append(CommandType(self._delete_child, w, row, column))
 
         for w, (row, column) in new_additions:
-            commands.append(_CommandType(self._add_child, w, row, column))
+            commands.append(CommandType(self._add_child, w, row, column))
 
         self._old_children = new_children
 
         if "row_stretch" in newprops:
-            commands.append(_CommandType(self._set_row_stretch, newprops["row_stretch"]))
+            commands.append(CommandType(self._set_row_stretch, newprops["row_stretch"]))
         if "column_stretch" in newprops:
-            commands.append(_CommandType(self._set_column_stretch, newprops["column_stretch"]))
+            commands.append(CommandType(self._set_column_stretch, newprops["column_stretch"]))
         if "row_minheight" in newprops:
-            commands.append(_CommandType(self._set_row_minheight, newprops["row_minheight"]))
+            commands.append(CommandType(self._set_row_minheight, newprops["row_minheight"]))
         if "column_minwidth" in newprops:
-            commands.append(_CommandType(self._set_column_minwidth, newprops["column_minwidth"]))
+            commands.append(CommandType(self._set_column_minwidth, newprops["column_minwidth"]))
 
         commands.extend(
             super()._qt_update_commands_super(widget_trees, newprops, self.underlying, self.underlying_layout)
         )
 
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/engine.py` & `pyedifice-0.5.4/edifice/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,31 +45,31 @@
         def wrapper(*args, **kwargs):
             return asyncio.ensure_future(fn(*args, **kwargs))
 
         return wrapper
     return fn
 
 
-class _CommandType:
+class CommandType:
     def __init__(self, fn: Callable[P, tp.Any], *args: P.args, **kwargs: P.kwargs):
         # The return value of fn is ignored and should thus return None. However, in
-        # order to test with equality on the _CommandTypes we need to allow fn to return
+        # order to test with equality on the CommandTypes we need to allow fn to return
         # Any value to not allocate wrapper functions ignoring the return value.
         self.fn = fn
         self.args = args
         self.kwargs = kwargs
 
     def __str__(self):
         return f"{self.fn}(*{self.args},**{self.kwargs})"
 
     def __repr__(self):
         return f"{self.fn.__repr__()}(*{self.args.__repr__()},**{self.kwargs.__repr__()})"
 
     def __eq__(self, other):
-        if not isinstance(other, _CommandType):
+        if not isinstance(other, CommandType):
             return False
         if self.fn != other.fn:
             return False
         if len(self.args) != len(other.args):
             return False
         if len(self.kwargs) != len(other.kwargs):
             return False
@@ -853,14 +853,18 @@
                         case QDropEvent():
                             # Handle finalized drop
                             if event.mimeData().hasUrls():
                                 dropped_files_set(proposed_files)
                                 proposed_files_set([])
 
             Note that the handler function cannot not be a coroutine.
+        on_resize:
+            Callback for `resize events <https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.QWidget.resizeEvent>`_.
+            Takes a `QResizeEvent <https://doc.qt.io/qtforpython-6/PySide6/QtGui/QResizeEvent.html>`_
+            as argument.
 
     """
 
     def __init__(
         self,
         style: StyleType = None,
         tool_tip: tp.Optional[tp.Text] = None,
@@ -877,14 +881,15 @@
         on_mouse_up: tp.Optional[tp.Callable[[QtGui.QMouseEvent], None | tp.Awaitable[None]]] = None,
         on_mouse_enter: tp.Optional[tp.Callable[[QtGui.QMouseEvent], None | tp.Awaitable[None]]] = None,
         on_mouse_leave: tp.Optional[tp.Callable[[QtGui.QMouseEvent], None | tp.Awaitable[None]]] = None,
         on_mouse_move: tp.Optional[tp.Callable[[QtGui.QMouseEvent], None | tp.Awaitable[None]]] = None,
         on_drop: tp.Optional[
             tp.Callable[[QtGui.QDragEnterEvent | QtGui.QDragMoveEvent | QtGui.QDragLeaveEvent | QtGui.QDropEvent], None]
         ] = None,
+        on_resize: tp.Optional[tp.Callable[[QtGui.QResizeEvent], None | tp.Awaitable[None]]] = None,
     ):
         super().__init__()
         self._register_props(
             {
                 "style": style,
                 "tool_tip": tool_tip,
                 "cursor": cursor,
@@ -898,14 +903,15 @@
                 "on_key_up": on_key_up,
                 "on_mouse_down": on_mouse_down,
                 "on_mouse_up": on_mouse_up,
                 "on_mouse_enter": on_mouse_enter,
                 "on_mouse_leave": on_mouse_leave,
                 "on_mouse_move": on_mouse_move,
                 "on_drop": on_drop,
+                "on_resize": on_resize,
             }
         )
         self._height = 0
         self._width = 0
         self._top = 0
         self._left = 0
         self._size_from_font = None  # TODO _size_from_font is unused
@@ -918,14 +924,15 @@
         self._on_mouse_leave = None
         self._on_mouse_down = None
         self._on_mouse_up = None
         self._on_mouse_move = None
         self._on_drop: tp.Optional[
             tp.Callable[[QtGui.QDragEnterEvent | QtGui.QDragMoveEvent | QtGui.QDragLeaveEvent | QtGui.QDropEvent], None]
         ] = None
+        self._on_resize: tp.Optional[tp.Callable[[QtGui.QResizeEvent], None]] = None
         self._default_mouse_press_event = None
         self._default_mouse_release_event = None
         self._default_mouse_move_event = None
         self._default_mouse_enter_event = None
         self._default_mouse_leave_event = None
         self._default_drag_enter_event = None
         self._default_drag_move_event = None
@@ -1109,21 +1116,34 @@
             self.underlying.dragMoveEvent = self._on_drop  # type: ignore
             self.underlying.dragLeaveEvent = self._on_drop  # type: ignore
             self.underlying.dropEvent = self._on_drop  # type: ignore
         else:
             self._on_drop = None
             self.underlying.setAcceptDrops(False)
 
+    def _resizeEvent(self, event: QtGui.QResizeEvent):
+        if self._on_resize is not None:
+            self._on_resize(event)
+
+    def _set_on_resize(self, on_resize: tp.Optional[tp.Callable[[QtGui.QResizeEvent], None]]):
+        assert self.underlying is not None
+        if on_resize is not None:
+            self._on_resize = _ensure_future(on_resize)
+            self.underlying.resizeEvent = self._resizeEvent
+        else:
+            self._on_resize = None
+            self.underlying.resizeEvent = lambda event: None
+
     def _gen_styling_commands(
         self,
         style,
         underlying: QtWidgets.QWidget | None,
         underlying_layout: QtWidgets.QLayout | None = None,
     ):
-        commands: list[_CommandType] = []
+        commands: list[CommandType] = []
 
         if underlying_layout is not None:
             set_margin = False
             new_margin = [0, 0, 0, 0]
             if "margin" in style:
                 new_margin = [int(_css_to_number(style["margin"]))] * 4
                 style.pop("margin")
@@ -1161,20 +1181,20 @@
                     set_align = QtCore.Qt.AlignmentFlag.AlignBottom
                 else:
                     logger.warning("Unknown alignment: %s", style["align"])
                 style.pop("align")
 
             if set_margin:
                 commands.append(
-                    _CommandType(
+                    CommandType(
                         underlying_layout.setContentsMargins, new_margin[0], new_margin[1], new_margin[2], new_margin[3]
                     )
                 )
             if set_align:
-                commands.append(_CommandType(underlying_layout.setAlignment, set_align))
+                commands.append(CommandType(underlying_layout.setAlignment, set_align))
         else:
             if "align" in style:
                 if style["align"] == "left":
                     set_align = "AlignLeft"
                 elif style["align"] == "center":
                     set_align = "AlignCenter"
                 elif style["align"] == "right":
@@ -1227,19 +1247,19 @@
         if "left" in style:
             set_move = True
             move_coords[0] = int(_css_to_number(style["left"]))
             self._left = move_coords[0]
 
         if set_move:
             assert self.underlying is not None
-            commands.append(_CommandType(self.underlying.move, move_coords[0], move_coords[1]))
+            commands.append(CommandType(self.underlying.move, move_coords[0], move_coords[1]))
 
         assert self.underlying is not None
         css_string = _dict_to_style(style, "QWidget#" + str(id(self)))
-        commands.append(_CommandType(self.underlying.setStyleSheet, css_string))
+        commands.append(CommandType(self.underlying.setStyleSheet, css_string))
         return commands
 
     def _set_context_menu(self, underlying: QtWidgets.QWidget):
         if self._context_menu_connected:
             underlying.customContextMenuRequested.disconnect()
         self._context_menu_connected = True
         underlying.customContextMenuRequested.connect(self._show_context_menu)
@@ -1252,96 +1272,98 @@
             menu.move(pos)
             menu.show()
 
     def _qt_update_commands(
         self,
         widget_trees: dict[Element, "_WidgetTree"],
         newprops: PropsDict,
-    ) -> list[_CommandType]:
+    ) -> list[CommandType]:
         raise NotImplementedError
 
     def _qt_update_commands_super(
         self,
         widget_trees: dict[Element, "_WidgetTree"],
         # We must pass all of the widget_trees because some elements
         # like TableGridView need to know the children of the children.
         newprops: PropsDict,
         underlying: QtWidgets.QWidget,
         underlying_layout: QtWidgets.QLayout | None = None,
-    ) -> list[_CommandType]:
-        commands: list[_CommandType] = []
+    ) -> list[CommandType]:
+        commands: list[CommandType] = []
         for prop in newprops:
             if prop == "style":
                 style = newprops[prop] or {}
                 if isinstance(style, list):
                     # style is nonempty since otherwise the or statement would make it a dict
                     first_style = style[0].copy()
                     for next_style in style[1:]:
                         first_style.update(next_style)
                     style = first_style
                 else:
                     style = dict(style)
                 commands.extend(self._gen_styling_commands(style, underlying, underlying_layout))
             elif prop == "size_policy":
                 if newprops.size_policy is not None:
-                    commands.append(_CommandType(underlying.setSizePolicy, newprops.size_policy))
+                    commands.append(CommandType(underlying.setSizePolicy, newprops.size_policy))
             elif prop == "focus_policy":
                 if newprops.focus_policy is not None:
-                    commands.append(_CommandType(underlying.setFocusPolicy, newprops.focus_policy))
+                    commands.append(CommandType(underlying.setFocusPolicy, newprops.focus_policy))
             elif prop == "enabled":
                 if newprops.enabled is not None:
-                    commands.append(_CommandType(underlying.setEnabled, newprops.enabled))
+                    commands.append(CommandType(underlying.setEnabled, newprops.enabled))
             elif prop == "on_click":
-                commands.append(_CommandType(self._set_on_click, underlying, newprops.on_click))
+                commands.append(CommandType(self._set_on_click, underlying, newprops.on_click))
                 if newprops.on_click is not None and self.props.cursor is not None:
-                    commands.append(_CommandType(underlying.setCursor, QtCore.Qt.CursorShape.PointingHandCursor))
+                    commands.append(CommandType(underlying.setCursor, QtCore.Qt.CursorShape.PointingHandCursor))
             elif prop == "on_key_down":
-                commands.append(_CommandType(self._set_on_key_down, underlying, newprops.on_key_down))
+                commands.append(CommandType(self._set_on_key_down, underlying, newprops.on_key_down))
             elif prop == "on_key_up":
-                commands.append(_CommandType(self._set_on_key_up, underlying, newprops.on_key_up))
+                commands.append(CommandType(self._set_on_key_up, underlying, newprops.on_key_up))
             elif prop == "on_mouse_down":
-                commands.append(_CommandType(self._set_on_mouse_down, underlying, newprops.on_mouse_down))
+                commands.append(CommandType(self._set_on_mouse_down, underlying, newprops.on_mouse_down))
             elif prop == "on_mouse_up":
-                commands.append(_CommandType(self._set_on_mouse_up, underlying, newprops.on_mouse_up))
+                commands.append(CommandType(self._set_on_mouse_up, underlying, newprops.on_mouse_up))
             elif prop == "on_mouse_enter":
-                commands.append(_CommandType(self._set_on_mouse_enter, underlying, newprops.on_mouse_enter))
+                commands.append(CommandType(self._set_on_mouse_enter, underlying, newprops.on_mouse_enter))
             elif prop == "on_mouse_leave":
-                commands.append(_CommandType(self._set_on_mouse_leave, underlying, newprops.on_mouse_leave))
+                commands.append(CommandType(self._set_on_mouse_leave, underlying, newprops.on_mouse_leave))
             elif prop == "on_mouse_move":
-                commands.append(_CommandType(self._set_on_mouse_move, underlying, newprops.on_mouse_move))
+                commands.append(CommandType(self._set_on_mouse_move, underlying, newprops.on_mouse_move))
             elif prop == "on_drop":
-                commands.append(_CommandType(self._set_on_drop, underlying, newprops.on_drop))
+                commands.append(CommandType(self._set_on_drop, underlying, newprops.on_drop))
+            elif prop == "on_resize":
+                commands.append(CommandType(self._set_on_resize, newprops.on_resize))
             elif prop == "tool_tip":
                 if newprops.tool_tip is not None:
-                    commands.append(_CommandType(underlying.setToolTip, newprops.tool_tip))
+                    commands.append(CommandType(underlying.setToolTip, newprops.tool_tip))
             elif prop == "css_class":
                 css_class = newprops.css_class
                 if css_class is None:
                     css_class = []
-                commands.append(_CommandType(underlying.setProperty, "css_class", css_class))
+                commands.append(CommandType(underlying.setProperty, "css_class", css_class))
                 commands.extend(
                     [
-                        _CommandType(underlying.style().unpolish, underlying),
-                        _CommandType(underlying.style().polish, underlying),
+                        CommandType(underlying.style().unpolish, underlying),
+                        CommandType(underlying.style().polish, underlying),
                     ]
                 )
             elif prop == "cursor":
                 cursor = self.props.cursor or ("default" if self.props.on_click is None else "pointer")
-                commands.append(_CommandType(underlying.setCursor, _CURSORS[cursor]))
+                commands.append(CommandType(underlying.setCursor, _CURSORS[cursor]))
             elif prop == "context_menu":
                 if self._context_menu_connected:
                     underlying.customContextMenuRequested.disconnect()
                 if self.props.context_menu is not None:
                     commands.append(
-                        _CommandType(underlying.setContextMenuPolicy, QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
+                        CommandType(underlying.setContextMenuPolicy, QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
                     )
-                    commands.append(_CommandType(self._set_context_menu, underlying))
+                    commands.append(CommandType(self._set_context_menu, underlying))
                 else:
                     commands.append(
-                        _CommandType(underlying.setContextMenuPolicy, QtCore.Qt.ContextMenuPolicy.DefaultContextMenu)
+                        CommandType(underlying.setContextMenuPolicy, QtCore.Qt.ContextMenuPolicy.DefaultContextMenu)
                     )
         return commands
 
 
 class _WidgetTree(object):
     """
     A QtWidgetElement and its QtWidgetElement children.
@@ -1386,17 +1408,17 @@
 
     Concretely, it stores information such as commands,
     which must be executed by the caller.
     """
 
     def __init__(
         self,
-        commands: list[_CommandType],
+        commands: list[CommandType],
     ):
-        self.commands: list[_CommandType] = commands
+        self.commands: list[CommandType] = commands
 
 
 @dataclass
 class _HookState:
     state: tp.Any
     updaters: list[tp.Callable[[tp.Any], tp.Any]]
 
@@ -1861,19 +1883,19 @@
             if old_rendering is not None:
                 render_context.enqueued_deletions.extend(old_rendering)
             render_context.component_tree[component] = [sub_component]
             render_context.widget_tree[component] = self._render(sub_component, render_context)
 
         return render_context.widget_tree[component]
 
-    def gen_qt_commands(self, element: QtWidgetElement, render_context: _RenderContext) -> list[_CommandType]:
+    def gen_qt_commands(self, element: QtWidgetElement, render_context: _RenderContext) -> list[CommandType]:
         """
         Recursively generate the update commands for the widget tree.
         """
-        commands: list[_CommandType] = []
+        commands: list[CommandType] = []
         if self.is_stopped:
             return commands
 
         children = _get_widget_children(render_context.widget_tree, element)
         for child in children:
             rendered = self.gen_qt_commands(child, render_context)
             commands.extend(rendered)
@@ -1907,23 +1929,23 @@
                         hook.state = updater
                 if state0 != hook.state:
                     # State changed so we need to re-render this component.
                     if element not in components_:
                         components_.append(element)
                 hook.updaters.clear()
 
-        all_commands: list[_CommandType] = []
+        all_commands: list[CommandType] = []
 
         # Here is the problem.
         # We need to render the child before parent if the child state changed.
         # We need to render the parent before child if the child props changed.
         # So we do a complete render of each component individually, and then
         # we don't have to solve the problem of the order of rendering.
         for component in components_:
-            commands: list[_CommandType] = []
+            commands: list[CommandType] = []
 
             render_context = _RenderContext(self)
             local_state.render_context = render_context
 
             widget_tree = self._render(component, render_context)
 
             # Generate the update commands from the widget trees
```

### Comparing `pyedifice-0.5.3/edifice/extra/matplotlib_figure.py` & `pyedifice-0.5.4/edifice/extra/matplotlib_figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typing as tp
-from ..base_components.base_components import _CommandType, QtWidgetElement
+from ..base_components.base_components import CommandType, QtWidgetElement
 
 from ..qt import QT_VERSION
 
 if QT_VERSION == "PyQt6":
     pass
 else:
     pass
@@ -78,22 +78,22 @@
                 self.current_plot_fun = tp.cast(tp.Callable[[Axes], None], self.props.plot_fun)
                 self.subplots.clear()
                 self.current_plot_fun(self.subplots)
                 self.underlying.draw()
                 # alternately we could do draw_idle() here, but I don't think it's
                 # any better and it messes up the mouse events.
 
-            commands.append(_CommandType(_command_plot_fun, self))
+            commands.append(CommandType(_command_plot_fun, self))
         if "on_figure_mouse_move" in newprops:
 
             def _command_mouse_move(self):
                 if self.on_mouse_move_connect_id is not None:
                     self.underlying.mpl_disconnect(self.on_mouse_move_connect_id)
                 if newprops["on_figure_mouse_move"] is not None:
                     self.on_mouse_move_connect_id = self.underlying.mpl_connect(
                         "motion_notify_event", newprops["on_figure_mouse_move"]
                     )
                 else:
                     self.on_mouse_move_connect_id = None
 
-            commands.append(_CommandType(_command_mouse_move, self))
+            commands.append(CommandType(_command_mouse_move, self))
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/extra/pyqtgraph_plot.py` & `pyedifice-0.5.4/edifice/extra/pyqtgraph_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typing as tp
-from ..base_components.base_components import _CommandType, QtWidgetElement
+from ..base_components.base_components import CommandType, QtWidgetElement
 
 # Import PySide6 or PyQt6 before importing pyqtgraph so that pyqtgraph detects the same
 from ..qt import QT_VERSION
 
 if QT_VERSION == "PyQt6" and not tp.TYPE_CHECKING:
     pass
 else:
@@ -94,10 +94,10 @@
             plot_widget = tp.cast(pg.PlotWidget, self.underlying)
             plot_item = tp.cast(pg.PlotItem, plot_widget.getPlotItem())
 
             def _update_plot():
                 plot_item.clear()
                 plot_fun(plot_item)
 
-            commands.append(_CommandType(_update_plot))
+            commands.append(CommandType(_update_plot))
 
         return commands
```

### Comparing `pyedifice-0.5.3/edifice/hooks.py` & `pyedifice-0.5.4/edifice/hooks.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/LICENSE.txt` & `pyedifice-0.5.4/edifice/icons/font-awesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/address-book.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/address-book.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/address-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/address-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/angry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/angry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/arrow-alt-circle-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/arrow-alt-circle-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/bell-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/bell-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/bell.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/bell.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/building.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/building.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-minus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-minus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar-times.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar-times.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/calendar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/calendar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/caret-square-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/caret-square-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/chart-bar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/chart-bar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/check-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/check-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/check-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/check-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/clipboard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/clock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/clock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/clone.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/clone.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/closed-captioning.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/closed-captioning.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment-dots.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment-dots.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/comment.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/comment.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/comments.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/comments.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/compass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/compass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/copy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/copy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/copyright.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/copyright.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/credit-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/credit-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/dizzy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/dizzy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/dot-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/dot-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/edit.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/edit.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/envelope-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/envelope-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/envelope.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/envelope.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/eye-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/eye-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/eye.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/eye.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-archive.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-archive.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-audio.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-audio.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-code.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-code.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-excel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-excel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-image.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-image.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-pdf.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-powerpoint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-powerpoint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-video.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-video.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/file-word.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/file-word.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/flag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/flag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/flushed.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/flushed.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/folder-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/folder-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/font-awesome-logo-full.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/font-awesome-logo-full.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/frown-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/frown-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/frown.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/frown.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/futbol.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/futbol.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/gem.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/gem.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grimace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grimace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-beam-sweat.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-beam-sweat.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-hearts.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-hearts.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-squint-tears.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-squint-tears.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-stars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-stars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tears.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tears.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-tongue.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-tongue.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/grin.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/grin.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-lizard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-lizard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-paper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-paper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-peace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-peace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-point-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-point-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-pointer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-pointer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-rock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-rock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-scissors.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-scissors.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hand-spock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hand-spock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/handshake.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/handshake.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hdd.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hdd.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/heart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/heart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hospital.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hospital.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/hourglass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/hourglass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/id-badge.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/id-badge.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/id-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/id-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/image.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/image.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/images.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/images.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/keyboard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss-wink-heart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss-wink-heart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/kiss.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/kiss.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/laugh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/laugh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/lemon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/lemon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/life-ring.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/life-ring.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/lightbulb.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/list-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/list-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/map.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/map.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh-blank.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh-blank.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh-rolling-eyes.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh-rolling-eyes.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/meh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/meh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/minus-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/minus-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/money-bill-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/money-bill-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/moon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/moon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/newspaper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/newspaper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/object-group.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/object-group.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/object-ungroup.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/object-ungroup.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/paper-plane.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/paper-plane.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/pause-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/pause-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/play-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/play-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/plus-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/plus-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/question-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/question-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/registered.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/registered.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/sad-cry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/sad-cry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/sad-tear.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/sad-tear.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/save.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/save.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/share-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/share-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/smile.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/smile.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/snowflake.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/snowflake.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/star.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/star.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/sticky-note.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/sticky-note.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/stop-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/stop-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/sun.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/sun.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/surprise.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/surprise.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/thumbs-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/thumbs-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/thumbs-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/times-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/times-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/tired.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/tired.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/trash-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/trash-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/user-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/user-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/user.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/user.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/regular/window-close.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/regular/window-close.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ad.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ad.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/address-book.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/address-book.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/address-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/address-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/air-freshener.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/air-freshener.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-center.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-center.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-justify.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-justify.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/align-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/align-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/allergies.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/allergies.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ambulance.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ambulance.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/american-sign-language-interpreting.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/american-sign-language-interpreting.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/anchor.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/anchor.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/angle-double-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/angle-double-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/angry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/angry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ankh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ankh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/apple-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/apple-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/archive.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/archive.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/archway.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/archway.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-circle-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-circle-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrow-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrow-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt-h.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt-h.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt-v.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt-v.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/arrows-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/arrows-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/assistive-listening-systems.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/assistive-listening-systems.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/asterisk.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/asterisk.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/at.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/at.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/atlas.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/atlas.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/atom.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/atom.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/audio-description.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/audio-description.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/award.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/award.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/baby-carriage.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/baby-carriage.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/baby.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/baby.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/backspace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/backspace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacteria.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacteria.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bacterium.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bacterium.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bahai.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bahai.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/balance-scale.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/balance-scale.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ban.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ban.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/band-aid.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/band-aid.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/barcode.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/barcode.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/baseball-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/baseball-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/basketball-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/basketball-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bath.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bath.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bed.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bed.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/beer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/beer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bell-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bell-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bell.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bell.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bezier-curve.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bezier-curve.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bible.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bible.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bicycle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bicycle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/biking.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/biking.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/binoculars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/binoculars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/biohazard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/biohazard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/birthday-cake.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/birthday-cake.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/blender-phone.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/blender-phone.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/blender.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/blender.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/blind.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/blind.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/blog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/blog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bold.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bold.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bomb.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bomb.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bone.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bone.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bong.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bong.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-dead.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-dead.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/book-reader.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/book-reader.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/book.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/book.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/border-none.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/border-none.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/border-style.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/border-style.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bowling-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bowling-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/box-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/box-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/box-tissue.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/box-tissue.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/boxes.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/boxes.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/braille.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/braille.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/brain.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/brain.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/briefcase-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/briefcase-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/briefcase.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/briefcase.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/broadcast-tower.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/broadcast-tower.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/broom.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/broom.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/brush.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/brush.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bug.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bug.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/building.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/building.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bullhorn.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bullhorn.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bullseye.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bullseye.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bus-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bus-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/bus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/bus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/business-time.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/business-time.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calculator.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calculator.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-day.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-day.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-minus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-minus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-times.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-times.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar-week.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar-week.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/calendar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/calendar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/camera-retro.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/camera-retro.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/camera.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/camera.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/campground.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/campground.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/candy-cane.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/candy-cane.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cannabis.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cannabis.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/capsules.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/capsules.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-battery.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-battery.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-crash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-crash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/car-side.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/car-side.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/car.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/car.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/caravan.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/caravan.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/caret-square-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/caret-square-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/carrot.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/carrot.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cart-arrow-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cart-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cart-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cart-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cash-register.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cash-register.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cat.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cat.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/certificate.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/certificate.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chair.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chair.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chalkboard-teacher.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chalkboard-teacher.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/charging-station.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/charging-station.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-bar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-bar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-line.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-line.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chart-pie.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chart-pie.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-double.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-double.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/check-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/check-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-bishop.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-bishop.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-board.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-board.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-king.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-king.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-knight.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-knight.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-pawn.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-pawn.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-queen.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-queen.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess-rook.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess-rook.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chess.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chess.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-circle-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-circle-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/chevron-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/chevron-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/child.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/child.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/church.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/church.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/circle-notch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/circle-notch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/city.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/city.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/clinic-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/clinic-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard-list.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard-list.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/clipboard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/clipboard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/closed-captioning.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/closed-captioning.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-download-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-download-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-meatball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-meatball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-moon-rain.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-moon-rain.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-moon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-moon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-rain.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-rain.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-showers-heavy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-showers-heavy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-sun-rain.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-sun-rain.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-sun.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-sun.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud-upload-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud-upload-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cloud.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cloud.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cocktail.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cocktail.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/code-branch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/code-branch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/code.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/code.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cogs.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cogs.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/coins.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/coins.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-dollar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-dollar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-dots.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-dots.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comment-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comment-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comments-dollar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comments-dollar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/comments.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/comments.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/compact-disc.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/compact-disc.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/compass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/compass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress-arrows-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress-arrows-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/compress.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/compress.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/concierge-bell.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/concierge-bell.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cookie-bite.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cookie-bite.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cookie.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cookie.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/copy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/copy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/copyright.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/copyright.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/couch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/couch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/credit-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/credit-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crop-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crop-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crop.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crop.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crosshairs.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crosshairs.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crow.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crow.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crown.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crown.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/crutch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/crutch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cube.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cube.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cubes.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cubes.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/cut.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/cut.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/database.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/database.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/deaf.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/deaf.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/democrat.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/democrat.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dharmachakra.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dharmachakra.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/diagnoses.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/diagnoses.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-d20.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-d20.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-d6.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-d6.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-five.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-five.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-four.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-four.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-six.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-six.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-three.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-three.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice-two.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice-two.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dice.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dice.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/digital-tachograph.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/digital-tachograph.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/directions.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/directions.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/disease.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/disease.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/divide.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/divide.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dizzy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dizzy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dna.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dna.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dollar-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dollar-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dolly-flatbed.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dolly-flatbed.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dolly.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dolly.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/donate.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/donate.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/door-closed.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/door-closed.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/door-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/door-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dove.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dove.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/download.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/download.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/drafting-compass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/drafting-compass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dragon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dragon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/draw-polygon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/draw-polygon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/drum-steelpan.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/drum-steelpan.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/drum.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/drum.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/drumstick-bite.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/drumstick-bite.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumbbell.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumbbell.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumpster-fire.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumpster-fire.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dumpster.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dumpster.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/dungeon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/dungeon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/edit.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/edit.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/eject.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/eject.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-open-text.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-open-text.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/envelope.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/envelope.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/eraser.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/eraser.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ethernet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ethernet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/euro-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/euro-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/exchange-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/exchange-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation-triangle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation-triangle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/exclamation.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/exclamation.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand-arrows-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand-arrows-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/expand.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/expand.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/external-link-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/external-link-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/external-link-square-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/external-link-square-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye-dropper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye-dropper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/eye.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/eye.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fan.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fan.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fast-backward.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fast-backward.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fast-forward.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fast-forward.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/faucet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/faucet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fax.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fax.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/feather-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/feather-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/feather.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/feather.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/female.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/female.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fighter-jet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fighter-jet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-archive.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-archive.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-audio.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-audio.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-code.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-code.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-contract.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-contract.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-csv.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-csv.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-download.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-download.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-excel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-excel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-export.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-export.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-image.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-image.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-import.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-import.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-invoice-dollar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-invoice-dollar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-invoice.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-invoice.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-medical-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-medical-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-pdf.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-powerpoint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-powerpoint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-prescription.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-prescription.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-signature.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-signature.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-upload.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-upload.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-video.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-video.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/file-word.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/file-word.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fill-drip.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fill-drip.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fill.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fill.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/film.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/film.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fingerprint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire-extinguisher.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire-extinguisher.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fire.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fire.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/first-aid.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/first-aid.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fish.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fish.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/fist-raised.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/fist-raised.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag-checkered.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag-checkered.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag-usa.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag-usa.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/flag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/flag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/flask.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/flask.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/flushed.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/flushed.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/folder-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/folder-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/font-awesome-logo-full.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/font-awesome-logo-full.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/font.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/font.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/football-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/football-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/frog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/frog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/frown-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/frown-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/frown.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/frown.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/funnel-dollar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/funnel-dollar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/futbol.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/futbol.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gamepad.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gamepad.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gas-pump.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gas-pump.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gavel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gavel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gem.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gem.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ghost.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ghost.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gift.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gift.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gifts.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gifts.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/glass-cheers.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/glass-cheers.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/glasses.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/glasses.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-africa.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-africa.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-americas.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-americas.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-asia.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-asia.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe-europe.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe-europe.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/globe.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/globe.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/golf-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/golf-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/gopuram.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/gopuram.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/graduation-cap.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/graduation-cap.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/greater-than-equal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/greater-than-equal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/greater-than.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/greater-than.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grimace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grimace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-beam-sweat.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-beam-sweat.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-hearts.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-hearts.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-squint-tears.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-squint-tears.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-stars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-stars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tears.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tears.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-tongue.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-tongue.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grin.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grin.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-horizontal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/grip-vertical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/grip-vertical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/guitar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/guitar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/h-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/h-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hamburger.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hamburger.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hammer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hammer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hamsa.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hamsa.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-heart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-heart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-usd.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-usd.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding-water.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding-water.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-holding.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-holding.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-lizard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-lizard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-middle-finger.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-middle-finger.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-paper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-paper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-peace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-peace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-point-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-point-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-pointer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-pointer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-rock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-rock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-scissors.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-scissors.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-sparkles.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-sparkles.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hand-spock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hand-spock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands-helping.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands-helping.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands-wash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands-wash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hands.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hands.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake-alt-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake-alt-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/handshake.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/handshake.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hanukiah.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hanukiah.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hashtag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hashtag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-cowboy-side.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-cowboy-side.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-cowboy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-cowboy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hat-wizard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hat-wizard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hdd.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hdd.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-cough-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-cough-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-cough.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-cough.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-mask.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-mask.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/head-side-virus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/head-side-virus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/heading.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/heading.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/headphones-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/headphones-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/headphones.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/headphones.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/headset.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/headset.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/heartbeat.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/heartbeat.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/helicopter.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/helicopter.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/highlighter.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/highlighter.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hiking.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hiking.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hippo.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hippo.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/history.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/history.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/holly-berry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/holly-berry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/home.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/home.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/horse-head.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/horse-head.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/horse.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/horse.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-symbol.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-symbol.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital-user.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital-user.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hospital.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hospital.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hot-tub.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hot-tub.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hotdog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hotdog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hotel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hotel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-end.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-end.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-half.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-half.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass-start.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass-start.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hourglass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hourglass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/house-damage.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/house-damage.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/house-user.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/house-user.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/hryvnia.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/hryvnia.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/i-cursor.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/i-cursor.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/icons.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/icons.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-badge.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-badge.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-card-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-card-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/id-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/id-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/igloo.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/igloo.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/image.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/image.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/images.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/images.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/inbox.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/inbox.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/indent.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/indent.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/infinity.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/infinity.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/info-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/info-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/info.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/info.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/jedi.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/jedi.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/joint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/joint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/journal-whills.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/journal-whills.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/kaaba.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/kaaba.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/key.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/key.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/keyboard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/khanda.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/khanda.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss-wink-heart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss-wink-heart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiss.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiss.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/kiwi-bird.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/kiwi-bird.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/landmark.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/landmark.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/language.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/language.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-code.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-code.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-house.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-house.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laptop.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laptop.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-squint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-squint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/laugh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/laugh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/layer-group.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/layer-group.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/leaf.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/leaf.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lemon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lemon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/less-than-equal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/less-than-equal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/less-than.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/less-than.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/level-down-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/level-down-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/level-up-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/level-up-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/life-ring.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/life-ring.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lightbulb.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/link.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/link.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lira-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lira-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-ol.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-ol.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/list-ul.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/list-ul.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/list.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/list.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lock-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lock-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/low-vision.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/low-vision.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/luggage-cart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/luggage-cart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lungs-virus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lungs-virus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/lungs.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/lungs.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/magic.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/magic.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/magnet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/magnet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mail-bulk.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mail-bulk.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/male.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/male.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marked-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marked-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-marked.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-marked.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-pin.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-pin.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/map-signs.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/map-signs.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/marker.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/marker.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-double.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-double.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke-h.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke-h.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke-v.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke-v.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars-stroke.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars-stroke.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mask.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mask.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/medal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/medal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/medkit.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/medkit.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/meh-rolling-eyes.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/meh-rolling-eyes.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/meh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/meh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/memory.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/memory.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/menorah.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/menorah.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mercury.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mercury.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/meteor.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/meteor.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microchip.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microchip.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-alt-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-alt-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microphone.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microphone.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/microscope.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/microscope.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mitten.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mitten.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mobile-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mobile-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-wave-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-wave-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill-wave.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill-wave.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-bill.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-bill.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-check-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-check-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/money-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/money-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/monument.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/monument.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/moon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/moon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mortar-pestle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mortar-pestle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mosque.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mosque.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/motorcycle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/motorcycle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mountain.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mountain.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mouse-pointer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mouse-pointer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/mug-hot.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/mug-hot.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/network-wired.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/network-wired.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/newspaper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/newspaper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/not-equal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/not-equal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/notes-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/notes-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/object-group.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/object-group.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/object-ungroup.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/object-ungroup.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/oil-can.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/oil-can.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/om.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/om.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/otter.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/otter.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/outdent.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/outdent.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pager.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pager.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/paint-brush.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/paint-brush.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/paint-roller.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/paint-roller.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/palette.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/palette.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pallet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pallet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/paperclip.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/paperclip.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/parachute-box.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/parachute-box.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/parking.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/parking.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/passport.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/passport.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pastafarianism.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pastafarianism.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/paste.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/paste.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pause-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pause-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/paw.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/paw.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/peace.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/peace.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-fancy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-fancy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-nib.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-nib.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pen-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pen-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pencil-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pencil-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pencil-ruler.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pencil-ruler.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/people-arrows.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/people-arrows.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/people-carry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/people-carry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pepper-hot.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pepper-hot.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/percent.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/percent.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/percentage.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/percentage.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/person-booth.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/person-booth.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-square-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-square-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone-volume.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone-volume.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/phone.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/phone.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/photo-video.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/photo-video.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/piggy-bank.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/piggy-bank.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pills.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pills.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pizza-slice.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pizza-slice.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/place-of-worship.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/place-of-worship.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-arrival.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-arrival.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-departure.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-departure.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plane.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plane.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plus-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plus-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/plus-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/plus-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/podcast.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/podcast.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/poll-h.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/poll-h.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/poll.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/poll.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/poo-storm.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/poo-storm.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/poo.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/poo.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/poop.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/poop.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/portrait.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/portrait.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pound-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pound-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/power-off.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/power-off.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pray.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pray.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/praying-hands.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/praying-hands.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription-bottle-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription-bottle-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription-bottle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription-bottle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/prescription.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/prescription.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/print.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/print.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/procedures.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/procedures.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/project-diagram.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/project-diagram.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pump-medical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pump-medical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/pump-soap.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/pump-soap.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/puzzle-piece.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/question-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/question-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/question.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/question.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/quidditch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/quidditch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/quote-left.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/quote-left.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/quote-right.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/quote-right.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/quran.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/quran.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/radiation-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/radiation-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/radiation.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/radiation.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/rainbow.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/rainbow.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/random.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/random.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/receipt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/receipt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/recycle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/recycle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/redo-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/redo-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/redo.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/redo.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/registered.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/registered.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/remove-format.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/remove-format.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/reply-all.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/reply-all.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/reply.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/reply.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/republican.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/republican.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/restroom.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/restroom.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/retweet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/retweet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ribbon.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ribbon.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ring.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ring.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/road.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/road.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/robot.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/robot.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/rocket.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/rocket.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/route.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/route.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/rss-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/rss-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/rss.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/rss.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruble-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruble-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-combined.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-combined.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-horizontal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler-vertical.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler-vertical.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ruler.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ruler.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/running.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/running.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/rupee-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/rupee-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sad-cry.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sad-cry.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sad-tear.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sad-tear.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/satellite-dish.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/satellite-dish.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/satellite.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/satellite.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/save.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/save.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/school.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/school.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/screwdriver.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/screwdriver.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/scroll.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/scroll.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-dollar.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-dollar.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-location.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-location.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-minus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-minus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/search-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/search-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/search.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/search.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/server.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/server.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shapes.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shapes.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-alt-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-alt-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/share-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/share-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/share.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/share.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shekel-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shekel-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shield-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shield-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shield-virus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shield-virus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ship.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ship.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shipping-fast.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shipping-fast.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shoe-prints.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shoe-prints.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-bag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-bag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-basket.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-basket.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shopping-cart.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shopping-cart.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shower.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shower.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/shuttle-van.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/shuttle-van.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-in-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-in-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-language.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-language.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sign-out-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sign-out-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/signal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/signal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/signature.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/signature.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sim-card.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sim-card.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sitemap.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sitemap.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/skating.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/skating.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/skiing-nordic.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/skiing-nordic.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/skiing.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/skiing.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/skull-crossbones.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/skull-crossbones.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/skull.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/skull.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sleigh.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sleigh.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sliders-h.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sliders-h.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile-beam.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile-beam.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile-wink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile-wink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smile.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smile.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smoking-ban.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smoking-ban.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/smoking.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/smoking.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sms.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sms.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowboarding.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowboarding.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowflake.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowflake.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowman.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowman.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/snowplow.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/snowplow.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/soap.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/soap.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/socks.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/socks.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/solar-panel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/solar-panel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-down-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-down-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-up-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-up-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-alpha-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-alpha-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-down-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-down-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-up-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-up-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-amount-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-amount-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-down-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-down-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-up-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-up-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sort-numeric-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sort-numeric-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/spa.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/spa.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/space-shuttle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/space-shuttle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/spell-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/spell-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/spider.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/spider.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/spinner.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/spinner.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/splotch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/splotch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/spray-can.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/spray-can.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/square-root-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/square-root-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stamp.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stamp.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-and-crescent.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-and-crescent.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-half-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-half-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-of-david.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-of-david.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/star-of-life.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/star-of-life.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/star.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/star.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stethoscope.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stethoscope.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stopwatch-20.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stopwatch-20.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stopwatch.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stopwatch.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-alt-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-alt-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/store-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/store-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/store.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/store.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stream.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stream.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/street-view.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/street-view.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/strikethrough.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/strikethrough.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/stroopwafel.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/stroopwafel.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/subscript.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/subscript.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/subway.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/subway.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/suitcase-rolling.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/suitcase-rolling.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sun.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sun.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/superscript.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/superscript.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/surprise.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/surprise.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/swatchbook.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/swatchbook.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/swimmer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/swimmer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/swimming-pool.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/swimming-pool.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/synagogue.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/synagogue.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sync-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sync-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/sync.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/sync.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/syringe.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/syringe.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/table-tennis.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/table-tennis.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tablet-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tablet-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tablets.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tablets.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tachometer-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tachometer-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tags.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tags.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tape.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tape.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tasks.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tasks.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/taxi.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/taxi.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/teeth-open.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/teeth-open.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/teeth.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/teeth.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/temperature-high.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/temperature-high.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/temperature-low.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/temperature-low.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/terminal.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/terminal.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/text-height.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/text-height.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/text-width.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/text-width.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/th-large.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/th-large.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/th-list.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/th-list.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/th.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/th.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/theater-masks.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/theater-masks.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-empty.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-empty.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-full.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-full.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-half.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-half.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-quarter.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-quarter.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer-three-quarters.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer-three-quarters.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thermometer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thermometer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbs-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbs-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbs-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/thumbtack.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/thumbtack.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/ticket-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/ticket-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/times-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/times-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/times.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/times.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tint-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tint-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tint.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tint.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tired.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tired.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/toggle-off.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/toggle-off.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet-paper-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet-paper-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet-paper.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet-paper.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/toilet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/toilet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/toolbox.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/toolbox.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tools.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tools.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tooth.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tooth.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/torah.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/torah.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/torii-gate.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/torii-gate.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tractor.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tractor.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trademark.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trademark.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/traffic-light.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/traffic-light.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trailer.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trailer.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/train.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/train.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tram.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tram.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/transgender-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/transgender-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/transgender.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/transgender.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-restore-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-restore-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trash-restore.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trash-restore.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tree.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tree.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/trophy.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/trophy.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-loading.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-loading.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-monster.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-monster.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-moving.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-moving.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck-pickup.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck-pickup.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/truck.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/truck.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tshirt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tshirt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/tty.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/tty.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/umbrella-beach.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/umbrella-beach.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/umbrella.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/umbrella.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/underline.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/underline.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/undo-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/undo-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/undo.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/undo.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/universal-access.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/universal-access.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/university.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/university.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlink.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlink.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlock-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlock-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/unlock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/unlock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/upload.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/upload.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-alt-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-alt-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-astronaut.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-astronaut.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-check.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-check.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-circle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-circle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-clock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-clock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-cog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-cog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-edit.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-edit.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-friends.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-friends.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-graduate.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-graduate.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-injured.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-injured.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-lock.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-lock.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-md.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-md.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-minus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-minus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-ninja.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-ninja.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-nurse.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-nurse.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-plus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-plus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-secret.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-secret.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-shield.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-shield.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-tag.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-tag.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user-times.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user-times.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/user.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/user.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/users-cog.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/users-cog.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/users-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/users-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/users.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/users.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/utensils.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/utensils.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vector-square.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vector-square.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus-double.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus-double.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus-mars.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus-mars.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/venus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/venus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vest-patches.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vest-patches.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vest.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vest.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vial.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vial.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vials.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vials.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/video-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/video-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vihara.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vihara.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/virus-slash.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/virus-slash.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/virus.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/virus.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/viruses.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/viruses.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/volleyball-ball.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/volleyball-ball.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-down.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-down.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-mute.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-mute.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/volume-up.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/volume-up.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vote-yea.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vote-yea.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/vr-cardboard.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/vr-cardboard.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/walking.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/walking.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wallet.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wallet.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/warehouse.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/warehouse.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/water.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/water.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/weight-hanging.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/weight-hanging.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/weight.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/weight.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wheelchair.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wheelchair.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wifi.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wifi.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wind.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wind.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-close.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-close.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/window-restore.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/window-restore.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-bottle.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-bottle.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-glass-alt.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-glass-alt.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wine-glass.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wine-glass.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/won-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/won-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/wrench.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/wrench.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/x-ray.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/x-ray.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/yen-sign.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/yen-sign.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/icons/font-awesome/solid/yin-yang.svg` & `pyedifice-0.5.4/edifice/icons/font-awesome/solid/yin-yang.svg`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/inspector/icon.png` & `pyedifice-0.5.4/edifice/inspector/icon.png`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/inspector/inspector.py` & `pyedifice-0.5.4/edifice/inspector/inspector.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/logger.py` & `pyedifice-0.5.4/edifice/logger.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/runner.py` & `pyedifice-0.5.4/edifice/runner.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/edifice/utilities.py` & `pyedifice-0.5.4/edifice/utilities.py`

 * *Files identical despite different names*

### Comparing `pyedifice-0.5.3/pyproject.toml` & `pyedifice-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "pyedifice"
-version = "0.5.3"
+version = "0.5.4"
 description = "Declarative GUI framework for Python and Qt"
 authors = ["David Ding", "James D. Brock", "Viktor Kronvall"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pyedifice.github.io"
 repository = "https://github.com/pyedifice/pyedifice"
 packages = [{include = "edifice", from = "."}]
+classifiers = [
+  'Topic :: Software Development :: User Interfaces',
+]
 
 [tool.nix]
 format = "poetry-core"
 
 [tool.poetry.dependencies]
 # we need typing and async features from python 3.10
 python = ">=3.10, <3.13"
@@ -45,11 +48,7 @@
 
 [tool.ruff]
 line-length = 120
 
 [tool.pyright]
 include = ["edifice"]
 exclude = ["**/__pycache__"]
-
-classifiers = [
-  'Topic :: Software Development :: User Interfaces',
-]
```

### Comparing `pyedifice-0.5.3/PKG-INFO` & `pyedifice-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyedifice
-Version: 0.5.3
+Version: 0.5.4
 Summary: Declarative GUI framework for Python and Qt
 Home-page: https://pyedifice.github.io
 License: MIT
 Author: David Ding
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: User Interfaces
 Requires-Dist: qasync (>=0.26.0)
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Repository, https://github.com/pyedifice/pyedifice
 Description-Content-Type: text/markdown
 
 <h3 align="center">
 <img src="https://raw.githubusercontent.com/pyedifice/pyedifice/master/docs/source/image/EdificePyramid.svg" width="200">
```

