# Comparing `tmp/excel_framework-0.1.1.tar.gz` & `tmp/excel_framework-0.2.0.tar.gz`

## Comparing `excel_framework-0.1.1.tar` & `excel_framework-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 excel_framework-0.1.1/test.py
--rw-r--r--   0        0        0   764403 2020-02-02 00:00:00.000000 excel_framework-0.1.1/testfile.xlsx
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 excel_framework-0.1.1/upload_guide.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/buildables/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/buildables/layout/column.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/buildables/layout/row.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/buildables/layout/table.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/buildables/non_layout/excel_cell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/excel/__init__.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/excel/excel_file.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/excel/excel_sheet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/internals/__init__.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/internals/build_context.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/internals/buildable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/sizes/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/sizes/dimension.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/sizes/resizer.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/sizes/size.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/__init__.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/border.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/color.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/fill.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/style.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/style_part.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/styler.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 excel_framework-0.1.1/src/excel_framework/styling/text_style.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 excel_framework-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 excel_framework-0.1.1/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.1.1/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 excel_framework-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 excel_framework-0.2.0/test.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 excel_framework-0.2.0/upload_guide.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/column.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/row.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/layout/table.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/buildables/non_layout/excel_cell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/excel_file.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/excel/excel_sheet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/build_context.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/internals/buildable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/dimension.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/resizer.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/sizes/size.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/border.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/color.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/fill.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/style.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/style_part.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/styler.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 excel_framework-0.2.0/src/excel_framework/styling/text_style.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 excel_framework-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 excel_framework-0.2.0/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.2.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 excel_framework-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.2.0/PKG-INFO
```

### Comparing `excel_framework-0.1.1/test.py` & `excel_framework-0.2.0/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from src.excel_framework import ExcelFile, ExcelSheet, Table, AutoWidth, Style, Fill, Colors, BorderSide, BorderStyle, TableColumn, Border
+from src.excel_framework import ExcelFile, ExcelSheet, Table, AutoWidth, Style, Fill, Colors, BorderSide, BorderStyle, TableColumn, Border, ConditionalStyle, TextStyle
 from openpyxl import Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.styles import PatternFill, Side, NamedStyle
 columns: list[TableColumn[list[str]]] = []
 for i in range(11):
     columns.append(TableColumn(str(i), lambda item, i=i: item[i], AutoWidth()))
-columns.append(TableColumn[list[str]](str(11), lambda item: item[11], AutoWidth(), value_style=lambda item: 0))
+columns.append(TableColumn[list[str]](str(11), lambda item: item[11], AutoWidth(),value_style=Style(text_style=TextStyle(bold=True)), conditional_style=ConditionalStyle([Style(fill=Fill(Colors.red))], lambda _: 0)))
 
 
 data: list[list[str]] = []
 for i in range(16000):
     row: list[str] = []
     for j in range(12):
         row.append(f"i: {i}, j: {j}")
@@ -17,12 +17,11 @@
 import time
 start = time.time() * 1000
 ExcelFile("testfile.xlsx", sheets=[
     ExcelSheet("Ordersheet", child=Table[list[str]](
         columns=columns,
         data=data,
         data_style=Style(fill=Fill(color=Colors.white), child_border=Border(all=BorderSide(border_style=BorderStyle.THICK))),
-        value_styles=[Style(fill=Fill(Colors.red))]
     ))
 ]).create()
 end = time.time() * 1000
 print(f"framework needed {end - start}ms")
```

### Comparing `excel_framework-0.1.1/src/excel_framework/__init__.py` & `excel_framework-0.2.0/src/excel_framework/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .internals.buildable import Buildable 
 from .excel.excel_file import ExcelFile
 from .excel.excel_sheet import ExcelSheet
 from .buildables.layout.column import Column
 from .buildables.layout.row import Row
