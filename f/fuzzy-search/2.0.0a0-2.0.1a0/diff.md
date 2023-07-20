# Comparing `tmp/fuzzy_search-2.0.0a0.tar.gz` & `tmp/fuzzy_search-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy_search-2.0.0a0.tar", last modified: Thu May 11 15:37:27 2023, max compression
+gzip compressed data, was "fuzzy_search-2.0.1a0.tar", last modified: Thu Jul 20 13:23:33 2023, max compression
```

## Comparing `fuzzy_search-2.0.0a0.tar` & `fuzzy_search-2.0.1a0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.237927 fuzzy_search-2.0.0a0/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1085 2020-12-08 10:17:28.000000 fuzzy_search-2.0.0a0/LICENSE
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-05-11 15:37:27.237813 fuzzy_search-2.0.0a0/PKG-INFO
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6746 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/README.md
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233013 fuzzy_search-2.0.0a0/fuzzy_search/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      513 2023-05-11 15:37:16.000000 fuzzy_search-2.0.0a0/fuzzy_search/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     8716 2019-10-29 21:19:08.000000 fuzzy_search-2.0.0a0/fuzzy_search/fuzzy_searcher.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233911 fuzzy_search-2.0.0a0/fuzzy_search/match/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:43:19.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    12788 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/candidate_match.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    10376 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/exact_match.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    31262 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/phrase_match.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    12964 2023-04-20 11:54:21.000000 fuzzy_search-2.0.0a0/fuzzy_search/match/skip_match.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.234196 fuzzy_search-2.0.0a0/fuzzy_search/pattern/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:17:29.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7716 2020-12-07 10:17:03.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_patterns.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    18032 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_template.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.234482 fuzzy_search-2.0.0a0/fuzzy_search/phrase/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:12:13.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9868 2023-04-24 06:58:56.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    33515 2023-04-21 11:38:57.000000 fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase_model.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.235429 fuzzy_search-2.0.0a0/fuzzy_search/search/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:16:54.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1179 2023-04-20 07:57:23.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/config.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6847 2023-04-19 10:36:26.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/context_searcher.py
--rw-rw-rw-   0 marijnkoolen   (501) staff       (20)    14654 2023-04-20 08:18:19.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/phrase_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    17372 2023-04-20 08:51:05.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    32894 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/template_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    25410 2023-04-24 10:58:42.000000 fuzzy_search-2.0.0a0/fuzzy_search/search/token_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9609 2023-04-18 13:00:52.000000 fuzzy_search-2.0.0a0/fuzzy_search/similarity.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.235792 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:18:47.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     8088 2023-02-02 18:33:08.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/string.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     5488 2023-04-18 12:51:10.000000 fuzzy_search-2.0.0a0/fuzzy_search/tokenization/token.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.233411 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-05-11 15:37:26.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/PKG-INFO
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1420 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/SOURCES.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        1 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/dependency_links.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)       18 2023-05-11 15:37:27.000000 fuzzy_search-2.0.0a0/fuzzy_search.egg-info/top_level.txt
--rw-r--r--   0 marijnkoolen   (501) staff       (20)       38 2023-05-11 15:37:27.237962 fuzzy_search-2.0.0a0/setup.cfg
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3983 2023-02-02 18:40:00.000000 fuzzy_search-2.0.0a0/setup.py
-drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-05-11 15:37:27.237653 fuzzy_search-2.0.0a0/test/
--rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2020-10-14 12:59:55.000000 fuzzy_search-2.0.0a0/test/__init__.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      945 2023-04-20 07:55:27.000000 fuzzy_search-2.0.0a0/test/test_match_candidate.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9352 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_match_phrase.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)      496 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_match_skip.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     6200 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_pattern_template.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     4153 2023-04-21 16:20:10.000000 fuzzy_search-2.0.0a0/test/test_phrase_phrase.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     4322 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_phrase_phrase_model.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1934 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_search_context_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)    16858 2023-04-20 07:55:28.000000 fuzzy_search-2.0.0a0/test/test_search_phrase_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     1680 2023-04-20 08:20:37.000000 fuzzy_search-2.0.0a0/test/test_search_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     5728 2023-04-20 07:55:27.000000 fuzzy_search-2.0.0a0/test/test_search_template_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     9306 2023-04-24 07:16:40.000000 fuzzy_search-2.0.0a0/test/test_search_token_searcher.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3255 2023-04-18 13:00:52.000000 fuzzy_search-2.0.0a0/test/test_tokenization_string.py
--rw-r--r--   0 marijnkoolen   (501) staff       (20)     3313 2023-04-18 12:39:41.000000 fuzzy_search-2.0.0a0/test/test_tokenization_token.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.874318 fuzzy_search-2.0.1a0/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1085 2020-12-08 10:17:28.000000 fuzzy_search-2.0.1a0/LICENSE
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-07-20 13:23:33.874206 fuzzy_search-2.0.1a0/PKG-INFO
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6746 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/README.md
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.869310 fuzzy_search-2.0.1a0/fuzzy_search/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      513 2023-07-20 13:22:19.000000 fuzzy_search-2.0.1a0/fuzzy_search/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     8716 2019-10-29 21:19:08.000000 fuzzy_search-2.0.1a0/fuzzy_search/fuzzy_searcher.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.870542 fuzzy_search-2.0.1a0/fuzzy_search/match/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:43:19.000000 fuzzy_search-2.0.1a0/fuzzy_search/match/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    12788 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/fuzzy_search/match/candidate_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    10562 2023-05-26 13:36:51.000000 fuzzy_search-2.0.1a0/fuzzy_search/match/exact_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    31262 2023-06-21 22:26:38.000000 fuzzy_search-2.0.1a0/fuzzy_search/match/phrase_match.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    12964 2023-04-20 11:54:21.000000 fuzzy_search-2.0.1a0/fuzzy_search/match/skip_match.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.871017 fuzzy_search-2.0.1a0/fuzzy_search/pattern/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:17:29.000000 fuzzy_search-2.0.1a0/fuzzy_search/pattern/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7716 2020-12-07 10:17:03.000000 fuzzy_search-2.0.1a0/fuzzy_search/pattern/fuzzy_patterns.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    18032 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/fuzzy_search/pattern/fuzzy_template.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.871354 fuzzy_search-2.0.1a0/fuzzy_search/phrase/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:12:13.000000 fuzzy_search-2.0.1a0/fuzzy_search/phrase/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9868 2023-04-24 06:58:56.000000 fuzzy_search-2.0.1a0/fuzzy_search/phrase/phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    33515 2023-04-21 11:38:57.000000 fuzzy_search-2.0.1a0/fuzzy_search/phrase/phrase_model.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.872192 fuzzy_search-2.0.1a0/fuzzy_search/search/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:16:54.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1179 2023-04-20 07:57:23.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/config.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6847 2023-04-19 10:36:26.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/context_searcher.py
+-rw-rw-rw-   0 marijnkoolen   (501) staff       (20)    14715 2023-06-23 10:42:48.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/phrase_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    17374 2023-06-25 13:53:34.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    32894 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/template_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    25410 2023-04-24 10:58:42.000000 fuzzy_search-2.0.1a0/fuzzy_search/search/token_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9609 2023-04-18 13:00:52.000000 fuzzy_search-2.0.1a0/fuzzy_search/similarity.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.872520 fuzzy_search-2.0.1a0/fuzzy_search/tokenization/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2023-04-18 08:18:47.000000 fuzzy_search-2.0.1a0/fuzzy_search/tokenization/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     8088 2023-02-02 18:33:08.000000 fuzzy_search-2.0.1a0/fuzzy_search/tokenization/string.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7188 2023-07-12 11:26:41.000000 fuzzy_search-2.0.1a0/fuzzy_search/tokenization/token.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.869723 fuzzy_search-2.0.1a0/fuzzy_search.egg-info/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     7666 2023-07-20 13:23:33.000000 fuzzy_search-2.0.1a0/fuzzy_search.egg-info/PKG-INFO
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1420 2023-07-20 13:23:33.000000 fuzzy_search-2.0.1a0/fuzzy_search.egg-info/SOURCES.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        1 2023-07-20 13:23:33.000000 fuzzy_search-2.0.1a0/fuzzy_search.egg-info/dependency_links.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)       18 2023-07-20 13:23:33.000000 fuzzy_search-2.0.1a0/fuzzy_search.egg-info/top_level.txt
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)       38 2023-07-20 13:23:33.874353 fuzzy_search-2.0.1a0/setup.cfg
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3983 2023-02-02 18:40:00.000000 fuzzy_search-2.0.1a0/setup.py
+drwxr-xr-x   0 marijnkoolen   (501) staff       (20)        0 2023-07-20 13:23:33.874038 fuzzy_search-2.0.1a0/test/
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)        0 2020-10-14 12:59:55.000000 fuzzy_search-2.0.1a0/test/__init__.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      945 2023-04-20 07:55:27.000000 fuzzy_search-2.0.1a0/test/test_match_candidate.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9352 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_match_phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)      496 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_match_skip.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     6200 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_pattern_template.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     4153 2023-04-21 16:20:10.000000 fuzzy_search-2.0.1a0/test/test_phrase_phrase.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     4322 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_phrase_phrase_model.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1934 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_search_context_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)    16858 2023-04-20 07:55:28.000000 fuzzy_search-2.0.1a0/test/test_search_phrase_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     1680 2023-04-20 08:20:37.000000 fuzzy_search-2.0.1a0/test/test_search_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     5728 2023-04-20 07:55:27.000000 fuzzy_search-2.0.1a0/test/test_search_template_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     9306 2023-04-24 07:16:40.000000 fuzzy_search-2.0.1a0/test/test_search_token_searcher.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3255 2023-04-18 13:00:52.000000 fuzzy_search-2.0.1a0/test/test_tokenization_string.py
+-rw-r--r--   0 marijnkoolen   (501) staff       (20)     3313 2023-04-18 12:39:41.000000 fuzzy_search-2.0.1a0/test/test_tokenization_token.py
```

### Comparing `fuzzy_search-2.0.0a0/LICENSE` & `fuzzy_search-2.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/PKG-INFO` & `fuzzy_search-2.0.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy_search
-Version: 2.0.0a0
+Version: 2.0.1a0
 Summary: Tool for fuzzy searching in texts with historical language use and OCR/HTR errors
 Home-page: https://github.com/marijnkoolen/fuzzy-search
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 License: MIT
 Keywords: information extraction,historical research,digital resources
 Platform: UNKNOWN
