# Comparing `tmp/tablate-0.0.1.tar.gz` & `tmp/tablate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablate-0.0.1.tar", last modified: Wed Jul 19 09:14:40 2023, max compression
+gzip compressed data, was "tablate-0.0.2.tar", last modified: Thu Jul 20 14:35:48 2023, max compression
```

## Comparing `tablate-0.0.1.tar` & `tablate-0.0.2.tar`

### file list

```diff
@@ -1,65 +1,99 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.534688 tablate-0.0.1/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.1/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22604 2023-07-19 09:14:40.533688 tablate-0.0.1/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 tablate-0.0.1/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      586 2023-07-19 09:14:30.000000 tablate-0.0.1/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-19 09:14:40.534688 tablate-0.0.1/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.528688 tablate-0.0.1/tablate.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22604 2023-07-19 09:14:40.000000 tablate-0.0.1/tablate.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1867 2023-07-19 09:14:40.000000 tablate-0.0.1/tablate.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-19 09:14:40.000000 tablate-0.0.1/tablate.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       10 2023-07-19 09:14:40.000000 tablate-0.0.1/tablate.egg-info/top_level.txt
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.528688 tablate-0.0.1/textframe/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      123 2023-07-17 22:02:31.000000 tablate-0.0.1/textframe/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.529688 tablate-0.0.1/textframe/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    12376 2023-07-19 09:13:17.000000 tablate-0.0.1/textframe/api/TextFrame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.1/textframe/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.529688 tablate-0.0.1/textframe/characters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.1/textframe/characters/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.1/textframe/characters/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.1/textframe/characters/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      106 2023-07-16 22:19:15.000000 tablate-0.0.1/textframe/characters/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2331 2023-07-19 03:41:47.000000 tablate-0.0.1/textframe/characters/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.1/textframe/characters/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.529688 tablate-0.0.1/textframe/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.1/textframe/helpers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.530688 tablate-0.0.1/textframe/helpers/calcs/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.1/textframe/helpers/calcs/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1063 2023-07-19 08:46:35.000000 tablate-0.0.1/textframe/helpers/calcs/calc_column_percent.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.1/textframe/helpers/calcs/calc_column_widths.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.530688 tablate-0.0.1/textframe/helpers/checkers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.1/textframe/helpers/checkers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.1/textframe/helpers/checkers/is_last_element.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.530688 tablate-0.0.1/textframe/helpers/formatters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.1/textframe/helpers/formatters/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.531688 tablate-0.0.1/textframe/helpers/formatters/string/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.1/textframe/helpers/formatters/string/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4560 2023-07-19 03:08:11.000000 tablate-0.0.1/textframe/helpers/formatters/string/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3115 2023-07-18 20:58:03.000000 tablate-0.0.1/textframe/helpers/formatters/string/row_frame_divider.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      536 2023-07-18 09:08:43.000000 tablate-0.0.1/textframe/helpers/formatters/string/row_outer_border.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.531688 tablate-0.0.1/textframe/helpers/renderers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.1/textframe/helpers/renderers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.531688 tablate-0.0.1/textframe/helpers/renderers/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.1/textframe/helpers/renderers/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.532688 tablate-0.0.1/textframe/helpers/renderers/html/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:49:46.000000 tablate-0.0.1/textframe/helpers/renderers/html/frames/render_html_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:05:40.000000 tablate-0.0.1/textframe/helpers/renderers/html/frames/render_html_table_body.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:49:32.000000 tablate-0.0.1/textframe/helpers/renderers/html/frames/render_html_table_head.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:50:17.000000 tablate-0.0.1/textframe/helpers/renderers/html/frames/render_html_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 05:07:16.000000 tablate-0.0.1/textframe/helpers/renderers/html/render_html_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:49:05.000000 tablate-0.0.1/textframe/helpers/renderers/html/render_html_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      869 2023-07-19 08:46:35.000000 tablate-0.0.1/textframe/helpers/renderers/html/render_html_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.532688 tablate-0.0.1/textframe/helpers/renderers/string/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.1/textframe/helpers/renderers/string/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3365 2023-07-19 03:00:00.000000 tablate-0.0.1/textframe/helpers/renderers/string/render_string_frame_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2708 2023-07-19 00:44:14.000000 tablate-0.0.1/textframe/helpers/renderers/string/render_string_frame_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1894 2023-07-19 03:06:14.000000 tablate-0.0.1/textframe/helpers/renderers/string/render_string_frame_text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.532688 tablate-0.0.1/textframe/helpers/validators/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.1/textframe/helpers/validators/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 09:14:40.533688 tablate-0.0.1/textframe/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:38:29.000000 tablate-0.0.1/textframe/tests/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2628 2023-07-19 04:18:29.000000 tablate-0.0.1/textframe/tests/test_decs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6863 2023-07-19 04:16:33.000000 tablate-0.0.1/textframe/tests/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       69 2023-07-19 04:18:54.000000 tablate-0.0.1/textframe/tests/test_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       67 2023-07-19 04:18:29.000000 tablate-0.0.1/textframe/tests/test_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3577 2023-07-19 03:16:02.000000 tablate-0.0.1/textframe/typing.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.267838 tablate-0.0.2/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.2/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 14:35:48.267838 tablate-0.0.2/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 tablate-0.0.2/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-20 14:35:41.000000 tablate-0.0.2/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-20 14:35:48.267838 tablate-0.0.2/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.257838 tablate-0.0.2/tablate/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      117 2023-07-19 10:35:23.000000 tablate-0.0.2/tablate/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.258838 tablate-0.0.2/tablate/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    10056 2023-07-20 13:47:58.000000 tablate-0.0.2/tablate/api/Tablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.2/tablate/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.258838 tablate-0.0.2/tablate/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.2/tablate/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.2/tablate/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.2/tablate/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.2/tablate/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.2/tablate/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.2/tablate/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.258838 tablate-0.0.2/tablate/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.2/tablate/helpers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.259838 tablate-0.0.2/tablate/helpers/calcs/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.2/tablate/helpers/calcs/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-19 21:31:48.000000 tablate-0.0.2/tablate/helpers/calcs/calc_column_percent.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.2/tablate/helpers/calcs/calc_column_widths.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.2/tablate/helpers/calcs/get_row_colspan.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-19 22:13:11.000000 tablate-0.0.2/tablate/helpers/calcs/random_string.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.259838 tablate-0.0.2/tablate/helpers/checkers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.2/tablate/helpers/checkers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.2/tablate/helpers/checkers/is_last_element.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.260838 tablate-0.0.2/tablate/helpers/formatters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.2/tablate/helpers/formatters/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.260838 tablate-0.0.2/tablate/helpers/formatters/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.2/tablate/helpers/formatters/console/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.2/tablate/helpers/formatters/console/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      539 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/formatters/console/row_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3160 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/formatters/console/row_divider.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.260838 tablate-0.0.2/tablate/helpers/formatters/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.2/tablate/helpers/formatters/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.261838 tablate-0.0.2/tablate/helpers/formatters/html/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.2/tablate/helpers/formatters/html/element/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:39.000000 tablate-0.0.2/tablate/helpers/formatters/html/element/frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:45.000000 tablate-0.0.2/tablate/helpers/formatters/html/element/row.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:34.000000 tablate-0.0.2/tablate/helpers/formatters/html/element/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.261838 tablate-0.0.2/tablate/helpers/formatters/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.261838 tablate-0.0.2/tablate/helpers/formatters/html/style/border/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:38.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/border/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:51.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/border/border_bottom.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:46:57.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/border/border_right.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/border/border_style.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      211 2023-07-20 10:49:54.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/selector.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.262838 tablate-0.0.2/tablate/helpers/formatters/html/style/text/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:34.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/text/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/text/alignment.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/text/multiline.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:48:28.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/text/overflow.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:12:25.000000 tablate-0.0.2/tablate/helpers/formatters/html/style/text/padding.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.262838 tablate-0.0.2/tablate/helpers/renderers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.2/tablate/helpers/renderers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.263838 tablate-0.0.2/tablate/helpers/renderers/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.2/tablate/helpers/renderers/console/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.264838 tablate-0.0.2/tablate/helpers/renderers/console/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.2/tablate/helpers/renderers/console/frames/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2113 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/frames/render_console_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2530 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/frames/render_console_frame_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3869 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/frames/render_string_frame_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1936 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/frames/render_string_frame_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      844 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/render_console_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2280 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/render_console_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      821 2023-07-20 09:59:11.000000 tablate-0.0.2/tablate/helpers/renderers/console/render_console_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.264838 tablate-0.0.2/tablate/helpers/renderers/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.2/tablate/helpers/renderers/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.265838 tablate-0.0.2/tablate/helpers/renderers/html/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      277 2023-07-19 20:38:22.000000 tablate-0.0.2/tablate/helpers/renderers/html/frames/render_html_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1375 2023-07-20 11:47:48.000000 tablate-0.0.2/tablate/helpers/renderers/html/frames/render_html_table_body.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1023 2023-07-20 11:47:48.000000 tablate-0.0.2/tablate/helpers/renderers/html/frames/render_html_table_head.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:50:17.000000 tablate-0.0.2/tablate/helpers/renderers/html/frames/render_html_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.2/tablate/helpers/renderers/html/render_html_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      760 2023-07-20 10:18:01.000000 tablate-0.0.2/tablate/helpers/renderers/html/render_html_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1157 2023-07-20 11:47:48.000000 tablate-0.0.2/tablate/helpers/renderers/html/render_html_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.265838 tablate-0.0.2/tablate/helpers/validators/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.2/tablate/helpers/validators/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.266838 tablate-0.0.2/tablate/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 00:45:20.000000 tablate-0.0.2/tablate/tests/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3513 2023-07-20 06:58:36.000000 tablate-0.0.2/tablate/tests/test_decs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8057 2023-07-20 00:01:38.000000 tablate-0.0.2/tablate/tests/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       67 2023-07-19 10:35:23.000000 tablate-0.0.2/tablate/tests/test_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       65 2023-07-19 09:16:41.000000 tablate-0.0.2/tablate/tests/test_text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.266838 tablate-0.0.2/tablate/type/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.2/tablate/type/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2473 2023-07-20 09:49:58.000000 tablate-0.0.2/tablate/type/dict_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1129 2023-07-20 07:45:25.000000 tablate-0.0.2/tablate/type/dict_input.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      538 2023-07-20 13:47:58.000000 tablate-0.0.2/tablate/type/dict_options.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.2/tablate/type/primitives.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:35:48.258838 tablate-0.0.2/tablate.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 14:35:48.000000 tablate-0.0.2/tablate.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3151 2023-07-20 14:35:48.000000 tablate-0.0.2/tablate.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-20 14:35:48.000000 tablate-0.0.2/tablate.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-20 14:35:48.000000 tablate-0.0.2/tablate.egg-info/top_level.txt
```

### Comparing `tablate-0.0.1/LICENCE` & `tablate-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tablate-0.0.1/PKG-INFO` & `tablate-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.1
+Version: 0.0.2
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ```python
```

