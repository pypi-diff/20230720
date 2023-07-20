# Comparing `tmp/fake_winreg-1.6.2.2.tar.gz` & `tmp/fake_winreg-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake_winreg-1.6.2.2.tar", last modified: Thu Jun  2 07:46:00 2022, max compression
+gzip compressed data, was "fake_winreg-1.6.3.tar", last modified: Thu Jul 20 09:37:37 2023, max compression
```

## Comparing `fake_winreg-1.6.2.2.tar` & `fake_winreg-1.6.3.tar`

### file list

```diff
@@ -1,28 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    82326 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    81648 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8095 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/fake_reg.py
--rw-r--r--   0 runner    (1001) docker     (121)     5709 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/fake_reg_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    84542 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/fake_winreg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/fake_winreg_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/registry_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/fake_winreg/types_custom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    82326 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 07:45:57.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/fake_winreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-02 07:46:00.000000 fake_winreg-1.6.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-06-02 07:45:06.000000 fake_winreg-1.6.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.630098 fake_winreg-1.6.3/.3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.3rd_party_stubs/wrapt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.630098 fake_winreg-1.6.3/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/commandline_help.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.626098 fake_winreg-1.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.630098 fake_winreg-1.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    83415 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    82451 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.630098 fake_winreg-1.6.3/fake_winreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/fake_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/fake_reg_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84542 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/fake_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/fake_winreg_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/registry_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg/types_custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/fake_winreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    83415 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 09:37:37.000000 fake_winreg-1.6.3/fake_winreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/fake_winreg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:37:37.634098 fake_winreg-1.6.3/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-20 09:36:47.000000 fake_winreg-1.6.3/tests/test_set_value_ex.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fake_winreg-1.6.2.2/CHANGES.rst` & `fake_winreg-1.6.3/CHANGES.rst`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,34 @@
 planned:
     - KEY_* Permissions on SetValue, ReadValue, etc ...
     - test matrix on windows to compare fake and original winreg in detail
     - auditing events
     - investigate SYSWOW32/64 Views
     - Admin Permissions
 
+v1.6.3
+---------
+2023-07-20:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.6.2.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
 
 v1.6.2.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `fake_winreg-1.6.2.2/LICENSE` & `fake_winreg-1.6.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 1990-2022 Robert Nowotny
+Copyright (c) 1990-2023 Robert Nowotny
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fake_winreg-1.6.2.2/PKG-INFO` & `fake_winreg-1.6.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,70 +1,51 @@
-Metadata-Version: 2.1
-Name: fake_winreg
-Version: 1.6.2.2
-Summary: fake winreg, in order to test registry related functions on linux
-Home-page: https://github.com/bitranox/fake_winreg
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 fake_winreg
 ===========
 
 
-Version v1.6.2.2 as of 2022-06-02 see `Changelog`_
-
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
+Version v1.6.3 as of 2023-07-20 see `Changelog`_
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/fake_winreg/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/fake_winreg/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/fake_winreg/master?filepath=fake_winreg.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/fake-winreg?label=PyPI%20Package
    :target: https://badge.fury.io/py/fake_winreg
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/fake_winreg
    :target: https://codecov.io/gh/bitranox/fake_winreg
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/fake_winreg?branch=master
-   :target: https://bettercodehub.com/results/bitranox/fake_winreg
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/fake_winreg?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/fake_winreg?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/fake_winreg?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/fake_winreg/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/fake_winreg
+.. |snyk| image:: https://snyk.io/test/github/bitranox/fake_winreg/badge.svg
    :target: https://snyk.io/test/github/bitranox/fake_winreg
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/fake-winreg
    :target: https://pypi.org/project/fake-winreg/
