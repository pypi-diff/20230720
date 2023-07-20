# Comparing `tmp/dynamicadaptor-0.4.3.tar.gz` & `tmp/dynamicadaptor-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.4.3.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.4.tar", max compression
```

## Comparing `dynamicadaptor-0.4.3.tar` & `dynamicadaptor-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/LICENSE
--rw-r--r--   0        0        0    10010 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/README.md
--rw-r--r--   0        0        0     2136 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    20217 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3402 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      500 2023-05-16 08:27:06.721344 dynamicadaptor-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/LICENSE
+-rw-r--r--   0        0        0    10010 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/README.md
+-rw-r--r--   0        0        0     2136 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20217 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3849 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      500 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.4/PKG-INFO
```

### Comparing `dynamicadaptor-0.4.3/LICENSE` & `dynamicadaptor-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/README.md` & `dynamicadaptor-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.4/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.4/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.4/dynamicadaptor/DynamicConversion.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.4/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.3/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.4/dynamicadaptor/Majors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List, Optional
+from typing import List, Optional,Union
 
 from pydantic import BaseModel, Json
 
 
 # 图片
 class DrawItem(BaseModel):
     height: int
     width: int
-    src: str
+    url: str
 
 
 class Draw(BaseModel):
     items: List[DrawItem]
 
 
 # 视频
@@ -127,22 +127,40 @@
     desc:Optional[str]
     stat:Optional[Stat]
     badge:Optional[Badge]
 
 class MNone(BaseModel):
     tips:str
 
+class Emoji(BaseModel):
+    icon_url: Optional[str]
+    text: Optional[str]
+    type: Union[int, str, None]
+class RichTextNodes(BaseModel):
+    type:str
+    text:str
+    orig_text: Optional[str]
+    emoji: Optional[Emoji]
+
+class Summary(BaseModel):
+    text:str
+    rich_text_nodes:List[RichTextNodes]
+    
+class OPUS(BaseModel):
+    pics:Optional[List[DrawItem]]
+    summary:Summary
+    title:str
 # class MajorDetail(Enum):
 #     """
 #     类型          动态类型        示例动态
 #     draw         图片            741262186696933397
 #     archive      视频            739851131027456201
 #     live_rcmd    直播
 #     ugc_season    合集           755703296984875092 
-#     article      专栏            720929682647679043
+#     article      专栏            819930757423169558
 #     common     装扮 活动等        551309621391003098/743181895357956118
 #     music       音乐             692040384055869478
 #     pgc         电影/电视剧等     633983562923638785
 #     medialist   收藏列表          645144864359448578
 #     courses     课程             440646043801479846
 #     live        转发直播          727260760787386403
 #     """
@@ -157,8 +175,9 @@
     common: Optional[Common]
     music: Optional[Music]
     pgc: Optional[Pgc]
     medialist: Optional[MediaList]
     courses: Optional[Courses]
     live: Optional[Live]
     ugc_season: Optional[UgcSeason]
+    opus:Optional[OPUS]
     none:Optional[MNone]
```

### Comparing `dynamicadaptor-0.4.3/PKG-INFO` & `dynamicadaptor-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

