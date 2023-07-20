# Comparing `tmp/fastapi_simple_pagination-1.3.0.tar.gz` & `tmp/fastapi_simple_pagination-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_simple_pagination-1.3.0.tar", max compression
+gzip compressed data, was "fastapi_simple_pagination-1.3.1.tar", max compression
```

## Comparing `fastapi_simple_pagination-1.3.0.tar` & `fastapi_simple_pagination-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      240 2023-02-06 17:53:10.890056 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/__init__.py
--rw-r--r--   0        0        0      561 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/common.py
--rw-r--r--   0        0        0     2287 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/cursor_pagination.py
--rw-r--r--   0        0        0     2000 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/deps.py
--rw-r--r--   0        0        0        0 2023-02-06 16:43:13.077613 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/py.typed
--rw-r--r--   0        0        0     4108 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/schemas.py
--rw-r--r--   0        0        0      751 2023-04-18 13:08:01.381787 fastapi_simple_pagination-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 fastapi_simple_pagination-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-02-06 17:53:10.000000 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/__init__.py
+-rw-r--r--   0        0        0      561 2023-04-18 13:07:42.000000 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/common.py
+-rw-r--r--   0        0        0     2305 2023-07-20 13:03:08.757860 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/cursor_pagination.py
+-rw-r--r--   0        0        0     2000 2023-04-18 13:07:42.000000 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/deps.py
+-rw-r--r--   0        0        0        0 2023-02-06 16:43:13.000000 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/py.typed
+-rw-r--r--   0        0        0     4079 2023-07-20 13:03:08.757860 fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/schemas.py
+-rw-r--r--   0        0        0      751 2023-07-20 13:03:08.757860 fastapi_simple_pagination-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 fastapi_simple_pagination-1.3.1/PKG-INFO
```

### Comparing `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/common.py` & `fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/common.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/cursor_pagination.py` & `fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/cursor_pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Any, Callable, List
 
 from fastapi import Query, Request
-from pydantic import HttpUrl, NonNegativeInt, parse_obj_as
+from pydantic import AnyHttpUrl, NonNegativeInt, parse_obj_as
 
 from .common import CountItems, Item, OtherItem, PaginatedMethodProtocol, QuerySize
 from .schemas import CursorPage
 
 
 def _identity(item: Any) -> Any:
     return item
@@ -40,32 +40,32 @@
 
     def _build_page(
         self, item_count: int, item_list: List[OtherItem], has_next: bool
     ) -> CursorPage[OtherItem]:
         return CursorPage(
             items=item_list,
             count=item_count,
-            current=parse_obj_as(HttpUrl, str(self.request.url)),
+            current=parse_obj_as(AnyHttpUrl, str(self.request.url)),
             next_url=self._build_next_url() if has_next else None,
             previous_url=self._build_previous_url() if self.offset > 0 else None,
             size=self.size,
             offset=self.offset,
         )
 
-    def _build_next_url(self) -> HttpUrl:
+    def _build_next_url(self) -> AnyHttpUrl:
         new_url = self.request.url.remove_query_params(
             ["offset", "size"]
         ).include_query_params(
             offset=self.offset + self.size,
             size=self.size,
         )
 
-        return parse_obj_as(HttpUrl, str(new_url))
+        return parse_obj_as(AnyHttpUrl, str(new_url))
 
-    def _build_previous_url(self) -> HttpUrl:
+    def _build_previous_url(self) -> AnyHttpUrl:
         offset = self.offset - self.size
         if offset < 0:
             offset = 0
         new_url = self.request.url.remove_query_params(
             ["offset", "size"]
         ).include_query_params(offset=offset, size=self.size)
-        return parse_obj_as(HttpUrl, str(new_url))
+        return parse_obj_as(AnyHttpUrl, str(new_url))
```

### Comparing `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/deps.py` & `fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/deps.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/schemas.py` & `fastapi_simple_pagination-1.3.1/fastapi_simple_pagination/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 from __future__ import annotations
 
 from asyncio import Task, create_task, ensure_future
 from typing import Any, Awaitable, Callable, Generic, List, Optional, Type, TypeVar
 
-from pydantic import (
-    AnyHttpUrl,
-    Field,
-    HttpUrl,
-    NonNegativeInt,
-    PositiveInt,
-    parse_obj_as,
-)
+from pydantic import AnyHttpUrl, Field, NonNegativeInt, PositiveInt, parse_obj_as
 from pydantic.generics import GenericModel
 
 from .common import Item, OtherItem
 
 
 class Page(GenericModel, Generic[Item]):
     count: int = Field(
@@ -92,21 +85,21 @@
     )
     size: PositiveInt = Field(
         description="The size of the page.",
     )
     count: NonNegativeInt = Field(
         description="How many items are saved in the store.",
     )
-    current: HttpUrl = Field(
+    current: AnyHttpUrl = Field(
         description="The URL of the current page.",
     )
-    next_url: Optional[HttpUrl] = Field(
+    next_url: Optional[AnyHttpUrl] = Field(
         description="The next page URL.",
     )
-    previous_url: Optional[HttpUrl] = Field(
+    previous_url: Optional[AnyHttpUrl] = Field(
         description="The previous page URL.",
     )
     items: List[Item] = Field(description="The items of the page.")
 
     def map(self, mapper: Callable[[Item], OtherItem]) -> "CursorPage[OtherItem]":
         items = [mapper(item) for item in self.items]
         return self._build_new_page(items)
```

### Comparing `fastapi_simple_pagination-1.3.0/pyproject.toml` & `fastapi_simple_pagination-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = "Simple and generic pagination dependencies for FastAPI."
 exclude = ["tests/"]
 name = "fastapi-simple-pagination"
-version = "1.3.0"
+version = "1.3.1"
 
 [tool.poetry.dependencies]
 fastapi = "<1.0.0"
 pydantic = "<2.0.0"
 python = ">=3.8.1, <4.0.0"
```

