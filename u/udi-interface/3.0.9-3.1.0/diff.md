# Comparing `tmp/udi_interface-3.0.9.tar.gz` & `tmp/udi_interface-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udi_interface-3.0.9.tar", last modified: Sat Aug  7 16:49:34 2021, max compression
+gzip compressed data, was "udi_interface-3.1.0.tar", last modified: Thu Jul 20 19:51:08 2023, max compression
```

## Comparing `udi_interface-3.0.9.tar` & `udi_interface-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-08-07 16:49:34.000000 udi_interface-3.0.9/PKG-INFO
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     1741 2021-01-05 00:52:20.000000 udi_interface-3.0.9/README.md
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      224 2021-08-07 16:49:34.000000 udi_interface-3.0.9/setup.cfg
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     1415 2021-07-07 22:57:13.000000 udi_interface-3.0.9/setup.py
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/udi_interface/
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)      543 2021-08-07 16:48:51.000000 udi_interface-3.0.9/udi_interface/__init__.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     4594 2021-07-26 20:10:10.000000 udi_interface-3.0.9/udi_interface/custom.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)    38294 2021-08-07 16:42:53.000000 udi_interface-3.0.9/udi_interface/interface.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2337 2021-02-03 14:43:06.000000 udi_interface-3.0.9/udi_interface/isy.py
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     5169 2021-07-29 16:04:23.000000 udi_interface-3.0.9/udi_interface/node.py
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     2803 2021-01-05 00:52:20.000000 udi_interface-3.0.9/udi_interface/polylogger.py
--rwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)     4004 2021-01-27 13:58:04.000000 udi_interface-3.0.9/udi_interface/udi_interface.py
-drwxr-xr-x   0 bpaauwe   (1001) bpaauwe   (1001)        0 2021-08-07 16:49:34.000000 udi_interface-3.0.9/udi_interface.egg-info/
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)     2801 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/PKG-INFO
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)      427 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/SOURCES.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/dependency_links.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)        1 2021-01-28 15:38:14.000000 udi_interface-3.0.9/udi_interface.egg-info/not-zip-safe
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       50 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/requires.txt
--rw-r--r--   0 bpaauwe   (1001) bpaauwe   (1001)       14 2021-08-07 16:49:33.000000 udi_interface-3.0.9/udi_interface.egg-info/top_level.txt
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2023-07-20 19:51:08.822211 udi_interface-3.1.0/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1068 2023-07-05 13:05:47.000000 udi_interface-3.1.0/LICENSE
+-rw-r--r--   0 admin     (1001) admin     (1001)     2418 2023-07-20 19:51:08.822348 udi_interface-3.1.0/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1769 2023-07-05 13:05:47.000000 udi_interface-3.1.0/README.md
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      224 2023-07-20 19:51:08.822848 udi_interface-3.1.0/setup.cfg
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1456 2023-07-05 20:48:22.000000 udi_interface-3.1.0/setup.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2023-07-20 19:51:08.820877 udi_interface-3.1.0/udi_interface/
+-rwxrw-r--   0 admin     (1001) admin     (1001)      560 2023-07-19 16:45:39.000000 udi_interface-3.1.0/udi_interface/__init__.py
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     4913 2023-07-05 13:05:47.000000 udi_interface-3.1.0/udi_interface/custom.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)    60676 2023-07-20 19:22:49.000000 udi_interface-3.1.0/udi_interface/interface.py
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     2337 2023-07-05 13:05:47.000000 udi_interface-3.1.0/udi_interface/isy.py
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     6939 2023-07-19 17:40:58.000000 udi_interface-3.1.0/udi_interface/node.py
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     3276 2023-07-05 13:05:47.000000 udi_interface-3.1.0/udi_interface/polylogger.py
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     4004 2023-07-05 13:05:47.000000 udi_interface-3.1.0/udi_interface/udi_interface.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2023-07-20 19:51:08.822059 udi_interface-3.1.0/udi_interface.egg-info/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     2418 2023-07-20 19:51:08.000000 udi_interface-3.1.0/udi_interface.egg-info/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      435 2023-07-20 19:51:08.000000 udi_interface-3.1.0/udi_interface.egg-info/SOURCES.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-20 19:51:08.000000 udi_interface-3.1.0/udi_interface.egg-info/dependency_links.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-05 20:51:23.000000 udi_interface-3.1.0/udi_interface.egg-info/not-zip-safe
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       78 2023-07-20 19:51:08.000000 udi_interface-3.1.0/udi_interface.egg-info/requires.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       14 2023-07-20 19:51:08.000000 udi_interface-3.1.0/udi_interface.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `udi_interface-3.0.9/PKG-INFO` & `udi_interface-3.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 Metadata-Version: 2.1
 Name: udi_interface
-Version: 3.0.9
+Version: 3.1.0
 Summary: UDI Python Interface for Polyglot version 3
-Home-page: https://github.com/UniversalDevicesInc/udi-python-interface
+Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
-Description: ![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg)
-        
-        # UDI Python Interface Module for Polyglot version 3
-        
-        This is the PG3 interface API module that is portable to be imported into your Python 3.4+ based NodeServers.
-        
-        ### Installation
-        
-        Pip > 9 should be installed. This typically isn't the case, so you will have to upgrade Pip first.
-        
-        ```
-        # Check your pip version
-        pip -V
-        pip 9.0.1 from /home/e42/.local/lib/python2.7/site-packages (python 2.7)
-        pip3 -V
-        pip 9.0.1 from /usr/lib/python3/dist-packages (python 3.5)
-        
-        # If Pip is < Version 9
-        sudo pip install -U pip
-        ```
-        
-        The module is updated in Pypi (Python's package interface Pip) on a regular basis. So simply install the module like you would any Python module:
-        
-        ```
-        # Install the UDI interface
-        pip install udi_interface --user
-        ```
-        
-        ### Starting your NodeServer build
-        
-        When you start building a NodeServer you are helping build the free and open Internet of Things. Thank you! If you run in to any issues please ask your questions on the [UDI Polyglot Forums](http://forum.universal-devices.com/forum/111-polyglot/).
-        
-        To get started, [use the python template.](https://github.com/UniversalDevicesInc/udi-poly-template-python)
-        
-        From there just read the code itself, it is fully explained step by step.
-        
-        ### How to Enable your NodeServer in the Cloud
-        
-        [Link to PGC Interface](https://github.com/UniversalDevicesInc/pgc-python-interface/blob/master/README.md)
-        
-        ### Controlling logging
-        
-        By default when the Polyglot Python Interface is started up the logging is in WARNING mode. If you want to change the level set logLevel: <level> in your server.json file.  Valid levels are:
-        
-        CRITICAL
-        ERROR
-        WARNING
-        INFO
-        DEBUG
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.6.*
+Requires-Python: >3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg "Test and Publish")
+
+# UDI Python Interface Module for Polyglot version 3
+
+This is the PG3 interface API module that is portable to be imported into your Python 3.4+ based NodeServers.
+
+### Installation
+
+Pip > 9 should be installed. This typically isn't the case, so you will have to upgrade Pip first.
+
+```
+# Check your pip version
+pip -V
+pip 9.0.1 from /home/e42/.local/lib/python2.7/site-packages (python 2.7)
+pip3 -V
+pip 9.0.1 from /usr/lib/python3/dist-packages (python 3.5)
+
+# If Pip is < Version 9
+sudo pip install -U pip
+```
+
+The module is updated in Pypi (Python's package interface Pip) on a regular basis. So simply install the module like you would any Python module:
+
+```
+# Install the UDI interface
+pip install udi_interface --user
+```
+
+### Starting your NodeServer build
+
+When you start building a NodeServer you are helping build the free and open Internet of Things. Thank you! If you run in to any issues please ask your questions on the [UDI Polyglot Forums](http://forum.universal-devices.com/forum/111-polyglot/).
+
+To get started, [use the python template.](https://github.com/UniversalDevicesInc/udi-poly-template-python)
+
+From there just read the code itself, it is fully explained step by step.
+
+### How to Enable your NodeServer in the Cloud
+
+[Link to PGC Interface](https://github.com/UniversalDevicesInc/pgc-python-interface/blob/master/README.md)
+
+### Controlling logging
+
+By default when the Polyglot Python Interface is started up the logging is in WARNING mode. If you want to change the level set logLevel: <level> in your server.json file.  Valid levels are:
+
+`CRITICAL` `ERROR` `WARNING` `INFO` `DEBUG`
```

