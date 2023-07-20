# Comparing `tmp/sflkit-0.2.5.tar.gz` & `tmp/sflkit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sflkit-0.2.5.tar", last modified: Thu Jul 20 07:41:19 2023, max compression
+gzip compressed data, was "sflkit-0.2.6.tar", last modified: Thu Jul 20 14:45:55 2023, max compression
```

## Comparing `sflkit-0.2.5.tar` & `sflkit-0.2.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.275492 sflkit-0.2.5/
--rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.5/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 07:41:19.275612 sflkit-0.2.5/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     4050 2023-07-19 14:43:48.000000 sflkit-0.2.5/README.md
--rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-19 18:23:10.000000 sflkit-0.2.5/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-20 07:41:19.276260 sflkit-0.2.5/setup.cfg
--rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.5/setup.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.255041 sflkit-0.2.5/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.259916 sflkit-0.2.5/src/SFLKit.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/entry_points.txt
--rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-20 07:41:19.000000 sflkit-0.2.5/src/SFLKit.egg-info/top_level.txt
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.261127 sflkit-0.2.5/src/sflkit/
--rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-19 18:23:01.000000 sflkit-0.2.5/src/sflkit/__init__.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.264185 sflkit-0.2.5/src/sflkit/analysis/
--rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/analysis/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3605 2023-07-20 07:25:14.000000 sflkit-0.2.5/src/sflkit/analysis/analysis_type.py
--rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.5/src/sflkit/analysis/analyzer.py
--rw-r--r--   0 marius     (501) staff       (20)    13819 2023-07-18 09:22:13.000000 sflkit-0.2.5/src/sflkit/analysis/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/analysis/mapping.py
--rw-r--r--   0 marius     (501) staff       (20)    12806 2023-07-20 07:34:00.000000 sflkit-0.2.5/src/sflkit/analysis/predicate.py
--rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.5/src/sflkit/analysis/similarity.py
--rw-r--r--   0 marius     (501) staff       (20)    18219 2023-07-20 07:33:28.000000 sflkit-0.2.5/src/sflkit/analysis/spectra.py
--rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.5/src/sflkit/analysis/suggestion.py
--rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.5/src/sflkit/cli.py
--rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/color.py
--rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.5/src/sflkit/config.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.264961 sflkit-0.2.5/src/sflkit/instrumentation/
--rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.5/src/sflkit/instrumentation/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.5/src/sflkit/instrumentation/dir_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/instrumentation/file_instrumentation.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.266706 sflkit-0.2.5/src/sflkit/language/
--rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/language/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.5/src/sflkit/language/extract.py
--rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.5/src/sflkit/language/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.5/src/sflkit/language/language.py
--rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.5/src/sflkit/language/meta.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.268659 sflkit-0.2.5/src/sflkit/language/python/
--rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/language/python/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.5/src/sflkit/language/python/extract.py
--rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.5/src/sflkit/language/python/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/language/python/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/language/python/visitor.py
--rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.5/src/sflkit/language/visitor.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.270043 sflkit-0.2.5/src/sflkit/model/
--rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/model/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.5/src/sflkit/model/event_file.py
--rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/model/model.py
--rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.5/src/sflkit/model/scope.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.270649 sflkit-0.2.5/src/sflkit/runners/
--rw-r--r--   0 marius     (501) staff       (20)      362 2023-07-19 11:34:17.000000 sflkit-0.2.5/src/sflkit/runners/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8895 2023-07-19 14:43:48.000000 sflkit-0.2.5/src/sflkit/runners/run.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 07:41:19.275250 sflkit-0.2.5/tests/
--rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.5/tests/test_analysis_objects.py
--rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.5/tests/test_cli.py
--rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.5/tests/test_color.py
--rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.5/tests/test_config.py
--rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.5/tests/test_events.py
--rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.5/tests/test_execution.py
--rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.5/tests/test_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.5/tests/test_language.py
--rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.5/tests/test_predicates.py
--rw-r--r--   0 marius     (501) staff       (20)     7727 2023-07-19 11:35:28.000000 sflkit-0.2.5/tests/test_runner.py
--rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.5/tests/test_scope.py
--rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.5/tests/test_spectra.py
--rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.5/tests/test_suggestions.py
--rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.5/tests/test_visitors.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.061460 sflkit-0.2.6/
+-rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.6/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 14:45:55.061619 sflkit-0.2.6/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     4050 2023-07-19 14:43:48.000000 sflkit-0.2.6/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-20 14:40:30.000000 sflkit-0.2.6/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-20 14:45:55.062301 sflkit-0.2.6/setup.cfg
+-rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.6/setup.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.033739 sflkit-0.2.6/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.039142 sflkit-0.2.6/src/SFLKit.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/entry_points.txt
+-rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.040287 sflkit-0.2.6/src/sflkit/
+-rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-20 14:40:30.000000 sflkit-0.2.6/src/sflkit/__init__.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.044592 sflkit-0.2.6/src/sflkit/analysis/
+-rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/analysis/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3707 2023-07-20 08:38:14.000000 sflkit-0.2.6/src/sflkit/analysis/analysis_type.py
+-rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.6/src/sflkit/analysis/analyzer.py
+-rw-r--r--   0 marius     (501) staff       (20)    15380 2023-07-20 14:39:25.000000 sflkit-0.2.6/src/sflkit/analysis/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/analysis/mapping.py
+-rw-r--r--   0 marius     (501) staff       (20)    12806 2023-07-20 07:34:00.000000 sflkit-0.2.6/src/sflkit/analysis/predicate.py
+-rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.6/src/sflkit/analysis/similarity.py
+-rw-r--r--   0 marius     (501) staff       (20)    18236 2023-07-20 08:39:14.000000 sflkit-0.2.6/src/sflkit/analysis/spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.6/src/sflkit/analysis/suggestion.py
+-rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.6/src/sflkit/cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/color.py
+-rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.6/src/sflkit/config.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.046098 sflkit-0.2.6/src/sflkit/instrumentation/
+-rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.6/src/sflkit/instrumentation/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.6/src/sflkit/instrumentation/dir_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/instrumentation/file_instrumentation.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.048777 sflkit-0.2.6/src/sflkit/language/
+-rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.6/src/sflkit/language/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.6/src/sflkit/language/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.6/src/sflkit/language/language.py
+-rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.6/src/sflkit/language/meta.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.052273 sflkit-0.2.6/src/sflkit/language/python/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.6/src/sflkit/language/python/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.6/src/sflkit/language/python/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/visitor.py
+-rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.6/src/sflkit/language/visitor.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.054152 sflkit-0.2.6/src/sflkit/model/
+-rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.6/src/sflkit/model/event_file.py
+-rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/model.py
+-rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/scope.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.054779 sflkit-0.2.6/src/sflkit/runners/
+-rw-r--r--   0 marius     (501) staff       (20)      362 2023-07-19 11:34:17.000000 sflkit-0.2.6/src/sflkit/runners/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8895 2023-07-19 14:43:48.000000 sflkit-0.2.6/src/sflkit/runners/run.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.061143 sflkit-0.2.6/tests/
+-rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.6/tests/test_analysis_objects.py
+-rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.6/tests/test_cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.6/tests/test_color.py
+-rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.6/tests/test_config.py
+-rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.6/tests/test_events.py
+-rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.6/tests/test_execution.py
+-rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.6/tests/test_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.6/tests/test_language.py
+-rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.6/tests/test_predicates.py
+-rw-r--r--   0 marius     (501) staff       (20)     7727 2023-07-19 11:35:28.000000 sflkit-0.2.6/tests/test_runner.py
+-rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.6/tests/test_scope.py
+-rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.6/tests/test_spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.6/tests/test_suggestions.py
+-rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.6/tests/test_visitors.py
```

### Comparing `sflkit-0.2.5/LICENSE` & `sflkit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/PKG-INFO` & `sflkit-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.5
+Version: 0.2.6
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.5/README.md` & `sflkit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/pyproject.toml` & `sflkit-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=67.6.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sflkit"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     { name = "Marius Smytzek", email = "marius.smytzek@cispa.de" },
 ]
 description = "SFLKit: : A Workbench for Statistical Fault Localization"
 readme = "README.md"
 license = { file = "COPYING" }
 requires-python = ">=3.10"
