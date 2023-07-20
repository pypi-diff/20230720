# Comparing `tmp/types-dateparser-1.1.4.8.tar.gz` & `tmp/types-dateparser-1.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-dateparser-1.1.4.8.tar", last modified: Tue Feb 21 01:32:56 2023, max compression
+gzip compressed data, was "types-dateparser-1.1.4.9.tar", last modified: Mon Mar 27 18:22:38 2023, max compression
```

## Comparing `types-dateparser-1.1.4.8.tar` & `types-dateparser-1.1.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-21 01:32:55.000000 types-dateparser-1.1.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:32:55.000000 types-dateparser-1.1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.159209 types-dateparser-1.1.4.8/dateparser-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-21 01:32:55.000000 types-dateparser-1.1.4.8/dateparser-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.159209 types-dateparser-1.1.4.8/dateparser-stubs/calendars/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/calendars/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/calendars/hijri.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/calendars/hijri_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/calendars/jalali.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/calendars/jalali_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/conf.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser-stubs/custom_language_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/custom_language_detection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/custom_language_detection/fasttext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/custom_language_detection/langdetect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/custom_language_detection/language_mapping.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/data/languages_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/date.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/date_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/freshness_date_parser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/languages/dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/languages/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/languages/locale.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/languages/validation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/parser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser-stubs/search/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/search/detection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/search/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/search/text_detection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/timezone_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/timezones.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser-stubs/utils/strptime.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/dateparser_data-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-21 01:32:55.000000 types-dateparser-1.1.4.8/dateparser_data-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser_data-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-21 01:26:21.000000 types-dateparser-1.1.4.8/dateparser_data-stubs/settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-21 01:32:55.000000 types-dateparser-1.1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:32:56.163210 types-dateparser-1.1.4.8/types_dateparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:32:56.000000 types-dateparser-1.1.4.8/types_dateparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-21 01:32:56.000000 types-dateparser-1.1.4.8/types_dateparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:32:56.000000 types-dateparser-1.1.4.8/types_dateparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-21 01:32:56.000000 types-dateparser-1.1.4.8/types_dateparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/dateparser-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/jalali.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/calendars/jalali_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/conf.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/fasttext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/langdetect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/custom_language_detection/language_mapping.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/data/languages_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/date.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/date_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/freshness_date_parser.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/languages/validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/parser.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.118065 types-dateparser-1.1.4.9/dateparser-stubs/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/search/text_detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/timezone_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/timezones.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/dateparser-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser-stubs/utils/strptime.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/dateparser_data-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-27 18:21:24.000000 types-dateparser-1.1.4.9/dateparser_data-stubs/settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-27 18:22:37.000000 types-dateparser-1.1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:38.122065 types-dateparser-1.1.4.9/types_dateparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 18:22:38.000000 types-dateparser-1.1.4.9/types_dateparser.egg-info/top_level.txt
```

### Comparing `types-dateparser-1.1.4.8/CHANGELOG.md` & `types-dateparser-1.1.4.9/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.1.4.9 (2023-03-27)
+
+Add defaults for third-party stubs A-D (#9952)
+
 ## 1.1.4.8 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 1.1.4.7 (2023-02-15)
```

### Comparing `types-dateparser-1.1.4.8/PKG-INFO` & `types-dateparser-1.1.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dateparser
-Version: 1.1.4.8
+Version: 1.1.4.9
 Summary: Typing stubs for dateparser
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dateparser`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/__init__.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     SKIP_TOKENS: list[str]
     NORMALIZE: bool
     RETURN_TIME_AS_PERIOD: bool
     PARSERS: list[_ParserKind]
 
 def parse(
     date_string: str,
-    date_formats: list[str] | tuple[str, ...] | set[str] | None = ...,
-    languages: list[str] | tuple[str, ...] | set[str] | None = ...,
-    locales: list[str] | tuple[str, ...] | set[str] | None = ...,
-    region: str | None = ...,
-    settings: _Settings | None = ...,
-    detect_languages_function: _DetectLanguagesFunction | None = ...,
+    date_formats: list[str] | tuple[str, ...] | set[str] | None = None,
+    languages: list[str] | tuple[str, ...] | set[str] | None = None,
+    locales: list[str] | tuple[str, ...] | set[str] | None = None,
+    region: str | None = None,
+    settings: _Settings | None = None,
+    detect_languages_function: _DetectLanguagesFunction | None = None,
 ) -> datetime.datetime | None: ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/calendars/hijri_parser.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/calendars/hijri_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/date.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/date.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,37 +25,37 @@
 RE_SANITIZE_APOSTROPHE: Pattern[str]
 RE_SEARCH_TIMESTAMP: Pattern[str]
 RE_SANITIZE_CROATIAN: Pattern[str]
 RE_SEARCH_NEGATIVE_TIMESTAMP: Pattern[str]
 
 def sanitize_spaces(date_string: str) -> str: ...
 def date_range(begin, end, **kwargs) -> None: ...
-def get_intersecting_periods(low, high, period: str = ...) -> None: ...
+def get_intersecting_periods(low, high, period: str = "day") -> None: ...
 def sanitize_date(date_string: str) -> str: ...
-def get_date_from_timestamp(date_string: str, settings: Settings, negative: bool = ...) -> datetime | None: ...
+def get_date_from_timestamp(date_string: str, settings: Settings, negative: bool = False) -> datetime | None: ...
 def parse_with_formats(date_string: str, date_formats: Iterable[str], settings: Settings) -> DateData: ...
 
 class _DateLocaleParser:
     locale: Locale
     date_string: str
     date_formats: list[str] | tuple[str, ...] | set[str] | None
     def __init__(
         self,
         locale: Locale,
         date_string: str,
         date_formats: list[str] | tuple[str, ...] | set[str] | None,
-        settings: Settings | None = ...,
+        settings: Settings | None = None,
     ) -> None: ...
     @classmethod
     def parse(
         cls,
         locale: Locale,
         date_string: str,
-        date_formats: list[str] | tuple[str, ...] | set[str] | None = ...,
-        settings: Settings | None = ...,
+        date_formats: list[str] | tuple[str, ...] | set[str] | None = None,
+        settings: Settings | None = None,
     ) -> DateData: ...
     def _parse(self) -> DateData | None: ...
     def _try_timestamp(self) -> DateData: ...
     def _try_freshness_parser(self) -> DateData | None: ...
     def _try_absolute_parser(self) -> DateData | None: ...
     def _try_nospaces_parser(self) -> DateData | None: ...
     def _try_parser(self, parse_method) -> DateData | None: ...
@@ -64,15 +64,15 @@
     def _get_translated_date_with_formatting(self) -> str: ...
     def _is_valid_date_data(self, date_data: DateData) -> bool: ...
 
 class DateData:
     date_obj: datetime | None
     locale: str | None
     period: _Period | None
-    def __init__(self, *, date_obj: datetime | None = ..., period: _Period | None = ..., locale: str | None = ...) -> None: ...
+    def __init__(self, *, date_obj: datetime | None = None, period: _Period | None = None, locale: str | None = None) -> None: ...
     @overload
     def __getitem__(self, k: Literal["date_obj"]) -> datetime | None: ...
     @overload
     def __getitem__(self, k: Literal["locale"]) -> str | None: ...
     @overload
     def __getitem__(self, k: Literal["period"]) -> _Period | None: ...
     @overload
@@ -90,21 +90,21 @@
     languages: list[str] | None
     locales: list[str] | tuple[str, ...] | set[str] | None
     region: str
     detect_languages_function: _DetectLanguagesFunction | None
     previous_locales: collections.OrderedDict[Locale, None]
     def __init__(
         self,
-        languages: list[str] | tuple[str, ...] | set[str] | None = ...,
-        locales: list[str] | tuple[str, ...] | set[str] | None = ...,
-        region: str | None = ...,
-        try_previous_locales: bool = ...,
-        use_given_order: bool = ...,
-        settings: _Settings | None = ...,
-        detect_languages_function: _DetectLanguagesFunction | None = ...,
+        languages: list[str] | tuple[str, ...] | set[str] | None = None,
+        locales: list[str] | tuple[str, ...] | set[str] | None = None,
+        region: str | None = None,
+        try_previous_locales: bool = False,
+        use_given_order: bool = False,
+        settings: _Settings | None = None,
+        detect_languages_function: _DetectLanguagesFunction | None = None,
     ) -> None: ...
-    def get_date_data(self, date_string: str, date_formats: list[str] | tuple[str, ...] | set[str] | None = ...) -> DateData: ...
+    def get_date_data(self, date_string: str, date_formats: list[str] | tuple[str, ...] | set[str] | None = None) -> DateData: ...
     def get_date_tuple(self, date_string: str, date_formats: list[str] | tuple[str, ...] | set[str] | None = ...): ...
     def _get_applicable_locales(self, date_string: str) -> Iterator[Locale]: ...
     def _is_applicable_locale(self, locale: Locale, date_string: str) -> bool: ...
     @classmethod
     def _get_locale_loader(cls: type[DateDataParser]) -> LocaleDataLoader: ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/languages/loader.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/languages/loader.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from .locale import Locale
 
 LOCALE_SPLIT_PATTERN: Any
 
 class LocaleDataLoader:
     def get_locale_map(
         self,
-        languages: list[str] | None = ...,
-        locales: list[str] | None = ...,
-        region: str | None = ...,
-        use_given_order: bool = ...,
-        allow_conflicting_locales: bool = ...,
+        languages: list[str] | None = None,
+        locales: list[str] | None = None,
+        region: str | None = None,
+        use_given_order: bool = False,
+        allow_conflicting_locales: bool = False,
     ) -> OrderedDict[str, list[Any] | str | int]: ...
     def get_locales(
         self,
-        languages: list[str] | None = ...,
-        locales: list[str] | None = ...,
-        region: str | None = ...,
-        use_given_order: bool = ...,
-        allow_conflicting_locales: bool = ...,
+        languages: list[str] | None = None,
+        locales: list[str] | None = None,
+        region: str | None = None,
+        use_given_order: bool = False,
+        allow_conflicting_locales: bool = False,
     ) -> Iterator[Locale]: ...
     def get_locale(self, shortname: str) -> Locale: ...
 
 default_loader: Any
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/languages/locale.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/languages/locale.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dateparser.conf import Settings
 
 NUMERAL_PATTERN: Pattern[str]
 
 class Locale:
     shortname: str
     def __init__(self, shortname: str, language_info) -> None: ...
-    def is_applicable(self, date_string: str, strip_timezone: bool = ..., settings: Settings | None = ...) -> bool: ...
-    def count_applicability(self, text: str, strip_timezone: bool = ..., settings: Settings | None = ...): ...
+    def is_applicable(self, date_string: str, strip_timezone: bool = False, settings: Settings | None = None) -> bool: ...
+    def count_applicability(self, text: str, strip_timezone: bool = False, settings: Settings | None = None): ...
     @staticmethod
-    def clean_dictionary(dictionary, threshold: int = ...): ...
-    def translate(self, date_string: str, keep_formatting: bool = ..., settings: Settings | None = ...) -> str: ...
-    def translate_search(self, search_string, settings: Settings | None = ...): ...
+    def clean_dictionary(dictionary, threshold: int = 2): ...
+    def translate(self, date_string: str, keep_formatting: bool = False, settings: Settings | None = None) -> str: ...
+    def translate_search(self, search_string, settings: Settings | None = None): ...
     def get_wordchars_for_detection(self, settings): ...
     def to_parserinfo(self, base_cls=...): ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/parser.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/parser.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 HOUR_MINUTE_REGEX: Any
 
 def no_space_parser_eligibile(datestring): ...
 def get_unresolved_attrs(parser_object): ...
 
 date_order_chart: Any
 
-def resolve_date_order(order, lst: Incomplete | None = ...): ...
+def resolve_date_order(order, lst: Incomplete | None = None): ...
 
 class _time_parser:
     time_directives: Any
     def __call__(self, timestring): ...
 
 time_parser: Any
 
@@ -39,15 +39,15 @@
     month: Any
     year: Any
     time: Any
     auto_order: Any
     ordered_num_directives: Any
     def __init__(self, tokens, settings): ...
     @classmethod
-    def parse(cls, datestring, settings, tz: datetime.tzinfo | None = ...): ...
+    def parse(cls, datestring, settings, tz: datetime.tzinfo | None = None): ...
 
 class tokenizer:
     digits: str
     letters: str
     instream: Any
     def __init__(self, ds) -> None: ...
     def tokenize(self) -> None: ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/search/__init__.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/search/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 @overload
 def search_dates(
     text: str,
     languages: list[str] | tuple[str, ...] | AbstractSet[str] | None,
     settings: Mapping[Any, Any] | None,
     add_detected_language: Literal[True],
-    detect_languages_function: _DetectLanguagesFunction | None = ...,
+    detect_languages_function: _DetectLanguagesFunction | None = None,
 ) -> list[tuple[str, datetime, str]]: ...
 @overload
 def search_dates(
     text: str,
-    languages: list[str] | tuple[str, ...] | AbstractSet[str] | None = ...,
-    settings: Mapping[Any, Any] | None = ...,
-    add_detected_language: Literal[False] = ...,
-    detect_languages_function: _DetectLanguagesFunction | None = ...,
+    languages: list[str] | tuple[str, ...] | AbstractSet[str] | None = None,
+    settings: Mapping[Any, Any] | None = None,
+    add_detected_language: Literal[False] = False,
+    detect_languages_function: _DetectLanguagesFunction | None = None,
 ) -> list[tuple[str, datetime]]: ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/search/detection.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/search/detection.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from _typeshed import Incomplete
 from typing import Any
 
 class BaseLanguageDetector:
     languages: Any
     def __init__(self, languages) -> None: ...
-    def iterate_applicable_languages(self, date_string, modify: bool = ..., settings: Incomplete | None = ...) -> None: ...
+    def iterate_applicable_languages(self, date_string, modify: bool = False, settings: Incomplete | None = None) -> None: ...
 
 class AutoDetectLanguage(BaseLanguageDetector):
     language_pool: Any
     allow_redetection: Any
-    def __init__(self, languages, allow_redetection: bool = ...) -> None: ...
+    def __init__(self, languages, allow_redetection: bool = False) -> None: ...
     languages: Any
-    def iterate_applicable_languages(self, date_string, modify: bool = ..., settings: Incomplete | None = ...) -> None: ...
+    def iterate_applicable_languages(self, date_string, modify: bool = False, settings: Incomplete | None = None) -> None: ...
 
 class ExactLanguages(BaseLanguageDetector):
     def __init__(self, languages) -> None: ...
-    def iterate_applicable_languages(self, date_string, modify: bool = ..., settings: Incomplete | None = ...) -> None: ...
+    def iterate_applicable_languages(self, date_string, modify: bool = False, settings: Incomplete | None = None) -> None: ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/search/search.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/search/search.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,20 @@
 class DateSearchWithDetection:
     loader: Any
     available_language_map: Any
     search: Any
     def __init__(self) -> None: ...
     language_detector: Any
     def detect_language(
-        self, text, languages, settings: Incomplete | None = ..., detect_languages_function: _DetectLanguagesFunction | None = ...
+        self,
+        text,
+        languages,
+        settings: Incomplete | None = None,
+        detect_languages_function: _DetectLanguagesFunction | None = None,
     ): ...
     def search_dates(
         self,
         text,
-        languages: Incomplete | None = ...,
-        settings: Incomplete | None = ...,
-        detect_languages_function: _DetectLanguagesFunction | None = ...,
+        languages: Incomplete | None = None,
+        settings: Incomplete | None = None,
+        detect_languages_function: _DetectLanguagesFunction | None = None,
     ): ...
```

### Comparing `types-dateparser-1.1.4.8/dateparser-stubs/utils/__init__.pyi` & `types-dateparser-1.1.4.9/dateparser-stubs/utils/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from _typeshed import Incomplete
 from collections import OrderedDict
 from collections.abc import Mapping
 from typing import Any
 
 def strip_braces(date_string: str) -> str: ...
-def normalize_unicode(string: str, form: str = ...) -> str: ...
+def normalize_unicode(string: str, form: str = "NFKD") -> str: ...
 def combine_dicts(
     primary_dict: Mapping[Any, Any], supplementary_dict: Mapping[Any, Any]
 ) -> OrderedDict[str, str | list[Any]]: ...
 def find_date_separator(format) -> Any: ...
 def localize_timezone(date_time, tz_string): ...
 def apply_tzdatabase_timezone(date_time, pytz_string): ...
 def apply_dateparser_timezone(utc_datetime, offset_or_timezone_abb): ...
 def apply_timezone(date_time, tz_string): ...
 def apply_timezone_from_settings(date_obj, settings): ...
 def get_last_day_of_month(year, month): ...
 def get_previous_leap_year(year): ...
 def get_next_leap_year(year): ...
-def set_correct_day_from_settings(date_obj, settings, current_day: Incomplete | None = ...): ...
+def set_correct_day_from_settings(date_obj, settings, current_day: Incomplete | None = None): ...
 def registry(cls): ...
 def get_logger() -> Any: ...
 def setup_logging() -> None: ...
 
 # TODO: this needs `types-pytz` and a type-alias
 def get_timezone_from_tz_string(tz_string: str) -> Incomplete: ...
```

### Comparing `types-dateparser-1.1.4.8/setup.py` & `types-dateparser-1.1.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dateparser`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.4.8",
+      version="1.1.4.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['dateparser_data-stubs', 'dateparser-stubs'],
-      package_data={'dateparser_data-stubs': ['__init__.pyi', 'settings.pyi', 'METADATA.toml'], 'dateparser-stubs': ['__init__.pyi', 'calendars/__init__.pyi', 'calendars/hijri.pyi', 'calendars/hijri_parser.pyi', 'calendars/jalali.pyi', 'calendars/jalali_parser.pyi', 'conf.pyi', 'custom_language_detection/__init__.pyi', 'custom_language_detection/fasttext.pyi', 'custom_language_detection/langdetect.pyi', 'custom_language_detection/language_mapping.pyi', 'data/__init__.pyi', 'data/languages_info.pyi', 'date.pyi', 'date_parser.pyi', 'freshness_date_parser.pyi', 'languages/__init__.pyi', 'languages/dictionary.pyi', 'languages/loader.pyi', 'languages/locale.pyi', 'languages/validation.pyi', 'parser.pyi', 'search/__init__.pyi', 'search/detection.pyi', 'search/search.pyi', 'search/text_detection.pyi', 'timezone_parser.pyi', 'timezones.pyi', 'utils/__init__.pyi', 'utils/strptime.pyi', 'METADATA.toml']},
+      packages=['dateparser-stubs', 'dateparser_data-stubs'],
+      package_data={'dateparser-stubs': ['__init__.pyi', 'calendars/__init__.pyi', 'calendars/hijri.pyi', 'calendars/hijri_parser.pyi', 'calendars/jalali.pyi', 'calendars/jalali_parser.pyi', 'conf.pyi', 'custom_language_detection/__init__.pyi', 'custom_language_detection/fasttext.pyi', 'custom_language_detection/langdetect.pyi', 'custom_language_detection/language_mapping.pyi', 'data/__init__.pyi', 'data/languages_info.pyi', 'date.pyi', 'date_parser.pyi', 'freshness_date_parser.pyi', 'languages/__init__.pyi', 'languages/dictionary.pyi', 'languages/loader.pyi', 'languages/locale.pyi', 'languages/validation.pyi', 'parser.pyi', 'search/__init__.pyi', 'search/detection.pyi', 'search/search.pyi', 'search/text_detection.pyi', 'timezone_parser.pyi', 'timezones.pyi', 'utils/__init__.pyi', 'utils/strptime.pyi', 'METADATA.toml'], 'dateparser_data-stubs': ['__init__.pyi', 'settings.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-dateparser-1.1.4.8/types_dateparser.egg-info/PKG-INFO` & `types-dateparser-1.1.4.9/types_dateparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dateparser
-Version: 1.1.4.8
+Version: 1.1.4.9
 Summary: Typing stubs for dateparser
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dateparser.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dateparser`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dateparser. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-dateparser-1.1.4.8/types_dateparser.egg-info/SOURCES.txt` & `types-dateparser-1.1.4.9/types_dateparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

