# Comparing `tmp/pabutools-0.9.tar.gz` & `tmp/pabutools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pabutools-0.9.tar", last modified: Wed Mar  1 18:57:25 2023, max compression
+gzip compressed data, was "pabutools-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pabutools-0.9.tar` & `pabutools-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,41 @@
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.053669 pabutools-0.9/
--rw-r--r--   0 grzegorz   (501) staff       (20)     1078 2022-11-25 13:52:47.000000 pabutools-0.9/LICENSE.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)     3575 2023-03-01 18:57:25.053310 pabutools-0.9/PKG-INFO
--rw-r--r--   0 grzegorz   (501) staff       (20)     3337 2023-03-01 18:56:58.000000 pabutools-0.9/README.md
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.050817 pabutools-0.9/pabutools/
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2022-11-25 13:42:45.000000 pabutools-0.9/pabutools/__init__.py
--rw-r--r--   0 grzegorz   (501) staff       (20)     5197 2023-03-01 18:53:29.000000 pabutools-0.9/pabutools/model.py
--rw-r--r--   0 grzegorz   (501) staff       (20)     6352 2023-01-17 11:59:18.000000 pabutools-0.9/pabutools/rules.py
-drwxr-xr-x   0 grzegorz   (501) staff       (20)        0 2023-03-01 18:57:25.052844 pabutools-0.9/pabutools.egg-info/
--rw-r--r--   0 grzegorz   (501) staff       (20)     3575 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/PKG-INFO
--rw-r--r--   0 grzegorz   (501) staff       (20)      254 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/SOURCES.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/dependency_links.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)        1 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/not-zip-safe
--rw-r--r--   0 grzegorz   (501) staff       (20)       10 2023-03-01 18:57:25.000000 pabutools-0.9/pabutools.egg-info/top_level.txt
--rw-r--r--   0 grzegorz   (501) staff       (20)       38 2023-03-01 18:57:25.053787 pabutools-0.9/setup.cfg
--rw-rw-r--   0 grzegorz   (501) staff       (20)      479 2023-03-01 18:55:41.000000 pabutools-0.9/setup.py
+-rw-r--r--   0        0        0    35149 2023-07-20 12:30:12.381212 pabutools-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0    17102 2023-07-20 12:30:12.381212 pabutools-1.0.0/README.md
+-rw-r--r--   0        0        0      134 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/analysis/__init__.py
+-rw-r--r--   0        0        0     2138 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/analysis/category.py
+-rw-r--r--   0        0        0     1081 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/analysis/instanceproperties.py
+-rw-r--r--   0        0        0     2024 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/analysis/profileproperties.py
+-rw-r--r--   0        0        0     3610 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/analysis/votersatisfaction.py
+-rw-r--r--   0        0        0      251 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/__init__.py
+-rw-r--r--   0        0        0     3204 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/__init__.py
+-rw-r--r--   0        0        0     6913 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/approvalballot.py
+-rw-r--r--   0        0        0     3975 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/ballot.py
+-rw-r--r--   0        0        0     6513 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/cardinalballot.py
+-rw-r--r--   0        0        0     6232 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/cumulativeballot.py
+-rw-r--r--   0        0        0     9531 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/ballot/ordinalballot.py
+-rw-r--r--   0        0        0    15595 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/instance.py
+-rw-r--r--   0        0        0     8893 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/pabulib.py
+-rw-r--r--   0        0        0    10683 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/preflib.py
+-rw-r--r--   0        0        0     3349 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/__init__.py
+-rw-r--r--   0        0        0    20172 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/approvalprofile.py
+-rw-r--r--   0        0        0    18347 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/cardinalprofile.py
+-rw-r--r--   0        0        0    21470 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/cumulativeprofile.py
+-rw-r--r--   0        0        0    13033 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/ordinalprofile.py
+-rw-r--r--   0        0        0    14897 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/profile/profile.py
+-rw-r--r--   0        0        0     6117 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/satisfaction/__init__.py
+-rw-r--r--   0        0        0    20855 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/satisfaction/additivesatisfaction.py
+-rw-r--r--   0        0        0    10480 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/satisfaction/functionalsatisfaction.py
+-rw-r--r--   0        0        0     4815 2023-07-20 12:30:12.421212 pabutools-1.0.0/pabutools/election/satisfaction/positionalsatisfaction.py
+-rw-r--r--   0        0        0     4230 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/election/satisfaction/satisfactionmeasure.py
+-rw-r--r--   0        0        0    11464 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/election/satisfaction/satisfactionprofile.py
+-rw-r--r--   0        0        0     1833 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/fractions.py
+-rw-r--r--   0        0        0      570 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/__init__.py
+-rw-r--r--   0        0        0     3587 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/exhaustion.py
+-rw-r--r--   0        0        0    10221 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/greedywelfare.py
+-rw-r--r--   0        0        0     6479 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/maxwelfare.py
+-rw-r--r--   0        0        0    12392 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/mes.py
+-rw-r--r--   0        0        0     7737 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/rules/phragmen.py
+-rw-r--r--   0        0        0     3245 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/tiebreaking.py
+-rw-r--r--   0        0        0     2290 2023-07-20 12:30:12.425212 pabutools-1.0.0/pabutools/utils.py
+-rw-r--r--   0        0        0     1226 2023-07-20 12:30:12.425212 pabutools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    18251 1970-01-01 00:00:00.000000 pabutools-1.0.0/PKG-INFO
```