-from .buildables.layout.table import Table, TableColumn
+from .buildables.layout.table import Table, TableColumn, ConditionalStyle
 from .buildables.non_layout.excel_cell import ExcelCell
 from .sizes.dimension import FixedWidth, AutoWidth, Dimension, RowDimension, ColumnDimension 
 from .styling.border import BorderStyle, BorderSide, Border
 from .styling.color import Color, Colors
 from .styling.fill import Fill
 from .styling.style import Style
-from .styling.styler import Styler
+from .styling.styler import Styler, ConditionalStyler
 from .styling.text_style import TextStyle, VerticalAlignment, HorizontalAlignment, Underline
```

### Comparing `excel_framework-0.1.1/src/excel_framework/buildables/layout/column.py` & `excel_framework-0.2.0/src/excel_framework/buildables/layout/column.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/buildables/layout/row.py` & `excel_framework-0.2.0/src/excel_framework/buildables/layout/row.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/buildables/layout/table.py` & `excel_framework-0.2.0/src/excel_framework/buildables/layout/table.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,67 +2,60 @@
 from overrides import override
 from dataclasses import dataclass
 from typing import Generic, TypeVar, Callable, Any, Union
 from .column import Column
 from .row import Row
 from ..non_layout.excel_cell import ExcelCell
 from ...styling.style import Style
-from ...styling.styler import Styler
+from ...styling.styler import Styler, ConditionalStyler
 from ...internals.build_context import BuildContext
 from ...sizes.dimension import ColumnDimension, AutoWidth, FixedWidth
 
 T = TypeVar("T")
 
+@dataclass(frozen=True)
+class ConditionalStyle(Generic[T]):
+    styles: list[Style]
+    selector: Callable[[T], int]
 
 @dataclass(frozen=True)
 class TableColumn(Generic[T]):
     name: str
     value: Callable[[T], Any]
     width: Union[AutoWidth, FixedWidth, None] = None
     column_name_style: Union[Style, None] = None
-    value_style: Union[Callable[[T], Union[int, None]], None] = None
+    value_style: Union[Style, None] = None
+    conditional_style: Union[ConditionalStyle[T], None] = None
 
 
 @dataclass(frozen=True)
 class Table(Buildable, Generic[T]):
     columns: list[TableColumn[T]]
     data: list[T]
     column_name_style: Union[Style, None] = None
     data_style: Union[Style, None] = None
-    value_styles: Union[list[Style], None] = None
 
     @override
     def internal_build(self, context: BuildContext) -> None:
         for i, column in enumerate(self.columns):
             if column.width:
                 context.collect_column_dimension(
                     ColumnDimension(context.column_index + i, column.width)
                 )
-        if self.value_styles:
-            joined_data_style = self.data_style
-            if context.style:
-                joined_data_style = context.style.join(self.data_style)
-            for i,value_style in enumerate(self.value_styles):
-                assert type(value_style) is Style
-                joined_style = value_style
-                if joined_data_style:
-                    joined_style = joined_data_style.join(value_style)
-                style_id = context.style_manager.add_named_style(context.workbook, joined_style)
-                self.value_styles[i] = style_id # type: ignore
         self.build().internal_build(context)
 
     @override
     def build(self) -> 'Buildable':
         return Column([
             Styler(
                 Row(children=self.__get_column_name_cells()),
                 self.column_name_style
             ),
             Styler(
-                Column(children=self.__get_value_rows()),
+                Row(children=self.__get_value_columns()),
                 self.data_style
             )
         ])
 
     def __get_column_name_cells(self) -> list[Buildable]:
         excel_cells: list[Buildable] = []
         for column in self.columns:
@@ -70,21 +63,29 @@
                 Styler(
                     ExcelCell(column.name),
                     column.column_name_style
                 )
             )
         return excel_cells
 
-    def __get_value_rows(self) -> list[Buildable]:
-        rows: list[Buildable] = []
-        for model in self.data:
+    def __get_value_columns(self) -> list[Buildable]:
+        columns: list[Buildable] = []
+        for column in self.columns:
             excel_cells = []
