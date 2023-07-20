# Comparing `tmp/raspi_gpio-0.1.8.tar.gz` & `tmp/raspi_gpio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.8.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.9.tar", max compression
```

## Comparing `raspi_gpio-0.1.8.tar` & `raspi_gpio-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-19 12:53:45.951187 raspi_gpio-0.1.8/LICENSE
--rw-r--r--   0        0        0      270 2023-07-19 12:53:45.951187 raspi_gpio-0.1.8/README.md
--rw-r--r--   0        0        0      741 2023-07-19 12:54:08.591309 raspi_gpio-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/GPIO_mock.py
--rw-r--r--   0        0        0      311 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      715 2023-07-19 12:53:45.955186 raspi_gpio-0.1.8/raspi_gpio/spidev_mock.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 18:30:06.338192 raspi_gpio-0.1.9/LICENSE
+-rw-r--r--   0        0        0      270 2023-07-20 18:30:06.338192 raspi_gpio-0.1.9/README.md
+-rw-r--r--   0        0        0      743 2023-07-20 18:30:31.338549 raspi_gpio-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-07-20 18:30:06.338192 raspi_gpio-0.1.9/raspi_gpio/GPIO_mock.py
+-rw-r--r--   0        0        0      311 2023-07-20 18:30:06.338192 raspi_gpio-0.1.9/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-20 18:30:06.338192 raspi_gpio-0.1.9/raspi_gpio/spidev_mock.py
+-rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 raspi_gpio-0.1.9/PKG-INFO
```

### Comparing `raspi_gpio-0.1.8/LICENSE` & `raspi_gpio-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.8/pyproject.toml` & `raspi_gpio-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.8"
+version = "0.1.9"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
-documentation = "https://github.com/MarkParker5/raspi-gpio/blob/main/README.md"
+documentation = "https://github.com/MarkParker5/raspi-gpio/blob/master/README.md"
 keywords = ["raspberry-pi", "gpio", "rpi", "rpi-gpio", "RPi.GPIO"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rpi-gpio = {version = "^0.7.1", platform = "linux"}
 spidev = {version = "^3.6", platform = "linux"}
```

### Comparing `raspi_gpio-0.1.8/raspi_gpio/GPIO_mock.py` & `raspi_gpio-0.1.9/raspi_gpio/GPIO_mock.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.8/raspi_gpio/spidev_mock.py` & `raspi_gpio-0.1.9/raspi_gpio/spidev_mock.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.8/PKG-INFO` & `raspi_gpio-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.8
+Version: 0.1.9
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rpi-gpio (>=0.7.1,<0.8.0) ; sys_platform == "linux"
 Requires-Dist: spidev (>=3.6,<4.0) ; sys_platform == "linux"
-Project-URL: Documentation, https://github.com/MarkParker5/raspi-gpio/blob/main/README.md
+Project-URL: Documentation, https://github.com/MarkParker5/raspi-gpio/blob/master/README.md
 Project-URL: Repository, https://github.com/MarkParker5/raspi-gpio
 Description-Content-Type: text/markdown
 
 # raspi-gpio
 RPi.GPIO and spidev wrapper with mocks for developmennt on any platform
 
 # Installation
```

