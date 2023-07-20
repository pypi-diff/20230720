# Comparing `tmp/rpi_reactive_gpio-0.1.7.tar.gz` & `tmp/rpi_reactive_gpio-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.7.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.8.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.7.tar` & `rpi_reactive_gpio-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/LICENSE
--rw-r--r--   0        0        0       80 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/README.md
--rw-r--r--   0        0        0      766 2023-06-30 22:31:14.886377 rpi_reactive_gpio-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      207 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1607 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3534 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      482 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      850 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1263 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 18:29:51.210267 rpi_reactive_gpio-0.1.8/LICENSE
+-rw-r--r--   0        0        0       80 2023-07-20 18:29:51.210267 rpi_reactive_gpio-0.1.8/README.md
+-rw-r--r--   0        0        0      768 2023-07-20 18:30:15.362476 rpi_reactive_gpio-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3534 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      482 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1263 2023-07-20 18:29:51.214267 rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.8/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.7/LICENSE` & `rpi_reactive_gpio-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.7/pyproject.toml` & `rpi_reactive_gpio-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.7"
+version = "0.1.8"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
-documentation = "https://github.com/MarkParker5/rpi-reactive-gpio/blob/main/README.md"
+documentation = "https://github.com/MarkParker5/rpi-reactive-gpio/blob/master/README.md"
 keywords = ["raspberry-pi", "gpio", "reactive", "rxpy", "rx", "rpi", "rpi-gpio", "RPi.GPIO"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 raspi-gpio = "^0.1.0"
 
 [tools.mypy]
```

### Comparing `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/buttons.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/leds.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.8/rpi_reactive_gpio/scene.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.7/PKG-INFO` & `rpi_reactive_gpio-0.1.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.7
+Version: 0.1.8
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: raspi-gpio (>=0.1.0,<0.2.0)
-Project-URL: Documentation, https://github.com/MarkParker5/rpi-reactive-gpio/blob/main/README.md
+Project-URL: Documentation, https://github.com/MarkParker5/rpi-reactive-gpio/blob/master/README.md
 Project-URL: Repository, https://github.com/MarkParker5/rpi-reactive-gpio
 Description-Content-Type: text/markdown
 
 # rpi-reactive-gpio
 
 Syntax sugar for controlling RPi.GPIO with reactive design.
```