### Comparing `tablate-0.0.1/README.md` & `tablate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tablate-0.0.1/pyproject.toml` & `tablate-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablate"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII plain text table renderer."
 readme = "README.md"
-requires-python = ">=3"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `tablate-0.0.1/tablate.egg-info/PKG-INFO` & `tablate-0.0.2/tablate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.1
+Version: 0.0.2
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 ```python
```

### Comparing `tablate-0.0.1/textframe/api/TextFrame.py` & `tablate-0.0.2/tablate/api/Tablate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,101 @@
 import copy
 import shutil
 from typing import List, Dict, Optional, Union
 
-from textframe.characters.corners import top_left, top_right, bottom_left, bottom_right
-from textframe.helpers.calcs.calc_column_percent import calc_column_percent
-from textframe.helpers.calcs.calc_column_widths import calc_column_widths
-from textframe.helpers.checkers.is_last_element import is_last_element
-from textframe.helpers.formatters.string.row_frame_divider import row_frame_divider
-from textframe.helpers.formatters.string.row_outer_border import row_outer_border
-from textframe.helpers.renderers.html.render_html_head import render_html_head
-from textframe.helpers.renderers.string.render_string_frame_grid import render_single_line_grid, render_multi_line_grid
-from textframe.helpers.renderers.string.render_string_frame_table import render_table_frame_string
-from textframe.helpers.renderers.string.render_string_frame_text import render_text_frame_string
-from textframe.typing import BaseBorder, TableInputColumnDict, HeaderAlignment, RowColumnDivider, \
-    HeaderColumnDivider, TextAlignment, GridInputColumnDict
+from tablate.helpers.calcs.calc_column_percent import calc_column_percent
+from tablate.helpers.calcs.calc_column_widths import calc_column_widths
+from tablate.helpers.calcs.random_string import random_string
+from tablate.helpers.renderers.console.render_console_foot import render_console_foot
+from tablate.helpers.renderers.console.render_console_frames import render_console_frames
+from tablate.helpers.renderers.console.render_console_head import render_console_head
+from tablate.helpers.renderers.html.render_html_head import render_html_head
+from tablate.type.dict_frame import TextFrameDict, GridFrameDict, TableRowsFrameDict, \
+    TableHeadColumnFrameDict, TableRowsColumnFrameDict, TableHeadFrameDict, FrameDictList
+from tablate.type.dict_options import Options
+from tablate.type.dict_input import GridInputColumnDict, TableInputColumnDict
+from tablate.type.primitives import Border, BaseDivider, TextAlignment, ColumnDivider, HeaderAlignment, \
+    HeaderColumnDivider
 
 
-class TextFrame:
+class Tablate:
 
     # todo: maybe allow align/padding/frame_divider defaults in constructor??
     # todo: allow frame names (will make TextFrame iPython friendly) -- also constructor options `show_frame_names` & `frame_name_align`
     # todo: allow cell level definition of padding/v_line/trunc_value in `add_` constructor objects??? => a lot of fuss and complication for marginal use... v_lines might be useful...
 
     def __init__(self,
-                 border: BaseBorder = "thick",
+                 border_style: Border = "thick",
+                 frame_padding: int = 1,
+                 frame_divider: BaseDivider = "thick",
                  frame_width: int = None,
-                 left_padding: int = 1,
-                 frame_divider: BaseBorder = "thick",
-                 html_block_size: int = 6,
-                 html_character_size: int = 12,
-                 html_width: str = "100%"):
-        self._border = border if border != 'none' else 'blank'
-        self._frame_width = frame_width if frame_width else shutil.get_terminal_size((120 + (left_padding * 2), 0))[0] - (left_padding * 2)
-        self._left_padding = left_padding
-        self._frame_divider = frame_divider
-        self._html_block_size = html_block_size
-        self._html_character_size = html_character_size
-        self._html_width = html_width
-        self._output_frame_list = []
+                 html_px_size: int = 6,
+                 html_text_size: int = 12,
+                 html_frame_width: str = "100%",
+                 html_css_injection: str = ""):
+
+        self._options: Options = {
+            "common": {
+                "border_style": border_style,
+                "frame_padding": frame_padding,
+                "frame_divider": frame_divider,
+                "frame_width": frame_width if frame_width else shutil.get_terminal_size((120 + (frame_padding * 2), 0))[
+                                                                   0] - (frame_padding * 2)
+            },
+            "html": {
+                "px_size": html_px_size,
+                "text_size": html_text_size,
+                "width": html_frame_width,
+                "css": html_css_injection,
+            }
+        }
+
+        self._frame_list: FrameDictList = []
 
 
     def add_text_frame(self,
                        text: Union[str, int, float],
                        multiline: bool = True,
                        max_lines: Optional[int] = None,
                        text_align: TextAlignment = "left",
                        text_padding: int = 1,
-                       frame_base_divider: BaseBorder = "thick",
+                       frame_base_divider: BaseDivider = "thick",
                        trunc_value: str = "..."):
 
