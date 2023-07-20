# Comparing `tmp/anime-api-1.0.0.tar.gz` & `tmp/anime_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anime-api-1.0.0.tar", max compression
+gzip compressed data, was "anime_api-1.0.1.tar", max compression
```

## Comparing `anime-api-1.0.0.tar` & `anime_api-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0     2880 2023-04-30 19:27:15.471233 anime-api-1.0.0/anime_api/__init__.py
--rw-r--r--   0        0        0      639 2023-04-30 19:28:07.202199 anime-api-1.0.0/anime_api/apis/__init__.py
--rw-r--r--   0        0        0     2310 2022-09-23 18:02:56.614001 anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/__init__.py
--rw-r--r--   0        0        0      691 2022-09-23 17:57:02.261044 anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/objects.py
--rw-r--r--   0        0        0     2773 2023-04-30 18:36:29.547204 anime-api-1.0.0/anime_api/apis/animechan/__init__.py
--rw-r--r--   0        0        0      291 2022-09-22 02:18:06.578699 anime-api-1.0.0/anime_api/apis/animechan/objects.py
--rw-r--r--   0        0        0     4279 2022-09-23 04:10:06.116378 anime-api-1.0.0/anime_api/apis/animu/__init__.py
--rw-r--r--   0        0        0     1173 2022-09-23 03:38:04.445841 anime-api-1.0.0/anime_api/apis/animu/objects.py
--rw-r--r--   0        0        0      305 2022-09-22 20:07:30.139095 anime-api-1.0.0/anime_api/apis/animu/operators.py
--rw-r--r--   0        0        0     1389 2022-09-23 18:09:21.227565 anime-api-1.0.0/anime_api/apis/animu/types.py
--rw-r--r--   0        0        0     2417 2023-04-30 19:43:43.560542 anime-api-1.0.0/anime_api/apis/catboys/__init__.py
--rw-r--r--   0        0        0      729 2023-04-30 19:41:10.887944 anime-api-1.0.0/anime_api/apis/catboys/objects.py
--rw-r--r--   0        0        0      954 2022-09-23 05:49:03.249801 anime-api-1.0.0/anime_api/apis/hmtai/__init__.py
--rw-r--r--   0        0        0      154 2022-09-23 05:30:57.313492 anime-api-1.0.0/anime_api/apis/hmtai/objects.py
--rw-r--r--   0        0        0     2695 2022-09-23 05:48:34.623887 anime-api-1.0.0/anime_api/apis/hmtai/types.py
--rw-r--r--   0        0        0     1878 2022-09-22 18:07:45.282716 anime-api-1.0.0/anime_api/apis/kyoko/__init__.py
--rw-r--r--   0        0        0      403 2022-09-22 18:05:57.144262 anime-api-1.0.0/anime_api/apis/kyoko/objects.py
--rw-r--r--   0        0        0     1093 2022-09-24 03:54:18.762863 anime-api-1.0.0/anime_api/apis/neko_love/__init__.py
--rw-r--r--   0        0        0      154 2022-09-24 03:48:07.233630 anime-api-1.0.0/anime_api/apis/neko_love/obejcts.py
--rw-r--r--   0        0        0      551 2022-09-24 03:50:18.715909 anime-api-1.0.0/anime_api/apis/neko_love/types.py
--rw-r--r--   0        0        0     2480 2023-01-05 00:21:13.478349 anime-api-1.0.0/anime_api/apis/nekobot/__init__.py
--rw-r--r--   0        0        0      218 2022-09-23 19:45:24.021158 anime-api-1.0.0/anime_api/apis/nekobot/objects.py
--rw-r--r--   0        0        0     2619 2022-09-23 19:34:10.172188 anime-api-1.0.0/anime_api/apis/nekobot/types.py
--rw-r--r--   0        0        0     8825 2023-04-30 18:42:02.897707 anime-api-1.0.0/anime_api/apis/nekos_api/__init__.py
--rw-r--r--   0        0        0     2866 2023-01-22 19:39:45.893226 anime-api-1.0.0/anime_api/apis/nekos_api/objects.py
--rw-r--r--   0        0        0      273 2023-01-07 01:51:02.302708 anime-api-1.0.0/anime_api/apis/nekos_api/types.py
--rw-r--r--   0        0        0      906 2023-01-20 16:26:36.249866 anime-api-1.0.0/anime_api/apis/nekos_api/utils.py
--rw-r--r--   0        0        0     3081 2022-09-25 06:27:20.877554 anime-api-1.0.0/anime_api/apis/nekos_best/__init__.py
--rw-r--r--   0        0        0      567 2022-09-24 07:23:19.795916 anime-api-1.0.0/anime_api/apis/nekos_best/objects.py
--rw-r--r--   0        0        0      968 2022-09-24 07:25:19.739409 anime-api-1.0.0/anime_api/apis/nekos_best/types.py
--rw-r--r--   0        0        0     3516 2022-09-23 06:53:16.302109 anime-api-1.0.0/anime_api/apis/nekos_life/__init__.py
--rw-r--r--   0        0        0      376 2022-09-23 06:53:10.701078 anime-api-1.0.0/anime_api/apis/nekos_life/objects.py
--rw-r--r--   0        0        0      572 2022-09-23 06:24:35.549196 anime-api-1.0.0/anime_api/apis/nekos_life/types.py
--rw-r--r--   0        0        0    13268 2022-09-24 06:38:01.720449 anime-api-1.0.0/anime_api/apis/nekos_moe/__init__.py
--rw-r--r--   0        0        0     7566 2022-09-24 06:29:46.181259 anime-api-1.0.0/anime_api/apis/nekos_moe/objects.py
--rw-r--r--   0        0        0      204 2022-09-24 05:11:01.078976 anime-api-1.0.0/anime_api/apis/nekos_moe/types.py
--rw-r--r--   0        0        0     8992 2022-09-22 07:09:04.847318 anime-api-1.0.0/anime_api/apis/studio_ghibli_api/__init__.py
--rw-r--r--   0        0        0    19826 2022-09-22 07:14:16.663507 anime-api-1.0.0/anime_api/apis/studio_ghibli_api/objects.py
--rw-r--r--   0        0        0     4432 2022-09-22 02:18:06.581683 anime-api-1.0.0/anime_api/apis/trace_moe/__init__.py
--rw-r--r--   0        0        0      838 2022-09-21 18:40:02.678562 anime-api-1.0.0/anime_api/apis/trace_moe/objects.py
--rw-r--r--   0        0        0     5117 2023-04-30 18:36:29.550442 anime-api-1.0.0/anime_api/apis/waifu_im/__init__.py
--rw-r--r--   0        0        0      851 2022-11-29 17:41:53.845590 anime-api-1.0.0/anime_api/apis/waifu_im/objects.py
--rw-r--r--   0        0        0     1328 2022-11-29 18:09:33.344067 anime-api-1.0.0/anime_api/apis/waifu_im/types.py
--rw-r--r--   0        0        0     2326 2022-09-22 17:42:34.392420 anime-api-1.0.0/anime_api/apis/waifu_pics/__init__.py
--rw-r--r--   0        0        0      154 2022-09-22 04:28:16.528286 anime-api-1.0.0/anime_api/apis/waifu_pics/objects.py
--rw-r--r--   0        0        0     1166 2022-09-22 04:22:41.729368 anime-api-1.0.0/anime_api/apis/waifu_pics/types.py
--rw-r--r--   0        0        0     1119 2023-01-07 02:40:38.038715 anime-api-1.0.0/anime_api/exceptions.py
--rw-r--r--   0        0        0      479 2022-12-31 21:12:21.271167 anime-api-1.0.0/anime_api/utils.py
--rw-r--r--   0        0        0    14851 2022-09-21 17:32:59.458040 anime-api-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      509 2023-04-30 19:30:20.930473 anime-api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11404 2023-04-30 19:29:40.267119 anime-api-1.0.0/README.md
--rw-r--r--   0        0        0    12608 1970-01-01 00:00:00.000000 anime-api-1.0.0/setup.py
--rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 anime-api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2878 2023-07-20 20:36:09.396266 anime_api-1.0.1/anime_api/__init__.py
+-rw-r--r--   0        0        0      639 2023-07-20 20:36:09.397266 anime_api-1.0.1/anime_api/apis/__init__.py
+-rw-r--r--   0        0        0     2310 2023-07-20 20:36:09.398266 anime_api-1.0.1/anime_api/apis/anime_facts_rest_api/__init__.py
+-rw-r--r--   0        0        0      691 2023-07-20 20:36:09.398266 anime_api-1.0.1/anime_api/apis/anime_facts_rest_api/objects.py
+-rw-r--r--   0        0        0     2773 2023-07-20 20:36:09.399266 anime_api-1.0.1/anime_api/apis/animechan/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-20 20:36:09.400266 anime_api-1.0.1/anime_api/apis/animechan/objects.py
+-rw-r--r--   0        0        0     4279 2023-07-20 20:36:09.401265 anime_api-1.0.1/anime_api/apis/animu/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-20 20:36:09.402433 anime_api-1.0.1/anime_api/apis/animu/objects.py
+-rw-r--r--   0        0        0      305 2023-07-20 20:36:09.402433 anime_api-1.0.1/anime_api/apis/animu/operators.py
+-rw-r--r--   0        0        0     1389 2023-07-20 20:36:09.403435 anime_api-1.0.1/anime_api/apis/animu/types.py
+-rw-r--r--   0        0        0     2417 2023-07-20 20:36:09.405433 anime_api-1.0.1/anime_api/apis/catboys/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-20 20:36:09.405433 anime_api-1.0.1/anime_api/apis/catboys/objects.py
+-rw-r--r--   0        0        0      952 2023-07-20 20:36:09.407493 anime_api-1.0.1/anime_api/apis/hmtai/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-20 20:36:09.408436 anime_api-1.0.1/anime_api/apis/hmtai/objects.py
+-rw-r--r--   0        0        0     2695 2023-07-20 20:36:09.409433 anime_api-1.0.1/anime_api/apis/hmtai/types.py
+-rw-r--r--   0        0        0     1878 2023-07-20 20:36:09.411595 anime_api-1.0.1/anime_api/apis/kyoko/__init__.py
+-rw-r--r--   0        0        0      403 2023-07-20 20:36:09.412622 anime_api-1.0.1/anime_api/apis/kyoko/objects.py
+-rw-r--r--   0        0        0     1093 2023-07-20 20:36:09.413622 anime_api-1.0.1/anime_api/apis/neko_love/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-20 20:36:09.414623 anime_api-1.0.1/anime_api/apis/neko_love/obejcts.py
+-rw-r--r--   0        0        0      551 2023-07-20 20:36:09.415624 anime_api-1.0.1/anime_api/apis/neko_love/types.py
+-rw-r--r--   0        0        0     2480 2023-07-20 20:36:09.416642 anime_api-1.0.1/anime_api/apis/nekobot/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-20 20:36:09.417622 anime_api-1.0.1/anime_api/apis/nekobot/objects.py
+-rw-r--r--   0        0        0     2619 2023-07-20 20:36:09.417622 anime_api-1.0.1/anime_api/apis/nekobot/types.py
+-rw-r--r--   0        0        0     8825 2023-07-20 20:36:09.418622 anime_api-1.0.1/anime_api/apis/nekos_api/__init__.py
+-rw-r--r--   0        0        0     2866 2023-07-20 20:36:09.419623 anime_api-1.0.1/anime_api/apis/nekos_api/objects.py
+-rw-r--r--   0        0        0      273 2023-07-20 20:36:09.420642 anime_api-1.0.1/anime_api/apis/nekos_api/types.py
+-rw-r--r--   0        0        0      906 2023-07-20 20:36:09.421769 anime_api-1.0.1/anime_api/apis/nekos_api/utils.py
+-rw-r--r--   0        0        0     3081 2023-07-20 20:36:09.424329 anime_api-1.0.1/anime_api/apis/nekos_best/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-20 20:36:09.425150 anime_api-1.0.1/anime_api/apis/nekos_best/objects.py
+-rw-r--r--   0        0        0      968 2023-07-20 20:36:09.426156 anime_api-1.0.1/anime_api/apis/nekos_best/types.py
+-rw-r--r--   0        0        0     3516 2023-07-20 20:36:09.427870 anime_api-1.0.1/anime_api/apis/nekos_life/__init__.py
+-rw-r--r--   0        0        0      376 2023-07-20 20:36:09.427870 anime_api-1.0.1/anime_api/apis/nekos_life/objects.py
+-rw-r--r--   0        0        0      572 2023-07-20 20:36:09.428874 anime_api-1.0.1/anime_api/apis/nekos_life/types.py
+-rw-r--r--   0        0        0    13268 2023-07-20 20:36:09.430874 anime_api-1.0.1/anime_api/apis/nekos_moe/__init__.py
+-rw-r--r--   0        0        0     7566 2023-07-20 20:36:09.431966 anime_api-1.0.1/anime_api/apis/nekos_moe/objects.py
+-rw-r--r--   0        0        0      204 2023-07-20 20:36:09.431966 anime_api-1.0.1/anime_api/apis/nekos_moe/types.py
+-rw-r--r--   0        0        0     8992 2023-07-20 20:36:09.434002 anime_api-1.0.1/anime_api/apis/studio_ghibli_api/__init__.py
+-rw-r--r--   0        0        0    19826 2023-07-20 20:36:09.435002 anime_api-1.0.1/anime_api/apis/studio_ghibli_api/objects.py
+-rw-r--r--   0        0        0     4432 2023-07-20 20:36:09.435002 anime_api-1.0.1/anime_api/apis/trace_moe/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-20 20:36:09.436002 anime_api-1.0.1/anime_api/apis/trace_moe/objects.py
+-rw-r--r--   0        0        0     5117 2023-07-20 20:36:09.438002 anime_api-1.0.1/anime_api/apis/waifu_im/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-20 20:36:09.439015 anime_api-1.0.1/anime_api/apis/waifu_im/objects.py
+-rw-r--r--   0        0        0     1328 2023-07-20 20:36:09.442033 anime_api-1.0.1/anime_api/apis/waifu_im/types.py
+-rw-r--r--   0        0        0     2326 2023-07-20 20:36:09.443172 anime_api-1.0.1/anime_api/apis/waifu_pics/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-20 20:36:09.443172 anime_api-1.0.1/anime_api/apis/waifu_pics/objects.py
+-rw-r--r--   0        0        0     1166 2023-07-20 20:36:09.444172 anime_api-1.0.1/anime_api/apis/waifu_pics/types.py
+-rw-r--r--   0        0        0     1119 2023-07-20 20:36:09.445171 anime_api-1.0.1/anime_api/exceptions.py
+-rw-r--r--   0        0        0      479 2023-07-20 20:36:09.445171 anime_api-1.0.1/anime_api/utils.py
+-rw-r--r--   0        0        0    14851 2023-07-20 20:36:09.390222 anime_api-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      509 2023-07-20 20:38:31.363775 anime_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11404 2023-07-20 20:36:09.391302 anime_api-1.0.1/README.md
+-rw-r--r--   0        0        0    11815 1970-01-01 00:00:00.000000 anime_api-1.0.1/PKG-INFO
```

### Comparing `anime-api-1.0.0/anime_api/__init__.py` & `anime_api-1.0.1/anime_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     (
         "Anime News Network",
         None,
         "https://www.animenewsnetwork.com/encyclopedia/api.php",
         False,
     ),
     ("Notify.moe", None, "https://notify.moe/api", False),
