# Comparing `tmp/excel_framework-0.0.9.tar.gz` & `tmp/excel_framework-0.1.0.tar.gz`

## Comparing `excel_framework-0.0.9.tar` & `excel_framework-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/buildables/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/buildables/layout/column.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/buildables/layout/row.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/buildables/layout/table.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/buildables/non_layout/excel_cell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/excel/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/excel/excel_file.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/excel/excel_sheet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/internals/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/internals/build_context.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/internals/buildable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/sizes/__init__.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/sizes/dimension.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/sizes/resizer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/sizes/size.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/__init__.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/border.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/color.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/fill.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/style.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/style_part.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/styler.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 excel_framework-0.0.9/src/excel_framework/styling/text_style.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_framework-0.0.9/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 excel_framework-0.0.9/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.0.9/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 excel_framework-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 excel_framework-0.1.0/test.py
+-rw-r--r--   0        0        0   764402 2020-02-02 00:00:00.000000 excel_framework-0.1.0/testfile.xlsx
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/buildables/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/buildables/layout/column.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/buildables/layout/row.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/buildables/layout/table.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/buildables/non_layout/excel_cell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/excel/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/excel/excel_file.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/excel/excel_sheet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/internals/__init__.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/internals/build_context.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/internals/buildable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/sizes/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/sizes/dimension.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/sizes/resizer.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/sizes/size.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/__init__.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/border.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/color.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/fill.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/style.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/style_part.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/styler.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 excel_framework-0.1.0/src/excel_framework/styling/text_style.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 excel_framework-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 excel_framework-0.1.0/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 excel_framework-0.1.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 excel_framework-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 excel_framework-0.1.0/PKG-INFO
```

### Comparing `excel_framework-0.0.9/src/excel_framework/__init__.py` & `excel_framework-0.1.0/src/excel_framework/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .internals.buildable import Buildable 
-from .excel.excel_file import ExcelFile
-from .excel.excel_sheet import ExcelSheet
-from .buildables.layout.column import Column
-from .buildables.layout.row import Row
-from .buildables.layout.table import Table
-from .buildables.non_layout.excel_cell import ExcelCell
-from .sizes.dimension import FixedWidth, AutoWidth, Dimension, RowDimension, ColumnDimension 
-from .styling.border import BorderStyle, BorderSide
-from .styling.color import Color, Colors
-from .styling.fill import Fill
-from .styling.style import Style
-from .styling.styler import Styler
+from .internals.buildable import Buildable 
+from .excel.excel_file import ExcelFile
+from .excel.excel_sheet import ExcelSheet
+from .buildables.layout.column import Column
+from .buildables.layout.row import Row
+from .buildables.layout.table import Table, TableColumn
+from .buildables.non_layout.excel_cell import ExcelCell
+from .sizes.dimension import FixedWidth, AutoWidth, Dimension, RowDimension, ColumnDimension 
+from .styling.border import BorderStyle, BorderSide, Border
+from .styling.color import Color, Colors
+from .styling.fill import Fill
+from .styling.style import Style
+from .styling.styler import Styler
 from .styling.text_style import TextStyle, VerticalAlignment, HorizontalAlignment, Underline
