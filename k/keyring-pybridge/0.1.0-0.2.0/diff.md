# Comparing `tmp/keyring_pybridge-0.1.0.tar.gz` & `tmp/keyring_pybridge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_pybridge-0.1.0.tar", max compression
+gzip compressed data, was "keyring_pybridge-0.2.0.tar", max compression
```

## Comparing `keyring_pybridge-0.1.0.tar` & `keyring_pybridge-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       23 2023-07-20 20:19:51.913516 keyring_pybridge-0.1.0/keyring_pybridge/__init__.py
--rw-r--r--   0        0        0     1158 2023-07-20 20:20:18.273783 keyring_pybridge-0.1.0/keyring_pybridge/backend.py
--rw-r--r--   0        0        0      747 2023-07-20 19:59:04.995483 keyring_pybridge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1181 2023-07-20 20:26:35.067880 keyring_pybridge-0.1.0/README.md
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 keyring_pybridge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1181 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/README.md
+-rw-r--r--   0        0        0       68 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/keyring_pybridge/__init__.py
+-rw-r--r--   0        0        0     1122 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/keyring_pybridge/backend.py
+-rw-r--r--   0        0        0      711 2023-07-20 21:38:00.373844 keyring_pybridge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 keyring_pybridge-0.2.0/PKG-INFO
```

### Comparing `keyring_pybridge-0.1.0/pyproject.toml` & `keyring_pybridge-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[tool.poetry]
-name = "keyring-pybridge"
-version = "0.1.0"
-description = ""
-authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-keyring = "~24.2.0"
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.0.278"
-black = "^23.7.0"
-twine = "^4.0.2"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.ruff]
-select = [
-	"E",  # pycodestyle
-	"F",  # pyflakes
-	"I",  # isort
-	"N",  # pep8-naming
-	"ARG",  # flake8-unused-arguments
-	"T10",  # flake8-debugger
-	"RUF",  # Ruff-specific rules
-]
-
-[tool.ruff.isort]
-force-sort-within-sections = true
-order-by-type = false
-lines-after-imports = 2
+[tool.poetry]
+name = "keyring-pybridge"
+version = "0.2.0"
+description = ""
+authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+keyring = "~24.2.0"
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.278"
+black = "^23.7.0"
+twine = "^4.0.2"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+select = [
+	"E",  # pycodestyle
+	"F",  # pyflakes
+	"I",  # isort
+	"N",  # pep8-naming
+	"ARG",  # flake8-unused-arguments
+	"T10",  # flake8-debugger
+	"RUF",  # Ruff-specific rules
+]
+
+[tool.ruff.isort]
+force-sort-within-sections = true
+order-by-type = false
+lines-after-imports = 2
```

### Comparing `keyring_pybridge-0.1.0/README.md` & `keyring_pybridge-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `keyring_pybridge-0.1.0/PKG-INFO` & `keyring_pybridge-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyring-pybridge
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn.vangolen@zimmerbiomet.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