@@ -107,22 +88,22 @@
 - some (few) winreg functions are not implemented - if You miss out something, give me a note, i will integrate it
 - obviously we can not connect to the registry of another windows computer over the network
 - KEY_WOW64_32KEY is not supported. We show always the same ...
 - auditing event's are not supported
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/fake_winreg>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/fake_winreg/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -2060,14 +2041,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade fake_winreg
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade fake_winreg[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/fake_winreg.git
 
@@ -2083,22 +2071,22 @@
     # for the latest development version :
     fake_winreg @ git+https://github.com/bitranox/fake_winreg.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/fake_winreg.git
     $ cd fake_winreg
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -2158,14 +2146,34 @@
 planned:
     - KEY_* Permissions on SetValue, ReadValue, etc ...
     - test matrix on windows to compare fake and original winreg in detail
     - auditing events
     - investigate SYSWOW32/64 Views
     - Admin Permissions
 
+v1.6.3
+---------
+2023-07-20:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.6.2.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
 
 v1.6.2.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `fake_winreg-1.6.2.2/README.rst` & `fake_winreg-1.6.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,73 @@
+Metadata-Version: 2.1
+Name: fake_winreg
+Version: 1.6.3
+Summary: fake winreg, in order to test registry related functions on linux
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/fake_winreg
+Project-URL: Documentation, https://github.com/bitranox/fake_winreg/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/fake_winreg.git
+Project-URL: Changelog, https://github.com/bitranox/fake_winreg/blob/master/CHANGES.rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8.0
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 fake_winreg
 ===========
 
 
-Version v1.6.2.2 as of 2022-06-02 see `Changelog`_
-
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
+Version v1.6.3 as of 2023-07-20 see `Changelog`_
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/fake_winreg/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/fake_winreg/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/fake_winreg/master?filepath=fake_winreg.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/fake-winreg?label=PyPI%20Package
    :target: https://badge.fury.io/py/fake_winreg
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/fake_winreg
    :target: https://codecov.io/gh/bitranox/fake_winreg
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/fake_winreg?branch=master
-   :target: https://bettercodehub.com/results/bitranox/fake_winreg
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/fake_winreg?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/fake_winreg?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/fake_winreg?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/fake_winreg/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/fake_winreg
+.. |snyk| image:: https://snyk.io/test/github/bitranox/fake_winreg/badge.svg
    :target: https://snyk.io/test/github/bitranox/fake_winreg
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/fake-winreg
    :target: https://pypi.org/project/fake-winreg/
@@ -89,22 +110,22 @@
 - some (few) winreg functions are not implemented - if You miss out something, give me a note, i will integrate it
 - obviously we can not connect to the registry of another windows computer over the network
 - KEY_WOW64_32KEY is not supported. We show always the same ...
 - auditing event's are not supported
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/fake_winreg>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/fake_winreg/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -2042,14 +2063,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade fake_winreg
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade fake_winreg[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/fake_winreg.git
 
@@ -2065,22 +2093,22 @@
     # for the latest development version :
     fake_winreg @ git+https://github.com/bitranox/fake_winreg.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/fake_winreg.git
     $ cd fake_winreg
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -2140,14 +2168,34 @@
 planned:
     - KEY_* Permissions on SetValue, ReadValue, etc ...
     - test matrix on windows to compare fake and original winreg in detail
     - auditing events
     - investigate SYSWOW32/64 Views
     - Admin Permissions
 
+v1.6.3
+---------
+2023-07-20:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.6.2.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
 
 v1.6.2.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `fake_winreg-1.6.2.2/fake_winreg/fake_reg.py` & `fake_winreg-1.6.3/fake_winreg/fake_reg.py`

 * *Files identical despite different names*

### Comparing `fake_winreg-1.6.2.2/fake_winreg/fake_reg_tools.py` & `fake_winreg-1.6.3/fake_winreg/fake_reg_tools.py`

 * *Files identical despite different names*

### Comparing `fake_winreg-1.6.2.2/fake_winreg/fake_winreg.py` & `fake_winreg-1.6.3/fake_winreg/fake_winreg.py`

 * *Files identical despite different names*

### Comparing `fake_winreg-1.6.2.2/fake_winreg/fake_winreg_cli.py` & `fake_winreg-1.6.3/fake_winreg/fake_winreg_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)  # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
@@ -45,13 +45,13 @@
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()  # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
```

### Comparing `fake_winreg-1.6.2.2/fake_winreg/helpers.py` & `fake_winreg-1.6.3/fake_winreg/helpers.py`

 * *Files identical despite different names*

### Comparing `fake_winreg-1.6.2.2/fake_winreg/registry_constants.py` & `fake_winreg-1.6.3/fake_winreg/registry_constants.py`

 * *Files identical despite different names*

### Comparing `fake_winreg-1.6.2.2/fake_winreg.egg-info/PKG-INFO` & `fake_winreg-1.6.3/fake_winreg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: fake-winreg
-Version: 1.6.2.2
+Version: 1.6.3
 Summary: fake winreg, in order to test registry related functions on linux
