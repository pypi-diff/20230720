# Comparing `tmp/pydal2sql-0.2.2.tar.gz` & `tmp/pydal2sql-0.2.3.tar.gz`

## Comparing `pydal2sql-0.2.2.tar` & `pydal2sql-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/coverage.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/examples.sh
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/settings_in_code.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    38096 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/htmlcov/style.css
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/cli.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/core.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/py.typed
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_cli.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_core.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/tests/test_helpers.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/README.md
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pydal2sql-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/coverage.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/examples.sh
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/settings_in_code.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    38096 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/style.css
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/core.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_core.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_helpers.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/README.md
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/PKG-INFO
```

### Comparing `pydal2sql-0.2.2/CHANGELOG.md` & `pydal2sql-0.2.3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.3 (2023-07-20)
+
+### Fix
+
+* Db type sometimes was an empty string, which is not None ([`d129cad`](https://github.com/robinvandernoord/pydal2sql/commit/d129cadacab0b8e5cef4799e6bff49c92d09731e))
+
 ## v0.2.2 (2023-07-20)
 
 ### Fix
 
 * Moved rich from dev to actual dependencies ([`03409c0`](https://github.com/robinvandernoord/pydal2sql/commit/03409c04ab7b01f49870f863956578b12b3de968))
 
 ## v0.2.1 (2023-07-20)
```

### Comparing `pydal2sql-0.2.2/coverage.svg` & `pydal2sql-0.2.3/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/coverage_html.js` & `pydal2sql-0.2.3/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/favicon_32.png` & `pydal2sql-0.2.3/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/index.html` & `pydal2sql-0.2.3/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/keybd_closed.png` & `pydal2sql-0.2.3/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/keybd_open.png` & `pydal2sql-0.2.3/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/status.json` & `pydal2sql-0.2.3/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/htmlcov/style.css` & `pydal2sql-0.2.3/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/src/pydal2sql/cli.py` & `pydal2sql-0.2.3/src/pydal2sql/cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/src/pydal2sql/core.py` & `pydal2sql-0.2.3/src/pydal2sql/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,17 @@
         However, your db_type can differ from the current database used.
         You can even use a dummy database to generate SQL code with:
         `db = pydal.DAL(None, migrate=False)`
 
     db_folder is the database folder where migration (`.table`) files are stored.
         By default, a random temporary dir is created.
     """
-    if db_type is None:
+    if not db_type:
         db_type = getattr(define_table._db, "_dbname", None)
+
         if db_type is None:
             raise ValueError("Please manually define a database type!")
 
     with TempdirOrExistingDir(db_folder) as db_folder:
         migrator = _build_dummy_migrator(db_type, db_folder=db_folder)
 
         sql: str = migrator.create_table(
```

### Comparing `pydal2sql-0.2.2/src/pydal2sql/helpers.py` & `pydal2sql-0.2.3/src/pydal2sql/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/tests/test_cli.py` & `pydal2sql-0.2.3/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,7 +62,36 @@
         )
     captured = capsys.readouterr()
 
 
     assert "CREATE TABLE" not in captured.out
     assert "CREATE TABLE" not in captured.err
     assert "db.define_table(" in captured.err
+
+def test_cli_guess_sqlite(capsys):
+    code = """
+       db = DAL('sqlite://:memory:', migrate=False)
+    
+       db.define_table(
+           "person",
+           Field(
+               "name",
+               "string",
+               nullable=False,
+           ),
+           Field("age", "integer", default=18),
+           Field("float", "decimal(2,3)"),
+           Field("nicknames", "list:string"),
+           Field("obj", "json"),
+       )
+       """
+
+    handle_cli(
+        code,
+        None,  # <-  set in code so no error
+        None
+    )
+    captured = capsys.readouterr()
+
+    print(captured.err)
+
+    assert "CREATE TABLE" in captured.out
```

### Comparing `pydal2sql-0.2.2/tests/test_core.py` & `pydal2sql-0.2.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/tests/test_helpers.py` & `pydal2sql-0.2.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/LICENSE.txt` & `pydal2sql-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/README.md` & `pydal2sql-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/pyproject.toml` & `pydal2sql-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.2/PKG-INFO` & `pydal2sql-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql
-Version: 0.2.2
+Version: 0.2.3
 Summary: Convert pydal define_tables to SQL using pydal's CREATE TABLE logic
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

