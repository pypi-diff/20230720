# Comparing `tmp/flordb-2.6.4.tar.gz` & `tmp/flordb-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.6.4.tar", last modified: Wed May 24 17:16:24 2023, max compression
+gzip compressed data, was "flordb-2.7.0.tar", last modified: Thu Jul 20 18:12:11 2023, max compression
```

## Comparing `flordb-2.6.4.tar` & `flordb-2.7.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.368499 flordb-2.6.4/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.4/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)     8299 2023-05-24 17:16:24.368264 flordb-2.6.4/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     7867 2023-05-24 17:15:50.000000 flordb-2.6.4/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.360337 flordb-2.6.4/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      281 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1779 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/__main__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/batch.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4416 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     6299 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.360918 flordb-2.6.4/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362059 flordb-2.6.4/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362175 flordb-2.6.4/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.362537 flordb-2.6.4/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.363531 flordb-2.6.4/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.4/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.364278 flordb-2.6.4/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.364895 flordb-2.6.4/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2116 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.365884 flordb-2.6.4/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.4/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.4/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.4/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.366497 flordb-2.6.4/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8042 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3721 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1752 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     9458 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.366775 flordb-2.6.4/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.4/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2558 2023-05-17 00:21:40.000000 flordb-2.6.4/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.4/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.367548 flordb-2.6.4/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.4/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.4/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.4/flor/state.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1078 2023-05-24 17:15:50.000000 flordb-2.6.4/flor/utils.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-24 17:16:24.368132 flordb-2.6.4/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8299 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-24 17:16:24.000000 flordb-2.6.4/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-24 17:16:24.368554 flordb-2.6.4/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-24 17:15:50.000000 flordb-2.6.4/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.739399 flordb-2.7.0/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.7.0/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)    19202 2023-07-20 18:12:11.739253 flordb-2.7.0/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)    18770 2023-07-20 17:48:12.000000 flordb-2.7.0/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.730409 flordb-2.7.0/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      281 2023-05-24 17:15:50.000000 flordb-2.7.0/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3100 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/__main__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.7.0/flor/batch.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6150 2023-07-03 18:24:51.000000 flordb-2.7.0/flor/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6481 2023-07-18 16:49:26.000000 flordb-2.7.0/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.731065 flordb-2.7.0/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4677 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732325 flordb-2.7.0/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6337 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3195 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-07-05 15:29:17.000000 flordb-2.7.0/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732458 flordb-2.7.0/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2955 2023-07-05 15:27:49.000000 flordb-2.7.0/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732895 flordb-2.7.0/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.733859 flordb-2.7.0/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.7.0/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.734627 flordb-2.7.0/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.735231 flordb-2.7.0/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4323 2023-07-05 15:27:49.000000 flordb-2.7.0/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2046 2023-07-05 15:30:58.000000 flordb-2.7.0/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.736065 flordb-2.7.0/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3518 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.7.0/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.7.0/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.736996 flordb-2.7.0/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9665 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3663 2023-07-05 15:29:55.000000 flordb-2.7.0/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1769 2023-07-05 15:30:42.000000 flordb-2.7.0/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2481 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9686 2023-07-20 17:21:04.000000 flordb-2.7.0/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.737401 flordb-2.7.0/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     5063 2023-07-19 21:03:15.000000 flordb-2.7.0/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.7.0/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.738514 flordb-2.7.0/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.7.0/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.7.0/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      913 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1078 2023-05-24 17:15:50.000000 flordb-2.7.0/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.739116 flordb-2.7.0/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    19202 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-07-20 18:12:11.739432 flordb-2.7.0/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-07-20 18:10:15.000000 flordb-2.7.0/setup.py
```

### Comparing `flordb-2.6.4/LICENSE` & `flordb-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/batch.py` & `flordb-2.7.0/flor/batch.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/constants.py` & `flordb-2.7.0/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/database.py` & `flordb-2.7.0/flor/database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sqlite3
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 from datetime import datetime
 
 from flor.shelf import home_shelf
 from flor.constants import *
 import math
 import random
 
@@ -66,59 +66,70 @@
         print(e)
         return None, None
     finally:
         cur.close()
 
 
 def server_completed(db_conn):
-    sql = """
-    UPDATE workers SET status = ? WHERE pid = ?;
-    """
     cur = db_conn.cursor()
     try:
+        # Step 1: Remove all occurrences of this worker in the pool table
         cur.execute(
-            sql,
-            (
-                "COMPLETED",
-                int(os.getpid()),
-            ),
+            "DELETE FROM pool WHERE pid = ?",
+            (int(os.getpid()),),
+        )
+
+        # Step 2: Update the workers table
+        cur.execute(
+            "UPDATE workers SET status = 'COMPLETED' WHERE pid = ?",
+            (int(os.getpid()),),
         )
