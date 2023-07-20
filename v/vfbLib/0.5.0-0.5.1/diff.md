# Comparing `tmp/vfbLib-0.5.0.tar.gz` & `tmp/vfbLib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfbLib-0.5.0.tar", last modified: Tue Jul 18 14:58:12 2023, max compression
+gzip compressed data, was "vfbLib-0.5.1.tar", last modified: Thu Jul 20 12:07:18 2023, max compression
```

## Comparing `vfbLib-0.5.0.tar` & `vfbLib-0.5.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-18 14:58:02.000000 vfbLib-0.5.0/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 14:58:02.000000 vfbLib-0.5.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.854471 vfbLib-0.5.0/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/cu2qu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/mm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/templates/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/Lib/vfbLib/ufo/
--rw-r--r--   0 runner    (1001) docker     (123)    29773 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/designspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/kerning.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/pshints.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/tth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/vfb2ufo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/value.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/Lib/vfbLib/vfb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/vfb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-18 14:58:12.862471 vfbLib-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-18 14:58:02.000000 vfbLib-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 14:58:02.000000 vfbLib-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-18 14:58:12.862471 vfbLib-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-18 14:58:02.000000 vfbLib-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.191898 vfbLib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-20 12:07:04.000000 vfbLib-0.5.1/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 12:07:04.000000 vfbLib-0.5.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.175898 vfbLib-0.5.1/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.179898 vfbLib-0.5.1/Lib/vfbLib/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.183898 vfbLib-0.5.1/Lib/vfbLib/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/compilers/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/cu2qu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.183898 vfbLib-0.5.1/Lib/vfbLib/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/mm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/parsers/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.187898 vfbLib-0.5.1/Lib/vfbLib/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/templates/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.187898 vfbLib-0.5.1/Lib/vfbLib/ufo/
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/kerning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/pshints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/tth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/ufo/vfb2ufo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.191898 vfbLib-0.5.1/Lib/vfbLib/vfb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/pens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-20 12:07:04.000000 vfbLib-0.5.1/Lib/vfbLib/vfb/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:18.179898 vfbLib-0.5.1/Lib/vfbLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:17.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 12:07:18.000000 vfbLib-0.5.1/Lib/vfbLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-20 12:07:18.191898 vfbLib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 12:07:04.000000 vfbLib-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 12:07:04.000000 vfbLib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-20 12:07:18.191898 vfbLib-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-20 12:07:04.000000 vfbLib-0.5.1/setup.py
```

### Comparing `vfbLib-0.5.0/DESCRIPTION.md` & `vfbLib-0.5.1/DESCRIPTION.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 Generate a representation that closely adheres to the VFB structure.
 
 ```bash
 $ vfb2json MyFile.vfb
 ```
 