-    ("Hmtai", apis.HmtaiAPI, "https://hmtai.herokuapp.com/endpoints", True),
+    ("Hmtai", apis.HmtaiAPI, "https://hmtai.hatsunia.cfd/endpoints", True),
     ("Nekos.life", None, "https://github.com/Nekos-life/nekos.py", False),
     ("NekoBot", apis.NekoBotAPI, "https://docs.nekobot.xyz/", True),
     ("Neko-love", apis.NekoLoveAPI, "https://docs.neko-love.xyz/", True),
     ("Nekos.moe", apis.NekosMoeAPI, "https://docs.nekos.moe/", True),
     ("Nekos.best", apis.NekosBest, "https://docs.nekos.best/", True),
     ("Shikimori", None, "https://shikimori.one/api/doc", False),
     ("Mangadex", None, "https://api.mangadex.org/docs.html", False),
@@ -63,10 +63,10 @@
         "Nekos API",
         apis.NekosAPI,
         "https://nekos.nekidev.com/docs/rest-api/endpoints",
         True,
     ),
 ]
 
-__version__ = '0.15.0'
+__version__ = '1.0.1'
 __authors__ = ['Nekidev <neki@nekidev.com>']
 __license__ = "MIT License"
```

### Comparing `anime-api-1.0.0/anime_api/apis/__init__.py` & `anime_api-1.0.1/anime_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/__init__.py` & `anime_api-1.0.1/anime_api/apis/anime_facts_rest_api/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/objects.py` & `anime_api-1.0.1/anime_api/apis/anime_facts_rest_api/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/animechan/__init__.py` & `anime_api-1.0.1/anime_api/apis/animechan/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/animu/__init__.py` & `anime_api-1.0.1/anime_api/apis/animu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Base module for the animu API. Documentation for the api can be found at
-https://docs.animu.ml
+https://docs.waifu.it
 """
 import typing
 import requests
 
 from anime_api import exceptions
 from anime_api.apis.animu.objects import (
     Image,
@@ -17,18 +17,18 @@
 )
 from anime_api.apis.animu.types import ImageType
 from anime_api.apis.animu.operators import AND, OR
 
 
 class AnimuAPI:
     """