+
+        # If all operations were successful, commit the changes
         db_conn.commit()
+
     except Exception as e:
         print(e)
+        # If an error occurred, roll back any changes
+        db_conn.rollback()
     finally:
         cur.close()
 
 
 def init_db(db_conn: sqlite3.Connection):
     """
     Initializes the database
     TODO: add GPU column to `workers`
     """
     cur = db_conn.cursor()
     cur.executescript(
         """
         BEGIN;
-        CREATE TABLE config(
-            name text,
-            value text
-        );
         CREATE TABLE workers(
             pid integer,
             tstamp text,
             gpu integer,
             status text
         );
         CREATE TABLE jobs(
             jobid integer,
             path text,
             script text,
             args text,
             done integer
         );
+        CREATE TABLE replay(
+            jobid integer,
+            path text,
+            script text,
+            vid text,
+            appvars text,
+            mode text, 
+            done integer
+        );
         CREATE TABLE pool(
             pid integer,
             tstamp text,
             jobid integer
         );
         COMMIT;
         """
@@ -142,47 +153,91 @@
         db_conn.commit()
     except Exception as e:
         print(e)
     finally:
         cur.close()
 
 
+def add_replay(
+    db_conn: sqlite3.Connection,
+    run_dir: str,
+    script: str,
+    vid_vars_mod: List[Any],
+):
+    cur = db_conn.cursor()
+    params = []
+    for vid, apply_vars, mode in vid_vars_mod:
+        params.append(
+            (random.randint(0, 999999999), run_dir, script, vid, apply_vars, mode, 0)
+        )
+    try:
+        cur.executemany("INSERT INTO replay VALUES (?, ?, ?, ?, ?, ?, ?)", params)
+        db_conn.commit()
+    except Exception as e:
+        print(e)
+        db_conn.rollback()
+    finally:
+        cur.close()
+
+
 def finish_job(db_conn: sqlite3.Connection, jobid):
     sql = """
     UPDATE jobs SET done = 1 WHERE jobid = ?
     """
     cur = db_conn.cursor()
     try:
         cur.execute(sql, (jobid,))
         db_conn.commit()
     except Exception as e:
         print(e)
     finally:
         cur.close()
 
 
+def finish_replay(db_conn: sqlite3.Connection, jobid):
+    cur = db_conn.cursor()
+    try:
+        cur.execute("UPDATE replay SET done = 1 WHERE jobid = ?", (jobid,))
+        db_conn.commit()
+    except Exception as e:
+        print(e)
+        db_conn.rollback()
+    finally:
+        cur.close()
+
+
 def step_worker(db_conn: sqlite3.Connection, pid, tstamp):
     sqls = [
         """
         SELECT jobid, path, script, args FROM jobs WHERE
             done = 0 AND
             jobid not in (SELECT jobid FROM pool)
             LIMIT 1;
         """,
         """
         INSERT INTO pool VALUES(?, ?, ?)
         """,
+        """
+        SELECT jobid, path, script, vid, appvars, mode FROM replay 
+          WHERE done = 0 AND jobid not in (SELECT jobid FROM pool) LIMIT 1;
+        """,
     ]
     cur = db_conn.cursor()
     try:
         res = cur.execute(sqls[0])
         if res is not None:
             for jobid, path, script, args in res.fetchall():
                 cur.execute(sqls[1], (pid, tstamp, jobid))
                 db_conn.commit()
-                return jobid, path, script, args
-        return None, None, None, None
+                return "jobs", (jobid, path, script, args)
+        res = cur.execute(sqls[2])
+        if res is not None:
+            for jobid, path, script, vid, apply_vars, mode in res.fetchall():
+                cur.execute(sqls[1], (pid, tstamp, jobid))
+                db_conn.commit()
+                return "replay", (jobid, path, script, vid, apply_vars, mode)
+        return None
     except Exception as e:
         print(e)
-        return None, None, None, None
+        return None
     finally:
         cur.close()
```

### Comparing `flordb-2.6.4/flor/flags.py` & `flordb-2.7.0/flor/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,21 @@
 
     def parse_remaining(self):
         skip = True
         for flg in [each for each in sys.argv if each[0:2] == "--"]:
             skip = False
             self.add_argument(flg)
         if not skip:
-            self.nsp, sys.argv[:] = self.parse_known_args()
+            _snapshot = list(sys.argv)
+            self.nsp, _ = self.parse_known_args()
+            sys.argv[:] = _snapshot
+        elif REPLAY:
+            # TODO: Replay case, load CLI from .flor/.replay.json
+            pass
+            
 
 
 parser = CLI_Args()
 
 
 def is_interactive():
     try:
```

### Comparing `flordb-2.6.4/flor/hlast/__init__.py` & `flordb-2.7.0/flor/hlast/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import ast
 from argparse import Namespace
 from os import PathLike
 from shutil import copyfile
 from pathlib import Path, PurePath
 from sys import stdout
 from typing import Dict, List, Set
+import pandas as pd
+import os
 
 from flor.hlast.gtpropagate import propagate, LogLinesVisitor  # type: ignore
 from flor.state import State
 import flor.query as q
 from .visitors import LoggedExpVisitor, NoGradVisitor, NoGradTransformer
 
 
@@ -53,62 +55,82 @@
             else:
                 super().generic_visit(node)
         else:
             super().generic_visit(node)
 
 
 def apply(names: List[str], dst: str):
+    """
+    Caller checks out a previous version
+    """
+
     fp = Path(dst)
     facts = q.log_records(skip_unpack=True)
+
     # Get latest timestamp for each variable name
-    valid_names = facts[facts["name"].isin(names)][["name", "tstamp", "vid", "value"]]
-    valid_names = valid_names[valid_names["value"].notna()]
-    name2tstamp = valid_names[["name", "tstamp", "vid"]].drop_duplicates()
+    historical_names = facts[facts["name"].isin(names)][
+        ["name", "tstamp", "vid", "value"]
+    ]
+    historical_names = historical_names[historical_names["value"].notna()]
+    hist_name2tstamp = historical_names[["name", "tstamp", "vid"]].drop_duplicates()
 
-    stash = q.clear_stash()
+    stash = q.get_stash()
     assert stash is not None
     assert State.repo is not None
     copyfile(fp, stash / fp)
-    hits: Set[str] = set([])
-    grouped_names: Dict[str, int] = {}
 
-    for _, row in name2tstamp.iterrows():
+    for _, row in hist_name2tstamp.iterrows():
+        if len(State.hls_hits) == len(names):
+            break
         n = row["name"]
         v = row["vid"]
         State.repo.git.checkout(v, "--", fp)
         lev = LoggedExpVisitor()
         with open(fp, "r") as f:
             lev.visit(ast.parse(f.read()))
         if n in lev.names:
-            grouped_names[n] = lev.names[n]
-            hits.add(n)
-            copyfile(src=fp, dst=stash / PurePath(n).with_suffix(".py"))
-        if len(hits) == len(names):
-            break
+            State.grouped_names[n] = lev.names[n]
+            State.hls_hits.add(n)
+            copyfile(src=fp, dst=stash / Path(n).with_suffix(".py"))
 
     copyfile(stash / fp, fp)
-    assert len(hits) == len(
+
+    for p in os.listdir(stash):
+        State.hls_hits.add(".".join(p.split(".")[0:-1]))
+
+    assert len(os.listdir(stash)) > len(
         names
-    ), f"Failed to find log statement for vars {[n for n in names if n not in hits]}"
+    ), f"Failed to find log statement for vars {[n for n in names if n not in State.hls_hits]}"
 
     # Next, from the stash you will apply each file to our main one
     parse_noGrad = []
     for name in names:
-        with open(stash / PurePath(name).with_suffix(".py"), "r") as f:
+        with open(stash / Path(name).with_suffix(".py"), "r") as f:
             tree = ast.parse(f.read())
 
         ng_visitor = NoGradVisitor()
         ng_visitor.visit(tree)
+
         if name not in ng_visitor.names:
-            lineno = int(grouped_names[name])
+            if name in State.grouped_names:
+                lineno = int(State.grouped_names[name])
+            else:
+                lev = LoggedExpVisitor()
+                lev.visit(tree)
+                lineno = int(lev.names[name])
             # lev possibly unbound
-            backprop(lineno, str(stash / PurePath(name).with_suffix(".py")), dst)
+            backprop(
+                lineno,
+                str(stash / Path(name).with_suffix(".py")).replace("\x1b[m", ""),
+                dst,
+            )
             print(f"Applied {name} to {dst}")
         else:
             parse_noGrad.append(ng_visitor.tree)
+            print(f"Applied {name} to {dst}")
 
     if len(parse_noGrad) > 1:
         raise NotImplementedError(
             "TODO: Will need to merge code blocks, union of logging statements"
         )
     elif len(parse_noGrad) == 1:
         their_tree = parse_noGrad[0]
```

### Comparing `flordb-2.6.4/flor/hlast/gtpropagate.py` & `flordb-2.7.0/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/__init__.py` & `flordb-2.7.0/flor/hlast/gumtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 from apted import APTED, Config
 from itertools import product, zip_longest
 from collections.abc import Iterable
 from typing import Generic, Optional, TypeVar
 from bidict._mut import MutableBidict
 
 from .adapter import Adapter
```

### Comparing `flordb-2.6.4/flor/hlast/gumtree/adapter.py` & `flordb-2.7.0/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/idmap.py` & `flordb-2.7.0/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/priorityq.py` & `flordb-2.7.0/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/python.py` & `flordb-2.7.0/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/test.py` & `flordb-2.7.0/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/gumtree/tree.py` & `flordb-2.7.0/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/hlast/visitors.py` & `flordb-2.7.0/flor/hlast/visitors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,54 @@
-from typing import Dict
+from typing import Any, Dict
 import ast
 
-
 class LoggedExpVisitor(ast.NodeVisitor):
     def __init__(self):
         super().__init__()
         self.names: Dict[str, int] = {}
+        self.loglevels: Dict[str, int] = {}
+        
+        self.lvl = 0 
+
+    def get_loglevel(self, filtered_keys):
+        i = max({k:self.loglevels[k] for k in (filtered_keys if filtered_keys is not None else self.loglevels)}.values())
+        if i == 0:
+            return "DATA_PREP"
+        elif i == 1:
+            return "OUTR_LOOP"
+        elif i >= 2:
+            return "INNR_LOOP"
+        raise
+
+    def visit_For(self, node: ast.For):
+        iter_s = ast.unparse(node.iter).strip()
+        if 'Flor.loop' == iter_s[0:len('Flor.loop')] or 'MTK.loop' == iter_s[0:len('MTK.loop')]:
+            start_lvl = self.lvl
+            try:
+                self.lvl += 1
+                tree = self.generic_visit(node)
+            finally:
+                self.lvl = start_lvl
+        else:
+            tree = self.generic_visit(node)
+        return tree
 
     def visit_Call(self, node: ast.Call):
         pred = (
             isinstance(node.func, ast.Attribute)
             and isinstance(node.func.value, ast.Name)
             and node.func.value.id == "flor"
             and node.func.attr == "log"
         )
         if not pred:
             return self.generic_visit(node)
         if len(node.args) == 2 and isinstance(node.args[0], ast.Constant):
-            self.names[str(node.args[0].value)] = node.lineno
+            n = str(node.args[0].value)
+            self.names[n] = node.lineno
+            self.loglevels[n] = self.lvl
         else:
             raise IndexError("FLOR: Did you give flor.log a key? It takes 2 args.")
 
 
 class NoGradVisitor(ast.NodeVisitor):
     def __init__(self):
         super().__init__()
```

### Comparing `flordb-2.6.4/flor/iterator.py` & `flordb-2.7.0/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/__init__.py` & `flordb-2.7.0/flor/journal/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
     def get_segment_window(self) -> List[Capsule]:
         assert flags.PID.ngpus <= self.tree.iterations_count
         if self.tree.sparse_checkpoints:
             assert (
                 flags.PID.ngpus <= len(self.tree.sparse_checkpoints) + 1
             ), f"Not enough checkpoints. Max degree of parallelism: {len(self.tree.sparse_checkpoints) + 1}"
-        if flags.MODE is REPLAY_MODE.weak and flags.PID.pid >= 0:
+        if flags.MODE is REPLAY_MODE.weak and flags.PID.pid != 1:
             self._advance_head()
             assert self.sub_tree is not None
             return self.sub_tree.get_segment()
         return self.tree.get_segment()
 
     def get_iterations_count(self):
-        return exp_json.get("EPOCHS")
+        return self.as_tree().iterations_count
 
     def as_tree(self) -> Tree:
         if (
             not flags.REPLAY
             or flags.MODE is REPLAY_MODE.strong
             or (flags.PID.pid == 1 and flags.PID.ngpus == 1)
         ):
```

### Comparing `flordb-2.6.4/flor/journal/entry/__init__.py` & `flordb-2.7.0/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/abstract.py` & `flordb-2.7.0/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/data/abstract.py` & `flordb-2.7.0/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/data/dataframe.py` & `flordb-2.7.0/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/data/reference.py` & `flordb-2.7.0/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.7.0/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/data/value.py` & `flordb-2.7.0/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/metadata/bracket.py` & `flordb-2.7.0/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/entry/metadata/eof.py` & `flordb-2.7.0/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/tree/block.py` & `flordb-2.7.0/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/tree/group.py` & `flordb-2.7.0/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/tree/tree.py` & `flordb-2.7.0/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/journal/tree/window.py` & `flordb-2.7.0/flor/journal/tree/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Union, Optional
 
 NO_INIT = None
 
 
 class Window:
     def __init__(self, iterations_count: int, sparse_checkpoints: List[int]):
-        self.iterations_count = exp_json.get("EPOCHS")
+        self.iterations_count = iterations_count
         self.extended_sparse_checkpoints: List[Optional[int]] = list(sparse_checkpoints)
         self.extended_sparse_checkpoints.insert(0, NO_INIT)
 
     def get_work_segment(self):
         if self._is_sparse():
             # Only a subset of epochs are valid entries
             # Only weak initialization is possible
@@ -110,7 +110,10 @@
         return pred_epoch
 
 
 class Capsule:
     def __init__(self, init_only: bool, epoch: Optional[int]):
         self.init_only = init_only
         self.epoch = epoch
+
+    def __str__(self) -> str:
+        return f"init_only: {self.init_only}, epoch: {self.epoch}"
```

### Comparing `flordb-2.6.4/flor/kits.py` & `flordb-2.7.0/flor/kits.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,22 +32,22 @@
             name = str(static_id) if name is None else name
             if State.loop_nesting_level == 1:
                 # Outer loop
                 assert State.import_time is not None
                 State.seconds["PREP"] = time() - State.import_time
                 State.seconds["EPOCHS"] = []
                 State.epoch = 0
-                State.seconds["EVAL"] = time()
+
                 for each in it(iter8r):
                     start_time = time()
                     State.step = 0
                     State.epoch += 1
                     yield each
                     State.seconds["EPOCHS"].append(time() - start_time)
-                State.seconds["EVAL"] = time() - State.seconds["EVAL"]
+                State.seconds["EVAL"] = time()
             else:
                 assert State.loop_nesting_level > 1
                 # Nested loop
                 if SkipBlock.step_into(name, probed):
                     assert State.step is not None
                     try:
                         while True:
```

### Comparing `flordb-2.6.4/flor/logger/__init__.py` & `flordb-2.7.0/flor/logger/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from copy import deepcopy
 import json
 
 
 from flor.logger import exp_json, log_records
 from flor.state import State
 from flor import flags
+from flor.constants import *
 
 
 def log(name, value) -> Any:
     def is_jsonable(x):
         try:
             json.dumps(x)
             return True
@@ -23,27 +24,58 @@
         log_records.put(name, serializable_value)
     else:
         exp_json.put(name, serializable_value, ow=False)
     return value
 
 
 def arg(name, default=None) -> Any:
-    #
-    # calls log(name, default)
+    historical_args = None
+    if flags.NAME and flags.REPLAY:
+        with open(REPLAY_JSON, "r") as f:
+            d = json.load(f)
+            if "CLI" in d:
+                historical_args = d["CLI"]
     if default is None:
-        if name in vars(flags.parser.nsp):
-            v = getattr(flags.parser.nsp, name)
-            # CLI is logged by EXP_JSON
-            return v
+        if historical_args is None or name not in historical_args:
+            if name in vars(flags.parser.nsp):
+                v = getattr(flags.parser.nsp, name)
+                # CLI is logged by EXP_JSON
+                return v
+            else:
+                raise RuntimeError(f"Args without defaults need CLI input: {name}")
         else:
-            raise RuntimeError(f"Args without defaults need CLI input: {name}")
+            return historical_args[name]
     else:
-        if name in vars(flags.parser.nsp):
-            # CLI takes precedence over default
-            v = getattr(flags.parser.nsp, name)
+        if historical_args is None or name not in historical_args:
+            if name in vars(flags.parser.nsp):
+                # CLI takes precedence over default
+                v = getattr(flags.parser.nsp, name)
+                if isinstance(default, bool):
+                    return bool(v)
+                if isinstance(default, int):
+                    return int(v)
+                elif isinstance(default, float):
+                    return float(v)
+                elif isinstance(default, str):
+                    return str(v) if v else ""
+                elif isinstance(default, list):
+                    return list(v) if v else []
+                elif isinstance(default, tuple):
+                    return tuple(v) if v else tuple([])
+                elif isinstance(default, bytes):
+                    return bytes(v)
+                elif isinstance(default, bytearray):
+                    return bytearray(v)
+                else:
+                    raise TypeError(f"Unsupported type: {type(default)}")
+            else:
+                log(name, default)
+                return default
+        else:
+            v = historical_args[name]
             if isinstance(default, bool):
                 return bool(v)
             if isinstance(default, int):
                 return int(v)
             elif isinstance(default, float):
                 return float(v)
             elif isinstance(default, str):
@@ -54,17 +86,14 @@
                 return tuple(v) if v else tuple([])
             elif isinstance(default, bytes):
                 return bytes(v)
             elif isinstance(default, bytearray):
                 return bytearray(v)
             else:
                 raise TypeError(f"Unsupported type: {type(default)}")
-        else:
-            log(name, default)
-            return default
 
 
 def pinned(name, callback, *args) -> Any:
     if not flags.REPLAY:
         value = callback(*args)
         if flags.NAME:
             exp_json.put(name, value, ow=False)
```

### Comparing `flordb-2.6.4/flor/logger/checkpoint_logger.py` & `flordb-2.7.0/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/logger/exp_json.py` & `flordb-2.7.0/flor/logger/exp_json.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/logger/future.py` & `flordb-2.7.0/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/logger/log_records.py` & `flordb-2.7.0/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/query/__init__.py` & `flordb-2.7.0/flor/query/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-import csv
-from typing import List, Set, Dict
+import ast
+from typing import List, Optional, Set, Dict
 import pandas as pd
 import numpy as np
 from flor.shelf import home_shelf, cwd_shelf
-from flor.query.unpack import unpack, clear_stash
+from flor.query.unpack import unpack, clear_stash, get_stash
 from flor.query import database
+
 from flor.shelf import cwd_shelf
 from pathlib import Path
 from IPython.display import display
 
 from flor.query.pivot import *
 from flor.query.engine import *
 from flor.constants import *
 from flor.state import State
 
-import math
+from flor.hlast.visitors import LoggedExpVisitor
+from shutil import copyfile
+
 
 pivot_vars: Dict[str, Set[str]] = {
     "DATA_PREP": set([]),
     "OUTR_LOOP": set([]),
     "INNR_LOOP": set([]),
 }
 
@@ -46,49 +49,57 @@
                 "value",
             ],
         )
         .astype(
             {
                 "projid": str,
                 "runid": str,
-                "tstamp": "datetime64[ns]",
+                "tstamp": str,
                 "vid": str,
                 "epoch": int,
                 "step": int,
                 "name": str,
                 "value": object,
             }
         )
         .sort_values(by=["tstamp", "epoch", "step"])
     )
