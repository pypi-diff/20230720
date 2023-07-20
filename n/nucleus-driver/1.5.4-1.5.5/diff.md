# Comparing `tmp/nucleus_driver-1.5.4.tar.gz` & `tmp/nucleus_driver-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.4.tar", last modified: Mon Jun 26 13:30:04 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.5.tar", last modified: Thu Jul 20 08:10:46 2023, max compression
```

## Comparing `nucleus_driver-1.5.4.tar` & `nucleus_driver-1.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-26 12:27:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17098 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39763 2023-06-26 13:25:07.000000 nucleus_driver-1.5.4/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.4/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-26 13:24:28.000000 nucleus_driver-1.5.4/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-26 13:30:04.463241 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-26 13:30:04.000000 nucleus_driver-1.5.4/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9494 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.698148 nucleus_driver-1.5.5/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-26 12:27:28.000000 nucleus_driver-1.5.5/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17098 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:48:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39942 2023-07-20 08:09:17.000000 nucleus_driver-1.5.5/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.5/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19446 2023-06-30 08:54:04.000000 nucleus_driver-1.5.5/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11213 2023-07-20 08:10:01.000000 nucleus_driver-1.5.5/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-20 08:10:46.702148 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9494 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-07-20 08:10:46.000000 nucleus_driver-1.5.5/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.4/LICENSE.txt` & `nucleus_driver-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/PKG-INFO` & `nucleus_driver-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.5.4
+Version: 1.5.5
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -274,7 +276,8 @@
 To run the console script, execute the command
 
 ```shell
 nucleus_driver
 ```
 
 ![Console script](docs/nucleus_driver_shell.png)
+
```

### Comparing `nucleus_driver-1.5.4/README.md` & `nucleus_driver-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/setup.cfg` & `nucleus_driver-1.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.4
+version = 1.5.5
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_connection.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,16 @@
             if len(binary_packet) == 0:
                 reading_packet = False
             else:
                 reading_packet = True
 
         elif 0xa5 in binary_packet[1:]:
             start_index = next(i + 1 for i, x in enumerate(binary_packet[1:]) if x == 0xa5)
-            ascii_packet.extend(binary_packet[:start_index])
+            # Check if gibberishb contains \r\n, thus determining that it is indeed an ascii packet
+            ascii_packet.extend(binary_packet[:start_index]) # skip this? pr write to condition
             binary_packet = binary_packet[start_index:]
             reading_packet = True
 
         else:
             self.write_condition(error_message='header checksum failed', packet=binary_packet)
             reading_packet = False
             binary_packet = bytearray()
@@ -662,14 +663,15 @@
 
         self.write_ascii(packet=ascii_packet)
 
     def add_data(self, data):
         for value in data:
             if value == 0xa5 and not self.reading_packet:
                 self.reading_packet = True
+                # write ascii to condition?
                 self.ascii_packet = list()
 
             if self.reading_packet:
                 self.binary_packet.append(value)
             else:
                 self.ascii_packet.append(value)
```

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.5/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/app.py` & `nucleus_driver-1.5.5/src/nucleus_driver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,18 @@
 
         command = command_args.command
 
         if not self.nucleus_driver.connection.get_connection_status():
             self.nucleus_driver.messages.write_message('Nucleus not connected')
             return
 
-        self.nucleus_driver.send_command(command)
+        reply = self.nucleus_driver.send_command(command)
+
+        for entry in reply:
+            self.nucleus_driver.messages.write_message(entry.decode(), skip_newline=True)
 
     flash_firmware_parser = Cmd2ArgumentParser(description='Flash firmware')
     flash_firmware_parser.add_argument('path', help='Set flash file. Extension must be in [.bin, .ldr, .zip]', completer=cmd2.Cmd.path_complete)
 
     @with_argparser(flash_firmware_parser)
     @with_category(CMD_CAT_FLASH)
     def do_flash_firmware(self, set_flash_path_args):
```

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.5/src/nucleus_driver/nucleus_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
         return self.connection.disconnect()
 
     ###########################################
     # Command
     ###########################################
 
-    def send_command(self, command: str):
+    def send_command(self, command: str) -> [bytes]:
+
+        reply = list()
 
         BLOCKED_COMMANDS = ['START', 'FIELDCAL', 'STARTSPECTRUM', 'STOP', 'UPLOAD', 'FWUPDATE', 'DVLUPDATE']
 
         command = command.rstrip('\n').rstrip('\r')
 
         if command.upper() in BLOCKED_COMMANDS:
             self.messages.write_message(f'{command} is not supported as a command in this application. Use the applications functionality instead')
@@ -86,19 +88,19 @@
 
             command_encoded = command.encode() + b'\r\n'
 
             self.commands._reset_buffer()
 
             self.connection.write(command_encoded)
 
-            message = self.commands._handle_reply(command=command_encoded, terminator=b'OK\r\n', timeout=1)
+            reply = self.commands._handle_reply(command=command_encoded, terminator=b'OK\r\n', timeout=1)
 
-            for entry in message:
-                self.messages.write_message(entry.decode(), skip_newline=True)
+        return reply
 
+            
     ###########################################
     # Logging
     ###########################################
 
     def set_log_path(self, path):
 
         self.logger.set_path(path=path)
```

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.5/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.5.4
+Version: 1.5.5
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -274,7 +276,8 @@
 To run the console script, execute the command
 
 ```shell
 nucleus_driver
 ```
 
 ![Console script](docs/nucleus_driver_shell.png)
+
```

### Comparing `nucleus_driver-1.5.4/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.5/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