```

### Comparing `fuzzy_search-2.0.0a0/README.md` & `fuzzy_search-2.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/__init__.py` & `fuzzy_search-2.0.1a0/fuzzy_search/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.0a'
+__version__ = '2.0.1a'
 
 from fuzzy_search.search.config import default_config
 from fuzzy_search.search.phrase_searcher import FuzzyPhraseSearcher
 from fuzzy_search.search.token_searcher import FuzzyTokenSearcher
 from fuzzy_search.match.phrase_match import PhraseMatch
 from fuzzy_search.phrase.phrase_model import PhraseModel
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/fuzzy_searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/fuzzy_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/match/candidate_match.py` & `fuzzy_search-2.0.1a0/fuzzy_search/match/candidate_match.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/match/exact_match.py` & `fuzzy_search-2.0.1a0/fuzzy_search/match/exact_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,32 +76,37 @@
                 print('\tsearch_exact_phrases_with_word_boundaries - text start, end:',
                       text["text"][phrase_start:phrase_end])
                 print('\tsearch_exact_phrases_with_word_boundaries - same?:',
                       text["text"][phrase_start:phrase_end] == phrase_string)
 
             if text["text"][phrase_start:phrase_end] == phrase_string:
                 if phrase_start > 0 and re.match(r'\w', text["text"][phrase_start - 1]):