+    facts["projid"] = facts["projid"].map(lambda x: x.replace("\x1b[m", ""))
     return facts
 
 
 def full_pivot(facts: pd.DataFrame):
     data_prep_gb = facts.drop_duplicates()[list(DATA_PREP) + ["name", "value"]].groupby(
         by=list(DATA_PREP + ("name",))
     )
+
+    skip_set = set([])
     for rowid, agg in data_prep_gb.count()["value"].items():
         name = str(tuple(rowid)[-1])  # type: ignore
-        if agg == 1:
+        if agg == 1 and name not in skip_set:
             pivot_vars["DATA_PREP"] |= {
                 name,
             }
+        else:
+            skip_set.add(name)
 
     outer_loop_gb = (
         facts[list(OUTR_LOOP) + ["name", "value"]]
         .drop_duplicates()
         .groupby(by=list(OUTR_LOOP + ("name",)))
     )
+    skip_set = set([])
     for rowid, agg in outer_loop_gb.count()["value"].items():
         name = str(tuple(rowid)[-1])  # type: ignore
-        if name not in pivot_vars["DATA_PREP"] and agg == 1:
+        if name not in pivot_vars["DATA_PREP"] and agg == 1 and name not in skip_set:
             pivot_vars["OUTR_LOOP"] |= {
                 name,
             }