### Comparing `udi_interface-3.0.9/README.md` & `udi_interface-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg)
+![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg "Test and Publish")
 
 # UDI Python Interface Module for Polyglot version 3
 
 This is the PG3 interface API module that is portable to be imported into your Python 3.4+ based NodeServers.
 
 ### Installation
 
@@ -38,13 +38,8 @@
 
 [Link to PGC Interface](https://github.com/UniversalDevicesInc/pgc-python-interface/blob/master/README.md)
 
 ### Controlling logging
 
 By default when the Polyglot Python Interface is started up the logging is in WARNING mode. If you want to change the level set logLevel: <level> in your server.json file.  Valid levels are:
 
-CRITICAL
-ERROR
-WARNING
-INFO
-DEBUG
-
+`CRITICAL` `ERROR` `WARNING` `INFO` `DEBUG`
```

### Comparing `udi_interface-3.0.9/setup.py` & `udi_interface-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     license=metadata['license'],
     packages=find_packages(),
     install_requires=[
         "paho-mqtt",
         "python-dotenv",
         "markdown2",
         "netifaces",
-        "pyisy"
+        "requests",
+        "pyisy >2.0, != 2.1.5, <3.0.0"
     ],
-    python_requires='>3.6.*',
+    python_requires='>3.6',
     zip_safe=False,
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How Mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
```

### Comparing `udi_interface-3.0.9/udi_interface/__init__.py` & `udi_interface-3.1.0/udi_interface/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-
-
-from .polylogger import LOG_HANDLER, LOGGER
-from .udi_interface import unload_interface, get_network_interface
-from .node import Node
-from .interface import Interface
-from .custom import Custom
-from .isy import ISY
-
-__version__ = '3.0.9'
-__description__ = 'UDI Python Interface for Polyglot version 3'
-__url__ = 'https://github.com/UniversalDevicesInc/udi-python-interface'
-__author__ = 'Universal Devices Inc.'
-__authoremail__ = 'bpaauwe@yahoo.com'
-__license__ = 'MIT'
-
-LOGGER.info('{} {} Starting...'.format(__description__, __version__))
+
+
+from .polylogger import LOG_HANDLER, LOGGER
+from .udi_interface import unload_interface, get_network_interface
+from .node import Node
+from .interface import Interface
+from .custom import Custom
+from .isy import ISY
+
+__version__ = '3.1.0'
+__description__ = 'UDI Python Interface for Polyglot version 3'
+__url__ = 'https://github.com/UniversalDevicesInc/udi_python_interface'
+__author__ = 'Universal Devices Inc.'
+__authoremail__ = 'bpaauwe@yahoo.com'
+__license__ = 'MIT'
+
+LOGGER.info('{} {} Starting...'.format(__description__, __version__))
```

### Comparing `udi_interface-3.0.9/udi_interface/custom.py` & `udi_interface-3.1.0/udi_interface/custom.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         #self.poly._saveCustom(self.__dict__['custom'])
 
         CLOGGER.info('Sending data {} to Polyglot.'.format(key))
         message = {'set': [{'key': key, 'value': self.__dict__['_rawdata']}]}
         self.poly.send(message, 'custom')
 
     def load(self, new_data, save=False):
+
+        if new_data is None:
+            self.__dict__['_rawdata'] = {}
+            return
+
         """
         FIXME: this is used to update the internal data
         structure from Polyglot's database.  Should this
         be overwriting or updating the internal structure?
         """
         CLOGGER.debug('CUSTOM: load {}'.format(new_data))
 
@@ -109,14 +114,23 @@
             return self.__dict__['_rawdata'][key]
         else:
             return None
 
     def __len__(self):
         return len(self.__dict__['_rawdata'])
 
+    def __contains__(self, item):
+        return item in self.__dict__['_rawdata']
+
+    def __repr__(self):
+        return repr(self.__dict__['_rawdata'])
+
+    def __str__(self):
+        return str(self.__dict__['_rawdata'])
+
     def delete(self, key):
         if key in self._rawdata:
             self._rawdata.pop(key)
             CLOGGER.debug('CUSTOM: delete {} ...saving'.format(key))
             self._save()
 
     def clear(self):
```

### Comparing `udi_interface-3.0.9/udi_interface/isy.py` & `udi_interface-3.1.0/udi_interface/isy.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.9/udi_interface/polylogger.py` & `udi_interface-3.1.0/udi_interface/polylogger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,72 @@
 
 import os
+import gzip
 import logging
 from logging import handlers as log_handlers
 import warnings
+import shutil
+
 
 class PolyLogger:
 
     NAME = __name__.split(".")[0]
     LOGS_DIR= './logs'
     LOG_FILE = 'debug.log'
     LEVEL = logging.DEBUG
     ROTATION = 'midnight'
     WARN_LOGGER_NAME = 'py.warnings'
-    BACKUP_COUNT = 30
+    BACKUP_COUNT = 14
     FMT_STRING = '%(asctime)s %(threadName)-10s %(name)-18s %(levelname)-8s %(module)s:%(funcName)s: %(message)s'
     IS_ROOT = True
 
     def __init__(self):
         if not os.path.exists(PolyLogger.LOGS_DIR):
             os.makedirs(PolyLogger.LOGS_DIR)
         self.handler = log_handlers.TimedRotatingFileHandler(
             os.path.join(PolyLogger.LOGS_DIR, PolyLogger.LOG_FILE),
             when=PolyLogger.ROTATION,
+            interval=1,
             backupCount=PolyLogger.BACKUP_COUNT
         )
+        self.handler.rotator = self.rotator
+        self.handler.namer = self.namer
+
         logging.captureWarnings(True)
         self.set_log_format(PolyLogger.FMT_STRING)
         # Get our logger for everyone to use.
         self.logger = logging.getLogger(PolyLogger.NAME)
         # Set the root logger name to our name
         self.logger.propagate = False # Duplicates when basicConfig is used
         self.logger.addHandler(self.handler)
         self.logger.setLevel(PolyLogger.LEVEL)
         # By default we only show warnings for others.
         self.set_basic_config(True,logging.WARNING)
         self.warnlog = logging.getLogger(PolyLogger.WARN_LOGGER_NAME)
         warnings.formatwarning = self.warning_on_one_line
         self.warnlog.addHandler(self.handler)
 
+    def namer(self, name):
+        return name + ".gz"
+
+    def rotator(self, source, dest):
+        with open(source, 'rb') as f_in:
+            with gzip.open(dest, "wb") as f_out:
+                shutil.copyfileobj(f_in, f_out)
+        os.remove(source)
+
     def set_log_format(self, fmt_string):
         # Format each log message like this
         formatter = logging.Formatter(fmt_string)
         # Attach the formatter to the handler
         self.handler.setFormatter(formatter)
 
+    def getLevelName(self, level):
+        return logging.getLevelName(level)
+
     def set_basic_config(self, enable=True, level=None):
         self.logger.info('set_basic_config: enable={} level={}'.format(enable,level))
         if level is None:
             level = self.logger.getEffectiveLevel()
             self.logger.info('set_basic_config: level={}'.format(level))
         # Remove all handlers associated with the root logger object.
         # Once everyone is on Python 3.8 we could use basicConfig force
```

### Comparing `udi_interface-3.0.9/udi_interface/udi_interface.py` & `udi_interface-3.1.0/udi_interface/udi_interface.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.0.9/udi_interface.egg-info/PKG-INFO` & `udi_interface-3.1.0/udi_interface.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 Metadata-Version: 2.1
 Name: udi-interface
-Version: 3.0.9
+Version: 3.1.0
 Summary: UDI Python Interface for Polyglot version 3
-Home-page: https://github.com/UniversalDevicesInc/udi-python-interface
+Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
-Description: ![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg)
-        
-        # UDI Python Interface Module for Polyglot version 3
-        
-        This is the PG3 interface API module that is portable to be imported into your Python 3.4+ based NodeServers.
-        
-        ### Installation
-        
-        Pip > 9 should be installed. This typically isn't the case, so you will have to upgrade Pip first.
-        
-        ```
-        # Check your pip version
-        pip -V
-        pip 9.0.1 from /home/e42/.local/lib/python2.7/site-packages (python 2.7)
-        pip3 -V
-        pip 9.0.1 from /usr/lib/python3/dist-packages (python 3.5)
-        
-        # If Pip is < Version 9
-        sudo pip install -U pip
-        ```
-        
-        The module is updated in Pypi (Python's package interface Pip) on a regular basis. So simply install the module like you would any Python module:
-        
-        ```
-        # Install the UDI interface
-        pip install udi_interface --user
-        ```
-        
-        ### Starting your NodeServer build
-        
-        When you start building a NodeServer you are helping build the free and open Internet of Things. Thank you! If you run in to any issues please ask your questions on the [UDI Polyglot Forums](http://forum.universal-devices.com/forum/111-polyglot/).
-        
-        To get started, [use the python template.](https://github.com/UniversalDevicesInc/udi-poly-template-python)
-        
-        From there just read the code itself, it is fully explained step by step.
-        
-        ### How to Enable your NodeServer in the Cloud
-        
-        [Link to PGC Interface](https://github.com/UniversalDevicesInc/pgc-python-interface/blob/master/README.md)
-        
-        ### Controlling logging
-        
-        By default when the Polyglot Python Interface is started up the logging is in WARNING mode. If you want to change the level set logLevel: <level> in your server.json file.  Valid levels are:
-        
-        CRITICAL
-        ERROR
-        WARNING
-        INFO
-        DEBUG
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.6.*
+Requires-Python: >3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Test And Publish](https://github.com/UniversalDevicesInc/udi-python-interface/workflows/Publish%20PyPI%20and%20TestPyPI/badge.svg "Test and Publish")
+
+# UDI Python Interface Module for Polyglot version 3
+
+This is the PG3 interface API module that is portable to be imported into your Python 3.4+ based NodeServers.
+
+### Installation
+
+Pip > 9 should be installed. This typically isn't the case, so you will have to upgrade Pip first.
+
+```
+# Check your pip version
+pip -V
+pip 9.0.1 from /home/e42/.local/lib/python2.7/site-packages (python 2.7)
+pip3 -V
+pip 9.0.1 from /usr/lib/python3/dist-packages (python 3.5)
+
+# If Pip is < Version 9
+sudo pip install -U pip
+```
+
+The module is updated in Pypi (Python's package interface Pip) on a regular basis. So simply install the module like you would any Python module:
+
+```
+# Install the UDI interface
+pip install udi_interface --user
+```
+
+### Starting your NodeServer build
+
+When you start building a NodeServer you are helping build the free and open Internet of Things. Thank you! If you run in to any issues please ask your questions on the [UDI Polyglot Forums](http://forum.universal-devices.com/forum/111-polyglot/).
+
+To get started, [use the python template.](https://github.com/UniversalDevicesInc/udi-poly-template-python)
+
+From there just read the code itself, it is fully explained step by step.
+
+### How to Enable your NodeServer in the Cloud
+
+[Link to PGC Interface](https://github.com/UniversalDevicesInc/pgc-python-interface/blob/master/README.md)
+
+### Controlling logging
+
+By default when the Polyglot Python Interface is started up the logging is in WARNING mode. If you want to change the level set logLevel: <level> in your server.json file.  Valid levels are:
+
+`CRITICAL` `ERROR` `WARNING` `INFO` `DEBUG`
```

