# Comparing `tmp/excel_framework-0.2.0.tar.gz` & `tmp/excel_framework-0.3.0.tar.gz`

## Comparing `excel_framework-0.2.0.tar` & `excel_framework-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 excel_framework-0.2.0/test.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 excel_framework-0.2.0/upload_guide.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/column.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/row.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/table.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/non_layout/excel_cell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/__init__.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/excel_file.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/excel_sheet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/build_context.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/buildable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/dimension.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/resizer.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/size.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/border.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/color.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/fill.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/style.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/style_part.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/styler.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/text_style.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 excel_framework-0.2.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 excel_framework-0.2.0/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.2.0/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 excel_framework-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 excel_framework-0.3.0/test.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 excel_framework-0.3.0/upload_guide.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/buildables/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/buildables/layout/column.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/buildables/layout/row.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/buildables/layout/table.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/buildables/non_layout/excel_cell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/excel/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/excel/excel_file.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/excel/excel_sheet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/internals/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/internals/build_context.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/internals/buildable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/sizes/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/sizes/dimension.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/sizes/resizer.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/sizes/size.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/border.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/color.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/fill.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/style.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/style_part.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/styler.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 excel_framework-0.3.0/src/excel_framework/styling/text_style.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 excel_framework-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 excel_framework-0.3.0/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.3.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 excel_framework-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.3.0/PKG-INFO
```

### Comparing `excel_framework-0.2.0/test.py` & `excel_framework-0.3.0/test.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/__init__.py` & `excel_framework-0.3.0/src/excel_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/buildables/layout/column.py` & `excel_framework-0.3.0/src/excel_framework/buildables/layout/column.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/buildables/layout/row.py` & `excel_framework-0.3.0/src/excel_framework/buildables/layout/row.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/buildables/layout/table.py` & `excel_framework-0.3.0/src/excel_framework/buildables/layout/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ...sizes.dimension import ColumnDimension, AutoWidth, FixedWidth
 
 T = TypeVar("T")
 
 @dataclass(frozen=True)
 class ConditionalStyle(Generic[T]):
     styles: list[Style]
-    selector: Callable[[T], int]
+    selector: Callable[[T], Union[int, None]]
 
 @dataclass(frozen=True)
 class TableColumn(Generic[T]):
     name: str
     value: Callable[[T], Any]
     width: Union[AutoWidth, FixedWidth, None] = None
     column_name_style: Union[Style, None] = None
```

### Comparing `excel_framework-0.2.0/src/excel_framework/buildables/non_layout/excel_cell.py` & `excel_framework-0.3.0/src/excel_framework/buildables/non_layout/excel_cell.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/excel/excel_file.py` & `excel_framework-0.3.0/src/excel_framework/excel/excel_file.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/internals/build_context.py` & `excel_framework-0.3.0/src/excel_framework/internals/build_context.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/internals/buildable.py` & `excel_framework-0.3.0/src/excel_framework/internals/buildable.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/sizes/dimension.py` & `excel_framework-0.3.0/src/excel_framework/sizes/dimension.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/sizes/resizer.py` & `excel_framework-0.3.0/src/excel_framework/sizes/resizer.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/border.py` & `excel_framework-0.3.0/src/excel_framework/styling/border.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/color.py` & `excel_framework-0.3.0/src/excel_framework/styling/color.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/fill.py` & `excel_framework-0.3.0/src/excel_framework/styling/fill.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/style.py` & `excel_framework-0.3.0/src/excel_framework/styling/style.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/styler.py` & `excel_framework-0.3.0/src/excel_framework/styling/styler.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/src/excel_framework/styling/text_style.py` & `excel_framework-0.3.0/src/excel_framework/styling/text_style.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/LICENSE` & `excel_framework-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_framework-0.2.0/pyproject.toml` & `excel_framework-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_framework"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Jonathan Dück", email="jonathan.dueck@digital-confidence.de" },
 ]
 description = "A small example package"
 readme = "README.md"
 dependencies = [
     "openpyxl",
```

### Comparing `excel_framework-0.2.0/PKG-INFO` & `excel_framework-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_framework
-Version: 0.2.0
+Version: 0.3.0
 Summary: A small example package
 Project-URL: Homepage, https://github.com/TheUltimateOptimist/excel_framework
 Project-URL: Bug Tracker, https://github.com/TheUltimateOptimist/excel_framework/issues
 Author-email: Jonathan Dück <jonathan.dueck@digital-confidence.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