+        else:
+            skip_set.add(name)
 
     pivot_vars["INNR_LOOP"] |= set(
         [
             name
             for name in facts["name"]
             if name not in pivot_vars["DATA_PREP"]
             and name not in pivot_vars["OUTR_LOOP"]
@@ -124,65 +135,107 @@
         return post_proc(dp_pivot, dp_keys)
     elif ol_pivot is not None:
         return post_proc(ol_pivot, ol_keys)
     elif il_pivot is not None:
         return post_proc(il_pivot, all_keys)
 
 
-def replay(apply_vars: List[str], where_clause: str, path: str):
+def replay(
+    apply_vars: List[str], where_clause: Optional[str] = None, path: str = "train.py"
+):
     """
     apply_vars : ['device', 'optimizer', 'learning_rate', ...]
     where_clause: stated in Pandas/SQL, passed to full_pivot
     path: `train_rnn.py` or such denoting main python script
     """
     assert Path(path).suffix == ".py"
     facts = log_records(skip_unpack=True)
     df = full_pivot(facts)
     assert df is not None
-    assert all([v in facts["name"].values for v in apply_vars])
+
+    stash = clear_stash()
+    assert stash is not None
+
+    with open(path, "r") as f:
+        tree = ast.parse(f.read())
+    lev = LoggedExpVisitor()
+    lev.visit(tree)
+
+    vars_in_latest = []
+    for var in apply_vars:
+        if var not in facts["name"].values:
+            assert (
+                var in lev.names
+            ), f"FLOR: could not find logged var `{var}` in any version of `{path}`."
+            copyfile(path, stash / Path(var).with_suffix(".py"))
+            vars_in_latest.append(var)
+            State.hls_hits.add(var)
+            State.grouped_names[var] = lev.names[var]
+
+    for var in vars_in_latest:
+        # find where in source code
+        # Prompt the user
+        # TODO: Infer which one with fast static analysis.
+        msg = input(
+            f"What is the log level of logging statement `{var}`? Leave blank to infer `{lev.get_loglevel([var,])}`: "
+        )
+        msg = msg.strip().upper()
+        if msg in pivot_vars:
+            pivot_vars[msg].add(var)
+        elif msg == "" or not msg:
+            pivot_vars[
+                lev.get_loglevel(
+                    [
+                        var,
+                    ]
+                )
+            ].add(var)
+        else:
+            raise
 
     loglvl = get_dims(pivot_vars, apply_vars)
     dp_schedule = (
-        df.query(where_clause)[list(DATA_PREP)]
+        (df.query(where_clause) if where_clause is not None else df)[list(DATA_PREP)]
         .drop_duplicates()
         .merge(
             pd.DataFrame(database.get_schedule(DATA_PREP)).astype(
                 {
                     "projid": str,
                     "runid": str,
-                    "tstamp": "datetime64[ns]",
+                    "tstamp": str,
                     "vid": str,
                     "prep_secs": float,
                     "eval_secs": float,
                 }
             ),
             how="inner",
             on=DATA_PREP,
         )[list(DATA_PREP) + ["prep_secs", "eval_secs"]]
     )
     if loglvl == DATA_PREP:
         versions = dp_schedule["vid"].drop_duplicates()
         display(dp_schedule)
-        print(
-            f"Continue replaying {len(versions)} versions at DATA_PREP level for {'{:.2f}'.format(3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs']))} seconds?"
+        res = input(
+            f"Continue replaying {len(versions)} versions at DATA_PREP level for {'{:.2f}'.format(3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs']))} seconds?[Y/n]? "
         )
-        res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, DATA_PREP)
     elif loglvl == OUTR_LOOP:
         size_bytes = home_shelf.get_checkpoint_bytes_per_epoch(cwd_shelf.get_projid())
         schedule = (
-            df.query(where_clause)[list(OUTR_LOOP)]
+            (df.query(where_clause) if where_clause is not None else df)[
+                list(OUTR_LOOP)
+            ]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": "datetime64[ns]",
+                        "tstamp": str,
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -192,30 +245,31 @@
                     "seconds",
                 ]
             ]
         )
         schedule["seconds"] = size_bytes * DESERIALIZATION_COEFF
         versions = schedule["vid"].drop_duplicates()
         display(schedule)