-            for column in self.columns:
+            conditional_style_names: list[str] = []
+            for model in self.data:
+                conditional_style_index: Union[int, None] = None
                 value = column.value(model)
-                style_id: Union[int, None] = None
-                style_index = column.value_style(
-                    model) if column.value_style else None
-                if style_index is not None:
-                    style_id = self.value_styles[style_index] # type: ignore
-                excel_cells.append(ExcelCell(value, style_id))
-            rows.append(Row(children=excel_cells))
-        return rows
+                if column.conditional_style is not None:
+                    conditional_style_index = column.conditional_style.selector(model)
+                excel_cells.append(ExcelCell(value, conditional_style_index))
+            columns.append(
+                Styler(
+                    ConditionalStyler(
+                        Column(children=excel_cells),
+                        column.conditional_style.styles if column.conditional_style is not None else [],
+                        conditional_style_names
+                    ),
+                    column.value_style
+                )
+            )
+        return columns
```

### Comparing `excel_framework-0.1.1/src/excel_framework/excel/excel_file.py` & `excel_framework-0.2.0/src/excel_framework/excel/excel_file.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/internals/build_context.py` & `excel_framework-0.2.0/src/excel_framework/internals/build_context.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,50 +2,39 @@
 from typing import Union
 from dataclasses import dataclass
 from openpyxl.workbook import Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.styles import NamedStyle
 from ..sizes.resizer import Resizer
 from ..sizes.dimension import Dimension, ColumnDimension
-from ..sizes.size import Size
-from ..styling.border import ParentBorderCoordinates
 from ..styling.style import Style
 
 @dataclass
 class StyleManager:
     next_style_id: int = 1
 
-    def add_named_style(self, workbook: Workbook, style: Style) -> int:
-        new_named_style = NamedStyle(f"{self.next_style_id}")
+    def add_named_style(self, workbook: Workbook, style: Style) -> str:
+        style_name = str(self.next_style_id) 
+        new_named_style = NamedStyle(style_name)
         style.apply_to(new_named_style)
         workbook.add_named_style(new_named_style)
-        if style.parent_border is not None:
-            for postfix in ("top", "right", "bottom", "left"):
-                has_top = postfix == "top"
-                has_right = postfix == "right"
-                has_bottom = postfix == "bottom"
-                has_left = postfix == "left"
-                new_named_style = NamedStyle(f"{self.next_style_id}-{postfix}")
-                style.apply_to(new_named_style)
-                style.parent_border.apply_as_parent_to(new_named_style, self.next_style_id, has_top, has_right, has_bottom, has_left)
-                workbook.add_named_style(new_named_style)
         self.next_style_id += 1
-        return self.next_style_id - 1
+        return style_name 
 
 @dataclass
 class BuildContext(ABC):
     workbook: Workbook
     sheet: Worksheet
     resizer: Resizer
     style_manager: StyleManager
     row_index: int = 1
     column_index: int = 1
     style: Union[Style, None] = None
-    style_id: Union[int, None] = None
-    parent_border_coordinates: Union[ParentBorderCoordinates, None] = None
+    style_name: Union[str, None] = None
+    conditional_style_names: Union[list[str], None] = None
 
     @classmethod
     def initial(cls, title: str, dimensions: list[Dimension]) -> 'BuildContext':
         workbook = Workbook()
         workbook.active.title = title
         return BuildContext(workbook, workbook.active, Resizer(workbook.active, dimensions), StyleManager())
 
@@ -55,32 +44,43 @@
 
     def collect_length(self, length: int):
         self.resizer.collect_length(self.row_index, self.column_index, length)
 
     def collect_column_dimension(self, dimension: ColumnDimension):
         self.resizer.collect_column_dimension(dimension)
 
-    def with_style_change(self, new_style: Union[Style, None], child_size: Size) -> 'BuildContext':
+    def with_style_change(self, new_style: Union[Style, None]) -> 'BuildContext':
         if new_style is None:
             return self
         if self.style:
             new_style = self.style.join(new_style)