-    Docs: https://docs.animu.ml
+    Docs: https://docs.waifu.it
     """
 
-    endpoint = "https://animu.ml/api"
+    endpoint = "https://waifu.it/api"
     api_token: str
 
     def __init__(self, api_token: str):
         self.api_token = api_token
 
     def get_random_image(self, category: ImageType) -> Image:
         """
```

### Comparing `anime-api-1.0.0/anime_api/apis/animu/objects.py` & `anime_api-1.0.1/anime_api/apis/animu/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/animu/types.py` & `anime_api-1.0.1/anime_api/apis/animu/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/catboys/__init__.py` & `anime_api-1.0.1/anime_api/apis/catboys/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/catboys/objects.py` & `anime_api-1.0.1/anime_api/apis/catboys/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/hmtai/types.py` & `anime_api-1.0.1/anime_api/apis/hmtai/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/kyoko/__init__.py` & `anime_api-1.0.1/anime_api/apis/kyoko/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/neko_love/__init__.py` & `anime_api-1.0.1/anime_api/apis/neko_love/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/neko_love/types.py` & `anime_api-1.0.1/anime_api/apis/neko_love/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekobot/__init__.py` & `anime_api-1.0.1/anime_api/apis/nekobot/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekobot/types.py` & `anime_api-1.0.1/anime_api/apis/nekobot/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_api/__init__.py` & `anime_api-1.0.1/anime_api/apis/nekos_api/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_api/objects.py` & `anime_api-1.0.1/anime_api/apis/nekos_api/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_api/utils.py` & `anime_api-1.0.1/anime_api/apis/nekos_api/utils.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_best/__init__.py` & `anime_api-1.0.1/anime_api/apis/nekos_best/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_best/objects.py` & `anime_api-1.0.1/anime_api/apis/nekos_best/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_best/types.py` & `anime_api-1.0.1/anime_api/apis/nekos_best/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_life/__init__.py` & `anime_api-1.0.1/anime_api/apis/nekos_life/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_life/types.py` & `anime_api-1.0.1/anime_api/apis/nekos_life/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_moe/__init__.py` & `anime_api-1.0.1/anime_api/apis/nekos_moe/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/nekos_moe/objects.py` & `anime_api-1.0.1/anime_api/apis/nekos_moe/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/studio_ghibli_api/__init__.py` & `anime_api-1.0.1/anime_api/apis/studio_ghibli_api/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/studio_ghibli_api/objects.py` & `anime_api-1.0.1/anime_api/apis/studio_ghibli_api/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/trace_moe/__init__.py` & `anime_api-1.0.1/anime_api/apis/trace_moe/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/trace_moe/objects.py` & `anime_api-1.0.1/anime_api/apis/trace_moe/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/waifu_im/__init__.py` & `anime_api-1.0.1/anime_api/apis/waifu_im/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/waifu_im/objects.py` & `anime_api-1.0.1/anime_api/apis/waifu_im/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/waifu_im/types.py` & `anime_api-1.0.1/anime_api/apis/waifu_im/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/waifu_pics/__init__.py` & `anime_api-1.0.1/anime_api/apis/waifu_pics/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/apis/waifu_pics/types.py` & `anime_api-1.0.1/anime_api/apis/waifu_pics/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/anime_api/exceptions.py` & `anime_api-1.0.1/anime_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/LICENSE.md` & `anime_api-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `anime-api-1.0.0/README.md` & `anime_api-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,19 +44,19 @@
 | Jikan (MyAnimeList)         | [Documentation](https://jikan.docs.apiary.io/)                                      | ❌        |
 | Waifu Pics                  | [Documentation](https://waifu.pics/docs)                                            | ✅        |
 | Studio Ghibli API           | [Documentation](https://ghibliapi.herokuapp.com/)                                   | ✅        |
 | Kitsu                       | [Documentation](https://kitsu.docs.apiary.io/)                                      | ❌        |
 | AniList                     | [Documentation](https://anilist.gitbook.io/anilist-apiv2-docs/)                     | ❌        |
 | AniDB                       | [Documentation](https://wiki.anidb.net/w/API)                                       | ❌        |
 | Kyoko                       | [Documentation](https://github.com/Elliottophellia/kyoko)                           | ✅        |
-| Animu                       | [Documentation](https://docs.animu.ml/)                                             | ✅ (down) |
+| Animu                       | [Documentation](https://docs.waifu.it/)                                             | ✅        |
 | Anisearch                   | [Documentation](https://anisearch.com/developers)                                   | ❌        |
 | Anime News Network          | [Documentation](https://www.animenewsnetwork.com/encyclopedia/api.php)              | ❌        |
 | Notify.moe (Anime Notifier) | [Documentation](https://notify.moe/api)                                             | ❌        |
-| Hmtai                       | [Documentation](https://hmtai.herokuapp.com/endpoints)                              | ✅ (down) |
+| Hmtai                       | [Documentation](https://hmtai.herokuapp.com/endpoints)                              | ✅        |
 | Nekos.life                  | [Documentation](https://github.com/Nekos-life/nekos.py)                             | ✅        |
 | NekoBot                     | [Documentation](https://docs.nekobot.xyz/)                                          | ✅        |
 | Neko-Love                   | [Documentation](https://docs.neko-love.xyz/)                                        | ✅        |
 | Nekos.best                  | [Documentation](https://docs.nekos.best/)                                           | ✅        |
 | Nekos.moe                   | [Documentation](https://docs.nekos.moe/)                                            | ✅        |
 | Shikimori                   | [Documentation](https://shikimori.one/api/doc)                                      | ❌        |
 | MangaDex                    | [Documentation](https://api.mangadex.org/docs.html)                                 | ❌        |
```