-Home-page: https://github.com/bitranox/fake_winreg
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/fake_winreg
+Project-URL: Documentation, https://github.com/bitranox/fake_winreg/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/fake_winreg.git
+Project-URL: Changelog, https://github.com/bitranox/fake_winreg/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 fake_winreg
 ===========
 
 
-Version v1.6.2.2 as of 2022-06-02 see `Changelog`_
+Version v1.6.3 as of 2023-07-20 see `Changelog`_
 
-|build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
-
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|build_badge| |codeql| |license| |jupyter| |pypi|
+|pypi-downloads| |black| |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml
 
 
+.. |codeql| image:: https://github.com/bitranox/fake_winreg/actions/workflows/codeql-analysis.yml/badge.svg?event=push
+   :target: https://github.com//bitranox/fake_winreg/actions/workflows/codeql-analysis.yml
+
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/bitranox/fake_winreg/master?filepath=fake_winreg.ipynb
 
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/fake-winreg?label=PyPI%20Package
    :target: https://badge.fury.io/py/fake_winreg
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/fake_winreg
    :target: https://codecov.io/gh/bitranox/fake_winreg
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/fake_winreg?branch=master
-   :target: https://bettercodehub.com/results/bitranox/fake_winreg
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/fake_winreg?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/fake_winreg?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/fake_winreg/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/fake_winreg?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/fake_winreg/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/fake_winreg
+.. |snyk| image:: https://snyk.io/test/github/bitranox/fake_winreg/badge.svg
    :target: https://snyk.io/test/github/bitranox/fake_winreg
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/fake-winreg
    :target: https://pypi.org/project/fake-winreg/
@@ -107,22 +110,22 @@
 - some (few) winreg functions are not implemented - if You miss out something, give me a note, i will integrate it
 - obviously we can not connect to the registry of another windows computer over the network
 - KEY_WOW64_32KEY is not supported. We show always the same ...
 - auditing event's are not supported
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.8.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.8, 3.9, 3.10, 3.11, 3.12-dev, pypy-3.9, pypy-3.10 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/fake_winreg>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/fake_winreg/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/fake_winreg/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -2060,14 +2063,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade fake_winreg
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade fake_winreg[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/fake_winreg.git
 
@@ -2083,22 +2093,22 @@
     # for the latest development version :
     fake_winreg @ git+https://github.com/bitranox/fake_winreg.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/fake_winreg.git
     $ cd fake_winreg
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -2158,14 +2168,34 @@
 planned:
     - KEY_* Permissions on SetValue, ReadValue, etc ...
     - test matrix on windows to compare fake and original winreg in detail
     - auditing events
     - investigate SYSWOW32/64 Views
     - Admin Permissions
 
+v1.6.3
+---------
+2023-07-20:
+    - require minimum python 3.8
+    - remove python 3.7 tests
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+    - clean ./tests/test_cli.py
+    - add codeql badge
+    - move 3rd_party_stubs outside the src directory to ``./.3rd_party_stubs``
+    - add pypy 3.10 tests
+    - add python 3.12-dev tests
+
 v1.6.2.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
 
 v1.6.2.1
 --------
 2022-06-01: update github actions test matrix
```