-        max_lines = 1 if not multiline else max_lines
-
-        self._output_frame_list.append({
+        text_frame_dict: TextFrameDict = {
             "type": "text",
-            "column_list": [{"width": self._frame_width - 2, "divider": "blank"}],
+            "column_list": [{"width": self._options["common"]["frame_width"] - 2, "divider": "blank"}],
             "string": text,
             "base_divider": frame_base_divider,
             "max_lines": max_lines,
             "align": text_align,
             "padding": text_padding,
             "trunc_value": trunc_value,
-        })
+            "multiline": multiline,
+        }
+
+        self._frame_list.append(text_frame_dict)
 
     def add_grid_frame(self,
                        columns: List[Union[str, GridInputColumnDict]],
                        column_padding: int = 1,
-                       column_divider: RowColumnDivider = "thin",
-                       frame_base_divider: BaseBorder = "thick",
+                       column_divider: ColumnDivider = "thin",
+                       frame_base_divider: BaseDivider = "thick",
                        multiline: bool = True,
                        max_lines: int = None,
                        trunc_value: str = "..."):
 
-        max_lines = 1 if not multiline else max_lines
-
         columns = copy.deepcopy(columns)
 
         grid_column_list = []
 
         for grid_column_item in columns:
             if type(grid_column_item) == str:
                 grid_column_list.append({
-                    "divider": self._frame_divider,
+                    "divider": self._options["common"]["frame_divider"],
                     "string": grid_column_item,
                     "align": "left",
                     "padding": column_padding,
                     "trunc_value": trunc_value,
                 })
             elif type(grid_column_item) == dict:
                 grid_column_item["string"] = grid_column_item["string"]
