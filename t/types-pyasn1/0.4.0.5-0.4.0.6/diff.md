# Comparing `tmp/types-pyasn1-0.4.0.5.tar.gz` & `tmp/types-pyasn1-0.4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyasn1-0.4.0.5.tar", last modified: Mon Mar 27 18:23:44 2023, max compression
+gzip compressed data, was "types-pyasn1-0.4.0.6.tar", last modified: Thu Jul 20 15:17:34 2023, max compression
```

## Comparing `types-pyasn1-0.4.0.5.tar` & `types-pyasn1-0.4.0.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.418773 types-pyasn1-0.4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-27 18:23:43.000000 types-pyasn1-0.4.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:43.000000 types-pyasn1-0.4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:23:44.418773 types-pyasn1-0.4.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.410773 types-pyasn1-0.4.0.5/pyasn1-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:23:43.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.410773 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.414773 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/eoo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.414773 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/encoder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.414773 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/der/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/der/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/der/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/der/encoder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.414773 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/encoder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.414773 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/calling.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/dateandtime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/integer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/octets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/compat/string.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.418773 types-pyasn1-0.4.0.5/pyasn1-stubs/type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/char.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/constraint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/namedtype.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/namedval.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/opentype.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/tagmap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/univ.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-27 18:21:24.000000 types-pyasn1-0.4.0.5/pyasn1-stubs/type/useful.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:44.418773 types-pyasn1-0.4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-27 18:23:43.000000 types-pyasn1-0.4.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:44.418773 types-pyasn1-0.4.0.5/types_pyasn1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:23:44.000000 types-pyasn1-0.4.0.5/types_pyasn1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-27 18:23:44.000000 types-pyasn1-0.4.0.5/types_pyasn1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:44.000000 types-pyasn1-0.4.0.5/types_pyasn1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:23:44.000000 types-pyasn1-0.4.0.5/types_pyasn1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.326089 types-pyasn1-0.4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-20 15:17:33.000000 types-pyasn1-0.4.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:33.000000 types-pyasn1-0.4.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:17:34.326089 types-pyasn1-0.4.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.318088 types-pyasn1-0.4.0.6/pyasn1-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 15:17:33.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.318088 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.322089 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/eoo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.322089 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/encoder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.322089 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/der/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/der/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/der/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/der/encoder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.322089 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/encoder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.322089 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/calling.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/dateandtime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/integer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/octets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/compat/string.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.326089 types-pyasn1-0.4.0.6/pyasn1-stubs/type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/char.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/constraint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/namedtype.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/namedval.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/opentype.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/tagmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/univ.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-20 15:15:13.000000 types-pyasn1-0.4.0.6/pyasn1-stubs/type/useful.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:34.326089 types-pyasn1-0.4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-20 15:17:33.000000 types-pyasn1-0.4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:34.326089 types-pyasn1-0.4.0.6/types_pyasn1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:17:34.000000 types-pyasn1-0.4.0.6/types_pyasn1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-20 15:17:34.000000 types-pyasn1-0.4.0.6/types_pyasn1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:34.000000 types-pyasn1-0.4.0.6/types_pyasn1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:17:34.000000 types-pyasn1-0.4.0.6/types_pyasn1.egg-info/top_level.txt
```

### Comparing `types-pyasn1-0.4.0.5/CHANGELOG.md` & `types-pyasn1-0.4.0.6/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.4.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.4.0.5 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 0.4.0.4 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-pyasn1-0.4.0.5/PKG-INFO` & `types-pyasn1-0.4.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyasn1
-Version: 0.4.0.5
+Version: 0.4.0.6
 Summary: Typing stubs for pyasn1
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/decoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/ber/encoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/ber/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/decoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/cer/encoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/cer/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/decoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/codec/native/encoder.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/codec/native/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/debug.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/debug.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/base.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/base.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/char.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/char.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/constraint.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/constraint.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/namedtype.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/namedtype.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/namedval.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/namedval.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/tag.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/tag.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/tagmap.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/tagmap.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/univ.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/univ.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/pyasn1-stubs/type/useful.pyi` & `types-pyasn1-0.4.0.6/pyasn1-stubs/type/useful.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.4.0.5/setup.py` & `types-pyasn1-0.4.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.4.0.5",
+      version="0.4.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md",
```

### Comparing `types-pyasn1-0.4.0.5/types_pyasn1.egg-info/PKG-INFO` & `types-pyasn1-0.4.0.6/types_pyasn1.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyasn1
-Version: 0.4.0.5
+Version: 0.4.0.6
 Summary: Typing stubs for pyasn1
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyasn1-0.4.0.5/types_pyasn1.egg-info/SOURCES.txt` & `types-pyasn1-0.4.0.6/types_pyasn1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

