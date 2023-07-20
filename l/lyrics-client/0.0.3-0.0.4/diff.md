# Comparing `tmp/lyrics_client-0.0.3.tar.gz` & `tmp/lyrics_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_client-0.0.3.tar", max compression
+gzip compressed data, was "lyrics_client-0.0.4.tar", max compression
```

## Comparing `lyrics_client-0.0.3.tar` & `lyrics_client-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/LICENSE
--rw-r--r--   0        0        0     2093 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/README.md
--rw-r--r--   0        0        0      440 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/__init__.py
--rw-r--r--   0        0        0      159 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/__init__.py
--rw-r--r--   0        0        0      355 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/__init__.py
--rw-r--r--   0        0        0     3975 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/abstract_lyrics_client.py
--rw-r--r--   0        0        0     2723 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/azlyrics_lyrics_client.py
--rw-r--r--   0        0        0     2575 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/genius_lyrics_client.py
--rw-r--r--   0        0        0     2165 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/clients/musixmatch_lyrics_client.py
--rw-r--r--   0        0        0      245 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/fetch_lyrics_command.py
--rw-r--r--   0        0        0      257 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/classes/fetch_lyrics_result.py
--rw-r--r--   0        0        0       83 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/di/__init__.py
--rw-r--r--   0        0        0      513 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/di/dependency_injector.py
--rw-r--r--   0        0        0      211 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/bad_format_error.py
--rw-r--r--   0        0        0       79 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/bad_title_match_error.py
--rw-r--r--   0        0        0       69 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/errors/no_result_error.py
--rw-r--r--   0        0        0       81 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/interfaces/__init__.py
--rw-r--r--   0        0        0      240 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/interfaces/base_lyrics_client.py
--rw-r--r--   0        0        0      978 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/main.py
--rw-r--r--   0        0        0        0 2023-06-22 20:30:21.088970 lyrics_client-0.0.3/lyrics_client/py.typed
--rw-r--r--   0        0        0     1340 2023-06-22 20:30:21.092970 lyrics_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 lyrics_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2093 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/README.md
+-rw-r--r--   0        0        0      440 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/clients/__init__.py
+-rw-r--r--   0        0        0     4003 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/clients/abstract_lyrics_client.py
+-rw-r--r--   0        0        0     2723 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/clients/azlyrics_lyrics_client.py
+-rw-r--r--   0        0        0     2575 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/clients/genius_lyrics_client.py
+-rw-r--r--   0        0        0     2251 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/clients/musixmatch_lyrics_client.py
+-rw-r--r--   0        0        0      245 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/fetch_lyrics_command.py
+-rw-r--r--   0        0        0      257 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/classes/fetch_lyrics_result.py
+-rw-r--r--   0        0        0       83 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/di/__init__.py
+-rw-r--r--   0        0        0      513 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/di/dependency_injector.py
+-rw-r--r--   0        0        0      211 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/errors/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/errors/bad_format_error.py
+-rw-r--r--   0        0        0       79 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/errors/bad_title_match_error.py
+-rw-r--r--   0        0        0       69 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/errors/no_result_error.py
+-rw-r--r--   0        0        0       81 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/interfaces/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/interfaces/base_lyrics_client.py
+-rw-r--r--   0        0        0      978 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/main.py
+-rw-r--r--   0        0        0        0 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/lyrics_client/py.typed
+-rw-r--r--   0        0        0     1340 2023-07-20 20:11:26.993510 lyrics_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 lyrics_client-0.0.4/PKG-INFO
```

### Comparing `lyrics_client-0.0.3/LICENSE` & `lyrics_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/README.md` & `lyrics_client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/lyrics_client/classes/clients/abstract_lyrics_client.py` & `lyrics_client-0.0.4/lyrics_client/classes/clients/abstract_lyrics_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from lyrics_client.errors import NoResultError, BadTitleMatchError
 
 __all__ = ["AbstractLyricsClient"]
 
 
 class AbstractLyricsClient(BaseLyricsClient, metaclass=abc.ABCMeta):
     def __init__(self) -> None:
+        super().__init__()
+
         self.headers = {
             "Connection": "keep-alive",
             "Pragma": "no-cache",
             "Cache-Control": "no-cache",
             "sec-ch-ua": '"Chromium";v="104", " Not A;Brand";v="99", "Google Chrome";v="104"',
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
             "(KHTML, like Gecko) Chrome/104.0.0.0 Safari/537.36",
```

### Comparing `lyrics_client-0.0.3/lyrics_client/classes/clients/azlyrics_lyrics_client.py` & `lyrics_client-0.0.4/lyrics_client/classes/clients/azlyrics_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/lyrics_client/classes/clients/genius_lyrics_client.py` & `lyrics_client-0.0.4/lyrics_client/classes/clients/genius_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/lyrics_client/classes/clients/musixmatch_lyrics_client.py` & `lyrics_client-0.0.4/lyrics_client/classes/clients/musixmatch_lyrics_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         
         results: Dict[str, str] = {}
 
         for card in song_cards:
             title_tag = card.select_one("a.title[href^='/lyrics/']")
             artist_tag = card.select_one("a.artist")
             
+            if not title_tag or not artist_tag:
+                continue
+            
             title = title_tag.get_text()
             artist = artist_tag.get_text()
             url = str(title_tag.get('href', ''))
             
             results[f"{title} - {artist}"] = f"{self.MUSIXMATCH_URL}{url}"
 
         return results
```

### Comparing `lyrics_client-0.0.3/lyrics_client/di/dependency_injector.py` & `lyrics_client-0.0.4/lyrics_client/di/dependency_injector.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/lyrics_client/main.py` & `lyrics_client-0.0.4/lyrics_client/main.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.3/pyproject.toml` & `lyrics_client-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-client"
-version = "0.0.3"
+version = "0.0.4"
 description = "A generic client to fetch lyrics from a song's data"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["lyrics client", "lyrics", "python", "genius", "azlyrics, musixmatch"]
```

### Comparing `lyrics_client-0.0.3/PKG-INFO` & `lyrics_client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A generic client to fetch lyrics from a song's data
 Home-page: https://github.com/Billuc/lyrics-client
 License: MIT
 Keywords: lyrics client,lyrics,python,genius,azlyrics, musixmatch
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
```

