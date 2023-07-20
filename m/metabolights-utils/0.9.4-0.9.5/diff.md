# Comparing `tmp/metabolights_utils-0.9.4.tar.gz` & `tmp/metabolights_utils-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolights_utils-0.9.4.tar", max compression
+gzip compressed data, was "metabolights_utils-0.9.5.tar", max compression
```

## Comparing `metabolights_utils-0.9.4.tar` & `metabolights_utils-0.9.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.4/LICENSE
--rw-r--r--   0        0        0    14350 2023-07-19 00:20:16.337975 metabolights_utils-0.9.4/README.md
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.4/metabolights_utils/__init__.py
--rw-r--r--   0        0        0      244 2023-07-19 00:16:47.503397 metabolights_utils-0.9.4/metabolights_utils/common.py
--rw-r--r--   0        0        0     2214 2023-07-19 00:16:47.523886 metabolights_utils-0.9.4/metabolights_utils/isatab/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.4/metabolights_utils/isatab/default/__init__.py
--rw-r--r--   0        0        0      716 2023-07-19 00:16:47.532744 metabolights_utils-0.9.4/metabolights_utils/isatab/default/assay_file.py
--rw-r--r--   0        0        0     1268 2023-07-19 00:16:47.587091 metabolights_utils-0.9.4/metabolights_utils/isatab/default/assignment_file.py
--rw-r--r--   0        0        0     1536 2023-07-19 00:16:47.626096 metabolights_utils-0.9.4/metabolights_utils/isatab/default/base_isa_file.py
--rw-r--r--   0        0        0     5906 2023-07-19 00:16:47.662335 metabolights_utils-0.9.4/metabolights_utils/isatab/default/base_isa_table_file.py
--rw-r--r--   0        0        0     1847 2023-07-19 00:16:47.732545 metabolights_utils-0.9.4/metabolights_utils/isatab/default/factory.py
--rw-r--r--   0        0        0    11163 2023-07-19 00:16:47.792874 metabolights_utils-0.9.4/metabolights_utils/isatab/default/investigation_file.py
--rw-r--r--   0        0        0      706 2023-07-19 00:16:47.861855 metabolights_utils-0.9.4/metabolights_utils/isatab/default/sample_file.py
--rw-r--r--   0        0        0     1488 2023-07-19 00:16:47.917232 metabolights_utils-0.9.4/metabolights_utils/isatab/default/writer.py
--rw-r--r--   0        0        0     9873 2023-07-19 00:16:47.934165 metabolights_utils-0.9.4/metabolights_utils/isatab/reader.py
--rw-r--r--   0        0        0     3692 2023-07-19 00:16:47.939412 metabolights_utils-0.9.4/metabolights_utils/isatab/writer.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.4/metabolights_utils/models/__init__.py
--rw-r--r--   0        0        0      442 2023-07-19 00:16:47.972240 metabolights_utils-0.9.4/metabolights_utils/models/common.py
--rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.4/metabolights_utils/models/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.4/metabolights_utils/models/isa/__init__.py
--rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.4/metabolights_utils/models/isa/assay_file.py
--rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.4/metabolights_utils/models/isa/assignment_file.py
--rw-r--r--   0        0        0    10914 2023-07-19 00:16:48.117594 metabolights_utils-0.9.4/metabolights_utils/models/isa/common.py
--rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.4/metabolights_utils/models/isa/enums.py
--rw-r--r--   0        0        0    11080 2023-07-19 00:16:48.173059 metabolights_utils-0.9.4/metabolights_utils/models/isa/investigation_file.py
--rw-r--r--   0        0        0    18241 2023-07-19 00:16:48.234817 metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/common.py
--rw-r--r--   0        0        0     9969 2023-07-19 00:16:48.272670 metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/filter.py
--rw-r--r--   0        0        0    22198 2023-07-19 00:16:48.338368 metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/investigation_parser.py
--rw-r--r--   0        0        0    18279 2023-07-19 00:16:48.365539 metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/isa_table_parser.py
--rw-r--r--   0        0        0     5421 2023-07-19 00:16:48.402690 metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/sort.py
--rw-r--r--   0        0        0      457 2023-07-19 00:16:48.411630 metabolights_utils-0.9.4/metabolights_utils/models/isa/samples_file.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.4/metabolights_utils/models/metabolights/__init__.py
--rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.4/metabolights_utils/models/metabolights/metabolights_study.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.4/metabolights_utils/models/parser/__init__.py
--rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.4/metabolights_utils/models/parser/common.py
--rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.4/metabolights_utils/models/parser/enums.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.4/metabolights_utils/tsv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/__init__.py
--rw-r--r--   0        0        0     3579 2023-07-19 00:16:48.555207 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/add_column.py
--rw-r--r--   0        0        0     3497 2023-07-19 00:16:48.581585 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/add_row.py
--rw-r--r--   0        0        0     1342 2023-07-19 00:16:48.626254 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/base.py
--rw-r--r--   0        0        0     3399 2023-07-19 00:16:48.661295 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/copy_column.py
--rw-r--r--   0        0        0     3153 2023-07-19 00:16:48.670576 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/copy_row.py
--rw-r--r--   0        0        0     2501 2023-07-19 00:16:48.688456 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/delete_column.py
--rw-r--r--   0        0        0     2012 2023-07-19 00:16:48.691703 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/delete_row.py
--rw-r--r--   0        0        0     2876 2023-07-19 00:16:48.694900 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/move_column.py
--rw-r--r--   0        0        0     3372 2023-07-19 00:16:48.711545 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/move_row.py
--rw-r--r--   0        0        0     3166 2023-07-19 00:16:48.717282 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_cell.py
--rw-r--r--   0        0        0     3564 2023-07-19 00:16:48.762152 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_column.py
--rw-r--r--   0        0        0     2103 2023-07-19 00:16:48.788616 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_column_header.py
--rw-r--r--   0        0        0     2238 2023-07-19 00:16:48.826031 metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_row.py
--rw-r--r--   0        0        0     3591 2023-07-19 00:16:48.859856 metabolights_utils-0.9.4/metabolights_utils/tsv/model.py
--rw-r--r--   0        0        0     5851 2023-07-19 00:16:48.880378 metabolights_utils-0.9.4/metabolights_utils/tsv/tsv_file_updater.py
--rw-r--r--   0        0        0     1310 2023-07-19 00:21:06.152561 metabolights_utils-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 metabolights_utils-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.5/LICENSE
+-rw-r--r--   0        0        0    14366 2023-07-19 20:51:58.143530 metabolights_utils-0.9.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.456526 metabolights_utils-0.9.5/metabolights_utils/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-19 00:16:47.503397 metabolights_utils-0.9.5/metabolights_utils/common.py
+-rw-r--r--   0        0        0     2198 2023-07-19 09:21:04.692280 metabolights_utils-0.9.5/metabolights_utils/isatab/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.525753 metabolights_utils-0.9.5/metabolights_utils/isatab/default/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-19 00:16:47.532744 metabolights_utils-0.9.5/metabolights_utils/isatab/default/assay_file.py
+-rw-r--r--   0        0        0     1268 2023-07-19 00:16:47.587091 metabolights_utils-0.9.5/metabolights_utils/isatab/default/assignment_file.py
+-rw-r--r--   0        0        0     1536 2023-07-19 00:16:47.626096 metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_file.py
+-rw-r--r--   0        0        0     5878 2023-07-20 09:45:20.078824 metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_table_file.py
+-rw-r--r--   0        0        0     1881 2023-07-19 09:14:50.131288 metabolights_utils-0.9.5/metabolights_utils/isatab/default/factory.py
+-rw-r--r--   0        0        0    11163 2023-07-19 00:16:47.792874 metabolights_utils-0.9.5/metabolights_utils/isatab/default/investigation_file.py
+-rw-r--r--   0        0        0      706 2023-07-19 00:16:47.861855 metabolights_utils-0.9.5/metabolights_utils/isatab/default/sample_file.py
+-rw-r--r--   0        0        0     1488 2023-07-19 00:16:47.917232 metabolights_utils-0.9.5/metabolights_utils/isatab/default/writer.py
+-rw-r--r--   0        0        0     9845 2023-07-20 09:45:19.894271 metabolights_utils-0.9.5/metabolights_utils/isatab/reader.py
+-rw-r--r--   0        0        0     3692 2023-07-19 00:16:47.939412 metabolights_utils-0.9.5/metabolights_utils/isatab/writer.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:47.940900 metabolights_utils-0.9.5/metabolights_utils/models/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-19 00:16:47.972240 metabolights_utils-0.9.5/metabolights_utils/models/common.py
+-rw-r--r--   0        0        0      149 2023-07-19 00:16:48.007068 metabolights_utils-0.9.5/metabolights_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.019187 metabolights_utils-0.9.5/metabolights_utils/models/isa/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-19 00:16:48.049609 metabolights_utils-0.9.5/metabolights_utils/models/isa/assay_file.py
+-rw-r--r--   0        0        0      402 2023-07-19 00:16:48.089220 metabolights_utils-0.9.5/metabolights_utils/models/isa/assignment_file.py
+-rw-r--r--   0        0        0     9506 2023-07-20 09:50:31.746316 metabolights_utils-0.9.5/metabolights_utils/models/isa/common.py
+-rw-r--r--   0        0        0      478 2023-07-19 00:16:48.146363 metabolights_utils-0.9.5/metabolights_utils/models/isa/enums.py
+-rw-r--r--   0        0        0    11080 2023-07-19 00:16:48.173059 metabolights_utils-0.9.5/metabolights_utils/models/isa/investigation_file.py
+-rw-r--r--   0        0        0    18440 2023-07-20 09:45:19.894366 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/common.py
+-rw-r--r--   0        0        0    22198 2023-07-19 00:16:48.338368 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/investigation_parser.py
+-rw-r--r--   0        0        0    18265 2023-07-20 09:45:18.997818 metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/isa_table_parser.py
+-rw-r--r--   0        0        0      457 2023-07-19 00:16:48.411630 metabolights_utils-0.9.5/metabolights_utils/models/isa/samples_file.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.415532 metabolights_utils-0.9.5/metabolights_utils/models/metabolights/__init__.py
+-rw-r--r--   0        0        0     1077 2023-07-19 00:16:48.427548 metabolights_utils-0.9.5/metabolights_utils/models/metabolights/metabolights_study.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.443379 metabolights_utils-0.9.5/metabolights_utils/models/parser/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-19 00:16:48.470689 metabolights_utils-0.9.5/metabolights_utils/models/parser/common.py
+-rw-r--r--   0        0        0      148 2023-07-19 00:16:48.476458 metabolights_utils-0.9.5/metabolights_utils/models/parser/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.501180 metabolights_utils-0.9.5/metabolights_utils/tsv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:16:48.528354 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/__init__.py
+-rw-r--r--   0        0        0     3559 2023-07-19 08:23:28.339563 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_column.py
+-rw-r--r--   0        0        0     3488 2023-07-19 08:26:08.140976 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_row.py
+-rw-r--r--   0        0        0     1339 2023-07-19 07:58:19.960337 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/base.py
+-rw-r--r--   0        0        0     3390 2023-07-19 08:23:28.347823 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_column.py
+-rw-r--r--   0        0        0     3144 2023-07-19 08:23:28.383070 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_row.py
+-rw-r--r--   0        0        0     2492 2023-07-19 08:23:28.528233 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_column.py
+-rw-r--r--   0        0        0     1986 2023-07-19 09:13:04.618046 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_row.py
+-rw-r--r--   0        0        0     2867 2023-07-19 08:23:28.613461 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_column.py
+-rw-r--r--   0        0        0     3363 2023-07-19 08:23:28.672360 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_row.py
+-rw-r--r--   0        0        0     3157 2023-07-19 08:23:28.701280 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_cell.py
+-rw-r--r--   0        0        0     3544 2023-07-19 09:13:21.371457 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column.py
+-rw-r--r--   0        0        0     2077 2023-07-19 09:13:17.513241 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column_header.py
+-rw-r--r--   0        0        0     2229 2023-07-19 08:23:28.847528 metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_row.py
+-rw-r--r--   0        0        0    19935 2023-07-20 13:14:00.106647 metabolights_utils-0.9.5/metabolights_utils/tsv/filter.py
+-rw-r--r--   0        0        0     6043 2023-07-19 09:10:39.601796 metabolights_utils-0.9.5/metabolights_utils/tsv/model.py
+-rw-r--r--   0        0        0    12899 2023-07-20 13:14:20.411943 metabolights_utils-0.9.5/metabolights_utils/tsv/sort.py
+-rw-r--r--   0        0        0     5647 2023-07-19 08:26:02.864303 metabolights_utils-0.9.5/metabolights_utils/tsv/tsv_file_updater.py
+-rw-r--r--   0        0        0     1310 2023-07-20 13:15:57.573603 metabolights_utils-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    15350 1970-01-01 00:00:00.000000 metabolights_utils-0.9.5/PKG-INFO
```

### Comparing `metabolights_utils-0.9.4/LICENSE` & `metabolights_utils-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/README.md` & `metabolights_utils-0.9.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -193,22 +193,22 @@
 
 def test_with_filter_and_sort_option_01():
     # Sample Name value does not start with 'control'  and
     # Parameter Value[Chromatography Instrument] value is 'Thermo Scientific TRACE GC Ultra'.
     # Both filters are applied in case insesitive mode.
     filter_options = [
         TsvFileFilterOption(
-            column_name="Sample Name",
+            search_columns=["Sample Name"],
             operation=FilterOperation.STARTSWITH,
             parameter="control",
             case_sensitive=False,
             negate_result=True,
         ),
         TsvFileFilterOption(
-            column_name="Parameter Value[Chromatography Instrument]",
+            search_columns=["Parameter Value[Chromatography Instrument]"],
             operation=FilterOperation.EQUAL,
             parameter="Thermo Scientific TRACE GC Ultra",
             case_sensitive=False,
         ),
     ]
 
     # sort by Sample Name and 'Parameter Value[Chromatography Instrument]'