@@ -92,156 +103,129 @@
                 grid_column_item["align"] = grid_column_item["align"] if "align" in grid_column_item else "left"
                 grid_column_item["padding"] = column_padding
                 grid_column_item["trunc_value"] = trunc_value
                 if "width" in grid_column_item:
                     grid_column_item["width"] = grid_column_item["width"]
                 grid_column_list.append(grid_column_item)
 
-        grid_column_list = calc_column_widths(columns=grid_column_list, frame_width=self._frame_width, column_padding=column_padding)
+        grid_column_list = calc_column_widths(columns=grid_column_list, frame_width=self._options["common"]["frame_width"], column_padding=column_padding)
 
-        self._output_frame_list.append({
+        grid_frame_dict: GridFrameDict = {
             "type": "grid",
             "column_list": grid_column_list,
             "base_divider": frame_base_divider,
-            "max_lines": max_lines
-        })
+            "max_lines": max_lines,
+            "multiline": multiline
+        }
+
+        self._frame_list.append(grid_frame_dict)
 
     def add_table_frame(self,
                         columns: List[TableInputColumnDict],
                         rows: List[Dict[str, Union[str, int, float]]],
                         column_padding: int = 1,
-                        row_line_divider: BaseBorder = "thin",
-                        row_column_divider: RowColumnDivider = "thin",
-                        frame_base_divider: BaseBorder = "thick",
+                        row_line_divider: BaseDivider = "thin",
+                        row_column_divider: ColumnDivider = "thin",
+                        frame_base_divider: BaseDivider = "thick",
                         header_align: HeaderAlignment = "column",
                         header_column_divider: HeaderColumnDivider = "rows",
-                        header_base_divider: BaseBorder = "thick",
-                        hide_header: bool = False):
+                        header_base_divider: BaseDivider = "thick",
+                        multiline: bool = False,
+                        max_lines: int = None,
+                        multiline_header: bool = False,
+                        max_lines_header: int = None,
+                        hide_header: bool = False,
+                        head_trunc_value: str = ".",
+                        row_trunc_value: str = "..."):
 
         columns = copy.deepcopy(columns)
         rows = copy.deepcopy(rows)
 
