# Comparing `tmp/logium-1.1.tar.gz` & `tmp/logium-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-1.1.tar", last modified: Thu Jul 20 12:57:23 2023, max compression
+gzip compressed data, was "logium-1.2.tar", last modified: Thu Jul 20 13:40:54 2023, max compression
```

## Comparing `logium-1.1.tar` & `logium-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.525413 logium-1.1/
--rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.527415 logium-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.503408 logium-1.1/logium/
--rw-rw-rw-   0        0        0     3653 2023-07-20 12:38:27.000000 logium-1.1/logium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:57:23.523407 logium-1.1/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 12:57:23.000000 logium-1.1/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 12:57:23.531407 logium-1.1/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-20 12:55:28.000000 logium-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:40:54.806384 logium-1.2/
+-rw-rw-rw-   0        0        0      157 2023-07-20 13:40:54.807385 logium-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 13:40:54.775176 logium-1.2/logium/
+-rw-rw-rw-   0        0        0     4254 2023-07-20 13:27:10.000000 logium-1.2/logium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:40:54.805390 logium-1.2/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-20 13:40:54.000000 logium-1.2/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-20 13:40:54.000000 logium-1.2/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:40:54.000000 logium-1.2/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 13:40:54.000000 logium-1.2/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 13:40:54.809394 logium-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-20 13:40:15.000000 logium-1.2/setup.py
```

### Comparing `logium-1.1/logium/__init__.py` & `logium-1.2/logium/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,79 @@
 """
 A simple logging library for recording and displaying log messages.
 Author: N0rmalUser
-Version: 1.1
+Version: 1.2
 
 A guide is in my GitHub repository: https://github.com/N0rmalUser/normallogger
         or logium.GitHub
 """
 from datetime import datetime
 import webbrowser
 
 
-def _printer(self):
+def GitHub():
     """
-    The inner function for printing the message to the console and/or file
+    Opens the GitHub repository in the browser
     """
-    if self.console_enabled:
-        print(f'{self.datetime} {self.message}' if self.console_enabled and self.date_in_console else self.message)
-    if self.file_enable:
-        file_output = f'{self.datetime} {self.message}' if self.file_enable and self.date_in_file else self.message
-        with open(self.logfile[0], "a", encoding='utf-8') as f:
-            f.write(f'{file_output}\n')
+    webbrowser.open('https://github.com/N0rmalUser/normallogger')
 
 
 def _tagger(func):
     """
     The inner decorator function tagger takes a function and adds a tag to the message.
     """
 
     def wrapper(self, *args):
+        if not all(isinstance(arg, str) for arg in args):
+            raise TypeError("Arguments to decorated functions must be of str type.")
+
         message = ' '.join(str(arg) + (':' if i != len(args) - 1 else '') for i, arg in enumerate(args))
+
+        if not message:
+            raise ValueError("Message is empty or None.")
+
         self.message = message
         return func(self)
 
     return wrapper
 
 
+def _printer(self):
+    """
+    The inner function for printing the message to the console and/or file
+    """
+    if self.console_enabled:
+        print(f'{self.datetime} {self.message}' if self.date_in_console else self.message)
+
+    if self.file_enable:
+        if not isinstance(self.logfile, list) or not all(isinstance(file, str) for file in self.logfile):
+            raise ValueError("logfile must be a list of strings if file_enable is True.")
+
+        file_output = f'{self.datetime} {self.message}' if self.date_in_file else self.message
+        with open(self.logfile[0], "a", encoding='utf-8') as f:
+            f.write(f'{file_output}\n')
+
+
 class logger:
     """
     Class for logging and recording logs
     """
 
-    def __init__(self, logfile, console_enabled=True, datetime_format='%d.%m.%Y %H:%M:%S',
+    def __init__(self, logfile=None, console_enabled=True, datetime_format='%d.%m.%Y %H:%M:%S',
                  date_in_console=True, file_enable=True, date_in_file=True, wrap='[level]'):
         """
         Initializes an instance of the logger class.
         """
         if not all(isinstance(var, bool) for var in (console_enabled, date_in_console, file_enable, date_in_file)):
             raise ValueError("console_enabled, date_in_console, date_in_file, and file_enabled must be of bool type")
         if not all(isinstance(var, str) for var in (datetime_format, wrap)):
             raise ValueError("datetime_format, wrap must be of str type")
-        if not isinstance(datetime_format, str):
-            raise ValueError("datetime_format must be of str type")
-        self.logfile = logfile
+        if logfile is not None and not isinstance(logfile, str):
+            raise ValueError("logfile must be of str type or None")
+        self.logfile = [logfile] if file_enable and logfile else []
         self.datetime = datetime.now().strftime(datetime_format)
         self.console_enabled = console_enabled
         self.file_enable = file_enable
         self.date_in_console = date_in_console
         self.date_in_file = date_in_file
         self.wrap = wrap
         self.message = ''
```