-will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
+will convert the file to `MyFile.vfb.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
 usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/cmdline.py` & `vfbLib-0.5.1/Lib/vfbLib/cmdline.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,22 @@
 
 import codecs
 import json
 import logging
 
 from argparse import ArgumentParser
 from pathlib import Path
-from vfbLib.reader import VFBReader
 from vfbLib.ufo import VfbToUfoBuilder
 from vfbLib.version import build_date
 from vfbLib.vfb.vfb import Vfb
 
 
 logger = logging.getLogger(__name__)
 
 
-def read_vfb(vfb_path: Path, minimal=False) -> VFBReader:
-    reader = VFBReader(vfb_path, minimal=minimal)
-    reader.read()
-    return reader
-
-
-def write_json(reader: VFBReader, json_path: Path) -> None:
-    with codecs.open(str(json_path), "wb", "utf-8") as f:
-        json.dump(reader.data, f, ensure_ascii=False, indent=4)
-
-
 def vfb2json():
     parser = ArgumentParser(
         description=(
             f"VFB2JSON Converter\nCopyright (c) 2023 by LucasFonts\nBuild {build_date}"
         )
     )
     parser.add_argument(
@@ -56,25 +44,37 @@
         "-p",
         "--path",
         type=str,
         nargs=1,
         help="output folder",
     )
     parser.add_argument(
+        "-u",
+        "--unicode-strings",
+        action="store_true",
+        default=False,
+        help="interpret name table strings as Unicode instead of Windows-1252",
+    )
+    parser.add_argument(
         "inputpath",
         type=str,
         nargs=1,
         help="input file path (.vfb)",
     )
     args = parser.parse_args()
     if args:
         vfb_path = Path(args.inputpath[0])
         print(parser.description)
         print(f"Reading file {vfb_path} ...")
-        vfb = Vfb(vfb_path, only_header=args.header, minimal=args.minimal)
+        vfb = Vfb(
+            vfb_path,
+            only_header=args.header,
+            minimal=args.minimal,
+            unicode_strings=args.unicode_strings,
+        )
         if not args.no_decompile:
             vfb.decompile()
         suffix = ".vfb.json"
         if args.path:
             out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(suffix)
         else:
             out_path = vfb_path.with_suffix(suffix)
@@ -154,22 +154,32 @@
     parser.add_argument(
         "-m",
         "--minimal",
         action="store_true",
         default=False,
         help="parse only minimal amount of data, drop missing glyphs from groups, etc.",
     )
+    parser.add_argument(
+        "-u",
+        "--unicode-strings",
+        action="store_true",
+        default=False,
+        help="interpret name table strings as Unicode instead of Windows-1252",
+    )
     args = parser.parse_args()
     if args:
         vfb_path = Path(args.inputpath[0])
         if not args.silent:
             print(parser.description)
             print(f"Reading file {vfb_path} ...")
         vfb = Vfb(
-            vfb_path, minimal=args.minimal, drop_keys={"Encoding", "Encoding Mac"}
+            vfb_path,
+            minimal=args.minimal,
+            drop_keys={"Encoding", "Encoding Mac"},
+            unicode_strings=args.unicode_strings,
         )
         suffix = ".ufo"
         if args.zip:
             suffix += "z"
         if args.path:
             out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(suffix)
         else:
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/compilers/glyph.py` & `vfbLib-0.5.1/Lib/vfbLib/compilers/glyph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from io import BytesIO
 from math import radians, tan
 from struct import pack
-from typing import Any, Tuple
+from typing import Any, List, Tuple
 from vfbLib import GLYPH_CONSTANT
 from vfbLib.compilers import BaseCompiler
 from vfbLib.truetype import TT_COMMAND_CONSTANTS, TT_COMMANDS
 
 import logging
 
 
@@ -20,212 +20,224 @@
     "curve": 3,
     "qcurve": 4,
 }
 
 
 class GlyphCompiler(BaseCompiler):
     @classmethod
-    def _compile_binary(cls, data):
+    def merge(cls, masters_data: List[Any], data: Any) -> None:
+        num_masters = len(masters_data)
+        if num_masters < 2:
+            return
+
+        for m in range(1, num_masters):
+            master_data = masters_data[m]
+            # See if there is any data to merge
+            if "nodes" in master_data:
+                assert "nodes" in data
+                for i, tgt in enumerate(data["nodes"]):
+                    src = master_data["nodes"][i]
+                    for key in ("type", "flags"):
+                        assert src[key] == tgt[key]
+                    tgt["points"][m] = src["points"][m]
+
+            if "components" in master_data:
+                assert "components" in data
+                for i, tgt in enumerate(data["components"]):
+                    src = master_data["components"][i]
+                    for key in ("gid",):
+                        assert src[key] == tgt[key]
+                    tgt["offsetX"][m] = src["offsetX"][m]
+                    tgt["offsetY"][m] = src["offsetY"][m]
+                    tgt["scaleX"][m] = src["scaleX"][m]
+                    tgt["scaleY"][m] = src["scaleY"][m]
+
+    def _compile_binary(self, data):
         # Imported binary data 8-)
         if not (imported := data.get("imported")):
             return
 
         logger.warning("Compiling imported binary data is not supported.")
         return
 
-        cls.write_uint1(9)
+        self.write_uint1(9)
 
-    @classmethod
-    def _compile_components(cls, data):
+    def _compile_components(self, data):
         # Components
         if not (components := data.get("components")):
             return
 
-        cls.write_uint1(5)
-        cls.write_encoded_value(len(components))
+        self.write_uint1(5)
+        self.write_encoded_value(len(components))
         for component in components:
-            cls.write_encoded_value(component["gid"])
-            for i in range(cls.num_masters):
-                cls.write_encoded_value(component["offsetX"][i])
-                cls.write_encoded_value(component["offsetY"][i])
-                cls.write_float(component["scaleX"][i])
-                cls.write_float(component["scaleY"][i])
+            self.write_encoded_value(component["gid"])
+            for i in range(self.num_masters):
+                self.write_encoded_value(component["offsetX"][i])
+                self.write_encoded_value(component["offsetY"][i])
+                self.write_float(component["scaleX"][i])
+                self.write_float(component["scaleY"][i])
 
-    @classmethod
-    def _compile_glyph_name(cls, data):
+    def _compile_glyph_name(self, data):
         # Glyph name
         if not (name := data.get("name")):
             return
 
         glyph_name = name.encode("cp1252")
         glyph_name_length = len(glyph_name)
-        cls.write_uint1(1)
-        cls.write_encoded_value(glyph_name_length)
-        cls.write_bytes(glyph_name)
+        self.write_uint1(1)
+        self.write_encoded_value(glyph_name_length)
+        self.write_bytes(glyph_name)
+        logger.debug(f"Compiling glyph '{name}'")
 
-    @classmethod
-    def _compile_guides(cls, data):
+    def _compile_guides(self, data):
         # Guidelines
         # TODO: Reuse for global guides
         if not (guides := data.get("guides")):
             return
 
-        cls.write_uint1(4)
+        self.write_uint1(4)
         for direction in ("h", "v"):
-            direction_guides = guides.get(direction, [])
-            cls.write_encoded_value(len(direction_guides))
-            for m in range(cls.num_masters):
+            direction_guides = guides.get(direction)
+            if direction_guides is None:
+                self.write_encoded_value(0)
+                continue
+
+            self.write_encoded_value(len(direction_guides[0]))  # first master
+            for m in range(self.num_masters):
                 for guide in direction_guides[m]:
                     pos = guide["pos"]
                     angle = round(tan(radians(guide["angle"])) * 10000)
-                    cls.write_encoded_value(pos)
-                    cls.write_encoded_value(angle)
+                    self.write_encoded_value(pos)
+                    self.write_encoded_value(angle)
 
-    @classmethod
-    def _compile_hints(cls, data):
+    def _compile_hints(self, data):
         # PostScript hints
         if not (hints := data.get("hints")):
             return
 
-        cls.write_uint1(3)
+        self.write_uint1(3)
         for direction in ("h", "v"):
             if direction_hints := hints.get(direction):
-                cls.write_encoded_value(len(direction_hints))
+                self.write_encoded_value(len(direction_hints))
                 for mm_hint in direction_hints:
-                    for i in range(cls.num_masters):
+                    for i in range(self.num_masters):
                         hint = mm_hint[i]
-                        cls.write_encoded_value(hint["pos"])
-                        cls.write_encoded_value(hint["width"])
+                        self.write_encoded_value(hint["pos"])
+                        self.write_encoded_value(hint["width"])
             else:
-                cls.write_encoded_value(0)
+                self.write_encoded_value(0)
 
         if not (hintmasks := hints.get("hintmasks")):
-            cls.write_encoded_value(0)
+            self.write_encoded_value(0)
             return
 
         # FIXME: Implement writing of hintmasks
-        # cls.write_encoded_value(len(hintmasks))
-        cls.write_encoded_value(0)
+        # self.write_encoded_value(len(hintmasks))
+        self.write_encoded_value(0)
         logger.warning("Compilation of hint masks is not supported.")
 
-    @classmethod
-    def _compile_instructions(cls, data):
+    def _compile_instructions(self, data):
         # TrueType instructions
         if not (tth := data.get("tth")):
             return
 
-        cls.write_uint1(0x0A)
-        instructions = InstructionsCompiler.compile(tth)
-        cls.write_encoded_value(len(instructions))
-        cls.stream.write(instructions)
+        self.write_uint1(0x0A)
+        instructions = InstructionsCompiler().compile(tth)
+        self.write_encoded_value(len(instructions))
+        self.stream.write(instructions)
 
-    @classmethod
-    def _compile_kerning(cls, data):
+    def _compile_kerning(self, data):
         # Kerning
         if not (kerning := data.get("kerning")):
             return
 
-        cls.write_uint1(6)
-        cls.write_encoded_value(len(kerning))
+        self.write_uint1(6)
+        self.write_encoded_value(len(kerning))
         for gid, values in kerning.items():
-            cls.write_encoded_value(gid)
+            self.write_encoded_value(gid)
             for value in values:
-                cls.write_encoded_value(value)
+                self.write_encoded_value(value)
 
-    @classmethod
-    def _compile_metrics(cls, data):
+    def _compile_metrics(self, data):
         # Metrics
         if not (metrics := data.get("metrics")):
             return
 
-        cls.write_uint1(2)
-        for i in range(cls.num_masters):
+        self.write_uint1(2)
+        for i in range(self.num_masters):
             x, y = metrics[i]
-            cls.write_encoded_value(x)
-            cls.write_encoded_value(y)
+            self.write_encoded_value(x)
+            self.write_encoded_value(y)
 
-    @classmethod
-    def _compile_outlines(cls, data):
+    def _compile_outlines(self, data):
         # Outlines
         # A minimal outlines structure is always written:
-        cls.write_uint1(8)
-        cls.write_encoded_value(cls.num_masters)  # Number of masters
+        self.write_uint1(8)
+        self.write_encoded_value(self.num_masters)  # Number of masters
 
         if not (nodes := data.get("nodes")):
             # 0 nodes with 0 values
-            cls.write_encoded_value(0)
-            cls.write_encoded_value(0)
+            self.write_encoded_value(0)
+            self.write_encoded_value(0)
             return
 
-        outlines, num_values = OutlinesCompiler.compile(nodes, cls.num_masters)
-        # try:
-        #     num_values_old = data["num_node_values"]
-        #     if num_values != num_values_old:
-        #         logger.warning(
-        #             "Number of node values has changed: "
-        #             f"{num_values_old} -> {num_values}"
-        #         )
-        # except KeyError:
-        #     pass
-        cls.write_encoded_value(num_values)
-        cls.stream.write(outlines)
+        outlines, num_values = OutlinesCompiler().compile(nodes, self.num_masters)
+        self.write_encoded_value(num_values)
+        self.stream.write(outlines)
 
-    @classmethod
-    def _compile(cls, data: Any) -> None:
+    def _compile(self, data: Any) -> None:
 
         # Constants?
-        cls.write_bytes(pack("<4B", *GLYPH_CONSTANT))
-        cls.num_masters = data["num_masters"]
+        self.write_bytes(pack("<4B", *GLYPH_CONSTANT))
+        self.num_masters = data["num_masters"]
 
-        cls._compile_glyph_name(data)
-        cls._compile_outlines(data)
-        cls._compile_metrics(data)
-        cls._compile_hints(data)
-        cls._compile_guides(data)
-        cls._compile_components(data)
-        cls._compile_kerning(data)
-        cls._compile_binary(data)
-        cls._compile_instructions(data)
-        cls.write_uint1(15)  # End of glyph
+        self._compile_glyph_name(data)
+        self._compile_outlines(data)
+        self._compile_metrics(data)
+        self._compile_hints(data)
+        self._compile_guides(data)
+        self._compile_components(data)
+        self._compile_kerning(data)
+        self._compile_binary(data)
+        self._compile_instructions(data)
+        self.write_uint1(15)  # End of glyph
 
 
 class InstructionsCompiler(BaseCompiler):
-    @classmethod
-    def _compile(cls, data: Any) -> None:
-        cls.write_encoded_value(len(data))
+    def _compile(self, data: Any) -> None:
+        self.write_encoded_value(len(data))
         for cmd in data:
             command_id = TT_COMMAND_CONSTANTS[cmd["cmd"]]
-            cls.write_uint1(command_id)
+            self.write_uint1(command_id)
             params = cmd["params"]
             for param_name in TT_COMMANDS[command_id]["params"]:
-                cls.write_encoded_value(params[param_name])
+                self.write_encoded_value(params[param_name])
         for _ in range(3):
-            cls.write_encoded_value(0)
+            self.write_encoded_value(0)
 
 
 class OutlinesCompiler(BaseCompiler):
-    @classmethod
-    def compile(cls, data: Any, num_masters: int) -> Tuple[bytes, int]:
-        cls.num_masters = num_masters
-        cls.stream = BytesIO()
-        num_values = cls._compile(data)
-        return cls.stream.getvalue(), num_values
+    def compile(self, data: Any, num_masters: int) -> Tuple[bytes, int]:
+        self.num_masters = num_masters
+        assert not hasattr(self, "stream")
+        self.stream = BytesIO()
+        num_values = self._compile(data)
+        return self.stream.getvalue(), num_values
 
-    @classmethod
-    def _compile(cls, data: Any) -> int:
-        cls.write_encoded_value(len(data))  # Number of nodes, may be 0
+    def _compile(self, data: Any) -> int:
+        self.write_encoded_value(len(data))  # Number of nodes, may be 0
         num_values = 0
-        ref_coords = [[0, 0] for _ in range(cls.num_masters)]
+        ref_coords = [[0, 0] for _ in range(self.num_masters)]
         for node in data:
             type_flags = node.get("flags", 0) * 16 + node_types[node["type"]]
-            cls.write_uint1(type_flags)
+            self.write_uint1(type_flags)
             num_values += 1
             for j in range(len(node["points"][0])):
-                for i in range(cls.num_masters):
+                for i in range(self.num_masters):
                     x, y = node["points"][i][j]
                     refx, refy = ref_coords[i]
                     # Coordinates are written relatively to the previous coords
-                    cls.write_encoded_value(x - refx)
-                    cls.write_encoded_value(y - refy)
+                    self.write_encoded_value(x - refx)
+                    self.write_encoded_value(y - refy)
                     num_values += 2
                     ref_coords[i] = [x, y]
         return 2 * num_values
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/compilers/value.py` & `vfbLib-0.5.1/Lib/vfbLib/compilers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/constants.py` & `vfbLib-0.5.1/Lib/vfbLib/constants.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/cu2qu.py` & `vfbLib-0.5.1/Lib/vfbLib/cu2qu.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,34 +63,35 @@
             "all_quadratic": True,
         }
         if args.max_err_em:
             kwargs["max_err_em"] = args.max_err_em[0]
         if vfb.num_masters == 1:
             modified = font_to_quadratic(vfb, **kwargs)
         elif vfb.num_masters > 1:
-            # FIXME: How do we set the master number?
-            modified = fonts_to_quadratic(vfb, **kwargs)
+            vfbs = vfb.get_masters()
+            modified = fonts_to_quadratic(vfbs, **kwargs)
         else:
             print(f"Unsupported number of masters: {vfb.num_masters}")
             return
 
         if not modified:
             print("File was not modified.")
             return
 
         suffix = ".qu.vfb"
         if args.path:
+            suffix = ".vfb"
             out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(suffix)
         else:
             out_path = vfb_path.with_suffix(suffix)
         if out_path.exists():
             if not args.force_overwrite:
                 print(
                     "Output file exists, new file was not saved. "
                     "Use -fo to force overwriting."
                 )
-                return
+                raise FileExistsError
 
         print(f"Saving converted file to {out_path}.")
         vfb.write(out_path)
     else:
         parser.print_help()
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/diff.py` & `vfbLib-0.5.1/Lib/vfbLib/diff.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/__init__.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class BaseParser:
     """
     Base class to parse data from a vfb file
     """
 
+    encoding = "cp1252"
     master_count: int | None = None
     stream: BytesIO = BytesIO()
 
     @classmethod
     def parse(
         cls,
         stream: BufferedReader,
@@ -183,23 +184,23 @@
         ]
 
 
 class GlyphEncodingParser(BaseParser):
     @classmethod
     def _parse(cls):
         gid = int.from_bytes(cls.stream.read(2), byteorder="little")
-        nam = cls.stream.read().decode("ascii")
+        nam = cls.stream.read().decode("cp1252")
         return gid, nam
 
 
 class OpenTypeClassFlagsParser(BaseParser):
     @classmethod
     def _parse(cls) -> ClassFlagDict:
         class_flags: ClassFlagDict = {}
         num_classes = read_encoded_value(cls.stream)
         for _ in range(num_classes):
             n = read_encoded_value(cls.stream)
-            name = cls.stream.read(n).decode("cp1252")
+            name = cls.stream.read(n).decode(cls.encoding)
             flag1 = read_encoded_value(cls.stream)
             flag2 = read_encoded_value(cls.stream)
             class_flags[name] = (flag1, flag2)
         return class_flags
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/bitmap.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/bitmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/cmap.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/cmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/glyph.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/glyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         num_anchors = read_encoded_value(stream)
         anchors = []
         for _ in range(num_anchors):
             anchor_name_length = read_encoded_value(stream)
             name = None
             if anchor_name_length > 0:
-                name = stream.read(anchor_name_length).decode("cp1252")
+                name = stream.read(anchor_name_length).decode(cls.encoding)
 
             x = read_encoded_value(stream)
             x1 = read_encoded_value(stream)
             y = read_encoded_value(stream)
             y1 = read_encoded_value(stream)
             anchor = Anchor(x=x, x1=x1, y=y, y1=y1)
             if name:
@@ -419,15 +419,15 @@
             # Read a value to decide what kind of information follows
             v = cls.read_uint8(s)
 
             if v == 0x01:
                 # Glyph name
                 glyph_name_length = read_encoded_value(s)
                 glyph_name = s.read(glyph_name_length)
-                glyphdata["name"] = glyph_name.decode("cp1252")
+                glyphdata["name"] = glyph_name.decode(cls.encoding)
                 logger.debug(f"Glyph: {glyphdata['name']}")
 
             elif v == 0x02:
                 # Metrics
                 cls.parse_metrics(s, glyphdata, num_masters)
 
             elif v == 0x03:
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/guides.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/header.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/mm.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/mm.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/numeric.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/numeric.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/options.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/options.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/ps.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/text.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,35 +22,35 @@
             langID = read_encoded_value(stream)
             name_length = read_encoded_value(stream)
             name_codes = [read_encoded_value(stream) for _ in range(name_length)]
             name = ""
             for c in name_codes:
                 try:
                     char = chr(c)
-                    # FIXME: Worth fixing the platform-specific encodings?
-                    # if platID == 1 and encID == 0:
-                    #     char = char.encode("utf-8").decode("macroman")
+                    # Fix platform-specific encodings for Mac
+                    if platID == 1 and encID == 0:
+                        char = c.to_bytes().decode("macroman")
                 except ValueError:
                     char = "\ufeff"
                 name += char
             result.append([nameID, platID, encID, langID, name])
 
         assert stream.read() == b""
         return result
 
 
 class OpenTypeClassParser(BaseParser):
     """
-    A parser that reads data as a Windows-1252-encoded strings and returns it formatted
-    to represent an OpenType class
+    A parser that reads data as strings and returns it formatted to represent an
+    OpenType class
     """
 
     @classmethod
     def _parse(cls) -> Dict[str, List[str] | str]:
-        s = cls.stream.read().decode("cp1252").strip("\u0000 ")
+        s = cls.stream.read().decode(cls.encoding).strip("\u0000 ")
         if ":" not in s:
             logger.warning(f"Malformed OpenType class: {s}")
             return {"str": s, "err": "PARSE_ERROR"}
             # raise ValueError
 
         name, contents = s.split(":")
 
@@ -60,24 +60,24 @@
             if glyph:
                 glyphs.append(glyph)
         return {"name": name, "glyphs": glyphs}
 
 
 class OpenTypeStringParser(BaseParser):
     """
-    A parser that reads data as a Windows-1252-encoded strings and returns it as a list.
+    A parser that reads data as a strings and returns it as a list.
     """
 
     @classmethod
     def _parse(cls) -> List[str]:
-        s = cls.stream.read().decode("cp1252").strip("\u0000 ")
+        s = cls.stream.read().decode(cls.encoding).strip("\u0000 ")
         return s.splitlines()
 
 
 class StringParser(BaseParser):
     """
-    A parser that reads data as Windows-1252-encoded strings.
+    A parser that reads data as strings.
     """
 
     @classmethod
     def _parse(cls):
-        return cls.stream.read().decode("cp1252").strip("\u0000 ")
+        return cls.stream.read().decode(cls.encoding).strip("\u0000 ")
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/truetype.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/parsers/value.py` & `vfbLib-0.5.1/Lib/vfbLib/parsers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/truetype.py` & `vfbLib-0.5.1/Lib/vfbLib/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/typing.py` & `vfbLib-0.5.1/Lib/vfbLib/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/__init__.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,11 +721,18 @@
                 styleMapStyleName=self.info.styleMapStyleName,
                 styleName=style_name,
                 userLocation=get_ds_location(self.axes, loc, 1),
             )
 
         return ds
 
-    def get_master_path(self, out_path: Path, master_index: int) -> Path:
+    @classmethod
+    def get_master_path(cls, out_path: Path, master_index: int) -> Path:
         if master_index > 0:
-            return out_path.with_stem(f"{out_path.stem}-{master_index}")
+            try:
+                return out_path.with_stem(f"{out_path.stem}-{master_index}")
+            except AttributeError:
+                # Python 3.8 doesn't have `Path.with_stem`
+                return out_path.with_name(
+                    f"{out_path.stem}-{master_index}{out_path.suffix}"
+                )
         return out_path
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/designspace.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/designspace.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/glyph.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/groups.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/groups.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/guides.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/helpers.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def fix_vfb2ufo_feature_encoding(ufo_path: Path) -> None:
     # Read vfb2ufo's Windows-1252-encoded feature file and convert to UTF-8
     fea_path = ufo_path / "features.fea"
     if not fea_path.exists():
         # UFOs may omit the fea file
         return
 
-    with codecs.open(str(fea_path), "rb", "windows-1252") as f:
+    with codecs.open(str(fea_path), "rb", "cp1252") as f:
         fea = f.read()
     with codecs.open(str(fea_path), "wb", "utf-8") as f:
         f.write(fea)
 
 
 def update_global_guides(f: Font):
     # Update Global Guides to UFO standard
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/info.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/kerning.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/kerning.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/paths.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/paths.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/pshints.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/pshints.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/tth.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/tth.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/typing.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/ufo/vfb2ufo.py` & `vfbLib-0.5.1/Lib/vfbLib/ufo/vfb2ufo.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/value.py` & `vfbLib-0.5.1/Lib/vfbLib/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/vfb/entry.py` & `vfbLib-0.5.1/Lib/vfbLib/vfb/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         parser: Type[BaseParser] | None = None,
         compiler: Type[BaseCompiler] | None = None,
     ) -> None:
         # The original or compiled binary data
         self.data: bytes | None = None
         # The decompiled data
         self.decompiled = None
+        # Temporary data for additional master, must be merged when compiling
+        self.temp_masters = None
         # The numeric and human-readable key of the entry
         self.id = None
         self.key = None
         # Has the data been modified, i.e. it needs recompilation
         self._modified = False
         # The parser which can convert data to decompiled
         self.parser = parser
@@ -118,14 +120,16 @@
         """
         self.id = BaseParser.read_uint16(self.stream)
         entry_info = parser_classes.get(
             self.id & ~0x8000, (str(self.id), FALLBACK_PARSER, None)
         )
         key, parser_class, compiler_class = entry_info
 
+        parser_class.encoding = self.vfb.encoding
+
         if self.id == 5:
             # File end marker?
             BaseParser.read_uint16(self.stream)
             two = BaseParser.read_uint16(self.stream)
             if two == 2:
                 BaseParser.read_uint16(self.stream)
                 raise EOFError
@@ -174,15 +178,17 @@
         """
         Compile the entry. The result is stored in VfbEntry.data.
         """
         if self.compiler is None:
             logger.error(f"Compiling '{self.key}' is not supported yet.")
             return
 
-        self.data = self.compiler.compile(
+        self.merge_masters_data()
+
+        self.data = self.compiler().compile(
             self.decompiled, master_count=self.vfb.num_masters
         )
         self.modified = False
 
     def decompile(self) -> None:
         """
         Decompile the entry. The result is stored in VfbEntry.decompiled.
@@ -206,14 +212,32 @@
             self.decompiled = self.parser.parse(
                 BytesIO(self.data), size=self.size, master_count=self.vfb.num_masters
             )
         except:  # noqa: E722
             logger.error(f"Parse error for data: {self.key}; {hexStr(self.data)}")
             logger.error(f"Parser class: {self.parser.__name__}")
             self.decompiled = None
+            raise
+
+    def merge_masters_data(self) -> None:
+        """
+        Merge any temporary masters data into the main decompiled structure. Such data
+        can be added as the result of drawing with a PointPen into a multiple master
+        Vfb.
+        """
+        if self.temp_masters is None:
+            return
+
+        if self.vfb.num_masters == 1:
+            return
+
+        if self.compiler is None:
+            return
+
+        self.compiler.merge(self.temp_masters, self.decompiled)
 
     def read(self, stream: BufferedReader) -> None:
         """
         Read the entry from the stream without decompiling the data.
         """
         self.stream = stream
         self.key, self.parser, self.compiler, size = self._read_entry()
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib/vfb/header.py` & `vfbLib-0.5.1/Lib/vfbLib/vfb/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/vfb/info.py` & `vfbLib-0.5.1/Lib/vfbLib/vfb/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/Lib/vfbLib/vfb/vfb.py` & `vfbLib-0.5.1/Lib/vfbLib/vfb/vfb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 
 from pathlib import Path
 from time import time
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Set, Tuple
-from vfbLib.vfb.glyph import VfbGlyph
+from vfbLib.vfb.glyph import VfbGlyph, VfbGlyphMaster
 from vfbLib.vfb.entry import VfbEntry
 from vfbLib.vfb.header import VfbHeader
 from vfbLib.vfb.info import VfbInfo
 
 if TYPE_CHECKING:
     from io import BufferedReader
 
@@ -30,32 +30,36 @@
     def __init__(
         self,
         vfb_path: Path,
         timing=True,
         minimal=False,
         drop_keys: Set[str] | None = None,
         only_header=False,
+        unicode_strings = False,
     ) -> None:
         self.vfb_path = vfb_path
         self.timing = timing
         self.minimal = minimal
         if drop_keys is None:
             self.drop_keys = set()
         else:
             self.drop_keys = set(drop_keys)
         self.only_header = only_header
+        # String encoding for nametable entries
+        self.encoding = "utf-8" if unicode_strings else "cp1252"
 
         # We need some minimal API to make pen access work ...
         self._glyphs: Dict[str, VfbGlyph] = {}
         self.glyph_order: List[str] = []
 
         # cu2qu accesses the info and lib ...
         self.info = VfbInfo(vfb=self)
         self.lib = {}
 
+        self.master_index = 0
         self.num_masters: int = 0
         self.read()
 
     def as_dict(self) -> Dict[str, Dict[str, Any]]:
         """
         Return the Vfb structure as Dict, e.g. for saving as JSON. The dict has the keys
         "header" and "entries".
@@ -75,30 +79,39 @@
         self.entries: List[VfbEntry] = []
 
     def _decompile_glyphs(self):
         for entry in self.entries:
             if entry.key == "Glyph":
                 glyph = VfbGlyph(entry, self)
                 name = glyph.decompile()
-                if name in self._glyphs:
+                i = 0
+                while name in self._glyphs:
                     logger.error(f"VFB contains duplicate glyph name: {name}")
-                    # FIXME: Disambiguate duplicate names
+                    # Disambiguate duplicate names
+                    i += 1
+                    name = f"{name}#{i}"
                 self._glyphs[name] = glyph
                 self.glyph_order.append(name)
 
     def __contains__(self, key: str) -> bool:
         if not self._glyphs:
             self._decompile_glyphs()
         return key in self._glyphs
 
     def __getitem__(self, key: str) -> VfbGlyph:
         if not self._glyphs:
             self._decompile_glyphs()
         return self._glyphs[key]
 
+    def getGlyphMaster(self, key: str, master_index: int) -> VfbGlyphMaster:
+        return VfbGlyphMaster(self[key], master_index)
+
+    def get_masters(self) -> List[VfbMaster]:
+        return [VfbMaster(self, i) for i in range(self.num_masters)]
+
     def decompile(self) -> None:
         """
         Decompile all entries, except for the ones listed in `drop_keys`.
         """
         start = time()
         for entry in self.entries:
             entry.decompile()
@@ -176,7 +189,36 @@
             for entry in self.entries:
                 if entry.modified:
                     entry.compile()
                 vfb.write(entry.header)
                 vfb.write(entry.data)
             # File end marker
             vfb.write(b"\05\00\00\00\02\00\00\00")
+
+
+class VfbMaster:
+    """
+    Minimal UFO interface for a single master of a multiple master VFB.
+    """
+
+    def __init__(self, vfb: Vfb, master_index: int = 0):
+        self.vfb = vfb
+        self.master_index = master_index
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.vfb
+
+    def __getitem__(self, key: str) -> VfbGlyphMaster:
+        return self.vfb.getGlyphMaster(key, self.master_index)
+
+    @property
+    def info(self) -> VfbInfo:
+        return self.vfb.info
+
+    def items(self) -> Iterable[Tuple[str, VfbGlyph]]:
+        return self.vfb.items()
+
+    def keys(self) -> Iterable[str]:
+        return self.vfb.keys()
+
+    def num_masters(self) -> int:
+        return self.vfb.num_masters
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib.egg-info/PKG-INFO` & `vfbLib-0.5.1/Lib/vfbLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,15 @@
 
 Generate a representation that closely adheres to the VFB structure.
 
 ```bash
 $ vfb2json MyFile.vfb
 ```
 
-will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
+will convert the file to `MyFile.vfb.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
 usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