-        columns = calc_column_widths(columns=columns, frame_width=self._frame_width, column_padding=column_padding)
+        columns = calc_column_widths(columns=columns, frame_width=self._options["common"]["frame_width"], column_padding=column_padding)
 
         header_column_list = []
-        row_column_list = []
+        rows_column_list = []
 
         for column_index, column_item in enumerate(columns):
+            # todo: add optional 'value' key to the column definition... if not used will use key as value
+            column_align_out: TextAlignment = column_item["align"] if "align" in column_item else "left"
+            header_align_out: TextAlignment = header_align if header_align != "column" else column_align_out
 
-            column_align_out = column_item["align"] if "align" in column_item else "left"
-            header_align_out = header_align if header_align != "column" else column_align_out
-
-            column_divider_out = column_item["divider"] if "divider" in column_item else row_column_divider
-            header_divider_out = header_column_divider if header_column_divider != "rows" else column_divider_out
+            column_divider_out: ColumnDivider = column_item["divider"] if "divider" in column_item else row_column_divider
+            header_divider_out: ColumnDivider = header_column_divider if header_column_divider != "rows" else column_divider_out
 
-            header_column_list.append({
+            header_column_dict: TableHeadColumnFrameDict = {
                 "width": column_item["width"],
                 "divider": header_divider_out,
                 "string": column_item["key"],
                 "align": header_align_out,
                 "padding": column_padding,
-                "trunc_value": ".",
-            })
+                "trunc_value": head_trunc_value,
+            }
 
-            row_column_list.append({
+            header_column_list.append(header_column_dict)
+
+            rows_column_dict: TableRowsColumnFrameDict = {
                 "width": column_item["width"],
                 "divider": column_divider_out,
                 "key": column_item["key"],
                 "align": column_align_out,
                 "padding": column_padding,
-                "trunc_value": "...",
-            })
+                "trunc_value": row_trunc_value,
+            }
+
+            rows_column_list.append(rows_column_dict)
 
         if not hide_header:
-            self._output_frame_list.append({
+
+            header_frame_dict: TableHeadFrameDict = {
                 "type": "table-head",
                 "column_list": header_column_list,
                 "base_divider": header_base_divider,
-                "max_lines": 1
-            })
+                "max_lines": max_lines_header,
+                "multiline": multiline_header
+            }
+
+            self._frame_list.append(header_frame_dict)
 
         # todo: check row keys all in place and give nice errors => validators
 
-        self._output_frame_list.append({
-            "type": "table",
-            "column_list": row_column_list,
+        rows_frame_dict: TableRowsFrameDict = {
+            "type": "table-body",
+            "column_list": rows_column_list,
             "table_row_list": rows,
             "row_line_divider": row_line_divider,
             "base_divider": frame_base_divider,
-        })
+            "max_lines": max_lines,
+            "multiline": multiline
+        }
+
+        self._frame_list.append(rows_frame_dict)
 
     def to_string(self):
         return_string = ""
-
-        if len(self._output_frame_list) > 0:
-            top_border_inner = row_frame_divider(divider=self._border,
-                                                 column_list_top=[],
-                                                 column_list_bottom=self._output_frame_list[0]["column_list"])
-            return_string += f"{' ' * self._left_padding}{top_left[self._border]}{top_border_inner}{top_right[self._border]}\n"
-            for frame_index, frame_item in enumerate(self._output_frame_list):
-                if frame_item["type"] == "text":
-                    return_string += render_text_frame_string(text_frame_dict=frame_item,
-                                                              frame_border=self._border,
-                                                              left_padding=self._left_padding)
-                if frame_item["type"] == "grid" or  frame_item["type"] == "table-head":
-                    if frame_item["max_lines"] == 1:
-                        return_string += render_single_line_grid(column_list=frame_item,
-                                                                 frame_border=self._border,
-                                                                 left_padding=self._left_padding)
-                    else:
-                        return_string += render_multi_line_grid(column_list=frame_item,
-                                                                 frame_border=self._border,
-                                                                 left_padding=self._left_padding)
-                if frame_item["type"] == "table-body":
-                    return_string += render_table_frame_string(table_dict=frame_item,
-                                                               frame_border=self._border,
-                                                               left_padding=self._left_padding)
-                if not is_last_element(frame_index, self._output_frame_list):
-                    if self._output_frame_list[frame_index]['base_divider'] != 'none':
-                        frame_divider_inner = row_frame_divider(divider=self._output_frame_list[frame_index]["base_divider"],
-                                          column_list_top=self._output_frame_list[frame_index]["column_list"],
-                                          column_list_bottom=self._output_frame_list[frame_index + 1]["column_list"])
-                        frame_divider_outer = row_outer_border(row_string=frame_divider_inner,
-                                                               outer_border=self._border,
-                                                               row_divider=self._output_frame_list[frame_index]['base_divider'])
-                        return_string += f"{' ' * self._left_padding}{frame_divider_outer}\n"
-
-            bottom_border_inner = row_frame_divider(divider=self._border,
-                                                    column_list_top=self._output_frame_list[-1]["column_list"],
-                                                    column_list_bottom=[])
-            return_string += f"{' ' * self._left_padding}{bottom_left[self._border]}{bottom_border_inner}{bottom_right[self._border]}\n"
-
+        if len(self._frame_list) > 0:
+            return_string += render_console_head(frame_list=self._frame_list, options=self._options)
+            return_string += render_console_frames(frame_list=self._frame_list, options=self._options)
+            return_string += render_console_foot(frame_list=self._frame_list, options=self._options)
         return return_string
 
     def print(self):
         print(self.to_string())
 
     def __repr__(self):
         return self.to_string()
 
     def to_html(self):