### Comparing `anime-api-1.0.0/setup.py` & `anime_api-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,286 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: anime-api
+Version: 1.0.1
+Summary: A collection of wrappers for anime-related APIs
+Author: Neki
+Author-email: 84998222+Nekidev@users.noreply.github.com
+Requires-Python: >=3.7,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pykakasi (>=2.2.1,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['anime_api',
- 'anime_api.apis',
- 'anime_api.apis.anime_facts_rest_api',
- 'anime_api.apis.animechan',
- 'anime_api.apis.animu',
- 'anime_api.apis.catboys',
- 'anime_api.apis.hmtai',
- 'anime_api.apis.kyoko',
- 'anime_api.apis.neko_love',
- 'anime_api.apis.nekobot',
- 'anime_api.apis.nekos_api',
- 'anime_api.apis.nekos_best',
- 'anime_api.apis.nekos_life',
- 'anime_api.apis.nekos_moe',
- 'anime_api.apis.studio_ghibli_api',
- 'anime_api.apis.trace_moe',
- 'anime_api.apis.waifu_im',
- 'anime_api.apis.waifu_pics']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pykakasi>=2.2.1,<3.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'anime-api',
-    'version': '1.0.0',
-    'description': 'A collection of wrappers for anime-related APIs',
-    'long_description': '# The Anime API Project\n\n![Loli count](https://count.getloli.com/get/@anime-api?theme=gelbooru)\n\nThe Anime API is a collection of wrappers for different types of free anime-related APIs. [Join our Discord server](https://discord.gg/PgQnuM3YnM).\n\n## Why anime-api (and not others)?\n\nThere are several reasons why would you prefer using anime-api:\n\n-   **Intuitive**: anime-api is designed to be intuitive. Supports autocompletion everywhere.\n-   **Complete**: Every actively supported API has no feature left apart.\n-   **Simple**: Get all the anime information you want with a single line of code.\n-   **Legal**: I shouldn\'t need to say this, but all the APIs are legal. (no free streaming services/others)\n-   **Actively supported**: Get new releases (with new API wrappers) every now and then.\n\n## Installation\n\nUsing Poetry:\n\n```\npoetry add anime-api\n```\n\nUsing pip:\n\n```\npip install anime-api\n```\n\n## Documentation\n\nThe full documentation can be found [here](docs/).\n\n## APIs\n\nThese are the currently supported and planned to add support for APIs:\n\n| Name                        | API Documentation                                                                   | Available |\n| --------------------------- | ----------------------------------------------------------------------------------- | --------- |\n| Anime Facts Rest API        | [Documentation](https://chandan-02.github.io/anime-facts-rest-api/)                 | ✅        |\n| Trace.moe                   | [Documentation](https://soruly.github.io/trace.moe-api/)                            | ✅        |\n| Animechan                   | [Documentation](https://animechan.vercel.app/docs)                                  | ✅        |\n| Jikan (MyAnimeList)         | [Documentation](https://jikan.docs.apiary.io/)                                      | ❌        |\n| Waifu Pics                  | [Documentation](https://waifu.pics/docs)                                            | ✅        |\n| Studio Ghibli API           | [Documentation](https://ghibliapi.herokuapp.com/)                                   | ✅        |\n| Kitsu                       | [Documentation](https://kitsu.docs.apiary.io/)                                      | ❌        |\n| AniList                     | [Documentation](https://anilist.gitbook.io/anilist-apiv2-docs/)                     | ❌        |\n| AniDB                       | [Documentation](https://wiki.anidb.net/w/API)                                       | ❌        |\n| Kyoko                       | [Documentation](https://github.com/Elliottophellia/kyoko)                           | ✅        |\n| Animu                       | [Documentation](https://docs.animu.ml/)                                             | ✅ (down) |\n| Anisearch                   | [Documentation](https://anisearch.com/developers)                                   | ❌        |\n| Anime News Network          | [Documentation](https://www.animenewsnetwork.com/encyclopedia/api.php)              | ❌        |\n| Notify.moe (Anime Notifier) | [Documentation](https://notify.moe/api)                                             | ❌        |\n| Hmtai                       | [Documentation](https://hmtai.herokuapp.com/endpoints)                              | ✅ (down) |\n| Nekos.life                  | [Documentation](https://github.com/Nekos-life/nekos.py)                             | ✅        |\n| NekoBot                     | [Documentation](https://docs.nekobot.xyz/)                                          | ✅        |\n| Neko-Love                   | [Documentation](https://docs.neko-love.xyz/)                                        | ✅        |\n| Nekos.best                  | [Documentation](https://docs.nekos.best/)                                           | ✅        |\n| Nekos.moe                   | [Documentation](https://docs.nekos.moe/)                                            | ✅        |\n| Shikimori                   | [Documentation](https://shikimori.one/api/doc)                                      | ❌        |\n| MangaDex                    | [Documentation](https://api.mangadex.org/docs.html)                                 | ❌        |\n| Danbooru                    | [Documentation](https://danbooru.donmai.us/wiki_pages/help:api)                     | ❌        |\n| Yandere                     | [Documentation](https://yande.re/help/api)                                          | ❌        |\n| Konachan                    | [Documentation](https://konachan.com/help/api)                                      | ❌        |\n| Waifu.im                    | [Documentation](https://waifu.im/)                                                  | ✅        |\n| Catboys                     | [Documentation](https://catboys.com/api)                                            | ✅        |\n| Anime Character Database    | [Documentation](http://wiki.animecharactersdatabase.com/index.php?title=API_Access) | ❌        |\n| Nekos API                   | [Documentation](https://v1.nekosapi.com/docs/rest-api/endpoints)                    | ✅        |\n\n### APIs by feature\n\nYou know what you want to do, but have no idea of what API will work for you? This list orders the APIs by features. See which fits you best!\n\n#### Images\n\n-   Nekos API:\n    -   Thousands of anime images\n    -   Lots of image metadata\n    -   Actively developed (frequent new features, images, categories, and more)\n    -   100% open-source\n    -   `v2.0.0` in its way\n    -   Official Python wrapper (this!)\n    -   Completely free\n-   Animu:\n    -   Tons of anime gifs and images\n    -   Get reaction gifs from +60 different categories\n    -   Completely free\n-   Hmtai:\n    -   Tons of anime gifs and images\n    -   SFW and NSFW images\n    -   Get random images from +70 different categories\n    -   Completely free\n-   Nekos.life\n    -   Lots of different neko pics\n    -   Get random neko images from +20 different categories\n    -   Completely free\n-   Waifu.pics\n    -   Lots of different waifu images\n    -   Get random images from +30 categories\n    -   SFW and NSFW images\n    -   Get 30 different images with a single API call\n    -   Get a different image every time\n    -   Completely free\n-   NekoBot\n    -   Lots of different neko images\n    -   Image generation (memes, ships, etc.)\n    -   Get random images from 30 different categories\n    -   SFW and NSFW images\n    -   Completely free\n-   Nekos.moe\n    -   Lots of different neko images\n    -   Advanced image search\n    -   Upload images\n    -   Like and favorite images\n    -   SFW and NSFW images\n    -   Get any amount of random images\n    -   Completely free\n-   Nekos.best\n    -   Lots of different neko images\n    -   Get random images from +35 different categories\n    -   Get many random images with a single API call\n    -   Search for images by category, format and more\n    -   Fully SFW\n    -   99.9% uptime\n    -   Fast response times\n    -   Get all image\'s source\n    -   Completely free\n\n#### Facts\n\n-   Anime Facts Rest API:\n    -   Lots of different anime facts\n    -   Get random fact from an anime\n    -   Save fact ID and refetch the fact later\n    -   Get a list of all available animes\n    -   Completely free\n-   Animu:\n    -   Lots of anime facts\n    -   Get random anime facts\n    -   Completely free\n-   Kyoko:\n    -   Lots of different anime facts\n    -   Get random reaction gifs from 3 different categories\n    -   Completely free\n-   Nekos.life\n    -   Lots of different anime facts\n    -   Get random anime facts\n    -   Completely free\n\n#### Quotes\n\n-   Animechan:\n    -   Lots of different quotes from a large list of characters and animes\n    -   Get random anime quotes\n    -   Get 10 random anime quotes with a single api call\n    -   Search quotes by character name or anime title\n    -   Get a list of all available animes\n    -   Completely free\n-   Animu:\n    -   Lots of different anime quotes with information about who said them and where\n    -   Get random anime quotes\n    -   Completely free.\n-   Kyoko:\n    -   Lots of different anime quotes\n    -   Get random quotes with information about who said them and where\n    -   Completely free\n\n#### Waifus\n\n-   Animu:\n    -   Lots of different waifus from Video Games, Animes, Movies and more.\n    -   Get random waifus with their statistics, source, many images and more.\n    -   Completely free\n\n#### Animes\n\n-   Anime Facts Rest API:\n    -   Get a list of lots of snake-case anime titles with their images and facts about them\n    -   Completely free\n-   Animechan:\n    -   Get a list of lots of anime titles with random quotes from them\n    -   Completely free\n-   Studio Ghibli API\n    -   Get Studio Ghibli animes with information such as director, producer, etc.\n    -   Dynamic loading support\n    -   Get super specific anime details such as veichles, locations, people, and species.\n    -   Completely free\n\n#### Entertainment\n\n-   Nekos.life\n    -   Get an answer from an 8ball with an aditional image of an 8ball showing the answer.\n    -   Get a random "why?" question\n    -   Completely free\n\n#### Utilities\n\n-   Trace.moe\n    -   Find an anime from a screenshot with information about the specific anime, episode and time of the screenshot.\n    -   Completely free\n-   Nekos.life\n    -   Get a random cat text emoji\n    -   Generate random names\n    -   Owoify text (`hello` => `hewwo`)\n    -   Mark text as spoiler (`hello` => `||hello||`) (API endpoint is currently bugged)\n    -   Completely free\n-   Animu:\n    -   Generate a secure password\n    -   Completely free\n\n### APIs that will not be supported\n\n-   Illegal anime streaming services\n-   Non anime-related APIs\n-   APIs that are not APIs (i.e. web scrapping)\n\n## Contributing\n\nRead the following before contributing:\n\n### Adding an API\n\nIf you want to add an API to the list, please make sure that:\n\n-   The API is free to use\n-   The API is anime-related (or manga-related)\n-   You follow the same architecture as the other API wrappers\n-   Document the code you write\n-   Add all the necessary tests to the `tests` folder\n\n### Fixing an API wrapper\n\nBefore fixing an API wrapper, please make sure that:\n\n-   The bug is not being fixed in another PR\n-   The bug is actually a bug and not a feature (xd)\n-   The bug is not a bug from the API itself\n-   You have created an issue. If you have not created an issue, please create one before fixing the bug.\n\n### Requesting a new API\n\nIf you want to request a new API, please make sure that:\n\n-   The API is free to use\n-   The API is anime-related (or manga-related)\n-   It is not already in the list (wether available or not)\n\nOnce you have checked this, please create an issue with the following information:\n\n-   The name of the API\n-   The API docs link\n-   List of all the features the API has\n\n## Mantainers\n\n<table>\n  <tr>\n    <td style="align:center;">\n      <a href="https://github.com/Nekidev">\n        <img src="https://avatars.githubusercontent.com/u/84998222?s=256&v=4" height="100" width="100" alt="Nekidev avatar" />\n        <br>\n        <span>Nekidev</span>\n      </a>\n    </td>\n  </tr>\n</table>\n',
-    'author': 'Neki',
-    'author_email': '84998222+Nekidev@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4',
-}
+# The Anime API Project
 
