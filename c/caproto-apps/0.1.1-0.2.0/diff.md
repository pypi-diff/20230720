# Comparing `tmp/caproto-apps-0.1.1.tar.gz` & `tmp/caproto-apps-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caproto-apps-0.1.1.tar", last modified: Sun Jul  2 02:25:51 2023, max compression
+gzip compressed data, was "caproto-apps-0.2.0.tar", last modified: Thu Jul 20 19:22:42 2023, max compression
```

## Comparing `caproto-apps-0.1.1.tar` & `caproto-apps-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/
--rw-------   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3177 2023-07-02 02:19:09.000000 caproto-apps-0.1.1/README.md
--rw-------   0 b268176   (2319) xsdspc    (1117)     1043 2023-07-02 02:25:13.000000 caproto-apps-0.1.1/pyproject.toml
--rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/setup.cfg
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.212747 caproto-apps-0.1.1/src/
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.213747 caproto-apps-0.1.1/src/caproto_apps.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      345 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       62 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/top_level.txt
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.214747 caproto-apps-0.1.1/src/caprotoapps/
--rw-------   0 b268176   (2319) xsdspc    (1117)       64 2023-07-02 02:10:14.000000 caproto-apps-0.1.1/src/caprotoapps/__init__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20766 2023-06-28 04:14:07.000000 caproto-apps-0.1.1/src/caprotoapps/alive.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     8403 2023-07-02 02:24:39.000000 caproto-apps-0.1.1/src/caprotoapps/manager.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.214747 caproto-apps-0.1.1/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10768 2023-07-01 02:49:25.000000 caproto-apps-0.1.1/tests/test_alive.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4002 2023-07-01 23:53:32.000000 caproto-apps-0.1.1/tests/test_manager.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-07-20 19:22:42.504041 caproto-apps-0.2.0/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4237 2023-07-20 19:22:42.503040 caproto-apps-0.2.0/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3678 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/README.md
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1043 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/pyproject.toml
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2023-07-20 19:22:42.505026 caproto-apps-0.2.0/setup.cfg
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-07-20 19:22:42.467038 caproto-apps-0.2.0/src/
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-07-20 19:22:42.485022 caproto-apps-0.2.0/src/caproto_apps.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4237 2023-07-20 19:22:42.000000 caproto-apps-0.2.0/src/caproto_apps.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      375 2023-07-20 19:22:42.000000 caproto-apps-0.2.0/src/caproto_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-07-20 19:22:42.000000 caproto-apps-0.2.0/src/caproto_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       62 2023-07-20 19:22:42.000000 caproto-apps-0.2.0/src/caproto_apps.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-07-20 19:22:42.000000 caproto-apps-0.2.0/src/caproto_apps.egg-info/top_level.txt
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-07-20 19:22:42.494027 caproto-apps-0.2.0/src/caprotoapps/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       64 2023-07-02 02:10:14.000000 caproto-apps-0.2.0/src/caprotoapps/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20814 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/src/caprotoapps/alive.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      119 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/src/caprotoapps/exceptions.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10284 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/src/caprotoapps/manager.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-07-20 19:22:42.500039 caproto-apps-0.2.0/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10766 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/tests/test_alive.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     5735 2023-07-20 19:21:39.000000 caproto-apps-0.2.0/tests/test_manager.py
```

### Comparing `caproto-apps-0.1.1/PKG-INFO` & `caproto-apps-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: caproto-apps
-Version: 0.1.1
-Summary: Variety of useful extensions for caproto IOCs.
-Author-email: Mark Wolfman <wolfman@anl.gov>
-Project-URL: Homepage, https://github.com/canismarko/caproto-apps
-Keywords: caproto,controls
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Caproto Apps
 
 [![Tests](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml)
 
 Implementations of select EPICS-compatible records in caproto.
 
 
@@ -109,14 +93,29 @@
 class MyIOC(PVGroup):
     ioc_manager = SubGroup(ManagerGroup,
     		           script="myuser@myhost:/path/to/script.sh")
 ```
 
 **Note:** The *console* PV is currently not implemented.
 
+It is possible to **limit which IOCs can be started or stopped** via
+an IOC ManagerGroup using the *allow_start* and *allow_stop*
+parameters during initialization:
+
+```
+class MyIOC(PVGroup):
+    mission_critical_manager = SubGroup(ManagerGroup,
+					allow_start=True,
+					allow_stop=False)
+```
+
+The status PVs *startable* and *stoppable* are read-only indicators of
+whether the IOC can be controlled via this ManagerGroup. Re-starting
+an IOC requires both *allow_start* and *allow_stop* to be true.
+
 ## Development
 
 To install caproto-apps for development, first clone the github repository:
 
 ```
 git clone https://github.com/canismarko/caproto-apps.git
 ```
@@ -130,8 +129,8 @@
 ## Building the Project for PyPI
 
 ```
 (venv) $ python -m build
 (venv) $ twine check dist/*
 (venv) $ twine upload -r testpypi dist/*
 (venv) $ twine upload dist/*
-```
+```
```

### Comparing `caproto-apps-0.1.1/README.md` & `caproto-apps-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: caproto-apps
+Version: 0.2.0
+Summary: Variety of useful extensions for caproto IOCs.
+Author-email: Mark Wolfman <wolfman@anl.gov>
+Project-URL: Homepage, https://github.com/canismarko/caproto-apps
+Keywords: caproto,controls
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # Caproto Apps
 
 [![Tests](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml)
 
 Implementations of select EPICS-compatible records in caproto.
 
 
@@ -93,14 +109,29 @@
 class MyIOC(PVGroup):
     ioc_manager = SubGroup(ManagerGroup,
     		           script="myuser@myhost:/path/to/script.sh")
 ```
 
 **Note:** The *console* PV is currently not implemented.
 
+It is possible to **limit which IOCs can be started or stopped** via
+an IOC ManagerGroup using the *allow_start* and *allow_stop*
+parameters during initialization:
+
+```
+class MyIOC(PVGroup):
+    mission_critical_manager = SubGroup(ManagerGroup,
+					allow_start=True,
+					allow_stop=False)
+```
+
+The status PVs *startable* and *stoppable* are read-only indicators of
+whether the IOC can be controlled via this ManagerGroup. Re-starting
+an IOC requires both *allow_start* and *allow_stop* to be true.
+
 ## Development
 
 To install caproto-apps for development, first clone the github repository:
 
 ```
 git clone https://github.com/canismarko/caproto-apps.git
 ```
@@ -114,8 +145,8 @@
 ## Building the Project for PyPI
 
 ```
 (venv) $ python -m build
 (venv) $ twine check dist/*
 (venv) $ twine upload -r testpypi dist/*
 (venv) $ twine upload dist/*
-```
+```
```

### Comparing `caproto-apps-0.1.1/pyproject.toml` & `caproto-apps-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # [build-system]
 # requires = ["hatchling"]
 # build-backend = "hatchling.build"
 
 [project]
 name = "caproto-apps"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "Variety of useful extensions for caproto IOCs."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `caproto-apps-0.1.1/src/caproto_apps.egg-info/PKG-INFO` & `caproto-apps-0.2.0/src/caproto_apps.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caproto-apps
-Version: 0.1.1
+Version: 0.2.0
 Summary: Variety of useful extensions for caproto IOCs.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/canismarko/caproto-apps
 Keywords: caproto,controls
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -109,14 +109,29 @@
 class MyIOC(PVGroup):
     ioc_manager = SubGroup(ManagerGroup,
     		           script="myuser@myhost:/path/to/script.sh")
 ```
 
 **Note:** The *console* PV is currently not implemented.
 
+It is possible to **limit which IOCs can be started or stopped** via
+an IOC ManagerGroup using the *allow_start* and *allow_stop*
+parameters during initialization:
+
+```
+class MyIOC(PVGroup):
+    mission_critical_manager = SubGroup(ManagerGroup,
+					allow_start=True,
+					allow_stop=False)
+```
+
+The status PVs *startable* and *stoppable* are read-only indicators of
+whether the IOC can be controlled via this ManagerGroup. Re-starting
+an IOC requires both *allow_start* and *allow_stop* to be true.
+
 ## Development
 
 To install caproto-apps for development, first clone the github repository:
 
 ```
 git clone https://github.com/canismarko/caproto-apps.git
 ```
```

### Comparing `caproto-apps-0.1.1/src/caprotoapps/alive.py` & `caproto-apps-0.2.0/src/caprotoapps/alive.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,53 +73,62 @@
         name=f".EVD{num}",
         value=value,
         dtype=ChannelType.STRING,
         doc=f"Default Environment Variable Name {num}",
         read_only=True,
     )
 
-def env_messages(*, version: int=5, ioc_type: int, env_variables: Sequence):
+
+def env_messages(*, version: int = 5, ioc_type: int, env_variables: Sequence):
     """Construct the environmental variables message.
 
     Message is suitable to send back to the remote host.
 
     """
     # Get the environmental variable messages
     env_messages = []
     encoding = "ascii"
     for key in env_variables:
         name = key.encode(encoding)
         val = os.environ.get(key, "")
         val = val.encode(encoding)
-        msg = b"".join([
-            struct.pack(">B", len(name)),  # name length
-            name,                          # variable name
-            struct.pack(">H", len(val)),   # value length
-            val,                           # variable value
-        ])
+        msg = b"".join(
+            [
+                struct.pack(">B", len(name)),  # name length
+                name,  # variable name
+                struct.pack(">H", len(val)),  # value length
+                val,  # variable value
+            ]
+        )
         env_messages.append(msg)
     # Build the extra os-specific info
     extra_messages = []
-        # Extra data depending on IOC type
+    # Extra data depending on IOC type
     if ioc_type == IOCType.LINUX:
         uid = getpass.getuser().encode(encoding)
-        uid_msg = b"".join([
-            struct.pack(">B", len(uid)),  # string length
-            uid,
-        ])
+        uid_msg = b"".join(
+            [
+                struct.pack(">B", len(uid)),  # string length
+                uid,
+            ]
+        )
         gid = grp.getgrgid(os.getegid()).gr_name.encode(encoding)
-        gid_msg = b"".join([
-            struct.pack(">B", len(gid)),  # string length
-            gid,
-        ])
+        gid_msg = b"".join(
+            [
+                struct.pack(">B", len(gid)),  # string length
+                gid,
+            ]
+        )
         hostname = socket.gethostname().encode(encoding)
-        hostname_msg = b"".join([
-            struct.pack(">B", len(hostname)),  # string length
-            hostname,
-        ])
+        hostname_msg = b"".join(
+            [
+                struct.pack(">B", len(hostname)),  # string length
+                hostname,
+            ]
+        )
         extra_messages = [uid_msg, gid_msg, hostname_msg]
         log.debug(f"Sending extra info: {uid_msg=}, {gid_msg=}, {hostname_msg=}")
     # Build the header message
     HEADER_LENGTH = 10
     body_length = sum([len(msg) for msg in env_messages])
     extra_info_length = sum([len(msg) for msg in extra_messages])
     message_length = HEADER_LENGTH + body_length + extra_info_length
@@ -129,14 +138,15 @@
     header_message += struct.pack(">H", ioc_type)
     header_message += struct.pack(">I", message_length)
     header_message += struct.pack(">H", num_variables)
     yield header_message
     yield from env_messages
     yield from extra_messages
 
+
 def heartbeat_message(
     magic_number: int,
     incarnation: int | float,
     current_time: int | float,
     heartbeat_value: int,
     period: int | float,
     request_read: bool,
@@ -279,15 +289,15 @@
         # Check for a valid remote host
         addr_is_valid = addr not in invalid_addrs
         port_is_valid = port > 0
         if addr_is_valid and port_is_valid:
             return (addr, port)
         else:
             raise InvalidServerAddress((addr, port))
-    
+
     async def send_heartbeat(self) -> bool:
         """Send a heartbeat message to the alive server.
 
         Returns
         =======
         heartbeat_sent
           True if the heartbeat message was sent, otherwise false.
@@ -296,15 +306,16 @@
 
         """
         if self.hrtbt.value == "Off":
             log.debug("No heartbeat this round, .HRTBT is off.")
             return False
         # Prepare the UDP message
         next_heartbeat = self.val.value + 1
-        make_message = partial(heartbeat_message, 
+        make_message = partial(
+            heartbeat_message,
             magic_number=self.hmag.value,
             incarnation=self.incarnation,
             current_time=time.time(),
             heartbeat_value=next_heartbeat,
             period=self.hprd.value,
             suppress_environment=self.isup.value == "On",
             return_port=self.iport.value,
@@ -331,59 +342,59 @@
         # Send the message to the aux host
         sent_to_aux_host = False
         try:
             addr, port = self.server_address(use_aux=True)
         except InvalidServerAddress:
             pass
         else:
-            request_read = (self.arsts.value=="Queued")
+            request_read = self.arsts.value == "Queued"
             message = make_message(request_read=request_read)
             await self.send_udp_message(message=message, address=(addr, port))
             sent_to_aux_host = True
             # Update read status variable
             match self.arsts.value:
                 case "Queued":
                     await self.arsts.write("Due")
                 case "Due":
                     await self.arsts.write("Overdue")
         # Update the read status PVs
         if sent_to_remote_host or sent_to_aux_host:
-            # Update the heartbeat counter            
+            # Update the heartbeat counter
             await self.val.write(next_heartbeat)
         else:
             log.debug(f"Skipping heartbeat, no valid host set.")
-            
 
     async def send_udp_message(self, message, address):
         """Open a socket and deliver the *message* via UDP to *address*."""
         log.debug(f"Sending UDP to {address}: {message}")
         with self.socket() as sock:
             sock.connect(address)
             loop = self.async_lib.get_running_loop()
             await loop.sock_sendall(sock=sock, data=message)
 
     async def handle_env_request(self, reader, writer):
         # Check for conditions that result in no data being sent
         remote_addr, remote_port = writer.get_extra_info("peername")
-        bad_hostname = (remote_addr not in [self.raddr.value, self.aaddr.value])
+        bad_hostname = remote_addr not in [self.raddr.value, self.aaddr.value]
         is_suppressed = self.isup.value not in ["Off", False, 0]
         if is_suppressed:
             log.debug(f"Suppressing environmental variable reply: {self.isup.value=}")
         if bad_hostname:
-            log.debug(f"Refused env request from host {remote_addr}. Expected {self.raddr.value}")
+            log.debug(
+                f"Refused env request from host {remote_addr}. Expected {self.raddr.value}"
+            )
         if is_suppressed or bad_hostname:
             # Invalid connection: close immediately
             writer.close()
             await writer.wait_closed()
             return
         # Send the env variables message
         messages = env_messages(
             ioc_type=self.ioc_type,
             env_variables=list(self.env_variables.keys()),
-            
         )
         for msg in messages:
             log.debug(f"Sending environment message: {msg}")
             writer.write(msg)
             await writer.drain()
         writer.close()
         await writer.wait_closed()
@@ -406,33 +417,31 @@
             if len(key) <= 0:
                 # No custom value, use default value instead
                 key = getattr(self, f"evd{i}").value
             # Make sure there's a variable there
             if len(key) > 0:
                 evars[key] = os.environ.get(key, "")
         return evars
-    
+
     val = pvproperty(
         name=".VAL", value=0, dtype=int, doc="Heartbeat Value", read_only=True
     )
 
     async def check_env(self, instance, async_lib=None):
         """Update read status PVs if environmental variables have changed."""
         new_vars = self.env_variables
         old_vars = self._env
         if new_vars != old_vars:
             # Environment has changed, so queue read status updates
             await self.rrsts.write("Queued")
             await self.arsts.write("Queued")
             self._env = new_vars
-            
 
     @property
     def ioc_type(self):
-
         """Determine the IOC type based on the current platform."""
         if sys.platform.startswith("linux"):
             return IOCType.LINUX
         elif sys.platform.startswith("darwin"):
             return IOCType.DARWIN
         elif sys.platform.startswith("win32"):
             return IOCType.WINDOWS
@@ -586,55 +595,57 @@
     iport = pvproperty(
         name=".IPORT",
         value=0,
         dtype=int,
         doc="TCP Information Port Number",
         read_only=True,
     )
+
     @iport.startup
     async def iport(self, instance, async_lib):
         """Start a TCP server for env request from the alive daemon."""
         try:
             # Start the server
             tcp_server = await async_lib.library.start_server(
                 client_connected_cb=self.handle_env_request,
                 port=instance.value,
-            )            
+            )
         except Exception as exc:
             # Failed
             await self.ipsts.write(self.InformationPortStatus.Inoperable)
             log.error(f"Could not listen for TCP packets: {exc}")
         else:
             log.info(f"Listening for environmental variable requests: {tcp_server}")
             # Determine listening port
             ip4socket = [s for s in tcp_server.sockets if s.family == socket.AF_INET][0]
             listen_port = ip4socket.getsockname()[1]
             await instance.write(listen_port)
             await self.ipsts.write(self.InformationPortStatus.Operable)
-        
+
     ipsts = pvproperty(
         name=".IPSTS",
         value=InformationPortStatus.Undetermined,
         dtype=InformationPortStatus,
         doc="Information Port Status",
         read_only=True,
     )
     itrig = pvproperty(
         name=".ITRIG",
         value=False,
         dtype=bool,
         doc="Trigger Information Request",
         read_only=False,
     )
+
     @itrig.putter
     async def itrig(self, instance, value):
         await self.rrsts.write(self.HostReadStatus.Queued)
         await self.arsts.write(self.HostReadStatus.Queued)
         return "Off"
-    
+
     isup = pvproperty(
         name=".ISUP",
         value="Off",
         dtype=bool,
         doc="Suppress Information Requests",
         read_only=False,
     )
@@ -657,15 +668,15 @@
     evd10 = envvar_default_property(10)
     evd11 = envvar_default_property(11)
     evd12 = envvar_default_property(12)
     evd13 = envvar_default_property(13)
     evd14 = envvar_default_property(14)
     evd15 = envvar_default_property(15)
     evd16 = envvar_default_property(16)
-    
+
     ev1 = envvar_property(1)
     ev2 = envvar_property(2)
     ev3 = envvar_property(3)
     ev4 = envvar_property(4)
     ev5 = envvar_property(5)
     ev6 = envvar_property(6)
     ev7 = envvar_property(7)
```

### Comparing `caproto-apps-0.1.1/src/caprotoapps/manager.py` & `caproto-apps-0.2.0/src/caprotoapps/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,25 +43,29 @@
     PvpropertyShort,
     PvpropertyShortRO,
     PvpropertyChar,
     SubGroup,
     scan_wrapper,
 )
 
+from . import exceptions
+
 log = logging.getLogger(__name__)
 
 
 script_re = re.compile(
     "^(?:(?P<user>.+)@)?"  # Username (optional)
     "(?:(?P<host>.+):)?"  # Host (optional)
     "(?P<path>/.+)$"  # Script location
 )
 
 
-def parse_script_location(script: str) -> tuple[Optional[str], Optional[str], Optional[str]]:
+def parse_script_location(
+    script: str,
+) -> tuple[Optional[str], Optional[str], Optional[str]]:
     """Extract key parameters from a script path.
 
     Accepts a script specifier in the form:
 
       [[user@]host:]/path/to/script
 
     Returns
@@ -79,23 +83,24 @@
     host = match.group("host")
     path = Path(match.group("path"))
     return (user, host, path)
 
 
 class IOCStatus(IntEnum):
     """Whether the IOC is running or not."""
+
     Unknown = 0
     Stopped = 1
     Running = 2
 
 
-class BaseRunner():
+class BaseRunner:
     def __init__(self, script_path: Path):
         self.script_path = script_path
-        
+
     def start_ioc(self):
         """Start the managed IOC."""
         raise NotImplementedError
 
     def stop_ioc(self):
         """Stop the managed."""
         raise NotImplementedError
@@ -110,30 +115,30 @@
         Returns
         =======
         status
           The running status of the IOC, based on ``IOCStatus`` enum.
 
         """
         raise NotImplementedError
-    
+
     def execute_script(self, args):
         """Execute *args* on target machine."""
         raise NotImplementedError
 
 
 class BCDARunner(BaseRunner):
     def __init__(self, script_path: Path):
         self.script_path = script_path
 
     def execute_script(self, args):
         """Execute *args* on local machine."""
         result = subprocess.run(args, stdout=PIPE, stderr=STDOUT)
         response = result.stdout.decode("utf-8").strip()
         return response
-        
+
     def start_ioc(self):
         """Start the managed IOC."""
         run_args = [str(self.script_path), "start"]
         self.execute_script(args=run_args)
 
     def stop_ioc(self):
         """Stop the managed."""
@@ -159,25 +164,24 @@
         # Parse the status response
         match = re.match(r"^\S+ is (not)? ?running", response)
         if match is None:
             # Garbled response
             log.warning(f"Could not parse IOC status response: {response}")
             return IOCStatus.Unknown
         # Determine the status from the response
-        is_stopped = (match.group(1) == "not")
+        is_stopped = match.group(1) == "not"
         if is_stopped:
             return IOCStatus.Stopped
         else:
             return IOCStatus.Running
-                
 
 
 class BCDASSHRunner(BCDARunner):
     ssh_connection: Connection = None
-    
+
     def __init__(self, user: str, host: str, script_path: Path):
         self.user = user
         self.host = host
         super().__init__(script_path=script_path)
 
     def execute_script(self, args):
         """Execute *args* on local machine."""
@@ -197,94 +201,155 @@
     user, host, path = parse_script_location(script)
     # Check for SSH connections (BCDA style)
     use_ssh = (user is not None) and (host is not None)
     if use_ssh:
         return BCDASSHRunner(user=user, host=host, script_path=path)
     # Last option, use local script
     return BCDARunner(script_path=path)
-    
-        
-    
+
 
 class ManagerGroup(PVGroup):
     """A caproto PV group for managing a separate IOC.
 
     Parameters
     ==========
     script
       The location of the script used to control the target IOC.
     runner
       An instance of ``BaseRunner`` or one of its subclasses. If
       omitted, a default runner will be used based on *script*.
+    allow_start
+      Whether or not it is permitted to start the IOC through this
+      manager
+    allow_stop
+      Whether or not it is permitted to stop the IOC through this
+      manager
 
     """
-    def __init__(self, *args, script: str, runner: BaseRunner = None, **kwargs):
+
+    def __init__(
+        self,
+        *args,
+        script: str,
+        runner: BaseRunner = None,
+        allow_start: bool = True,
+        allow_stop: bool = True,
+        **kwargs,
+    ):
         self._script = script
+        self.allow_start = allow_start
+        self.allow_stop = allow_stop
         # Set up a runner if one does not exist
         if runner is None:
             self.runner = guess_runner(script)
         else:
             self.runner = runner
         super().__init__(*args, **kwargs)
 
     # PVs for changing the IOC state
-    start = pvproperty(name="start", value="Off", dtype=bool, doc="Start the remote IOC.")
+    startable = pvproperty(
+        name="startable",
+        value="On",
+        dtype=bool,
+        read_only=True,
+        doc="Can the remote IOC be started.",
+    )
+
+    @startable.startup
+    async def startable(self, instance, async_lib):
+        is_startable = "On" if self.allow_start else "Off"
+        await instance.write(is_startable)
+
+    start = pvproperty(
+        name="start", value="Off", dtype=bool, doc="Start the remote IOC."
+    )
 
     @start.putter
     async def start(self, instance, value):
         """Trigger a remote IOC to start."""
+        # Confirm we are allow to start the IOC
+        if self.startable.value != "On":
+            msg = "Cannot start IOC. Provide *allow_start=True* to enable remote starting."
+            raise exceptions.NotPermitted(msg)
         # Execute the runner's control function
         loop = self.async_lib.get_running_loop()
         await loop.run_in_executor(None, self.runner.start_ioc)
         # Return the trigger to its default value
         return "Off"
 
     @start.startup
     async def start(self, instance, async_lib):
         # Just here to get the async lib on startup
         self.async_lib = async_lib.library
-    
+
+    # PVs for changing the IOC state
+    stoppable = pvproperty(
+        name="stoppable",
+        value="On",
+        dtype=bool,
+        read_only=True,
+        doc="Can the remote IOC be stopped.",
+    )
+
+    @stoppable.startup
+    async def stoppable(self, instance, async_lib):
+        is_stoppable = "On" if self.allow_stop else "Off"
+        await instance.write(is_stoppable)
+
     stop = pvproperty(name="stop", value="Off", dtype=bool, doc="Stop the remote IOC.")
 
     @stop.putter
     async def stop(self, instance, value):
+        # Confirm we are allow to start the IOC
+        if self.stoppable.value != "On":
+            msg = (
+                "Cannot stop IOC. Provide *allow_stop=True* to enable remote stopping."
+            )
+            raise exceptions.NotPermitted(msg)
         # Execute the runner's control function
         loop = self.async_lib.get_running_loop()
         await loop.run_in_executor(None, self.runner.stop_ioc)
         # Return the trigger to its default value
         return "Off"
-    
-    restart = pvproperty(name="restart", value="Off", dtype=bool, doc="Restart the remote IOC.")
+
+    restart = pvproperty(
+        name="restart", value="Off", dtype=bool, doc="Restart the remote IOC."
+    )
 
     @restart.putter
     async def restart(self, instance, value):
+        # Confirm we are allowed to restart the IOC
+        if (self.startable.value != "On") or (self.stoppable.value != "On"):
+            msg = (
+                "Cannot stop IOC. Provide *allow_stop=True* to enable remote stopping."
+            )
+            raise exceptions.NotPermitted(msg)
         # Execute the runner's control function
         loop = self.async_lib.get_running_loop()
         await loop.run_in_executor(None, self.runner.restart_ioc)
         # Return the trigger to its default value
         return "Off"
-    
 
     # PVs for monitoring the IOC state
     status = pvproperty(
         name="status",
         value="Unknown",
         enum_strings=["Unknown", "Stopped", "Running"],
         record="mbbi",
         dtype=ChannelType.ENUM,
-        doc="The current status of the IOC."
+        doc="The current status of the IOC.",
     )
 
     @status.scan(1, use_scan_field=True)
     async def status(self, instance, async_lib):
         loop = self.async_lib.get_running_loop()
         new_status = await loop.run_in_executor(None, self.runner.ioc_status)
         old_status = getattr(IOCStatus, instance.value)
         if new_status != old_status:
             await instance.write(new_status)
-        
+
     console_command = pvproperty(
         name="console",
         value="",
         dtype=ChannelType.STRING,
-        doc="The command needed to connect to the remote console."
+        doc="The command needed to connect to the remote console.",
     )
```

### Comparing `caproto-apps-0.1.1/tests/test_alive.py` & `caproto-apps-0.2.0/tests/test_alive.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     await ioc.alive.iocnm.startup(ioc.alive.iocnm, None)
     assert ioc.alive.iocnm.value == "my_ioc"
 
 
 @pytest.fixture()
 def writer():
     writer = mock.AsyncMock()
-    writer.get_extra_info = mock.MagicMock(return_value = ("9.9.9.9", 0))
+    writer.get_extra_info = mock.MagicMock(return_value=("9.9.9.9", 0))
     writer.write = mock.MagicMock()
     writer.close = mock.MagicMock()
     yield writer
 
 
 @pytest.mark.asyncio
 async def test_env_callback_suppressed(test_ioc, writer):
@@ -213,40 +213,42 @@
     reader = mock.AsyncMock()
     # Ask for some environmental variables
     await alive_group.handle_env_request(reader, writer)
     assert writer.write.called
     # Check response messages
     messages = [call.args[0] for call in writer.write.call_args_list]
     # Information message
-    info_target = (
-        b"\x00\x05"  # Version
-        b"\x00\x02"  # IOC type: Linux
-    )
+    info_target = b"\x00\x05" b"\x00\x02"  # Version  # IOC type: Linux
     assert messages[0].startswith(info_target)
 
 
 def test_env_messages(monkeypatch):
     env_variables = [
         ("ENGINEER", "Quig"),
         ("PREFIX", "test_ioc:"),
     ]
     body_length = sum([len(k) + len(v) for k, v in env_variables])
     for key, val in env_variables:
         monkeypatch.setenv(key, val)
-    messages = alive.env_messages(version=4, ioc_type=alive.IOCType.LINUX,
-                                  env_variables=[d[0] for d in env_variables])
+    messages = alive.env_messages(
+        version=4,
+        ioc_type=alive.IOCType.LINUX,
+        env_variables=[d[0] for d in env_variables],
+    )
     # Check the header
     header, *remaining_messages = messages
     expected_length = 10 + sum([len(m) for m in remaining_messages])
-    expected_header = b"".join([
-        b"\x00\x04",  # Version
-        b"\x00\x02",  # IOC type: Linux
-        struct.pack(">I", expected_length), # E.g. b"\x00\x00\x00\x50" 
-        b"\x00\x02", # Variable count
-    ])
+    expected_header = b"".join(
+        [
+            b"\x00\x04",  # Version
+            b"\x00\x02",  # IOC type: Linux
+            struct.pack(">I", expected_length),  # E.g. b"\x00\x00\x00\x50"
+            b"\x00\x02",  # Variable count
+        ]
+    )
     assert header == expected_header
     # Check individual variable's messages
     assert len(remaining_messages) == len(env_variables) + 3  # +3 for IOC-specific data
 
 
 @pytest.mark.asyncio
 async def test_env_variable_list(test_ioc):
@@ -255,42 +257,42 @@
     await alive_group.evd1.write("ENGINEER")
     await alive_group.evd2.write("ARCH")
     await alive_group.evd3.write("")
     await alive_group.evd4.write("")
     await alive_group.evd5.write("")
     await alive_group.ev2.write("HOST_ARCH")
     assert list(alive_group.env_variables.keys()) == ["ENGINEER", "HOST_ARCH"]
-    
-    
+
+
 @pytest.mark.asyncio
 async def test_read_status_fields(test_ioc, writer):
     """Check that the ITRIG field gets set automatically."""
     reader = mock.AsyncMock()
     alive_group = test_ioc.alive
     await alive_group.raddr.write("9.9.9.9")
     await alive_group.rport.write(999)
     await alive_group.rrsts.write("Idle")
     # Check that the flag is off if no env update is requested
     await alive_group.send_heartbeat()
     assert alive_group.send_udp_message.called
-    msg = alive_group.send_udp_message.call_args.kwargs['message']
+    msg = alive_group.send_udp_message.call_args.kwargs["message"]
     flags = msg[20:22]
     assert flags == b"\x00\x00"
     # Setup the trigger status
     assert alive_group.rrsts.value == "Idle"
     await alive_group.itrig.write(True)
     assert alive_group.itrig.value == "Off"
     assert alive_group.rrsts.value == "Queued"
     # Does the ITRIG field get once the next heartbeat goes out?
     await alive_group.send_heartbeat()
     assert alive_group.itrig.value == "Off"
     assert alive_group.rrsts.value == "Due"
     # Check that the message had the right flags set
     assert alive_group.send_udp_message.called
-    msg = alive_group.send_udp_message.call_args.kwargs['message']
+    msg = alive_group.send_udp_message.call_args.kwargs["message"]
     flags = msg[20:22]
     assert flags == b"\x00\x01"
     # Check that the read status flag gets cleared
     await alive_group.handle_env_request(reader, writer)
     assert alive_group.rrsts.value == "Idle"
```

