# Comparing `tmp/pydal2sql-0.3.0.tar.gz` & `tmp/pydal2sql-0.3.1.tar.gz`

## Comparing `pydal2sql-0.3.0.tar` & `pydal2sql-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/coverage.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/examples.sh
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/magic.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/settings_in_code.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    49364 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0    27150 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0    45751 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/style.css
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/cli.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/core.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/helpers.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/py.typed
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_core.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_helpers.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/README.md
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/coverage.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/examples.sh
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/magic.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/settings_in_code.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    49364 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0    27150 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    45751 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/htmlcov/style.css
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/core.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/helpers.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_core.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/tests/test_helpers.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/README.md
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 pydal2sql-0.3.1/PKG-INFO
```

### Comparing `pydal2sql-0.3.0/CHANGELOG.md` & `pydal2sql-0.3.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.1 (2023-07-20)
+
+### Documentation
+
+* **readme:** Add another video ([`ce4312d`](https://github.com/robinvandernoord/pydal2sql/commit/ce4312deb4e9ef6b9261971214d88afc3c431345))
+
 ## v0.3.0 (2023-07-20)
 
 ### Feature
 
 * 🪄✨ Add`--magic`™️ to the cli tooll! ([`b3f2409`](https://github.com/robinvandernoord/pydal2sql/commit/b3f24091a9201d60e392ac03a5360df35cdabc3e))
 
 ## v0.2.4 (2023-07-20)
```

### Comparing `pydal2sql-0.3.0/coverage.svg` & `pydal2sql-0.3.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/coverage_html.js` & `pydal2sql-0.3.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-0.3.1/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/favicon_32.png` & `pydal2sql-0.3.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/index.html` & `pydal2sql-0.3.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/keybd_closed.png` & `pydal2sql-0.3.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/keybd_open.png` & `pydal2sql-0.3.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/status.json` & `pydal2sql-0.3.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/htmlcov/style.css` & `pydal2sql-0.3.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/src/pydal2sql/cli.py` & `pydal2sql-0.3.1/src/pydal2sql/cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/src/pydal2sql/core.py` & `pydal2sql-0.3.1/src/pydal2sql/core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/src/pydal2sql/helpers.py` & `pydal2sql-0.3.1/src/pydal2sql/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/src/pydal2sql/magic.py` & `pydal2sql-0.3.1/src/pydal2sql/magic.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/tests/test_cli.py` & `pydal2sql-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/tests/test_core.py` & `pydal2sql-0.3.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/tests/test_helpers.py` & `pydal2sql-0.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/LICENSE.txt` & `pydal2sql-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/README.md` & `pydal2sql-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,24 +86,26 @@
 cat model_fragment.py | pydal2sql # without cli args if settings are set in code, or
 cat model_fragment.py | pydal2sql postgres --table person # with args if settings are not in code
 # both output the CREATE TABLE statements to stdout.
 
 # alternatively, you can simply run `pydal2sql` and you will be prompted for the code, which you can then paste.
 ```
 
+### Example with pipx
+
+[![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
+
 ### ⚠️ Experimental 🪄✨Magic🌟💻
 
 If you're copy-pasting some `define_table` statements which have validators or defaults that are defined elsewhere,
 the SQL generation could crash due to msising variables. However, if these variables are irrelevant to the samentics of
 the table definition (i.e. only used at runtime, not for the schema definition), you can now try the `--magic` flag.
 
 This flag will replace all missing variables with a special `Empty` class, which does nothing but
 prevent `NameError`, `AttributeError` and `TypeError`s.   
 This is of course not production-safe, so it shouldn't be used anywhere else.
 
-### Example with pipx
-
-[![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
+[![asciicast](https://asciinema.org/a/UQFaG2DWmXsJYzQ72CXer4oCu.svg)](https://asciinema.org/a/UQFaG2DWmXsJYzQ72CXer4oCu)
 
 ## License
 
 `pydal2sql` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pydal2sql-0.3.0/pyproject.toml` & `pydal2sql-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.3.0/PKG-INFO` & `pydal2sql-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal2sql
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convert pydal define_tables to SQL using pydal's CREATE TABLE logic
 Project-URL: Documentation, https://github.com/robinvandernoord/pydal2sql#readme
 Project-URL: Issues, https://github.com/robinvandernoord/pydal2sql/issues
 Project-URL: Source, https://github.com/robinvandernoord/pydal2sql
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -122,24 +122,26 @@
 cat model_fragment.py | pydal2sql # without cli args if settings are set in code, or
 cat model_fragment.py | pydal2sql postgres --table person # with args if settings are not in code
 # both output the CREATE TABLE statements to stdout.
 
 # alternatively, you can simply run `pydal2sql` and you will be prompted for the code, which you can then paste.
 ```
 
+### Example with pipx
+
+[![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
+
 ### ⚠️ Experimental 🪄✨Magic🌟💻
 
 If you're copy-pasting some `define_table` statements which have validators or defaults that are defined elsewhere,
 the SQL generation could crash due to msising variables. However, if these variables are irrelevant to the samentics of
 the table definition (i.e. only used at runtime, not for the schema definition), you can now try the `--magic` flag.
 
 This flag will replace all missing variables with a special `Empty` class, which does nothing but
 prevent `NameError`, `AttributeError` and `TypeError`s.   
 This is of course not production-safe, so it shouldn't be used anywhere else.
 
-### Example with pipx
-
-[![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
+[![asciicast](https://asciinema.org/a/UQFaG2DWmXsJYzQ72CXer4oCu.svg)](https://asciinema.org/a/UQFaG2DWmXsJYzQ72CXer4oCu)
 
 ## License
 
 `pydal2sql` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