+        self._options["html"]["uid"] = random_string(6)
+        frame_list, self._options["html"]["column_widths"] = calc_column_percent(frame_list=self._frame_list,
+                                                                                 frame_width=self._options["common"]["frame_width"])
+
         return_html = ""
-        frame_list, column_widths = calc_column_percent(self._output_frame_list, self._frame_width)
-        return_html += render_html_head(frame_list=frame_list,
-                                        column_widths=column_widths,
-                                        html_width=self._html_width,
-                                        outer_border=self._border,
-                                        left_padding=self._left_padding,
-                                        html_block_size=self._html_block_size)
-        for frame_item in frame_list:
-            if frame_item["type"] == "text":
-                print("here be text")
-            if frame_item["type"] == "grid" or frame_item["type"] == "table-head":
-                if frame_item["max_lines"] == 1:
-                    print("here be grid single")
-                else:
-                    print("here be grid multi")
-            if frame_item["type"] == "table-head":
-                print("here be table head")
-            if frame_item["type"] == "table-body":
-                print("here be table body")
-        print(return_html)
+
+        return_html += render_html_head(options=self._options)
+
 
     def _repr_html_(self):
         return self.to_html()
```

### Comparing `tablate-0.0.1/textframe/characters/matrix_cross.py` & `tablate-0.0.2/tablate/characters/matrix_cross.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             "double": "╦"
         }
     },
     "thin": {
         "blank": {
             "blank": " ",
             "thin": "│",
-            "thick": "┃",
+            "thick": "╽",
             "double": "║"
         },
         "thin": {
             "blank": "┴",
             "thin": "┼",
             "thick": "╁",
             "double": "╁"
@@ -50,17 +50,17 @@
             "thick": "╬",
             "double": "╬"
         }
     },
     "thick": {
         "blank": {
             "blank": " ",
-            "thin": " ",
-            "thick": " ",
-            "double": " "
+            "thin": "╿",
+            "thick": "┃",
+            "double": "║"
         },
         "thin": {
             "blank": "┸",
             "thin": "╀",
             "thick": "╂",
             "double": "╂"
         },
@@ -76,17 +76,17 @@
             "thick": "╬",
             "double": "╬"
         }
     },
     "double": {
         "blank": {
             "blank": " ",
-            "thin": " ",
-            "thick": " ",
-            "double": " "
+            "thin": "║",
+            "thick": "║",
+            "double": "║"
         },
         "thin": {
             "blank": "╨",
             "thin": "╀",
             "thick": "╂",
             "double": "╫"
         },
```

### Comparing `tablate-0.0.1/textframe/characters/matrix_side.py` & `tablate-0.0.2/tablate/characters/matrix_side.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.1/textframe/helpers/calcs/calc_column_percent.py` & `tablate-0.0.2/tablate/helpers/calcs/calc_column_percent.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     frame_list = copy.deepcopy(frame_list)
     baseline_width_set = set()
     frame_width = frame_width - 1
     for frame_item in frame_list:
         frame_width_total = 0
         for column_item in frame_item["column_list"]:
             frame_width_total += column_item["width"] + 1
-            column_width = math.floor((100 / frame_width) * frame_width_total)
-            baseline_width_set.add(math.floor(column_width))
-            column_item["width_percent"] = column_width
+            acc_column_width = math.floor((100 / frame_width) * frame_width_total)
+            baseline_width_set.add(math.floor(acc_column_width))
+            column_item["baseline_width_percent"] = acc_column_width
     sorted_baseline_array = sorted(baseline_width_set)
     column_widths = []
-    for baselines_index, _ in enumerate(sorted_baseline_array):
-        if baselines_index > 0:
-            column_widths.append(sorted_baseline_array[baselines_index] - sorted_baseline_array[baselines_index - 1])
-        else:
-            column_widths.append(sorted_baseline_array[baselines_index])
-    return frame_list, column_widths
+    # for baselines_index, _ in enumerate(sorted_baseline_array):
+    #     if baselines_index > 0:
+    #         column_widths.append(sorted_baseline_array[baselines_index] - sorted_baseline_array[baselines_index - 1])
+    #     else:
+    #         column_widths.append(sorted_baseline_array[baselines_index])
+    return frame_list, sorted_baseline_array
```

### Comparing `tablate-0.0.1/textframe/helpers/calcs/calc_column_widths.py` & `tablate-0.0.2/tablate/helpers/calcs/calc_column_widths.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.1/textframe/helpers/formatters/string/cell_string.py` & `tablate-0.0.2/tablate/helpers/formatters/console/cell_string.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import List, Optional
 
-from textframe.typing import TextAlignment
+from tablate.type.primitives import TextAlignment
 
 
 def cell_string_single_line(string: str,
                             width: int,
                             padding: int,
                             align: TextAlignment,
                             trunc_value: str = "...") -> str:
@@ -67,15 +67,15 @@
     reached_max_lines = False
 
     for initial_string_item in initial_string_array:
         word_string_array = initial_string_item.split(" ")
         character_count = 0
         current_line_array = []
         for word_string_index, word_string_item in enumerate(word_string_array):
-            last_line = max_lines and len(return_string_array) == max_lines - 1
+            last_line = max_lines is not None and len(return_string_array) == max_lines - 1
             character_count += len(word_string_item)
             if (character_count + (padding * 2) < width) or (last_line and character_count + (padding * 2) < width + len(trunc_value)):
                 current_line_array.append(word_string_item)
             else:
                 if last_line:
                     current_line_array.append(word_string_item)
                     current_line_string = " ".join(current_line_array)
```

### Comparing `tablate-0.0.1/textframe/helpers/formatters/string/row_frame_divider.py` & `tablate-0.0.2/tablate/helpers/formatters/console/row_divider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
 
-from textframe.characters.line_h import h_line
-from textframe.characters.matrix_cross import cross_matrix
-from textframe.typing import BaseBorder
+from tablate.characters.line_h import h_line
+from tablate.characters.matrix_cross import cross_matrix
+from tablate.type.dict_options import Options
+from tablate.type.primitives import BaseDivider
 
 
-def row_frame_divider(divider: BaseBorder, column_list_top: list, column_list_bottom: list) -> str:
+def row_divider(column_list_top: list, column_list_bottom: list, divider: BaseDivider) -> str:
 
     """
     :param divider: BorderType
     :param column_list_top: [[col_width, BorderType]]
     :param column_list_bottom: [[col_width, BorderType]]
     :return: str
     """
```

### Comparing `tablate-0.0.1/textframe/tests/test_decs.py` & `tablate-0.0.2/tablate/tests/test_decs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,67 @@
-import textframe as tf
-from textframe.tests.test_defs import column_list1, row_list1, column_list2a, row_list2, column_list2b, column_list2c, \
-    column_list3, column_list4, column_list5
+import tablate as tf
+from tablate.tests.test_defs import column_list1, row_list1, column_list2a, row_list2, column_list2b, column_list2c, \
+    column_list3, column_list4, column_list5, really_long_string
 
-new_frame = tf.TextFrame(border="thin")
+new_frame = tf.Tablate(border_style="double")
 
 new_frame.add_table_frame(column_list1, row_list1)
 
+new_frame.add_table_frame(column_list1, row_list1, multiline=True)
+new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=3)
+new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=6)
+new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=100)
+new_frame.add_table_frame(column_list1, row_list1, max_lines=100)
+
+new_frame.add_table_frame(column_list1, row_list1, multiline_header=True)
+new_frame.add_table_frame(column_list1, row_list1, multiline_header=True, max_lines_header=2)
+new_frame.add_table_frame(column_list1, row_list1, multiline_header=True, max_lines_header=100)
+new_frame.add_table_frame(column_list1, row_list1, max_lines_header=100)
+
+
 new_frame.add_text_frame("Default text")
 
