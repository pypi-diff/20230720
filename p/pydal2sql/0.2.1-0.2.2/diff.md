# Comparing `tmp/pydal2sql-0.2.1.tar.gz` & `tmp/pydal2sql-0.2.2.tar.gz`

## Comparing `pydal2sql-0.2.1.tar` & `pydal2sql-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/coverage.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/.github/workflows/su6.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/examples/examples.sh
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/examples/settings_in_code.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    38096 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/htmlcov/style.css
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/cli.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/core.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/py.typed
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/tests/test_cli.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/tests/test_core.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/tests/test_helpers.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/README.md
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pydal2sql-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/coverage.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/examples.sh
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/settings_in_code.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    38096 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/style.css
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/core.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_core.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_helpers.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/README.md
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/PKG-INFO
```

### Comparing `pydal2sql-0.2.1/coverage.svg` & `pydal2sql-0.2.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/coverage_html.js` & `pydal2sql-0.2.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/favicon_32.png` & `pydal2sql-0.2.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/index.html` & `pydal2sql-0.2.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/keybd_closed.png` & `pydal2sql-0.2.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/keybd_open.png` & `pydal2sql-0.2.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/status.json` & `pydal2sql-0.2.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/htmlcov/style.css` & `pydal2sql-0.2.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/src/pydal2sql/cli.py` & `pydal2sql-0.2.2/src/pydal2sql/cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/src/pydal2sql/core.py` & `pydal2sql-0.2.2/src/pydal2sql/core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/src/pydal2sql/helpers.py` & `pydal2sql-0.2.2/src/pydal2sql/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/tests/test_cli.py` & `pydal2sql-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/tests/test_core.py` & `pydal2sql-0.2.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/tests/test_helpers.py` & `pydal2sql-0.2.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/LICENSE.txt` & `pydal2sql-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/README.md` & `pydal2sql-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.1/pyproject.toml` & `pydal2sql-0.2.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+    "rich",
     "pydal",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
-    "rich",
     "su6[all]",
     "python-semantic-release < 8",
     "psycopg2-binary",
     "pymysql",
 ]
 
 all = [
```

### Comparing `pydal2sql-0.2.1/PKG-INFO` & `pydal2sql-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Convert pydal define_tables to SQL using pydal's CREATE TABLE logic
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,23 +14,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pydal
+Requires-Dist: rich
 Provides-Extra: all
 Requires-Dist: psycopg2-binary; extra == 'all'
 Requires-Dist: pymysql; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: psycopg2-binary; extra == 'dev'
 Requires-Dist: pymysql; extra == 'dev'
 Requires-Dist: python-semantic-release<8; extra == 'dev'
-Requires-Dist: rich; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Provides-Extra: mysql
 Requires-Dist: pymysql; extra == 'mysql'
 Provides-Extra: psql
 Requires-Dist: psycopg2-binary; extra == 'psql'
 Description-Content-Type: text/markdown
```