```

### Comparing `vfbLib-0.5.0/Lib/vfbLib.egg-info/SOURCES.txt` & `vfbLib-0.5.1/Lib/vfbLib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 Lib/vfbLib/ufo/typing.py
 Lib/vfbLib/ufo/vfb2ufo.py
 Lib/vfbLib/vfb/__init__.py
 Lib/vfbLib/vfb/entry.py
 Lib/vfbLib/vfb/glyph.py
 Lib/vfbLib/vfb/header.py
 Lib/vfbLib/vfb/info.py
+Lib/vfbLib/vfb/pens.py
 Lib/vfbLib/vfb/vfb.py
```

### Comparing `vfbLib-0.5.0/PKG-INFO` & `vfbLib-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,15 @@
 
 Generate a representation that closely adheres to the VFB structure.
 
 ```bash
 $ vfb2json MyFile.vfb
 ```
 
-will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
+will convert the file to `MyFile.vfb.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
 usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
```

### Comparing `vfbLib-0.5.0/README.md` & `vfbLib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.5.0/setup.cfg` & `vfbLib-0.5.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = vfbLib
-version = 0.5.0
+version = 0.5.1
 description = Tools for converting FontLab Studio 5 (VFB) files.
 long_description = file: DESCRIPTION.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/vfblib/
 author = Jens Kutilek
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Environment :: Console
 project_urls = 
 	Source = https://github.com/LucasFonts/vfbLib
```