-                    print('\tsearch_exact_phrases_with_word_boundaries - match word is not at start word boundary')
+                    if debug > 0:
+                        print('\tsearch_exact_phrases_with_word_boundaries - match word is not at start word boundary')
                     continue
                 if phrase_end < len(text['text']) - 1 and re.match(r'\w', text['text'][phrase_end]):
-                    print('\tsearch_exact_phrases_with_word_boundaries - match word is not at end word boundary')
+                    if debug > 0:
+                        print('\tsearch_exact_phrases_with_word_boundaries - match word is not at end word boundary')
                     continue
 
-                print('\tsearch_exact_phrases_with_word_boundaries - phrase_string, phrase_type:', phrase_string,
+                if debug > 0:
+                    print('\tsearch_exact_phrases_with_word_boundaries - phrase_string, phrase_type:', phrase_string,
                       phrase_model.phrase_type[phrase_string])
                 if "phrase" in phrase_model.phrase_type[phrase_string]:
-                    print('\tsearch_exact_phrases_with_word_boundaries - match word is phrase')
+                    if debug > 0:
+                        print('\tsearch_exact_phrases_with_word_boundaries - match word is phrase')
                     phrase = phrase_model.phrase_index[phrase_string]
                     match = PhraseMatch(phrase, phrase, phrase_string, phrase_start, text_id=text["id"],
                                         ignorecase=ignorecase)
                     yield add_exact_match_score(match)
                     if debug > 0:
                         print("\tsearch_exact_phrases_with_word_boundaries - the matching phrase:", phrase)
                 elif "variant" in phrase_model.phrase_type[phrase_string] and include_variants:
-                    print('\tsearch_exact_phrases_with_word_boundaries - match word is variant')
+                    if debug > 0:
+                        print('\tsearch_exact_phrases_with_word_boundaries - match word is variant')
                     variant_phrase = phrase_model.variant_index[phrase_string]
                     main_phrase_string = phrase_model.is_variant_of[phrase_string]
                     main_phrase = phrase_model.phrase_index[main_phrase_string]
                     match = PhraseMatch(main_phrase, variant_phrase, phrase_string, phrase_start,
                                         text_id=text["id"], ignorecase=ignorecase)
                     yield add_exact_match_score(match)
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/match/phrase_match.py` & `fuzzy_search-2.0.1a0/fuzzy_search/match/phrase_match.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/match/skip_match.py` & `fuzzy_search-2.0.1a0/fuzzy_search/match/skip_match.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_patterns.py` & `fuzzy_search-2.0.1a0/fuzzy_search/pattern/fuzzy_patterns.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/pattern/fuzzy_template.py` & `fuzzy_search-2.0.1a0/fuzzy_search/pattern/fuzzy_template.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase.py` & `fuzzy_search-2.0.1a0/fuzzy_search/phrase/phrase.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/phrase/phrase_model.py` & `fuzzy_search-2.0.1a0/fuzzy_search/phrase/phrase_model.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/config.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/config.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/context_searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/context_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/phrase_searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/phrase_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         text["id"] = None
     return text
 
 
 class FuzzyPhraseSearcher(FuzzySearcher):
 
     def __init__(self, phrase_list: List[any] = None,
-                 phrase_model: Union[Dict[str, any], PhraseModel] = None,
+                 phrase_model: Union[Dict[str, any], List[Dict[str, any]], PhraseModel] = None,
                  config: Union[None, Dict[str, Union[str, int, float]]] = None,
                  tokenizer: Tokenizer = None,
                  token_searcher: FuzzyTokenSearcher = None):
         """This class represents the basic fuzzy searcher. You can pass a list of phrases or a phrase model and
         configuration dictionary that overrides the default configuration values. The default config dictionary
         is available via `fuzzy_search.default_config`.
 
@@ -227,22 +227,22 @@
         filtered_matches = self.filter_matches_by_threshold(matches)
         if filter_distractors is None:
             filter_distractors = self.filter_distractors
         if filter_distractors:
             filtered_matches = self.filter_matches_by_distractors(filtered_matches)
         if allow_overlapping_matches is None:
             allow_overlapping_matches = self.allow_overlapping_matches
+        filtered_matches = filtered_matches + exact_matches
         if not allow_overlapping_matches:
             filtered_matches = filter_matches_by_overlap(filtered_matches)
         # print(exact_matches)
         if debug > 0:
             time_step()
             print('find_matches - filtered_matches:', filtered_matches)
-        selected_matches = filtered_matches + exact_matches
-        return sorted(selected_matches, key=lambda x: x.offset)
+        return sorted(filtered_matches, key=lambda x: (x.text_id, x.offset, x.offset + len(x.string)))
 
     def find_exact_matches(self, text: Union[str, Dict[str, str]],
                            use_word_boundaries: Union[None, bool] = None,
                            include_variants: Union[None, bool] = None,
                            debug: int = 0) -> List[PhraseMatch]:
         """Find all fuzzy matching phrases for a given text.
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/searcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         known_word = None
         if include_variants is None:
             include_variants = self.include_variants
         if known_word_offset is None:
             known_word_offset = {}
         # print(known_word_offset)
         skip_matches = SkipMatches(self.ngram_size, self.skip_size)
-        text_string = text['text_lower'] if self.ignorecase else text['text']
+        text_string = text['text'].lower() if self.ignorecase else text['text']
         for skipgram in text2skipgrams(text_string, self.ngram_size, self.skip_size):
             # print(skipgram.offset, skipgram.string)
             # print("skipgram:", skipgram.string)
             if skipgram.offset in known_word_offset:
                 known_word = known_word_offset[skipgram.offset]
                 # print("known word offset reached:", known_word)
             if known_word and skipgram.offset == known_word["end"]:
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/template_searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/template_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/search/token_searcher.py` & `fuzzy_search-2.0.1a0/fuzzy_search/search/token_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/similarity.py` & `fuzzy_search-2.0.1a0/fuzzy_search/similarity.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/tokenization/string.py` & `fuzzy_search-2.0.1a0/fuzzy_search/tokenization/string.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search/tokenization/token.py` & `fuzzy_search-2.0.1a0/fuzzy_search/tokenization/token.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 import copy
 import re
 from collections import defaultdict
 from typing import Callable, Dict, List, Set, Union
 
 
+class Annotation:
+
+    def __init__(self, tag_type: str, text: str, offset: int, doc_id: str = None):
+        self.tag_type = tag_type
+        self.text = text
+        self.offset = offset
+        self.end = offset + len(text)
+        self.doc_id = doc_id
+
+
+class Tag:
+
+    def __init__(self, tag_type: str, text: str, offset: int, doc_id: str = None):
+        self.type = tag_type
+        self.text = text
+        self.offset = offset
+        self.tag_string = f"<{tag_type}>{text}</{tag_type}>"
+        self.end = offset + len(self.tag_string)
+        self.doc_id = doc_id
+
+
 class Token:
 
     def __init__(self, string: str, index: int, char_index: int, doc_id: str = None,
                  normalised_string: str = None, label: Union[str, Set[str]] = None,
                  metadata: Dict[str, any] = None):
         self.string = string
         self.index = index
@@ -66,82 +87,102 @@
         self.id = doc_id
         self.tokens = tokens
         self.label_token_index = defaultdict(set)
         for token in tokens:
             for label in token.label:
                 self.label_token_index[label].add(token)
         self.metadata = metadata if metadata else {}
+        self.annotations: List[Annotation] = []
 
     def __repr__(self):
         return f"Doc(id='{self.id}', metadata={self.metadata}, text=\"{self.text}\", tokens={self.tokens}"
 
     def __len__(self):
         return len(self.normalized)
 
     def __getitem__(self, item):
         return self.tokens[item]
 
     def __iter__(self):
         for token in self.tokens:
             yield token
 
+    def add_annotations(self, annotations: List[Annotation]):
+        self.annotations = annotations
+
     @property
     def original(self):
         return [token.t for token in self.tokens]
 
     @property
     def normalized(self):
         return [token.n for token in self.tokens]
 
 
 class Tokenizer:
 
-    def __init__(self, ignorecase: bool = False, include_boundary_tokens: bool = False):
+    def __init__(self, ignorecase: bool = False, include_boundary_tokens: bool = False,
+                 remove_punctuation: bool = False):
         self.ignorecase = ignorecase
         self.include_boundary_tokens = include_boundary_tokens
+        self.remove_punctuation = remove_punctuation
 
     def _tokenize(self, text: str) -> List[str]:
-        return [token for token in text.strip().split() if token != '']
+        non_whitespace_tokens = [token for token in text.strip().split() if token != '']
+        tokens = []
+        for nw_token in non_whitespace_tokens:
+            if self.remove_punctuation:
+                sub_tokens = re.split(r'\W+', nw_token)
+            else:
+                sub_tokens = re.split(r'(\W+)', nw_token)
+            tokens.extend([token for token in sub_tokens if token != ''])
+        return tokens
 
     def tokenize(self, doc_text: str, doc_id: str = None) -> Doc:
-        if self.include_boundary_tokens:
-            doc_text = f"<START> {doc_text} <END>"
+        dummy_text = f"<START> {doc_text} <END>" if self.include_boundary_tokens else doc_text
         token_strings = self._tokenize(doc_text)
-        # if self.include_boundary_tokens:
-        #     tokens = ['<START>'] + token_strings + ['<END>']
+        if self.include_boundary_tokens:
+            token_strings = ['<START>'] + token_strings + ['<END>']
         # tokens = [Token(token, index=ti, doc_id=doc_id) for ti, token in enumerate(tokens)]
         tokens = []
-        dummy_text = doc_text
         prefix_text = ''
         for ti, token_string in enumerate(token_strings):
             # print('tokenize - ti, token_string:', ti, token_string)
             # print('tokenize - prefix_text:', prefix_text)
             char_index = dummy_text.index(token_string) + len(prefix_text)
             # print('tokenize - char_index:', char_index)
             prefix_text += dummy_text[:dummy_text.index(token_string) + len(token_string)]
             dummy_text = dummy_text[dummy_text.index(token_string)+len(token_string):]
             # print('tokenize - dummy_text:', dummy_text)
             token = Token(token_string, index=ti, char_index=char_index, doc_id=doc_id)
             # print('tokenize - token.char_index:', token.char_index)
+            if self.ignorecase:
+                if not self.include_boundary_tokens or (ti != 0 and ti != len(token_strings) - 1):
+                    token.lower()
             tokens.append(token)
-        if self.ignorecase:
-            for t in tokens:
-                t.lower()
         return Doc(text=doc_text, doc_id=doc_id, tokens=tokens)
 
 
 class RegExTokenizer(Tokenizer):
 
     def __init__(self, ignorecase: bool = False, include_boundary_tokens: bool = False,
                  split_pattern: str = r'\b'):
         super().__init__(ignorecase=ignorecase, include_boundary_tokens=include_boundary_tokens)
         self.split_pattern = re.compile(split_pattern)
 
     def _tokenize(self, text: str) -> List[str]:
-        return [token.replace(' ', '') for token in re.split(self.split_pattern, text) if token.replace(' ', '') != '']
+        # print(re.split(self.split_pattern, text))
+        tokens = [token.strip() for token in re.split(self.split_pattern, text) if token.strip() != '']
+        non_whitespace_tokens = []
+        for token in tokens:
+            split_tokens = token.split(' ')
+            non_whitespace_tokens.extend([token for token in split_tokens if token != ''])
+        # print('non_whitespace_tokens:', non_whitespace_tokens)
+        return non_whitespace_tokens
+        # return [token.replace(' ', '') for token in re.split(self.split_pattern, text) if token.replace(' ', '') != '']
         # return [token for token in re.split(r'\W+', text) if token != '']
 
 
 class CustomTokenizer(Tokenizer):
 
     def __init__(self, tokenizer_func: Callable, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search.egg-info/PKG-INFO` & `fuzzy_search-2.0.1a0/fuzzy_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy-search
-Version: 2.0.0a0
+Version: 2.0.1a0
 Summary: Tool for fuzzy searching in texts with historical language use and OCR/HTR errors
 Home-page: https://github.com/marijnkoolen/fuzzy-search
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 License: MIT
 Keywords: information extraction,historical research,digital resources
 Platform: UNKNOWN
```

### Comparing `fuzzy_search-2.0.0a0/fuzzy_search.egg-info/SOURCES.txt` & `fuzzy_search-2.0.1a0/fuzzy_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/setup.py` & `fuzzy_search-2.0.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_match_candidate.py` & `fuzzy_search-2.0.1a0/test/test_match_candidate.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_match_phrase.py` & `fuzzy_search-2.0.1a0/test/test_match_phrase.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_pattern_template.py` & `fuzzy_search-2.0.1a0/test/test_pattern_template.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_phrase_phrase.py` & `fuzzy_search-2.0.1a0/test/test_phrase_phrase.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_phrase_phrase_model.py` & `fuzzy_search-2.0.1a0/test/test_phrase_phrase_model.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_search_context_searcher.py` & `fuzzy_search-2.0.1a0/test/test_search_context_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_search_phrase_searcher.py` & `fuzzy_search-2.0.1a0/test/test_search_phrase_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_search_searcher.py` & `fuzzy_search-2.0.1a0/test/test_search_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_search_template_searcher.py` & `fuzzy_search-2.0.1a0/test/test_search_template_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_search_token_searcher.py` & `fuzzy_search-2.0.1a0/test/test_search_token_searcher.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_tokenization_string.py` & `fuzzy_search-2.0.1a0/test/test_tokenization_string.py`

 * *Files identical despite different names*

### Comparing `fuzzy_search-2.0.0a0/test/test_tokenization_token.py` & `fuzzy_search-2.0.1a0/test/test_tokenization_token.py`

 * *Files identical despite different names*

