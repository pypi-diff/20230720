# Comparing `tmp/kcp_py-0.1.3.tar.gz` & `tmp/kcp_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcp_py-0.1.3.tar", max compression
+gzip compressed data, was "kcp_py-0.1.4.tar", max compression
```

## Comparing `kcp_py-0.1.3.tar` & `kcp_py-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1779 2023-01-17 18:35:47.938062 kcp_py-0.1.3/build.py
--rw-r--r--   0        0        0      411 2023-01-31 20:08:45.020948 kcp_py-0.1.3/kcp/__init__.py
--rw-r--r--   0        0        0     3234 2023-01-20 10:45:41.918551 kcp_py-0.1.3/kcp/client.py
--rw-r--r--   0        0        0      346 2023-01-15 19:20:40.559581 kcp_py-0.1.3/kcp/exceptions.py
--rw-r--r--   0        0        0     4666 2023-01-24 22:34:07.771480 kcp_py-0.1.3/kcp/extension.pyi
--rw-r--r--   0        0        0     9932 2023-01-24 22:34:31.411249 kcp_py-0.1.3/kcp/extension.pyx
--rw-r--r--   0        0        0    32985 2023-01-15 12:41:33.257786 kcp_py-0.1.3/kcp/ikcp.c
--rw-r--r--   0        0        0    12436 2023-01-15 12:41:33.259786 kcp_py-0.1.3/kcp/ikcp.h
--rw-r--r--   0        0        0        0 2023-01-14 21:22:51.329350 kcp_py-0.1.3/kcp/py.typed
--rw-r--r--   0        0        0     7202 2023-01-31 20:08:18.871503 kcp_py-0.1.3/kcp/server.py
--rw-r--r--   0        0        0     1090 2023-01-14 17:49:15.682359 kcp_py-0.1.3/LICENSE
--rw-r--r--   0        0        0     1998 2023-01-31 20:08:45.020948 kcp_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1807 2023-01-23 22:30:07.675183 kcp_py-0.1.3/README.md
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 kcp_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1779 2023-01-17 18:35:47.938062 kcp_py-0.1.4/build.py
+-rw-r--r--   0        0        0      411 2023-07-20 15:55:39.339596 kcp_py-0.1.4/kcp/__init__.py
+-rw-r--r--   0        0        0     4473 2023-07-12 18:31:08.825939 kcp_py-0.1.4/kcp/client.py
+-rw-r--r--   0        0        0      310 2023-07-12 18:37:43.552801 kcp_py-0.1.4/kcp/exceptions.py
+-rw-r--r--   0        0        0     4666 2023-01-24 22:34:07.771480 kcp_py-0.1.4/kcp/extension.pyi
+-rw-r--r--   0        0        0     9932 2023-07-20 15:59:24.081818 kcp_py-0.1.4/kcp/extension.pyx
+-rw-r--r--   0        0        0    32985 2023-01-15 12:41:33.257786 kcp_py-0.1.4/kcp/ikcp.c
+-rw-r--r--   0        0        0    12436 2023-01-15 12:41:33.259786 kcp_py-0.1.4/kcp/ikcp.h
+-rw-r--r--   0        0        0        0 2023-01-14 21:22:51.329350 kcp_py-0.1.4/kcp/py.typed
+-rw-r--r--   0        0        0    10282 2023-07-19 20:36:48.280064 kcp_py-0.1.4/kcp/server.py
+-rw-r--r--   0        0        0     1090 2023-01-14 17:49:15.682359 kcp_py-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1998 2023-07-20 16:03:35.743013 kcp_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2052 2023-07-12 18:39:09.412762 kcp_py-0.1.4/README.md
+-rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 kcp_py-0.1.4/PKG-INFO
```

### Comparing `kcp_py-0.1.3/build.py` & `kcp_py-0.1.4/build.py`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/kcp/extension.pyi` & `kcp_py-0.1.4/kcp/extension.pyi`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/kcp/extension.pyx` & `kcp_py-0.1.4/kcp/extension.pyx`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/kcp/ikcp.c` & `kcp_py-0.1.4/kcp/ikcp.c`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/kcp/ikcp.h` & `kcp_py-0.1.4/kcp/ikcp.h`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/kcp/server.py` & `kcp_py-0.1.4/kcp/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .extension import KCP
 
 
 DataMutator = Callable[[bytes], bytes]
 
 
-@dataclass()
+@dataclass
 class Connection:
     _kcp: KCP
     _server: KCPServerAsync
     address: str
     port: int
     last_active: float
     _data_mutators: list[DataMutator]
@@ -33,29 +33,32 @@
 
     def _perform_mutations(self, data: bytes) -> bytes:
         for mutator in self._data_mutators:
             data = mutator(data)
 
         return data
 
+    def __update_activity(self) -> None:
+        self.last_active = time.perf_counter()
+
     async def receive(self, data: bytes) -> None:
         """Handles receiving data from the client."""
         self._kcp.receive(data)
 
-        self.last_active = time.perf_counter()
-        assert self._server._data_handler is not None # SHUT UP MYPY
+        self.__update_activity()
+        assert self._server._data_handler is not None  # SHUT UP MYPY
 
         for data in self._kcp.get_all_received():
             data = self._perform_mutations(data)
             await self._server._data_handler(self, data)
 
     def enqueue(self, data: bytes) -> None:
         """Enqueues data to be sent to the client."""
         self._kcp.enqueue(data)
-        self.last_active = time.perf_counter()
+        self.__update_activity()
 
     # Functions for the kcp extension
     def _send_kcp(self, _, data: bytes) -> None:
         self._server._transport.sendto(  # type: ignore
             data,
             self.address_tuple,
         )
@@ -88,24 +91,39 @@
     def __init__(
         self,
         address: str,
         port: int,
         conv_id: int,
         delay: int = 100,
         connection_timeout: int = 600,
+        max_transmission: int = 1400,
+        no_delay: bool = False,
+        resend_count: int = 2,
+        no_congestion_control: bool = False,
+        receive_window_size: int = 128,
+        send_window_size: int = 32,
     ) -> None:
         """Configures the asynchronous KCP server.
 
         :param address: The address to listen on (usually `127.0.0.1`).
         :param port: The port to listen on.
         :param conv: The conversation number to use for the KCP protocol.
         :param delay: The delay between KCP updates in milliseconds.
         :param connection_timeout: The amount of time in seconds to wait before
             cleaning up after a connection.
+        :param max_transmission: The maximum transmission unit (MTU) of outbound
+            packets.
+        :param no_delay: Whether to enable no-delay mode.
+        :param resend_count: The number of times to resend a packet if it is
+            not acknowledged.
+        :param no_congestion_control: Whether to disable congestion control.
+        :param receive_window_size: The size of the receive window in packets.
+        :param send_window_size: The size of the send window in packets.
         """
+
         self.address = address
         self.port = port
         self._transport: Optional[transports.DatagramTransport] = None
         self._loop = asyncio.get_event_loop()
         self._conv = conv_id
         self._delay = delay
 
@@ -116,25 +134,43 @@
         # Event handlers
         self._data_handler: Optional[DataHandler] = None
         self._on_start: Optional[EventHandler] = None
         self._on_stop: Optional[EventHandler] = None
 
         self._data_mutators: list[DataMutator] = []
 
+        # Connection settings.
+        self._max_transmission = max_transmission
+        self._no_delay = no_delay
+        self._resend_count = resend_count
+        self._no_congestion_control = no_congestion_control
+        self._send_window_size = send_window_size
+        self._receive_window_size = receive_window_size
+
     # Private API
     # Called by the protocol.
     def datagram_received(self, data: bytes, address: AddressType) -> None:
         connection = self._ensure_connection(address)
         self._loop.create_task(connection.receive(data))
 
     def _ensure_connection(self, address: AddressType) -> Connection:
         connection = self._connections.get(address)
         if connection is None:
+            kcp = KCP(
+                self._conv,
+                max_transmission=self._max_transmission,
+                no_delay=self._no_delay,
+                update_interval=self._delay,
+                resend_count=self._resend_count,
+                no_congestion_control=self._no_congestion_control,
+                send_window_size=self._send_window_size,
+                receive_window_size=self._receive_window_size,
+            )
             connection = Connection(
-                _kcp=KCP(self._conv),
+                _kcp=kcp,
                 _server=self,
                 address=address[0],
                 port=address[1],
                 last_active=time.perf_counter(),
                 _data_mutators=self._data_mutators.copy(),
             )
             self._connections[address] = connection
@@ -171,14 +207,47 @@
         self._transport.close()
         self._transport = None
         self._connections.clear()
 
         if self._on_stop is not None:
             await self._on_stop()
 
+    def set_performance_options(
+        self,
+        no_delay: Optional[bool] = None,
+        update_interval: Optional[int] = None,
+        resend_count: Optional[int] = None,
+        no_congestion_control: Optional[bool] = None,
+        receive_window_size: Optional[int] = None,
+        send_window_size: Optional[int] = None,
+    ) -> None:
+        """Configures the performance options for all **future** KCP connections.
+
+        :param no_delay: Whether to enable no-delay mode.
+        :param update_interval: The internal update interval in milliseconds.
+        :param resend_count: The number of times to resend a packet if it is
+        not acknowledged.
+        :param no_congestion_control: Whether to disable congestion control.
+        """
+
+        self._no_delay = no_delay if no_delay is not None else self._no_delay
+        self._delay = update_interval if update_interval is not None else self._delay
+        self._resend_count = resend_count if resend_count is not None else self._resend_count
+        self._no_congestion_control = (
+            no_congestion_control
+            if no_congestion_control is not None
+            else self._no_congestion_control
+        )
+        self._receive_window_size = (
+            receive_window_size if receive_window_size is not None else self._receive_window_size
+        )
+        self._send_window_size = (
+            send_window_size if send_window_size is not None else self._send_window_size
+        )
+
     def start(self) -> None:
         """Creates the event loop and starts listening for connections."""
         self._loop.run_until_complete(self.listen())
 
     def stop(self) -> None:
         """Tells the server to stop listening for connections after the next
         update loop."""
```

