# Comparing `tmp/micropython-motor-0.1.0.tar.gz` & `tmp/micropython-motor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-motor-0.1.0.tar", last modified: Sun Jul  9 00:02:36 2023, max compression
+gzip compressed data, was "micropython-motor-0.2.0.tar", last modified: Thu Jul 20 15:49:34 2023, max compression
```

## Comparing `micropython-motor-0.1.0.tar` & `micropython-motor-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.635987 micropython-motor-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/examples/motor_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/examples/servo_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/micropython_motor/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/micropython_motor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/micropython_motor/motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/micropython_motor/servo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/micropython_motor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-09 00:02:36.000000 micropython-motor-0.1.0/micropython_motor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-09 00:02:36.000000 micropython-motor-0.1.0/micropython_motor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 00:02:36.000000 micropython-motor-0.1.0/micropython_motor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 00:02:36.000000 micropython-motor-0.1.0/micropython_motor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-09 00:02:28.000000 micropython-motor-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-09 00:02:17.000000 micropython-motor-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 00:02:36.639987 micropython-motor-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.469231 micropython-motor-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.461230 micropython-motor-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.465230 micropython-motor-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 15:49:34.469231 micropython-motor-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.465230 micropython-motor-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.465230 micropython-motor-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.465230 micropython-motor-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/examples/motor_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/examples/servo_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/examples/stepper_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.465230 micropython-motor-0.2.0/micropython_motor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/micropython_motor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/micropython_motor/motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/micropython_motor/servo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/micropython_motor/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:49:34.469231 micropython-motor-0.2.0/micropython_motor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 15:49:34.000000 micropython-motor-0.2.0/micropython_motor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 15:49:34.000000 micropython-motor-0.2.0/micropython_motor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:49:34.000000 micropython-motor-0.2.0/micropython_motor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:49:34.000000 micropython-motor-0.2.0/micropython_motor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-20 15:49:25.000000 micropython-motor-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 15:49:12.000000 micropython-motor-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:49:34.469231 micropython-motor-0.2.0/setup.cfg
```

### Comparing `micropython-motor-0.1.0/.pre-commit-config.yaml` & `micropython-motor-0.2.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `micropython-motor-0.1.0/.pylintrc` & `micropython-motor-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/LICENSE` & `micropython-motor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/PKG-INFO` & `micropython-motor-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-motor
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Helpers for controlling PWM based motors and servos 
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MOTOR
-Keywords: sensor,micropython,motor,micropython,pwm,motor,servo,drv8833
+Keywords: sensor,micropython,motor,pwm,motor,servo,drv8833,stepper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
@@ -45,17 +45,14 @@
 https://github.com/adafruit/Adafruit_CircuitPython_Motor
 
 This library can work with other MCU (Not tested) that used the following PWM methods:
 
 * freq
 * duty_u16
 
-Sadly do not have the hardware to test the step motor part of the library so, this will
-be an exercise for the reader.:)
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-motor-0.1.0/README.rst` & `micropython-motor-0.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 https://github.com/adafruit/Adafruit_CircuitPython_Motor
 
 This library can work with other MCU (Not tested) that used the following PWM methods:
 
 * freq
 * duty_u16
 
-Sadly do not have the hardware to test the step motor part of the library so, this will
-be an exercise for the reader.:)
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-motor-0.1.0/docs/_static/Logo.png` & `micropython-motor-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/docs/_static/favicon.ico` & `micropython-motor-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/docs/conf.py` & `micropython-motor-0.2.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import datetime
@@ -28,15 +26,14 @@
     raise SystemExit("micropython_motor has to be importable")
 
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 intersphinx_mapping = {
@@ -181,17 +178,14 @@
     },
     {
         "name": "important",
         "icon": "material/school",
         "override": True,
     },
 ]
-python_type_aliases = {
-    "DigitalInOut": "digitalio.DigitalInOut",
-}
 
 object_description_options = [
     ("py:.*", dict(generate_synopses="first_sentence")),
 ]
 # Set link name generated in the top bar.
 html_title = "MicroPython MOTOR"
 
@@ -199,65 +193,7 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
 html_css_files = ["extra_css.css"]
-
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "MicroPython_motor_Library.tex",
-        "MicroPython motor Library Documentation",
-        author,
-        "manual",
-    ),
-]
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "MicroPython_motor_Library",
-        "MicroPython motor Library Documentation",
-        [author],
-        1,
-    ),
-]
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "MicroPython_motor_Library",
-        "MicroPython motor Library Documentation",
-        author,
-        "MicroPython_motor_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-motor-0.1.0/examples/motor_simpletest.py` & `micropython-motor-0.2.0/examples/motor_simpletest.py`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/examples/servo_simpletest.py` & `micropython-motor-0.2.0/examples/servo_simpletest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
-from machine import Pin, PWM
 import time
+from machine import Pin, PWM
 from micropython_motor.servo import Servo
 
 servo = PWM(Pin(10, Pin.OUT))
 servo.freq(50)
 
 servo7 = Servo(servo)
 
@@ -21,9 +21,7 @@
 
 # You can also specify the movement fractionally.
 fraction = 0.0
 while fraction < 1.0:
     servo7.fraction = fraction
     fraction += 0.01
     time.sleep(0.06)
-
-
```

### Comparing `micropython-motor-0.1.0/micropython_motor/motor.py` & `micropython-motor-0.2.0/micropython_motor/motor.py`

 * *Files identical despite different names*

### Comparing `micropython-motor-0.1.0/micropython_motor/servo.py` & `micropython-motor-0.2.0/micropython_motor/servo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 """
-`motor`
+`servo`
 ================================================================================
 
 MicroPython Helper for controlling PWM based servos
 
 
 * Author(s): Scott Shawcroft, Jose D. Montoya
```

### Comparing `micropython-motor-0.1.0/micropython_motor.egg-info/PKG-INFO` & `micropython-motor-0.2.0/micropython_motor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-motor
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Helpers for controlling PWM based motors and servos 
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MOTOR
-Keywords: sensor,micropython,motor,micropython,pwm,motor,servo,drv8833
+Keywords: sensor,micropython,motor,pwm,motor,servo,drv8833,stepper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
@@ -45,17 +45,14 @@
 https://github.com/adafruit/Adafruit_CircuitPython_Motor
 
 This library can work with other MCU (Not tested) that used the following PWM methods:
 
 * freq
 * duty_u16
 
-Sadly do not have the hardware to test the step motor part of the library so, this will
-be an exercise for the reader.:)
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-motor-0.1.0/micropython_motor.egg-info/SOURCES.txt` & `micropython-motor-0.2.0/micropython_motor.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/motor_simpletest.py
 examples/servo_simpletest.py
+examples/stepper_simpletest.py
 micropython_motor/__init__.py
 micropython_motor/motor.py
 micropython_motor/servo.py
+micropython_motor/stepper.py
 micropython_motor.egg-info/PKG-INFO
 micropython_motor.egg-info/SOURCES.txt
 micropython_motor.egg-info/dependency_links.txt
 micropython_motor.egg-info/top_level.txt
```

### Comparing `micropython-motor-0.1.0/pyproject.toml` & `micropython-motor-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-motor"
 description = "MicroPython Helpers for controlling PWM based motors and servos "
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MOTOR"}
 keywords = [
     "sensor",
     "micropython",
     "motor",
-    "micropython",
     "pwm",
     "motor",
     "servo",
     "drv8833",
+    "stepper",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
```