+![Loli count](https://count.getloli.com/get/@anime-api?theme=gelbooru)
+
+The Anime API is a collection of wrappers for different types of free anime-related APIs. [Join our Discord server](https://discord.gg/PgQnuM3YnM).
+
+## Why anime-api (and not others)?
+
+There are several reasons why would you prefer using anime-api:
+
+-   **Intuitive**: anime-api is designed to be intuitive. Supports autocompletion everywhere.
+-   **Complete**: Every actively supported API has no feature left apart.
+-   **Simple**: Get all the anime information you want with a single line of code.
+-   **Legal**: I shouldn't need to say this, but all the APIs are legal. (no free streaming services/others)
+-   **Actively supported**: Get new releases (with new API wrappers) every now and then.
+
+## Installation
+
+Using Poetry:
+
+```
+poetry add anime-api
+```
+
+Using pip:
+
+```
+pip install anime-api
+```
+
+## Documentation
+
+The full documentation can be found [here](docs/).
+
+## APIs
+
+These are the currently supported and planned to add support for APIs:
+
+| Name                        | API Documentation                                                                   | Available |
+| --------------------------- | ----------------------------------------------------------------------------------- | --------- |
+| Anime Facts Rest API        | [Documentation](https://chandan-02.github.io/anime-facts-rest-api/)                 | ✅        |
+| Trace.moe                   | [Documentation](https://soruly.github.io/trace.moe-api/)                            | ✅        |
+| Animechan                   | [Documentation](https://animechan.vercel.app/docs)                                  | ✅        |
+| Jikan (MyAnimeList)         | [Documentation](https://jikan.docs.apiary.io/)                                      | ❌        |
+| Waifu Pics                  | [Documentation](https://waifu.pics/docs)                                            | ✅        |
+| Studio Ghibli API           | [Documentation](https://ghibliapi.herokuapp.com/)                                   | ✅        |
+| Kitsu                       | [Documentation](https://kitsu.docs.apiary.io/)                                      | ❌        |
+| AniList                     | [Documentation](https://anilist.gitbook.io/anilist-apiv2-docs/)                     | ❌        |
+| AniDB                       | [Documentation](https://wiki.anidb.net/w/API)                                       | ❌        |
+| Kyoko                       | [Documentation](https://github.com/Elliottophellia/kyoko)                           | ✅        |
+| Animu                       | [Documentation](https://docs.waifu.it/)                                             | ✅        |
+| Anisearch                   | [Documentation](https://anisearch.com/developers)                                   | ❌        |
+| Anime News Network          | [Documentation](https://www.animenewsnetwork.com/encyclopedia/api.php)              | ❌        |
+| Notify.moe (Anime Notifier) | [Documentation](https://notify.moe/api)                                             | ❌        |
+| Hmtai                       | [Documentation](https://hmtai.herokuapp.com/endpoints)                              | ✅        |
+| Nekos.life                  | [Documentation](https://github.com/Nekos-life/nekos.py)                             | ✅        |
+| NekoBot                     | [Documentation](https://docs.nekobot.xyz/)                                          | ✅        |
+| Neko-Love                   | [Documentation](https://docs.neko-love.xyz/)                                        | ✅        |
+| Nekos.best                  | [Documentation](https://docs.nekos.best/)                                           | ✅        |
+| Nekos.moe                   | [Documentation](https://docs.nekos.moe/)                                            | ✅        |
+| Shikimori                   | [Documentation](https://shikimori.one/api/doc)                                      | ❌        |
+| MangaDex                    | [Documentation](https://api.mangadex.org/docs.html)                                 | ❌        |
+| Danbooru                    | [Documentation](https://danbooru.donmai.us/wiki_pages/help:api)                     | ❌        |
+| Yandere                     | [Documentation](https://yande.re/help/api)                                          | ❌        |
+| Konachan                    | [Documentation](https://konachan.com/help/api)                                      | ❌        |
+| Waifu.im                    | [Documentation](https://waifu.im/)                                                  | ✅        |
+| Catboys                     | [Documentation](https://catboys.com/api)                                            | ✅        |
+| Anime Character Database    | [Documentation](http://wiki.animecharactersdatabase.com/index.php?title=API_Access) | ❌        |
+| Nekos API                   | [Documentation](https://v1.nekosapi.com/docs/rest-api/endpoints)                    | ✅        |
+
+### APIs by feature
+
+You know what you want to do, but have no idea of what API will work for you? This list orders the APIs by features. See which fits you best!
+
+#### Images
+
+-   Nekos API:
+    -   Thousands of anime images
+    -   Lots of image metadata
+    -   Actively developed (frequent new features, images, categories, and more)
+    -   100% open-source
+    -   `v2.0.0` in its way
+    -   Official Python wrapper (this!)
+    -   Completely free
+-   Animu:
+    -   Tons of anime gifs and images
+    -   Get reaction gifs from +60 different categories
+    -   Completely free
+-   Hmtai:
+    -   Tons of anime gifs and images
+    -   SFW and NSFW images
+    -   Get random images from +70 different categories
+    -   Completely free
+-   Nekos.life
+    -   Lots of different neko pics
+    -   Get random neko images from +20 different categories
+    -   Completely free
+-   Waifu.pics
+    -   Lots of different waifu images
+    -   Get random images from +30 categories
+    -   SFW and NSFW images
+    -   Get 30 different images with a single API call
+    -   Get a different image every time
+    -   Completely free
+-   NekoBot
+    -   Lots of different neko images
+    -   Image generation (memes, ships, etc.)
+    -   Get random images from 30 different categories
+    -   SFW and NSFW images
+    -   Completely free
+-   Nekos.moe
+    -   Lots of different neko images
+    -   Advanced image search
+    -   Upload images
+    -   Like and favorite images
+    -   SFW and NSFW images
+    -   Get any amount of random images
+    -   Completely free
+-   Nekos.best
+    -   Lots of different neko images
+    -   Get random images from +35 different categories
+    -   Get many random images with a single API call
+    -   Search for images by category, format and more
+    -   Fully SFW
+    -   99.9% uptime
+    -   Fast response times
+    -   Get all image's source
+    -   Completely free
+
+#### Facts
+
+-   Anime Facts Rest API:
+    -   Lots of different anime facts
+    -   Get random fact from an anime
+    -   Save fact ID and refetch the fact later
+    -   Get a list of all available animes
+    -   Completely free
+-   Animu:
+    -   Lots of anime facts
+    -   Get random anime facts
+    -   Completely free
+-   Kyoko:
+    -   Lots of different anime facts
+    -   Get random reaction gifs from 3 different categories
+    -   Completely free
+-   Nekos.life
+    -   Lots of different anime facts
+    -   Get random anime facts
+    -   Completely free
+
+#### Quotes
+
+-   Animechan:
+    -   Lots of different quotes from a large list of characters and animes
+    -   Get random anime quotes
+    -   Get 10 random anime quotes with a single api call
+    -   Search quotes by character name or anime title
+    -   Get a list of all available animes
+    -   Completely free
+-   Animu:
+    -   Lots of different anime quotes with information about who said them and where
+    -   Get random anime quotes
+    -   Completely free.
+-   Kyoko:
+    -   Lots of different anime quotes
+    -   Get random quotes with information about who said them and where
+    -   Completely free
+
+#### Waifus
+
+-   Animu:
+    -   Lots of different waifus from Video Games, Animes, Movies and more.
+    -   Get random waifus with their statistics, source, many images and more.
+    -   Completely free
+
+#### Animes
+
+-   Anime Facts Rest API:
+    -   Get a list of lots of snake-case anime titles with their images and facts about them
+    -   Completely free
+-   Animechan:
+    -   Get a list of lots of anime titles with random quotes from them
+    -   Completely free
+-   Studio Ghibli API
+    -   Get Studio Ghibli animes with information such as director, producer, etc.
+    -   Dynamic loading support
+    -   Get super specific anime details such as veichles, locations, people, and species.
+    -   Completely free
+
+#### Entertainment
+
+-   Nekos.life
+    -   Get an answer from an 8ball with an aditional image of an 8ball showing the answer.
+    -   Get a random "why?" question
+    -   Completely free
+
+#### Utilities
+
+-   Trace.moe
+    -   Find an anime from a screenshot with information about the specific anime, episode and time of the screenshot.
+    -   Completely free
+-   Nekos.life
+    -   Get a random cat text emoji
+    -   Generate random names
+    -   Owoify text (`hello` => `hewwo`)
+    -   Mark text as spoiler (`hello` => `||hello||`) (API endpoint is currently bugged)
+    -   Completely free
+-   Animu:
+    -   Generate a secure password
+    -   Completely free
+
+### APIs that will not be supported
+
+-   Illegal anime streaming services
+-   Non anime-related APIs
+-   APIs that are not APIs (i.e. web scrapping)
+
+## Contributing
+
+Read the following before contributing:
+
+### Adding an API
+
+If you want to add an API to the list, please make sure that:
+
+-   The API is free to use
+-   The API is anime-related (or manga-related)
+-   You follow the same architecture as the other API wrappers
+-   Document the code you write
+-   Add all the necessary tests to the `tests` folder
+
+### Fixing an API wrapper
+
+Before fixing an API wrapper, please make sure that:
+
+-   The bug is not being fixed in another PR
+-   The bug is actually a bug and not a feature (xd)
+-   The bug is not a bug from the API itself
+-   You have created an issue. If you have not created an issue, please create one before fixing the bug.
+
+### Requesting a new API
+
+If you want to request a new API, please make sure that:
+
+-   The API is free to use
+-   The API is anime-related (or manga-related)
+-   It is not already in the list (wether available or not)
+
+Once you have checked this, please create an issue with the following information:
+
+-   The name of the API
+-   The API docs link
+-   List of all the features the API has
+
+## Mantainers
+
+<table>
+  <tr>
+    <td style="align:center;">
+      <a href="https://github.com/Nekidev">
+        <img src="https://avatars.githubusercontent.com/u/84998222?s=256&v=4" height="100" width="100" alt="Nekidev avatar" />
+        <br>
+        <span>Nekidev</span>
+      </a>
+    </td>
+  </tr>
+</table>
 
-setup(**setup_kwargs)
```

