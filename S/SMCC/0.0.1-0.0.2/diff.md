# Comparing `tmp/smcc-0.0.1.tar.gz` & `tmp/smcc-0.0.2.tar.gz`

## Comparing `smcc-0.0.1.tar` & `smcc-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     9575 2020-02-02 00:00:00.000000 smcc-0.0.1/REFERENCE.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 smcc-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/Pipfile
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/README.md
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/jupyter_example.ipynb
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/python_example.py
--rw-r--r--   0        0        0    45589 2020-02-02 00:00:00.000000 smcc-0.0.1/Examples/images/example_serial_port.gif
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 smcc-0.0.1/github_images/icon.png
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 smcc-0.0.1/src/SMCC/Commands.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 smcc-0.0.1/src/SMCC/Constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smcc-0.0.1/src/SMCC/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 smcc-0.0.1/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 smcc-0.0.1/COPYING.LESSER
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smcc-0.0.1/LICENSE
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 smcc-0.0.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 smcc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 smcc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 smcc-0.0.2/REFERENCE.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 smcc-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/Pipfile
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/README.md
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/jupyter_example.ipynb
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/python_example.py
+-rw-r--r--   0        0        0    45589 2020-02-02 00:00:00.000000 smcc-0.0.2/Examples/images/example_serial_port.gif
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 smcc-0.0.2/github_images/icon.png
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 smcc-0.0.2/src/SMCC/Commands.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 smcc-0.0.2/src/SMCC/Constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smcc-0.0.2/src/SMCC/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 smcc-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 smcc-0.0.2/COPYING.LESSER
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smcc-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 smcc-0.0.2/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 smcc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 smcc-0.0.2/PKG-INFO
```

### Comparing `smcc-0.0.1/REFERENCE.md` & `smcc-0.0.2/REFERENCE.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </p>
 
 - [API Reference](#api-reference)
   - [Functions](#functions)
     - [1. `filBool(value, start=0)`](#1-filboolvalue-start0)
     - [2. `SETUP_CMD(control_dict)`](#2-setup_cmdcontrol_dict)
     - [3. `STEP_CMD(control_dict)`](#3-step_cmdcontrol_dict)
-    - [4. `sendCommand(coms, cmd)`](#4-sendcommandcoms-cmd)
+    - [4. `sendCommand(coms, cmd, check=True)`](#4-sendcommandcoms-cmd-checktrue)
     - [5. `convert2Binary(number, size)`](#5-convert2binarynumber-size)
     - [6. `getFrequency(control_dict)`](#6-getfrequencycontrol_dict)
     - [7. `generateControlDict()`](#7-generatecontroldict)
     - [8. `checkConnection(ctrl_dict)`](#8-checkconnectionctrl_dict)
   - [Templates](#templates)
     - [1. `SETUP_BLANK`:](#1-setup_blank)
     - [2. `STEP_BLANK`:](#2-step_blank)
@@ -69,21 +69,22 @@
 Returns a STEP Command with the `control_dict` configurations. Mainly the direction and step counter information.
 
 **Parameters:**
 - `control_dict`: Dictionary that groups all the controlable elements of the SMC-Driver.
 
 **Returns:** A dictionary with the step command with the information of ctrl_dict and the number of bytes expected for the controller response. The dictionary is based on the `STEP_BLANK` with the `control_dict` information written on top.
 
-### 4. `sendCommand(coms, cmd)`
+### 4. `sendCommand(coms, cmd, check=True)`
 
 Sends the desired command `cmd` via the `coms` serial port.
 
 **Parameters:**
 - `coms`: A PySerial serial port connection. Typically corresponds to `ctrl_dict['comms']`.
 - `cmd`: The desired command to send. Values can be: `SETUP_CMD`, `STEP_CMD`, `INFO_CMD` and `HALT_CMD`.
+- `check`: Indicates if symmetry on the response must be enforced. By default (True) the function checks if response must match the sent command. 
 
 **Returns:** The bytes associated with the controller response. 
 
 ### 5. `convert2Binary(number, size)`
 
 Converts the integer stored on `number` to a binary number of `size` bits. 
 
@@ -203,16 +204,14 @@
 
 Indicates the structure of the INFO Command. The controller responds this command with the SETUP information (control information, frequency, frequency counter) and the current STEP information (number of steps and direction)
 
 ```python
 INFO_CMD = {
     'cmd': [
             bitarray('01000000'), # Command packet
-            bitarray('00000000'), # Filler packets
-            bitarray('00000000')
             ],
     'response_size': 6, # 3 bytes for : setup + freq_counter
                         # 3 bytes for : step + step_counter
 }
 ```
 
 The response size corresponds to 6 bytes: 
@@ -234,16 +233,14 @@
 
 Indicates the structure of the HALT Command. When sent the controller stops all motor operations.
 
 ```python
 HALT_CMD = {
     'cmd': [
             bitarray('11000000'), # Command packet
-            bitarray('00000000'), # Filler packets
-            bitarray('00000000')
             ],
     'response_size': 1,
 }
 ```
 
 **Example use:**
```

### Comparing `smcc-0.0.1/.github/workflows/python-publish.yml` & `smcc-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/Examples/Pipfile.lock` & `smcc-0.0.2/Examples/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/Examples/jupyter_example.ipynb` & `smcc-0.0.2/Examples/jupyter_example.ipynb`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/Examples/python_example.py` & `smcc-0.0.2/Examples/python_example.py`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/Examples/images/example_serial_port.gif` & `smcc-0.0.2/Examples/images/example_serial_port.gif`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/github_images/icon.png` & `smcc-0.0.2/github_images/icon.png`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/src/SMCC/Commands.py` & `smcc-0.0.2/src/SMCC/Commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import copy
 from bitarray import bitarray
 from bitarray.util import int2ba, zeros
 from .Constants import ARDUINO_CONSTANTS, DEFAULTS, SOFTWARE_LIMITS
 
 # Commands template
 
-SETUP_BLANK = { #Works as a template for SETUP and STEP CMD
+SETUP_BLANK = { #Works as a template for SETUP CMD
     'cmd': [
             bitarray('10000000'), 
             bitarray('00000000'), 
             bitarray('00000000')
             ],
     'response_size': 3, # 3 bytes
 }
 
-STEP_BLANK = { #Works as a template for SETUP and STEP CMD
+STEP_BLANK = { #Works as a template for STEP CMD
     'cmd': [
             bitarray('00000000'), 
             bitarray('00000000'), 
             bitarray('00000000')
             ],
     'response_size': 3, # 3 bytes
 }
 
 INFO_CMD = {
     'cmd': [
             bitarray('01000000'), # Command packet
-            bitarray('00000000'), # Filler packets
-            bitarray('00000000')
             ],
     'response_size': 6, # 3 bytes for : setup + freq_counter
                         # 3 bytes for : step + step_counter
 }
 
 HALT_CMD = {
     'cmd': [
             bitarray('11000000'), # Command packet
-            bitarray('00000000'), # Filler packets
-            bitarray('00000000')
             ],
-    'response_size': 1, # 3 bytes for : setup + freq_counter
-                        # 3 bytes for : step + step_counter
+    'response_size': 1, 
 }
 
 
 # Allows to place a boolean flag in a 8bit array
 def fillBool(values, start=0):
     padded = bitarray('0000 0000')
     n_bits = len(values)
@@ -101,31 +96,32 @@
 
     step_cmd['cmd'] = cmd
 
     return step_cmd
 
 
 # Sends a command through coms
-def sendCommand(coms, cmd):
+def sendCommand(coms, cmd, check=True):
     k_cmd, k_r_size = cmd
     # Write command
     for byte_arr in cmd[k_cmd]:
         coms.write(byte_arr)
 
     # Wait for automatic reply
     response = coms.read(cmd[k_r_size])
     # Convert the response to bitarrays    
     n_response = []
 
     for i in response:
         n_response.append(convert2Binary(i, 8))
 
     # Check if response matches cmd sent
-    if(cmd['cmd'] != n_response):
-        raise Exception('Response received from controller does not matches sent command.')
+    if(check):
+        if(cmd['cmd'] != n_response):
+            raise Exception('Response received from controller does not matches sent command.')
 
     return n_response
 
 
 # Convert an integer number to binary according to <size>
 def convert2Binary(number, size):
     number_bin = int2ba(number)
```

### Comparing `smcc-0.0.1/src/SMCC/Constants.py` & `smcc-0.0.2/src/SMCC/Constants.py`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/COPYING.LESSER` & `smcc-0.0.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/LICENSE` & `smcc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smcc-0.0.1/README.md` & `smcc-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 To install the `SMCC` just use pip as follows: 
 
 ```bash
 $ pip install smcc
 
 ```
 
-The project is hosted on the pypi register: https://pypi.org/projects/smcc
+The project is hosted on the pypi register: https://pypi.org/projects/SMCC
 
 
 ## Example use
 
 ### Quick Start
 
 Configure a 3.75°/step stepper motor to perform a full clockwise rotation at 20 rpm:
```

### Comparing `smcc-0.0.1/pyproject.toml` & `smcc-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SMCC"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mauricio Aravena Cifuentes", email="maurio.aravena@sansano.usm.cl" },
 ]
 description = "SMC_core (SMCC) allows for direct communication and control of the Serial-Motor-Controller project via Python-code."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `smcc-0.0.1/PKG-INFO` & `smcc-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMCC
-Version: 0.0.1
+Version: 0.0.2
 Summary: SMC_core (SMCC) allows for direct communication and control of the Serial-Motor-Controller project via Python-code.
 Project-URL: Homepage, https://github.com/Wauro21/SMCC
 Project-URL: Bug Tracker, https://github.com/Wauro21/SMCC/issues
 Author-email: Mauricio Aravena Cifuentes <maurio.aravena@sansano.usm.cl>
 License-File: COPYING.LESSER
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -39,15 +39,15 @@
 To install the `SMCC` just use pip as follows: 
 
 ```bash
 $ pip install smcc
 
 ```
 
-The project is hosted on the pypi register: https://pypi.org/projects/smcc
+The project is hosted on the pypi register: https://pypi.org/projects/SMCC
 
 
 ## Example use
 
 ### Quick Start
 
 Configure a 3.75°/step stepper motor to perform a full clockwise rotation at 20 rpm:
```

