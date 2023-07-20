# Comparing `tmp/pydal2sql-0.2.3.tar.gz` & `tmp/pydal2sql-0.3.0.tar.gz`

## Comparing `pydal2sql-0.2.3.tar` & `pydal2sql-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/coverage.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/.github/workflows/su6.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/examples.sh
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/settings_in_code.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/examples/settings_via_cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
--rw-r--r--   0        0        0    38096 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
--rw-r--r--   0        0        0    27001 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/htmlcov/style.css
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/__about__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/cli.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/core.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/py.typed
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/src/pydal2sql/types.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_cli.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_core.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/tests/test_helpers.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/README.md
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pydal2sql-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/coverage.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/examples.sh
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/magic.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/settings_in_code.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/examples/settings_via_cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html
+-rw-r--r--   0        0        0    49364 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html
+-rw-r--r--   0        0        0    27150 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html
+-rw-r--r--   0        0        0    45751 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_magic_py.html
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/htmlcov/style.css
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/__about__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/__init__.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/cli.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/core.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/helpers.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/py.typed
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/src/pydal2sql/types.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_core.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/tests/test_helpers.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/README.md
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 pydal2sql-0.3.0/PKG-INFO
```

### Comparing `pydal2sql-0.2.3/coverage.svg` & `pydal2sql-0.3.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/coverage_html.js` & `pydal2sql-0.3.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___about___py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___about___py.html`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 16:57 +0200
+            created at 2023-07-20 20:23 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Stores the version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.2.4"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 16:57 +0200
+            created at 2023-07-20 20:23 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 16:57 +0200
+at 2023-07-20 20:23 +0200
 
 
 1""" 
 2Stores the version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "0.1.0" 
+8__version__ = "0.2.4" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 16:57 +0200
+at 2023-07-20 20:23 +0200
```

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74___init___py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74___init___py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_cli_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">16 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">16<span class="text"> run</span></button>
+            <span class="text">28 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">28<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">22<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">29<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:05 +0200
+            created at 2023-07-20 20:24 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -81,161 +81,198 @@
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">CLI tool to generate SQL from PyDAL code.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">select</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">string</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">prompt</span> <span class="key">import</span> <span class="nam">Prompt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">flatten</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">class</span> <span class="nam">PrettyParser</span><span class="op">(</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    Add 'rich' to the argparse output.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">def</span> <span class="nam">_print_message</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">file</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">IO</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">message</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="key">def</span> <span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>   <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    Check if the program starts with cli data (pipe | or redirect >&lt;).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    See Also:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-some-data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">select</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="num">0.0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="key">def</span> <span class="nam">handle_cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">code</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">db_type</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">tables</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">verbose</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">noop</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">    Handle user input.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">to_execute</span> <span class="op">=</span> <span class="nam">string</span><span class="op">.</span><span class="nam">Template</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">        from pydal import *</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">        from pydal.objects import *</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">        from pydal.validators import *</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        from pydal2sql import generate_sql</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">        db = database = DAL(None, migrate=False)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="str">        tables = $tables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        db_type = '$db_type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">pathlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">select</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">string</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">textwrap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">import</span> <span class="nam">rich</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span><span class="op">.</span><span class="nam">prompt</span> <span class="key">import</span> <span class="nam">Prompt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">flatten</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">magic</span> <span class="key">import</span> <span class="nam">find_missing_variables</span><span class="op">,</span> <span class="nam">generate_magic_code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">class</span> <span class="nam">PrettyParser</span><span class="op">(</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    Add 'rich' to the argparse output.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">def</span> <span class="nam">_print_message</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">file</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">IO</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">message</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="key">def</span> <span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Check if the program starts with cli data (pipe | or redirect >&lt;).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    See Also:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">        https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-some-data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">select</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">                <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="op">[</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="num">0.0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">handle_cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">code</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">db_type</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">tables</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">verbose</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">noop</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="nam">magic</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    Handle user input.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="nam">to_execute</span> <span class="op">=</span> <span class="nam">string</span><span class="op">.</span><span class="nam">Template</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">        from pydal import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        from pydal.objects import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">        from pydal.validators import *</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">        from pydal2sql import generate_sql</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        db = database = DAL(None, migrate=False)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">        $code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t"><span class="str">        if not tables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">            tables = db._tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">        tables = $tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">        db_type = '$db_type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">        $extra</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        for table in tables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">            print(generate_sql(db[table], db_type))</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">            <span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">if</span> <span class="nam">verbose</span> <span class="key">or</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="key">def</span> <span class="nam">app</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">    Entrypoint for the pydal2sql cli command.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">PrettyParser</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">prog</span><span class="op">=</span><span class="str">"pydal2sql"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">formatter_class</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">RawDescriptionHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"""[green]CLI tool to generate SQL from PyDAL code.[/green]\n</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="str">        Aside from using cli arguments, you can also configure the tool in your code.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">        You can set the following variables:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">        db_type: str = 'sqlite' # your desired database type;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        tables: list[str] = []  # your desired tables to generate SQL for;"""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">epilog</span><span class="op">=</span><span class="str">"Example: [i]cat models.py | pydal2sql sqlite[/i]"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="str">"db_type"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which database dialect to generate ([blue]postgres, sqlite, mysql[/blue])"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--verbose"</span><span class="op">,</span> <span class="str">"-v"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Show more info"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        $code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">        if not tables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">            tables = db._tables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="str">        for table in tables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">            print(generate_sql(db[table], db_type))</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="op">{</span><span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span> <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span> <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span> <span class="str">"extra"</span><span class="op">:</span> <span class="str">""</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">if</span> <span class="nam">verbose</span> <span class="key">or</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">noop</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">except</span> <span class="nam">NameError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="com"># something is missing!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">            <span class="nam">missing_vars</span> <span class="op">=</span> <span class="nam">find_missing_variables</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">magic</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">                <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">                    <span class="str">f"Your code is missing some variables: {missing_vars}. Add these or try --magic"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="nam">extra_code</span> <span class="op">=</span> <span class="nam">generate_magic_code</span><span class="op">(</span><span class="nam">missing_vars</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                <span class="nam">generated_code</span> <span class="op">=</span> <span class="nam">to_execute</span><span class="op">.</span><span class="nam">substitute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                    <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                        <span class="str">"tables"</span><span class="op">:</span> <span class="nam">flatten</span><span class="op">(</span><span class="nam">tables</span> <span class="key">or</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                        <span class="str">"db_type"</span><span class="op">:</span> <span class="nam">db_type</span> <span class="key">or</span> <span class="str">""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                        <span class="str">"extra"</span><span class="op">:</span> <span class="nam">extra_code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                        <span class="str">"code"</span><span class="op">:</span> <span class="nam">textwrap</span><span class="op">.</span><span class="nam">dedent</span><span class="op">(</span><span class="nam">code</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                <span class="key">if</span> <span class="nam">verbose</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                    <span class="nam">print</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="str">"--noop"</span><span class="op">,</span> <span class="str">"-n"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Only show code, don't run it."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="str">"-t"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="str">"--table"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="str">"--tables"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">action</span><span class="op">=</span><span class="str">"append"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"+"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"One or more tables to generate. By default, all tables in the file will be used."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">db_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">Prompt</span><span class="op">.</span><span class="nam">ask</span><span class="op">(</span><span class="str">"Which database type do you want to use?"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"sqlite"</span><span class="op">,</span> <span class="str">"postgres"</span><span class="op">,</span> <span class="str">"mysql"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="nam">exec</span><span class="op">(</span><span class="nam">generated_code</span><span class="op">)</span>  <span class="com"># nosec: B102</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="key">def</span> <span class="nam">app</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t"><span class="str">    Entrypoint for the pydal2sql cli command.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="nam">parser</span> <span class="op">=</span> <span class="nam">PrettyParser</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">prog</span><span class="op">=</span><span class="str">"pydal2sql"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">formatter_class</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">RawDescriptionHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"""[green]CLI tool to generate SQL from PyDAL code.[/green]\n</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">        Aside from using cli arguments, you can also configure the tool in your code.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="str">        You can set the following variables:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        db_type: str = 'sqlite' # your desired database type;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">        tables: list[str] = []  # your desired tables to generate SQL for;"""</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">epilog</span><span class="op">=</span><span class="str">"Example: [i]cat models.py | pydal2sql sqlite[/i]"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"filename"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which file to load? Can also be done with stdin."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"Please paste your define tables code below and press ctrl-D when finished."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="com"># else: data from stdin</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="com"># py code or cli args should define settings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="nam">text</span> <span class="op">=</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="key">return</span> <span class="nam">handle_cli</span><span class="op">(</span><span class="nam">text</span><span class="op">,</span> <span class="nam">db_type</span><span class="op">,</span> <span class="nam">args</span><span class="op">.</span><span class="nam">table</span><span class="op">,</span> <span class="nam">verbose</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">verbose</span><span class="op">,</span> <span class="nam">noop</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">noop</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="str">"db_type"</span><span class="op">,</span> <span class="nam">nargs</span><span class="op">=</span><span class="str">"?"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Which database dialect to generate ([blue]postgres, sqlite, mysql[/blue])"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--verbose"</span><span class="op">,</span> <span class="str">"-v"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Show more info"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="str">"--noop"</span><span class="op">,</span> <span class="str">"-n"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Only show code, don't run it."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="str">"--magic"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"Perform magic to fix missing vars."</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">BooleanOptionalAction</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="str">"-t"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="str">"--table"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="str">"--tables"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">action</span><span class="op">=</span><span class="str">"append"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">nargs</span><span class="op">=</span><span class="str">"+"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"One or more tables to generate. By default, all tables in the file will be used."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="nam">parser</span><span class="op">.</span><span class="nam">parse_args</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span> <span class="key">or</span> <span class="nam">args</span><span class="op">.</span><span class="nam">filename</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="nam">load_file_mode</span> <span class="op">=</span> <span class="op">(</span><span class="nam">filename</span> <span class="op">:=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">filename</span><span class="op">)</span> <span class="key">and</span> <span class="nam">filename</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">".py"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">has_stdin_data</span><span class="op">(</span><span class="op">)</span> <span class="key">or</span> <span class="nam">load_file_mode</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">db_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">Prompt</span><span class="op">.</span><span class="nam">ask</span><span class="op">(</span><span class="str">"Which database type do you want to use?"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"sqlite"</span><span class="op">,</span> <span class="str">"postgres"</span><span class="op">,</span> <span class="str">"mysql"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="nam">rich</span><span class="op">.</span><span class="nam">print</span><span class="op">(</span><span class="str">"Please paste your define tables code below and press ctrl-D when finished."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="com"># else: data from stdin</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="com"># py code or cli args should define settings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">if</span> <span class="nam">load_file_mode</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">args</span><span class="op">.</span><span class="nam">db_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">pathlib</span><span class="op">.</span><span class="nam">Path</span><span class="op">(</span><span class="nam">filename</span><span class="op">)</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">stdin</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">return</span> <span class="nam">handle_cli</span><span class="op">(</span><span class="nam">text</span><span class="op">,</span> <span class="nam">db_type</span><span class="op">,</span> <span class="nam">args</span><span class="op">.</span><span class="nam">table</span><span class="op">,</span> <span class="nam">verbose</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">verbose</span><span class="op">,</span> <span class="nam">noop</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">noop</span><span class="op">,</span> <span class="nam">magic</span><span class="op">=</span><span class="nam">args</span><span class="op">.</span><span class="nam">magic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:05 +0200
+            created at 2023-07-20 20:24 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,169 +5,210 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 16 statements   16 run 0 missing 22 excluded *****
+***** 28 statements   28 run 0 missing 29 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 17:05 +0200
+at 2023-07-20 20:24 +0200
 
 
 1""" 
 2CLI tool to generate SQL from PyDAL code. 
 3""" 
 4 
 5import argparse 
-6import select 
-7import string 
-8import sys 
-9import textwrap 
-10from typing import IO, Optional 
-11 
-12import rich 
-13from rich.prompt import Prompt 
-14 
-15from .helpers import flatten 
-16 
-17 
-18class PrettyParser(argparse.ArgumentParser): # pragma: no cover 
-19 """ 
-20 Add 'rich' to the argparse output. 
+6import pathlib 
+7import select 
+8import string 
+9import sys 
+10import textwrap 
+11from typing import IO, Optional 
+12 
+13import rich 
+14from rich.prompt import Prompt 
+15 
+16from .helpers import flatten 
+17from .magic import find_missing_variables, generate_magic_code 
+18 
+19 
+20class PrettyParser(argparse.ArgumentParser): # pragma: no cover 
 21 """ 
-22 
-23 def _print_message(self, message: str, file: Optional[IO[str]] = None) -
+22 Add 'rich' to the argparse output. 
+23 """ 
+24 
+25 def _print_message(self, message: str, file: Optional[IO[str]] = None) -
 > None: 
-24 rich.print(message, file=file) 
-25 
-26 
-27def has_stdin_data() -> bool: # pragma: no cover 
-28 """ 
-29 Check if the program starts with cli data (pipe | or redirect ><). 
-30 
-31 See Also: 
-32 https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-
+26 rich.print(message, file=file) 
+27 
+28 
+29def has_stdin_data() -> bool: # pragma: no cover 
+30 """ 
+31 Check if the program starts with cli data (pipe | or redirect ><). 
+32 
+33 See Also: 
+34 https://stackoverflow.com/questions/3762881/how-do-i-check-if-stdin-has-
 some-data 
-33 """ 
-34 return any( 
-35 select.select( 
-36 [ 
-37 sys.stdin, 
-38 ], 
-39 [], 
-40 [], 
-41 0.0, 
-42 )[0] 
-43 ) 
-44 
-45 
-46def handle_cli( 
-47 code: str, 
-48 db_type: str = None, 
-49 tables: list[list[str]] = None, 
-50 verbose: bool = False, 
-51 noop: bool = False, 
-52) -> None: 
-53 """ 
-54 Handle user input. 
-55 """ 
-56 to_execute = string.Template( 
-57 textwrap.dedent( 
+35 """ 
+36 return any( 
+37 select.select( 
+38 [ 
+39 sys.stdin, 
+40 ], 
+41 [], 
+42 [], 
+43 0.0, 
+44 )[0] 
+45 ) 
+46 
+47 
+48def handle_cli( 
+49 code: str, 
+50 db_type: str = None, 
+51 tables: list[list[str]] = None, 
+52 verbose: bool = False, 
+53 noop: bool = False, 
+54 magic: bool = False, 
+55) -> None: 
+56 """ 
+57 Handle user input. 
 58 """ 
-59 from pydal import * 
-60 from pydal.objects import * 
-61 from pydal.validators import * 
-62 
-63 from pydal2sql import generate_sql 
-64 
-65 db = database = DAL(None, migrate=False) 
-66 
-67 tables = $tables 
-68 db_type = '$db_type' 
+59 to_execute = string.Template( 
+60 textwrap.dedent( 
+61 """ 
+62 from pydal import * 
+63 from pydal.objects import * 
+64 from pydal.validators import * 
+65 
+66 from pydal2sql import generate_sql 
+67 
+68 db = database = DAL(None, migrate=False) 
 69 
-70 $code 
-71 
-72 if not tables: 
-73 tables = db._tables 
+70 tables = $tables 
+71 db_type = '$db_type' 
+72 
+73 $extra 
 74 
-75 for table in tables: 
-76 print(generate_sql(db[table], db_type)) 
-77 """ 
-78 ) 
-79 ) 
-80 
-81 generated_code = to_execute.substitute( 
-82 { 
-83 "tables": flatten(tables or []), 
-84 "db_type": db_type or "", 
-85 "code": textwrap.dedent(code), 
-86 } 
-87 ) 
-88 if verbose or noop: 
-89 rich.print(generated_code, file=sys.stderr) 
-90 
-91 if not noop: 
-92 exec(generated_code) # nosec: B102 
-93 
-94 
-95def app() -> None: # pragma: no cover 
-96 """ 
-97 Entrypoint for the pydal2sql cli command. 
-98 """ 
-99 parser = PrettyParser( 
-100 prog="pydal2sql", 
-101 formatter_class=argparse.RawDescriptionHelpFormatter, 
-102 description="""[green]CLI tool to generate SQL from PyDAL code.[/green]\n 
-103 Aside from using cli arguments, you can also configure the tool in your
+75 $code 
+76 
+77 if not tables: 
+78 tables = db._tables 
+79 
+80 for table in tables: 
+81 print(generate_sql(db[table], db_type)) 
+82 """ 
+83 ) 
+84 ) 
+85 
+86 generated_code = to_execute.substitute( 
+87 {"tables": flatten(tables or []), "db_type": db_type or "", "code":
+textwrap.dedent(code), "extra": ""} 
+88 ) 
+89 if verbose or noop: 
+90 rich.print(generated_code, file=sys.stderr) 
+91 
+92 if not noop: 
+93 try: 
+94 exec(generated_code) # nosec: B102 
+95 except NameError: 
+96 # something is missing! 
+97 missing_vars = find_missing_variables(generated_code) 
+98 if not magic: 
+99 rich.print( 
+100 f"Your code is missing some variables: {missing_vars}. Add these or try --
+magic", file=sys.stderr 
+101 ) 
+102 else: 
+103 extra_code = generate_magic_code(missing_vars) 
+104 
+105 generated_code = to_execute.substitute( 
+106 { 
+107 "tables": flatten(tables or []), 
+108 "db_type": db_type or "", 
+109 "extra": extra_code, 
+110 "code": textwrap.dedent(code), 
+111 } 
+112 ) 
+113 
+114 if verbose: 
+115 print(generated_code, file=sys.stderr) 
+116 
+117 exec(generated_code) # nosec: B102 
+118 
+119 
+120def app() -> None: # pragma: no cover 
+121 """ 
+122 Entrypoint for the pydal2sql cli command. 
+123 """ 
+124 parser = PrettyParser( 
+125 prog="pydal2sql", 
+126 formatter_class=argparse.RawDescriptionHelpFormatter, 
+127 description="""[green]CLI tool to generate SQL from PyDAL code.[/green]\n 
+128 Aside from using cli arguments, you can also configure the tool in your
 code. 
-104 You can set the following variables: 
-105 
-106 db_type: str = 'sqlite' # your desired database type; 
-107 tables: list[str] = [] # your desired tables to generate SQL for;""", 
-108 epilog="Example: [i]cat models.py | pydal2sql sqlite[/i]", 
-109 ) 
-110 
-111 parser.add_argument( 
-112 "db_type", nargs="?", help="Which database dialect to generate (
+129 You can set the following variables: 
+130 
+131 db_type: str = 'sqlite' # your desired database type; 
+132 tables: list[str] = [] # your desired tables to generate SQL for;""", 
+133 epilog="Example: [i]cat models.py | pydal2sql sqlite[/i]", 
+134 ) 
+135 
+136 parser.add_argument("filename", nargs="?", help="Which file to load? Can
+also be done with stdin.") 
+137 
+138 parser.add_argument( 
+139 "db_type", nargs="?", help="Which database dialect to generate (
 [blue]postgres, sqlite, mysql[/blue])" 
-113 ) 
-114 
-115 parser.add_argument("--verbose", "-v", help="Show more info",
+140 ) 
+141 
+142 parser.add_argument("--verbose", "-v", help="Show more info",
 action=argparse.BooleanOptionalAction, default=False) 
-116 
-117 parser.add_argument( 
-118 "--noop", "-n", help="Only show code, don't run it.",
+143 
+144 parser.add_argument( 
+145 "--noop", "-n", help="Only show code, don't run it.",
 action=argparse.BooleanOptionalAction, default=False 
-119 ) 
-120 
-121 parser.add_argument( 
-122 "-t", 
-123 "--table", 
-124 "--tables", 
-125 action="append", 
-126 nargs="+", 
-127 help="One or more tables to generate. By default, all tables in the file
+146 ) 
+147 
+148 parser.add_argument( 
+149 "--magic", "-m", help="Perform magic to fix missing vars.",
+action=argparse.BooleanOptionalAction, default=False 
+150 ) 
+151 
+152 parser.add_argument( 
+153 "-t", 
+154 "--table", 
+155 "--tables", 
+156 action="append", 
+157 nargs="+", 
+158 help="One or more tables to generate. By default, all tables in the file
 will be used.", 
-128 ) 
-129 
-130 args = parser.parse_args() 
-131 
-132 db_type = args.db_type 
-133 
-134 if not has_stdin_data(): 
-135 if not db_type: 
-136 db_type = Prompt.ask("Which database type do you want to use?", choices=
+159 ) 
+160 
+161 args = parser.parse_args() 
+162 
+163 db_type = args.db_type or args.filename 
+164 
+165 load_file_mode = (filename := args.filename) and filename.endswith(".py") 
+166 
+167 if not (has_stdin_data() or load_file_mode): 
+168 if not db_type: 
+169 db_type = Prompt.ask("Which database type do you want to use?", choices=
 ["sqlite", "postgres", "mysql"]) 
-137 
-138 rich.print("Please paste your define tables code below and press ctrl-
+170 
+171 rich.print("Please paste your define tables code below and press ctrl-
 D when finished.", file=sys.stderr) 
-139 
-140 # else: data from stdin 
-141 # py code or cli args should define settings. 
-142 
-143 text = sys.stdin.read() 
-144 return handle_cli(text, db_type, args.table, verbose=args.verbose,
-noop=args.noop) 
+172 
+173 # else: data from stdin 
+174 # py code or cli args should define settings. 
+175 if load_file_mode: 
+176 db_type = args.db_type 
+177 text = pathlib.Path(filename).read_text() 
+178 else: 
+179 text = sys.stdin.read() 
+180 
+181 return handle_cli(text, db_type, args.table, verbose=args.verbose,
+noop=args.noop, magic=args.magic) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 17:05 +0200
+at 2023-07-20 20:24 +0200
```

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_core_py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_core_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:06 +0200
+            created at 2023-07-20 20:23 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -151,36 +151,37 @@
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="str">        However, your db_type can differ from the current database used.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">        You can even use a dummy database to generate SQL code with:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">        `db = pydal.DAL(None, migrate=False)`</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">    db_folder is the database folder where migration (`.table`) files are stored.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">        By default, a random temporary dir is created.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">if</span> <span class="nam">db_type</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">db_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">db_type</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">define_table</span><span class="op">.</span><span class="nam">_db</span><span class="op">,</span> <span class="str">"_dbname"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">if</span> <span class="nam">db_type</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Please manually define a database type!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">with</span> <span class="nam">TempdirOrExistingDir</span><span class="op">(</span><span class="nam">db_folder</span><span class="op">)</span> <span class="key">as</span> <span class="nam">db_folder</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">migrator</span> <span class="op">=</span> <span class="nam">_build_dummy_migrator</span><span class="op">(</span><span class="nam">db_type</span><span class="op">,</span> <span class="nam">db_folder</span><span class="op">=</span><span class="nam">db_folder</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">sql</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">migrator</span><span class="op">.</span><span class="nam">create_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="nam">define_table</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">migrate</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="nam">fake_migrate</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="key">return</span> <span class="nam">sql</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="key">if</span> <span class="nam">db_type</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Database dialect could not be guessed from code; Please manually define a database type!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">with</span> <span class="nam">TempdirOrExistingDir</span><span class="op">(</span><span class="nam">db_folder</span><span class="op">)</span> <span class="key">as</span> <span class="nam">db_folder</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">migrator</span> <span class="op">=</span> <span class="nam">_build_dummy_migrator</span><span class="op">(</span><span class="nam">db_type</span><span class="op">,</span> <span class="nam">db_folder</span><span class="op">=</span><span class="nam">db_folder</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">sql</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">migrator</span><span class="op">.</span><span class="nam">create_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">define_table</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="nam">migrate</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">            <span class="nam">fake_migrate</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">return</span> <span class="nam">sql</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:06 +0200
+            created at 2023-07-20 20:23 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 32 statements   32 run 0 missing 2 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 17:06 +0200
+at 2023-07-20 20:23 +0200
 
 
 1""" 
 2Main functionality. 
 3""" 
 4 
 5import typing 
@@ -92,24 +92,26 @@
 70 You can even use a dummy database to generate SQL code with: 
 71 `db = pydal.DAL(None, migrate=False)` 
 72 
 73 db_folder is the database folder where migration (`.table`) files are
 stored. 
 74 By default, a random temporary dir is created. 
 75 """ 
-76 if db_type is None: 
+76 if not db_type: 
 77 db_type = getattr(define_table._db, "_dbname", None) 
-78 if db_type is None: 
-79 raise ValueError("Please manually define a database type!") 
-80 
-81 with TempdirOrExistingDir(db_folder) as db_folder: 
-82 migrator = _build_dummy_migrator(db_type, db_folder=db_folder) 
-83 
-84 sql: str = migrator.create_table( 
-85 define_table, 
-86 migrate=True, 
-87 fake_migrate=True, 
-88 ) 
-89 return sql 
+78 
+79 if db_type is None: 
+80 raise ValueError("Database dialect could not be guessed from code; Please
+manually define a database type!") 
+81 
+82 with TempdirOrExistingDir(db_folder) as db_folder: 
+83 migrator = _build_dummy_migrator(db_type, db_folder=db_folder) 
+84 
+85 sql: str = migrator.create_table( 
+86 define_table, 
+87 migrate=True, 
+88 fake_migrate=True, 
+89 ) 
+90 return sql 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-20 17:06 +0200
+at 2023-07-20 20:23 +0200
```

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/d_8bc7b9c2c0d01e74_types_py.html` & `pydal2sql-0.3.0/htmlcov/d_8bc7b9c2c0d01e74_types_py.html`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/favicon_32.png` & `pydal2sql-0.3.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/index.html` & `pydal2sql-0.3.0/htmlcov/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:06 +0200
+            created at 2023-07-20 20:28 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,18 +73,18 @@
                 <td>5</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_cli_py.html">src/pydal2sql/cli.py</a></td>
-                <td>16</td>
+                <td>28</td>
                 <td>0</td>
-                <td>22</td>
-                <td class="right" data-ratio="16 16">100%</td>
+                <td>29</td>
+                <td class="right" data-ratio="28 28">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_core_py.html">src/pydal2sql/core.py</a></td>
                 <td>32</td>
                 <td>0</td>
                 <td>2</td>
                 <td class="right" data-ratio="32 32">100%</td>
@@ -93,40 +93,47 @@
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_helpers_py.html">src/pydal2sql/helpers.py</a></td>
                 <td>29</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="29 29">100%</td>
             </tr>
             <tr class="file">
+                <td class="name left"><a href="d_8bc7b9c2c0d01e74_magic_py.html">src/pydal2sql/magic.py</a></td>
+                <td>58</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="58 58">100%</td>
+            </tr>
+            <tr class="file">
                 <td class="name left"><a href="d_8bc7b9c2c0d01e74_types_py.html">src/pydal2sql/types.py</a></td>
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>90</td>
+                <td>160</td>
                 <td>0</td>
-                <td>24</td>
-                <td class="right" data-ratio="90 90">100%</td>
+                <td>31</td>
+                <td class="right" data-ratio="160 160">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-20 17:06 +0200
+            created at 2023-07-20 20:28 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_8bc7b9c2c0d01e74_types_py.html"/>
         <a id="nextFileLink" class="nav" href="d_8bc7b9c2c0d01e74___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,21 +2,22 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-07-20 17:06 +0200
+coverage.py_v7.2.7, created at 2023-07-20 20:28 +0200
 
 Module                     statements missing excluded coverage
 src/pydal2sql/__about__.py 1          0       0        100%
 src/pydal2sql/__init__.py  5          0       0        100%
-src/pydal2sql/cli.py       16         0       22       100%
+src/pydal2sql/cli.py       28         0       29       100%
 src/pydal2sql/core.py      32         0       2        100%
 src/pydal2sql/helpers.py   29         0       0        100%
+src/pydal2sql/magic.py     58         0       0        100%
 src/pydal2sql/types.py     7          0       0        100%
-Total                      90         0       24       100%
+Total                      160        0       31       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-07-20 17:06 +0200
+coverage.py_v7.2.7, created at 2023-07-20 20:28 +0200
  ____
```

### Comparing `pydal2sql-0.2.3/htmlcov/keybd_closed.png` & `pydal2sql-0.3.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/keybd_open.png` & `pydal2sql-0.3.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/htmlcov/status.json` & `pydal2sql-0.3.0/htmlcov/status.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975297619047619%*

 * *Differences: {"'files'": "{'d_8bc7b9c2c0d01e74___about___py': {'hash': 'f8f1e1d653598950fd214fe7148d3ce5'}, "*

 * *            "'d_8bc7b9c2c0d01e74_core_py': {'hash': 'e894cc475c49f167f090bde99e7ebec2'}, "*

 * *            "'d_8bc7b9c2c0d01e74_cli_py': {'hash': '7773c51a1e8e8c8fd3e312f193802ef2', 'index': "*

 * *            "{'nums': {insert: [(2, 28), (3, 29)], delete: [3, 2]}}}, "*

 * *            "'d_8bc7b9c2c0d01e74_magic_py': OrderedDict([('hash', "*

 * *            "'6451df20c0fd7823828282fd793bd339'), ('index', OrderedDict([('nums', [0,  […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_8bc7b9c2c0d01e74___about___py": {
-            "hash": "3592b798a3808739f1f5987a6cc3d40e",
+            "hash": "f8f1e1d653598950fd214fe7148d3ce5",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -31,32 +31,32 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/__init__.py"
             }
         },
         "d_8bc7b9c2c0d01e74_cli_py": {
-            "hash": "3e94b7d647e852520b2ef3bb2b22130b",
+            "hash": "7773c51a1e8e8c8fd3e312f193802ef2",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    16,
-                    22,
+                    28,
+                    29,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/cli.py"
             }
         },
         "d_8bc7b9c2c0d01e74_core_py": {
-            "hash": "2328f23ef6330c30c0f195de355d5b5d",
+            "hash": "e894cc475c49f167f090bde99e7ebec2",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74_core_py.html",
                 "nums": [
                     0,
                     1,
                     32,
                     2,
@@ -81,14 +81,31 @@
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/pydal2sql/helpers.py"
             }
         },
+        "d_8bc7b9c2c0d01e74_magic_py": {
+            "hash": "6451df20c0fd7823828282fd793bd339",
+            "index": {
+                "html_filename": "d_8bc7b9c2c0d01e74_magic_py.html",
+                "nums": [
+                    0,
+                    1,
+                    58,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/pydal2sql/magic.py"
+            }
+        },
         "d_8bc7b9c2c0d01e74_types_py": {
             "hash": "38b7f79d811770970b84d0f66578713a",
             "index": {
                 "html_filename": "d_8bc7b9c2c0d01e74_types_py.html",
                 "nums": [
                     0,
                     1,
```

### Comparing `pydal2sql-0.2.3/htmlcov/style.css` & `pydal2sql-0.3.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/src/pydal2sql/cli.py` & `pydal2sql-0.3.0/src/pydal2sql/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 CLI tool to generate SQL from PyDAL code.
 """
 
 import argparse
+import pathlib
 import select
 import string
 import sys
 import textwrap
 from typing import IO, Optional
 
 import rich
 from rich.prompt import Prompt
 
 from .helpers import flatten
+from .magic import find_missing_variables, generate_magic_code
 
 
 class PrettyParser(argparse.ArgumentParser):  # pragma: no cover
     """
     Add 'rich' to the argparse output.
     """
 
@@ -45,14 +47,15 @@
 
 def handle_cli(
     code: str,
     db_type: str = None,
     tables: list[list[str]] = None,
     verbose: bool = False,
     noop: bool = False,
+    magic: bool = False,
 ) -> None:
     """
     Handle user input.
     """
     to_execute = string.Template(
         textwrap.dedent(
             """
@@ -63,37 +66,59 @@
         from pydal2sql import generate_sql
 
         db = database = DAL(None, migrate=False)
 
         tables = $tables
         db_type = '$db_type'
 
+        $extra
+
         $code
 
         if not tables:
             tables = db._tables
 
         for table in tables:
             print(generate_sql(db[table], db_type))
     """
         )
     )
 
     generated_code = to_execute.substitute(
-        {
-            "tables": flatten(tables or []),
-            "db_type": db_type or "",
-            "code": textwrap.dedent(code),
-        }
+        {"tables": flatten(tables or []), "db_type": db_type or "", "code": textwrap.dedent(code), "extra": ""}
     )
     if verbose or noop:
         rich.print(generated_code, file=sys.stderr)
 
     if not noop:
-        exec(generated_code)  # nosec: B102
+        try:
+            exec(generated_code)  # nosec: B102
+        except NameError:
+            # something is missing!
+            missing_vars = find_missing_variables(generated_code)
+            if not magic:
+                rich.print(
+                    f"Your code is missing some variables: {missing_vars}. Add these or try --magic", file=sys.stderr
+                )
+            else:
+                extra_code = generate_magic_code(missing_vars)
+
+                generated_code = to_execute.substitute(
+                    {
+                        "tables": flatten(tables or []),
+                        "db_type": db_type or "",
+                        "extra": extra_code,
+                        "code": textwrap.dedent(code),
+                    }
+                )
+
+                if verbose:
+                    print(generated_code, file=sys.stderr)
+
+                exec(generated_code)  # nosec: B102
 
 
 def app() -> None:  # pragma: no cover
     """
     Entrypoint for the pydal2sql cli command.
     """
     parser = PrettyParser(
@@ -104,41 +129,53 @@
         You can set the following variables:
 
         db_type: str = 'sqlite' # your desired database type;
         tables: list[str] = []  # your desired tables to generate SQL for;""",
         epilog="Example: [i]cat models.py | pydal2sql sqlite[/i]",
     )
 
+    parser.add_argument("filename", nargs="?", help="Which file to load? Can also be done with stdin.")
+
     parser.add_argument(
         "db_type", nargs="?", help="Which database dialect to generate ([blue]postgres, sqlite, mysql[/blue])"
     )
 
     parser.add_argument("--verbose", "-v", help="Show more info", action=argparse.BooleanOptionalAction, default=False)
 
     parser.add_argument(
         "--noop", "-n", help="Only show code, don't run it.", action=argparse.BooleanOptionalAction, default=False
     )
 
     parser.add_argument(
+        "--magic", "-m", help="Perform magic to fix missing vars.", action=argparse.BooleanOptionalAction, default=False
+    )
+
+    parser.add_argument(
         "-t",
         "--table",
         "--tables",
         action="append",
         nargs="+",
         help="One or more tables to generate. By default, all tables in the file will be used.",
     )
 
     args = parser.parse_args()
 
-    db_type = args.db_type
+    db_type = args.db_type or args.filename
+
+    load_file_mode = (filename := args.filename) and filename.endswith(".py")
 
-    if not has_stdin_data():
+    if not (has_stdin_data() or load_file_mode):
         if not db_type:
             db_type = Prompt.ask("Which database type do you want to use?", choices=["sqlite", "postgres", "mysql"])
 
         rich.print("Please paste your define tables code below and press ctrl-D when finished.", file=sys.stderr)
 
     # else: data from stdin
     # py code or cli args should define settings.
+    if load_file_mode:
+        db_type = args.db_type
+        text = pathlib.Path(filename).read_text()
+    else:
+        text = sys.stdin.read()
 
-    text = sys.stdin.read()
-    return handle_cli(text, db_type, args.table, verbose=args.verbose, noop=args.noop)
+    return handle_cli(text, db_type, args.table, verbose=args.verbose, noop=args.noop, magic=args.magic)
```

### Comparing `pydal2sql-0.2.3/src/pydal2sql/core.py` & `pydal2sql-0.3.0/src/pydal2sql/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     db_folder is the database folder where migration (`.table`) files are stored.
         By default, a random temporary dir is created.
     """
     if not db_type:
         db_type = getattr(define_table._db, "_dbname", None)
 
         if db_type is None:
-            raise ValueError("Please manually define a database type!")
+            raise ValueError("Database dialect could not be guessed from code; Please manually define a database type!")
 
     with TempdirOrExistingDir(db_folder) as db_folder:
         migrator = _build_dummy_migrator(db_type, db_folder=db_folder)
 
         sql: str = migrator.create_table(
             define_table,
             migrate=True,
```

### Comparing `pydal2sql-0.2.3/src/pydal2sql/helpers.py` & `pydal2sql-0.3.0/src/pydal2sql/helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/tests/test_core.py` & `pydal2sql-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/tests/test_helpers.py` & `pydal2sql-0.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/LICENSE.txt` & `pydal2sql-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal2sql-0.2.3/README.md` & `pydal2sql-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -56,31 +56,54 @@
 );
 ```
 
 ## Installation
 
 ```console
 pip install pydal2sql
+# or
+pipx install pydal2sql
 ```
 
 ## cli
+
+Given a Python file:
+
 ```python
 # model_fragment.py
 db.define_table(
     "person",
     Field(...)
 )
 
 # optionally:
 # db_type = 'postgres'
 # tables = ['person']
 ```
 
+Then in the terminal:
+
 ```bash
 cat model_fragment.py | pydal2sql # without cli args if settings are set in code, or
 cat model_fragment.py | pydal2sql postgres --table person # with args if settings are not in code
 # both output the CREATE TABLE statements to stdout.
+
+# alternatively, you can simply run `pydal2sql` and you will be prompted for the code, which you can then paste.
 ```
 
+### ⚠️ Experimental 🪄✨Magic🌟💻
+
+If you're copy-pasting some `define_table` statements which have validators or defaults that are defined elsewhere,
+the SQL generation could crash due to msising variables. However, if these variables are irrelevant to the samentics of
+the table definition (i.e. only used at runtime, not for the schema definition), you can now try the `--magic` flag.
+
+This flag will replace all missing variables with a special `Empty` class, which does nothing but
+prevent `NameError`, `AttributeError` and `TypeError`s.   
+This is of course not production-safe, so it shouldn't be used anywhere else.
+
+### Example with pipx
+
+[![asciicast](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby.svg)](https://asciinema.org/a/upl4wB4QPDf9qO278ijWyPMby)
+
 ## License
 
 `pydal2sql` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydal2sql-0.2.3/pyproject.toml` & `pydal2sql-0.3.0/pyproject.toml`

 * *Files identical despite different names*