-new_frame.add_text_frame("Example text frame with left indentation", multiline=False,text_align="left")
+new_frame.add_text_frame(really_long_string)
+new_frame.add_text_frame(really_long_string, multiline=True)
+
+new_frame.add_text_frame(really_long_string, multiline=False)
+new_frame.add_text_frame(really_long_string, max_lines=6)
+
+new_frame.add_text_frame(really_long_string, multiline=True, max_lines=6)
+new_frame.add_text_frame(really_long_string, multiline=True, max_lines=100)
+
+new_frame.add_text_frame(really_long_string, multiline=False, max_lines=6)
+new_frame.add_text_frame(really_long_string, multiline=False, max_lines=100)
+
+new_frame.add_text_frame("Example text frame with left indentation", multiline=False,text_align="left", max_lines=100)
 new_frame.add_text_frame("Example text frame with center indentation", multiline=False,text_align="center")
 new_frame.add_text_frame("Example text frame with right indentation", multiline=False,text_align="right")
 
 new_frame.add_text_frame(666)
 
-really_long_string = "Commodo elit at imperdiet dui accumsan sit amet nulla. Sodales neque sodales ut etiam sit amet nisl purus. Convallis posuere morbi leo urna molestie at elementum. Enim nunc faucibus a pellentesque sit amet porttitor. Enim nulla aliquet porttitor lacus luctus accumsan tortor. Ullamcorper velit sed ullamcorper morbi. Sit amet porttitor eget dolor morbi non arcu. Eget mauris pharetra et ultrices neque ornare aenean euismod elementum. Euismod lacinia at quis risus sed vulputate odio. Varius quam quisque id diam. Habitant morbi tristique senectus et netus et malesuada fames ac. Ornare quam viverra orci sagittis eu volutpat odio. Nisl suscipit adipiscing bibendum est ultricies. Adipiscing elit pellentesque habitant morbi tristique senectus. Tellus cras adipiscing enim eu turpis egestas pretium aenean pharetra. At consectetur lorem donec massa sapien faucibus et molestie. Neque ornare aenean euismod elementum nisi quis eleifend quam. A arcu cursus vitae congue mauris."
 