-        print(
-            f"Continue replaying {len(versions)} versions at OUTR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds?"
+        res = input(
+            f"Continue replaying {len(versions)} versions at OUTR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds [Y/n]? "
         )
-        res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, OUTR_LOOP)
     elif loglvl == INNR_LOOP:
         schedule = (
-            df.query(where_clause)[list(OUTR_LOOP)]
+            (df.query(where_clause) if where_clause is not None else df)[
+                list(OUTR_LOOP)
+            ]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": "datetime64[ns]",
+                        "tstamp": str,
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -224,18 +278,17 @@
                 + [
                     "seconds",
                 ]
             ]
         )
         versions = schedule["vid"].drop_duplicates()
         display(schedule)
-        print(
-            f"Continue replaying {len(versions)} versions at INNR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds?"
+        res = input(
+            f"Continue replaying {len(versions)} versions at INNR_LOOP level for {'{:.2f}'.format((3 * len(versions) + sum(dp_schedule['prep_secs']) + sum(dp_schedule['eval_secs'])) + sum(schedule['seconds']))} seconds [Y/n]? "
         )
-        res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, INNR_LOOP)
     else:
         raise
 
 
-__all__ = ["log_records", "full_pivot", "clear_stash", "replay"]
+__all__ = ["log_records", "full_pivot", "clear_stash", "get_stash", "replay"]
```

### Comparing `flordb-2.6.4/flor/query/database.py` & `flordb-2.7.0/flor/query/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 def exists():
     return dbp is not None and dbp.exists()
 
 
 def start_db(projid: str):
     global dbp
