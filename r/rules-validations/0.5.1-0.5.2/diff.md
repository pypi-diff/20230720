# Comparing `tmp/rules_validations-0.5.1.tar.gz` & `tmp/rules_validations-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules_validations-0.5.1.tar", max compression
+gzip compressed data, was "rules_validations-0.5.2.tar", max compression
```

## Comparing `rules_validations-0.5.1.tar` & `rules_validations-0.5.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2023-07-17 18:51:32.347143 rules_validations-0.5.1/README.md
--rw-r--r--   0        0        0      337 2023-07-17 18:51:42.955287 rules_validations-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1926 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/baseEnum.py
--rw-r--r--   0        0        0      633 2023-07-17 18:51:32.347143 rules_validations-0.5.1/rules_validations/normalize.py
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 rules_validations-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-07-20 14:41:31.736883 rules_validations-0.5.2/README.md
+-rw-r--r--   0        0        0      337 2023-07-20 14:41:50.353132 rules_validations-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1926 2023-07-20 14:41:31.736883 rules_validations-0.5.2/rules_validations/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-20 14:41:31.736883 rules_validations-0.5.2/rules_validations/baseEnum.py
+-rw-r--r--   0        0        0      663 2023-07-20 14:41:31.736883 rules_validations-0.5.2/rules_validations/normalize.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 rules_validations-0.5.2/PKG-INFO
```

### Comparing `rules_validations-0.5.1/rules_validations/__init__.py` & `rules_validations-0.5.2/rules_validations/__init__.py`

 * *Files identical despite different names*

### Comparing `rules_validations-0.5.1/rules_validations/baseEnum.py` & `rules_validations-0.5.2/rules_validations/baseEnum.py`

 * *Files identical despite different names*

### Comparing `rules_validations-0.5.1/rules_validations/normalize.py` & `rules_validations-0.5.2/rules_validations/normalize.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         .replace('í', 'i').replace('ï', 'i') \
         .replace('ó', 'o').replace('ö', 'o') \
         .replace('ú', 'u').replace('ü', 'u') \
         .replace('ñ', 'n') \
         .replace('(', '_') \
         .replace(')', '_') \
         .replace('/', '_') \
+        .replace('\\', '_') \
         .replace('+', 'p') \
         .replace('.', '') \
         .replace(',', '_') \
         .replace(':', '') \
         .replace(';', '') \
         .replace('-', '_') \
         .replace(' ', '_')
```

