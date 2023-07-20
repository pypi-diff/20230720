# Comparing `tmp/pytest-excel-1.5.1.tar.gz` & `tmp/pytest-excel-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-excel-1.5.1.tar", last modified: Thu Jul 20 04:33:06 2023, max compression
+gzip compressed data, was "pytest-excel-1.5.2.tar", last modified: Thu Jul 20 09:52:07 2023, max compression
```

## Comparing `pytest-excel-1.5.1.tar` & `pytest-excel-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 04:33:06.188549 pytest-excel-1.5.1/
--rw-rw-rw-   0        0        0     1064 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/LICENSE
--rw-rw-rw-   0        0        0       76 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1971 2023-07-20 04:33:06.188549 pytest-excel-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-20 04:33:06.058949 pytest-excel-1.5.1/pytest_excel/
--rw-rw-rw-   0        0        0        0 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/pytest_excel/__init__.py
--rw-rw-rw-   0        0        0     7171 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/pytest_excel/pytest_excel.py
-drwxrwxrwx   0        0        0        0 2023-07-20 04:33:06.180523 pytest-excel-1.5.1/pytest_excel.egg-info/
--rw-rw-rw-   0        0        0     1971 2023-07-20 04:33:04.000000 pytest-excel-1.5.1/pytest_excel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-20 04:33:05.000000 pytest-excel-1.5.1/pytest_excel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 04:33:04.000000 pytest-excel-1.5.1/pytest_excel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-20 04:33:04.000000 pytest-excel-1.5.1/pytest_excel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-07-20 04:33:04.000000 pytest-excel-1.5.1/pytest_excel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 04:33:04.000000 pytest-excel-1.5.1/pytest_excel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-20 04:33:06.188549 pytest-excel-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-07-20 04:30:05.000000 pytest-excel-1.5.1/setup.py
--rw-rw-rw-   0        0        0      885 2023-07-20 04:26:11.000000 pytest-excel-1.5.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-20 09:52:06.968527 pytest-excel-1.5.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-20 09:40:20.000000 pytest-excel-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-07-20 09:40:20.000000 pytest-excel-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1971 2023-07-20 09:52:06.969529 pytest-excel-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-07-20 09:40:20.000000 pytest-excel-1.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-20 09:52:06.898526 pytest-excel-1.5.2/pytest_excel/
+-rw-rw-rw-   0        0        0        0 2023-07-20 09:40:20.000000 pytest-excel-1.5.2/pytest_excel/__init__.py
+-rw-rw-rw-   0        0        0     7418 2023-07-20 09:43:17.000000 pytest-excel-1.5.2/pytest_excel/pytest_excel.py
+drwxrwxrwx   0        0        0        0 2023-07-20 09:52:06.963529 pytest-excel-1.5.2/pytest_excel.egg-info/
+-rw-rw-rw-   0        0        0     1971 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-20 09:52:06.000000 pytest-excel-1.5.2/pytest_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-20 09:52:06.978529 pytest-excel-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-07-20 09:46:27.000000 pytest-excel-1.5.2/setup.py
+-rw-rw-rw-   0        0        0      909 2023-07-20 09:40:20.000000 pytest-excel-1.5.2/tox.ini
```

### Comparing `pytest-excel-1.5.1/LICENSE` & `pytest-excel-1.5.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 santosh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 santosh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pytest-excel-1.5.1/PKG-INFO` & `pytest-excel-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-excel
-Version: 1.5.1
+Version: 1.5.2
 Summary: pytest plugin for generating excel reports
 Home-page: https://github.com/ssrikanta/pytest-excel
 Author: santosh
 Author-email: santosh.srikanta@gmail.com
 License: MIT
 Keywords: py.test pytest excel report
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-excel-1.5.1/pytest_excel.egg-info/PKG-INFO` & `pytest-excel-1.5.2/pytest_excel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-excel
-Version: 1.5.1
+Version: 1.5.2
 Summary: pytest plugin for generating excel reports
 Home-page: https://github.com/ssrikanta/pytest-excel
 Author: santosh
 Author-email: santosh.srikanta@gmail.com
 License: MIT
 Keywords: py.test pytest excel report
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-excel-1.5.1/setup.py` & `pytest-excel-1.5.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
-import re
-import io
-
-from setuptools import setup
-
-
-
-setup(name='pytest-excel',
-      version='1.5.1',
-      description='pytest plugin for generating excel reports',
-      long_description=io.open('README.rst', encoding='utf-8', errors='ignore').read(),
-      author='santosh',
-      author_email=u'santosh.srikanta@gmail.com',
-      url=u'https://github.com/ssrikanta/pytest-excel',
-      license = 'MIT',
-      license_file = 'LICENSE',
-      packages=['pytest_excel'],
-      entry_points={'pytest11': ['excel = pytest_excel.pytest_excel']},
-      install_requires=['pytest>=3.6', 'openpyxl'],
-      keywords='py.test pytest excel report',
-      classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'Framework :: Pytest',
-          'Intended Audience :: Developers',
-          ' License :: OSI Approved :: MIT License',
-          'Operating System :: POSIX',
-          'Operating System :: Microsoft :: Windows',
-          'Operating System :: MacOS :: MacOS X',
-          'Topic :: Software Development :: Testing',
-          'Topic :: Software Development :: Quality Assurance',
-          'Topic :: Software Development :: Libraries',
-          'Topic :: Utilities',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11',
-      ]
-      )
-
+import os
+import re
+import io
+
+from setuptools import setup
+
+
+
+setup(name='pytest-excel',
+      version='1.5.2',
+      description='pytest plugin for generating excel reports',
+      long_description=io.open('README.rst', encoding='utf-8', errors='ignore').read(),
+      author='santosh',
+      author_email=u'santosh.srikanta@gmail.com',
+      url=u'https://github.com/ssrikanta/pytest-excel',
+      license = 'MIT',
+      license_file = 'LICENSE',
+      packages=['pytest_excel'],
+      entry_points={'pytest11': ['excel = pytest_excel.pytest_excel']},
+      install_requires=['pytest>=3.6', 'openpyxl'],
+      keywords='py.test pytest excel report',
+      classifiers=[
+          'Development Status :: 5 - Production/Stable',
+          'Framework :: Pytest',
+          'Intended Audience :: Developers',
+          ' License :: OSI Approved :: MIT License',
+          'Operating System :: POSIX',
+          'Operating System :: Microsoft :: Windows',
+          'Operating System :: MacOS :: MacOS X',
+          'Topic :: Software Development :: Testing',
+          'Topic :: Software Development :: Quality Assurance',
+          'Topic :: Software Development :: Libraries',
+          'Topic :: Utilities',
+          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
+      ]
+      )
+
```

