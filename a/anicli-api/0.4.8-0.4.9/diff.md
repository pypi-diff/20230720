# Comparing `tmp/anicli_api-0.4.8.tar.gz` & `tmp/anicli_api-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.4.8.tar", max compression
+gzip compressed data, was "anicli_api-0.4.9.tar", max compression
```

## Comparing `anicli_api-0.4.8.tar` & `anicli_api-0.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     4216 2023-05-14 13:35:05.718934 anicli_api-0.4.8/README.MD
--rw-r--r--   0        0        0     2940 2023-07-18 19:39:10.511076 anicli_api-0.4.8/anicli_api/_http.py
--rw-r--r--   0        0        0      501 2023-07-18 19:39:10.500076 anicli_api-0.4.8/anicli_api/_logger.py
--rw-r--r--   0        0        0     3367 2023-07-18 11:11:13.119093 anicli_api-0.4.8/anicli_api/base.py
--rw-r--r--   0        0        0      615 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      921 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     2147 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0     1055 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3434 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/base.py
--rw-r--r--   0        0        0     1198 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1456 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     3999 2023-07-18 16:07:07.929504 anicli_api-0.4.8/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1837 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1697 2023-07-18 11:11:13.120093 anicli_api-0.4.8/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1106 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0     1139 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1527 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     2516 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     6163 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0    10726 2023-07-18 11:11:13.121093 anicli_api-0.4.8/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8722 2023-07-18 11:11:13.122093 anicli_api-0.4.8/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     5543 2023-07-18 11:11:13.122093 anicli_api-0.4.8/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     6462 2023-07-18 11:11:13.122093 anicli_api-0.4.8/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0       58 2023-01-25 23:19:25.549656 anicli_api-0.4.8/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-06 17:11:19.675846 anicli_api-0.4.8/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0      198 2023-07-18 11:11:13.122093 anicli_api-0.4.8/anicli_api/tools/utils.py
--rw-r--r--   0        0        0     2362 2023-07-18 19:40:13.203426 anicli_api-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 anicli_api-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-14 13:35:05.718934 anicli_api-0.4.9/README.MD
+-rw-r--r--   0        0        0     2940 2023-07-18 19:39:10.511076 anicli_api-0.4.9/anicli_api/_http.py
+-rw-r--r--   0        0        0      501 2023-07-18 19:39:10.500076 anicli_api-0.4.9/anicli_api/_logger.py
+-rw-r--r--   0        0        0     3442 2023-07-20 11:45:08.959241 anicli_api-0.4.9/anicli_api/base.py
+-rw-r--r--   0        0        0      615 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2147 2023-07-20 11:30:31.005346 anicli_api-0.4.9/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1055 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3434 2023-07-19 19:01:13.520443 anicli_api-0.4.9/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1198 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1456 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     3999 2023-07-19 19:01:13.520443 anicli_api-0.4.9/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1837 2023-07-19 19:01:13.520443 anicli_api-0.4.9/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1697 2023-07-18 11:11:13.120093 anicli_api-0.4.9/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1106 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1139 2023-07-19 19:01:13.520443 anicli_api-0.4.9/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1527 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2516 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     6163 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0    10726 2023-07-18 11:11:13.121093 anicli_api-0.4.9/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8722 2023-07-18 11:11:13.122093 anicli_api-0.4.9/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5543 2023-07-18 11:11:13.122093 anicli_api-0.4.9/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     6462 2023-07-18 11:11:13.122093 anicli_api-0.4.9/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0       58 2023-01-25 23:19:25.549656 anicli_api-0.4.9/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-06 17:11:19.675846 anicli_api-0.4.9/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0      198 2023-07-18 11:11:13.122093 anicli_api-0.4.9/anicli_api/tools/utils.py
+-rw-r--r--   0        0        0     2362 2023-07-20 11:45:20.152371 anicli_api-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 anicli_api-0.4.9/PKG-INFO
```

### Comparing `anicli_api-0.4.8/README.MD` & `anicli_api-0.4.9/README.MD`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/_http.py` & `anicli_api-0.4.9/anicli_api/_http.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/base.py` & `anicli_api-0.4.9/anicli_api/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, ClassVar, List, Optional, Type
+from typing import TYPE_CHECKING, ClassVar, List, Optional, Type, Any
 
 from parsel import Selector
 from scrape_schema import BaseSchema
 
 from anicli_api._http import HTTPAsync, HTTPSync
 from anicli_api.player import ALL_DECODERS
 
@@ -113,25 +113,25 @@
     url: str = NotImplemented
     dub: str = NotImplemented
 
     def _pre_validate_url_attr(self) -> None:
         if self.url is NotImplemented:
             raise AttributeError(f"{self.__class__.__name__} missing url attribute.")
 
-    def get_videos(self) -> List["Video"]:
+    def get_videos(self, **httpx_kwargs: Any) -> List["Video"]:
         self._pre_validate_url_attr()
         for extractor in self.ALL_VIDEO_EXTRACTORS:
             if self.url == extractor():
-                return extractor().parse(self.url)
+                return extractor(**httpx_kwargs).parse(self.url)
         warnings.warn(f"Failed extractor videos from {self.url}", stacklevel=4)
         return []
 
-    async def a_get_videos(self) -> List["Video"]:
+    async def a_get_videos(self, **httpx_kwargs: Any) -> List["Video"]:
         self._pre_validate_url_attr()
         for extractor in self.ALL_VIDEO_EXTRACTORS:
             if self.url == extractor():
-                return await extractor().a_parse(self.url)
+                return await extractor(**httpx_kwargs).a_parse(self.url)
         warnings.warn(
             f"Failed extractor videos from {self.url}. " f"Maybe needed video extractor not implemented?",
             stacklevel=4,
         )
         return []
```

### Comparing `anicli_api-0.4.8/anicli_api/player/__init__.py` & `anicli_api-0.4.9/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/__template__.py` & `anicli_api-0.4.9/anicli_api/player/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/aniboom.py` & `anicli_api-0.4.9/anicli_api/player/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/animejoy.py` & `anicli_api-0.4.9/anicli_api/player/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/base.py` & `anicli_api-0.4.9/anicli_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/csst.py` & `anicli_api-0.4.9/anicli_api/player/csst.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/dzen.py` & `anicli_api-0.4.9/anicli_api/player/dzen.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/kodik.py` & `anicli_api-0.4.9/anicli_api/player/kodik.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/mailru.py` & `anicli_api-0.4.9/anicli_api/player/mailru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/okru.py` & `anicli_api-0.4.9/anicli_api/player/okru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/sibnet.py` & `anicli_api-0.4.9/anicli_api/player/sibnet.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/sovetromantica.py` & `anicli_api-0.4.9/anicli_api/player/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/player/vkcom.py` & `anicli_api-0.4.9/anicli_api/player/vkcom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/__template__.py` & `anicli_api-0.4.9/anicli_api/source/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/anilibria.py` & `anicli_api-0.4.9/anicli_api/source/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/animego.py` & `anicli_api-0.4.9/anicli_api/source/animego.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/animejoy.py` & `anicli_api-0.4.9/anicli_api/source/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/animevost.py` & `anicli_api-0.4.9/anicli_api/source/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/source/sovetromantica.py` & `anicli_api-0.4.9/anicli_api/source/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.9/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.8/pyproject.toml` & `anicli_api-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.4.8"
+version = "0.4.9"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
```

### Comparing `anicli_api-0.4.8/PKG-INFO` & `anicli_api-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-api
-Version: 0.4.8
+Version: 0.4.9
 Summary: Anime extractor api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: Georgiy aka Vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