-    # print('projid', projid)
     dir_n = "_".join(projid.split("_")[0:-1])
-    # print('dir_n', dir_n)
     dbp = home_shelf.florin / Path(dir_n).with_suffix(SUFFIX)
     is_first_start = not dbp.exists()
     assert State.db_conn is None, "Did you try to start_db more than once?"
     State.db_conn = sqlite3.connect(dbp)
     if is_first_start:
         init_db()
```

### Comparing `flordb-2.6.4/flor/query/pivot.py` & `flordb-2.7.0/flor/query/pivot.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,11 +65,9 @@
         if rolling_dataframe is None:
             rolling_dataframe = pivot_f
         else:
             rolling_dataframe = rolling_dataframe.merge(
                 pivot_f, how="outer", on=list(INNR_LOOP)
             )
     if rolling_dataframe is not None:
-        rolling_dataframe = rolling_dataframe.drop_duplicates(
-            subset=list(INNR_LOOP)
-        )
+        rolling_dataframe = rolling_dataframe.drop_duplicates(subset=list(INNR_LOOP))
         return rolling_dataframe
```

### Comparing `flordb-2.6.4/flor/query/unpack.py` & `flordb-2.7.0/flor/query/unpack.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,31 @@
 import os
 import shutil
 import json
 import csv
 import pandas as pd
 
 