-        new_parent_border_coordinates = self.parent_border_coordinates
-        if new_style.parent_border:
-            new_parent_border_coordinates = ParentBorderCoordinates(
-                self.row_index,
-                self.column_index,
-                self.row_index + child_size.height - 1,
-                self.column_index + child_size.width - 1
-            )
-        style_id = self.style_manager.add_named_style(self.workbook, new_style)
+        added_style_name = self.style_manager.add_named_style(self.workbook, new_style)
         return BuildContext(
             self.workbook,
             self.sheet,
             self.resizer,
             self.style_manager,
             self.row_index,
             self.column_index,
             new_style,
-            style_id,
-            new_parent_border_coordinates
-        )
+            added_style_name,
+            self.conditional_style_names
+        )
+    
+    def with_conditional_styles(self, styles: list[Style], style_names: list[str]) -> 'BuildContext':
+        for style in styles:
+            if self.style:
+                style = self.style.join(style) 
+            added_style_name = self.style_manager.add_named_style(self.workbook, style)
+            style_names.append(added_style_name)
+        return BuildContext(
+            self.workbook,
+            self.sheet,
+            self.resizer,
+            self.style_manager,
+            self.row_index,
+            self.column_index,
+            self.style,
+            self.style_name,
+            style_names
+        )
+
```

### Comparing `excel_framework-0.1.1/src/excel_framework/internals/buildable.py` & `excel_framework-0.2.0/src/excel_framework/internals/buildable.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/sizes/dimension.py` & `excel_framework-0.2.0/src/excel_framework/sizes/dimension.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/sizes/resizer.py` & `excel_framework-0.2.0/src/excel_framework/sizes/resizer.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/styling/color.py` & `excel_framework-0.2.0/src/excel_framework/styling/color.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/styling/fill.py` & `excel_framework-0.2.0/src/excel_framework/styling/fill.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/src/excel_framework/styling/style.py` & `excel_framework-0.2.0/src/excel_framework/styling/style.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,25 @@
 from .border import Border
 
 
 @dataclass(frozen=True)
 class Style(StylePart):
     fill: Union[Fill, None] = None
     text_style: Union[TextStyle, None] = None
-    parent_border: Union[Border, None] = None
     child_border: Union[Border, None] = None
 
     @override
     def join(self, other: Union['Style', None]) -> 'Style':
         if other is None:
             return self
         return Style(
             fill=other.fill if self.fill is None else self.fill.join(
                 other.fill),
             text_style=other.text_style if self.text_style is None else self.text_style.join(
                 other.text_style),
-            parent_border=other.parent_border if self.parent_border is None else self.parent_border.join(
-                other.parent_border),
             child_border=other.child_border if self.child_border is None else self.child_border.join(
                 other.child_border)
         )
 
     def apply_to(self, cell: Union[NamedStyle, Cell]) -> None:
         if self.fill:
             self.fill.apply_to(cell)
```

### Comparing `excel_framework-0.1.1/src/excel_framework/styling/text_style.py` & `excel_framework-0.2.0/src/excel_framework/styling/text_style.py`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/LICENSE` & `excel_framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_framework-0.1.1/pyproject.toml` & `excel_framework-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_framework"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Jonathan Dück", email="jonathan.dueck@digital-confidence.de" },
 ]
 description = "A small example package"
 readme = "README.md"
 dependencies = [
     "openpyxl",
```

### Comparing `excel_framework-0.1.1/PKG-INFO` & `excel_framework-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_framework
-Version: 0.1.1
+Version: 0.2.0
 Summary: A small example package
 Project-URL: Homepage, https://github.com/TheUltimateOptimist/excel_framework
 Project-URL: Bug Tracker, https://github.com/TheUltimateOptimist/excel_framework/issues
 Author-email: Jonathan Dück <jonathan.dueck@digital-confidence.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