@@ -258,21 +258,21 @@
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 50
 
     # First filter applies regex epression math on Sample Name column in case insensitive mode
     # Second filter is exact match on Parameter Value[Chromatography Instrument]
     filter_options = [
         TsvFileFilterOption(
-            column_name="Sample Name",
+            search_columns=["Sample Name"],
             operation=FilterOperation.REGEX,
             parameter="^PG[\d]5.*_5$",
             case_sensitive=False,
         ),
         TsvFileFilterOption(
-            column_name="Parameter Value[Chromatography Instrument]",
+            search_columns=["Parameter Value[Chromatography Instrument]"],
             operation=FilterOperation.EQUAL,
             parameter="Thermo Scientific TRACE GC Ultra",
             case_sensitive=False,
         ),
     ]
 
     selected_columns = [
@@ -363,10 +363,10 @@
 ```
 
 ### Apply actions on ISA table files
 
 User can manuplate ISA table files in row, column or cell level.
 
 
-View **actions and model definition** from [a this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/metabolights_utils/tsv/model.py).
+View **actions and model definition** from [this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/metabolights_utils/tsv/model.py).
 
-View **examples** from [a this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/tests/metabolights_utils/isatab/test_isa_table_actions.py).
+View **examples** from [this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/tests/metabolights_utils/isatab/test_isa_table_actions.py).
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/__init__.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 @lru_cache
 def get_writer_factory():
     writer_factory: IsaTabWriterFactory = DefaultIsaTabWriterFactory()
     return writer_factory
 
 
 class Reader:
-    reader_factory: IsaTabReaderFactory = DefaultIsaTabReaderFactory()
+    reader_factory: IsaTabReaderFactory = get_reader_factory()
 
     @classmethod
     def get_investigation_file_reader(cls) -> InvestigationFileReader:
         return cls.reader_factory.get_investigation_file_reader()
 
     @classmethod
     def get_assay_file_reader(cls, results_per_page=100) -> IsaTableFileReader:
@@ -51,15 +51,15 @@
     def get_assignment_file_reader(cls, results_per_page=100) -> IsaTableFileReader:
         return cls.reader_factory.get_assay_file_reader(
             results_per_page=results_per_page
         )
 
 
 class Writer:
-    writer_factory: IsaTabWriterFactory = DefaultIsaTabWriterFactory()
+    writer_factory: IsaTabWriterFactory = get_writer_factory()
 
     @classmethod
     def get_investigation_file_writer(cls) -> InvestigationFileWriter:
         return cls.writer_factory.get_investigation_file_writer()
 
     @classmethod
     def get_assay_file_writer(cls) -> IsaTableFileWriter:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/assay_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/assignment_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/assignment_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/base_isa_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/base_isa_table_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/base_isa_table_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from typing import List, Union
 
 from metabolights_utils.isatab.default.base_isa_file import BaseIsaFile
 from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
     IsaTableFileReaderResult,
 )
-from metabolights_utils.models.isa.parser.filter import TsvFileFilterOption
 from metabolights_utils.models.isa.parser.isa_table_parser import get_isa_table
-from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserMessage, ParserReport
 from metabolights_utils.models.parser.enums import ParserMessageType
+from metabolights_utils.tsv.filter import TsvFileFilterOption
+from metabolights_utils.tsv.sort import TsvFileSortOption
 
 
 class BaseIsaTableFileReader(BaseIsaFile, IsaTableFileReader, ABC):
     def __init__(self, results_per_page=100) -> None:
         self.results_per_page = results_per_page if results_per_page > 0 else 100
 
     @abstractmethod
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/factory.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,24 @@
 )
 from metabolights_utils.isatab.default.investigation_file import (
     DefaultInvestigationFileReader,
     DefaultInvestigationFileWriter,
 )
 from metabolights_utils.isatab.default.sample_file import DefaultSampleFileReader
 from metabolights_utils.isatab.default.writer import DefaultIsaTableFileWriter
-from metabolights_utils.isatab.reader import InvestigationFileReader, IsaTabReaderFactory, IsaTableFileReader
-from metabolights_utils.isatab.writer import InvestigationFileWriter, IsaTabWriterFactory, IsaTableFileWriter
+from metabolights_utils.isatab.reader import (
+    InvestigationFileReader,
+    IsaTabReaderFactory,
+    IsaTableFileReader,
+)
+from metabolights_utils.isatab.writer import (
+    InvestigationFileWriter,
+    IsaTabWriterFactory,
+    IsaTableFileWriter,
+)
 
 
 class DefaultIsaTabReaderFactory(IsaTabReaderFactory):
     def get_investigation_file_reader(self) -> InvestigationFileReader:
         return DefaultInvestigationFileReader()
 
     def get_assay_file_reader(self, results_per_page=100) -> IsaTableFileReader:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/investigation_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/investigation_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/sample_file.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/sample_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/default/writer.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/default/writer.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/reader.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import List, Union
 
 from pydantic import Field
 
 from metabolights_utils.models.common import MetabolightsBaseModel
 from metabolights_utils.models.isa.common import IsaTableFile
 from metabolights_utils.models.isa.investigation_file import Investigation
-from metabolights_utils.models.isa.parser.filter import TsvFileFilterOption
-from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserReport
+from metabolights_utils.tsv.filter import TsvFileFilterOption
+from metabolights_utils.tsv.sort import TsvFileSortOption
 
 
 class IsaTableFileReaderResult(MetabolightsBaseModel):
     isa_table_file: IsaTableFile = Field(IsaTableFile())
     parser_report: ParserReport = Field(ParserReport())
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/isatab/writer.py` & `metabolights_utils-0.9.5/metabolights_utils/isatab/writer.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/assay_file.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/common.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from enum import Enum
 from typing import Dict, List, Union
-import humps
 
+import humps
 from pydantic import BaseModel, Extra, Field
 
 from metabolights_utils.models.common import MetabolightsBaseModel
 from metabolights_utils.models.isa.enums import ColumnsStructure
+from metabolights_utils.tsv.filter import TsvFileFilterOption
+from metabolights_utils.tsv.sort import TsvFileSortOption
 
 INVESTIGATION_FILE_INITIAL_ROWS = [
     "ONTOLOGY SOURCE REFERENCE",
     "Term Source Name",
     "Term Source File",
     "Term Source Version",
     "Term Source Description",
@@ -281,76 +282,14 @@
     column_prefix: str = ""
     column_search_pattern: str = ""
 
     def __hash__(self):
         return hash(self.column_name)
 
 
-class FilterParameterType(str, Enum):
-    AUTO = "AUTO"
-    STRING = "STRING"
-    INTEGER = "INTEGER"
-    FLOAT = "FLOAT"
-    DATETIME = "DATETIME"
-
-
-class FilterOperation(str, Enum):
-    CONTAINS = "like"
-    EQUAL = "eq"
-    STARTSWITH = "startswith"
-    ENDSWITH = "endswith"
-    GREATER = "gt"
-    GREATER_EQUAL = "ge"
-    LESS = "lt"
-    LESS_EQUAL = "le"
-    REGEX = "regex"
-    EMPTY = "empty"
-
-
-class TsvFileFilterOption(MetabolightsBaseModel):
-    column_name: str
-    operation: FilterOperation = FilterOperation.CONTAINS
-    parameter: Union[str, int, float] = ""
-    parameter_type: FilterParameterType = FilterParameterType.AUTO
-    case_sensitive: bool = True
-    negate_result: bool = False
-    default_datetime_pattern: str = "%m/%d/%Y"
-
-
-class SortType(str, Enum):
-    STRING = "STRING"
-    INTEGER = "INTEGER"
-    FLOAT = "FLOAT"
-    DATETIME = "DATETIME"
-
-
-class SortValueClassification(int, Enum):
-    EMPTY = 1
-    INVALID = 2
-    VALID = 3
-
-
-class TsvFileSortValueOrder(int, Enum):
-    EMPTY_INVALID_VALID = 0o123
-    EMPTY_VALID_INVALID = 0o132
-    INVALID_EMPTY_VALID = 0o213
-    INVALID_VALID_EMPTY = 0o231
-    VALID_INVALID_EMPTY = 0o321
-    VALID_EMPTY_INVALID = 0o312
-
-
-class TsvFileSortOption(MetabolightsBaseModel):
-    column_name: str
-    reverse: bool = False
-    column_sort_type: SortType = SortType.STRING
-    case_sensitive: bool = True
-    default_datetime_pattern: str = "%m/%d/%Y"
-    value_order: TsvFileSortValueOrder = TsvFileSortValueOrder.VALID_EMPTY_INVALID
-
-
 class IsaTable(IsaAbstractModel):
     columns: List[str] = Field([])
     headers: List[IsaTableColumn] = Field([])
     data: Dict[str, List[str]] = Field({})
     row_indices: List[int] = []
     column_indices: List[int] = []
     filtered_total_row_count: int = 0
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/investigation_file.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/investigation_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/common.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import csv
 import re
-from datetime import datetime
-from enum import Enum
+import sys
 from functools import reduce
 from io import IOBase
-from typing import Any, Dict, List, Union
+from typing import Dict, List, Union
 
-from pydantic import BaseModel
 from metabolights_utils.models.common import MetabolightsBaseModel
-
 from metabolights_utils.models.isa.common import (
     INVESTIGATION_FILE_INITIAL_ROWS_SET,
     INVESTIGATION_FILE_STUDY_ROWS_SET,
 )
-from metabolights_utils.models.isa.parser.filter import (
-    TsvFileFilterOption,
-    get_filter_operation,
-)
-from metabolights_utils.models.isa.parser.sort import (
-    TsvFileSortOption,
-    get_sorter,
-    sort_by_multiple_column,
-)
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
+from metabolights_utils.tsv.filter import Filter, FilterRegistry, TsvFileFilterOption
+from metabolights_utils.tsv.sort import (
+    Sorter,
+    SorterRegistry,
+    TsvFileSortOption,
+    TsvSortException,
+)
 
 
 def read_investigation_file(file_buffer: IOBase, messages: List[ParserMessage]):
     new_lines = read_investigation_file_lines(file_buffer, messages)
     dict_format = {}
     for i in range(len(new_lines)):
         detail = {}
@@ -262,15 +257,16 @@
     filter_options: List[TsvFileFilterOption] = None,
     sort_options: List[TsvFileSortOption] = None,
 ) -> SelectedTsvFileContent:
     columns: Dict[str, TsvColumn] = {}
     column_indices: Dict[int, str] = {}
     selected_column_indices: Dict[int, str] = {}
     column_name_indices: Dict[str, int] = {}
-    filter_operations: Dict[str, List[Any]] = {}
+    filters: List[Filter] = []
+
     try:
         next_row_index = 0
         filtered_rows = []
         for row in reader:
             next_row_index += 1
             row_index = next_row_index - 1
             if row_index == 0:
@@ -281,48 +277,61 @@
                     columns,
                     column_indices,
                     column_name_indices,
                     selected_column_indices,
                 )
                 if filter_options:
                     for filter_option in filter_options:
-                        filter_operation = get_filter_operation(filter_option)
-                        if filter_option.column_name not in filter_operations:
-                            filter_operations[filter_option.column_name] = []
-                        filter_operations[filter_option.column_name].append(
-                            filter_operation
+                        filter_option.search_columns = (
+                            filter_option.search_columns
+                            if filter_option.search_columns
+                            else []
                         )
+                        filter: Filter = FilterRegistry.get_filter(
+                            filter_option, column_name_indices, column_indices
+                        )
+                        filters.append(filter)
+                    # empty search column filters will be moved to end
+                    filters.sort(
+                        key=lambda x: len(x.filter_option.search_columns)
+                        if x.filter_option.search_columns
+                        else sys.maxsize
+                    )
             else:
                 if not filter_options:
                     filtered_rows.append((row_index - 1, row))
                 else:
-                    selected = True
-
-                    for filter_option in filter_options:
-                        col_index = column_name_indices[filter_option.column_name]
-                        val = row[col_index]
-                        for filter_operation in filter_operations[
-                            filter_option.column_name
-                        ]:
-                            if not filter_operation(val):
-                                selected = False
-                                break
-                        if not selected:
+                    select: bool = True
+                    for filter in filters:
+                        select = filter.filter(row)
+                        if not select:
                             break
-                    if selected:
+                    if select:
                         filtered_rows.append((row_index - 1, row))
         reader = None
 
-        sort_list = []
+        sorters: List[Sorter] = []
         if sort_options:
             for sort_option in sort_options:
                 col_index = column_name_indices[sort_option.column_name]
-                row_sorter = get_sorter(sort_option, col_index)
-                sort_list.append((row_sorter, sort_option.reverse))
-        filtered_rows = sort_by_multiple_column(filtered_rows, sort_list)
+                sorter: Sorter = SorterRegistry.get_sorter(
+                    sort_option,
+                    col_index,
+                    column_name_indices,
+                    column_indices,
+                )
+                sorters.append(sorter)
+        if sorters:
+            filtered_rows = reduce(
+                lambda s, sorter: sorted(
+                    s, key=sorter.sort, reverse=sorter.sort_option.reverse
+                ),
+                reversed(sorters),
+                filtered_rows,
+            )
 
         content.total_filtered_rows = len(filtered_rows)
         offset = 0 if not offset else offset
 
         content.offset = (
             offset
             if offset < content.total_filtered_rows
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/investigation_parser.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/investigation_parser.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/isa/parser/isa_table_parser.py` & `metabolights_utils-0.9.5/metabolights_utils/models/isa/parser/isa_table_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     IsaTableAdditionalColumn,
 )
 from metabolights_utils.models.isa.parser.common import (
     SelectedTsvFileContent,
     TsvFileFilterOption,
     read_table_file,
 )
-from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
+from metabolights_utils.tsv.sort import TsvFileSortOption
 
 
 def parse_isa_table_sheet_from_fs(
     file_path: str,
     expected_patterns: Union[None, List[List[str]]] = None,
     selected_columns: Union[None, List[str]] = None,
     offset: Union[int, None] = None,
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/metabolights/metabolights_study.py` & `metabolights_utils-0.9.5/metabolights_utils/models/metabolights/metabolights_study.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/models/parser/common.py` & `metabolights_utils-0.9.5/metabolights_utils/models/parser/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/add_column.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_column.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pathlib
-import sys
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class AddColumnsActionHelper(BaseActionHelper):
+class AddColumnsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvAddColumnsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.ADD_COLUMN:
+        if action.type != actions.TsvActionType.ADD_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvAddColumnsAction = action
 
         column_data: Dict[int, actions.TsvColumnData] = (
             action.columns if action.columns else {}
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/add_row.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/add_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class AddRowsActionHelper(BaseActionHelper):
+class AddRowsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: model.TsvAddRowsAction,
     ) -> model.TsvActionResult:
         result: model.TsvActionResult = model.TsvActionResult(action=action)
-        if action.name != model.TsvActionName.ADD_ROW:
+        if action.type != model.TsvActionType.ADD_ROW:
             result.message = "Action name is not valid"
             return result
 
         action: model.TsvAddRowsAction = action
         target_row_indices: List[int] = action.new_row_indices
 
         if not target_row_indices:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/base.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class TsvActionException(Exception):
     def __init__(self, message: str) -> None:
         self.message = message
 
 
-class BaseActionHelper(ABC):
+class BaseTsvAction(ABC):
     @abstractmethod
     def apply_action(
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvAction,
     ) -> actions.TsvActionResult:
         pass
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/copy_column.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class CopyColumnActionHelper(BaseActionHelper):
+class CopyColumnTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvCopyColumnAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.COPY_COLUMN:
+        if action.type != actions.TsvActionType.COPY_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvCopyColumnAction = action
         source_column_index = action.source_column_index
         source_column_header = action.source_column_header
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/copy_row.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/copy_row.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 import uuid
 from typing import List, Set
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class CopyRowActionHelper(BaseActionHelper):
+class CopyRowTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvCopyRowAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.COPY_ROW:
+        if action.type != actions.TsvActionType.COPY_ROW:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvCopyRowAction = action
         target_row_indices: List[int] = action.target_row_indices
         selected_column_indices: Set[int] = set(action.selected_column_indices)
         if not target_row_indices:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/delete_column.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_column.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class DeleteColumnsActionHelper(BaseActionHelper):
+class DeleteColumnsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvDeleteColumnsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.DELETE_COLUMN:
+        if action.type != actions.TsvActionType.DELETE_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvDeleteColumnsAction = action
 
         columns: Dict[int, str] = (
             action.current_columns if action.current_columns else {}
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/delete_row.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/delete_row.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pathlib
-import sys
 import uuid
-from typing import Dict, List
+from typing import List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class DeleteRowsActionHelper(BaseActionHelper):
+class DeleteRowsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvDeleteRowsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.DELETE_ROW:
+        if action.type != actions.TsvActionType.DELETE_ROW:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvDeleteRowsAction = action
         target_row_indices: List[int] = action.current_row_indices
 
         if not target_row_indices:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/move_column.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pathlib
 import uuid
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class MoveColumnActionHelper(BaseActionHelper):
+class MoveColumnTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvMoveColumnAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.MOVE_COLUMN:
+        if action.type != actions.TsvActionType.MOVE_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvMoveColumnAction = action
         source_column_index = action.source_column_index
         source_column_header = action.source_column_header
         new_column_index = action.new_column_index
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/move_row.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/move_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pathlib
 import sys
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class MoveRowActionHelper(BaseActionHelper):
+class MoveRowTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvMoveRowAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.MOVE_ROW:
+        if action.type != actions.TsvActionType.MOVE_ROW:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvMoveRowAction = action
         new_row_index = action.new_row_index
 
         if new_row_index is None or new_row_index < 0:
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_cell.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pathlib
 import sys
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class UpdateCellsActionHelper(BaseActionHelper):
+class UpdateCellsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvUpdateCellsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.UPDATE_CELL_DATA:
+        if action.type != actions.TsvActionType.UPDATE_CELL_DATA:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvUpdateCellsAction = action
 
         cells: List[actions.TsvCellData] = action.cells if action.cells else []
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_column.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pathlib
-import sys
 import uuid
 from typing import Dict, List
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class UpdateColumnsActionHelper(BaseActionHelper):
+class UpdateColumnsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvUpdateColumnsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.UPDATE_COLUMN_DATA:
+        if action.type != actions.TsvActionType.UPDATE_COLUMN_DATA:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvUpdateColumnsAction = action
 
         columns: Dict[int, actions.TsvColumnData] = (
             action.columns if action.columns else {}
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_column_header.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_column_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pathlib
-import sys
 import uuid
-from typing import Dict, List
+from typing import Dict
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class UpdateColumnHeadersActionHelper(BaseActionHelper):
+class UpdateColumnHeadersTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvUpdateColumnHeaderAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.UPDATE_COLUMN_HEADER:
+        if action.type != actions.TsvActionType.UPDATE_COLUMN_HEADER:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvUpdateColumnHeaderAction = action
 
         headers: Dict[int, str] = action.new_headers if action.new_headers else {}
```

### Comparing `metabolights_utils-0.9.4/metabolights_utils/tsv/actions/update_row.py` & `metabolights_utils-0.9.5/metabolights_utils/tsv/actions/update_row.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pathlib
 import uuid
 from typing import Dict
 
 from metabolights_utils.tsv import model as actions
-from metabolights_utils.tsv.actions.base import BaseActionHelper
+from metabolights_utils.tsv.actions.base import BaseTsvAction
 
 
-class UpdateRowsActionHelper(BaseActionHelper):
+class UpdateRowsTsvAction(BaseTsvAction):
     def apply_action(
         self,
         source_file_path: pathlib.Path,
         target_file_path: pathlib.Path,
         action: actions.TsvUpdateRowsAction,
     ) -> actions.TsvActionResult:
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
-        if action.name != actions.TsvActionName.UPDATE_ROW_DATA:
+        if action.type != actions.TsvActionType.UPDATE_ROW_DATA:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvUpdateRowsAction = action
 
         row_data: Dict[int, actions.TsvRowData] = action.rows if action.rows else {}
         if not row_data:
```

### Comparing `metabolights_utils-0.9.4/pyproject.toml` & `metabolights_utils-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabolights-utils"
-version = "0.9.4"
+version = "0.9.5"
 description = "Metabolights common models, utility methods and classes for python-based Metabolights projects."
 authors = ["Ozgur Yurekten <ozgur@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "metabolights_utils"}]
 license = "Apache-2.0"
 homepage = "https://github.com/EBI-Metabolights"
 repository = "https://github.com/EBI-Metabolights/metabolights-utils"
```

### Comparing `metabolights_utils-0.9.4/PKG-INFO` & `metabolights_utils-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolights-utils
-Version: 0.9.4
+Version: 0.9.5
 Summary: Metabolights common models, utility methods and classes for python-based Metabolights projects.
 Home-page: https://github.com/EBI-Metabolights
 License: Apache-2.0
 Keywords: metabolights,metabolomics,ISA data model
 Author: Ozgur Yurekten
 Author-email: ozgur@ebi.ac.uk
 Requires-Python: >=3.8.1,<3.9
@@ -216,22 +216,22 @@
 
 def test_with_filter_and_sort_option_01():
     # Sample Name value does not start with 'control'  and
     # Parameter Value[Chromatography Instrument] value is 'Thermo Scientific TRACE GC Ultra'.
     # Both filters are applied in case insesitive mode.
     filter_options = [
         TsvFileFilterOption(
-            column_name="Sample Name",
+            search_columns=["Sample Name"],
             operation=FilterOperation.STARTSWITH,
             parameter="control",
             case_sensitive=False,
             negate_result=True,
         ),
         TsvFileFilterOption(
-            column_name="Parameter Value[Chromatography Instrument]",
+            search_columns=["Parameter Value[Chromatography Instrument]"],
             operation=FilterOperation.EQUAL,
             parameter="Thermo Scientific TRACE GC Ultra",
             case_sensitive=False,
         ),
     ]
 
     # sort by Sample Name and 'Parameter Value[Chromatography Instrument]'
@@ -281,21 +281,21 @@
     assert len(result.parser_report.messages) == 0
     assert result.isa_table_file.table.row_count == 50
 
     # First filter applies regex epression math on Sample Name column in case insensitive mode
     # Second filter is exact match on Parameter Value[Chromatography Instrument]
     filter_options = [
         TsvFileFilterOption(
-            column_name="Sample Name",
+            search_columns=["Sample Name"],
             operation=FilterOperation.REGEX,
             parameter="^PG[\d]5.*_5$",
             case_sensitive=False,
         ),
         TsvFileFilterOption(
-            column_name="Parameter Value[Chromatography Instrument]",
+            search_columns=["Parameter Value[Chromatography Instrument]"],
             operation=FilterOperation.EQUAL,
             parameter="Thermo Scientific TRACE GC Ultra",
             case_sensitive=False,
         ),
     ]
 
     selected_columns = [
@@ -386,11 +386,11 @@
 ```
 
 ### Apply actions on ISA table files
 
 User can manuplate ISA table files in row, column or cell level.
 
 
-View **actions and model definition** from [a this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/metabolights_utils/tsv/model.py).
+View **actions and model definition** from [this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/metabolights_utils/tsv/model.py).
 
-View **examples** from [a this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/tests/metabolights_utils/isatab/test_isa_table_actions.py).
+View **examples** from [this file](https://github.com/EBI-Metabolights/metabolights-utils/blob/master/tests/metabolights_utils/isatab/test_isa_table_actions.py).
```

