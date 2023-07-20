# Comparing `tmp/metabolights_utils-0.9.5.tar.gz` & `tmp/metabolights_utils-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolights_utils-0.9.5.tar", max compression
+gzip compressed data, was "metabolights_utils-0.9.6.tar", max compression
```

## Comparing `metabolights_utils-0.9.5.tar` & `metabolights_utils-0.9.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.5/LICENSE
--rw-r--r--   0        0        0    14366 2023-07-19 20:51:58.143530 metabolights_utils-0.9.5/README.md
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.5/metabolights_utils/__init__.py
--rw-r--r--   0        0        0      244 2023-07-19 00:16:47.503397 metabolights_utils-0.9.5/metabolights_utils/common.py
--rw-r--r--   0        0        0     2198 2023-07-19 09:21:04.692280 metabolights_utils-0.9.5/metabolights_utils/isatab/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.5/metabolights_utils/isatab/default/__init__.py
--rw-r--r--   0        0        0      716 2023-07-19 00:16:47.532744 metabolights_utils-0.9.5/metabolights_utils/isatab/default/assay_file.py
--rw-r--r--   0        0        0     1268 2023-07-19 00:16:47.587091 metabolights_utils-0.9.5/metabolights_utils/isatab/default/assignment_file.py
--rw-r--r--   0        0        0     1536 2023-07-19 00:16:47.626096 metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_file.py
--rw-r--r--   0        0        0     5878 2023-07-20 09:45:20.078824 metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_table_file.py
--rw-r--r--   0        0        0     1881 2023-07-19 09:14:50.131288 metabolights_utils-0.9.5/metabolights_utils/isatab/default/factory.py
--rw-r--r--   0        0        0    11163 2023-07-19 00:16:47.792874 metabolights_utils-0.9.5/metabolights_utils/isatab/default/investigation_file.py
--rw-r--r--   0        0        0      706 2023-07-19 00:16:47.861855 metabolights_utils-0.9.5/metabolights_utils/isatab/default/sample_file.py
--rw-r--r--   0        0        0     1488 2023-07-19 00:16:47.917232 metabolights_utils-0.9.5/metabolights_utils/isatab/default/writer.py
--rw-r--r--   0        0        0     9845 2023-07-20 09:45:19.894271 metabolights_utils-0.9.5/metabolights_utils/isatab/reader.py
--rw-r--r--   0        0        0     3692 2023-07-19 00:16:47.939412 metabolights_utils-0.9.5/metabolights_utils/isatab/writer.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.5/metabolights_utils/models/__init__.py
--rw-r--r--   0        0        0      442 2023-07-19 00:16:47.972240 metabolights_utils-0.9.5/metabolights_utils/models/common.py
--rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.5/metabolights_utils/models/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.5/metabolights_utils/models/isa/__init__.py
--rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.5/metabolights_utils/models/isa/assay_file.py
--rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.5/metabolights_utils/models/isa/assignment_file.py
--rw-r--r--   0        0        0     9506 2023-07-20 09:50:31.746316 metabolights_utils-0.9.5/metabolights_utils/models/isa/common.py
--rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.5/metabolights_utils/models/isa/enums.py
--rw-r--r--   0        0        0    11080 2023-07-19 00:16:48.173059 metabolights_utils-0.9.5/metabolights_utils/models/isa/investigation_file.py
--rw-r--r--   0        0        0    18440 2023-07-20 09:45:19.894366 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/common.py
--rw-r--r--   0        0        0    22198 2023-07-19 00:16:48.338368 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/investigation_parser.py
--rw-r--r--   0        0        0    18265 2023-07-20 09:45:18.997818 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/isa_table_parser.py
--rw-r--r--   0        0        0      457 2023-07-19 00:16:48.411630 metabolights_utils-0.9.5/metabolights_utils/models/isa/samples_file.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.5/metabolights_utils/models/metabolights/__init__.py
--rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.5/metabolights_utils/models/metabolights/metabolights_study.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.5/metabolights_utils/models/parser/__init__.py
--rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.5/metabolights_utils/models/parser/common.py
--rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.5/metabolights_utils/models/parser/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.5/metabolights_utils/tsv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/__init__.py
--rw-r--r--   0        0        0     3559 2023-07-19 08:23:28.339563 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_column.py
--rw-r--r--   0        0        0     3488 2023-07-19 08:26:08.140976 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_row.py
--rw-r--r--   0        0        0     1339 2023-07-19 07:58:19.960337 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/base.py
--rw-r--r--   0        0        0     3390 2023-07-19 08:23:28.347823 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_column.py
--rw-r--r--   0        0        0     3144 2023-07-19 08:23:28.383070 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_row.py
--rw-r--r--   0        0        0     2492 2023-07-19 08:23:28.528233 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_column.py
--rw-r--r--   0        0        0     1986 2023-07-19 09:13:04.618046 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_row.py
--rw-r--r--   0        0        0     2867 2023-07-19 08:23:28.613461 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_column.py
--rw-r--r--   0        0        0     3363 2023-07-19 08:23:28.672360 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_row.py
--rw-r--r--   0        0        0     3157 2023-07-19 08:23:28.701280 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_cell.py
--rw-r--r--   0        0        0     3544 2023-07-19 09:13:21.371457 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column.py
--rw-r--r--   0        0        0     2077 2023-07-19 09:13:17.513241 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column_header.py
--rw-r--r--   0        0        0     2229 2023-07-19 08:23:28.847528 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_row.py
--rw-r--r--   0        0        0    19935 2023-07-20 13:14:00.106647 metabolights_utils-0.9.5/metabolights_utils/tsv/filter.py
--rw-r--r--   0        0        0     6043 2023-07-19 09:10:39.601796 metabolights_utils-0.9.5/metabolights_utils/tsv/model.py
--rw-r--r--   0        0        0    12899 2023-07-20 13:14:20.411943 metabolights_utils-0.9.5/metabolights_utils/tsv/sort.py
--rw-r--r--   0        0        0     5647 2023-07-19 08:26:02.864303 metabolights_utils-0.9.5/metabolights_utils/tsv/tsv_file_updater.py
--rw-r--r--   0        0        0     1310 2023-07-20 13:15:57.573603 metabolights_utils-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    15350 1970-01-01 00:00:00.000000 metabolights_utils-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.6/LICENSE
+-rw-r--r--   0        0        0    17013 2023-07-20 14:29:23.829603 metabolights_utils-0.9.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.6/metabolights_utils/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-19 00:16:47.503397 metabolights_utils-0.9.6/metabolights_utils/common.py
+-rw-r--r--   0        0        0     2198 2023-07-19 09:21:04.692280 metabolights_utils-0.9.6/metabolights_utils/isatab/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.6/metabolights_utils/isatab/default/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-19 00:16:47.532744 metabolights_utils-0.9.6/metabolights_utils/isatab/default/assay_file.py
+-rw-r--r--   0        0        0     1268 2023-07-19 00:16:47.587091 metabolights_utils-0.9.6/metabolights_utils/isatab/default/assignment_file.py
+-rw-r--r--   0        0        0     1536 2023-07-19 00:16:47.626096 metabolights_utils-0.9.6/metabolights_utils/isatab/default/base_isa_file.py
+-rw-r--r--   0        0        0     5878 2023-07-20 09:45:20.078824 metabolights_utils-0.9.6/metabolights_utils/isatab/default/base_isa_table_file.py
+-rw-r--r--   0        0        0     1881 2023-07-19 09:14:50.131288 metabolights_utils-0.9.6/metabolights_utils/isatab/default/factory.py
+-rw-r--r--   0        0        0    11163 2023-07-19 00:16:47.792874 metabolights_utils-0.9.6/metabolights_utils/isatab/default/investigation_file.py
+-rw-r--r--   0        0        0      706 2023-07-19 00:16:47.861855 metabolights_utils-0.9.6/metabolights_utils/isatab/default/sample_file.py
+-rw-r--r--   0        0        0     1488 2023-07-19 00:16:47.917232 metabolights_utils-0.9.6/metabolights_utils/isatab/default/writer.py
+-rw-r--r--   0        0        0     9845 2023-07-20 09:45:19.894271 metabolights_utils-0.9.6/metabolights_utils/isatab/reader.py
+-rw-r--r--   0        0        0     3692 2023-07-19 00:16:47.939412 metabolights_utils-0.9.6/metabolights_utils/isatab/writer.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.6/metabolights_utils/models/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-19 00:16:47.972240 metabolights_utils-0.9.6/metabolights_utils/models/common.py
+-rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.6/metabolights_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.6/metabolights_utils/models/isa/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.6/metabolights_utils/models/isa/assay_file.py
+-rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.6/metabolights_utils/models/isa/assignment_file.py
+-rw-r--r--   0        0        0     9506 2023-07-20 09:50:31.746316 metabolights_utils-0.9.6/metabolights_utils/models/isa/common.py
+-rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.6/metabolights_utils/models/isa/enums.py
+-rw-r--r--   0        0        0    11080 2023-07-19 00:16:48.173059 metabolights_utils-0.9.6/metabolights_utils/models/isa/investigation_file.py
+-rw-r--r--   0        0        0    18440 2023-07-20 09:45:19.894366 metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/common.py
+-rw-r--r--   0        0        0    22198 2023-07-19 00:16:48.338368 metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/investigation_parser.py
+-rw-r--r--   0        0        0    18265 2023-07-20 09:45:18.997818 metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/isa_table_parser.py
+-rw-r--r--   0        0        0      457 2023-07-19 00:16:48.411630 metabolights_utils-0.9.6/metabolights_utils/models/isa/samples_file.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.6/metabolights_utils/models/metabolights/__init__.py
+-rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.6/metabolights_utils/models/metabolights/metabolights_study.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.6/metabolights_utils/models/parser/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.6/metabolights_utils/models/parser/common.py
+-rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.6/metabolights_utils/models/parser/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.6/metabolights_utils/tsv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/__init__.py
+-rw-r--r--   0        0        0     3559 2023-07-19 08:23:28.339563 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/add_column.py
+-rw-r--r--   0        0        0     3488 2023-07-19 08:26:08.140976 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/add_row.py
+-rw-r--r--   0        0        0     1339 2023-07-19 07:58:19.960337 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/base.py
+-rw-r--r--   0        0        0     3390 2023-07-19 08:23:28.347823 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/copy_column.py
+-rw-r--r--   0        0        0     3144 2023-07-19 08:23:28.383070 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/copy_row.py
+-rw-r--r--   0        0        0     2492 2023-07-19 08:23:28.528233 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/delete_column.py
+-rw-r--r--   0        0        0     1986 2023-07-19 09:13:04.618046 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/delete_row.py
+-rw-r--r--   0        0        0     2867 2023-07-19 08:23:28.613461 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/move_column.py
+-rw-r--r--   0        0        0     3363 2023-07-19 08:23:28.672360 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/move_row.py
+-rw-r--r--   0        0        0     3157 2023-07-19 08:23:28.701280 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_cell.py
+-rw-r--r--   0        0        0     3544 2023-07-19 09:13:21.371457 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_column.py
+-rw-r--r--   0        0        0     2077 2023-07-19 09:13:17.513241 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_column_header.py
+-rw-r--r--   0        0        0     2229 2023-07-19 08:23:28.847528 metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_row.py
+-rw-r--r--   0        0        0    19935 2023-07-20 13:14:00.106647 metabolights_utils-0.9.6/metabolights_utils/tsv/filter.py
+-rw-r--r--   0        0        0     6043 2023-07-19 09:10:39.601796 metabolights_utils-0.9.6/metabolights_utils/tsv/model.py
+-rw-r--r--   0        0        0    12899 2023-07-20 13:14:20.411943 metabolights_utils-0.9.6/metabolights_utils/tsv/sort.py
+-rw-r--r--   0        0        0     5647 2023-07-19 08:26:02.864303 metabolights_utils-0.9.6/metabolights_utils/tsv/tsv_file_updater.py
+-rw-r--r--   0        0        0     1310 2023-07-20 14:29:34.570867 metabolights_utils-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    17997 1970-01-01 00:00:00.000000 metabolights_utils-0.9.6/PKG-INFO
```

### Comparing `metabolights_utils-0.9.5/LICENSE` & `metabolights_utils-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/README.md` & `metabolights_utils-0.9.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -9,43 +9,63 @@
 ![Python](https://img.shields.io/badge/Python-3.8%7C3.9-dark_blue)
 ![Coverage](https://img.shields.io/badge/Coverage-80%25-dark_blue)
 
 # MetaboLights Utils Library
 MetaboLigts-utils is a lightweight library to read and validate ISA files. 
 
 Selected features:
-1. Read and update ISA investigation files. Reading investigation files has *no pandas library dependency*.
+1. Read and update ISA files without *pandas library dependency*.
 2. Read tab seperated ISA files (s_*.txt, a_*.txt, m_*.txt) with **pagination support**.
+    * Update page size (number of rows in a page) and read results with the selected page size.
+    * Define custom row offset and read rows with a limit. Row indices in a page can be unordered after filter and sort operations. You can get actual row index of the selected row using result.
+    * Read only the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined, they will be in result. Column names may be different than header if there are multiple column with same header. 
+    * If no column selected, columns will be ordered. If columns are selected, result will contain columns in the selected order. You can get actual column index of a column using result.
 3. Apply **multi-column filters and sort options** before reading ISA table files. 
-    * Multiple sort options can be defined for different columns. For example; sort by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. Moreover, columns can be sorted as different data type (if column values are valid for the selected data type). Supported data types are str, int, float and datetime. 
+    * Case sensitive or case insensitive multi-column sort is supported.
+        - Multi-column sorts with ascending and descending order can be defined. For example; You can sort  by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. 
+        - Columns can be sorted as different data type. Supported sort data types are str, int, float and datetime. datetime pattern can be defined for datetime data type.
+        - Sort orders for invalid and empty values can be defined. For example, If sort value order is defined as VALID_EMPTY_INVALID, invalid values will follow empty values and empty values will follow valid values. This value order option is applicable for int, datetime and float data types. All combinations are poossible for EMPTY, INVALID, VALID values.
+        - You can define your custom sorters. "enum-sorter" as a custom sorter has been already implemented. It sorts enums with given string values.
     * There are **10 different filters** (with inverse options). Any filter can be applied to any column. Multiple filters can be defined. 
         - CONTAINS / NOT CONTAINS
         - EQUAL / NOT EQUAL
         - STARTSWITH / NOT STARTSWITH
         - ENDSWITH / NOT ENDSWITH
         - GREATER / NOT GREATER
         - GREATER_EQUAL / NOT GREATER_EQUAL
         - LESS / NOT LESS
         - LESS_EQUAL / NOT LESS_EQUAL
         - REGEX (regex match) / NOT REGEX (not regex match)
         - EMPTY / NOT EMPTY (None or empty)
+    * You can define multiple filters. If one filter rejects row, row will not be selected (AND operation).
+    * You can define one or more columns for a filter. If there are multiple columns for a filter. If any column matches the parameter, filter selects the row (OR operation).
+    * If you do not select any column for filter, filter will evaluate all columns of the row. If filter matches the parameter with any column, it will select the row. You can define column names to skip them while evaluating all rows. 
+    * You can define your custom filters. Some custom filters have been already implemented.
+        - "between-equal": Returns row if value between given min and max. Min and max inputs can be datetime, str, int or float.
+        - "valid-datetime" Return row if value is valid datetime with given pattern. Default pattern is DD/MM/YYYY.
+        - "valid-number": Return row if value is valid int or float.
+        - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum-mapped text. Enums can be any allowed type (str, int, etc.).
+            + Example: Enum values are 1, 2, 3, 4. Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 and 4 will be returned.
+
 4. Define and **apply actions** to manuplate ISA table files. Supported operations:
     * ADD_ROW: Insert rows to given index
     * DELETE_ROW: delete selected rows
     * MOVE_ROW: move row to new index
     * ADD_COLUMN: Add new column
     * DELETE_COLUMN: delete selected columns
     * MOVE_COLUMN: move column to new index
     * COPY_ROW: copy row data to other selected rows
     * COPY_COLUMN: copy column data to other selected columns
     * UPDATE_ROW_DATA: update selected rows
     * UPDATE_COLUMN_DATA: selected columns
     * UPDATE_COLUMN_HEADER: update column headers
     * UPDATE_CELL_DATA: update cells given with row and column index
 
+
+
 ### Investigation file operations
 
 Read and update an investigation file
 ```python 
 import os
 import pathlib
 import uuid
```

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/__init__.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/__init__.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/assay_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/assignment_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/assignment_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/base_isa_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_table_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/base_isa_table_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/factory.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/factory.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/investigation_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/investigation_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/sample_file.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/sample_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/default/writer.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/default/writer.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/reader.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/reader.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/isatab/writer.py` & `metabolights_utils-0.9.6/metabolights_utils/isatab/writer.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/assay_file.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/common.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/investigation_file.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/investigation_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/common.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/investigation_parser.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/investigation_parser.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/isa_table_parser.py` & `metabolights_utils-0.9.6/metabolights_utils/models/isa/parser/isa_table_parser.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/metabolights/metabolights_study.py` & `metabolights_utils-0.9.6/metabolights_utils/models/metabolights/metabolights_study.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/models/parser/common.py` & `metabolights_utils-0.9.6/metabolights_utils/models/parser/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_column.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/add_column.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_row.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/add_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/base.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/base.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_column.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/copy_column.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_row.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/copy_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_column.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/delete_column.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_row.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/delete_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_column.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/move_column.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_row.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/move_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_cell.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_cell.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_column.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column_header.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_column_header.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_row.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/actions/update_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/filter.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/filter.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/model.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/model.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/sort.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/sort.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/metabolights_utils/tsv/tsv_file_updater.py` & `metabolights_utils-0.9.6/metabolights_utils/tsv/tsv_file_updater.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.5/pyproject.toml` & `metabolights_utils-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabolights-utils"
-version = "0.9.5"
+version = "0.9.6"
 description = "Metabolights common models, utility methods and classes for python-based Metabolights projects."
 authors = ["Ozgur Yurekten <ozgur@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "metabolights_utils"}]
 license = "Apache-2.0"
 homepage = "https://github.com/EBI-Metabolights"
 repository = "https://github.com/EBI-Metabolights/metabolights-utils"
```

### Comparing `metabolights_utils-0.9.5/PKG-INFO` & `metabolights_utils-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolights-utils
-Version: 0.9.5
+Version: 0.9.6
 Summary: Metabolights common models, utility methods and classes for python-based Metabolights projects.
 Home-page: https://github.com/EBI-Metabolights
 License: Apache-2.0
 Keywords: metabolights,metabolomics,ISA data model
 Author: Ozgur Yurekten
 Author-email: ozgur@ebi.ac.uk
 Requires-Python: >=3.8.1,<3.9
@@ -32,43 +32,63 @@
 ![Python](https://img.shields.io/badge/Python-3.8%7C3.9-dark_blue)
 ![Coverage](https://img.shields.io/badge/Coverage-80%25-dark_blue)
 
 # MetaboLights Utils Library
 MetaboLigts-utils is a lightweight library to read and validate ISA files. 
 
 Selected features:
-1. Read and update ISA investigation files. Reading investigation files has *no pandas library dependency*.
+1. Read and update ISA files without *pandas library dependency*.
 2. Read tab seperated ISA files (s_*.txt, a_*.txt, m_*.txt) with **pagination support**.
+    * Update page size (number of rows in a page) and read results with the selected page size.
+    * Define custom row offset and read rows with a limit. Row indices in a page can be unordered after filter and sort operations. You can get actual row index of the selected row using result.
+    * Read only the selected columns you defined. If a selected column has additional columns (Term Source REF, etc) and these columns are not defined, they will be in result. Column names may be different than header if there are multiple column with same header. 
+    * If no column selected, columns will be ordered. If columns are selected, result will contain columns in the selected order. You can get actual column index of a column using result.
 3. Apply **multi-column filters and sort options** before reading ISA table files. 
-    * Multiple sort options can be defined for different columns. For example; sort by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. Moreover, columns can be sorted as different data type (if column values are valid for the selected data type). Supported data types are str, int, float and datetime. 
+    * Case sensitive or case insensitive multi-column sort is supported.
+        - Multi-column sorts with ascending and descending order can be defined. For example; You can sort  by 'Parameter Value\[Gender\]' as ascending and Parameter Value\[Age\] as descending order. 
+        - Columns can be sorted as different data type. Supported sort data types are str, int, float and datetime. datetime pattern can be defined for datetime data type.
+        - Sort orders for invalid and empty values can be defined. For example, If sort value order is defined as VALID_EMPTY_INVALID, invalid values will follow empty values and empty values will follow valid values. This value order option is applicable for int, datetime and float data types. All combinations are poossible for EMPTY, INVALID, VALID values.
+        - You can define your custom sorters. "enum-sorter" as a custom sorter has been already implemented. It sorts enums with given string values.
     * There are **10 different filters** (with inverse options). Any filter can be applied to any column. Multiple filters can be defined. 
         - CONTAINS / NOT CONTAINS
         - EQUAL / NOT EQUAL
         - STARTSWITH / NOT STARTSWITH
         - ENDSWITH / NOT ENDSWITH
         - GREATER / NOT GREATER
         - GREATER_EQUAL / NOT GREATER_EQUAL
         - LESS / NOT LESS
         - LESS_EQUAL / NOT LESS_EQUAL
         - REGEX (regex match) / NOT REGEX (not regex match)
         - EMPTY / NOT EMPTY (None or empty)
+    * You can define multiple filters. If one filter rejects row, row will not be selected (AND operation).
+    * You can define one or more columns for a filter. If there are multiple columns for a filter. If any column matches the parameter, filter selects the row (OR operation).
+    * If you do not select any column for filter, filter will evaluate all columns of the row. If filter matches the parameter with any column, it will select the row. You can define column names to skip them while evaluating all rows. 
+    * You can define your custom filters. Some custom filters have been already implemented.
+        - "between-equal": Returns row if value between given min and max. Min and max inputs can be datetime, str, int or float.
+        - "valid-datetime" Return row if value is valid datetime with given pattern. Default pattern is DD/MM/YYYY.
+        - "valid-number": Return row if value is valid int or float.
+        - "enum-contains": Gets a map to define a text for each enum value. Returns row if input parameter is in the enum-mapped text. Enums can be any allowed type (str, int, etc.).
+            + Example: Enum values are 1, 2, 3, 4. Enum values are mapped to 1: "In Review", 2: "Published", 3: "In Curation", 4: "Public". If parameter is "Pub", all rows contain enum value 2 and 4 will be returned.
+
 4. Define and **apply actions** to manuplate ISA table files. Supported operations:
     * ADD_ROW: Insert rows to given index
     * DELETE_ROW: delete selected rows
     * MOVE_ROW: move row to new index
     * ADD_COLUMN: Add new column
     * DELETE_COLUMN: delete selected columns
     * MOVE_COLUMN: move column to new index
     * COPY_ROW: copy row data to other selected rows
     * COPY_COLUMN: copy column data to other selected columns
     * UPDATE_ROW_DATA: update selected rows
     * UPDATE_COLUMN_DATA: selected columns
     * UPDATE_COLUMN_HEADER: update column headers
     * UPDATE_CELL_DATA: update cells given with row and column index
 
+
+
 ### Investigation file operations
 
 Read and update an investigation file
 ```python 
 import os
 import pathlib
 import uuid
```