+def get_stash():
+    projid = cwd_shelf.get_projid()
+    projid = str(projid).replace("\x1b[m", "")
+    out = Path.home() / ".flor" / projid / "stash"
+    return out
+
+
 def clear_stash():
     global stash
+
+    projid = cwd_shelf.get_projid()
+    projid = str(projid).replace("\x1b[m", "")
+
     (Path.home() / ".flor").mkdir(exist_ok=True)
-    (Path.home() / ".flor" / cwd_shelf.get_projid()).mkdir(exist_ok=True)
-    stash = Path.home() / ".flor" / cwd_shelf.get_projid() / "stash"
+
+    (Path.home() / ".flor" / projid).mkdir(exist_ok=True)
+    stash = ((Path.home() / ".flor") / projid) / "stash"
     if stash.exists():
         shutil.rmtree(stash)
     stash.mkdir()
     return stash
 
 
 def filtered_versions():
@@ -64,15 +76,15 @@
     active_branch = State.active_branch
     try:
         commits = filtered_versions()
         for version in commits["RECORD"]:
             if wmrk is not None and version.hexsha in wmrk:
                 break
             try:
-                print(f"STEPPING IN {version.hexsha}")
+                # print(f"STEPPING IN {version.hexsha}")
                 r.git.checkout(version)
                 cp_seconds(version)
                 cp_log_records(version)
             except Exception as e:
                 print("Line Exception", e)
     finally:
         r.git.checkout(active_branch)