### Comparing `kcp_py-0.1.3/LICENSE` & `kcp_py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kcp_py-0.1.3/pyproject.toml` & `kcp_py-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kcp.py"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python bindings and networking for the KCP protocol."
 authors = ["RealistikDash"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/RealistikDash/kcp.py"
@@ -47,46 +47,46 @@
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.8.0"
+black = "23.1.0"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
+version = "5.11.5"
 python = "^3.7"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
+pytest = "7.2.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.2"
+mkdocs-material = "9.1.0"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.20.0"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.0.0"
+changelogging = "1.1.0"
 
 [tool.black]
 line_length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [build-system]
-requires = ["poetry-core >= 1.3.2", "cython >= 0.29.32", "entrypoint >= 1.3.0", "setuptools >= 65.6.3"]
+requires = ["poetry-core >= 1.3.2", "cython == 0.29.32", "entrypoint >= 1.3.0", "setuptools >= 65.6.3"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kcp_py-0.1.3/README.md` & `kcp_py-0.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,41 +8,50 @@
 kcp.py is available on [PyPi](https://pypi.org/project/kcp-py/), meaning installing is as simple as running
 ```sh
 pip install kcp.py
 ```
 
 ## Examples
 ### Asynchronous Server
-kcp.py features an implementation of an asynchronous servers using the event loop protocol API.
+kcp.py features an implementation of an asynchronous server using the event loop protocol API.
 ```py
 from kcp.server import Connection
 from kcp.server import KCPServerAsync
 
+# Create the initial server instance.
 server = KCPServerAsync(
     "127.0.0.1",
     9999,
     conv_id=1,
+    no_delay=True,
+)
+
+# Ability to set performance options after initialisation.
+server.set_performance_options(
+    update_interval=10,
 )
 
 
+# Ran when the server starts.
 @server.on_start
 async def on_start() -> None:
     print("Server started!")
 
 
+# Ran when a connection is made.
 @server.on_data
 async def on_data(connection: Connection, data: bytes) -> None:
     print(f"Received data from {connection.address}: {data}")
 
 
 server.start()
 ```
 
 ### Client
-kcp.py also implements a KCP clients using Python's sockets and threads.
+kcp.py also implements a KCP client using Python's sockets and threads.
 ```py
 from kcp import KCPClientSync
 
 client = KCPClientSync(
     "127.0.0.1",
     9999,
     conv_id=1,
```

### Comparing `kcp_py-0.1.3/PKG-INFO` & `kcp_py-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcp-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings and networking for the KCP protocol.
 Home-page: https://github.com/RealistikDash/kcp.py
 License: MIT
 Keywords: kcp,server,client,async,asyncio
 Author: RealistikDash
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -34,41 +34,50 @@
 kcp.py is available on [PyPi](https://pypi.org/project/kcp-py/), meaning installing is as simple as running
 ```sh
 pip install kcp.py
 ```
 
 ## Examples
 ### Asynchronous Server
-kcp.py features an implementation of an asynchronous servers using the event loop protocol API.
+kcp.py features an implementation of an asynchronous server using the event loop protocol API.
 ```py
 from kcp.server import Connection
 from kcp.server import KCPServerAsync
 
+# Create the initial server instance.
 server = KCPServerAsync(
     "127.0.0.1",
     9999,
     conv_id=1,
+    no_delay=True,
+)
+
+# Ability to set performance options after initialisation.
+server.set_performance_options(
+    update_interval=10,
 )
 
 
+# Ran when the server starts.
 @server.on_start
 async def on_start() -> None:
     print("Server started!")
 
 
+# Ran when a connection is made.
 @server.on_data
 async def on_data(connection: Connection, data: bytes) -> None:
     print(f"Received data from {connection.address}: {data}")
 
 
 server.start()
 ```
 
 ### Client
-kcp.py also implements a KCP clients using Python's sockets and threads.
+kcp.py also implements a KCP client using Python's sockets and threads.
 ```py
 from kcp import KCPClientSync
 
 client = KCPClientSync(
     "127.0.0.1",
     9999,
     conv_id=1,
```

