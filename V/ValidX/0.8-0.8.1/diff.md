# Comparing `tmp/ValidX-0.8.tar.gz` & `tmp/ValidX-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValidX-0.8.tar", last modified: Wed May 31 16:29:55 2023, max compression
+gzip compressed data, was "ValidX-0.8.1.tar", last modified: Thu Jul 20 18:26:48 2023, max compression
```

## Comparing `ValidX-0.8.tar` & `ValidX-0.8.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.026445 ValidX-0.8/
--rw-rw-r--   0 krat      (1000) krat      (1000)     2681 2023-05-31 15:39:05.000000 ValidX-0.8/CHANGES.rst
--rw-rw-r--   0 krat      (1000) krat      (1000)      156 2023-03-01 14:03:51.000000 ValidX-0.8/CONTRIBUTORS.rst
--rw-rw-r--   0 krat      (1000) krat      (1000)     1336 2023-03-01 14:03:51.000000 ValidX-0.8/LICENCE.txt
--rw-rw-r--   0 krat      (1000) krat      (1000)       20 2023-03-01 14:03:51.000000 ValidX-0.8/MANIFEST.in
--rw-rw-r--   0 krat      (1000) krat      (1000)     4629 2023-05-31 16:29:55.026445 ValidX-0.8/PKG-INFO
--rw-rw-r--   0 krat      (1000) krat      (1000)      899 2023-03-01 14:03:51.000000 ValidX-0.8/README.rst
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/ValidX.egg-info/
--rw-rw-r--   0 krat      (1000) krat      (1000)     4629 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/PKG-INFO
--rw-rw-r--   0 krat      (1000) krat      (1000)     1462 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/SOURCES.txt
--rw-rw-r--   0 krat      (1000) krat      (1000)        1 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/dependency_links.txt
--rw-rw-r--   0 krat      (1000) krat      (1000)        1 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/not-zip-safe
--rw-rw-r--   0 krat      (1000) krat      (1000)        7 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/top_level.txt
--rw-rw-r--   0 krat      (1000) krat      (1000)       38 2023-05-31 16:29:55.026445 ValidX-0.8/setup.cfg
--rw-rw-r--   0 krat      (1000) krat      (1000)     2476 2023-05-31 15:43:17.000000 ValidX-0.8/setup.py
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/
--rw-rw-r--   0 krat      (1000) krat      (1000)     1275 2023-05-31 15:39:22.000000 ValidX-0.8/validx/__init__.py
--rw-rw-r--   0 krat      (1000) krat      (1000)    13918 2023-03-01 14:03:51.000000 ValidX-0.8/validx/contracts.py
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/cy/
--rw-rw-r--   0 krat      (1000) krat      (1000)     1016 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/__init__.py
--rw-rw-r--   0 krat      (1000) krat      (1000)       31 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/abstract.pxd
--rw-rw-r--   0 krat      (1000) krat      (1000)      802 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/abstract.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     8539 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/abstract.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)      561 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/bools.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     2470 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/bools.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)     1338 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/chars.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     7607 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/chars.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)       43 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pxd
--rw-rw-r--   0 krat      (1000) krat      (1000)      181 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     1023 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)     2461 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/containers.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    18133 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/containers.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)     2579 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/datetimes.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    20718 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/datetimes.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)       97 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pxd
--rw-rw-r--   0 krat      (1000) krat      (1000)      250 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     1498 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)     1915 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/numbers.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    12285 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/numbers.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)      584 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/pipelines.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     2639 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/pipelines.pyx
--rw-rw-r--   0 krat      (1000) krat      (1000)     1382 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/special.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     8367 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/special.pyx
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/exc/
--rw-rw-r--   0 krat      (1000) krat      (1000)     1112 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/__init__.py
--rw-rw-r--   0 krat      (1000) krat      (1000)    10278 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/errors.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     2587 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/errors.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     5411 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/formatter.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      520 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/formatter.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     2869 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/markers.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      451 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/markers.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)      949 2023-03-01 14:03:51.000000 ValidX-0.8/validx/platform.py
-drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.026445 ValidX-0.8/validx/py/
--rw-rw-r--   0 krat      (1000) krat      (1000)     1016 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/__init__.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     8922 2023-03-27 17:33:25.000000 ValidX-0.8/validx/py/abstract.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      802 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/abstract.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     2239 2023-03-27 17:49:57.000000 ValidX-0.8/validx/py/bools.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      561 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/bools.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     6481 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/chars.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     1338 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/chars.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     1010 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/classes.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      181 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/classes.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    15987 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/containers.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     2461 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/containers.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    18974 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/datetimes.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     2579 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/datetimes.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     1473 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/instances.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      250 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/instances.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)    10735 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/numbers.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     1915 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/numbers.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     2389 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/pipelines.py
--rw-rw-r--   0 krat      (1000) krat      (1000)      584 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/pipelines.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)     7350 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/special.py
--rw-rw-r--   0 krat      (1000) krat      (1000)     1382 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/special.pyi
--rw-rw-r--   0 krat      (1000) krat      (1000)        0 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.272745 ValidX-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2967 2023-07-20 18:26:35.000000 ValidX-0.8.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-20 18:26:35.000000 ValidX-0.8.1/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-07-20 18:26:35.000000 ValidX-0.8.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-20 18:26:35.000000 ValidX-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-07-20 18:26:48.272745 ValidX-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-20 18:26:35.000000 ValidX-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.268745 ValidX-0.8.1/ValidX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-07-20 18:26:48.000000 ValidX-0.8.1/ValidX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-07-20 18:26:48.000000 ValidX-0.8.1/ValidX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 18:26:48.000000 ValidX-0.8.1/ValidX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 18:26:48.000000 ValidX-0.8.1/ValidX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-20 18:26:48.000000 ValidX-0.8.1/ValidX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 18:26:48.272745 ValidX-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-07-20 18:26:35.000000 ValidX-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.268745 ValidX-0.8.1/validx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13918 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.268745 ValidX-0.8.1/validx/cy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/abstract.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8539 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/abstract.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/bools.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2470 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/bools.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/chars.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7607 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/chars.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/classes.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/classes.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    18335 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/containers.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/datetimes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20718 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/datetimes.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/instances.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/instances.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/instances.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    12285 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/numbers.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/pipelines.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/pipelines.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8517 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/cy/special.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.272745 ValidX-0.8.1/validx/exc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10278 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/formatter.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2869 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/markers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/exc/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:48.272745 ValidX-0.8.1/validx/py/
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8922 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/abstract.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/bools.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/bools.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     6481 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/chars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/chars.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    16189 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    18974 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/datetimes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/instances.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/instances.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    10735 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/pipelines.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7500 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/special.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 18:26:35.000000 ValidX-0.8.1/validx/py.typed
```

### Comparing `ValidX-0.8/CHANGES.rst` & `ValidX-0.8.1/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+0.8.1
+-----
+
+*   Fixed ``List`` and ``Set`` restricting mappings from their valid input.
+*   Fixed cloning and representing of ``Const`` validator
+    constructed with ``False`` or ``None`` a value.
+*   Fixed nullable check of ``Type`` validator constructed with ``object`` as a type.
+
 
 0.8
 ---
 
 *   Dropped Python 3.5 support.
 *   Added Python 3.10, 3.11 support.
 *   Fixed handling UNIX-timestamps by ``Date`` and ``Datetime`` validators.