-new_frame.add_text_frame(really_long_string, multiline=False)
-new_frame.add_text_frame(really_long_string, max_lines=3)
+
 
 new_frame.add_text_frame(really_long_string)
 
 new_frame.add_table_frame(column_list2a, row_list2, row_column_divider="blank", row_line_divider="none")
 
-new_frame.add_table_frame(column_list2b, row_list2, row_column_divider="double", row_line_divider="double")
+new_frame.add_table_frame(column_list2b, row_list2, row_column_divider="double", row_line_divider="double", frame_base_divider="blank")
+
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="blank", header_base_divider="thin", header_column_divider="double", frame_base_divider="thin")
 
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="double", row_line_divider="thin", header_base_divider="double", header_column_divider="double")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="none", header_base_divider="none", header_column_divider="double", frame_base_divider="double")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thin", row_line_divider="thin", header_base_divider="thin", header_column_divider="double", frame_base_divider="thick")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thick", row_line_divider="thick", header_base_divider="thick", header_column_divider="double", frame_base_divider="thin")
 
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thick", row_line_divider="thick", header_base_divider="thin", header_column_divider="double")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="double", row_line_divider="double", header_base_divider="double", header_column_divider="double", frame_base_divider="none")
+new_frame.add_table_frame(column_list2c, row_list2)
 
 new_frame.add_grid_frame(column_list3, max_lines=1)
-new_frame.add_grid_frame(column_list4, max_lines=6)
+new_frame.add_grid_frame(column_list4, max_lines=100)
 new_frame.add_grid_frame(column_list4)
 new_frame.add_grid_frame(column_list5)
 
 some_set = {1,2,3}
 some_set.add(1)
 
 some_set.add(4)
```

### Comparing `tablate-0.0.1/textframe/tests/test_defs.py` & `tablate-0.0.2/tablate/tests/test_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import List, Dict
 
 column_list1 = [
     {
-        "key": "Key One",
+        "key": "A really really long key like this - maybe even longer",
         "width":  30
     },
     {
         "key": "Key Two"
     },
     {
         "key": "Key Three",
         "width": 20
     }
 ]
 
 row_list1 = [
     {
-        "Key One": "Row One Column One",
-        "Key Two": "Row One Column Two",
-        "Key Three": "Row One Column Three"
+        "A really really long key like this - maybe even longer": "Quam elementum pulvinar etiam non quam lacus suspendisse faucibus. Enim nec dui nunc mattis enim ut tellus. Est placerat in egestas erat imperdiet sed euismod nisi porta. At tempor commodo ullamcorper a lacus vestibulum sed. Porta nibh venenatis cras sed. Cras sed felis eget velit aliquet sagittis id consectetur. Aliquam id diam maecenas ultricies mi. ",
+        "Key Two": "Quam elementum pulvinar etiam non quam lacus suspendisse faucibus. Enim nec dui nunc mattis enim ut tellus. Est placerat in egestas erat imperdiet sed euismod nisi porta. At tempor commodo ullamcorper a lacus vestibulum sed. Porta nibh venenatis cras sed. Cras sed felis eget velit aliquet sagittis id consectetur. Aliquam id diam maecenas ultricies mi. ",
+        "Key Three": "Quam elementum pulvinar etiam non quam lacus suspendisse faucibus. Enim nec dui nunc mattis enim ut tellus. Est placerat in egestas erat imperdiet sed euismod nisi porta. At tempor commodo ullamcorper a lacus vestibulum sed. Porta nibh venenatis cras sed. Cras sed felis eget velit aliquet sagittis id consectetur. Aliquam id diam maecenas ultricies mi. ",
 
     },
     {
-        "Key One": "Row Two Column Two",
+        "A really really long key like this - maybe even longer": "Row Two Column Two",
         "Key Two": "Row Two Column Two",
         "Key Three": "Row Two Column Three"
 
     },
     {
-        "Key One": "Row Three Column One",
+        "A really really long key like this - maybe even longer": "Row Three Column One",
         "Key Two": "Row Three Column Two",
         "Key Three": "Row Three Column Three"
 
     },
 ]
 
 column_list2a = [
@@ -72,15 +72,15 @@
         "key": "Key One",
         "width": "30%",
         "divider": "thick"
     },
     {
         "key": "Key Two",
         "align": "right",
-        "divider": "thick"
+        "divider": "thin"
     },
     {
         "key": "Key Three",
         "align": "right"
     }
 ]
```