```

### Comparing `sflkit-0.2.5/setup.cfg` & `sflkit-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/SFLKit.egg-info/PKG-INFO` & `sflkit-0.2.6/src/SFLKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.5
+Version: 0.2.6
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.5/src/SFLKit.egg-info/SOURCES.txt` & `sflkit-0.2.6/src/SFLKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/__init__.py` & `sflkit-0.2.6/src/sflkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from sflkit.analysis.analyzer import Analyzer
 from sflkit.analysis.predicate import Predicate
 from sflkit.config import Config, parse_config
 from sflkit.instrumentation.dir_instrumentation import DirInstrumentation
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 
 def instrument_config(conf: Config, event_dump: str = None):
     instrumentation = DirInstrumentation(conf.visitor)
     instrumentation.instrument(
         conf.target_path,
         conf.instrument_working,
```

### Comparing `sflkit-0.2.5/src/sflkit/analysis/analysis_type.py` & `sflkit-0.2.6/src/sflkit/analysis/analysis_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         AnalysisObject.branch_finder = branch_finder
 
     # noinspection PyUnusedLocal
     def __init__(self, event):
         self.suspiciousness: float = 0
         self.last_evaluation: EvaluationResult = EvaluationResult.UNOBSERVED
 
+    def get_last_evaluation(self, id_: int) -> EvaluationResult:
+        return self.last_evaluation
+
     def __repr__(self):
         return f"{self.analysis_type()}:{self.suspiciousness}"
 
     def __str__(self):
         return f"{self.analysis_type()}"
 
     @staticmethod
```

### Comparing `sflkit-0.2.5/src/sflkit/analysis/analyzer.py` & `sflkit-0.2.6/src/sflkit/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/analysis/factory.py` & `sflkit-0.2.6/src/sflkit/analysis/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import abc
 from abc import abstractmethod
 from typing import List, Type, Set
 
 from sflkitlib.events import EventType
 
 from sflkit.analysis.analysis_type import AnalysisObject, AnalysisType
 from sflkit.analysis.predicate import (
@@ -71,21 +72,25 @@
             key = (Line.analysis_type(), event.file, event.line)
             if key not in self.objects:
                 self.objects[key] = Line(event)
             return [self.objects[key]]
 
 
 class BranchFactory(AnalysisFactory):
+    def __init__(self, else_: bool = True):
+        super().__init__()
+        self.else_ = else_
+
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type == EventType.BRANCH:
             key = (Branch.analysis_type(), event.file, event.line, event.then_id)
             then = event.then_id < event.else_id
             if key not in self.objects:
                 self.objects[key] = Branch(event, then=then)
-            if event.else_id >= 0:
+            if self.else_ and event.else_id >= 0:
                 else_key = (
                     Branch.analysis_type(),
                     event.file,
                     event.line,
                     event.else_id,
                 )
                 if else_key not in self.objects:
@@ -100,30 +105,38 @@
             key = (Function.analysis_type(), event.file, event.line, event.function_id)
             if key not in self.objects:
                 self.objects[key] = Function(event)
             return [self.objects[key]]
 
 
 class LoopFactory(AnalysisFactory):
+    def __init__(self, hit_0: bool = True, hit_1: bool = True, hit_more: bool = True):
+        super().__init__()
+        self.hit_0 = hit_0
+        self.hit_1 = hit_1
+        self.hit_more = hit_more
+
     def get_all(self) -> Set[AnalysisObject]:
         return set(obj for value in self.objects.values() for obj in value)
 
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type in (
             EventType.LOOP_BEGIN,
             EventType.LOOP_HIT,
             EventType.LOOP_END,
         ):
             key = (Loop.analysis_type(), event.file, event.line, event.loop_id)
             if key not in self.objects:
-                self.objects[key] = [
-                    Loop(event, Loop.evaluate_hit_0),
-                    Loop(event, Loop.evaluate_hit_1),
-                    Loop(event, Loop.evaluate_hit_more),
-                ]
+                self.objects[key] = []
+                if self.hit_0:
+                    self.objects[key].append(Loop(event, Loop.evaluate_hit_0)),
+                if self.hit_1:
+                    self.objects[key].append(Loop(event, Loop.evaluate_hit_1)),
+                if self.hit_more:
+                    self.objects[key].append(Loop(event, Loop.evaluate_hit_more)),
             if event.event_type == EventType.LOOP_BEGIN:
                 list(map(Loop.start_loop, self.objects[key]))
             elif event.event_type == EventType.LOOP_HIT:
                 list(map(Loop.hit_loop, self.objects[key]))
             elif event.event_type == EventType.LOOP_END:
                 return self.objects[key][:]
             return list()
@@ -160,26 +173,52 @@
         if event.event_type == EventType.CONDITION:
             key = (Condition.analysis_type(), event.file, event.line, event.condition)
             if key not in self.objects:
                 self.objects[key] = Condition(event.file, event.line, event.condition)
             return [self.objects[key]]
 
 
-class ScalarPairFactory(AnalysisFactory):
+class ComparisonFactory(AnalysisFactory, abc.ABC):
+    def __init__(
+        self,
+        eq: bool = True,
+        ne: bool = True,
+        lt: bool = True,
+        le: bool = True,
+        gt: bool = True,
+        ge: bool = True,
+    ):
+        super().__init__()
+        self.comparators = []
+        if eq:
+            self.comparators.append(Comp.EQ)
+        if ne:
+            self.comparators.append(Comp.NE)
+        if lt:
+            self.comparators.append(Comp.LT)
+        if le:
+            self.comparators.append(Comp.LE)
+        if gt:
+            self.comparators.append(Comp.GT)
+        if ge:
+            self.comparators.append(Comp.GE)
+
+
+class ScalarPairFactory(ComparisonFactory):
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type == EventType.DEF:
             variables = scope.get_all_vars()
             objects = list()
             if event.type_ in ["int", "float", "bool", "str", "bytes"]:
                 for types in (["int", "float", "bool"], ["str"], ["bytes"]):
                     if event.type_ in types:
                         for variable in variables:
                             if variable.var != event.var:
                                 if variable.type_ in types:
-                                    for comp in Comp:
+                                    for comp in self.comparators:
                                         key = (
                                             ScalarPair.analysis_type(),
                                             event.file,
                                             event.line,
                                             event.var,
                                             variable.var,
                                             comp,
@@ -190,105 +229,109 @@
                                                 event, comp, variable.var
                                             )
                                         objects.append(self.objects[key])
             else:
                 for variable in variables:
                     if variable.type_ == event.type_:
                         for comp in (Comp.EQ, Comp.NE):
-                            key = (
-                                ScalarPair.analysis_type(),
-                                event.file,
-                                event.line,
-                                event.var,
-                                variable.var,
-                                comp,
-                                event.type_,
-                            )
-                            if key not in self.objects:
-                                self.objects[key] = ScalarPair(
-                                    event, comp, variable.var
+                            if comp in self.comparators:
+                                key = (
+                                    ScalarPair.analysis_type(),
+                                    event.file,
+                                    event.line,
+                                    event.var,
+                                    variable.var,
+                                    comp,
+                                    event.type_,
                                 )
-                            objects.append(self.objects[key])
+                                if key not in self.objects:
+                                    self.objects[key] = ScalarPair(
+                                        event, comp, variable.var
+                                    )
+                                objects.append(self.objects[key])
             return objects
 
 
-class VariableFactory(AnalysisFactory):
+class VariableFactory(ComparisonFactory):
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type == EventType.DEF and event.type_ in [
             "int",
             "float",
             "bool",
         ]:
             objects = list()
-            for comp in Comp:
+            for comp in self.comparators:
                 key = (
                     VariablePredicate.analysis_type(),
                     event.file,
                     event.line,
                     event.var,
                     comp,
                     "int",
                 )
                 if key not in self.objects:
                     self.objects[key] = VariablePredicate(event, comp)
                 objects.append(self.objects[key])
             return objects
 
 
-class ReturnFactory(AnalysisFactory):
+class ReturnFactory(ComparisonFactory):
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type == EventType.FUNCTION_EXIT:
             objects = list()
             if event.type_ in ("int", "float", "bool", "str", "bytes"):
                 if event.type_ in ("int", "float", "bool"):
                     type_, tr = "num", 0
                     compare = Comp
                 elif event.type_ == "str":
                     type_, tr = "str", ""
                     compare = Comp.EQ, Comp.NE
                 else:
                     type_, tr = "bytes", b""
                     compare = Comp.EQ, Comp.NE
                 for comp in compare:
-                    key = (
-                        ReturnPredicate.analysis_type(),
-                        event.file,
-                        event.line,
-                        event.function,
-                        comp,
-                        type_,
-                    )
-                    if key not in self.objects:
-                        self.objects[key] = ReturnPredicate(event, comp, value=tr)
-                    objects.append(self.objects[key])
+                    if comp in self.comparators:
+                        key = (
+                            ReturnPredicate.analysis_type(),
+                            event.file,
+                            event.line,
+                            event.function,
+                            comp,
+                            type_,
+                        )
+                        if key not in self.objects:
+                            self.objects[key] = ReturnPredicate(event, comp, value=tr)
+                        objects.append(self.objects[key])
             if event.type_ == "NoneType":
                 for comp in Comp.EQ, Comp.NE:
-                    key = (
-                        ReturnPredicate.analysis_type(),
-                        event.file,
-                        event.line,
-                        event.function,
-                        comp,
-                        event.type_,
-                    )
-                    if key not in self.objects:
-                        self.objects[key] = ReturnPredicate(event, comp, value=None)
-                    objects.append(self.objects[key])
+                    if comp in self.comparators:
+                        key = (
+                            ReturnPredicate.analysis_type(),
+                            event.file,
+                            event.line,
+                            event.function,
+                            comp,
+                            event.type_,
+                        )
+                        if key not in self.objects:
+                            self.objects[key] = ReturnPredicate(event, comp, value=None)
+                        objects.append(self.objects[key])
             else:
                 for comp in Comp.EQ, Comp.NE:
-                    key = (
-                        ReturnPredicate.analysis_type(),
-                        event.file,
-                        event.line,
-                        event.function,
-                        comp,
-                        "NoneType",
-                    )
-                    if key in self.objects:
-                        objects.append(self.objects[key])
+                    if comp in self.comparators:
+                        key = (
+                            ReturnPredicate.analysis_type(),
+                            event.file,
+                            event.line,
+                            event.function,
+                            comp,
+                            "NoneType",
+                        )
+                        if key in self.objects:
+                            objects.append(self.objects[key])
             return objects
 
 
 class ConstantCompFactory(AnalysisFactory):
     def __init__(self, class_: Type[AnalysisObject]):
         super().__init__()
         self.class_ = class_
```

### Comparing `sflkit-0.2.5/src/sflkit/analysis/mapping.py` & `sflkit-0.2.6/src/sflkit/analysis/mapping.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/analysis/predicate.py` & `sflkit-0.2.6/src/sflkit/analysis/predicate.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/analysis/similarity.py` & `sflkit-0.2.6/src/sflkit/analysis/similarity.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/analysis/spectra.py` & `sflkit-0.2.6/src/sflkit/analysis/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.assign_suspiciousness(metric)
         return Suggestion([Location(self.file, self.line)], self.suspiciousness)
 
     def assign_suspiciousness(self, metric: Callable = None):
         self.suspiciousness = self.get_metric(metric)
 
     def hit(self, id_, event, scope_: Scope = None):
-        self.last_evaluation = True
+        self.last_evaluation = EvaluationResult.TRUE
         if id_ not in self.hits:
             self.hits[id_] = 1
         else:
             self.hits[id_] += 1
 
     def pass_observed(self):
         self.passed_observed += 1
```

### Comparing `sflkit-0.2.5/src/sflkit/analysis/suggestion.py` & `sflkit-0.2.6/src/sflkit/analysis/suggestion.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/cli.py` & `sflkit-0.2.6/src/sflkit/cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/color.py` & `sflkit-0.2.6/src/sflkit/color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/config.py` & `sflkit-0.2.6/src/sflkit/config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/instrumentation/__init__.py` & `sflkit-0.2.6/src/sflkit/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/instrumentation/dir_instrumentation.py` & `sflkit-0.2.6/src/sflkit/instrumentation/dir_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/finder.py` & `sflkit-0.2.6/src/sflkit/language/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/language.py` & `sflkit-0.2.6/src/sflkit/language/language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/meta.py` & `sflkit-0.2.6/src/sflkit/language/meta.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/python/extract.py` & `sflkit-0.2.6/src/sflkit/language/python/extract.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/python/factory.py` & `sflkit-0.2.6/src/sflkit/language/python/factory.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/python/finder.py` & `sflkit-0.2.6/src/sflkit/language/python/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/python/visitor.py` & `sflkit-0.2.6/src/sflkit/language/python/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/language/visitor.py` & `sflkit-0.2.6/src/sflkit/language/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/model/event_file.py` & `sflkit-0.2.6/src/sflkit/model/event_file.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/model/model.py` & `sflkit-0.2.6/src/sflkit/model/model.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/model/scope.py` & `sflkit-0.2.6/src/sflkit/model/scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/src/sflkit/runners/run.py` & `sflkit-0.2.6/src/sflkit/runners/run.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_analysis_objects.py` & `sflkit-0.2.6/tests/test_analysis_objects.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_cli.py` & `sflkit-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_color.py` & `sflkit-0.2.6/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_config.py` & `sflkit-0.2.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_events.py` & `sflkit-0.2.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_execution.py` & `sflkit-0.2.6/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_instrumentation.py` & `sflkit-0.2.6/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_language.py` & `sflkit-0.2.6/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_predicates.py` & `sflkit-0.2.6/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_runner.py` & `sflkit-0.2.6/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_scope.py` & `sflkit-0.2.6/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_spectra.py` & `sflkit-0.2.6/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_suggestions.py` & `sflkit-0.2.6/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.5/tests/test_visitors.py` & `sflkit-0.2.6/tests/test_visitors.py`

 * *Files identical despite different names*