```

### Comparing `ValidX-0.8/LICENCE.txt` & `ValidX-0.8.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/README.rst` & `ValidX-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/ValidX.egg-info/SOURCES.txt` & `ValidX-0.8.1/ValidX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/setup.py` & `ValidX-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/__init__.py` & `ValidX-0.8.1/validx/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,10 +77,10 @@
     "Const",
     "Any",
     "classes",
     "instances",
 ]
 
 __impl__ = __impl__
-__version__ = "0.8"
+__version__ = "0.8.1"
 __author__ = "Cottonwood Technology <info@cottonwood.tech>"
 __license__ = "BSD"
```

### Comparing `ValidX-0.8/validx/contracts.py` & `ValidX-0.8.1/validx/contracts.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/__init__.py` & `ValidX-0.8.1/validx/cy/__init__.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/abstract.pyi` & `ValidX-0.8.1/validx/cy/abstract.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/abstract.pyx` & `ValidX-0.8.1/validx/cy/abstract.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/bools.pyi` & `ValidX-0.8.1/validx/cy/bools.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/bools.pyx` & `ValidX-0.8.1/validx/cy/bools.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/chars.pyi` & `ValidX-0.8.1/validx/cy/chars.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/chars.pyx` & `ValidX-0.8.1/validx/cy/chars.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/classes.pyx` & `ValidX-0.8.1/validx/cy/classes.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/containers.pyi` & `ValidX-0.8.1/validx/cy/containers.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/containers.pyx` & `ValidX-0.8.1/validx/cy/containers.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         upper length limit.
 
     :param bool unique:
         drop duplicate items.
 
 
     :raises InvalidTypeError:
-        if ``not isinstance(value, Iterable)``.
+        if ``not isinstance(value, Iterable)``
+        or ``isinstance(value, (str, bytes, Mapping))``.
 
     :raises MinLengthError:
         if ``len(value) < self.minlen``.
 
     :raises MaxLengthError:
         if ``len(value) > self.maxlen``.
 
@@ -130,15 +131,17 @@
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
         if not isinstance(value, (list, tuple, set, frozenset)):
-            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+            if not isinstance(value, Iterable) or isinstance(
+                value, (str, bytes, dict, Mapping)
+            ):
                 raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
 
         result = []
         errors = []
         if self.unique:
             unique = set()
 
@@ -184,15 +187,16 @@
         lower length limit.
 
     :param int maxlen:
         upper length limit.
 
 
     :raises InvalidTypeError:
-        if ``not isinstance(value, Iterable)``.
+        if ``not isinstance(value, Iterable)``
+        or ``isinstance(value, (str, bytes, Mapping))``.
 
     :raises MinLengthError:
         if ``len(value) < self.minlen``.
 
     :raises MaxLengthError:
         if ``len(value) > self.maxlen``.
 
@@ -249,15 +253,17 @@
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
         if not isinstance(value, (list, tuple, set, frozenset)):
-            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+            if not isinstance(value, Iterable) or isinstance(
+                value, (str, bytes, dict, Mapping)
+            ):
                 raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
 
         result = set()
         errors = []
 
         for num, val in _enumerate(value):
             try:
```

### Comparing `ValidX-0.8/validx/cy/datetimes.pyi` & `ValidX-0.8.1/validx/cy/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/datetimes.pyx` & `ValidX-0.8.1/validx/cy/datetimes.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/instances.pyx` & `ValidX-0.8.1/validx/cy/instances.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/numbers.pyi` & `ValidX-0.8.1/validx/cy/numbers.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/numbers.pyx` & `ValidX-0.8.1/validx/cy/numbers.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/pipelines.pyi` & `ValidX-0.8.1/validx/cy/pipelines.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/pipelines.pyx` & `ValidX-0.8.1/validx/cy/pipelines.pyx`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/special.pyi` & `ValidX-0.8.1/validx/cy/special.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/cy/special.pyx` & `ValidX-0.8.1/validx/cy/special.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,18 @@
         self._minlen = 0 if minlen is None else minlen
         self._maxlen = limits.LONG_MAX if maxlen is None else maxlen
         self._options = options
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
-        if value is None and self.nullable:
-            return value
+        if value is None:
+            if self.nullable:
+                return value
+            raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
         if not isinstance(value, self.tp):
             if not self.coerce:
                 raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
             else:
                 try:
                     value = self.tp(value)
                 except Exception:
@@ -300,14 +302,17 @@
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value != self.value:
             raise exc.OptionsError(expected=[self.value], actual=value)
         return value
 
+    def params(self):
+        yield "value", self.value
+
 
 cdef class Any(abstract.Validator):
     """
     Pass-Any Validator
 
     It literally accepts any value.
```