```

### Comparing `excel_framework-0.0.9/src/excel_framework/buildables/layout/column.py` & `excel_framework-0.1.0/src/excel_framework/buildables/layout/row.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from ...internals.buildable import Buildable
-from ...internals.build_context import BuildContext
-from ...sizes.size import Size
-from overrides import override
-
-class Column(Buildable):
-    def __init__(self, children: list[Buildable] = []) -> None:
-        self.children = children
-        super().__init__()
-
-    @override
-    def get_size(self) -> Size:
-        width = 0
-        height = 0
-        for child in self.children:
-            child_size = child.get_size()
-            height += child_size.height
-            if child_size.width > width:
-                width = child_size.width
-        return Size(width, height)
-
-    @override
-    def internal_build(self, context: BuildContext) -> None:
-        row_index = context.row_index
-        column_index = context.column_index
-        for child in self.children:
-            child_size = child.get_size()
-            child.internal_build(context)
-            row_index += child_size.height
-            context.row_index = row_index
-            context.column_index = column_index
+from ...internals.buildable import Buildable
+from ...internals.build_context import BuildContext
+from ...sizes.size import Size
+from overrides import override
+
+class Row(Buildable):
+    def __init__(self, children: list[Buildable] = []) -> None:
+        self.children = children
+        super().__init__()
+
+    @override
+    def get_size(self) -> Size:
+        width = 0
+        height = 0
+        for child in self.children:
+            child_size = child.get_size()
+            width += child_size.width
+            if child_size.height > height:
+                height = child_size.height
+        return Size(width, height)
+
+    @override
+    def internal_build(self, context: BuildContext) -> None:
+        row_index = context.row_index
+        column_index = context.column_index
+        for child in self.children:
+            child_size = child.get_size()
+            child.internal_build(context)
+            column_index += child_size.width
+            context.column_index = column_index
+            context.row_index = row_index
+
+
+
```

### Comparing `excel_framework-0.0.9/src/excel_framework/buildables/layout/row.py` & `excel_framework-0.1.0/src/excel_framework/buildables/layout/column.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from ...internals.buildable import Buildable
-from ...internals.build_context import BuildContext
-from ...sizes.size import Size
-from overrides import override
-
-class Row(Buildable):
-    def __init__(self, children: list[Buildable] = []) -> None:
-        self.children = children
-        super().__init__()
-
-    @override
-    def get_size(self) -> Size:
-        width = 0
-        height = 0
-        for child in self.children:
-            child_size = child.get_size()
-            width += child_size.width
-            if child_size.height > height:
-                height = child_size.height
-        return Size(width, height)
-
-    @override
-    def internal_build(self, context: BuildContext) -> None:
-        row_index = context.row_index
-        column_index = context.column_index
-        for child in self.children:
-            child_size = child.get_size()
-            child.internal_build(context)
-            column_index += child_size.width
-            context.column_index = column_index
-            context.row_index = row_index
-
-
-
+from ...internals.buildable import Buildable
+from ...internals.build_context import BuildContext
+from ...sizes.size import Size
+from overrides import override
+
+class Column(Buildable):
+    def __init__(self, children: list[Buildable] = []) -> None:
+        self.children = children
+        super().__init__()
+
+    @override
+    def get_size(self) -> Size:
+        width = 0
+        height = 0
+        for child in self.children:
+            child_size = child.get_size()
+            height += child_size.height
+            if child_size.width > width:
+                width = child_size.width
+        return Size(width, height)
+
+    @override
+    def internal_build(self, context: BuildContext) -> None:
+        row_index = context.row_index
+        column_index = context.column_index
+        for child in self.children:
+            child_size = child.get_size()
+            child.internal_build(context)
+            row_index += child_size.height
+            context.row_index = row_index
+            context.column_index = column_index
```

### Comparing `excel_framework-0.0.9/src/excel_framework/excel/excel_file.py` & `excel_framework-0.1.0/src/excel_framework/excel/excel_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Union
-from dataclasses import dataclass, field
-from .excel_sheet import ExcelSheet
-from ..styling.styler import Styler
-from ..styling.style import Style
-from ..internals.build_context import BuildContext
-
-
-@dataclass(frozen=True)
-class ExcelFile:
-    filename: str
-    sheets: list[ExcelSheet] = field(default_factory=list)
-    global_style: Union[Style, None] = None
-
-    def create(self):
-        if len(self.sheets) == 0:
-            return
-        context = BuildContext.initial(
-            self.sheets[0].title, self.sheets[0].dimensions)
-        for i, sheet in enumerate(self.sheets):
-            if i > 0:
-                context = context.new_sheet(sheet.title, sheet.dimensions)
-            if sheet.child and self.global_style:
-                Styler.from_style(
-                    sheet.child, self.global_style).internal_build(context)
-            elif sheet.child:
-                sheet.child.internal_build(context)
-            context.resizer.resize()
-        context.workbook.save(self.filename)
+from typing import Union
+from dataclasses import dataclass, field
+from .excel_sheet import ExcelSheet
+from ..styling.styler import Styler
+from ..styling.style import Style
+from ..internals.build_context import BuildContext
+
+
+@dataclass(frozen=True)
+class ExcelFile:
+    filename: str
+    sheets: list[ExcelSheet] = field(default_factory=list)
+    global_style: Union[Style, None] = None
+
+    def create(self):
+        if len(self.sheets) == 0:
+            return
+        context = BuildContext.initial(
+            self.sheets[0].title, self.sheets[0].dimensions)
+        for i, sheet in enumerate(self.sheets):
+            if i > 0:
+                context = context.new_sheet(sheet.title, sheet.dimensions)
+            if sheet.child and self.global_style:
+                Styler(
+                    sheet.child, self.global_style).internal_build(context)
+            elif sheet.child:
+                sheet.child.internal_build(context)
+            context.resizer.resize()
+        context.workbook.save(self.filename)
```

### Comparing `excel_framework-0.0.9/src/excel_framework/internals/buildable.py` & `excel_framework-0.1.0/src/excel_framework/internals/buildable.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from abc import ABC
-from overrides import EnforceOverrides
-from ..sizes.size import Size
-from .build_context import BuildContext
-
-
-class Buildable(ABC, EnforceOverrides):
-    def build(self) -> 'Buildable':
-        return self
-
-    def internal_build(self, context: BuildContext) -> None:
-        if self.build() == self:
-            raise Exception(
-                f"Error: build method not defined: The class {self.__class__.__name__,} failed to override the build method")
-        self.build().internal_build(context)
-
-    def get_size(self) -> Size:
-        if self.build() == self:
-            raise Exception(
-                f"Error: build method not defined: The class {self.__class__.__name__,} failed to override the build method")
-        return self.build().get_size()
+from abc import ABC
+from overrides import EnforceOverrides
+from ..sizes.size import Size
+from .build_context import BuildContext
+
+
+class Buildable(ABC, EnforceOverrides):
+    def build(self) -> 'Buildable':
+        return self
+
+    def internal_build(self, context: BuildContext) -> None:
+        if self.build() == self:
+            raise Exception(
+                f"Error: build method not defined: The class {self.__class__.__name__,} failed to override the build method")
+        self.build().internal_build(context)
+
+    def get_size(self) -> Size:
+        if self.build() == self:
+            raise Exception(
+                f"Error: build method not defined: The class {self.__class__.__name__,} failed to override the build method")
+        return self.build().get_size()
```

### Comparing `excel_framework-0.0.9/src/excel_framework/sizes/resizer.py` & `excel_framework-0.1.0/src/excel_framework/sizes/resizer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from openpyxl.worksheet.worksheet import Worksheet
-from typing import Union
-from openpyxl.utils import get_column_letter
-from .dimension import ColumnDimension, RowDimension, Dimension, FixedInternalDimension, InternalDimension
-
-
-class Resizer:
-    def __init__(self, sheet: Worksheet, dimensions: list[Dimension]) -> None:
-        self.sheet = sheet
-        self.row_dimensions = dict[Union[int, None], FixedInternalDimension]()
-        self.column_dimensions = dict[Union[int,
-                                            None], InternalDimension]()
-        for dimension in dimensions:
-            if isinstance(dimension, RowDimension):
-                self.row_dimensions[dimension.index] = dimension.to_internal()
-            elif isinstance(dimension, ColumnDimension):
-                self.column_dimensions[dimension.index] = dimension.to_internal(
-                )
-
-    def collect_length(self, row_index: int, column_index: int, length: int) -> None:
-        if row_index not in self.row_dimensions and None in self.row_dimensions:
-            self.row_dimensions[row_index] = self.row_dimensions[None]
-        if column_index in self.column_dimensions:
-            dimension = self.column_dimensions[column_index]
-            self.column_dimensions[column_index] = dimension.with_length(
-                length)
-        elif None in self.column_dimensions:
-            dimension = self.column_dimensions[None]
-            self.column_dimensions[column_index] = dimension.with_length(
-                length)
-
-    def collect_column_dimension(self, dimension: ColumnDimension):
-        self.column_dimensions[dimension.index] = dimension.to_internal()
-
-    def resize(self):
-        self.__resize_rows()
-        self.__resize_columns()
-
-    def __resize_rows(self):
-        if None in self.row_dimensions:
-            del self.row_dimensions[None]
-        for row_index in self.row_dimensions:
-            self.sheet.row_dimensions[row_index].height = self.row_dimensions[row_index].final_value()
-
-    def __resize_columns(self):
-        if None in self.column_dimensions:
-            del self.column_dimensions[None]
-        for col_index in self.column_dimensions:
-            assert(type(col_index) is int)
-            column_dimension = self.column_dimensions[col_index]
-            column_letter = get_column_letter(col_index)
-            self.sheet.column_dimensions[column_letter].width = column_dimension.final_value()
+from openpyxl.worksheet.worksheet import Worksheet
+from typing import Union
+from openpyxl.utils import get_column_letter
+from .dimension import ColumnDimension, RowDimension, Dimension, FixedInternalDimension, InternalDimension
+
+
+class Resizer:
+    def __init__(self, sheet: Worksheet, dimensions: list[Dimension]) -> None:
+        self.sheet = sheet
+        self.row_dimensions = dict[Union[int, None], FixedInternalDimension]()
+        self.column_dimensions = dict[Union[int,
+                                            None], InternalDimension]()
+        for dimension in dimensions:
+            if isinstance(dimension, RowDimension):
+                self.row_dimensions[dimension.index] = dimension.to_internal()
+            elif isinstance(dimension, ColumnDimension):
+                self.column_dimensions[dimension.index] = dimension.to_internal(
+                )
+
+    def collect_length(self, row_index: int, column_index: int, length: int) -> None:
+        if row_index not in self.row_dimensions and None in self.row_dimensions:
+            self.row_dimensions[row_index] = self.row_dimensions[None]
+        if column_index in self.column_dimensions:
+            dimension = self.column_dimensions[column_index]
+            self.column_dimensions[column_index] = dimension.with_length(
+                length)
+        elif None in self.column_dimensions:
+            dimension = self.column_dimensions[None]
+            self.column_dimensions[column_index] = dimension.with_length(
+                length)
+
+    def collect_column_dimension(self, dimension: ColumnDimension):
+        self.column_dimensions[dimension.index] = dimension.to_internal()
+
+    def resize(self):
+        self.__resize_rows()
+        self.__resize_columns()
+
+    def __resize_rows(self):
+        if None in self.row_dimensions:
+            del self.row_dimensions[None]
+        for row_index in self.row_dimensions:
+            self.sheet.row_dimensions[row_index].height = self.row_dimensions[row_index].final_value()
+
+    def __resize_columns(self):
+        if None in self.column_dimensions:
+            del self.column_dimensions[None]
+        for col_index in self.column_dimensions:
+            assert(type(col_index) is int)
+            column_dimension = self.column_dimensions[col_index]
+            column_letter = get_column_letter(col_index)
+            self.sheet.column_dimensions[column_letter].width = column_dimension.final_value()
```

### Comparing `excel_framework-0.0.9/src/excel_framework/styling/fill.py` & `excel_framework-0.1.0/src/excel_framework/styling/fill.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from dataclasses import dataclass
-from overrides import override
-from typing import Union
-from openpyxl.cell import Cell
-from openpyxl.styles import PatternFill
-from .color import *
-from .style import StylePart
-
-
-@dataclass(frozen=True)
-class Fill(StylePart):
-    color: Union[Color, None] = None
-
-    @override
-    def join(self, other: Union['Fill', None]) -> 'Fill':
-        if other is None:
-            return self
-        if other.color is not None:
-            return Fill(other.color)
-        return self
-
-    @override
-    def apply_to(self, cell: Cell) -> None:
-        if self.color is not None:
-            cell.fill = PatternFill(
-                start_color=self.color.hex, end_color=self.color.hex, fill_type="solid")
+from dataclasses import dataclass
+from overrides import override
+from typing import Union
+from openpyxl.cell import Cell
+from openpyxl.styles import PatternFill, NamedStyle
+from .color import *
+from .style import StylePart
+
+
+@dataclass(frozen=True)
+class Fill(StylePart):
+    color: Union[Color, None] = None
+
+    @override
+    def join(self, other: Union['Fill', None]) -> 'Fill':
+        if other is None:
+            return self
+        if other.color is not None:
+            return Fill(other.color)
+        return self
+
+    @override
+    def apply_to(self, cell: Union[Cell, NamedStyle]) -> None:
+        if self.color is not None:
+            cell.fill = PatternFill(
+                start_color=self.color.hex, end_color=self.color.hex, fill_type="solid")
```

### Comparing `excel_framework-0.0.9/src/excel_framework/styling/style.py` & `excel_framework-0.1.0/src/excel_framework/styling/style.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from typing import Union
-from dataclasses import dataclass
-
-from overrides import override
-from openpyxl.cell import Cell
-
-from .style_part import StylePart
-from .text_style import TextStyle
-from .fill import Fill
-from .border import Border
-
-
-@dataclass(frozen=True)
-class Style(StylePart):
-    fill: Union[Fill, None] = None
-    text_style: Union[TextStyle, None] = None
-    parent_border: Union[Border, None] = None
-    child_border: Union[Border, None] = None
-
-    @override
-    def join(self, other: Union['Style', None]) -> 'Style':
-        if other is None:
-            return self
-        return Style(
-            fill=other.fill if self.fill is None else self.fill.join(
-                other.fill),
-            text_style=other.text_style if self.text_style is None else self.text_style.join(
-                other.text_style),
-            parent_border=other.parent_border if self.parent_border is None else self.parent_border.join(
-                other.parent_border),
-            child_border=other.child_border if self.child_border is None else self.child_border.join(
-                other.child_border)
-        )
-
-    def apply_to(self, cell: Cell) -> None:
-        if self.fill:
-            self.fill.apply_to(cell)
-        if self.text_style:
-            self.text_style.apply_to(cell)
-        if self.child_border:
-            self.child_border.apply_to(cell)
+from typing import Union
+from dataclasses import dataclass
+
+from overrides import override
+from openpyxl.cell import Cell
+from openpyxl.styles import NamedStyle
+
+from .style_part import StylePart
+from .text_style import TextStyle
+from .fill import Fill
+from .border import Border
+
+
+@dataclass(frozen=True)
+class Style(StylePart):
+    fill: Union[Fill, None] = None
+    text_style: Union[TextStyle, None] = None
+    parent_border: Union[Border, None] = None
+    child_border: Union[Border, None] = None
+
+    @override
+    def join(self, other: Union['Style', None]) -> 'Style':
+        if other is None:
+            return self
+        return Style(
+            fill=other.fill if self.fill is None else self.fill.join(
+                other.fill),
+            text_style=other.text_style if self.text_style is None else self.text_style.join(
+                other.text_style),
+            parent_border=other.parent_border if self.parent_border is None else self.parent_border.join(
+                other.parent_border),
+            child_border=other.child_border if self.child_border is None else self.child_border.join(
+                other.child_border)
+        )
+
+    def apply_to(self, cell: Union[NamedStyle, Cell]) -> None:
+        if self.fill:
+            self.fill.apply_to(cell)
+        if self.text_style:
+            self.text_style.apply_to(cell)
+        if self.child_border:
+            self.child_border.apply_to(cell)
```

### Comparing `excel_framework-0.0.9/src/excel_framework/styling/text_style.py` & `excel_framework-0.1.0/src/excel_framework/styling/text_style.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from dataclasses import dataclass
-from typing import Union
-from overrides import override
-from .color import *
-from enum import Enum
-from openpyxl.cell import Cell
-import openpyxl.styles as openpyxl
-from .style import StylePart
-
-
-class VerticalAlignment(Enum):
-    TOP = 1
-    BOTTOM = 2
-    CENTER = 3
-
-
-class HorizontalAlignment(Enum):
-    LEFT = 1
-    RIGHT = 2
-    CENTER = 3
-
-
-class Underline(Enum):
-    single = "single"
-    double = "double"
-
-
-@dataclass(frozen=True)
-class TextStyle(StylePart):
-    font_size: Union[float, None] = None
-    font_color: Union[Color, None] = None
-    font_family: Union[str, None] = None
-    number_format: Union[str, None] = None
-    wrap_text: Union[bool, None] = None
-    shrink_to_fit: Union[bool, None] = None
-    horizontal_alignment: Union[HorizontalAlignment, None] = None
-    vertical_alignment: Union[VerticalAlignment, None] = None
-    bold: Union[bool, None] = None
-    italic: Union[bool, None] = None
-    underline: Union[Underline, None] = None
-
-    @override
-    def join(self, other: Union['TextStyle', None]) -> 'TextStyle':
-        if other is None:
-            return self
-        return TextStyle(
-            font_size=self.font_size if other.font_size is None else other.font_size,
-            font_color=self.font_color if other.font_color is None else other.font_color,
-            font_family=self.font_family if other.font_family is None else other.font_family,
-            number_format=self.number_format if other.number_format is None else other.number_format,
-            wrap_text=self.wrap_text if other.wrap_text is None else other.wrap_text,
-            shrink_to_fit=self.shrink_to_fit if other.shrink_to_fit is None else other.shrink_to_fit,
-            horizontal_alignment=self.horizontal_alignment if other.horizontal_alignment is None else other.horizontal_alignment,
-            vertical_alignment=self.vertical_alignment if other.vertical_alignment is None else other.vertical_alignment,
-            bold=self.bold if other.bold is None else other.bold,
-            italic=self.italic if other.italic is None else other.italic,
-            underline=self.underline if other.underline is None else other.underline,
-        )
-
-    @override
-    def apply_to(self, cell: Cell) -> None:
-        alignment = openpyxl.Alignment()
-        font = openpyxl.Font()
-        font.size = self.font_size
-        font.color = self.font_color if self.font_color is None else self.font_color.to_openpyxl()
-        font.name = self.font_family
-        cell.number_format = "" if self.number_format is None else self.number_format
-        alignment.wrap_text = self.wrap_text
-        alignment.shrink_to_fit = self.shrink_to_fit
-        alignment.horizontal = self.horizontal_alignment
-        alignment.vertical = self.vertical_alignment
-        font.bold = self.bold
-        font.italic = self.italic
-        font.underline = self.underline if self.underline is None else self.underline.value
-        cell.alignment = alignment
-        cell.font = font
+from dataclasses import dataclass
+from typing import Union
+from overrides import override
+from .color import *
+from enum import Enum
+from openpyxl.cell import Cell
+import openpyxl.styles as openpyxl
+from .style import StylePart
+
+
+class VerticalAlignment(Enum):
+    TOP = "top"
+    BOTTOM = "bottom"
+    CENTER = "center"
+
+
+class HorizontalAlignment(Enum):
+    LEFT = "left"
+    RIGHT = "right"
+    CENTER = "center"
+
+
+class Underline(Enum):
+    single = "single"
+    double = "double"
+
+
+@dataclass(frozen=True)
+class TextStyle(StylePart):
+    font_size: Union[float, None] = None
+    font_color: Union[Color, None] = None
+    font_family: Union[str, None] = None
+    number_format: Union[str, None] = None
+    wrap_text: Union[bool, None] = None
+    shrink_to_fit: Union[bool, None] = None
+    horizontal_alignment: Union[HorizontalAlignment, None] = None
+    vertical_alignment: Union[VerticalAlignment, None] = None
+    bold: Union[bool, None] = None
+    italic: Union[bool, None] = None
+    underline: Union[Underline, None] = None
+
+    @override
+    def join(self, other: Union['TextStyle', None]) -> 'TextStyle':
+        if other is None:
+            return self
+        return TextStyle(
+            font_size=self.font_size if other.font_size is None else other.font_size,
+            font_color=self.font_color if other.font_color is None else other.font_color,
+            font_family=self.font_family if other.font_family is None else other.font_family,
+            number_format=self.number_format if other.number_format is None else other.number_format,
+            wrap_text=self.wrap_text if other.wrap_text is None else other.wrap_text,
+            shrink_to_fit=self.shrink_to_fit if other.shrink_to_fit is None else other.shrink_to_fit,
+            horizontal_alignment=self.horizontal_alignment if other.horizontal_alignment is None else other.horizontal_alignment,
+            vertical_alignment=self.vertical_alignment if other.vertical_alignment is None else other.vertical_alignment,
+            bold=self.bold if other.bold is None else other.bold,
+            italic=self.italic if other.italic is None else other.italic,
+            underline=self.underline if other.underline is None else other.underline,
+        )
+
+    @override
+    def apply_to(self, cell: Union[Cell, openpyxl.NamedStyle]) -> None:
+        alignment = openpyxl.Alignment()
+        font = openpyxl.Font()
+        font.size = self.font_size
+        font.color = self.font_color if self.font_color is None else self.font_color.to_openpyxl()
+        font.name = self.font_family
+        cell.number_format = "" if self.number_format is None else self.number_format
+        alignment.wrap_text = self.wrap_text
+        alignment.shrink_to_fit = self.shrink_to_fit
+        alignment.horizontal = self.horizontal_alignment.value if self.horizontal_alignment else None
+        alignment.vertical = self.vertical_alignment.value if self.vertical_alignment else None
+        font.bold = self.bold
+        font.italic = self.italic
+        font.underline = self.underline if self.underline is None else self.underline.value
+        cell.alignment = alignment
+        cell.font = font
```

### Comparing `excel_framework-0.0.9/LICENSE` & `excel_framework-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2023 Jonathan Dück
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright © 2023 Jonathan Dück
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `excel_framework-0.0.9/PKG-INFO` & `excel_framework-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_framework
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Project-URL: Homepage, https://github.com/TheUltimateOptimist/excel_framework
 Project-URL: Bug Tracker, https://github.com/TheUltimateOptimist/excel_framework/issues
 Author-email: Jonathan Dück <jonathan.dueck@digital-confidence.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