```

### Comparing `flordb-2.6.4/flor/shelf/home_shelf.py` & `flordb-2.7.0/flor/shelf/home_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/skipblock/abstract.py` & `flordb-2.7.0/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/skipblock/readblock.py` & `flordb-2.7.0/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/skipblock/writeblock.py` & `flordb-2.7.0/flor/skipblock/writeblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flor/state.py` & `flordb-2.7.0/flor/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,12 +9,23 @@
     epoch: Optional[int] = None
     step: Optional[int] = None
     timestamp: Optional[str] = None
     repo: Optional[Repo] = None
     common_dir: Optional[Path] = None
     active_branch: Optional[str] = None
     db_conn: Optional[sqlite3.Connection] = None
+
     import_time: Optional[float] = None
     seconds: Dict[str, Optional[Union[float, List[float]]]] = {
         "PREP": None,
     }  # May add "EPOCHS" at runtime
     target_block = None
+    
+    hls_hits = set([]) # hindsight logging stmt hits
+    grouped_names: Dict[str, int] = {}
+
+    @staticmethod
+    def get_vid():
+        if State.repo is not None:
+            for v in State.repo.iter_commits():
+                if str(v.message).count("RECORD::") == 1:
+                    return v.hexsha
```

### Comparing `flordb-2.6.4/flor/utils.py` & `flordb-2.7.0/flor/utils.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/flordb.egg-info/SOURCES.txt` & `flordb-2.7.0/flordb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flordb-2.6.4/setup.py` & `flordb-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.6.4",
+    version="2.7.0",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
```