### Comparing `ValidX-0.8/validx/exc/__init__.py` & `ValidX-0.8.1/validx/exc/__init__.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/exc/errors.py` & `ValidX-0.8.1/validx/exc/errors.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/exc/errors.pyi` & `ValidX-0.8.1/validx/exc/errors.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/exc/formatter.py` & `ValidX-0.8.1/validx/exc/formatter.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/exc/formatter.pyi` & `ValidX-0.8.1/validx/exc/formatter.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/exc/markers.py` & `ValidX-0.8.1/validx/exc/markers.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/platform.py` & `ValidX-0.8.1/validx/platform.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/__init__.py` & `ValidX-0.8.1/validx/py/__init__.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/abstract.py` & `ValidX-0.8.1/validx/py/abstract.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/abstract.pyi` & `ValidX-0.8.1/validx/py/abstract.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/bools.py` & `ValidX-0.8.1/validx/py/bools.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/bools.pyi` & `ValidX-0.8.1/validx/py/bools.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/chars.py` & `ValidX-0.8.1/validx/py/chars.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/chars.pyi` & `ValidX-0.8.1/validx/py/chars.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/classes.py` & `ValidX-0.8.1/validx/py/classes.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/containers.py` & `ValidX-0.8.1/validx/py/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         upper length limit.
 
     :param bool unique:
         drop duplicate items.
 
 
     :raises InvalidTypeError:
-        if ``not isinstance(value, Iterable)``.
+        if ``not isinstance(value, Iterable)``
+        or ``isinstance(value, (str, bytes, Mapping))``.
 
     :raises MinLengthError:
         if ``len(value) < self.minlen``.
 
     :raises MaxLengthError:
         if ``len(value) > self.maxlen``.
 
@@ -93,15 +94,17 @@
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
         if not isinstance(value, (list, tuple, set, frozenset)):
-            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+            if not isinstance(value, Iterable) or isinstance(
+                value, (str, bytes, dict, Mapping)
+            ):
                 raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
 
         result = []
         errors = []
         if self.unique:
             unique = set()
 
@@ -147,15 +150,16 @@
         lower length limit.
 
     :param int maxlen:
         upper length limit.
 
 
     :raises InvalidTypeError:
-        if ``not isinstance(value, Iterable)``.
+        if ``not isinstance(value, Iterable)``
+        or ``isinstance(value, (str, bytes, Mapping))``.
 
     :raises MinLengthError:
         if ``len(value) < self.minlen``.
 
     :raises MaxLengthError:
         if ``len(value) > self.maxlen``.
 
@@ -192,15 +196,17 @@
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
         if not isinstance(value, (list, tuple, set, frozenset)):
-            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+            if not isinstance(value, Iterable) or isinstance(
+                value, (str, bytes, dict, Mapping)
+            ):
                 raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
 
         result = set()
         errors = []
 
         for num, val in _enumerate(value):
             try:
```

### Comparing `ValidX-0.8/validx/py/containers.pyi` & `ValidX-0.8.1/validx/py/containers.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/datetimes.py` & `ValidX-0.8.1/validx/py/datetimes.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/datetimes.pyi` & `ValidX-0.8.1/validx/py/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/instances.py` & `ValidX-0.8.1/validx/py/instances.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/numbers.py` & `ValidX-0.8.1/validx/py/numbers.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/numbers.pyi` & `ValidX-0.8.1/validx/py/numbers.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/pipelines.py` & `ValidX-0.8.1/validx/py/pipelines.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/pipelines.pyi` & `ValidX-0.8.1/validx/py/pipelines.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.8/validx/py/special.py` & `ValidX-0.8.1/validx/py/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,16 +188,18 @@
         setattr(self, "minlen", minlen)
         setattr(self, "maxlen", maxlen)
         setattr(self, "options", options)
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
-        if value is None and self.nullable:
-            return value
+        if value is None:
+            if self.nullable:
+                return value
+            raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
         if not isinstance(value, self.tp):
             if not self.coerce:
                 raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
             else:
                 try:
                     value = self.tp(value)
                 except Exception:
@@ -242,14 +244,17 @@
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value != self.value:
             raise exc.OptionsError(expected=[self.value], actual=value)
         return value
 
+    def params(self):
+        yield "value", self.value
+
 
 class Any(abstract.Validator):
     """
     Pass-Any Validator
 
     It literally accepts any value.
```

### Comparing `ValidX-0.8/validx/py/special.pyi` & `ValidX-0.8.1/validx/py/special.pyi`

 * *Files identical despite different names*

