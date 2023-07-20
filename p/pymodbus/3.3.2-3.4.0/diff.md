# Comparing `tmp/pymodbus-3.3.2.tar.gz` & `tmp/pymodbus-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.3.2.tar", last modified: Wed Jun 21 15:05:43 2023, max compression
+gzip compressed data, was "pymodbus-3.4.0.tar", last modified: Thu Jul 20 12:31:08 2023, max compression
```

## Comparing `pymodbus-3.3.2.tar` & `pymodbus-3.4.0.tar`

### file list

```diff
@@ -1,139 +1,135 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.915977 pymodbus-3.3.2/
--rw-r--r--   0 jan        (501) staff       (20)    26849 2023-06-21 13:55:50.000000 pymodbus-3.3.2/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-09 17:19:30.000000 pymodbus-3.3.2/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-09 17:19:30.000000 pymodbus-3.3.2/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    18292 2023-06-21 15:05:43.916066 pymodbus-3.3.2/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    16798 2023-06-21 15:05:31.000000 pymodbus-3.3.2/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.904849 pymodbus-3.3.2/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9540 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9532 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.906506 pymodbus-3.3.2/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    11845 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/serial.py
--rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907039 pymodbus-3.3.2/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4796 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/datastore/remote.py
--rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907738 pymodbus-3.3.2/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/base.py
--rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/mei_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14300 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12510 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.907845 pymodbus-3.3.2/pymodbus/repl/
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908309 pymodbus-3.3.2/pymodbus/repl/client/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/client/completer.py
--rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/client/helper.py
--rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/repl/client/main.py
--rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/repl/client/mclient.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908645 pymodbus-3.3.2/pymodbus/repl/server/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/repl/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/repl/server/cli.py
--rw-r--r--   0 jan        (501) staff       (20)     6417 2023-06-21 13:55:50.000000 pymodbus-3.3.2/pymodbus/repl/server/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.908888 pymodbus-3.3.2/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    47906 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.909250 pymodbus-3.3.2/pymodbus/server/reactive/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.2/pymodbus/server/reactive/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/reactive/default_config.py
--rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/server/reactive/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.909843 pymodbus-3.3.2/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/setup.json
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.911462 pymodbus-3.3.2/pymodbus/server/simulator/web/
--rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple120.png
--rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple152.png
--rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple60.png
--rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/apple76.png
--rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/favicon.ico
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912192 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/
--rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/calls
--rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/log
--rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
--rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/registers
--rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/generator/server
--rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/index.html
--rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/pymodbus.css
--rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/server/simulator/web/welcome.html
--rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/transaction.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912420 pymodbus-3.3.2/pymodbus/transport/
--rw-r--r--   0 jan        (501) staff       (20)       17 2023-06-14 11:10:10.000000 pymodbus-3.3.2/pymodbus/transport/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.912529 pymodbus-3.3.2/pymodbus/transport/serial_asyncio/
--rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/transport/serial_asyncio/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    14940 2023-06-21 15:05:31.000000 pymodbus-3.3.2/pymodbus/transport/transport.py
--rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-09 17:19:30.000000 pymodbus-3.3.2/pymodbus/utilities.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.905601 pymodbus-3.3.2/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    18292 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-21 15:05:43.000000 pymodbus-3.3.2/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.2/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-21 15:05:31.000000 pymodbus-3.3.2/requirements.txt
--rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-21 15:05:43.916674 pymodbus-3.3.2/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-09 17:19:30.000000 pymodbus-3.3.2/setup.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-21 15:05:43.915874 pymodbus-3.3.2/test/
--rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_all_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_bit_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_bit_write_messages.py
--rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_client.py
--rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_client_faulty_response.py
--rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_client_sync.py
--rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_diag_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_events.py
--rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_example_client_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     7228 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_examples.py
--rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_mei_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_other_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_register_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_register_write_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2661 2023-06-21 13:55:50.000000 pymodbus-3.3.2/test/test_remote_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_repl_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_server_asyncio.py
--rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_server_context.py
--rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_server_multidrop.py
--rwxr-xr-x   0 jan        (501) staff       (20)    10930 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_server_task.py
--rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_simulator.py
--rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_sparse_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_transaction.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-21 15:05:31.000000 pymodbus-3.3.2/test/test_unix_socket.py
--rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-09 17:19:30.000000 pymodbus-3.3.2/test/test_utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.408580 pymodbus-3.4.0/
+-rw-r--r--   0 jan        (501) staff       (20)    28645 2023-07-20 12:09:25.000000 pymodbus-3.4.0/CHANGELOG.rst
+-rw-r--r--   0 jan        (501) staff       (20)     1392 2023-07-20 10:02:40.000000 pymodbus-3.4.0/LICENSE
+-rw-r--r--   0 jan        (501) staff       (20)       82 2023-07-20 10:02:40.000000 pymodbus-3.4.0/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)    12723 2023-07-20 12:31:08.408671 pymodbus-3.4.0/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    11229 2023-07-20 12:09:40.000000 pymodbus-3.4.0/README.rst
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.397452 pymodbus-3.4.0/pymodbus/
+-rw-r--r--   0 jan        (501) staff       (20)      316 2023-07-20 12:10:15.000000 pymodbus-3.4.0/pymodbus/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     9422 2023-07-20 12:10:28.000000 pymodbus-3.4.0/pymodbus/bit_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     9532 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/bit_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.399142 pymodbus-3.4.0/pymodbus/client/
+-rw-r--r--   0 jan        (501) staff       (20)      602 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    12304 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/base.py
+-rw-r--r--   0 jan        (501) staff       (20)    21046 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/client/mixin.py
+-rw-r--r--   0 jan        (501) staff       (20)     9723 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     9337 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/tcp.py
+-rw-r--r--   0 jan        (501) staff       (20)     5779 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/tls.py
+-rw-r--r--   0 jan        (501) staff       (20)     5629 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/udp.py
+-rw-r--r--   0 jan        (501) staff       (20)     3982 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/constants.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.399712 pymodbus-3.4.0/pymodbus/datastore/
+-rw-r--r--   0 jan        (501) staff       (20)      491 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/datastore/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7130 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/context.py
+-rw-r--r--   0 jan        (501) staff       (20)     4761 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/remote.py
+-rw-r--r--   0 jan        (501) staff       (20)    30290 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)    11410 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/datastore/store.py
+-rw-r--r--   0 jan        (501) staff       (20)    22669 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/device.py
+-rw-r--r--   0 jan        (501) staff       (20)    30455 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/diag_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     6481 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/events.py
+-rw-r--r--   0 jan        (501) staff       (20)     3206 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)    13673 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    14708 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/file_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.400491 pymodbus-3.4.0/pymodbus/framer/
+-rw-r--r--   0 jan        (501) staff       (20)      509 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/framer/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5303 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     4448 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/base.py
+-rw-r--r--   0 jan        (501) staff       (20)     6059 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)    12255 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     6445 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     4332 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     3921 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     7745 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/mei_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15360 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/other_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15651 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     7713 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)        0 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/py.typed
+-rw-r--r--   0 jan        (501) staff       (20)    14208 2023-07-20 12:10:38.000000 pymodbus-3.4.0/pymodbus/register_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    12510 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/register_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.400598 pymodbus-3.4.0/pymodbus/repl/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401157 pymodbus-3.4.0/pymodbus/repl/client/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5187 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/repl/client/completer.py
+-rw-r--r--   0 jan        (501) staff       (20)     9526 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/client/helper.py
+-rw-r--r--   0 jan        (501) staff       (20)    13184 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/repl/client/main.py
+-rw-r--r--   0 jan        (501) staff       (20)    23074 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/repl/client/mclient.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401557 pymodbus-3.4.0/pymodbus/repl/server/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6912 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/server/cli.py
+-rw-r--r--   0 jan        (501) staff       (20)     6417 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/server/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401775 pymodbus-3.4.0/pymodbus/server/
+-rw-r--r--   0 jan        (501) staff       (20)      996 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    29227 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/server/async_io.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.402138 pymodbus-3.4.0/pymodbus/server/reactive/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/server/reactive/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1824 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/reactive/default_config.py
+-rw-r--r--   0 jan        (501) staff       (20)    18653 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/reactive/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.402772 pymodbus-3.4.0/pymodbus/server/simulator/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 jan        (501) staff       (20)    25319 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     4198 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/main.py
+-rw-r--r--   0 jan        (501) staff       (20)     7619 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.404024 pymodbus-3.4.0/pymodbus/server/simulator/web/
+-rw-r--r--   0 jan        (501) staff       (20)    11369 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 jan        (501) staff       (20)    15391 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 jan        (501) staff       (20)     4817 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 jan        (501) staff       (20)     6344 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 jan        (501) staff       (20)    12014 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.404773 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 jan        (501) staff       (20)     4314 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 jan        (501) staff       (20)     1132 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 jan        (501) staff       (20)     5850 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 jan        (501) staff       (20)     2710 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 jan        (501) staff       (20)      893 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 jan        (501) staff       (20)     1944 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 jan        (501) staff       (20)      919 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 jan        (501) staff       (20)      710 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 jan        (501) staff       (20)    23600 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/transaction.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.405009 pymodbus-3.4.0/pymodbus/transport/
+-rw-r--r--   0 jan        (501) staff       (20)       17 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/transport/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.405138 pymodbus-3.4.0/pymodbus/transport/serial_asyncio/
+-rw-r--r--   0 jan        (501) staff       (20)    19336 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/transport/serial_asyncio/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    19112 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/transport/transport.py
+-rw-r--r--   0 jan        (501) staff       (20)     7797 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.398200 pymodbus-3.4.0/pymodbus.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    12723 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)     3402 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)      173 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 jan        (501) staff       (20)      481 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.4.0/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 jan        (501) staff       (20)     1897 2023-07-20 12:08:56.000000 pymodbus-3.4.0/requirements.txt
+-rw-r--r--   0 jan        (501) staff       (20)     4391 2023-07-20 12:31:08.409390 pymodbus-3.4.0/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1105 2023-07-20 10:02:40.000000 pymodbus-3.4.0/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.408479 pymodbus-3.4.0/test/
+-rw-r--r--   0 jan        (501) staff       (20)     3643 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_all_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     4594 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_bit_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5244 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_bit_write_messages.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    17813 2023-07-20 12:30:55.000000 pymodbus-3.4.0/test/test_client.py
+-rw-r--r--   0 jan        (501) staff       (20)     1315 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_client_faulty_response.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    15957 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_client_sync.py
+-rw-r--r--   0 jan        (501) staff       (20)    13200 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_device.py
+-rw-r--r--   0 jan        (501) staff       (20)     8354 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_diag_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2359 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_events.py
+-rw-r--r--   0 jan        (501) staff       (20)      771 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)     8499 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    10180 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_file_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    11230 2023-07-20 12:30:55.000000 pymodbus-3.4.0/test/test_framers.py
+-rw-r--r--   0 jan        (501) staff       (20)     1238 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     6297 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_mei_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5687 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_other_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     8771 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     2814 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)     7450 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_register_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     7658 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_register_write_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2661 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_remote_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_repl_client.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    14440 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_server_asyncio.py
+-rw-r--r--   0 jan        (501) staff       (20)     3546 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_server_context.py
+-rw-r--r--   0 jan        (501) staff       (20)     8192 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_server_multidrop.py
+-rw-r--r--   0 jan        (501) staff       (20)    23028 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)      649 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_sparse_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    31231 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_transaction.py
+-rw-r--r--   0 jan        (501) staff       (20)     3107 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_utilities.py
```

### Comparing `pymodbus-3.3.2/CHANGELOG.rst` & `pymodbus-3.4.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,62 @@
+version 3.4.0
+----------------------------------------------------------
+* Prepare v3.4.0.
+* Handle partial local echo. (#1675)
+* clarify handle_local_echo. (#1674)
+* async_client: add retries/reconnect. (#1672)
+* Fix 3.11 problem. (#1673)
+* Add new example simulator server/client. (#1671)
+* `examples/contrib/explain.py` leveraging Rapid SCADA (#1665)
+* _logger missed basicConfig. (#1670)
+* Bug fix for #1662 (#1663)
+* Bug fix for #1661 (#1664)
+* Fix typo in config.rst (#1660)
+* test action_increment. (#1659)
+* test codeql (#1655)
+* mypy complaints. (#1656)
+* Remove self.params from async client (#1640)
+* Drop test of pypy with python 3.8.
+* repair server_async.py (#1644)
+* move common framer to base. (#1639)
+* Restrict Return diag call to bytes. (#1638)
+* use slave= in diag requests. (#1636)
+* transport listen in server. (#1628)
+* CI test.
+* Integrate transport in server. (#1617)
+* fix getFrameStart for ExceptionResponse (#1627)
+* Add min/min to simulator actions.
+* Change to "sync client" in forwarder example (#1625)
+* Remove docker (lack of maintenance). (#1623)
+* Clean defaults (#1618)
+* Reduce CI log with no debug. (#1616)
+* prepare server to use transport. (#1607)
+* Fix RemoteSlaveContext (#1599)
+* Combine stale and lock. (#1608)
+* update pytest + extensions. (#1610)
+* Change version follow PEP 440. (#1609)
+* Fix regression with REPL server not listening (#1604)
+* Remove handler= for server classes. (#1602)
+* Fix write function codes (#1598)
+* transport nullmodem (#1591)
+* move test of examples to subdirectory. (#1592)
+* transport as object, not base class. (#1572)
+* Simple examples. (#1590)
+* transport_connect as bool. (#1587)
+* Prepare dev (#1588)
+* Release corrections. (#1586)
+
+Thanks to:
+    Alex
+    Fredo70
+    Hangyu Fan
+    James Braza
+    jan iversen
+
+
 version 3.3.2
 ----------------------------------------------------------
 * Fix RemoteSlaveContext (#1599)
 * Change version follow PEP 440. (#1609)
 * Fix regression with REPL server not listening (#1604)
 * Fix write function codes (#1598)
 * Release corrections. (#1586)
```

### Comparing `pymodbus-3.3.2/LICENSE` & `pymodbus-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/bit_read_message.py` & `pymodbus-3.4.0/pymodbus/bit_read_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,25 @@
     "ReadDiscreteInputsRequest",
     "ReadDiscreteInputsResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
-from pymodbus.constants import Defaults
 from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
 from pymodbus.utilities import pack_bitstring, unpack_bitstring
 
 
 class ReadBitsRequestBase(ModbusRequest):
     """Base class for Messages Requesting bit values."""
 
     _rtu_frame_size = 8
 
-    def __init__(self, address, count, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address, count, slave=0, **kwargs):
         """Initialize the read request data.
 
         :param address: The start address to read from
         :param count: The number of bits after "address" to read
         :param slave: Modbus slave slave ID
         """
         ModbusRequest.__init__(self, slave, **kwargs)
@@ -72,15 +71,15 @@
     """Base class for Messages responding to bit-reading values.
 
     The requested bits can be found in the .bits list.
     """
 
     _rtu_byte_count_pos = 2
 
-    def __init__(self, values, slave=Defaults.Slave, **kwargs):
+    def __init__(self, values, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param values: The requested values to be returned
         :param slave: Modbus slave slave ID
         """
         ModbusResponse.__init__(self, slave, **kwargs)
 
@@ -143,15 +142,15 @@
     coils. In the PDU Coils are addressed starting at zero. Therefore coils
     numbered 1-16 are addressed as 0-15.
     """
 
     function_code = 1
     function_code_name = "read_coils"
 
-    def __init__(self, address=None, count=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address=None, count=None, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param address: The address to start reading from
         :param count: The number of bits to read
         :param slave: Modbus slave slave ID
         """
         ReadBitsRequestBase.__init__(self, address, count, slave, **kwargs)
@@ -190,15 +189,15 @@
     the quantity of complete bytes of data.
 
     The requested coils can be found in boolean form in the .bits list.
     """
 
     function_code = 1
 
-    def __init__(self, values=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, values=None, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param values: The request values to respond with
         :param slave: Modbus slave slave ID
         """
         ReadBitsResponseBase.__init__(self, values, slave, **kwargs)
 
@@ -211,15 +210,15 @@
     number of inputs. In the PDU Discrete Inputs are addressed starting at
     zero. Therefore Discrete inputs numbered 1-16 are addressed as 0-15.
     """
 
     function_code = 2
     function_code_name = "read_discrete_input"
 
-    def __init__(self, address=None, count=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address=None, count=None, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param address: The address to start reading from
         :param count: The number of bits to read
         :param slave: Modbus slave slave ID
         """
         ReadBitsRequestBase.__init__(self, address, count, slave, **kwargs)
@@ -258,14 +257,14 @@
     the quantity of complete bytes of data.
 
     The requested coils can be found in boolean form in the .bits list.
     """
 
     function_code = 2
 
-    def __init__(self, values=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, values=None, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param values: The request values to respond with
         :param slave: Modbus slave slave ID
         """
         ReadBitsResponseBase.__init__(self, values, slave, **kwargs)
```

### Comparing `pymodbus-3.3.2/pymodbus/bit_write_message.py` & `pymodbus-3.4.0/pymodbus/bit_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/client/__init__.py` & `pymodbus-3.4.0/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/client/base.py` & `pymodbus-3.4.0/pymodbus/client/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 
 import asyncio
 import socket
 from dataclasses import dataclass
 from typing import Any, Callable
 
 from pymodbus.client.mixin import ModbusClientMixin
-from pymodbus.constants import Defaults
-from pymodbus.exceptions import ConnectionException
+from pymodbus.exceptions import ConnectionException, ModbusIOException
 from pymodbus.factory import ClientDecoder
 from pymodbus.framer import ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.transaction import DictTransactionManager
-from pymodbus.transport.transport import Transport
+from pymodbus.transport.transport import CommParams, ModbusProtocol
 from pymodbus.utilities import ModbusTransactionState
 
 
-class ModbusBaseClient(ModbusClientMixin, Transport):
+class ModbusBaseClient(ModbusClientMixin, ModbusProtocol):
     """**ModbusBaseClient**
 
     **Parameters common to all clients**:
 
     :param framer: (optional) Modbus Framer class.
     :param timeout: (optional) Timeout for a request, in seconds.
     :param retries: (optional) Max number of retries per request.
@@ -46,117 +45,122 @@
 
     :mod:`ModbusBaseClient` is normally not referenced outside :mod:`pymodbus`.
 
     **Application methods, common to all clients**:
     """
 
     @dataclass
-    class _params:  # pylint: disable=too-many-instance-attributes
+    class _params:
         """Parameter class."""
 
-        host: str = None
-        port: str | int = None
-        framer: type[ModbusFramer] = None
-        timeout: float = None
         retries: int = None
         retry_on_empty: bool = None
         close_comm_on_error: bool = None
         strict: bool = None
         broadcast_enable: bool = None
-        kwargs: dict = None
         reconnect_delay: int = None
 
-        baudrate: int = None
-        bytesize: int = None
-        parity: str = None
-        stopbits: int = None
-        handle_local_echo: bool = None
-
         source_address: tuple[str, int] = None
 
-        sslctx: str = None
-        certfile: str = None
-        keyfile: str = None
-        password: str = None
         server_hostname: str = None
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         framer: type[ModbusFramer] = None,
-        timeout: str | float = Defaults.Timeout,
-        retries: str | int = Defaults.Retries,
-        retry_on_empty: bool = Defaults.RetryOnEmpty,
-        close_comm_on_error: bool = Defaults.CloseCommOnError,
-        strict: bool = Defaults.Strict,
-        broadcast_enable: bool = Defaults.BroadcastEnable,
-        reconnect_delay: int = 0.1,
-        reconnect_delay_max: int = 300,
+        timeout: float = 3,
+        retries: int = 3,
+        retry_on_empty: bool = False,
+        close_comm_on_error: bool = False,
+        strict: bool = True,
+        broadcast_enable: bool = False,
+        reconnect_delay: float = 0.1,
+        reconnect_delay_max: float = 300,
         on_reconnect_callback: Callable[[], None] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize a client instance."""
-        Transport.__init__(
-            self,
-            "comm",
-            reconnect_delay * 1000,
-            reconnect_delay_max * 1000,
-            timeout * 1000,
-            lambda: None,
-            self.cb_base_connection_lost,
-            self.cb_base_handle_data,
+        ModbusClientMixin.__init__(self)
+        self.use_sync = kwargs.get("use_sync", False)
+        setup_params = CommParams(
+            comm_type=kwargs.get("CommType"),
+            comm_name="comm",
+            source_address=kwargs.get("source_address", ("127.0.0.1", 0)),
+            reconnect_delay=reconnect_delay,
+            reconnect_delay_max=reconnect_delay_max,
+            timeout_connect=timeout,
+            host=kwargs.get("host", None),
+            port=kwargs.get("port", None),
+            sslctx=kwargs.get("sslctx", None),
+            baudrate=kwargs.get("baudrate", None),
+            bytesize=kwargs.get("bytesize", None),
+            parity=kwargs.get("parity", None),
+            stopbits=kwargs.get("stopbits", None),
+            handle_local_echo=kwargs.get("handle_local_echo", False),
         )
-        self.framer = framer
+        if not self.use_sync:
+            ModbusProtocol.__init__(
+                self,
+                setup_params,
+                False,
+            )
+        else:
+            self.comm_params = setup_params
         self.params = self._params()
-        self.params.framer = framer
-        self.params.timeout = float(timeout)
         self.params.retries = int(retries)
         self.params.retry_on_empty = bool(retry_on_empty)
         self.params.close_comm_on_error = bool(close_comm_on_error)
         self.params.strict = bool(strict)
         self.params.broadcast_enable = bool(broadcast_enable)
         self.params.reconnect_delay = int(reconnect_delay)
         self.reconnect_delay_max = int(reconnect_delay_max)
         self.on_reconnect_callback = on_reconnect_callback
-        self.params.kwargs = kwargs
         self.retry_on_empty: int = 0
         # -> retry read on nothing
 
         self.slaves: list[int] = []
         # -> list of acceptable slaves (0 for accept all)
 
         # Common variables.
-        self.framer = self.params.framer(ClientDecoder(), self)
+        self.framer = framer(ClientDecoder(), self)
         self.transaction = DictTransactionManager(
             self, retries=retries, retry_on_empty=retry_on_empty, **kwargs
         )
         self.reconnect_delay = self.params.reconnect_delay
         self.reconnect_delay_current = self.params.reconnect_delay
-        self.use_sync = False
         self.use_udp = False
         self.state = ModbusTransactionState.IDLE
         self.last_frame_end: float = 0
         self.silent_interval: float = 0
 
-        # Initialize  mixin
-        ModbusClientMixin.__init__(self)
-
     # ----------------------------------------------------------------------- #
     # Client external interface
     # ----------------------------------------------------------------------- #
+    @property
+    def connected(self):
+        """Connect internal."""
+        return True
+
     def register(self, custom_response_class: ModbusResponse) -> None:
         """Register a custom response class with the decoder (call **sync**).
 
         :param custom_response_class: (optional) Modbus response class.
         :raises MessageRegisterException: Check exception text.
 
         Use register() to add non-standard responses (like e.g. a login prompt) and
         have them interpreted automatically.
         """
         self.framer.decoder.register(custom_response_class)
 
+    def close(self, reconnect=False) -> None:
+        """Close connection."""
+        if reconnect:
+            self.connection_lost(asyncio.TimeoutError("Server not responding"))
+        else:
+            self.transport_close()
+
     def idle_time(self) -> float:
         """Time before initiating next transaction (call **sync**).
 
         Applications can call message functions without checking idle_time(),
         this is done automatically.
         """
         if self.last_frame_end is None or self.silent_interval is None:
@@ -167,54 +171,59 @@
         """Execute request and get response (call **sync/async**).
 
         :param request: The request to process
         :returns: The result of the request execution
         :raises ConnectionException: Check exception text.
         """
         if self.use_sync:
-            if not self.connect():
+            if not self.connected:
                 raise ConnectionException(f"Failed to connect[{str(self)}]")
             return self.transaction.execute(request)
         if not self.transport:
             raise ConnectionException(f"Not connected[{str(self)}]")
         return self.async_execute(request)
 
     # ----------------------------------------------------------------------- #
     # Merged client methods
     # ----------------------------------------------------------------------- #
     async def async_execute(self, request=None):
         """Execute requests asynchronously."""
         request.transaction_id = self.transaction.getNextTID()
         packet = self.framer.buildPacket(request)
-        Log.debug("send: {}", packet, ":hex")
-        if self.use_udp:
-            self.transport.sendto(packet)
-        else:
-            self.transport.write(packet)
+        self.transport_send(packet)
         req = self._build_response(request.transaction_id)
         if self.params.broadcast_enable and not request.slave_id:
             resp = b"Broadcast write sent - no response expected"
         else:
-            try:
-                resp = await asyncio.wait_for(req, timeout=self.params.timeout)
-            except asyncio.exceptions.TimeoutError:
+            count = 0
+            while count < self.params.retries:
+                count += 1
+                try:
+                    resp = await asyncio.wait_for(
+                        req, timeout=self.comm_params.timeout_connect
+                    )
+                    break
+                except asyncio.exceptions.TimeoutError:
+                    pass
+            if count == self.params.retries:
                 self.close(reconnect=True)
-                raise
+                raise ModbusIOException(
+                    f"ERROR: No response received after {self.params.retries} retries"
+                )
         return resp
 
-    def cb_base_handle_data(self, data: bytes) -> int:
+    def callback_data(self, data: bytes, addr: tuple = None) -> int:
         """Handle received data
 
         returns number of bytes consumed
         """
-        Log.debug("recv: {}", data, ":hex")
         self.framer.processIncomingPacket(data, self._handle_response, slave=0)
         return len(data)
 
-    def cb_base_connection_lost(self, _reason: Exception) -> None:
+    def callback_disconnected(self, _reason: Exception) -> None:
         """Handle lost connection"""
         for tid in list(self.transaction):
             self.raise_future(
                 self.transaction.getTransaction(tid),
                 ConnectionException("Connection lost during request"),
             )
 
@@ -244,15 +253,15 @@
         else:
             self.transaction.addTransaction(my_future, tid)
         return my_future
 
     # ----------------------------------------------------------------------- #
     # Internal methods
     # ----------------------------------------------------------------------- #
-    def send(self, request):  # pylint: disable=invalid-overridden-method
+    def send(self, request):
         """Send request.
 
         :meta private:
         """
         if self.state != ModbusTransactionState.RETRYING:
             Log.debug('New Transaction state "SENDING"')
             self.state = ModbusTransactionState.SENDING
@@ -307,8 +316,10 @@
         self.close()
 
     def __str__(self):
         """Build a string representation of the connection.
 
         :returns: The string representation
         """
-        return f"{self.__class__.__name__} {self.params.host}:{self.params.port}"
+        return (
+            f"{self.__class__.__name__} {self.comm_params.host}:{self.comm_params.port}"
+        )
```

### Comparing `pymodbus-3.3.2/pymodbus/client/mixin.py` & `pymodbus-3.4.0/pymodbus/client/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,196 +163,208 @@
         """Diagnose query data (code 0x08 sub 0x00).
 
         :param msg: Message to be returned
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnQueryDataRequest(msg, slave, **kwargs))
+        return self.execute(pdu_diag.ReturnQueryDataRequest(msg, slave=slave, **kwargs))
 
     def diag_restart_communication(
         self, toggle: bool, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose restart communication (code 0x08 sub 0x01).
 
         :param toggle: True if toogled.
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
         return self.execute(
-            pdu_diag.RestartCommunicationsOptionRequest(toggle, slave, **kwargs)
+            pdu_diag.RestartCommunicationsOptionRequest(toggle, slave=slave, **kwargs)
         )
 
     def diag_read_diagnostic_register(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read diagnostic register (code 0x08 sub 0x02).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnDiagnosticRegisterRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ReturnDiagnosticRegisterRequest(slave=slave, **kwargs)
+        )
 
     def diag_change_ascii_input_delimeter(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose change ASCII input delimiter (code 0x08 sub 0x03).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ChangeAsciiInputDelimiterRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ChangeAsciiInputDelimiterRequest(slave=slave, **kwargs)
+        )
 
     def diag_force_listen_only(self, slave: int = 0, **kwargs: Any) -> ModbusResponse:
         """Diagnose force listen only (code 0x08 sub 0x04).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ForceListenOnlyModeRequest(slave, **kwargs))
+        return self.execute(pdu_diag.ForceListenOnlyModeRequest(slave=slave, **kwargs))
 
     def diag_clear_counters(self, slave: int = 0, **kwargs: Any) -> ModbusResponse:
         """Diagnose clear counters (code 0x08 sub 0x0A).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ClearCountersRequest(slave, **kwargs))
+        return self.execute(pdu_diag.ClearCountersRequest(slave=slave, **kwargs))
 
     def diag_read_bus_message_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read bus message count (code 0x08 sub 0x0B).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnBusMessageCountRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ReturnBusMessageCountRequest(slave=slave, **kwargs)
+        )
 
     def diag_read_bus_comm_error_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Bus Communication Error Count (code 0x08 sub 0x0C).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
         return self.execute(
-            pdu_diag.ReturnBusCommunicationErrorCountRequest(slave, **kwargs)
+            pdu_diag.ReturnBusCommunicationErrorCountRequest(slave=slave, **kwargs)
         )
 
     def diag_read_bus_exception_error_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Bus Exception Error Count (code 0x08 sub 0x0D).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
         return self.execute(
-            pdu_diag.ReturnBusExceptionErrorCountRequest(slave, **kwargs)
+            pdu_diag.ReturnBusExceptionErrorCountRequest(slave=slave, **kwargs)
         )
 
     def diag_read_slave_message_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Slave Message Count (code 0x08 sub 0x0E).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnSlaveMessageCountRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ReturnSlaveMessageCountRequest(slave=slave, **kwargs)
+        )
 
     def diag_read_slave_no_response_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Slave No Response Count (code 0x08 sub 0x0F).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnSlaveNoResponseCountRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ReturnSlaveNoResponseCountRequest(slave=slave, **kwargs)
+        )
 
     def diag_read_slave_nak_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Slave NAK Count (code 0x08 sub 0x10).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnSlaveNAKCountRequest(slave, **kwargs))
+        return self.execute(pdu_diag.ReturnSlaveNAKCountRequest(slave=slave, **kwargs))
 
     def diag_read_slave_busy_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Slave Busy Count (code 0x08 sub 0x11).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnSlaveBusyCountRequest(slave, **kwargs))
+        return self.execute(pdu_diag.ReturnSlaveBusyCountRequest(slave=slave, **kwargs))
 
     def diag_read_bus_char_overrun_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Bus Character Overrun Count (code 0x08 sub 0x12).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
         return self.execute(
-            pdu_diag.ReturnSlaveBusCharacterOverrunCountRequest(slave, **kwargs)
+            pdu_diag.ReturnSlaveBusCharacterOverrunCountRequest(slave=slave, **kwargs)
         )
 
     def diag_read_iop_overrun_count(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose read Iop overrun count (code 0x08 sub 0x13).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ReturnIopOverrunCountRequest(slave, **kwargs))
+        return self.execute(
+            pdu_diag.ReturnIopOverrunCountRequest(slave=slave, **kwargs)
+        )
 
     def diag_clear_overrun_counter(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose Clear Overrun Counter and Flag (code 0x08 sub 0x14).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.ClearOverrunCountRequest(slave, **kwargs))
+        return self.execute(pdu_diag.ClearOverrunCountRequest(slave=slave, **kwargs))
 
     def diag_getclear_modbus_response(
         self, slave: int = 0, **kwargs: Any
     ) -> ModbusResponse:
         """Diagnose Get/Clear modbus plus (code 0x08 sub 0x15).
 
         :param slave: (optional) Modbus slave ID
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
-        return self.execute(pdu_diag.GetClearModbusPlusRequest(slave, **kwargs))
+        return self.execute(pdu_diag.GetClearModbusPlusRequest(slave=slave, **kwargs))
 
     def diag_get_comm_event_counter(self, **kwargs: Any) -> ModbusResponse:
         """Diagnose get event counter (code 0x0B).
 
         :param kwargs: (optional) Experimental parameters.
         :raises ModbusException:
         """
```

### Comparing `pymodbus-3.3.2/pymodbus/client/serial.py` & `pymodbus-3.4.0/pymodbus/client/tcp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,289 +1,278 @@
-"""Modbus client async serial communication."""
+"""Modbus client async TCP communication."""
 import asyncio
+import select
+import socket
 import time
-from contextlib import suppress
-from functools import partial
-from typing import Any, Type
+from typing import Any, Tuple, Type
 
 from pymodbus.client.base import ModbusBaseClient
-from pymodbus.constants import Defaults
 from pymodbus.exceptions import ConnectionException
 from pymodbus.framer import ModbusFramer
-from pymodbus.framer.rtu_framer import ModbusRtuFramer
+from pymodbus.framer.socket_framer import ModbusSocketFramer
 from pymodbus.logging import Log
+from pymodbus.transport.transport import CommType
 from pymodbus.utilities import ModbusTransactionState
 
 
-with suppress(ImportError):
-    import serial
+class AsyncModbusTcpClient(ModbusBaseClient, asyncio.Protocol):
+    """**AsyncModbusTcpClient**.
 
-
-class AsyncModbusSerialClient(ModbusBaseClient, asyncio.Protocol):
-    """**AsyncModbusSerialClient**.
-
-    :param port: Serial port used for communication.
-    :param framer: (optional) Framer class.
-    :param baudrate: (optional) Bits per second.
-    :param bytesize: (optional) Number of bits per byte 7-8.
-    :param parity: (optional) 'E'ven, 'O'dd or 'N'one
-    :param stopbits: (optional) Number of stop bits 0-2¡.
-    :param handle_local_echo: (optional) Discard local echo from dongle.
+    :param host: Host IP address or host name
+    :param port: (optional) Port used for communication
+    :param framer: (optional) Framer class
+    :param source_address: (optional) source address of client
     :param kwargs: (optional) Experimental parameters
 
-    The serial communication is RS-485 based, and usually used with a usb RS485 dongle.
-
     Example::
 
-        from pymodbus.client import AsyncModbusSerialClient
+        from pymodbus.client import AsyncModbusTcpClient
 
         async def run():
-            client = AsyncModbusSerialClient("dev/serial0")
+            client = AsyncModbusTcpClient("localhost")
 
             await client.connect()
             ...
             client.close()
     """
 
-    transport = None
-    framer = None
-
     def __init__(
         self,
-        port: str,
-        framer: Type[ModbusFramer] = ModbusRtuFramer,
-        baudrate: int = Defaults.Baudrate,
-        bytesize: int = Defaults.Bytesize,
-        parity: str = Defaults.Parity,
-        stopbits: int = Defaults.Stopbits,
-        handle_local_echo: bool = Defaults.HandleLocalEcho,
+        host: str,
+        port: int = 502,
+        framer: Type[ModbusFramer] = ModbusSocketFramer,
+        source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize Asyncio Modbus Serial Client."""
+        """Initialize Asyncio Modbus TCP Client."""
         asyncio.Protocol.__init__(self)
-        ModbusBaseClient.__init__(self, framer=framer, **kwargs)
-        self.params.port = port
-        self.params.baudrate = baudrate
-        self.params.bytesize = bytesize
-        self.params.parity = parity
-        self.params.stopbits = stopbits
-        self.params.handle_local_echo = handle_local_echo
-        self.setup_serial(False, port, baudrate, bytesize, parity, stopbits)
+        if "CommType" not in kwargs:
+            kwargs["CommType"] = CommType.TCP
+        ModbusBaseClient.__init__(
+            self,
+            framer=framer,
+            host=host,
+            port=port,
+            **kwargs,
+        )
+        self.params.source_address = source_address
 
-    @property
-    def connected(self):
-        """Connect internal."""
-        return self.transport is not None
+    async def connect(self) -> bool:
+        """Initiate connection to start client."""
 
-    async def connect(self):
-        """Connect Async client."""
         # if reconnect_delay_current was set to 0 by close(), we need to set it back again
         # so this instance will work
         self.reset_delay()
 
         # force reconnect if required:
-        Log.debug("Connecting to {}.", self.params.host)
+        Log.debug(
+            "Connecting to {}:{}.",
+            self.comm_params.host,
+            self.comm_params.port,
+        )
         return await self.transport_connect()
 
+    @property
+    def connected(self):
+        """Return true if connected."""
+        return self.is_active()
 
-class ModbusSerialClient(ModbusBaseClient):
-    """**ModbusSerialClient**.
 
-    :param port: Serial port used for communication.
-    :param framer: (optional) Framer class.
-    :param baudrate: (optional) Bits per second.
-    :param bytesize: (optional) Number of bits per byte 7-8.
-    :param parity: (optional) 'E'ven, 'O'dd or 'N'one
-    :param stopbits: (optional) Number of stop bits 0-2¡.
-    :param handle_local_echo: (optional) Discard local echo from dongle.
-    :param kwargs: (optional) Experimental parameters
+class ModbusTcpClient(ModbusBaseClient):
+    """**ModbusTcpClient**.
 
-    The serial communication is RS-485 based, and usually used with a usb RS485 dongle.
+    :param host: Host IP address or host name
+    :param port: (optional) Port used for communication
+    :param framer: (optional) Framer class
+    :param source_address: (optional) source address of client
+    :param kwargs: (optional) Experimental parameters
 
     Example::
 
-        from pymodbus.client import ModbusSerialClient
+        from pymodbus.client import ModbusTcpClient
 
-        def run():
-            client = ModbusSerialClient("dev/serial0")
+        async def run():
+            client = ModbusTcpClient("localhost")
 
             client.connect()
             ...
             client.close()
 
-
-    Remark: There are no automatic reconnect as with AsyncModbusSerialClient
+    Remark: There are no automatic reconnect as with AsyncModbusTcpClient
     """
 
-    state = ModbusTransactionState.IDLE
-    inter_char_timeout: float = 0
-    silent_interval: float = 0
-
     def __init__(
         self,
-        port: str,
-        framer: Type[ModbusFramer] = ModbusRtuFramer,
-        baudrate: int = Defaults.Baudrate,
-        bytesize: int = Defaults.Bytesize,
-        parity: str = Defaults.Parity,
-        stopbits: int = Defaults.Stopbits,
-        handle_local_echo: bool = Defaults.HandleLocalEcho,
+        host: str,
+        port: int = 502,
+        framer: Type[ModbusFramer] = ModbusSocketFramer,
+        source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize Modbus Serial Client."""
-        super().__init__(framer=framer, **kwargs)
-        self.params.port = port
-        self.params.baudrate = baudrate
-        self.params.bytesize = bytesize
-        self.params.parity = parity
-        self.params.stopbits = stopbits
-        self.params.handle_local_echo = handle_local_echo
+        """Initialize Modbus TCP Client."""
+        if "CommType" not in kwargs:
+            kwargs["CommType"] = CommType.TCP
+        kwargs["use_sync"] = True
+        self.transport = None
+        super().__init__(framer=framer, host=host, port=port, **kwargs)
+        self.params.source_address = source_address
         self.socket = None
-        self.use_sync = True
-
-        self.last_frame_end = None
-
-        self._t0 = float(1 + 8 + 2) / self.params.baudrate
-
-        """
-        The minimum delay is 0.01s and the maximum can be set to 0.05s.
-        Setting too large a setting affects efficiency.
-        """
-        self._recv_interval = (
-            (round((100 * self._t0), 2) + 0.01)
-            if (round((100 * self._t0), 2) + 0.01) < 0.05
-            else 0.05
-        )
-
-        if self.params.baudrate > 19200:
-            self.silent_interval = 1.75 / 1000  # ms
-        else:
-            self.inter_char_timeout = 1.5 * self._t0
-            self.silent_interval = 3.5 * self._t0
-        self.silent_interval = round(self.silent_interval, 6)
 
     @property
     def connected(self):
         """Connect internal."""
-        return self.connect()
+        return self.socket is not None
 
     def connect(self):  # pylint: disable=invalid-overridden-method
-        """Connect to the modbus serial server."""
+        """Connect to the modbus tcp server."""
         if self.socket:
             return True
         try:
-            self.socket = serial.serial_for_url(
-                self.params.port,
-                timeout=self.params.timeout,
-                bytesize=self.params.bytesize,
-                stopbits=self.params.stopbits,
-                baudrate=self.params.baudrate,
-                parity=self.params.parity,
+            self.socket = socket.create_connection(
+                (self.comm_params.host, self.comm_params.port),
+                timeout=self.comm_params.timeout_connect,
+                source_address=self.params.source_address,
+            )
+            Log.debug(
+                "Connection to Modbus server established. Socket {}",
+                self.socket.getsockname(),
+            )
+        except OSError as msg:
+            Log.error(
+                "Connection to ({}, {}) failed: {}",
+                self.comm_params.host,
+                self.comm_params.port,
+                msg,
             )
-            if isinstance(self.framer, ModbusRtuFramer):
-                if self.params.strict:
-                    self.socket.interCharTimeout = self.inter_char_timeout
-                self.last_frame_end = None
-        except serial.SerialException as msg:
-            Log.error("{}", msg)
             self.close()
         return self.socket is not None
 
     def close(self):  # pylint: disable=arguments-differ
         """Close the underlying socket connection."""
         if self.socket:
             self.socket.close()
         self.socket = None
 
-    def _in_waiting(self):
-        """Return _in_waiting."""
-        in_waiting = "in_waiting" if hasattr(self.socket, "in_waiting") else "inWaiting"
-
-        if in_waiting == "in_waiting":
-            waitingbytes = getattr(self.socket, in_waiting)
-        else:
-            waitingbytes = getattr(self.socket, in_waiting)()
-        return waitingbytes
+    def _check_read_buffer(self):
+        """Check read buffer."""
+        time_ = time.time()
+        end = time_ + self.comm_params.timeout_connect
+        data = None
+        ready = select.select([self.socket], [], [], end - time_)
+        if ready[0]:
+            data = self.socket.recv(1024)
+        return data
 
     def send(self, request):
-        """Send data on the underlying socket.
-
-        If receive buffer still holds some data then flush it.
-
-        Sleep if last send finished less than 3.5 character times ago.
-        """
+        """Send data on the underlying socket."""
         super().send(request)
         if not self.socket:
             raise ConnectionException(str(self))
+        if self.state == ModbusTransactionState.RETRYING:
+            if data := self._check_read_buffer():
+                return data
+
         if request:
-            try:
-                if waitingbytes := self._in_waiting():
-                    result = self.socket.read(waitingbytes)
-                    if self.state == ModbusTransactionState.RETRYING:
-                        Log.debug(
-                            "Sending available data in recv buffer {}", result, ":hex"
-                        )
-                        return result
-                    Log.warning("Cleanup recv buffer before send: {}", result, ":hex")
-            except NotImplementedError:
-                pass
-            if self.state != ModbusTransactionState.SENDING:
-                Log.debug('New Transaction state "SENDING"')
-                self.state = ModbusTransactionState.SENDING
-            size = self.socket.write(request)
-            return size
+            return self.socket.send(request)
         return 0
 
-    def _wait_for_data(self):
-        """Wait for data."""
-        size = 0
-        more_data = False
-        if self.params.timeout is not None and self.params.timeout:
-            condition = partial(
-                lambda start, timeout: (time.time() - start) <= timeout,
-                timeout=self.params.timeout,
-            )
-        else:
-            condition = partial(lambda dummy1, dummy2: True, dummy2=None)
-        start = time.time()
-        while condition(start):
-            available = self._in_waiting()
-            if (more_data and not available) or (more_data and available == size):
-                break
-            if available and available != size:
-                more_data = True
-                size = available
-            time.sleep(self._recv_interval)
-        return size
-
     def recv(self, size):
         """Read data from the underlying descriptor."""
         super().recv(size)
         if not self.socket:
-            raise ConnectionException(
-                self.__str__()  # pylint: disable=unnecessary-dunder-call
-            )
+            raise ConnectionException(str(self))
+
+        # socket.recv(size) waits until it gets some data from the host but
+        # not necessarily the entire response that can be fragmented in
+        # many packets.
+        # To avoid split responses to be recognized as invalid
+        # messages and to be discarded, loops socket.recv until full data
+        # is received or timeout is expired.
+        # If timeout expires returns the read data, also if its length is
+        # less than the expected size.
+        self.socket.setblocking(0)
+
+        timeout = self.comm_params.timeout_connect
+
+        # If size isn't specified read up to 4096 bytes at a time.
         if size is None:
-            size = self._wait_for_data()
-        if size > self._in_waiting():
-            self._wait_for_data()
-        result = self.socket.read(size)
-        return result
+            recv_size = 4096
+        else:
+            recv_size = size
+
+        data = []
+        data_length = 0
+        time_ = time.time()
+        end = time_ + timeout
+        while recv_size > 0:
+            try:
+                ready = select.select([self.socket], [], [], end - time_)
+            except ValueError:
+                return self._handle_abrupt_socket_close(size, data, time.time() - time_)
+            if ready[0]:
+                if (recv_data := self.socket.recv(recv_size)) == b"":
+                    return self._handle_abrupt_socket_close(
+                        size, data, time.time() - time_
+                    )
+                data.append(recv_data)
+                data_length += len(recv_data)
+            time_ = time.time()
+
+            # If size isn't specified continue to read until timeout expires.
+            if size:
+                recv_size = size - data_length
+
+            # Timeout is reduced also if some data has been received in order
+            # to avoid infinite loops when there isn't an expected response
+            # size and the slave sends noisy data continuously.
+            if time_ > end:
+                break
+
+        return b"".join(data)
+
+    def _handle_abrupt_socket_close(self, size, data, duration):
+        """Handle unexpected socket close by remote end.
+
+        Intended to be invoked after determining that the remote end
+        has unexpectedly closed the connection, to clean up and handle
+        the situation appropriately.
+
+        :param size: The number of bytes that was attempted to read
+        :param data: The actual data returned
+        :param duration: Duration from the read was first attempted
+               until it was determined that the remote closed the
+               socket
+        :return: The more than zero bytes read from the remote end
+        :raises ConnectionException: If the remote end didn't send any
+                 data at all before closing the connection.
+        """
+        self.close()
+        size_txt = size if size else "unbounded read"
+        readsize = f"read of {size_txt} bytes"
+        msg = (
+            f"{self}: Connection unexpectedly closed "
+            f"{duration} seconds into {readsize}"
+        )
+        if data:
+            result = b"".join(data)
+            Log.warning(" after returning {} bytes: {} ", len(result), result)
+            return result
+        msg += " without response from slave before it closed connection"
+        raise ConnectionException(msg)
 
     def is_socket_open(self):
         """Check if socket is open."""
-        if self.socket:
-            if hasattr(self.socket, "is_open"):
-                return self.socket.is_open
-            return self.socket.isOpen()
-        return False
+        return self.socket is not None
 
     def __str__(self):
-        """Build a string representation of the connection."""
-        return f"ModbusSerialClient({self.framer} baud[{self.params.baudrate}])"
+        """Build a string representation of the connection.
+
+        :returns: The string representation
+        """
+        return f"ModbusTcpClient({self.comm_params.host}:{self.comm_params.port})"
 
     def __repr__(self):
         """Return string representation."""
         return (
             f"<{self.__class__.__name__} at {hex(id(self))} socket={self.socket}, "
-            f"framer={self.framer}, timeout={self.params.timeout}>"
+            f"ipaddr={self.comm_params.host}, port={self.comm_params.port}, timeout={self.comm_params.timeout_connect}>"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymodbus-3.3.2/pymodbus/client/tls.py` & `pymodbus-3.4.0/pymodbus/client/tls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,17 @@
 """Modbus client async TLS communication."""
 import socket
 import ssl
 from typing import Any, Type
 
 from pymodbus.client.tcp import AsyncModbusTcpClient, ModbusTcpClient
-from pymodbus.constants import Defaults
 from pymodbus.framer import ModbusFramer
 from pymodbus.framer.tls_framer import ModbusTlsFramer
 from pymodbus.logging import Log
-
-
-def sslctx_provider(
-    sslctx=None, certfile=None, keyfile=None, password=None
-):  # pylint: disable=missing-type-doc
-    """Provide the SSLContext for ModbusTlsClient.
-
-    If the user defined SSLContext is not passed in, sslctx_provider will
-    produce a default one.
-
-    :param sslctx: The user defined SSLContext to use for TLS (default None and
-                   auto create)
-    :param certfile: The optional client's cert file path for TLS server request
-    :param keyfile: The optional client's key file path for TLS server request
-    :param password: The password for decrypting client's private key file
-    """
-    if sslctx:
-        return sslctx
-
-    sslctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-    sslctx.check_hostname = False
-    sslctx.verify_mode = ssl.CERT_NONE
-    sslctx.options |= ssl.OP_NO_TLSv1_1
-    sslctx.options |= ssl.OP_NO_TLSv1
-    sslctx.options |= ssl.OP_NO_SSLv3
-    sslctx.options |= ssl.OP_NO_SSLv2
-    if certfile and keyfile:
-        sslctx.load_cert_chain(certfile=certfile, keyfile=keyfile, password=password)
-    return sslctx
+from pymodbus.transport.transport import CommParams, CommType
 
 
 class AsyncModbusTlsClient(AsyncModbusTcpClient):
     """**AsyncModbusTlsClient**.
 
     :param host: Host IP address or host name
     :param port: (optional) Port used for communication
@@ -67,45 +38,50 @@
             ...
             client.close()
     """
 
     def __init__(
         self,
         host: str,
-        port: int = Defaults.TlsPort,
+        port: int = 802,
         framer: Type[ModbusFramer] = ModbusTlsFramer,
         sslctx: ssl.SSLContext = None,
         certfile: str = None,
         keyfile: str = None,
         password: str = None,
         server_hostname: str = None,
         **kwargs: Any,
     ):
         """Initialize Asyncio Modbus TLS Client."""
         AsyncModbusTcpClient.__init__(
-            self, host, port=port, framer=framer, internal_no_setup=True, **kwargs
+            self,
+            host,
+            port=port,
+            framer=framer,
+            CommType=CommType.TLS,
+            sslctx=CommParams.generate_ssl(
+                False, certfile, keyfile, password, sslctx=sslctx
+            ),
+            **kwargs,
         )
-        self.sslctx = sslctx_provider(sslctx, certfile, keyfile, password)
-        self.params.certfile = certfile
-        self.params.keyfile = keyfile
-        self.params.password = password
         self.params.server_hostname = server_hostname
-        self.setup_tls(
-            False, host, port, sslctx, certfile, keyfile, password, server_hostname
-        )
 
-    async def connect(self):
+    async def connect(self) -> bool:
         """Initiate connection to start client."""
 
         # if reconnect_delay_current was set to 0 by close(), we need to set it back again
         # so this instance will work
         self.reset_delay()
 
         # force reconnect if required:
-        Log.debug("Connecting to {}:{}.", self.params.host, self.params.port)
+        Log.debug(
+            "Connecting to {}:{}.",
+            self.comm_params.host,
+            self.comm_params.port,
+        )
         return await self.transport_connect()
 
 
 class ModbusTlsClient(ModbusTcpClient):
     """**ModbusTlsClient**.
 
     :param host: Host IP address or host name
@@ -136,30 +112,31 @@
 
     Remark: There are no automatic reconnect as with AsyncModbusTlsClient
     """
 
     def __init__(
         self,
         host: str,
-        port: int = Defaults.TlsPort,
+        port: int = 802,
         framer: Type[ModbusFramer] = ModbusTlsFramer,
-        sslctx: str = None,
+        sslctx: ssl.SSLContext = None,
         certfile: str = None,
         keyfile: str = None,
         password: str = None,
         server_hostname: str = None,
         **kwargs: Any,
     ):
         """Initialize Modbus TLS Client."""
-        super().__init__(host, port=port, framer=framer, **kwargs)
-        self.sslctx = sslctx_provider(sslctx, certfile, keyfile, password)
-        self.params.sslctx = sslctx
-        self.params.certfile = certfile
-        self.params.keyfile = keyfile
-        self.params.password = password
+        self.transport = None
+        super().__init__(
+            host, CommType=CommType.TLS, port=port, framer=framer, **kwargs
+        )
+        self.sslctx = CommParams.generate_ssl(
+            False, certfile, keyfile, password, sslctx=sslctx
+        )
         self.params.server_hostname = server_hostname
 
     @property
     def connected(self):
         """Connect internal."""
         return self.transport is not None
 
@@ -168,32 +145,32 @@
         if self.socket:
             return True
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             if self.params.source_address:
                 sock.bind(self.params.source_address)
             self.socket = self.sslctx.wrap_socket(
-                sock, server_side=False, server_hostname=self.params.host
+                sock, server_side=False, server_hostname=self.comm_params.host
             )
-            self.socket.settimeout(self.params.timeout)
-            self.socket.connect((self.params.host, self.params.port))
+            self.socket.settimeout(self.comm_params.timeout_connect)
+            self.socket.connect((self.comm_params.host, self.comm_params.port))
         except OSError as msg:
             Log.error(
                 "Connection to ({}, {}) failed: {}",
-                self.params.host,
-                self.params.port,
+                self.comm_params.host,
+                self.comm_params.port,
                 msg,
             )
             self.close()
         return self.socket is not None
 
     def __str__(self):
         """Build a string representation of the connection."""
-        return f"ModbusTlsClient({self.params.host}:{self.params.port})"
+        return f"ModbusTlsClient({self.comm_params.host}:{self.comm_params.port})"
 
     def __repr__(self):
         """Return string representation."""
         return (
             f"<{self.__class__.__name__} at {hex(id(self))} socket={self.socket}, "
-            f"ipaddr={self.params.host}, port={self.params.port}, sslctx={self.sslctx}, "
-            f"timeout={self.params.timeout}>"
+            f"ipaddr={self.comm_params.host}, port={self.comm_params.port}, sslctx={self.sslctx}, "
+            f"timeout={self.comm_params.timeout_connect}>"
         )
```

### Comparing `pymodbus-3.3.2/pymodbus/client/udp.py` & `pymodbus-3.4.0/pymodbus/client/udp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Modbus client async UDP communication."""
 import asyncio
 import socket
 from typing import Any, Tuple, Type
 
 from pymodbus.client.base import ModbusBaseClient
-from pymodbus.constants import Defaults
 from pymodbus.exceptions import ConnectionException
 from pymodbus.framer import ModbusFramer
 from pymodbus.framer.socket_framer import ModbusSocketFramer
 from pymodbus.logging import Log
+from pymodbus.transport.transport import CommType
 
 
 DGRAM_TYPE = socket.SOCK_DGRAM
 
 
 class AsyncModbusUdpClient(
     ModbusBaseClient, asyncio.Protocol, asyncio.DatagramProtocol
@@ -39,43 +39,47 @@
             ...
             client.close()
     """
 
     def __init__(
         self,
         host: str,
-        port: int = Defaults.UdpPort,
+        port: int = 502,
         framer: Type[ModbusFramer] = ModbusSocketFramer,
         source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize Asyncio Modbus UDP Client."""
         asyncio.DatagramProtocol.__init__(self)
         asyncio.Protocol.__init__(self)
-        ModbusBaseClient.__init__(self, framer=framer, **kwargs)
-        self.params.port = port
+        ModbusBaseClient.__init__(
+            self, framer=framer, CommType=CommType.UDP, host=host, port=port, **kwargs
+        )
         self.params.source_address = source_address
-        self.setup_udp(False, host, port)
 
     @property
     def connected(self):
         """Return true if connected."""
-        return self.transport is not None
+        return self.is_active()
 
-    async def connect(self):
+    async def connect(self) -> bool:
         """Start reconnecting asynchronous udp client.
 
         :meta private:
         """
         # if reconnect_delay_current was set to 0 by close(), we need to set it back again
         # so this instance will work
         self.reset_delay()
 
         # force reconnect if required:
-        Log.debug("Connecting to {}:{}.", self.comm_params.host, self.comm_params.port)
+        Log.debug(
+            "Connecting to {}:{}.",
+            self.comm_params.host,
+            self.comm_params.port,
+        )
         return await self.transport_connect()
 
 
 class ModbusUdpClient(ModbusBaseClient):
     """**ModbusUdpClient**.
 
     :param host: Host IP address or host name
@@ -100,39 +104,45 @@
 
     Remark: There are no automatic reconnect as with AsyncModbusUdpClient
     """
 
     def __init__(
         self,
         host: str,
-        port: int = Defaults.UdpPort,
+        port: int = 502,
         framer: Type[ModbusFramer] = ModbusSocketFramer,
         source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize Modbus UDP Client."""
-        super().__init__(framer=framer, **kwargs)
-        self.params.host = host
-        self.params.port = port
+        kwargs["use_sync"] = True
+        self.transport = None
+        super().__init__(
+            framer=framer, port=port, host=host, CommType=CommType.UDP, **kwargs
+        )
         self.params.source_address = source_address
 
         self.socket = None
-        self.use_sync = True
+
+    @property
+    def connected(self):
+        """Connect internal."""
+        return self.socket is not None
 
     def connect(self):  # pylint: disable=invalid-overridden-method
         """Connect to the modbus tcp server.
 
         :meta private:
         """
         if self.socket:
             return True
         try:
-            family = ModbusUdpClient._get_address_family(self.params.host)
+            family = ModbusUdpClient._get_address_family(self.comm_params.host)
             self.socket = socket.socket(family, socket.SOCK_DGRAM)
-            self.socket.settimeout(self.params.timeout)
+            self.socket.settimeout(self.comm_params.timeout_connect)
         except OSError as exc:
             Log.error("Unable to create udp socket {}", exc)
             self.close()
         return self.socket is not None
 
     def close(self):  # pylint: disable=arguments-differ
         """Close the underlying socket connection.
@@ -146,15 +156,17 @@
 
         :meta private:
         """
         super().send(request)
         if not self.socket:
             raise ConnectionException(str(self))
         if request:
-            return self.socket.sendto(request, (self.params.host, self.params.port))
+            return self.socket.sendto(
+                request, (self.comm_params.host, self.comm_params.port)
+            )
         return 0
 
     def recv(self, size):
         """Read data from the underlying descriptor.
 
         :meta private:
         """
@@ -168,15 +180,15 @@
 
         :meta private:
         """
         return True
 
     def __str__(self):
         """Build a string representation of the connection."""
-        return f"ModbusUdpClient({self.params.host}:{self.params.port})"
+        return f"ModbusUdpClient({self.comm_params.host}:{self.comm_params.port})"
 
     def __repr__(self):
         """Return string representation."""
         return (
             f"<{self.__class__.__name__} at {hex(id(self))} socket={self.socket}, "
-            f"ipaddr={self.params.host}, port={self.params.port}, timeout={self.params.timeout}>"
+            f"ipaddr={self.comm_params.host}, port={self.comm_params.port}, timeout={self.comm_params.timeout_connect}>"
         )
```

### Comparing `pymodbus-3.3.2/pymodbus/datastore/context.py` & `pymodbus-3.4.0/pymodbus/datastore/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Context for datastore."""
 # pylint: disable=missing-type-doc
-from pymodbus.constants import Defaults
 from pymodbus.datastore.store import ModbusSequentialDataBlock
 from pymodbus.exceptions import NoSuchSlaveException
 from pymodbus.logging import Log
 
 
 class ModbusBaseSlaveContext:  # pylint: disable=too-few-public-methods
     """Interface for a modbus slave data context.
@@ -34,30 +33,27 @@
 # ---------------------------------------------------------------------------#
 class ModbusSlaveContext(ModbusBaseSlaveContext):
     """This creates a modbus data model with each data access stored in a block."""
 
     def __init__(self, *_args, **kwargs):
         """Initialize the datastores.
 
-        Defaults to fully populated
-        sequential data blocks if none are passed in.
-
         :param kwargs: Each element is a ModbusDataBlock
 
             "di" - Discrete Inputs initializer
             "co" - Coils initializer
             "hr" - Holding Register initializer
             "ir" - Input Registers iniatializer
         """
         self.store = {}
         self.store["d"] = kwargs.get("di", ModbusSequentialDataBlock.create())
         self.store["c"] = kwargs.get("co", ModbusSequentialDataBlock.create())
         self.store["i"] = kwargs.get("ir", ModbusSequentialDataBlock.create())
         self.store["h"] = kwargs.get("hr", ModbusSequentialDataBlock.create())
-        self.zero_mode = kwargs.get("zero_mode", Defaults.ZeroMode)
+        self.zero_mode = kwargs.get("zero_mode", False)
 
     def __str__(self):
         """Return a string representation of the context.
 
         :returns: A string representation of the context
         """
         return "Modbus Slave Context"
@@ -130,15 +126,15 @@
 
         :param slaves: A dictionary of client contexts
         :param single: Set to true to treat this as a single context
         """
         self.single = single
         self._slaves = slaves or {}
         if self.single:
-            self._slaves = {Defaults.Slave: self._slaves}
+            self._slaves = {0: self._slaves}
 
     def __iter__(self):
         """Iterate over the current collection of slave contexts.
 
         :returns: An iterator over the slave contexts
         """
         return iter(self._slaves.items())
@@ -157,15 +153,15 @@
         """Use to set a new slave context.
 
         :param slave: The slave context to set
         :param context: The new context to set for this slave
         :raises NoSuchSlaveException:
         """
         if self.single:
-            slave = Defaults.Slave
+            slave = 0
         if 0xF7 >= slave >= 0x00:
             self._slaves[slave] = context
         else:
             raise NoSuchSlaveException(f"slave index :{slave} out of range")
 
     def __delitem__(self, slave):
         """Use to access the slave context.
@@ -182,15 +178,15 @@
         """Use to get access to a slave context.
 
         :param slave: The slave context to get
         :returns: The requested slave context
         :raises NoSuchSlaveException:
         """
         if self.single:
-            slave = Defaults.Slave
+            slave = 0
         if slave in self._slaves:
             return self._slaves.get(slave)
         raise NoSuchSlaveException(
             f"slave - {slave} does not exist, or is out of range"
         )
 
     def slaves(self):
```

### Comparing `pymodbus-3.3.2/pymodbus/datastore/remote.py` & `pymodbus-3.4.0/pymodbus/datastore/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Remote datastore."""
-# pylint: disable=missing-type-doc
 from pymodbus.datastore import ModbusBaseSlaveContext
 from pymodbus.exceptions import NotImplementedException
 from pymodbus.logging import Log
 
 
 # ---------------------------------------------------------------------------#
 #  Context
```

### Comparing `pymodbus-3.3.2/pymodbus/datastore/simulator.py` & `pymodbus-3.4.0/pymodbus/datastore/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -568,18 +568,17 @@
         :meta private:
         """
         result = []
         if func_code not in self._bits_func_code:
             real_address = self.fc_offset[func_code] + address
             for i in range(real_address, real_address + count):
                 reg = self.registers[i]
+                kwargs = reg.action_kwargs if reg.action_kwargs else {}
                 if reg.action:
-                    self.action_methods[reg.action](
-                        self.registers, i, reg, reg.action_kwargs
-                    )
+                    self.action_methods[reg.action](self.registers, i, reg, **kwargs)
                 self.registers[i].count_read += 1
                 result.append(reg.value)
         else:
             # bit access
             real_address = self.fc_offset[func_code] + int(address / 16)
             bit_index = address % 16
             reg_count = int((count + bit_index + 15) / 16)
@@ -627,82 +626,97 @@
         return
 
     # --------------------------------------------
     # Internal action methods
     # --------------------------------------------
 
     @classmethod
-    def action_random(cls, registers, inx, cell, _kwargs):
+    def action_random(cls, registers, inx, cell, minval=1, maxval=65536):
         """Update with random value.
 
         :meta private:
         """
         if cell.type in (CellType.BITS, CellType.UINT16):
-            registers[inx].value = random.randint(1, 65536)
+            registers[inx].value = random.randint(int(minval), int(maxval))
         elif cell.type == CellType.FLOAT32:
-            regs = cls.build_registers_from_value(random.uniform(1.0, 65000.0), False)
+            regs = cls.build_registers_from_value(
+                random.uniform(float(minval), float(maxval)), False
+            )
             registers[inx].value = regs[0]
             registers[inx + 1].value = regs[1]
         elif cell.type == CellType.UINT32:
             regs = cls.build_registers_from_value(
-                int(random.uniform(0.0, 65000.0)), True
+                random.randint(int(minval), int(maxval)), True
             )
             registers[inx].value = regs[0]
             registers[inx + 1].value = regs[1]
 
     @classmethod
-    def action_increment(cls, registers, inx, cell, _kwargs):
+    def action_increment(cls, registers, inx, cell, minval=None, maxval=None):
         """Increment value reset with overflow.
 
         :meta private:
         """
         reg = registers[inx]
         reg2 = registers[inx + 1]
         if cell.type in (CellType.BITS, CellType.UINT16):
-            reg.value += 1
+            value = reg.value + 1
+            if maxval and value > maxval:
+                value = minval
+            if minval and value < minval:
+                value = minval
+            reg.value = value
         elif cell.type == CellType.FLOAT32:
             tmp_reg = [reg.value, reg2.value]
             value = cls.build_value_from_registers(tmp_reg, False)
             value += 1.0
+            if maxval and value > maxval:
+                value = minval
+            if minval and value < minval:
+                value = minval
             new_regs = cls.build_registers_from_value(value, False)
             reg.value = new_regs[0]
             reg2.value = new_regs[1]
         elif cell.type == CellType.UINT32:
             tmp_reg = [reg.value, reg2.value]
             value = cls.build_value_from_registers(tmp_reg, True)
             value += 1
+            if maxval and value > maxval:
+                value = minval
+            if minval and value < minval:
+                value = minval
             new_regs = cls.build_registers_from_value(value, True)
             reg.value = new_regs[0]
             reg2.value = new_regs[1]
 
     @classmethod
-    def action_timestamp(cls, registers, inx, _cell, _kwargs):
+    def action_timestamp(cls, registers, inx, _cell, **_kwargs):
         """Set current time.
 
         :meta private:
         """
         system_time = datetime.now()
         registers[inx].value = system_time.year
         registers[inx + 1].value = system_time.month - 1
         registers[inx + 2].value = system_time.day
         registers[inx + 3].value = system_time.weekday() + 1
         registers[inx + 4].value = system_time.hour
         registers[inx + 5].value = system_time.minute
         registers[inx + 6].value = system_time.second
 
     @classmethod
-    def action_reset(cls, _registers, _inx, _cell, _kwargs):
+    def action_reset(cls, _registers, _inx, _cell, **_kwargs):
         """Reboot server.
 
         :meta private:
         """
         raise RuntimeError("RESET server")
 
     @classmethod
-    def action_uptime(cls, registers, inx, cell, _kwargs):
+    def action_uptime(cls, registers, inx, cell, **_kwargs):
         """Return uptime in seconds.
 
         :meta private:
         """
         value = int(datetime.now().timestamp()) - cls.start_time + 1
 
         if cell.type in (CellType.BITS, CellType.UINT16):
@@ -749,23 +763,23 @@
     @classmethod
     def build_registers_from_value(cls, value, is_int):
         """Build registers from int32 or float32"""
         regs = [0, 0]
         if is_int:
             value_bytes = int.to_bytes(value, 4, "big")
         else:
-            value_bytes = struct.pack("f", value)
+            value_bytes = struct.pack(">f", value)
         regs[0] = int.from_bytes(value_bytes[:2], "big")
         regs[1] = int.from_bytes(value_bytes[-2:], "big")
         return regs
 
     @classmethod
     def build_value_from_registers(cls, registers, is_int):
         """Build registers from int32 or float32"""
         value_bytes = int.to_bytes(registers[0], 2, "big") + int.to_bytes(
             registers[1], 2, "big"
         )
         if is_int:
             value = int.from_bytes(value_bytes, "big")
         else:
-            value = struct.unpack("f", value_bytes)[0]
+            value = struct.unpack(">f", value_bytes)[0]
         return value
```

### Comparing `pymodbus-3.3.2/pymodbus/datastore/store.py` & `pymodbus-3.4.0/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/device.py` & `pymodbus-3.4.0/pymodbus/device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/diag_message.py` & `pymodbus-3.4.0/pymodbus/diag_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.constants import ModbusPlusOperation, ModbusStatus
 from pymodbus.device import ModbusControlBlock
-from pymodbus.exceptions import NotImplementedException
+from pymodbus.exceptions import ModbusException, NotImplementedException
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.utilities import pack_bitstring
 
 
 _MCB = ModbusControlBlock()
 
 
@@ -83,30 +83,33 @@
         """
         packet = struct.pack(">H", self.sub_function_code)
         if self.message is not None:
             if isinstance(self.message, str):
                 packet += self.message.encode()
             elif isinstance(self.message, bytes):
                 packet += self.message
-            elif isinstance(self.message, list):
+            elif isinstance(self.message, (list, tuple)):
                 for piece in self.message:
                     packet += struct.pack(">H", piece)
             elif isinstance(self.message, int):
                 packet += struct.pack(">H", self.message)
         return packet
 
     def decode(self, data):
         """Decode a diagnostic request.
 
         :param data: The data to decode into the function code
         """
         (
             self.sub_function_code,  # pylint: disable=attribute-defined-outside-init
-            self.message,
-        ) = struct.unpack(">HH", data)
+        ) = struct.unpack(">H", data[:2])
+        if self.sub_function_code == ReturnQueryDataRequest.sub_function_code:
+            self.message = data[2:]
+        else:
+            (self.message,) = struct.unpack(">H", data[2:])
 
     def get_response_pdu_size(self):
         """Get response pdu size.
 
         Func_code (1 byte) + Sub function code (2 byte) + Data (2 * N bytes)
         :return:
         """
@@ -154,26 +157,27 @@
         return packet
 
     def decode(self, data):
         """Decode diagnostic response.
 
         :param data: The data to decode into the function code
         """
-        word_len = len(data) // 2
-        if len(data) % 2:
-            word_len += 1
-            data += b"0"
-        data = struct.unpack(">" + "H" * word_len, data)
         (
             self.sub_function_code,  # pylint: disable=attribute-defined-outside-init
-            self.message,
-        ) = (
-            data[0],
-            data[1:],
-        )
+        ) = struct.unpack(">H", data[:2])
+        data = data[2:]
+        if self.sub_function_code == ReturnQueryDataRequest.sub_function_code:
+            self.message = data
+        else:
+            word_len = len(data) // 2
+            if len(data) % 2:
+                word_len += 1
+                data += b"0"
+            data = struct.unpack(">" + "H" * word_len, data)
+            self.message = data
 
 
 class DiagnosticStatusSimpleRequest(DiagnosticStatusRequest):
     """Return diagnostic status.
 
     A large majority of the diagnostic functions are simple
     status request functions.  They work by sending 0x0000
@@ -227,24 +231,23 @@
     The data passed in the request data field is to be returned (looped back)
     in the response. The entire response message should be identical to the
     request.
     """
 
     sub_function_code = 0x0000
 
-    def __init__(self, message=0x0000, slave=None, **kwargs):
+    def __init__(self, message=b"\x00\x00", slave=None, **kwargs):
         """Initialize a new instance of the request.
 
         :param message: The message to send to loopback
         """
         DiagnosticStatusRequest.__init__(self, slave=slave, **kwargs)
-        if isinstance(message, list):
-            self.message = message
-        else:
-            self.message = [message]
+        if not isinstance(message, bytes):
+            raise ModbusException(f"message({type(message)}) must be bytes")
+        self.message = message
 
     def execute(self, *_args):
         """Execute the loopback request (builds the response).
 
         :returns: The populated loopback response message
         """
         return ReturnQueryDataResponse(self.message)
@@ -256,24 +259,23 @@
     The data passed in the request data field is to be returned (looped back)
     in the response. The entire response message should be identical to the
     request.
     """
 
     sub_function_code = 0x0000
 
-    def __init__(self, message=0x0000, **kwargs):
+    def __init__(self, message=b"\x00\x00", **kwargs):
         """Initialize a new instance of the response.
 
         :param message: The message to loopback
         """
         DiagnosticStatusResponse.__init__(self, **kwargs)
-        if isinstance(message, list):
-            self.message = message
-        else:
-            self.message = [message]
+        if not isinstance(message, bytes):
+            raise ModbusException(f"message({type(message)}) must be bytes")
+        self.message = message
 
 
 # ---------------------------------------------------------------------------#
 #  Diagnostic Sub Code 01
 # ---------------------------------------------------------------------------#
 class RestartCommunicationsOptionRequest(DiagnosticStatusRequest):
     """Restart communication.
```

### Comparing `pymodbus-3.3.2/pymodbus/events.py` & `pymodbus-3.4.0/pymodbus/events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/exceptions.py` & `pymodbus-3.4.0/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/factory.py` & `pymodbus-3.4.0/pymodbus/factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/file_message.py` & `pymodbus-3.4.0/pymodbus/file_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # ---------------------------------------------------------------------------#
 class FileRecord:  # pylint: disable=eq-without-hash
     """Represents a file record and its relevant data."""
 
     def __init__(self, **kwargs):
         """Initialize a new instance.
 
-        :params reference_type: Defaults to 0x06 (must be)
+        :params reference_type: must be 0x06
         :params file_number: Indicates which file number we are reading
         :params record_number: Indicates which record in the file
         :params record_data: The actual data of the record
         :params record_length: The length in registers of the record
         :params response_length: The length in bytes of the record
         """
         self.reference_type = kwargs.get("reference_type", 0x06)
```

### Comparing `pymodbus-3.3.2/pymodbus/framer/ascii_framer.py` & `pymodbus-3.4.0/pymodbus/framer/socket_framer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,207 +1,182 @@
-"""Ascii_framer."""
+"""Socket framer."""
 # pylint: disable=missing-type-doc
 import struct
-from binascii import a2b_hex, b2a_hex
 
-from pymodbus.exceptions import ModbusIOException
-from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
+from pymodbus.exceptions import (
+    InvalidMessageReceivedException,
+    ModbusIOException,
+)
+from pymodbus.framer.base import SOCKET_FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
-from pymodbus.utilities import checkLRC, computeLRC
-
-
-ASCII_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 
 # --------------------------------------------------------------------------- #
-# Modbus ASCII Message
+# Modbus TCP Message
 # --------------------------------------------------------------------------- #
-class ModbusAsciiFramer(ModbusFramer):
-    r"""Modbus ASCII Frame Controller.
 
-        [ Start ][Address ][ Function ][ Data ][ LRC ][ End ]
-          1c        2c         2c         Nc     2c      2c
 
-        * data can be 0 - 2x252 chars
-        * end is "\\r\\n" (Carriage return line feed), however the line feed
-          character can be changed via a special command
-        * start is ":"
+class ModbusSocketFramer(ModbusFramer):
+    """Modbus Socket Frame controller.
+
+    Before each modbus TCP message is an MBAP header which is used as a
+    message frame.  It allows us to easily separate messages as follows::
+
+        [         MBAP Header         ] [ Function Code] [ Data ] \
+        [ tid ][ pid ][ length ][ uid ]
+          2b     2b     2b        1b           1b           Nb
+
+        while len(message) > 0:
+            tid, pid, length`, uid = struct.unpack(">HHHB", message)
+            request = message[0:7 + length - 1`]
+            message = [7 + length - 1:]
 
-    This framer is used for serial transmission.  Unlike the RTU protocol,
-    the data in this framer is transferred in plain text ascii.
+        * length = uid + function code + data
+        * The -1 is to account for the uid byte
     """
 
-    method = "ascii"
+    method = "socket"
 
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
-        :param decoder: The decoder implementation to use
+        :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
-        self._buffer = b""
-        self._header = {"lrc": "0000", "len": 0, "uid": 0x00}
-        self._hsize = 0x02
-        self._start = b":"
-        self._end = b"\r\n"
+        self._hsize = 0x07
 
     # ----------------------------------------------------------------------- #
     # Private Helper Functions
     # ----------------------------------------------------------------------- #
-    def decode_data(self, data):
-        """Decode data."""
-        if len(data) > 1:
-            uid = int(data[1:3], 16)
-            fcode = int(data[3:5], 16)
-            return {"slave": uid, "fcode": fcode}
-        return {}
-
     def checkFrame(self):
         """Check and decode the next frame.
 
-        :returns: True if we successful, False otherwise
+        Return true if we were successful.
         """
-        start = self._buffer.find(self._start)
-        if start == -1:
-            return False
-        if start > 0:  # go ahead and skip old bad data
-            self._buffer = self._buffer[start:]
-            start = 0
-
-        if (end := self._buffer.find(self._end)) != -1:
-            self._header["len"] = end
-            self._header["uid"] = int(self._buffer[1:3], 16)
-            self._header["lrc"] = int(self._buffer[end - 2 : end], 16)
-            data = a2b_hex(self._buffer[start + 1 : end - 2])
-            return checkLRC(data, self._header["lrc"])
+        if self.isFrameReady():
+            (
+                self._header["tid"],
+                self._header["pid"],
+                self._header["len"],
+                self._header["uid"],
+            ) = struct.unpack(">HHHB", self._buffer[0 : self._hsize])
+
+            # someone sent us an error? ignore it
+            if self._header["len"] < 2:
+                self.advanceFrame()
+            # we have at least a complete message, continue
+            elif len(self._buffer) - self._hsize + 1 >= self._header["len"]:
+                return True
+        # we don't have enough of a message yet, wait
         return False
 
     def advanceFrame(self):
         """Skip over the current framed message.
 
         This allows us to skip over the current message after we have processed
         it or determined that it contains an error. It also has to reset the
         current frame header handle
         """
-        self._buffer = self._buffer[self._header["len"] + 2 :]
-        self._header = {"lrc": "0000", "len": 0, "uid": 0x00}
+        length = self._hsize + self._header["len"] - 1
+        self._buffer = self._buffer[length:]
+        self._header = {"tid": 0, "pid": 0, "len": 0, "uid": 0}
 
     def isFrameReady(self):
         """Check if we should continue decode logic.
 
         This is meant to be used in a while loop in the decoding phase to let
-        the decoder know that there is still data in the buffer.
+        the decoder factory know that there is still data in the buffer.
 
         :returns: True if ready, False otherwise
         """
-        return len(self._buffer) > 1
-
-    def addToFrame(self, message):
-        """Add the next message to the frame buffer.
-
-        This should be used before the decoding while loop to add the received
-        data to the buffer handle.
-
-        :param message: The most recent packet
-        """
-        self._buffer += message
+        return len(self._buffer) > self._hsize
 
     def getFrame(self):
-        """Get the next frame from the buffer.
+        """Return the next frame from the buffered data.
 
-        :returns: The frame data or ""
+        :returns: The next full frame buffer
         """
-        start = self._hsize + 1
-        end = self._header["len"] - 2
-        buffer = self._buffer[start:end]
-        if end > 0:
-            return a2b_hex(buffer)
-        return b""
-
-    def resetFrame(self):
-        """Reset the entire message frame.
-
-        This allows us to skip ovver errors that may be in the stream.
-        It is hard to know if we are simply out of sync or if there is
-        an error in the stream as we have no way to check the start or
-        end of the message (python just doesn't have the resolution to
-        check for millisecond delays).
-        """
-        self._buffer = b""
-        self._header = {"lrc": "0000", "len": 0, "uid": 0x00}
-
-    def populateResult(self, result):
-        """Populate the modbus result header.
-
-        The serial packets do not have any header information
-        that is copied.
-
-        :param result: The response packet
-        """
-        result.slave_id = self._header["uid"]
+        length = self._hsize + self._header["len"] - 1
+        return self._buffer[self._hsize : length]
 
     # ----------------------------------------------------------------------- #
     # Public Member Functions
     # ----------------------------------------------------------------------- #
-    def processIncomingPacket(self, data, callback, slave, **kwargs):
+    def decode_data(self, data):
+        """Decode data."""
+        if len(data) > self._hsize:
+            tid, pid, length, uid, fcode = struct.unpack(
+                SOCKET_FRAME_HEADER, data[0 : self._hsize + 1]
+            )
+            return {
+                "tid": tid,
+                "pid": pid,
+                "length": length,
+                "slave": uid,
+                "fcode": fcode,
+            }
+        return {}
+
+    def frameProcessIncomingPacket(self, single, callback, slave, tid=None, **kwargs):
         """Process new packet pattern.
 
         This takes in a new request packet, adds it to the current
         packet stream, and performs framing on it. That is, checks
         for complete messages, and once found, will process all that
         exist.  This handles the case when we read N + 1 or 1 // N
         messages at a time instead of 1.
 
         The processed and decoded messages are pushed to the callback
         function to process and send.
-
-        :param data: The new packet data
-        :param callback: The function to send results to
-        :param slave: Process if slave id matches, ignore otherwise (could be a
-               list of slave ids (server) or single slave id(client/server))
-        :param kwargs:
-        :raises ModbusIOException:
-        """
-        if not isinstance(slave, (list, tuple)):
-            slave = [slave]
-        single = kwargs.get("single", False)
-        self.addToFrame(data)
-        while self.isFrameReady():
-            if not self.checkFrame():
+        """
+        while True:
+            if not self.isFrameReady():
+                if len(self._buffer):
+                    # Possible error ???
+                    if self._header["len"] < 2:
+                        self._process(callback, tid, error=True)
                 break
+            if not self.checkFrame():
+                Log.debug("Frame check failed, ignoring!!")
+                self.resetFrame()
+                continue
             if not self._validate_slave_id(slave, single):
                 header_txt = self._header["uid"]
-                Log.error("Not a valid slave id - {}, ignoring!!", header_txt)
+                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
                 self.resetFrame()
                 continue
+            self._process(callback, tid)
 
-            frame = self.getFrame()
-            if (result := self.decoder.decode(frame)) is None:
-                raise ModbusIOException("Unable to decode response")
-            self.populateResult(result)
-            self.advanceFrame()
-            callback(result)  # defer this
+    def _process(self, callback, tid, error=False):
+        """Process incoming packets irrespective error condition."""
+        data = self._buffer if error else self.getFrame()
+        if (result := self.decoder.decode(data)) is None:
+            self.resetFrame()
+            raise ModbusIOException("Unable to decode request")
+        if error and result.function_code < 0x80:
+            raise InvalidMessageReceivedException(result)
+        self.populateResult(result)
+        self.advanceFrame()
+        if tid and tid != result.transaction_id:
+            self.resetFrame()
+        else:
+            callback(result)  # defer or push to a thread?
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
-        Built off of a  modbus request/response
-
-        :param message: The request/response to send
-        :return: The encoded packet
+        :param message: The populated request/response to send
         """
-        encoded = message.encode()
-        buffer = struct.pack(
-            ASCII_FRAME_HEADER, message.slave_id, message.function_code
+        data = message.encode()
+        packet = struct.pack(
+            SOCKET_FRAME_HEADER,
+            message.transaction_id,
+            message.protocol_id,
+            len(data) + 2,
+            message.slave_id,
+            message.function_code,
         )
-        checksum = computeLRC(encoded + buffer)
-
-        packet = bytearray()
-        packet.extend(self._start)
-        packet.extend(f"{message.slave_id:02x}{message.function_code:02x}".encode())
-        packet.extend(b2a_hex(encoded))
-        packet.extend(f"{checksum:02x}".encode())
-        packet.extend(self._end)
-        return bytes(packet).upper()
+        packet += data
+        return packet
 
 
 # __END__
```

### Comparing `pymodbus-3.3.2/pymodbus/framer/binary_framer.py` & `pymodbus-3.4.0/pymodbus/utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,270 @@
-"""Binary framer."""
+"""Modbus Utilities.
+
+A collection of utilities for packing data, unpacking
+data computing checksums, and decode checksums.
+"""
+
+__all__ = [
+    "pack_bitstring",
+    "unpack_bitstring",
+    "default",
+    "computeCRC",
+    "checkCRC",
+    "computeLRC",
+    "checkLRC",
+    "rtuFrameSize",
+]
+
 # pylint: disable=missing-type-doc
 import struct
+from typing import List
+
+
+class ModbusTransactionState:  # pylint: disable=too-few-public-methods
+    """Modbus Client States."""
+
+    IDLE = 0
+    SENDING = 1
+    WAITING_FOR_REPLY = 2
+    WAITING_TURNAROUND_DELAY = 3
+    PROCESSING_REPLY = 4
+    PROCESSING_ERROR = 5
+    TRANSACTION_COMPLETE = 6
+    RETRYING = 7
+    NO_RESPONSE_STATE = 8
+
+    @classmethod
+    def to_string(cls, state):
+        """Convert to string."""
+        states = {
+            ModbusTransactionState.IDLE: "IDLE",
+            ModbusTransactionState.SENDING: "SENDING",
+            ModbusTransactionState.WAITING_FOR_REPLY: "WAITING_FOR_REPLY",
+            ModbusTransactionState.WAITING_TURNAROUND_DELAY: "WAITING_TURNAROUND_DELAY",
+            ModbusTransactionState.PROCESSING_REPLY: "PROCESSING_REPLY",
+            ModbusTransactionState.PROCESSING_ERROR: "PROCESSING_ERROR",
+            ModbusTransactionState.TRANSACTION_COMPLETE: "TRANSACTION_COMPLETE",
+            ModbusTransactionState.RETRYING: "RETRYING TRANSACTION",
+        }
+        return states.get(state, None)
+
+
+# --------------------------------------------------------------------------- #
+# Helpers
+# --------------------------------------------------------------------------- #
 
-from pymodbus.exceptions import ModbusIOException
-from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
-from pymodbus.logging import Log
-from pymodbus.utilities import checkCRC, computeCRC
-
-
-BINARY_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
-
-# --------------------------------------------------------------------------- #
-# Modbus Binary Message
-# --------------------------------------------------------------------------- #
-
-
-class ModbusBinaryFramer(ModbusFramer):
-    """Modbus Binary Frame Controller.
-
-        [ Start ][Address ][ Function ][ Data ][ CRC ][ End ]
-          1b        1b         1b         Nb     2b     1b
-
-        * data can be 0 - 2x252 chars
-        * end is   "}"
-        * start is "{"
-
-    The idea here is that we implement the RTU protocol, however,
-    instead of using timing for message delimiting, we use start
-    and end of message characters (in this case { and }). Basically,
-    this is a binary framer.
-
-    The only case we have to watch out for is when a message contains
-    the { or } characters.  If we encounter these characters, we
-    simply duplicate them.  Hopefully we will not encounter those
-    characters that often and will save a little bit of bandwitch
-    without a real-time system.
-
-    Protocol defined by jamod.sourceforge.net.
-    """
-
-    method = "binary"
-
-    def __init__(self, decoder, client=None):
-        """Initialize a new instance of the framer.
-
-        :param decoder: The decoder implementation to use
-        """
-        super().__init__(decoder, client)
-        self._buffer = b""
-        self._header = {"crc": 0x0000, "len": 0, "uid": 0x00}
-        self._hsize = 0x01
-        self._start = b"\x7b"  # {
-        self._end = b"\x7d"  # }
-        self._repeat = [b"}"[0], b"{"[0]]  # python3 hack
-
-    # ----------------------------------------------------------------------- #
-    # Private Helper Functions
-    # ----------------------------------------------------------------------- #
-    def decode_data(self, data):
-        """Decode data."""
-        if len(data) > self._hsize:
-            uid = struct.unpack(">B", data[1:2])[0]
-            fcode = struct.unpack(">B", data[2:3])[0]
-            return {"slave": uid, "fcode": fcode}
-        return {}
-
-    def checkFrame(self) -> bool:
-        """Check and decode the next frame.
-
-        :returns: True if we are successful, False otherwise
-        """
-        start = self._buffer.find(self._start)
-        if start == -1:
-            return False
-        if start > 0:  # go ahead and skip old bad data
-            self._buffer = self._buffer[start:]
-
-        if (end := self._buffer.find(self._end)) != -1:
-            self._header["len"] = end
-            self._header["uid"] = struct.unpack(">B", self._buffer[1:2])[0]
-            self._header["crc"] = struct.unpack(">H", self._buffer[end - 2 : end])[0]
-            data = self._buffer[start + 1 : end - 2]
-            return checkCRC(data, self._header["crc"])
-        return False
-
-    def advanceFrame(self) -> None:
-        """Skip over the current framed message.
-
-        This allows us to skip over the current message after we have processed
-        it or determined that it contains an error. It also has to reset the
-        current frame header handle
-        """
-        self._buffer = self._buffer[self._header["len"] + 2 :]
-        self._header = {"crc": 0x0000, "len": 0, "uid": 0x00}
-
-    def isFrameReady(self) -> bool:
-        """Check if we should continue decode logic.
-
-        This is meant to be used in a while loop in the decoding phase to let
-        the decoder know that there is still data in the buffer.
-
-        :returns: True if ready, False otherwise
-        """
-        return len(self._buffer) > 1
-
-    def addToFrame(self, message):
-        """Add the next message to the frame buffer.
-
-        This should be used before the decoding while loop to add the received
-        data to the buffer handle.
-
-        :param message: The most recent packet
-        """
-        self._buffer += message
-
-    def getFrame(self):
-        """Get the next frame from the buffer.
-
-        :returns: The frame data or ""
-        """
-        start = self._hsize + 1
-        end = self._header["len"] - 2
-        buffer = self._buffer[start:end]
-        if end > 0:
-            return buffer
-        return b""
-
-    def populateResult(self, result):
-        """Populate the modbus result header.
-
-        The serial packets do not have any header information
-        that is copied.
-
-        :param result: The response packet
-        """
-        result.slave_id = self._header["uid"]
-
-    # ----------------------------------------------------------------------- #
-    # Public Member Functions
-    # ----------------------------------------------------------------------- #
-    def processIncomingPacket(self, data, callback, slave, **kwargs):
-        """Process new packet pattern.
-
-        This takes in a new request packet, adds it to the current
-        packet stream, and performs framing on it. That is, checks
-        for complete messages, and once found, will process all that
-        exist.  This handles the case when we read N + 1 or 1 // N
-        messages at a time instead of 1.
-
-        The processed and decoded messages are pushed to the callback
-        function to process and send.
-
-        :param data: The new packet data
-        :param callback: The function to send results to
-        :param slave: Process if slave id matches, ignore otherwise (could be a
-               list of slave ids (server) or single slave id(client/server)
-        :param kwargs:
-        :raises ModbusIOException:
-        """
-        self.addToFrame(data)
-        if not isinstance(slave, (list, tuple)):
-            slave = [slave]
-        single = kwargs.get("single", False)
-        while self.isFrameReady():
-            if not self.checkFrame():
-                Log.debug("Frame check failed, ignoring!!")
-                self.resetFrame()
-                break
-            if not self._validate_slave_id(slave, single):
-                header_txt = self._header["uid"]
-                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
-                self.resetFrame()
-                break
-            if (result := self.decoder.decode(self.getFrame())) is None:
-                raise ModbusIOException("Unable to decode response")
-            self.populateResult(result)
-            self.advanceFrame()
-            callback(result)  # defer or push to a thread?
-
-    def buildPacket(self, message):
-        """Create a ready to send modbus packet.
-
-        :param message: The request/response to send
-        :returns: The encoded packet
-        """
-        data = self._preflight(message.encode())
-        packet = (
-            struct.pack(BINARY_FRAME_HEADER, message.slave_id, message.function_code)
-            + data
+
+def default(value):
+    """Return the default value of object.
+
+    :param value: The value to get the default of
+    :returns: The default value
+    """
+    return type(value)()
+
+
+def dict_property(store, index):
+    """Create class properties from a dictionary.
+
+    Basically this allows you to remove a lot of possible
+    boilerplate code.
+
+    :param store: The store store to pull from
+    :param index: The index into the store to close over
+    :returns: An initialized property set
+    """
+    if hasattr(store, "__call__"):
+        getter = lambda self: store(  # pylint: disable=unnecessary-lambda-assignment
+            self
+        )[index]
+        setter = lambda self, value: store(  # pylint: disable=unnecessary-dunder-call,unnecessary-lambda-assignment
+            self
+        ).__setitem__(
+            index, value
+        )
+    elif isinstance(store, str):
+        getter = lambda self: self.__getattribute__(  # pylint: disable=unnecessary-dunder-call,unnecessary-lambda-assignment
+            store
+        )[
+            index
+        ]
+        setter = lambda self, value: self.__getattribute__(  # pylint: disable=unnecessary-dunder-call,unnecessary-lambda-assignment
+            store
+        ).__setitem__(
+            index, value
         )
-        packet += struct.pack(">H", computeCRC(packet))
-        packet = self._start + packet + self._end
-        return packet
-
-    def _preflight(self, data):
-        """Do preflight buffer test.
-
-        This basically scans the buffer for start and end
-        tags and if found, escapes them.
-
-        :param data: The message to escape
-        :returns: the escaped packet
-        """
-        array = bytearray()
-        for item in data:
-            if item in self._repeat:
-                array.append(item)
-            array.append(item)
-        return bytes(array)
-
-    def resetFrame(self):
-        """Reset the entire message frame.
-
-        This allows us to skip ovver errors that may be in the stream.
-        It is hard to know if we are simply out of sync or if there is
-        an error in the stream as we have no way to check the start or
-        end of the message (python just doesn't have the resolution to
-        check for millisecond delays).
-        """
-        self._buffer = b""
-        self._header = {"crc": 0x0000, "len": 0, "uid": 0x00}
+    else:
+        getter = lambda self: store[  # pylint: disable=unnecessary-lambda-assignment
+            index
+        ]
+        setter = lambda self, value: store.__setitem__(  # pylint: disable=unnecessary-dunder-call,unnecessary-lambda-assignment
+            index, value
+        )
+
+    return property(getter, setter)
+
+
+# --------------------------------------------------------------------------- #
+# Bit packing functions
+# --------------------------------------------------------------------------- #
+def pack_bitstring(bits: List[bool]) -> bytes:
+    """Create a bytestring out of a list of bits.
+
+    :param bits: A list of bits
+
+    example::
+
+        bits   = [False, True, False, True]
+        result = pack_bitstring(bits)
+    """
+    ret = b""
+    i = packed = 0
+    for bit in bits:
+        if bit:
+            packed += 128
+        i += 1
+        if i == 8:
+            ret += struct.pack(">B", packed)
+            i = packed = 0
+        else:
+            packed >>= 1
+    if 0 < i < 8:
+        packed >>= 7 - i
+        ret += struct.pack(">B", packed)
+    return ret
+
+
+def unpack_bitstring(data: bytes) -> List[bool]:
+    """Create bit list out of a bytestring.
+
+    :param data: The modbus data packet to decode
+
+    example::
+
+        bytes  = "bytes to decode"
+        result = unpack_bitstring(bytes)
+    """
+    byte_count = len(data)
+    bits = []
+    for byte in range(byte_count):
+        value = int(int(data[byte]))
+        for _ in range(8):
+            bits.append((value & 1) == 1)
+            value >>= 1
+    return bits
+
+
+# --------------------------------------------------------------------------- #
+# Error Detection Functions
+# --------------------------------------------------------------------------- #
+
+
+def __generate_crc16_table():
+    """Generate a crc16 lookup table.
+
+    .. note:: This will only be generated once
+    """
+    result = []
+    for byte in range(256):
+        crc = 0x0000
+        for _ in range(8):
+            if (byte ^ crc) & 0x0001:
+                crc = (crc >> 1) ^ 0xA001
+            else:
+                crc >>= 1
+            byte >>= 1
+        result.append(crc)
+    return result
+
+
+__crc16_table = __generate_crc16_table()
+
+
+def computeCRC(data):  # pylint: disable=invalid-name
+    """Compute a crc16 on the passed in string.
+
+    For modbus, this is only used on the binary serial protocols (in this
+    case RTU).
+
+    The difference between modbus's crc16 and a normal crc16
+    is that modbus starts the crc value out at 0xffff.
+
+    :param data: The data to create a crc16 of
+    :returns: The calculated CRC
+    """
+    crc = 0xFFFF
+    for data_byte in data:
+        idx = __crc16_table[(crc ^ int(data_byte)) & 0xFF]
+        crc = ((crc >> 8) & 0xFF) ^ idx
+    swapped = ((crc << 8) & 0xFF00) | ((crc >> 8) & 0x00FF)
+    return swapped
+
+
+def checkCRC(data, check):  # pylint: disable=invalid-name
+    """Check if the data matches the passed in CRC.
+
+    :param data: The data to create a crc16 of
+    :param check: The CRC to validate
+    :returns: True if matched, False otherwise
+    """
+    return computeCRC(data) == check
+
+
+def computeLRC(data):  # pylint: disable=invalid-name
+    """Use to compute the longitudinal redundancy check against a string.
 
+    This is only used on the serial ASCII
+    modbus protocol. A full description of this implementation
+    can be found in appendix B of the serial line modbus description.
 
-# __END__
+    :param data: The data to apply a lrc to
+    :returns: The calculated LRC
+
+    """
+    lrc = sum(int(a) for a in data) & 0xFF
+    lrc = (lrc ^ 0xFF) + 1
+    return lrc & 0xFF
+
+
+def checkLRC(data, check):  # pylint: disable=invalid-name
+    """Check if the passed in data matches the LRC.
+
+    :param data: The data to calculate
+    :param check: The LRC to validate
+    :returns: True if matched, False otherwise
+    """
+    return computeLRC(data) == check
+
+
+def rtuFrameSize(data, byte_count_pos):  # pylint: disable=invalid-name
+    """Calculate the size of the frame based on the byte count.
+
+    :param data: The buffer containing the frame.
+    :param byte_count_pos: The index of the byte count in the buffer.
+    :returns: The size of the frame.
+
+    The structure of frames with a byte count field is always the
+    same:
+
+    - first, there are some header fields
+    - then the byte count field
+    - then as many data bytes as indicated by the byte count,
+    - finally the CRC (two bytes).
+
+    To calculate the frame size, it is therefore sufficient to extract
+    the contents of the byte count field, add the position of this
+    field, and finally increment the sum by three (one byte for the
+    byte count field, two for the CRC).
+    """
+    return int(data[byte_count_pos]) + byte_count_pos + 3
+
+
+def hexlify_packets(packet):
+    """Return hex representation of bytestring received.
+
+    :param packet:
+    :return:
+    """
+    if not packet:
+        return ""
+    return " ".join([hex(int(x)) for x in packet])
```

### Comparing `pymodbus-3.3.2/pymodbus/framer/rtu_framer.py` & `pymodbus-3.4.0/pymodbus/framer/rtu_framer.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,14 @@
 
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
         :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
-        self._buffer = b""
-        self._header = {"uid": 0x00, "len": 0, "crc": b"\x00\x00"}
         self._hsize = 0x01
         self._end = b"\x0d\x0a"
         self._min_frame_size = 4
         self.function_codes = set(self.decoder.lookup) if self.decoder else {}
 
     # ----------------------------------------------------------------------- #
     # Private Helper Functions
@@ -111,19 +109,17 @@
 
         This allows us to skip over errors that may be in the stream.
         It is hard to know if we are simply out of sync or if there is
         an error in the stream as we have no way to check the start or
         end of the message (python just doesn't have the resolution to
         check for millisecond delays).
         """
-        Log.debug(
-            "Resetting frame - Current Frame in buffer - {}", self._buffer, ":hex"
-        )
-        # self._buffer = b""
-        self._header = {"uid": 0x00, "len": 0, "crc": b"\x00\x00"}
+        x = self._buffer
+        super().resetFrame()
+        self._buffer = x
 
     def isFrameReady(self):
         """Check if we should continue decode logic.
 
         This is meant to be used in a while loop in the decoding phase to let
         the decoder know that there is still data in the buffer.
 
@@ -148,30 +144,24 @@
         information into `self._header`.
 
         Beware that this method will raise an IndexError if
         `self._buffer` is not yet long enough.
         """
         data = data if data is not None else self._buffer
         self._header["uid"] = int(data[0])
+        self._header["tid"] = int(data[0])
         size = self.get_expected_response_length(data)
         self._header["len"] = size
 
         if len(data) < size:
             # crc yet not available
             raise IndexError
         self._header["crc"] = data[size - 2 : size]
         return size
 
-    def addToFrame(self, message):
-        """Add the received data to the buffer handle.
-
-        :param message: The most recent packet
-        """
-        self._buffer += message
-
     def getFrame(self):
         """Get the next frame from the buffer.
 
         :returns: The frame data or ""
         """
         start = self._hsize
         end = self._header["len"] - 2
@@ -186,63 +176,46 @@
 
         The serial packets do not have any header information
         that is copied.
 
         :param result: The response packet
         """
         result.slave_id = self._header["uid"]
-        result.transaction_id = self._header["uid"]
+        result.transaction_id = self._header["tid"]
 
     def getFrameStart(self, slaves, broadcast, skip_cur_frame):
         """Scan buffer for a relevant frame start."""
         start = 1 if skip_cur_frame else 0
         if (buf_len := len(self._buffer)) < 4:
             return False
         for i in range(start, buf_len - 3):  # <slave id><function code><crc 2 bytes>
             if not broadcast and self._buffer[i] not in slaves:
                 continue
-            if self._buffer[i + 1] not in self.function_codes:
+            if (
+                self._buffer[i + 1] not in self.function_codes
+                and (self._buffer[i + 1] - 0x80) not in self.function_codes
+            ):
                 continue
             if i:
                 self._buffer = self._buffer[i:]  # remove preceding trash.
             return True
         if buf_len > 3:
             self._buffer = self._buffer[-3:]
         return False
 
     # ----------------------------------------------------------------------- #
     # Public Member Functions
     # ----------------------------------------------------------------------- #
-    def processIncomingPacket(self, data, callback, slave, **kwargs):
-        """Process new packet pattern.
-
-        This takes in a new request packet, adds it to the current
-        packet stream, and performs framing on it. That is, checks
-        for complete messages, and once found, will process all that
-        exist.  This handles the case when we read N + 1 or 1 // N
-        messages at a time instead of 1.
-
-        The processed and decoded messages are pushed to the callback
-        function to process and send.
-
-        :param data: The new packet data
-        :param callback: The function to send results to
-        :param slave: Process if slave id matches, ignore otherwise (could be a
-               list of slave ids (server) or single slave id(client/server)
-        :param kwargs:
-        """
-        if not isinstance(slave, (list, tuple)):
-            slave = [slave]
+    def frameProcessIncomingPacket(self, single, callback, slave, _tid=None, **kwargs):
+        """Process new packet pattern."""
         broadcast = not slave[0]
-        self.addToFrame(data)
-        single = kwargs.get("single", False)
         skip_cur_frame = False
         while self.getFrameStart(slave, broadcast, skip_cur_frame):
             if not self.isFrameReady():
-                Log.debug("Frame - [{}] not ready", data)
+                Log.debug("Frame - not ready")
                 break
             if not self.checkFrame():
                 Log.debug("Frame check failed, ignoring!!")
                 self.resetFrame()
                 skip_cur_frame = True
                 continue
             if not self._validate_slave_id(slave, single):
@@ -271,15 +244,15 @@
     def sendPacket(self, message):
         """Send packets on the bus with 3.5char delay between frames.
 
         :param message: Message to be sent over the bus
         :return:
         """
         start = time.time()
-        timeout = start + self.client.params.timeout
+        timeout = start + self.client.comm_params.timeout_connect
         while self.client.state != ModbusTransactionState.IDLE:
             if self.client.state == ModbusTransactionState.TRANSACTION_COMPLETE:
                 timestamp = round(time.time(), 6)
                 Log.debug(
                     "Changing state to IDLE - Last Frame End - {} Current Time stamp - {}",
                     self.client.last_frame_end,
                     timestamp,
@@ -295,15 +268,15 @@
                 else:
                     # Recovering from last error ??
                     time.sleep(self.client.silent_interval)
                 self.client.state = ModbusTransactionState.IDLE
             elif self.client.state == ModbusTransactionState.RETRYING:
                 # Simple lets settle down!!!
                 # To check for higher baudrates
-                time.sleep(self.client.params.timeout)
+                time.sleep(self.client.comm_params.timeout_connect)
                 break
             elif time.time() > timeout:
                 Log.debug(
                     "Spent more time than the read time out, "
                     "resetting the transaction to IDLE"
                 )
                 self.client.state = ModbusTransactionState.IDLE
@@ -322,28 +295,23 @@
         """
         result = self.client.recv(size)
         self.client.last_frame_end = round(time.time(), 6)
         return result
 
     def _process(self, callback, error=False):
         """Process incoming packets irrespective error condition."""
-        data = self.getRawFrame() if error else self.getFrame()
+        data = self._buffer if error else self.getFrame()
         if (result := self.decoder.decode(data)) is None:
             raise ModbusIOException("Unable to decode request")
         if error and result.function_code < 0x80:
             raise InvalidMessageReceivedException(result)
         self.populateResult(result)
         self.advanceFrame()
         callback(result)  # defer or push to a thread?
 
-    def getRawFrame(self):
-        """Return the complete buffer."""
-        Log.debug("Getting Raw Frame - {}", self._buffer, ":hex")
-        return self._buffer
-
     def get_expected_response_length(self, data):
         """Get the expected response length.
 
         :param data: Message data read so far
         :raises IndexError: If not enough data to read byte count
         :return: Total frame size
         """
```

### Comparing `pymodbus-3.3.2/pymodbus/framer/socket_framer.py` & `pymodbus-3.4.0/pymodbus/framer/ascii_framer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,224 +1,152 @@
-"""Socket framer."""
+"""Ascii_framer."""
 # pylint: disable=missing-type-doc
 import struct
+from binascii import a2b_hex, b2a_hex
 
-from pymodbus.exceptions import (
-    InvalidMessageReceivedException,
-    ModbusIOException,
-)
-from pymodbus.framer.base import SOCKET_FRAME_HEADER, ModbusFramer
+from pymodbus.exceptions import ModbusIOException
+from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
+from pymodbus.utilities import checkLRC, computeLRC
 
 
-# --------------------------------------------------------------------------- #
-# Modbus TCP Message
-# --------------------------------------------------------------------------- #
+ASCII_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 
-class ModbusSocketFramer(ModbusFramer):
-    """Modbus Socket Frame controller.
+# --------------------------------------------------------------------------- #
+# Modbus ASCII Message
+# --------------------------------------------------------------------------- #
+class ModbusAsciiFramer(ModbusFramer):
+    r"""Modbus ASCII Frame Controller.
 
-    Before each modbus TCP message is an MBAP header which is used as a
-    message frame.  It allows us to easily separate messages as follows::
+        [ Start ][Address ][ Function ][ Data ][ LRC ][ End ]
+          1c        2c         2c         Nc     2c      2c
 
-        [         MBAP Header         ] [ Function Code] [ Data ] \
-        [ tid ][ pid ][ length ][ uid ]
-          2b     2b     2b        1b           1b           Nb
-
-        while len(message) > 0:
-            tid, pid, length`, uid = struct.unpack(">HHHB", message)
-            request = message[0:7 + length - 1`]
-            message = [7 + length - 1:]
+        * data can be 0 - 2x252 chars
+        * end is "\\r\\n" (Carriage return line feed), however the line feed
+          character can be changed via a special command
+        * start is ":"
 
-        * length = uid + function code + data
-        * The -1 is to account for the uid byte
+    This framer is used for serial transmission.  Unlike the RTU protocol,
+    the data in this framer is transferred in plain text ascii.
     """
 
-    method = "socket"
+    method = "ascii"
 
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
-        :param decoder: The decoder factory implementation to use
+        :param decoder: The decoder implementation to use
         """
         super().__init__(decoder, client)
-        self._buffer = b""
-        self._header = {"tid": 0, "pid": 0, "len": 0, "uid": 0}
-        self._hsize = 0x07
+        self._hsize = 0x02
+        self._start = b":"
+        self._end = b"\r\n"
 
     # ----------------------------------------------------------------------- #
     # Private Helper Functions
     # ----------------------------------------------------------------------- #
+    def decode_data(self, data):
+        """Decode data."""
+        if len(data) > 1:
+            uid = int(data[1:3], 16)
+            fcode = int(data[3:5], 16)
+            return {"slave": uid, "fcode": fcode}
+        return {}
+
     def checkFrame(self):
         """Check and decode the next frame.
 
-        Return true if we were successful.
+        :returns: True if we successful, False otherwise
         """
-        if self.isFrameReady():
-            (
-                self._header["tid"],
-                self._header["pid"],
-                self._header["len"],
-                self._header["uid"],
-            ) = struct.unpack(">HHHB", self._buffer[0 : self._hsize])
-
-            # someone sent us an error? ignore it
-            if self._header["len"] < 2:
-                self.advanceFrame()
-            # we have at least a complete message, continue
-            elif len(self._buffer) - self._hsize + 1 >= self._header["len"]:
-                return True
-        # we don't have enough of a message yet, wait
+        start = self._buffer.find(self._start)
+        if start == -1:
+            return False
+        if start > 0:  # go ahead and skip old bad data
+            self._buffer = self._buffer[start:]
+            start = 0
+
+        if (end := self._buffer.find(self._end)) != -1:
+            self._header["len"] = end
+            self._header["uid"] = int(self._buffer[1:3], 16)
+            self._header["lrc"] = int(self._buffer[end - 2 : end], 16)
+            data = a2b_hex(self._buffer[start + 1 : end - 2])
+            return checkLRC(data, self._header["lrc"])
         return False
 
     def advanceFrame(self):
         """Skip over the current framed message.
 
         This allows us to skip over the current message after we have processed
         it or determined that it contains an error. It also has to reset the
         current frame header handle
         """
-        length = self._hsize + self._header["len"] - 1
-        self._buffer = self._buffer[length:]
-        self._header = {"tid": 0, "pid": 0, "len": 0, "uid": 0}
+        self._buffer = self._buffer[self._header["len"] + 2 :]
+        self._header = {"lrc": "0000", "len": 0, "uid": 0x00}
 
     def isFrameReady(self):
         """Check if we should continue decode logic.
 
         This is meant to be used in a while loop in the decoding phase to let
-        the decoder factory know that there is still data in the buffer.
+        the decoder know that there is still data in the buffer.
 
         :returns: True if ready, False otherwise
         """
-        return len(self._buffer) > self._hsize
-
-    def addToFrame(self, message):
-        """Add new packet data to the current frame buffer.
-
-        :param message: The most recent packet
-        """
-        self._buffer += message
+        return len(self._buffer) > 1
 
     def getFrame(self):
-        """Return the next frame from the buffered data.
-
-        :returns: The next full frame buffer
-        """
-        length = self._hsize + self._header["len"] - 1
-        return self._buffer[self._hsize : length]
+        """Get the next frame from the buffer.
 
-    def populateResult(self, result):
-        """Populate the modbus result.
-
-        With the transport specific header
-        information (pid, tid, uid, checksum, etc)
-
-        :param result: The response packet
+        :returns: The frame data or ""
         """
-        result.transaction_id = self._header["tid"]
-        result.protocol_id = self._header["pid"]
-        result.slave_id = self._header["uid"]
+        start = self._hsize + 1
+        end = self._header["len"] - 2
+        buffer = self._buffer[start:end]
+        if end > 0:
+            return a2b_hex(buffer)
+        return b""
 
     # ----------------------------------------------------------------------- #
     # Public Member Functions
     # ----------------------------------------------------------------------- #
-    def decode_data(self, data):
-        """Decode data."""
-        if len(data) > self._hsize:
-            tid, pid, length, uid, fcode = struct.unpack(
-                SOCKET_FRAME_HEADER, data[0 : self._hsize + 1]
-            )
-            return {
-                "tid": tid,
-                "pid": pid,
-                "length": length,
-                "slave": uid,
-                "fcode": fcode,
-            }
-        return {}
-
-    def processIncomingPacket(self, data, callback, slave, tid: int = None, **kwargs):
-        """Process new packet pattern.
-
-        This takes in a new request packet, adds it to the current
-        packet stream, and performs framing on it. That is, checks
-        for complete messages, and once found, will process all that
-        exist.  This handles the case when we read N + 1 or 1 // N
-        messages at a time instead of 1.
-
-        The processed and decoded messages are pushed to the callback
-        function to process and send.
-        """
-        if not isinstance(slave, (list, tuple)):
-            slave = [slave]
-        single = kwargs.get("single", False)
-        Log.debug("Processing: {}", data, ":hex")
-        self.addToFrame(data)
-        while True:
-            if not self.isFrameReady():
-                if len(self._buffer):
-                    # Possible error ???
-                    if self._header["len"] < 2:
-                        self._process(callback, tid, error=True)
-                break
+    def frameProcessIncomingPacket(self, single, callback, slave, _tid=None, **kwargs):
+        """Process new packet pattern."""
+        while self.isFrameReady():
             if not self.checkFrame():
-                Log.debug("Frame check failed, ignoring!!")
-                self.resetFrame()
-                continue
+                break
             if not self._validate_slave_id(slave, single):
                 header_txt = self._header["uid"]
-                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
+                Log.error("Not a valid slave id - {}, ignoring!!", header_txt)
                 self.resetFrame()
                 continue
-            self._process(callback, tid)
 
-    def _process(self, callback, tid, error=False):
-        """Process incoming packets irrespective error condition."""
-        data = self.getRawFrame() if error else self.getFrame()
-        if (result := self.decoder.decode(data)) is None:
-            self.resetFrame()
-            raise ModbusIOException("Unable to decode request")
-        if error and result.function_code < 0x80:
-            raise InvalidMessageReceivedException(result)
-        self.populateResult(result)
-        self.advanceFrame()
-        if tid and tid != result.transaction_id:
-            self.resetFrame()
-        else:
-            callback(result)  # defer or push to a thread?
-
-    def resetFrame(self):
-        """Reset the entire message frame.
-
-        This allows us to skip ovver errors that may be in the stream.
-        It is hard to know if we are simply out of sync or if there is
-        an error in the stream as we have no way to check the start or
-        end of the message (python just doesn't have the resolution to
-        check for millisecond delays).
-        """
-        self._buffer = b""
-        self._header = {"tid": 0, "pid": 0, "len": 0, "uid": 0}
-
-    def getRawFrame(self):
-        """Return the complete buffer."""
-        return self._buffer
+            frame = self.getFrame()
+            if (result := self.decoder.decode(frame)) is None:
+                raise ModbusIOException("Unable to decode response")
+            self.populateResult(result)
+            self.advanceFrame()
+            callback(result)  # defer this
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
-        :param message: The populated request/response to send
+        Built off of a  modbus request/response
+
+        :param message: The request/response to send
+        :return: The encoded packet
         """
-        data = message.encode()
-        packet = struct.pack(
-            SOCKET_FRAME_HEADER,
-            message.transaction_id,
-            message.protocol_id,
-            len(data) + 2,
-            message.slave_id,
-            message.function_code,
+        encoded = message.encode()
+        buffer = struct.pack(
+            ASCII_FRAME_HEADER, message.slave_id, message.function_code
         )
-        packet += data
-        return packet
+        checksum = computeLRC(encoded + buffer)
+
+        packet = bytearray()
+        packet.extend(self._start)
+        packet.extend(f"{message.slave_id:02x}{message.function_code:02x}".encode())
+        packet.extend(b2a_hex(encoded))
+        packet.extend(f"{checksum:02x}".encode())
+        packet.extend(self._end)
+        return bytes(packet).upper()
 
 
 # __END__
```

### Comparing `pymodbus-3.3.2/pymodbus/framer/tls_framer.py` & `pymodbus-3.4.0/pymodbus/framer/tls_framer.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 
     def __init__(self, decoder, client=None):
         """Initialize a new instance of the framer.
 
         :param decoder: The decoder factory implementation to use
         """
         super().__init__(decoder, client)
-        self._buffer = b""
-        self._header = {}
         self._hsize = 0x0
 
     # ----------------------------------------------------------------------- #
     # Private Helper Functions
     # ----------------------------------------------------------------------- #
     def checkFrame(self):
         """Check and decode the next frame.
@@ -69,104 +67,56 @@
         This is meant to be used in a while loop in the decoding phase to let
         the decoder factory know that there is still data in the buffer.
 
         :returns: True if ready, False otherwise
         """
         return len(self._buffer) > self._hsize
 
-    def addToFrame(self, message):
-        """Add new packet data to the current frame buffer.
-
-        :param message: The most recent packet
-        """
-        self._buffer += message
-
     def getFrame(self):
         """Return the next frame from the buffered data.
 
         :returns: The next full frame buffer
         """
         return self._buffer[self._hsize :]
 
-    def populateResult(self, _result):
-        """Populate the modbus result."""
-        return
-
     # ----------------------------------------------------------------------- #
     # Public Member Functions
     # ----------------------------------------------------------------------- #
     def decode_data(self, data):
         """Decode data."""
         if len(data) > self._hsize:
             (fcode,) = struct.unpack(TLS_FRAME_HEADER, data[0 : self._hsize + 1])
             return {"fcode": fcode}
         return {}
 
-    def processIncomingPacket(self, data, callback, slave, **kwargs):
-        """Process new packet pattern.
-
-        This takes in a new request packet, adds it to the current
-        packet stream, and performs framing on it. That is, checks
-        for complete messages, and once found, will process all that
-        exist.  This handles the case when we read N + 1 or 1 // N
-        messages at a time instead of 1.
-
-        The processed and decoded messages are pushed to the callback
-        function to process and send.
-
-        :param data: The new packet data
-        :param callback: The function to send results to
-        :param slave: Process if slave id matcheks, ignore otherwise (could be a
-               list of slave ids (server) or single slave id(client/server)
-        :param kwargs:
-        """
-        if not isinstance(slave, (list, tuple)):
-            slave = [slave]
+    def frameProcessIncomingPacket(self, single, callback, slave, _tid=None, **kwargs):
+        """Process new packet pattern."""
         # no slave id for Modbus Security Application Protocol
-        single = kwargs.get("single", True)
-        Log.debug("Processing: {}", data, ":hex")
-        self.addToFrame(data)
-
         if not self.isFrameReady():
             return
         if not self.checkFrame():
             Log.debug("Frame check failed, ignoring!!")
             self.resetFrame()
             return
         if not self._validate_slave_id(slave, single):
             Log.debug("Not in valid slave id - {}, ignoring!!", slave)
             self.resetFrame()
         self._process(callback)
 
     def _process(self, callback, error=False):
         """Process incoming packets irrespective error condition."""
-        data = self.getRawFrame() if error else self.getFrame()
+        data = self._buffer if error else self.getFrame()
         if (result := self.decoder.decode(data)) is None:
             raise ModbusIOException("Unable to decode request")
         if error and result.function_code < 0x80:
             raise InvalidMessageReceivedException(result)
         self.populateResult(result)
         self.advanceFrame()
         callback(result)  # defer or push to a thread?
 
-    def resetFrame(self):
-        """Reset the entire message frame.
-
-        This allows us to skip ovver errors that may be in the stream.
-        It is hard to know if we are simply out of sync or if there is
-        an error in the stream as we have no way to check the start or
-        end of the message (python just doesn't have the resolution to
-        check for millisecond delays).
-        """
-        self._buffer = b""
-
-    def getRawFrame(self):
-        """Return the complete buffer."""
-        return self._buffer
-
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The populated request/response to send
         """
         data = message.encode()
         packet = struct.pack(TLS_FRAME_HEADER, message.function_code)
```

### Comparing `pymodbus-3.3.2/pymodbus/logging.py` & `pymodbus-3.4.0/pymodbus/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pymodbus.utilities import hexlify_packets
 
 
 # ---------------------------------------------------------------------------#
 #  Block unhandled logging
 # ---------------------------------------------------------------------------#
-logging.getLogger(__name__).addHandler(__null())
+logging.getLogger("pymodbus_internal").addHandler(__null())
 
 
 def pymodbus_apply_logging_config(
     level: Union[str, int] = logging.DEBUG, log_file_name: str = None
 ):
     """Apply basic logging configuration used by default by Pymodbus maintainers.
```

### Comparing `pymodbus-3.3.2/pymodbus/mei_message.py` & `pymodbus-3.4.0/pymodbus/mei_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/other_message.py` & `pymodbus-3.4.0/pymodbus/other_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "ReportSlaveIdRequest",
     "ReportSlaveIdResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
-from pymodbus.constants import Defaults, ModbusStatus
+from pymodbus.constants import ModbusStatus
 from pymodbus.device import DeviceInformationFactory, ModbusControlBlock
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 
 
 _MCB = ModbusControlBlock()
 
 
@@ -84,15 +84,15 @@
 
     def __init__(self, status=0x00, **kwargs):
         """Initialize a new instance.
 
         :param status: The status response to report
         """
         ModbusResponse.__init__(self, **kwargs)
-        self.status = status
+        self.status = status if status < 256 else 255
 
     def encode(self):
         """Encode the response.
 
         :returns: The byte encoded message
         """
         return struct.pack(">B", self.status)
@@ -373,15 +373,15 @@
     The current status, and other information specific to a remote device.
     """
 
     function_code = 0x11
     function_code_name = "report_slave_id"
     _rtu_frame_size = 4
 
-    def __init__(self, slave=Defaults.Slave, **kwargs):
+    def __init__(self, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param slave: Modbus slave slave ID
 
         """
         ModbusRequest.__init__(self, slave, **kwargs)
```

### Comparing `pymodbus-3.3.2/pymodbus/payload.py` & `pymodbus-3.4.0/pymodbus/payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/pdu.py` & `pymodbus-3.4.0/pymodbus/pdu.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     "ExceptionResponse",
     "IllegalFunctionRequest",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
-from pymodbus.constants import Defaults
 from pymodbus.exceptions import NotImplementedException
 from pymodbus.logging import Log
 from pymodbus.utilities import rtuFrameSize
 
 
 # --------------------------------------------------------------------------- #
 # Base PDUs
@@ -50,22 +49,22 @@
        This is used when the message payload has already been encoded.
        Generally this will occur when the PayloadBuilder is being used
        to create a complicated message. By setting this to True, the
        request will pass the currently encoded message through instead
        of encoding it again.
     """
 
-    def __init__(self, slave=Defaults.Slave, **kwargs):
+    def __init__(self, slave=0, **kwargs):
         """Initialize the base data for a modbus request.
 
         :param slave: Modbus slave slave ID
 
         """
-        self.transaction_id = kwargs.get("transaction", Defaults.TransactionId)
-        self.protocol_id = kwargs.get("protocol", Defaults.ProtocolId)
+        self.transaction_id = kwargs.get("transaction", 0)
+        self.protocol_id = kwargs.get("protocol", 0)
         self.slave_id = slave
         self.skip_encode = kwargs.get("skip_encode", False)
         self.check = 0x0000
 
     def encode(self):
         """Encode the message.
 
@@ -99,15 +98,15 @@
 
 
 class ModbusRequest(ModbusPDU):
     """Base class for a modbus request PDU."""
 
     function_code = -1
 
-    def __init__(self, slave=Defaults.Slave, **kwargs):
+    def __init__(self, slave=0, **kwargs):  # pylint: disable=useless-parent-delegation
         """Proxy to the lower level initializer.
 
         :param slave: Modbus slave slave ID
         """
         super().__init__(slave, **kwargs)
 
     def doException(self, exception):
@@ -133,15 +132,15 @@
 
        Indicates the size of the modbus rtu response used for
        calculating how much to read.
     """
 
     should_respond = True
 
-    def __init__(self, slave=Defaults.Slave, **kwargs):
+    def __init__(self, slave=0, **kwargs):
         """Proxy the lower level initializer.
 
         :param slave: Modbus slave slave ID
 
         """
         super().__init__(slave, **kwargs)
         self.bits = []
```

### Comparing `pymodbus-3.3.2/pymodbus/register_read_message.py` & `pymodbus-3.4.0/pymodbus/register_read_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,24 @@
     "ReadWriteMultipleRegistersRequest",
     "ReadWriteMultipleRegistersResponse",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
 
-from pymodbus.constants import Defaults
 from pymodbus.pdu import ExceptionResponse, ModbusRequest, ModbusResponse
 from pymodbus.pdu import ModbusExceptions as merror
 
 
 class ReadRegistersRequestBase(ModbusRequest):
     """Base class for reading a modbus register."""
 
     _rtu_frame_size = 8
 
-    def __init__(self, address, count, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address, count, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param address: The address to start the read from
         :param count: The number of registers to read
         :param slave: Modbus slave slave ID
         """
         super().__init__(slave, **kwargs)
@@ -67,15 +66,15 @@
     """Base class for responding to a modbus register read.
 
     The requested registers can be found in the .registers list.
     """
 
     _rtu_byte_count_pos = 2
 
-    def __init__(self, values, slave=Defaults.Slave, **kwargs):
+    def __init__(self, values, slave=0, **kwargs):
         """Initialize a new instance.
 
         :param values: The values to write to
         :param slave: Modbus slave slave ID
         """
         super().__init__(slave, **kwargs)
 
@@ -127,15 +126,15 @@
     Registers are addressed starting at zero. Therefore registers numbered
     1-16 are addressed as 0-15.
     """
 
     function_code = 3
     function_code_name = "read_holding_registers"
 
-    def __init__(self, address=None, count=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address=None, count=None, slave=0, **kwargs):
         """Initialize a new instance of the request.
 
         :param address: The starting address to read from
         :param count: The number of registers to read from address
         :param slave: Modbus slave slave ID
         """
         super().__init__(address, count, slave, **kwargs)
@@ -188,15 +187,15 @@
     Registers are addressed starting at zero. Therefore input registers
     numbered 1-16 are addressed as 0-15.
     """
 
     function_code = 4
     function_code_name = "read_input_registers"
 
-    def __init__(self, address=None, count=None, slave=Defaults.Slave, **kwargs):
+    def __init__(self, address=None, count=None, slave=0, **kwargs):
         """Initialize a new instance of the request.
 
         :param address: The starting address to read from
         :param count: The number of registers to read from address
         :param slave: Modbus slave slave ID
         """
         super().__init__(address, count, slave, **kwargs)
```

### Comparing `pymodbus-3.3.2/pymodbus/register_write_message.py` & `pymodbus-3.4.0/pymodbus/register_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/repl/client/completer.py` & `pymodbus-3.4.0/pymodbus/repl/client/completer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/repl/client/helper.py` & `pymodbus-3.4.0/pymodbus/repl/client/helper.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/repl/client/main.py` & `pymodbus-3.4.0/pymodbus/repl/client/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -332,23 +332,23 @@
     "--port",
     default=None,
     type=str,
     help="Modbus RTU port",
 )
 @click.option(
     "--baudrate",
-    help="Modbus RTU serial baudrate to use. Defaults to 9600",
+    help="Modbus RTU serial baudrate to use.",
     default=9600,
     type=int,
 )
 @click.option(
     "--bytesize",
     help="Modbus RTU serial Number of data bits. "
     "Possible values: FIVEBITS, SIXBITS, SEVENBITS, "
-    "EIGHTBITS. Defaults to 8",
+    "EIGHTBITS.",
     type=NumericChoice(["5", "6", "7", "8"], int),
     default="8",
 )
 @click.option(
     "--parity",
     help="Modbus RTU serial parity. "
     " Enable parity checking. Possible values: "
@@ -363,41 +363,39 @@
     "Number of stop bits. Possible values: STOPBITS_ONE, "
     'STOPBITS_ONE_POINT_FIVE, STOPBITS_TWO. Default to "1"',
     default="1",
     type=NumericChoice(["1", "1.5", "2"], float),
 )
 @click.option(
     "--xonxoff",
-    help="Modbus RTU serial xonxoff.  Enable software flow control. Defaults to 0",
+    help="Modbus RTU serial xonxoff.  Enable software flow control.",
     default=0,
     type=int,
 )
 @click.option(
     "--rtscts",
-    help="Modbus RTU serial rtscts. Enable hardware (RTS/CTS) flow "
-    "control. Defaults to 0",
+    help="Modbus RTU serial rtscts. Enable hardware (RTS/CTS) flow " "control.",
     default=0,
     type=int,
 )
 @click.option(
     "--dsrdtr",
-    help="Modbus RTU serial dsrdtr. Enable hardware (DSR/DTR) flow "
-    "control. Defaults to 0",
+    help="Modbus RTU serial dsrdtr. Enable hardware (DSR/DTR) flow " "control.",
     default=0,
     type=int,
 )
 @click.option(
     "--timeout",
-    help="Modbus RTU serial read timeout. Defaults to 0.025 sec",
+    help="Modbus RTU serial read timeout.",
     default=0.25,
     type=float,
 )
 @click.option(
     "--write-timeout",
-    help="Modbus RTU serial write timeout. Defaults to 2 sec",
+    help="Modbus RTU serial write timeout.",
     default=2,
     type=float,
 )
 def serial(  # pylint: disable=too-many-arguments
     ctx,
     method,
     port,
```

### Comparing `pymodbus-3.3.2/pymodbus/repl/client/mclient.py` & `pymodbus-3.4.0/pymodbus/repl/client/mclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Modbus Clients to be used with REPL."""
 # pylint: disable=missing-type-doc
 import functools
 
 from pymodbus.client import ModbusSerialClient as _ModbusSerialClient
 from pymodbus.client import ModbusTcpClient as _ModbusTcpClient
-from pymodbus.constants import Defaults
 from pymodbus.diag_message import (
     ChangeAsciiInputDelimiterRequest,
     ClearCountersRequest,
     ClearOverrunCountRequest,
     ForceListenOnlyModeRequest,
     GetClearModbusPlusRequest,
     RestartCommunicationsOptionRequest,
@@ -86,15 +85,15 @@
                     "original_function_code": f"{resp.fcode} ({hex(resp.fcode)})",
                     "error": resp.message,
                 }
             else:
                 err = {"error": str(resp)}
         return err
 
-    def read_coils(self, address, count=1, slave=Defaults.Slave, **kwargs):
+    def read_coils(self, address, count=1, slave=0, **kwargs):
         """Read `count` coils from a given slave starting at `address`.
 
         :param address: The starting address to read from
         :param count: The number of coils to read
         :param slave: Modbus slave slave ID
         :param kwargs:
         :returns: List of register values
@@ -102,15 +101,15 @@
         resp = super().read_coils(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "bits": resp.bits}
         return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
-    def read_discrete_inputs(self, address, count=1, slave=Defaults.Slave, **kwargs):
+    def read_discrete_inputs(self, address, count=1, slave=0, **kwargs):
         """Read `count` number of discrete inputs starting at offset `address`.
 
         :param address: The starting address to read from
         :param count: The number of coils to read
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return: List of bits
@@ -119,74 +118,74 @@
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "bits": resp.bits}
         return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     @handle_brodcast
-    def write_coil(self, address, value, slave=Defaults.Slave, **kwargs):
+    def write_coil(self, address, value, slave=0, **kwargs):
         """Write `value` to coil at `address`.
 
         :param address: coil offset to write to
         :param value: bit value to write
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
         """
         resp = super().write_coil(  # pylint: disable=no-member
             address, value, slave, **kwargs
         )
         return resp
 
     @handle_brodcast
-    def write_coils(self, address, values, slave=Defaults.Slave, **kwargs):
+    def write_coils(self, address, values, slave=0, **kwargs):
         """Write `value` to coil at `address`.
 
         :param address: coil offset to write to
         :param values: list of bit values to write (comma separated)
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
         """
         resp = super().write_coils(  # pylint: disable=no-member
             address, values, slave, **kwargs
         )
         return resp
 
     @handle_brodcast
-    def write_register(self, address, value, slave=Defaults.Slave, **kwargs):
+    def write_register(self, address, value, slave=0, **kwargs):
         """Write `value` to register at `address`.
 
         :param address: register offset to write to
         :param value: register value to write
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
         """
         resp = super().write_register(  # pylint: disable=no-member
             address, value, slave, **kwargs
         )
         return resp
 
     @handle_brodcast
-    def write_registers(self, address, values, slave=Defaults.Slave, **kwargs):
+    def write_registers(self, address, values, slave=0, **kwargs):
         """Write list of `values` to registers starting at `address`.
 
         :param address: register offset to write to
         :param values: list of register value to write (comma separated)
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
         """
         resp = super().write_registers(  # pylint: disable=no-member
             address, values, slave, **kwargs
         )
         return resp
 
-    def read_holding_registers(self, address, count=1, slave=Defaults.Slave, **kwargs):
+    def read_holding_registers(self, address, count=1, slave=0, **kwargs):
         """Read `count` number of holding registers starting at `address`.
 
         :param address: starting register offset to read from
         :param count: Number of registers to read
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
@@ -194,15 +193,15 @@
         resp = super().read_holding_registers(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "registers": resp.registers}
         return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
-    def read_input_registers(self, address, count=1, slave=Defaults.Slave, **kwargs):
+    def read_input_registers(self, address, count=1, slave=0, **kwargs):
         """Read `count` number of input registers starting at `address`.
 
         :param address: starting register offset to read from to
         :param count: Number of registers to read
         :param slave: Modbus slave slave ID
         :param kwargs:
         :return:
@@ -216,15 +215,15 @@
 
     def readwrite_registers(
         self,
         read_address=0,
         read_count=0,
         write_address=0,
         values=0,
-        slave=Defaults.Slave,
+        slave=0,
         **kwargs,
     ):
         """Read `read_count` number of holding registers.
 
         Starting at `read_address`
         and write `write_registers` starting at `write_address`.
 
@@ -249,15 +248,15 @@
         return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def mask_write_register(
         self,
         address=0x0000,
         and_mask=0xFFFF,
         or_mask=0x0000,
-        slave=Defaults.Slave,
+        slave=0,
         **kwargs,
     ):
         """Mask content of holding register at `address` with `and_mask` and `or_mask`.
 
         :param address: Reference address of register
         :param and_mask: And Mask
         :param or_mask: OR Mask
@@ -295,15 +294,15 @@
                 "conformity": resp.conformity,
                 "next object id": resp.next_object_id,
                 "more follows": resp.more_follows,
                 "space left": resp.space_left,
             }
         return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
-    def report_slave_id(self, slave=Defaults.Slave, **kwargs):
+    def report_slave_id(self, slave=0, **kwargs):
         """Report information about remote slave ID.
 
         :param slave: Modbus slave ID
         :param kwargs:
         :return:
         """
         request = ReportSlaveIdRequest(slave, **kwargs)
@@ -313,15 +312,15 @@
                 "function_code": resp.function_code,
                 "identifier": resp.identifier.decode("cp1252"),
                 "status": resp.status,
                 "byte count": resp.byte_count,
             }
         return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
-    def read_exception_status(self, slave=Defaults.Slave, **kwargs):
+    def read_exception_status(self, slave=0, **kwargs):
         """Read contents of eight Exception Status output in a remote device.
 
         :param slave: Modbus slave ID
         :param kwargs:
         :return:
         """
         request = ReadExceptionStatusRequest(slave, **kwargs)
@@ -563,22 +562,22 @@
         super().__init__(framer=framer, **kwargs)
 
     def get_port(self):
         """Get serial Port.
 
         :return: Current Serial port
         """
-        return self.params.port
+        return self.comm_params.port
 
     def set_port(self, value):
         """Set serial Port setter.
 
         :param value: New port
         """
-        self.params.port = value
+        self.comm_params.port = value
         if self.is_socket_open():
             self.close()
 
     def get_stopbits(self):
         """Get number of stop bits.
 
         :return: Current Stop bits
@@ -595,23 +594,23 @@
             self.close()
 
     def get_bytesize(self):
         """Get number of data bits.
 
         :return: Current bytesize
         """
-        return self.params.bytesize
+        return self.comm_params.bytesize
 
     def set_bytesize(self, value):
         """Set Byte size.
 
         :param value: Possible values (5, 6, 7, 8)
 
         """
-        self.params.bytesize = int(value)
+        self.comm_params.bytesize = int(value)
         if self.is_socket_open():
             self.close()
 
     def get_parity(self):
         """Enable Parity Checking.
 
         :return: Current parity setting
@@ -628,53 +627,53 @@
             self.close()
 
     def get_baudrate(self):
         """Get serial Port baudrate.
 
         :return: Current baudrate
         """
-        return self.params.baudrate
+        return self.comm_params.baudrate
 
     def set_baudrate(self, value):
         """Set baudrate setter.
 
         :param value: <supported baudrate>
         """
-        self.params.baudrate = int(value)
+        self.comm_params.baudrate = int(value)
         if self.is_socket_open():
             self.close()
 
     def get_timeout(self):
         """Get serial Port Read timeout.
 
         :return: Current read imeout.
         """
-        return self.params.timeout
+        return self.comm_params.timeout_connect
 
     def set_timeout(self, value):
         """Read timeout setter.
 
         :param value: Read Timeout in seconds
         """
-        self.params.timeout = float(value)
+        self.comm_params.timeout_connect = float(value)
         if self.is_socket_open():
             self.close()
 
     def get_serial_settings(self):
         """Get Current Serial port settings.
 
         :return: Current Serial settings as dict.
         """
         return {
-            "baudrate": self.params.baudrate,
-            "port": self.params.port,
-            "parity": self.params.parity,
-            "stopbits": self.params.stopbits,
-            "bytesize": self.params.bytesize,
-            "read timeout": self.params.timeout,
+            "baudrate": self.comm_params.baudrate,
+            "port": self.comm_params.port,
+            "parity": self.comm_params.parity,
+            "stopbits": self.comm_params.stopbits,
+            "bytesize": self.comm_params.bytesize,
+            "read timeout": self.comm_params.timeout_connect,
             "t1.5": self.inter_char_timeout,
             "t3.5": self.silent_interval,
         }
 
 
 class ModbusTcpClient(ExtendedRequestSupport, _ModbusTcpClient):
     """TCP client."""
```

### Comparing `pymodbus-3.3.2/pymodbus/repl/server/cli.py` & `pymodbus-3.4.0/pymodbus/repl/server/cli.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/repl/server/main.py` & `pymodbus-3.4.0/pymodbus/repl/server/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/__init__.py` & `pymodbus-3.4.0/pymodbus/server/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 """Server.
 
 import external classes, to make them easier to use:
 """
 
 __all__ = [
+    "get_simulator_commandline",
     "ModbusSerialServer",
     "ModbusSimulatorServer",
     "ModbusTcpServer",
     "ModbusTlsServer",
     "ModbusUdpServer",
-    "ModbusUnixServer",
     "ServerAsyncStop",
     "ServerStop",
     "StartAsyncSerialServer",
     "StartAsyncTcpServer",
     "StartAsyncTlsServer",
     "StartAsyncUdpServer",
-    "StartAsyncUnixServer",
     "StartSerialServer",
     "StartTcpServer",
     "StartTlsServer",
     "StartUdpServer",
 ]
 
 from pymodbus.server.async_io import (
     ModbusSerialServer,
     ModbusTcpServer,
     ModbusTlsServer,
     ModbusUdpServer,
-    ModbusUnixServer,
     ServerAsyncStop,
     ServerStop,
     StartAsyncSerialServer,
     StartAsyncTcpServer,
     StartAsyncTlsServer,
     StartAsyncUdpServer,
-    StartAsyncUnixServer,
     StartSerialServer,
     StartTcpServer,
     StartTlsServer,
     StartUdpServer,
 )
 from pymodbus.server.simulator.http_server import ModbusSimulatorServer
+from pymodbus.server.simulator.main import get_commandline as get_simulator_commandline
```

### Comparing `pymodbus-3.3.2/pymodbus/server/reactive/default_config.py` & `pymodbus-3.4.0/pymodbus/server/reactive/default_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 """Configuration for Pymodbus REPL Reactive Module."""
 
 DEFAULT_CONFIG = {
     "tcp": {
         "handler": "ModbusConnectedRequestHandler",
-        "allow_reuse_address": True,
         "allow_reuse_port": True,
-        "backlog": 20,
         "ignore_missing_slaves": False,
     },
     "serial": {
         "handler": "ModbusSingleRequestHandler",
         "stopbits": 1,
         "bytesize": 8,
         "parity": "N",
         "baudrate": 9600,
         "timeout": 3,
-        "auto_reconnect": False,
         "reconnect_delay": 2,
     },
     "tls": {
         "handler": "ModbusConnectedRequestHandler",
         "certfile": None,
         "keyfile": None,
-        "allow_reuse_address": True,
         "allow_reuse_port": True,
-        "backlog": 20,
         "ignore_missing_slaves": False,
     },
     "udp": {
         "handler": "ModbusDisonnectedRequestHandler",
         "ignore_missing_slaves": False,
     },
     "data_block_settings": {
```

### Comparing `pymodbus-3.3.2/pymodbus/server/reactive/main.py` & `pymodbus-3.4.0/pymodbus/server/reactive/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,16 @@
     ModbusSequentialDataBlock,
     ModbusSparseDataBlock,
 )
 from pymodbus.device import ModbusDeviceIdentification
 from pymodbus.logging import Log
 from pymodbus.pdu import ExceptionResponse, ModbusExceptions
 from pymodbus.server.async_io import (
-    ModbusConnectedRequestHandler,
-    ModbusDisconnectedRequestHandler,
     ModbusSerialServer,
-    ModbusSingleRequestHandler,
+    ModbusServerRequestHandler,
     ModbusTcpServer,
     ModbusTlsServer,
     ModbusUdpServer,
 )
 from pymodbus.transaction import (
     ModbusAsciiFramer,
     ModbusBinaryFramer,
@@ -68,17 +66,17 @@
 DEFAULT_MANIPULATOR = {
     "response_type": "normal",  # normal, error, delayed, empty
     "delay_by": 0,
     "error_code": ModbusExceptions.IllegalAddress,
     "clear_after": 5,  # request count
 }
 DEFUALT_HANDLERS = {
-    "ModbusSingleRequestHandler": ModbusSingleRequestHandler,
-    "ModbusConnectedRequestHandler": ModbusConnectedRequestHandler,
-    "ModbusDisconnectedRequestHandler": ModbusDisconnectedRequestHandler,
+    "ModbusSingleRequestHandler": ModbusServerRequestHandler,
+    "ModbusConnectedRequestHandler": ModbusServerRequestHandler,
+    "ModbusDisconnectedRequestHandler": ModbusServerRequestHandler,
 }
 DEFAULT_MODBUS_MAP = {
     "block_start": 0,
     "block_size": 100,
     "default": 0,
     "sparse": False,
 }
```

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/http_server.py` & `pymodbus-3.4.0/pymodbus/server/simulator/http_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 try:
     from aiohttp import web
 except ImportError:
     web = None
 
+import contextlib
+
 from pymodbus.datastore import ModbusServerContext, ModbusSimulatorContext
 from pymodbus.datastore.simulator import Label
 from pymodbus.device import ModbusDeviceIdentification
 from pymodbus.factory import ServerDecoder
 from pymodbus.logging import Log
 from pymodbus.pdu import ExceptionResponse
 from pymodbus.server import (
@@ -81,16 +83,16 @@
 
 
 class ModbusSimulatorServer:
     """**ModbusSimulatorServer**.
 
     :param modbus_server: Server name in json file (default: "server")
     :param modbus_device: Device name in json file (default: "client")
-    :param http_host: TCP host for HTTP (default: 8080)
-    :param http_port: TCP port for HTTP (default: "localhost")
+    :param http_host: TCP host for HTTP (default: "localhost")
+    :param http_port: TCP port for HTTP (default: 8080)
     :param json_file: setup file (default: "setup.json")
     :param custom_actions_module: python module with custom actions (default: none)
 
     if either http_port or http_host is none, HTTP will not be started.
     This class starts a http server, that serves a couple of endpoints:
 
     - **"<addr>/"** static files
@@ -145,15 +147,14 @@
         }
         if custom_actions_module:
             actions_module = importlib.import_module(custom_actions_module)
             custom_actions_dict = actions_module.custom_actions_dict
         else:
             custom_actions_dict = None
         server = setup["server_list"][modbus_server]
-        server["loop"] = asyncio.get_running_loop()
         if server["comm"] != "serial":
             server["address"] = (server["host"], server["port"])
             del server["host"]
             del server["port"]
         device = setup["device_list"][modbus_device]
         self.datastore_context = ModbusSimulatorContext(
             device, custom_actions_dict or None
@@ -222,41 +223,48 @@
                 await self.modbus_server.start()
             app["modbus_server"] = asyncio.create_task(
                 self.modbus_server.serve_forever()
             )
         except Exception as exc:
             Log.error("Error starting modbus server, reason: {}", exc)
             raise exc
-        Log.info("Modbus server started")
+        Log.info(
+            "Modbus server started on {}", self.modbus_server.comm_params.source_address
+        )
 
     async def stop_modbus_server(self, app):
         """Stop modbus server."""
         Log.info("Stopping modbus server")
         app["modbus_server"].cancel()
-        await app["modbus_server"]
+        with contextlib.suppress(asyncio.exceptions.CancelledError):
+            await app["modbus_server"]
+
         Log.info("Modbus server Stopped")
 
-    async def run_forever(self):
+    async def run_forever(self, only_start=False):
         """Start modbus and http servers."""
         try:
             runner = web.AppRunner(self.web_app)
             await runner.setup()
             self.site = web.TCPSite(runner, self.http_host, self.http_port)
             await self.site.start()
         except Exception as exc:
             Log.error("Error starting http server, reason: {}", exc)
             raise exc
-        Log.info("HTTP server started")
+        Log.info("HTTP server started on ({}:{})", self.http_host, self.http_port)
+        if only_start:
+            return
         while True:
             await asyncio.sleep(1)
 
     async def stop(self):
         """Stop modbus and http servers."""
-        self.site.stop()
+        await self.site.stop()
         self.site = None
+        await asyncio.sleep(1)
 
     async def handle_html_static(self, request):
         """Handle static html."""
         if not (page := request.path[1:]):
             page = "index.html"
         file = os.path.join(self.web_path, page)
         try:
```

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/main.py` & `pymodbus-3.4.0/pymodbus/server/simulator/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 import os
 
 from pymodbus import pymodbus_apply_logging_config
 from pymodbus.logging import Log
 from pymodbus.server.simulator.http_server import ModbusSimulatorServer
 
 
-def get_commandline():
+def get_commandline(extras=None, cmdline=None):
     """Get command line arguments."""
     parser = argparse.ArgumentParser(
         description="Modbus server with REST-API and web server"
     )
     parser.add_argument(
         "--modbus_server",
         help="use <modbus_server> from server_list in json file",
@@ -93,15 +93,18 @@
         type=str,
     )
     parser.add_argument(
         "--custom_actions_module",
         help="python file with custom actions, default is none",
         type=str,
     )
-    args = parser.parse_args()
+    if extras:
+        for extra in extras:
+            parser.add_argument(extra[0], **extra[1])
+    args = parser.parse_args(cmdline)
     pymodbus_apply_logging_config(args.log.upper())
     Log.info("Start simulator")
     cmd_args = {}
     for argument in args.__dict__:
         if argument == "log":
             continue
         if args.__dict__[argument] is not None:
```

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/setup.json` & `pymodbus-3.4.0/pymodbus/server/simulator/setup.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767074647210643%*

 * *Differences: {"'device_list'": "{'device_try': {'setup': {'defaults': {'action': {'uint16': None, 'uint32': "*

 * *                  "None, 'float32': None}}}, 'write': {delete: [1]}, 'uint16': {5: {'addr': "*

 * *                  "{insert: [(1, 2304)], delete: [1]}, 'action': 'increment'}, insert: [(6, "*

 * *                  "OrderedDict([('addr', 2305), ('value', 50), ('action', 'increment'), ('kwargs', "*

 * *                  "OrderedDict([('minval', 45), ('maxval', 155)]))])), (7, OrderedDict([('addr', "*

 * *                  "2306), ( […]*

```diff
@@ -132,70 +132,73 @@
                     "value": 1
                 },
                 {
                     "addr": [
                         4188,
                         4191
                     ],
-                    "value": 32514.1
+                    "value": 32514.2
                 },
                 {
                     "action": null,
                     "addr": [
                         4308,
                         4407
                     ]
                 },
                 {
                     "action": "increment",
                     "addr": [
                         4688,
-                        4879
+                        4875
                     ],
                     "value": 115.7
-                }
-            ],
-            "invalid": [
-                [
-                    0,
-                    5
-                ],
-                77
-            ],
-            "repeat": [
+                },
                 {
+                    "action": "increment",
                     "addr": [
-                        0,
-                        999
+                        4876,
+                        4877
                     ],
-                    "to": [
-                        10000,
-                        10999
-                    ]
+                    "kwargs": {
+                        "maxval": 55000.0,
+                        "minval": 45000.0
+                    },
+                    "value": 50000.0
                 },
                 {
+                    "action": "random",
                     "addr": [
-                        10,
-                        1999
+                        4878,
+                        48779
                     ],
-                    "to": [
-                        11000,
-                        11999
-                    ]
+                    "kwargs": {
+                        "maxval": 55000.0,
+                        "minval": 45000.0
+                    },
+                    "value": 50000.0
                 }
             ],
+            "invalid": [
+                [
+                    0,
+                    5
+                ],
+                77
+            ],
+            "repeat": [],
             "setup": {
                 "co size": 63000,
                 "defaults": {
                     "action": {
                         "bits": null,
-                        "float32": "register",
+                        "float32": null,
                         "string": null,
-                        "uint16": "register",
-                        "uint32": "register"
+                        "uint16": null,
+                        "uint32": null
                     },
                     "value": {
                         "bits": 0,
                         "float32": 0.0,
                         "string": " ",
                         "uint16": 0,
                         "uint32": 0
@@ -211,19 +214,14 @@
                 {
                     "addr": [
                         16,
                         20
                     ],
                     "value": "A_B_C_D_E_"
                 },
-                5047,
-                [
-                    5146,
-                    5149
-                ],
                 {
                     "addr": [
                         529,
                         544
                     ],
                     "value": "Brand name, 32 bytes...........X"
                 }
@@ -243,19 +241,37 @@
                     "addr": [
                         2168,
                         2169
                     ],
                     "value": 32117
                 },
                 {
-                    "action": null,
+                    "action": "increment",
                     "addr": [
                         2208,
-                        2306
+                        2304
                     ]
+                },
+                {
+                    "action": "increment",
+                    "addr": 2305,
+                    "kwargs": {
+                        "maxval": 155,
+                        "minval": 45
+                    },
+                    "value": 50
+                },
+                {
+                    "action": "random",
+                    "addr": 2306,
+                    "kwargs": {
+                        "maxval": 55,
+                        "minval": 45
+                    },
+                    "value": 50
                 }
             ],
             "uint32": [
                 [
                     12,
                     13
                 ],
@@ -288,31 +304,50 @@
                         3407
                     ]
                 },
                 {
                     "action": "increment",
                     "addr": [
                         3688,
-                        3879
+                        3875
                     ],
                     "value": 115
+                },
+                {
+                    "action": "increment",
+                    "addr": [
+                        3876,
+                        3877
+                    ],
+                    "kwargs": {
+                        "maxval": 55000,
+                        "minval": 45000
+                    },
+                    "value": 50000
+                },
+                {
+                    "action": "random",
+                    "addr": [
+                        3878,
+                        3879
+                    ],
+                    "kwargs": {
+                        "maxval": 55000,
+                        "minval": 45000
+                    },
+                    "value": 50000
                 }
             ],
             "write": [
-                10,
-                [
-                    61,
-                    76
-                ]
+                10
             ]
         }
     },
     "server_list": {
         "server": {
-            "allow_reuse_address": true,
             "comm": "tcp",
             "framer": "socket",
             "host": "0.0.0.0",
             "identity": {
                 "MajorMinorRevision": "3.1.0",
                 "ModelName": "pymodbus Server",
                 "ProductCode": "PM",
@@ -335,15 +370,14 @@
                 "VendorName": "pymodbus",
                 "VendorUrl": "https://github.com/pymodbus-dev/pymodbus/"
             },
             "ignore_missing_slaves": false,
             "port": 5020
         },
         "server_try_serial": {
-            "auto_reconnect": false,
             "baudrate": 9600,
             "bytesize": 8,
             "comm": "serial",
             "framer": "rtu",
             "identity": {
                 "MajorMinorRevision": "3.1.0",
                 "ModelName": "pymodbus Server",
@@ -355,16 +389,14 @@
             "parity": "N",
             "port": "/dev/tty0",
             "reconnect_delay": 2,
             "stopbits": 1,
             "timeout": 3
         },
         "server_try_tls": {
-            "allow_reuse_address": true,
-            "backlog": 20,
             "certfile": "certificates/pymodbus.crt",
             "comm": "tls",
             "framer": "tls",
             "host": "0.0.0.0",
             "identity": {
                 "MajorMinorRevision": "3.1.0",
                 "ModelName": "pymodbus Server",
```

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/apple120.png` & `pymodbus-3.4.0/pymodbus/server/simulator/web/apple120.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/apple152.png` & `pymodbus-3.4.0/pymodbus/server/simulator/web/apple152.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/apple60.png` & `pymodbus-3.4.0/pymodbus/server/simulator/web/apple60.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/apple76.png` & `pymodbus-3.4.0/pymodbus/server/simulator/web/apple76.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/favicon.ico` & `pymodbus-3.4.0/pymodbus/server/simulator/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/calls` & `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/calls`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/log` & `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/log`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png` & `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/registers` & `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/registers`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/generator/server` & `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/server`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/index.html` & `pymodbus-3.4.0/pymodbus/server/simulator/web/index.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/pymodbus.css` & `pymodbus-3.4.0/pymodbus/server/simulator/web/pymodbus.css`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/server/simulator/web/welcome.html` & `pymodbus-3.4.0/pymodbus/server/simulator/web/welcome.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus/transaction.py` & `pymodbus-3.4.0/pymodbus/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # pylint: disable=missing-type-doc
 import struct
 import time
 from contextlib import suppress
 from functools import partial
 from threading import RLock
 
-from pymodbus.constants import Defaults
 from pymodbus.exceptions import (
     InvalidMessageReceivedException,
     ModbusIOException,
     NotImplementedException,
 )
 from pymodbus.framer.ascii_framer import ModbusAsciiFramer
 from pymodbus.framer.binary_framer import ModbusBinaryFramer
@@ -54,20 +53,20 @@
     def __init__(self, client, **kwargs):
         """Initialize an instance of the ModbusTransactionManager.
 
         :param client: The client socket wrapper
         :param retry_on_empty: Should the client retry on empty
         :param retries: The number of retries to allow
         """
-        self.tid = Defaults.TransactionId
+        self.tid = 0
         self.client = client
-        self.backoff = kwargs.get("backoff", Defaults.Backoff) or 0.3
-        self.retry_on_empty = kwargs.get("retry_on_empty", Defaults.RetryOnEmpty)
-        self.retry_on_invalid = kwargs.get("retry_on_invalid", Defaults.RetryOnInvalid)
-        self.retries = kwargs.get("retries", Defaults.Retries) or 1
+        self.backoff = kwargs.get("backoff", 0.3)
+        self.retry_on_empty = kwargs.get("retry_on_empty", False)
+        self.retry_on_invalid = kwargs.get("retry_on_invalid", False)
+        self.retries = kwargs.get("retries", 3)
         self.reset_socket = kwargs.get("reset_socket", True)
         self._transaction_lock = RLock()
         self._no_response_devices = []
         if client:
             self._set_adu_size()
 
     def _set_adu_size(self):
@@ -162,15 +161,15 @@
                         full = True
                     else:
                         full = False
                     c_str = str(self.client)
                     if "modbusudpclient" in c_str.lower().strip():
                         full = True
                         if not expected_response_length:
-                            expected_response_length = Defaults.ReadSize
+                            expected_response_length = 1024
                     response, last_exception = self._transact(
                         request,
                         expected_response_length,
                         full=full,
                         broadcast=broadcast,
                     )
                     while retries > 0:
@@ -459,15 +458,15 @@
         :returns: The next unique transaction identifier
         """
         self.tid = (self.tid + 1) & 0xFFFF
         return self.tid
 
     def reset(self):
         """Reset the transaction identifier."""
-        self.tid = Defaults.TransactionId
+        self.tid = 0
         self.transactions = type(  # pylint: disable=attribute-defined-outside-init
             self.transactions
         )()
 
 
 class DictTransactionManager(ModbusTransactionManager):
     """Implements a transaction for a manager.
```

### Comparing `pymodbus-3.3.2/pymodbus/transport/serial_asyncio/__init__.py` & `pymodbus-3.4.0/pymodbus/transport/serial_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.4.0/pymodbus.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -91,16 +91,14 @@
 test/test_bit_write_messages.py
 test/test_client.py
 test/test_client_faulty_response.py
 test/test_client_sync.py
 test/test_device.py
 test/test_diag_messages.py
 test/test_events.py
-test/test_example_client_server.py
-test/test_examples.py
 test/test_exceptions.py
 test/test_factory.py
 test/test_file_message.py
 test/test_framers.py
 test/test_logging.py
 test/test_mei_messages.py
 test/test_other_messages.py
@@ -109,13 +107,11 @@
 test/test_register_read_messages.py
 test/test_register_write_messages.py
 test/test_remote_datastore.py
 test/test_repl_client.py
 test/test_server_asyncio.py
 test/test_server_context.py
 test/test_server_multidrop.py
-test/test_server_task.py
 test/test_simulator.py
 test/test_sparse_datastore.py
 test/test_transaction.py
-test/test_unix_socket.py
 test/test_utilities.py
```

### Comparing `pymodbus-3.3.2/requirements.txt` & `pymodbus-3.4.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 coverage==7.1.0
 mypy==1.3.0
 pre-commit==3.1.1
 pyflakes==3.0.1
 pydocstyle==6.3.0
 pycodestyle==2.10.0
 pylint==2.17.2
-pytest==7.2.1
+pytest==7.3.1
 pytest-asyncio==0.20.3
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-timeout==2.1.0
-pytest-xdist==3.1.0
+pytest-xdist==3.3.1
 ruff==0.0.261
 types-Pygments
 types-pyserial
```

### Comparing `pymodbus-3.3.2/setup.cfg` & `pymodbus-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/setup.py` & `pymodbus-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_all_messages.py` & `pymodbus-3.4.0/test/test_all_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 from pymodbus.bit_write_message import (
     WriteMultipleCoilsRequest,
     WriteMultipleCoilsResponse,
     WriteSingleCoilRequest,
     WriteSingleCoilResponse,
 )
-from pymodbus.constants import Defaults
 from pymodbus.register_read_message import (
     ReadHoldingRegistersRequest,
     ReadHoldingRegistersResponse,
     ReadInputRegistersRequest,
     ReadInputRegistersResponse,
     ReadWriteMultipleRegistersRequest,
     ReadWriteMultipleRegistersResponse,
@@ -87,10 +86,10 @@
         """Test that the kwargs are forwarded to the pdu correctly"""
         request = ReadCoilsRequest(1, 5, slave=0x12, transaction=0x12, protocol=0x12)
         assert request.slave_id == 0x12
         assert request.transaction_id == 0x12
         assert request.protocol_id == 0x12
 
         request = ReadCoilsRequest(1, 5)
-        assert request.slave_id == Defaults.Slave
-        assert request.transaction_id == Defaults.TransactionId
-        assert request.protocol_id == Defaults.ProtocolId
+        assert not request.slave_id
+        assert not request.transaction_id
+        assert not request.protocol_id
```

### Comparing `pymodbus-3.3.2/test/test_bit_read_messages.py` & `pymodbus-3.4.0/test/test_bit_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_bit_write_messages.py` & `pymodbus-3.4.0/test/test_bit_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_client.py` & `pymodbus-3.4.0/test/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 import pymodbus.client as lib_client
 import pymodbus.diag_message as pdu_diag
 import pymodbus.other_message as pdu_other_msg
 import pymodbus.register_read_message as pdu_reg_read
 import pymodbus.register_write_message as pdu_req_write
 from pymodbus.client.base import ModbusBaseClient
 from pymodbus.client.mixin import ModbusClientMixin
-from pymodbus.constants import Defaults
 from pymodbus.exceptions import ConnectionException
 from pymodbus.framer.ascii_framer import ModbusAsciiFramer
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
 from pymodbus.framer.socket_framer import ModbusSocketFramer
 from pymodbus.framer.tls_framer import ModbusTlsFramer
+from pymodbus.transport.transport import NULLMODEM_HOST, CommType
+
+
+BASE_PORT = 6500
 
 
 @pytest.mark.parametrize(
     "arglist",
     [
         [
             {},
             {"address": 0x01},
             {"address": 0x01, "value": False},
-            {"msg": "long message"},
+            {"msg": b"long message"},
             {"toggle": False},
             {"address": 0x01, "values": [False, True]},
             {"address": 0x01, "values": [22, 44]},
         ]
     ],
 )
 @pytest.mark.parametrize(
@@ -100,72 +103,71 @@
         pdu_to_call = request
 
     with mock.patch.object(ModbusClientMixin, "execute", fake_execute):
         getattr(ModbusClientMixin(), method)(**arglist[arg])
         assert isinstance(pdu_to_call, pdu_request)
 
 
-@pytest.mark.xdist_group(name="client")
 @pytest.mark.parametrize(
     "arg_list",
     [
         {
             "fix": {
                 "opt_args": {
-                    "timeout": Defaults.Timeout + 2,
-                    "retries": Defaults.Retries + 2,
-                    "retry_on_empty": not Defaults.RetryOnEmpty,
-                    "close_comm_on_error": not Defaults.CloseCommOnError,
-                    "strict": not Defaults.Strict,
-                    "broadcast_enable": not Defaults.BroadcastEnable,
+                    "timeout": 3 + 2,
+                    "retries": 3 + 2,
+                    "retry_on_empty": True,
+                    "close_comm_on_error": True,
+                    "strict": False,
+                    "broadcast_enable": not False,
                     "reconnect_delay": 117,
                     "reconnect_delay_max": 250,
                 },
                 "defaults": {
-                    "timeout": Defaults.Timeout,
-                    "retries": Defaults.Retries,
-                    "retry_on_empty": Defaults.RetryOnEmpty,
-                    "close_comm_on_error": Defaults.CloseCommOnError,
-                    "strict": Defaults.Strict,
-                    "broadcast_enable": Defaults.BroadcastEnable,
-                    "reconnect_delay": Defaults.ReconnectDelay,
-                    "reconnect_delay_max": Defaults.ReconnectDelayMax,
+                    "timeout": 3,
+                    "retries": 3,
+                    "retry_on_empty": False,
+                    "close_comm_on_error": False,
+                    "strict": True,
+                    "broadcast_enable": False,
+                    "reconnect_delay": 100,
+                    "reconnect_delay_max": 1000 * 60 * 5,
                 },
             },
             "serial": {
                 "pos_arg": "/dev/tty",
                 "opt_args": {
                     "framer": ModbusAsciiFramer,
-                    "baudrate": Defaults.Baudrate + 500,
-                    "bytesize": Defaults.Bytesize - 1,
+                    "baudrate": 19200 + 500,
+                    "bytesize": 8 - 1,
                     "parity": "E",
-                    "stopbits": Defaults.Stopbits + 1,
-                    "handle_local_echo": not Defaults.HandleLocalEcho,
+                    "stopbits": 1 + 1,
+                    "handle_local_echo": True,
                 },
                 "defaults": {
                     "host": None,
                     "port": "/dev/tty",
                     "framer": ModbusRtuFramer,
-                    "baudrate": Defaults.Baudrate,
-                    "bytesize": Defaults.Bytesize,
-                    "parity": Defaults.Parity,
-                    "stopbits": Defaults.Stopbits,
-                    "handle_local_echo": Defaults.HandleLocalEcho,
+                    "baudrate": 19200,
+                    "bytesize": 8,
+                    "parity": "N",
+                    "stopbits": 1,
+                    "handle_local_echo": False,
                 },
             },
             "tcp": {
                 "pos_arg": "192.168.1.2",
                 "opt_args": {
                     "port": 112,
                     "framer": ModbusAsciiFramer,
                     "source_address": ("195.6.7.8", 1025),
                 },
                 "defaults": {
                     "host": "192.168.1.2",
-                    "port": Defaults.TcpPort,
+                    "port": 502,
                     "framer": ModbusSocketFramer,
                     "source_address": None,
                 },
             },
             "tls": {
                 "pos_arg": "192.168.1.2",
                 "opt_args": {
@@ -175,15 +177,15 @@
                     "sslctx": None,
                     "certfile": None,
                     "keyfile": None,
                     "password": None,
                 },
                 "defaults": {
                     "host": "192.168.1.2",
-                    "port": Defaults.TlsPort,
+                    "port": 802,
                     "framer": ModbusTlsFramer,
                     "source_address": None,
                     "sslctx": None,
                     "certfile": None,
                     "keyfile": None,
                     "password": None,
                 },
@@ -193,15 +195,15 @@
                 "opt_args": {
                     "port": 121,
                     "framer": ModbusAsciiFramer,
                     "source_address": ("195.6.7.8", 1025),
                 },
                 "defaults": {
                     "host": "192.168.1.2",
-                    "port": Defaults.UdpPort,
+                    "port": 502,
                     "framer": ModbusSocketFramer,
                     "source_address": None,
                 },
             },
         },
     ],
 )
@@ -242,74 +244,45 @@
     # Test information methods
     client.last_frame_end = 2
     client.silent_interval = 2
     assert client.idle_time() == 4
     client.last_frame_end = None
     assert not client.idle_time()
 
-    rc1 = client._get_address_family("127.0.0.1")  # pylint: disable=protected-access
-    assert rc1 == socket.AF_INET
-    rc2 = client._get_address_family("::1")  # pylint: disable=protected-access
-    assert rc2 == socket.AF_INET6
-
     # a successful execute
     client.connect = lambda: True
     client.transport = lambda: None
     client.transaction = mock.Mock(**{"execute.return_value": True})
 
     # a unsuccessful connect
     client.connect = lambda: False
     client.transport = None
     with pytest.raises(ConnectionException):
         client.execute()
 
 
 async def test_client_modbusbaseclient():
     """Test modbus base client class."""
-    client = ModbusBaseClient(framer=ModbusAsciiFramer)
+    client = ModbusBaseClient(
+        framer=ModbusAsciiFramer,
+        host=NULLMODEM_HOST,
+        port=BASE_PORT + 1,
+        CommType=CommType.TCP,
+    )
     client.register(pdu_bit_read.ReadCoilsResponse)
-    buffer = "123ABC"
-    assert client.send(buffer) == buffer
-    assert client.recv(10) == 10
-
-    with mock.patch(
-        "pymodbus.client.base.ModbusBaseClient.connect"
-    ) as p_connect, mock.patch(
-        "pymodbus.client.base.ModbusBaseClient.close"
-    ) as p_close:
-        p_connect.return_value = True
-        p_close.return_value = True
-        with ModbusBaseClient(framer=ModbusAsciiFramer) as b_client:
-            str(b_client)
-        p_connect.return_value = False
+    assert str(client)
+    client.close()
 
 
 async def test_client_connection_made():
     """Test protocol made connection."""
     client = lib_client.AsyncModbusTcpClient("127.0.0.1")
     assert not client.connected
-    client.connection_made(mock.sentinel.PROTOCOL)
+    client.connection_made(mock.AsyncMock())
     assert client.connected
-
-    client.connection_made(mock.sentinel.PROTOCOL_UNEXPECTED)
-    assert client.connected
-
-
-async def test_client_connection_lost():
-    """Test protocol lost connection."""
-    client = lib_client.AsyncModbusTcpClient("127.0.0.1")
-    assert not client.connected
-
-    # fake client is connected and *then* looses connection:
-    client.params.host = mock.sentinel.HOST
-    client.params.port = mock.sentinel.PORT
-    client.connection_lost(mock.sentinel.PROTOCOL_UNEXPECTED)
-    assert not client.connected
-    client.connection_lost(mock.sentinel.PROTOCOL)
-    assert not client.connected
     client.close()
 
 
 async def test_client_base_async():
     """Test modbus base client class."""
     with mock.patch(
         "pymodbus.client.base.ModbusBaseClient.connect"
@@ -317,22 +290,28 @@
         "pymodbus.client.base.ModbusBaseClient.close"
     ) as p_close:
         asyncio.get_event_loop()
         p_connect.return_value = asyncio.Future()
         p_connect.return_value.set_result(True)
         p_close.return_value = asyncio.Future()
         p_close.return_value.set_result(True)
-        async with ModbusBaseClient(framer=ModbusAsciiFramer) as client:
+        async with ModbusBaseClient(
+            framer=ModbusAsciiFramer,
+            host=NULLMODEM_HOST,
+            port=BASE_PORT + 2,
+            CommType=CommType.TCP,
+        ) as client:
             str(client)
         p_connect.return_value = asyncio.Future()
         p_connect.return_value.set_result(False)
         p_close.return_value = asyncio.Future()
         p_close.return_value.set_result(False)
 
 
+@pytest.mark.skip()
 async def test_client_protocol_receiver():
     """Test the client protocol data received"""
     base = ModbusBaseClient(framer=ModbusSocketFramer)
     transport = mock.MagicMock()
     base.connection_made(transport)
     assert base.transport == transport
     assert base.transport
@@ -346,14 +325,15 @@
     assert isinstance(result, pdu_bit_read.ReadCoilsResponse)
 
     base.transport = None
     with pytest.raises(ConnectionException):
         await base._build_response(0x00)  # pylint: disable=protected-access
 
 
+@pytest.mark.skip()
 async def test_client_protocol_response():
     """Test the udp client protocol builds responses"""
     base = ModbusBaseClient(framer=ModbusSocketFramer)
     response = base._build_response(0x00)  # pylint: disable=protected-access
     excp = response.exception()
     assert isinstance(excp, ConnectionException)
     assert not list(base.transaction)
@@ -361,15 +341,17 @@
     base.transport = lambda: None
     base._build_response(0x00)  # pylint: disable=protected-access
     assert len(list(base.transaction)) == 1
 
 
 async def test_client_protocol_handler():
     """Test the client protocol handles responses"""
-    base = ModbusBaseClient(framer=ModbusSocketFramer)
+    base = ModbusBaseClient(
+        framer=ModbusAsciiFramer, host=NULLMODEM_HOST, port=+3, CommType=CommType.TCP
+    )
     transport = mock.MagicMock()
     base.connection_made(transport=transport)
     reply = pdu_bit_read.ReadCoilsRequest(1, 1)
     reply.transaction_id = 0x00
     base._handle_response(None)  # pylint: disable=protected-access
     base._handle_response(reply)  # pylint: disable=protected-access
     response = base._build_response(0x00)  # pylint: disable=protected-access
@@ -393,23 +375,14 @@
     assert response == f_trans
 
     base.params.broadcast_enable = True
     request = pdu_bit_read.ReadCoilsRequest(1, 1)
     response = await base.async_execute(request)
 
 
-def test_client_udp():
-    """Test client udp."""
-    base = ModbusBaseClient(host="127.0.0.1", framer=ModbusSocketFramer)
-    base.datagram_received(bytes("00010000", "utf-8"), 1)
-    base.transport = mock.MagicMock()
-    base.use_udp = True
-    base.transport.sendto(bytes("00010000", "utf-8"))
-
-
 def test_client_udp_connect():
     """Test the Udp client connection method"""
     with mock.patch.object(socket, "socket") as mock_method:
 
         class DummySocket:
             """Dummy socket."""
```

### Comparing `pymodbus-3.3.2/test/test_client_faulty_response.py` & `pymodbus-3.4.0/test/test_client_faulty_response.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_client_sync.py` & `pymodbus-3.4.0/test/test_client_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Test client sync."""
-import ssl
 from itertools import count
 from test.conftest import mockSocket
 from unittest import mock
 
 import pytest
 import serial
 
 from pymodbus.client import (
     ModbusSerialClient,
     ModbusTcpClient,
     ModbusTlsClient,
     ModbusUdpClient,
 )
-from pymodbus.client.tls import sslctx_provider
 from pymodbus.exceptions import ConnectionException
 from pymodbus.transaction import (
     ModbusAsciiFramer,
     ModbusBinaryFramer,
     ModbusRtuFramer,
     ModbusSocketFramer,
     ModbusTlsFramer,
@@ -93,15 +91,15 @@
         client.close()
 
     def test_udp_client_repr(self):
         """Test udp client representation."""
         client = ModbusUdpClient("127.0.0.1")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
-            f"ipaddr={client.params.host}, port={client.params.port}, timeout={client.params.timeout}>"
+            f"ipaddr={client.comm_params.host}, port={client.comm_params.port}, timeout={client.comm_params.timeout_connect}>"
         )
         assert repr(client) == rep
 
     # -----------------------------------------------------------------------#
     # Test TCP Client
     # -----------------------------------------------------------------------#
 
@@ -158,15 +156,15 @@
         assert client.recv(0) == b""
         client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(4) == b"\x00" * 4
 
         mock_socket = mock.MagicMock()
         mock_socket.recv.side_effect = iter([b"\x00", b"\x01", b"\x02"])
         client.socket = mock_socket
-        client.params.timeout = 3
+        client.comm_params.timeout_connect = 3
         assert client.recv(3) == b"\x00\x01\x02"
         mock_socket.recv.side_effect = iter([b"\x00", b"\x01", b"\x02"])
         assert client.recv(2) == b"\x00\x01"
         mock_select.select.return_value = [False]
         assert client.recv(2) == b""
         client.socket = mockSocket()
         client.socket.mock_prepare_receive(b"\x00")
@@ -183,15 +181,15 @@
         assert client.recv(1024) == b"\x00\x01\x02"
 
     def test_tcp_client_repr(self):
         """Test tcp client."""
         client = ModbusTcpClient("127.0.0.1")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
-            f"ipaddr={client.params.host}, port={client.params.port}, timeout={client.params.timeout}>"
+            f"ipaddr={client.comm_params.host}, port={client.comm_params.port}, timeout={client.comm_params.timeout_connect}>"
         )
         assert repr(client) == rep
 
     def test_tcp_client_register(self):
         """Test tcp client."""
 
         class CustomRequest:  # pylint: disable=too-few-public-methods
@@ -204,36 +202,14 @@
         client.register(CustomRequest)
         assert client.framer.decoder.register.called_once_with(CustomRequest)
 
     # -----------------------------------------------------------------------#
     # Test TLS Client
     # -----------------------------------------------------------------------#
 
-    def test_tls_sslctx_provider(self):
-        """Test that sslctx_provider() produce SSLContext correctly"""
-        with mock.patch.object(ssl.SSLContext, "load_cert_chain") as mock_method:
-            sslctx1 = sslctx_provider(certfile="cert.pem")
-            assert sslctx1
-            assert isinstance(sslctx1, ssl.SSLContext)
-            assert not mock_method.called
-
-            sslctx2 = sslctx_provider(keyfile="key.pem")
-            assert sslctx2
-            assert isinstance(sslctx2, ssl.SSLContext)
-            assert not mock_method.called
-
-            sslctx3 = sslctx_provider(certfile="cert.pem", keyfile="key.pem")
-            assert sslctx3
-            assert isinstance(sslctx3, ssl.SSLContext)
-            assert mock_method.called
-
-            sslctx_old = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
-            sslctx_new = sslctx_provider(sslctx=sslctx_old)
-            assert sslctx_new == sslctx_old
-
     def test_syn_tls_client_instantiation(self):
         """Test sync tls client."""
         # default SSLContext
         client = ModbusTlsClient("127.0.0.1")
         assert client
         assert isinstance(client.framer, ModbusTlsFramer)
         assert client.sslctx
@@ -284,25 +260,25 @@
         mock_time.time.side_effect = count()
 
         client.socket = mockSocket()
         client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(0) == b""
         assert client.recv(4) == b"\x00" * 4
 
-        client.params.timeout = 2
+        client.comm_params.timeout_connect = 2
         client.socket.mock_prepare_receive(b"\x00")
         assert b"\x00" in client.recv(None)
 
     def test_tls_client_repr(self):
         """Test tls client."""
         client = ModbusTlsClient("127.0.0.1")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
-            f"ipaddr={client.params.host}, port={client.params.port}, sslctx={client.sslctx}, "
-            f"timeout={client.params.timeout}>"
+            f"ipaddr={client.comm_params.host}, port={client.comm_params.port}, sslctx={client.sslctx}, "
+            f"timeout={client.comm_params.timeout_connect}>"
         )
         assert repr(client) == rep
 
     def test_tls_client_register(self):
         """Test tls client."""
 
         class CustomeRequest:  # pylint: disable=too-few-public-methods
@@ -444,10 +420,10 @@
         assert client.recv(0) == b""
 
     def test_serial_client_repr(self):
         """Test serial client."""
         client = ModbusSerialClient("/dev/null")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
-            f"framer={client.framer}, timeout={client.params.timeout}>"
+            f"framer={client.framer}, timeout={client.comm_params.timeout_connect}>"
         )
         assert repr(client) == rep
```

### Comparing `pymodbus-3.3.2/test/test_device.py` & `pymodbus-3.4.0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_diag_messages.py` & `pymodbus-3.4.0/test/test_diag_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,24 +162,24 @@
         """Testing diagnostic message execution"""
         for message, encoded, executed in self.requests:
             encoded = message().execute().encode()
             assert encoded == executed
 
     def test_return_query_data_request(self):
         """Testing diagnostic message execution"""
-        message = ReturnQueryDataRequest([0x0000] * 2)
+        message = ReturnQueryDataRequest(b"\x00\x00\x00\x00")
         assert message.encode() == b"\x00\x00\x00\x00\x00\x00"
-        message = ReturnQueryDataRequest(0x0000)
+        message = ReturnQueryDataRequest(b"\x00\x00")
         assert message.encode() == b"\x00\x00\x00\x00"
 
     def test_return_query_data_response(self):
         """Testing diagnostic message execution"""
-        message = ReturnQueryDataResponse([0x0000] * 2)
+        message = ReturnQueryDataResponse(b"\x00\x00\x00\x00")
         assert message.encode() == b"\x00\x00\x00\x00\x00\x00"
-        message = ReturnQueryDataResponse(0x0000)
+        message = ReturnQueryDataResponse(b"\x00\x00")
         assert message.encode() == b"\x00\x00\x00\x00"
 
     def test_restart_cmmunications_option(self):
         """Testing diagnostic message execution"""
         request = RestartCommunicationsOptionRequest(True)
         assert request.encode() == b"\x00\x01\xff\x00"
         request = RestartCommunicationsOptionRequest(False)
```

### Comparing `pymodbus-3.3.2/test/test_events.py` & `pymodbus-3.4.0/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_exceptions.py` & `pymodbus-3.4.0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_factory.py` & `pymodbus-3.4.0/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_file_message.py` & `pymodbus-3.4.0/test/test_file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_framers.py` & `pymodbus-3.4.0/test/test_framers.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 from pymodbus.bit_read_message import ReadCoilsRequest
 from pymodbus.client import ModbusBaseClient
 from pymodbus.exceptions import ModbusIOException
 from pymodbus.factory import ClientDecoder
 from pymodbus.framer.ascii_framer import ModbusAsciiFramer
 from pymodbus.framer.binary_framer import ModbusBinaryFramer
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
+from pymodbus.transport.transport import NULLMODEM_HOST, CommType
 from pymodbus.utilities import ModbusTransactionState
 
 
+BASE_PORT = 6600
+
+
 TEST_MESSAGE = b"\x00\x01\x00\x01\x00\n\xec\x1c"
 
 
 @pytest.fixture(name="rtu_framer")
 def fixture_rtu_framer():
     """RTU framer."""
     return ModbusRtuFramer(ClientDecoder())
@@ -47,33 +51,42 @@
     decoder = ClientDecoder()
     framer = framer(decoder)
     assert framer.client is None
     assert framer._buffer == b""  # pylint: disable=protected-access
     assert framer.decoder == decoder
     if isinstance(framer, ModbusAsciiFramer):
         assert framer._header == {  # pylint: disable=protected-access
+            "tid": 0,
+            "pid": 0,
             "lrc": "0000",
             "len": 0,
             "uid": 0x00,
+            "crc": b"\x00\x00",
         }
         assert framer._hsize == 0x02  # pylint: disable=protected-access
         assert framer._start == b":"  # pylint: disable=protected-access
         assert framer._end == b"\r\n"  # pylint: disable=protected-access
     elif isinstance(framer, ModbusRtuFramer):
         assert framer._header == {  # pylint: disable=protected-access
+            "tid": 0,
+            "pid": 0,
+            "lrc": "0000",
             "uid": 0x00,
             "len": 0,
             "crc": b"\x00\x00",
         }
         assert framer._hsize == 0x01  # pylint: disable=protected-access
         assert framer._end == b"\x0d\x0a"  # pylint: disable=protected-access
         assert framer._min_frame_size == 4  # pylint: disable=protected-access
     else:
         assert framer._header == {  # pylint: disable=protected-access
-            "crc": 0x0000,
+            "tid": 0,
+            "pid": 0,
+            "lrc": "0000",
+            "crc": b"\x00\x00",
             "len": 0,
             "uid": 0x00,
         }
         assert framer._hsize == 0x01  # pylint: disable=protected-access
         assert framer._start == b"\x7b"  # pylint: disable=protected-access
         assert framer._end == b"\x7d"  # pylint: disable=protected-access
         assert framer._repeat == [  # pylint: disable=protected-access
@@ -135,17 +148,20 @@
 
 @pytest.mark.parametrize("data", [b"", b"abcd"])
 def test_rtu_reset_framer(rtu_framer, data):
     """Test rtu reset framer."""
     rtu_framer._buffer = data  # pylint: disable=protected-access
     rtu_framer.resetFrame()
     assert rtu_framer._header == {  # pylint: disable=protected-access
-        "uid": 0x00,
-        "len": 0,
+        "lrc": "0000",
         "crc": b"\x00\x00",
+        "len": 0,
+        "uid": 0x00,
+        "pid": 0,
+        "tid": 0,
     }
 
 
 @pytest.mark.parametrize(
     "data",
     [
         (b"", False),
@@ -182,39 +198,46 @@
 
 
 @pytest.mark.parametrize(
     "data",
     [
         (
             b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD",
-            {"crc": b"\x49\xAD", "uid": 17, "len": 11},
+            {
+                "crc": b"\x49\xAD",
+                "uid": 17,
+                "len": 11,
+                "lrc": "0000",
+                "tid": 17,
+                "pid": 0,
+            },
         ),
         (
             b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD\x11\x03",
-            {"crc": b"\x49\xAD", "uid": 17, "len": 11},
+            {
+                "crc": b"\x49\xAD",
+                "uid": 17,
+                "len": 11,
+                "lrc": "0000",
+                "tid": 17,
+                "pid": 0,
+            },
         ),
     ],
 )
 def test_rtu_populate_header(rtu_framer, data):
     """Test rtu populate header."""
     buffer, expected = data
     rtu_framer.populateHeader(buffer)
     assert rtu_framer._header == expected  # pylint: disable=protected-access
 
 
-def test_add_to_frame(rtu_framer):
-    """Test add to frame."""
-    assert rtu_framer._buffer == b""  # pylint: disable=protected-access
-    rtu_framer.addToFrame(b"abcd")
-    assert rtu_framer._buffer == b"abcd"  # pylint: disable=protected-access
-
-
 def test_get_frame(rtu_framer):
     """Test get frame."""
-    rtu_framer.addToFrame(b"\x02\x01\x01\x00Q\xcc")
+    rtu_framer._buffer = b"\x02\x01\x01\x00Q\xcc"  # pylint: disable=protected-access
     rtu_framer.populateHeader(b"\x02\x01\x01\x00Q\xcc")
     assert rtu_framer.getFrame() == b"\x01\x01\x00"
 
 
 def test_populate_result(rtu_framer):
     """Test populate result."""
     rtu_framer._header["uid"] = 255  # pylint: disable=protected-access
@@ -280,19 +303,24 @@
     message = ReadCoilsRequest(1, 10)
     assert rtu_framer.buildPacket(message) == TEST_MESSAGE
 
 
 def test_send_packet(rtu_framer):
     """Test send packet."""
     message = TEST_MESSAGE
-    client = ModbusBaseClient(framer=ModbusRtuFramer)
+    client = ModbusBaseClient(
+        framer=ModbusAsciiFramer,
+        host=NULLMODEM_HOST,
+        port=BASE_PORT + 1,
+        CommType=CommType.TCP,
+    )
     client.state = ModbusTransactionState.TRANSACTION_COMPLETE
     client.silent_interval = 1
     client.last_frame_end = 1
-    client.params.timeout = 0.25
+    client.comm_params.timeout_connect = 0.25
     client.idle_time = mock.Mock(return_value=1)
     client.send = mock.Mock(return_value=len(message))
     rtu_framer.client = client
     assert rtu_framer.sendPacket(message) == len(message)
     client.state = ModbusTransactionState.PROCESSING_REPLY
     assert rtu_framer.sendPacket(message) == len(message)
 
@@ -310,23 +338,14 @@
     """Test process."""
 
     rtu_framer._buffer = TEST_MESSAGE  # pylint: disable=protected-access
     with pytest.raises(ModbusIOException):
         rtu_framer._process(None)  # pylint: disable=protected-access
 
 
-def test_get_raw_frame(rtu_framer):
-    """Test get raw frame."""
-    rtu_framer._buffer = TEST_MESSAGE  # pylint: disable=protected-access
-    assert (
-        rtu_framer.getRawFrame()
-        == rtu_framer._buffer  # pylint: disable=protected-access
-    )
-
-
 def test_validate__slave_id(rtu_framer):
     """Test validate slave."""
     rtu_framer.populateHeader(TEST_MESSAGE)
     assert rtu_framer._validate_slave_id([0], False)  # pylint: disable=protected-access
     assert rtu_framer._validate_slave_id([1], True)  # pylint: disable=protected-access
```

### Comparing `pymodbus-3.3.2/test/test_logging.py` & `pymodbus-3.4.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_mei_messages.py` & `pymodbus-3.4.0/test/test_mei_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_other_messages.py` & `pymodbus-3.4.0/test/test_other_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_payload.py` & `pymodbus-3.4.0/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_pdu.py` & `pymodbus-3.4.0/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_register_read_messages.py` & `pymodbus-3.4.0/test/test_register_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_register_write_messages.py` & `pymodbus-3.4.0/test/test_register_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_remote_datastore.py` & `pymodbus-3.4.0/test/test_remote_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_repl_client.py` & `pymodbus-3.4.0/test/test_repl_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_server_asyncio.py` & `pymodbus-3.4.0/test/test_server_asyncio.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         BasicClient.connected = None
         BasicClient.done = None
         BasicClient.received_data = None
         BasicClient.eof = None
         BasicClient.my_protocol = None
 
 
-class TestAsyncioServer:  # pylint: disable=too-many-public-methods
+class TestAsyncioServer:
     """Unittest for the pymodbus.server.asyncio module.
 
     The scope of this test is the life-cycle management of the network
     connections and server objects.
 
     This test suite does not attempt to test any of the underlying protocol details
     """
@@ -163,41 +163,37 @@
         assert self.server
         if do_forever:
             self.task = asyncio.create_task(self.server.serve_forever())
             self.task.add_done_callback(self.handle_task)
             assert not self.task.cancelled()
             await asyncio.wait_for(self.server.serving, timeout=0.1)
             if not do_udp:
-                assert self.server.server
+                assert self.server.transport
         elif not do_udp:  # pylint: disable=confusing-consecutive-elif
-            assert not self.server.server
+            assert not self.server.transport
         assert self.server.control.Identity.VendorName == "VendorName"
         await asyncio.sleep(0.1)
 
     async def connect_server(self):
         """Handle connect to server"""
         BasicClient.connected = asyncio.Future()
         BasicClient.done = asyncio.Future()
         BasicClient.eof = asyncio.Future()
-        random_port = self.server.server.sockets[0].getsockname()[
+        random_port = self.server.transport.sockets[0].getsockname()[
             1
         ]  # get the random server port
         (
             BasicClient.transport,
             BasicClient.my_protocol,
         ) = await self.loop.create_connection(
             BasicClient, host="127.0.0.1", port=random_port
         )
         await asyncio.wait_for(BasicClient.connected, timeout=0.1)
         await asyncio.sleep(0.1)
 
-    # -----------------------------------------------------------------------#
-    #  Test ModbusConnectedRequestHandler
-    # -----------------------------------------------------------------------#
-
     async def test_async_start_server_no_loop(self):
         """Test that the modbus tcp asyncio server starts correctly"""
         await self.start_server(do_forever=False)
 
     async def test_async_start_server(self):
         """Test that the modbus tcp asyncio server starts correctly"""
         await self.start_server()
@@ -229,21 +225,19 @@
         await asyncio.wait_for(BasicClient.done, timeout=0.1)
         assert BasicClient.received_data, expected_response
 
     async def test_async_tcp_server_connection_lost(self):
         """Test tcp stream interruption"""
         await self.start_server()
         await self.connect_server()
-        assert len(self.server.active_connections), 1
 
         BasicClient.transport.close()
         await asyncio.sleep(0.2)  # so we have to wait a bit
-        assert not self.server.active_connections
 
-    async def test_async_tcp_server_close_active_connection(self):
+    async def test_async_tcp_server_close_connection(self):
         """Test server_close() while there are active TCP connections"""
         await self.start_server()
         await self.connect_server()
 
         # On Windows we seem to need to give this an extra chance to finish,
         # otherwise there ends up being an active connection at the assert.
         await asyncio.sleep(0.5)
@@ -276,31 +270,20 @@
     # Test ModbusTlsProtocol
     # -----------------------------------------------------------------------#
     async def test_async_start_tls_server_no_loop(self):
         """Test that the modbus tls asyncio server starts correctly"""
         with mock.patch.object(ssl.SSLContext, "load_cert_chain"):
             await self.start_server(do_tls=True, do_forever=False, do_ident=True)
             assert self.server.control.Identity.VendorName == "VendorName"
-            assert self.server.sslctx
 
     async def test_async_start_tls_server(self):
         """Test that the modbus tls asyncio server starts correctly"""
         with mock.patch.object(ssl.SSLContext, "load_cert_chain"):
             await self.start_server(do_tls=True, do_ident=True)
             assert self.server.control.Identity.VendorName == "VendorName"
-            assert self.server.sslctx
-
-    async def test_async_tls_server_serve_forever(self):
-        """Test StartAsyncTcpServer serve_forever() method"""
-        with mock.patch(
-            "asyncio.base_events.Server.serve_forever", new_callable=mock.AsyncMock
-        ) as serve, mock.patch.object(ssl.SSLContext, "load_cert_chain"):
-            await self.start_server(do_tls=True, do_forever=False)
-            await self.server.serve_forever()
-            serve.assert_awaited()
 
     async def test_async_tls_server_serve_forever_twice(self):
         """Call on serve_forever() twice should result in a runtime error"""
         with mock.patch.object(ssl.SSLContext, "load_cert_chain"):
             await self.start_server(do_tls=True)
             with pytest.raises(RuntimeError):
                 await self.server.serve_forever()
@@ -309,85 +292,41 @@
     # Test ModbusUdpProtocol
     # -----------------------------------------------------------------------#
 
     async def test_async_start_udp_server_no_loop(self):
         """Test that the modbus udp asyncio server starts correctly"""
         await self.start_server(do_udp=True, do_forever=False, do_ident=True)
         assert self.server.control.Identity.VendorName == "VendorName"
-        assert not self.server.protocol
+        assert not self.server.transport
 
     async def test_async_start_udp_server(self):
         """Test that the modbus udp asyncio server starts correctly"""
         await self.start_server(do_udp=True, do_ident=True)
         assert self.server.control.Identity.VendorName == "VendorName"
-        assert self.server.protocol
-
-    async def test_async_udp_server_serve_forever_start(self):
-        """Test StartAsyncUdpServer serve_forever() method"""
-        with mock.patch(
-            "asyncio.base_events.Server.serve_forever", new_callable=mock.AsyncMock
-        ) as serve:
-            await self.start_server(do_forever=False, do_ident=True)
-            await self.server.serve_forever()
-            serve.assert_awaited()
+        assert self.server.transport
 
     async def test_async_udp_server_serve_forever_close(self):
         """Test StarAsyncUdpServer serve_forever() method"""
         await self.start_server(do_udp=True)
-        assert asyncio.isfuture(self.server.on_connection_terminated)
-        assert not self.server.on_connection_terminated.done()
         await self.server.server_close()
         self.server = None
 
     async def test_async_udp_server_serve_forever_twice(self):
         """Call on serve_forever() twice should result in a runtime error"""
         await self.start_server(do_udp=True, do_ident=True)
         with pytest.raises(RuntimeError):
             await self.server.serve_forever()
 
-    @pytest.mark.skipif(pytest.IS_WINDOWS, reason="Windows have a timeout problem.")
-    async def test_async_udp_server_receive_data(self):
-        """Test that the sending data on datagram socket gets data pushed to framer"""
-        await self.start_server(do_udp=True)
-        with mock.patch(
-            "pymodbus.transaction.ModbusSocketFramer.processIncomingPacket",
-            new_callable=mock.Mock,
-        ) as process:
-            self.server.endpoint.datagram_received(data=b"12345", addr=(SERV_IP, 12345))
-            await asyncio.sleep(0.1)
-            process.seal()
-            process.assert_called_once()
-            assert process.call_args[1]["data"] == b"12345"
-
-    async def test_async_udp_server_send_data(self):
-        """Test that the modbus udp asyncio server correctly sends data outbound"""
-        BasicClient.dataTo = b"x\01\x00\x00\x00\x00\x06\x01\x03\x00\x00\x00\x19"
-        await self.start_server(do_udp=True)
-        random_port = self.server.protocol._sock.getsockname()[  # pylint: disable=protected-access
-            1
-        ]
-        received = self.server.endpoint.datagram_received = mock.Mock(
-            wraps=self.server.endpoint.datagram_received
-        )
-        await self.loop.create_datagram_endpoint(
-            BasicClient, remote_addr=("127.0.0.1", random_port)
-        )
-        await asyncio.sleep(0.1)
-        received.assert_called_once()
-        assert received.call_args[0][0] == BasicClient.dataTo
-        await self.server.server_close()
-        self.server = None
-
     async def test_async_udp_server_roundtrip(self):
         """Test sending and receiving data on udp socket"""
         expected_response = b"\x01\x00\x00\x00\x00\x05\x01\x03\x02\x00\x11"  # value of 17 as per context
         BasicClient.dataTo = TEST_DATA  # slave 1, read register
         BasicClient.done = asyncio.Future()
         await self.start_server(do_udp=True)
-        random_port = self.server.protocol._sock.getsockname()[  # pylint: disable=protected-access
+        random_port = self.server.transport._sock.getsockname()[  # pylint: disable=protected-access
             1
         ]
         transport, _ = await self.loop.create_datagram_endpoint(
             BasicClient, remote_addr=("127.0.0.1", random_port)
         )
         await asyncio.wait_for(BasicClient.done, timeout=0.1)
         assert BasicClient.received_data == expected_response
@@ -400,21 +339,21 @@
         BasicClient.done = asyncio.Future()
         await self.start_server(do_udp=True)
         with mock.patch(
             "pymodbus.transaction.ModbusSocketFramer.processIncomingPacket",
             new_callable=lambda: mock.Mock(side_effect=Exception),
         ):
             # get the random server port pylint: disable=protected-access
-            random_port = self.server.protocol._sock.getsockname()[1]
+            random_port = self.server.transport._sock.getsockname()[1]
             _, _ = await self.loop.create_datagram_endpoint(
                 BasicClient, remote_addr=("127.0.0.1", random_port)
             )
             await asyncio.wait_for(BasicClient.connected, timeout=0.1)
             assert not BasicClient.done.done()
-            assert not self.server.protocol._sock._closed
+            assert not self.server.transport._sock._closed
 
     async def test_async_tcp_server_exception(self):
         """Send garbage data on a TCP socket should drop the connection"""
         BasicClient.data = b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF"
         await self.start_server()
         with mock.patch(
             "pymodbus.transaction.ModbusSocketFramer.processIncomingPacket",
```

### Comparing `pymodbus-3.3.2/test/test_server_context.py` & `pymodbus-3.4.0/test/test_server_context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_server_multidrop.py` & `pymodbus-3.4.0/test/test_server_multidrop.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_simulator.py` & `pymodbus-3.4.0/test/test_simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Test datastore."""
+import asyncio
 import copy
+import json
+from unittest.mock import mock_open, patch
 
 import pytest
 
 from pymodbus.datastore import ModbusSimulatorContext
 from pymodbus.datastore.simulator import Cell, CellType, Label
+from pymodbus.server import ModbusSimulatorServer
 
 
 FX_READ_BIT = 1
 FX_READ_REG = 3
 FX_WRITE_BIT = 5
 FX_WRITE_REG = 6
 
@@ -64,40 +68,58 @@
         "uint16": [
             {"addr": 16, "value": 3124},
             {"addr": [17, 18], "value": 5678},
             {
                 "addr": [19, 20],
                 "value": 14661,
                 "action": "increment",
-                "args": {"min": 1, "max": 100},
+                "args": {"minval": 1, "maxval": 100},
             },
         ],
         "uint32": [
             {"addr": [21, 22], "value": 3124},
             {"addr": [23, 26], "value": 5678},
             {"addr": [27, 30], "value": 345000, "action": "increment"},
             {
                 "addr": [31, 32],
                 "value": 50,
                 "action": "random",
-                "kwargs": {"min": 10, "max": 80},
+                "kwargs": {"minval": 10, "maxval": 80},
             },
         ],
         "float32": [
             {"addr": [33, 34], "value": 3124.5},
             {"addr": [35, 38], "value": 5678.19},
             {"addr": [39, 42], "value": 345000.18, "action": "increment"},
         ],
         "string": [
             {"addr": [43, 44], "value": "Str"},
             {"addr": [45, 48], "value": "Strxyz12"},
         ],
         "repeat": [{"addr": [0, 48], "to": [49, 147]}],
     }
 
+    default_server_config = {
+        "server": {
+            "comm": "tcp",
+            "host": "0.0.0.0",
+            "port": 5020,
+            "ignore_missing_slaves": False,
+            "framer": "socket",
+            "identity": {
+                "VendorName": "pymodbus",
+                "ProductCode": "PM",
+                "VendorUrl": "https://github.com/pymodbus-dev/pymodbus/",
+                "ProductName": "pymodbus Server",
+                "ModelName": "pymodbus Server",
+                "MajorMinorRevision": "3.1.0",
+            },
+        },
+    }
+
     test_registers = [
         Cell(),
         Cell(),
         Cell(),
         Cell(),
         Cell(),
         Cell(type=CellType.BITS, access=True, value=0x0708),
@@ -122,26 +144,28 @@
         Cell(type=CellType.NEXT, access=True, value=5678),
         Cell(type=CellType.UINT32, access=True),
         Cell(type=CellType.NEXT, access=True, value=5678),
         Cell(type=CellType.UINT32, value=5, action=1),
         Cell(type=CellType.NEXT, value=17320),
         Cell(type=CellType.UINT32, value=5, action=1),
         Cell(type=CellType.NEXT, value=17320),  # 30
-        Cell(type=CellType.UINT32, action=2, action_kwargs={"min": 10, "max": 80}),
+        Cell(
+            type=CellType.UINT32, action=2, action_kwargs={"minval": 10, "maxval": 80}
+        ),
         Cell(type=CellType.NEXT, value=50),
-        Cell(type=CellType.FLOAT32, access=True, value=72),
-        Cell(type=CellType.NEXT, access=True, value=17221),
-        Cell(type=CellType.FLOAT32, access=True, value=34161),
-        Cell(type=CellType.NEXT, access=True, value=45381),
-        Cell(type=CellType.FLOAT32, access=True, value=34161),
-        Cell(type=CellType.NEXT, access=True, value=45381),
-        Cell(type=CellType.FLOAT32, value=1653, action=1),
-        Cell(type=CellType.NEXT, value=43080),  # 40
-        Cell(type=CellType.FLOAT32, value=1653, action=1),
-        Cell(type=CellType.NEXT, value=43080),
+        Cell(type=CellType.FLOAT32, access=True, value=17731),
+        Cell(type=CellType.NEXT, access=True, value=18432),
+        Cell(type=CellType.FLOAT32, access=True, value=17841),
+        Cell(type=CellType.NEXT, access=True, value=29061),
+        Cell(type=CellType.FLOAT32, access=True, value=17841),
+        Cell(type=CellType.NEXT, access=True, value=29061),
+        Cell(type=CellType.FLOAT32, value=18600, action=1),
+        Cell(type=CellType.NEXT, value=29958),  # 40
+        Cell(type=CellType.FLOAT32, value=18600, action=1),
+        Cell(type=CellType.NEXT, value=29958),
         Cell(type=CellType.STRING, value=int.from_bytes(bytes("St", "utf-8"), "big")),
         Cell(type=CellType.NEXT, value=int.from_bytes(bytes("r ", "utf-8"), "big")),
         Cell(type=CellType.STRING, value=int.from_bytes(bytes("St", "utf-8"), "big")),
         Cell(type=CellType.NEXT, value=int.from_bytes(bytes("rx", "utf-8"), "big")),
         Cell(type=CellType.NEXT, value=int.from_bytes(bytes("yz", "utf-8"), "big")),
         Cell(type=CellType.NEXT, value=int.from_bytes(bytes("12", "utf-8"), "big")),
         # 48 MAX before repeat
@@ -382,15 +406,15 @@
             (1, "1", Cell(type=Label.invalid, action="none", value="0")),
             (5, "5", Cell(type=Label.type_bits, action="none", value="0x708")),
             (
                 31,
                 "31-32",
                 Cell(
                     type=Label.type_uint32,
-                    action="random({'min': 10, 'max': 80})",
+                    action="random({'minval': 10, 'maxval': 80})",
                     value="50",
                 ),
             ),
             (33, "33-34", Cell(type=Label.type_float32, action="none", value="3124.5")),
             (43, "43-44", Cell(type=Label.type_string, action="none", value="Str ")),
         ):
             reg = self.simulator.registers[test_reg]
@@ -431,26 +455,127 @@
         reg2.value = 0
         if func == FX_READ_BIT:
             addr = addr * 16 - 16 + 14
         values = exc_simulator.getValues(func, addr, 2)
         assert values[0] or values[1]
 
     def test_simulator_action_timestamp(self):
-        """Test action random"""
+        """Test action timestamp"""
         exc_setup = copy.deepcopy(self.default_config)
         exc_simulator = ModbusSimulatorContext(exc_setup, None)
         addr = 12
         exc_simulator.registers[addr].action = exc_simulator.action_name_to_id[
             Label.timestamp
         ]
         exc_simulator.getValues(FX_READ_REG, addr, 1)
 
     def test_simulator_action_reset(self):
-        """Test action random"""
+        """Test action reset"""
         exc_setup = copy.deepcopy(self.default_config)
         exc_simulator = ModbusSimulatorContext(exc_setup, None)
         addr = 12
         exc_simulator.registers[addr].action = exc_simulator.action_name_to_id[
             Label.reset
         ]
         with pytest.raises(RuntimeError):
             exc_simulator.getValues(FX_READ_REG, addr, 1)
+
+    @pytest.mark.parametrize(
+        ("celltype", "minval", "maxval", "value", "expected"),
+        [
+            (CellType.BITS, 50, 75, 73, (74, 75, 50)),
+            (CellType.BITS, 50, 75, 45, (50, 51, 52)),
+            (CellType.UINT16, 50, 15075, 15073, (15074, 15075, 50)),
+            (CellType.UINT16, 50, 75, 45, (50, 51, 52)),
+            (CellType.UINT32, 50, 63075, 63073, (63074, 63075, 50)),
+            (CellType.UINT32, 50, 75, 45, (50, 51, 52)),
+            (CellType.FLOAT32, 27.0, 16100.5, 16098.0, (16099.0, 16100.0, 27.0)),
+            (CellType.FLOAT32, 27.0, 75.5, 24.0, (27.0, 28.0, 29.0)),
+        ],
+    )
+    def test_simulator_action_increment(
+        self, celltype, minval, maxval, value, expected
+    ):
+        """Test action increment"""
+        exc_setup = copy.deepcopy(self.default_config)
+        exc_simulator = ModbusSimulatorContext(exc_setup, None)
+        action = exc_simulator.action_name_to_id[Label.increment]
+        kwargs = {
+            "minval": minval,
+            "maxval": maxval,
+        }
+        exc_simulator.registers[30].type = celltype
+        exc_simulator.registers[30].action = action
+        exc_simulator.registers[30].action_kwargs = kwargs
+        exc_simulator.registers[31].type = CellType.NEXT
+
+        is_int = celltype != CellType.FLOAT32
+        reg_count = 1 if celltype in (CellType.BITS, CellType.UINT16) else 2
+        regs = (
+            [value, 0]
+            if reg_count == 1
+            else ModbusSimulatorContext.build_registers_from_value(value, is_int)
+        )
+        exc_simulator.registers[30].value = regs[0]
+        exc_simulator.registers[31].value = regs[1]
+        for expect_value in expected:
+            regs = exc_simulator.getValues(FX_READ_REG, 30, reg_count)
+            if reg_count == 1:
+                assert expect_value == regs[0], f"type({celltype})"
+            else:
+                new_value = ModbusSimulatorContext.build_value_from_registers(
+                    regs, is_int
+                )
+                assert expect_value == new_value, f"type({celltype})"
+
+    @pytest.mark.parametrize(
+        ("celltype", "minval", "maxval"),
+        [
+            (CellType.BITS, 50, 75),
+            (CellType.UINT16, 50, 15075),
+            (CellType.UINT32, 50, 63075),
+            (CellType.FLOAT32, 27.0, 16100.5),
+            (CellType.FLOAT32, 65.0, 78.0),
+        ],
+    )
+    def test_simulator_action_random(self, celltype, minval, maxval):
+        """Test action random"""
+        exc_setup = copy.deepcopy(self.default_config)
+        exc_simulator = ModbusSimulatorContext(exc_setup, None)
+        action = exc_simulator.action_name_to_id[Label.random]
+        kwargs = {
+            "minval": minval,
+            "maxval": maxval,
+        }
+        exc_simulator.registers[30].type = celltype
+        exc_simulator.registers[30].action = action
+        exc_simulator.registers[30].action_kwargs = kwargs
+        exc_simulator.registers[31].type = CellType.NEXT
+        is_int = celltype != CellType.FLOAT32
+        reg_count = 1 if celltype in (CellType.BITS, CellType.UINT16) else 2
+        for _i in range(100):
+            regs = exc_simulator.getValues(FX_READ_REG, 30, reg_count)
+            if reg_count == 1:
+                new_value = regs[0]
+            else:
+                new_value = ModbusSimulatorContext.build_value_from_registers(
+                    regs, is_int
+                )
+            assert minval <= new_value <= maxval
+
+    @patch(
+        "builtins.open",
+        mock_open(
+            read_data=json.dumps(
+                {
+                    "server_list": default_server_config,
+                    "device_list": {"device": default_config},
+                }
+            )
+        ),
+    )
+    async def test_simulator_server_tcp(self):
+        """Test init simulator server"""
+        task = ModbusSimulatorServer()
+        await task.run_forever(only_start=True)
+        await asyncio.sleep(5)
+        await task.stop()
```

### Comparing `pymodbus-3.3.2/test/test_sparse_datastore.py` & `pymodbus-3.4.0/test/test_sparse_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.2/test/test_transaction.py` & `pymodbus-3.4.0/test/test_transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -283,97 +283,97 @@
     # TCP tests
     # ----------------------------------------------------------------------- #
     def test_tcp_framer_transaction_ready(self):
         """Test a tcp frame transaction"""
         msg = b"\x00\x01\x12\x34\x00\x04\xff\x02\x12\x34"
         assert not self._tcp.isFrameReady()
         assert not self._tcp.checkFrame()
-        self._tcp.addToFrame(msg)
+        self._tcp._buffer = msg  # pylint: disable=protected-access
         assert self._tcp.isFrameReady()
         assert self._tcp.checkFrame()
         self._tcp.advanceFrame()
         assert not self._tcp.isFrameReady()
         assert not self._tcp.checkFrame()
         assert self._ascii.getFrame() == b""
 
     def test_tcp_framer_transaction_full(self):
         """Test a full tcp frame transaction"""
         msg = b"\x00\x01\x12\x34\x00\x04\xff\x02\x12\x34"
-        self._tcp.addToFrame(msg)
+        self._tcp._buffer = msg  # pylint: disable=protected-access
         assert self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == msg[7:]
         self._tcp.advanceFrame()
 
     def test_tcp_framer_transaction_half(self):
         """Test a half completed tcp frame transaction"""
         msg1 = b"\x00\x01\x12\x34\x00"
         msg2 = b"\x04\xff\x02\x12\x34"
-        self._tcp.addToFrame(msg1)
+        self._tcp._buffer = msg1  # pylint: disable=protected-access
         assert not self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == b""
-        self._tcp.addToFrame(msg2)
+        self._tcp._buffer += msg2
         assert self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == msg2[2:]
         self._tcp.advanceFrame()
 
     def test_tcp_framer_transaction_half2(self):
         """Test a half completed tcp frame transaction"""
         msg1 = b"\x00\x01\x12\x34\x00\x04\xff"
         msg2 = b"\x02\x12\x34"
-        self._tcp.addToFrame(msg1)
+        self._tcp._buffer = msg1  # pylint: disable=protected-access
         assert not self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == b""
-        self._tcp.addToFrame(msg2)
+        self._tcp._buffer += msg2
         assert self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert msg2 == result
         self._tcp.advanceFrame()
 
     def test_tcp_framer_transaction_half3(self):
         """Test a half completed tcp frame transaction"""
         msg1 = b"\x00\x01\x12\x34\x00\x04\xff\x02\x12"
         msg2 = b"\x34"
-        self._tcp.addToFrame(msg1)
+        self._tcp._buffer = msg1  # pylint: disable=protected-access
         assert not self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == msg1[7:]
-        self._tcp.addToFrame(msg2)
+        self._tcp._buffer += msg2
         assert self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == msg1[7:] + msg2
         self._tcp.advanceFrame()
 
     def test_tcp_framer_transaction_short(self):
         """Test that we can get back on track after an invalid message"""
         msg1 = b"\x99\x99\x99\x99\x00\x01\x00\x01"
         msg2 = b"\x00\x01\x12\x34\x00\x04\xff\x02\x12\x34"
-        self._tcp.addToFrame(msg1)
+        self._tcp._buffer = msg1  # pylint: disable=protected-access
         assert not self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == b""
         self._tcp.advanceFrame()
-        self._tcp.addToFrame(msg2)
+        self._tcp._buffer += msg2
         assert len(self._tcp._buffer) == 10  # pylint: disable=protected-access
         assert self._tcp.checkFrame()
         result = self._tcp.getFrame()
         assert result == msg2[7:]
         self._tcp.advanceFrame()
 
     def test_tcp_framer_populate(self):
         """Test a tcp frame packet build"""
         expected = ModbusRequest()
         expected.transaction_id = 0x0001
         expected.protocol_id = 0x1234
         expected.slave_id = 0xFF
         msg = b"\x00\x01\x12\x34\x00\x04\xff\x02\x12\x34"
-        self._tcp.addToFrame(msg)
+        self._tcp._buffer = msg  # pylint: disable=protected-access
         assert self._tcp.checkFrame()
         actual = ModbusRequest()
         self._tcp.populateResult(actual)
         for name in ("transaction_id", "protocol_id", "slave_id"):
             assert getattr(expected, name) == getattr(actual, name)
         self._tcp.advanceFrame()
 
@@ -395,55 +395,55 @@
     # TLS tests
     # ----------------------------------------------------------------------- #
     def test_framer_tls_framer_transaction_ready(self):
         """Test a tls frame transaction"""
         msg = b"\x01\x12\x34\x00\x08"
         assert not self._tls.isFrameReady()
         assert not self._tls.checkFrame()
-        self._tls.addToFrame(msg)
+        self._tls._buffer = msg  # pylint: disable=protected-access
         assert self._tls.isFrameReady()
         assert self._tls.checkFrame()
         self._tls.advanceFrame()
         assert not self._tls.isFrameReady()
         assert not self._tls.checkFrame()
         assert self._tls.getFrame() == b""
 
     def test_framer_tls_framer_transaction_full(self):
         """Test a full tls frame transaction"""
         msg = b"\x01\x12\x34\x00\x08"
-        self._tls.addToFrame(msg)
+        self._tls._buffer = msg  # pylint: disable=protected-access
         assert self._tls.checkFrame()
         result = self._tls.getFrame()
         assert result == msg[0:]
         self._tls.advanceFrame()
 
     def test_framer_tls_framer_transaction_half(self):
         """Test a half completed tls frame transaction"""
         msg1 = b""
         msg2 = b"\x01\x12\x34\x00\x08"
-        self._tls.addToFrame(msg1)
+        self._tls._buffer = msg1  # pylint: disable=protected-access
         assert not self._tls.checkFrame()
         result = self._tls.getFrame()
         assert result == b""
-        self._tls.addToFrame(msg2)
+        self._tls._buffer += msg2
         assert self._tls.checkFrame()
         result = self._tls.getFrame()
         assert result == msg2[0:]
         self._tls.advanceFrame()
 
     def test_framer_tls_framer_transaction_short(self):
         """Test that we can get back on track after an invalid message"""
         msg1 = b""
         msg2 = b"\x01\x12\x34\x00\x08"
-        self._tls.addToFrame(msg1)
+        self._tls._buffer = msg1  # pylint: disable=protected-access
         assert not self._tls.checkFrame()
         result = self._tls.getFrame()
         assert result == b""
         self._tls.advanceFrame()
-        self._tls.addToFrame(msg2)
+        self._tls._buffer = msg2  # pylint: disable=protected-access
         assert len(self._tls._buffer) == 5  # pylint: disable=protected-access
         assert self._tls.checkFrame()
         result = self._tls.getFrame()
         assert result == msg2[0:]
         self._tls.advanceFrame()
 
     def test_framer_tls_framer_decode(self):
@@ -464,27 +464,27 @@
 
         def mock_callback():
             """Mock callback."""
 
         self._tls._process = mock.MagicMock()  # pylint: disable=protected-access
         self._tls.isFrameReady = mock.MagicMock(return_value=False)
         self._tls.processIncomingPacket(msg, mock_callback, slave)
-        assert msg == self._tls.getRawFrame()
+        assert msg == self._tls._buffer  # pylint: disable=protected-access
         self._tls.advanceFrame()
 
         self._tls.isFrameReady = mock.MagicMock(return_value=True)
         x = mock.MagicMock(return_value=False)
         self._tls._validate_slave_id = x  # pylint: disable=protected-access
         self._tls.processIncomingPacket(msg, mock_callback, slave)
-        assert not self._tls.getRawFrame()
+        assert not self._tls._buffer  # pylint: disable=protected-access
         self._tls.advanceFrame()
         x = mock.MagicMock(return_value=True)
         self._tls._validate_slave_id = x  # pylint: disable=protected-access
         self._tls.processIncomingPacket(msg, mock_callback, slave)
-        assert msg == self._tls.getRawFrame()
+        assert msg == self._tls._buffer  # pylint: disable=protected-access
         self._tls.advanceFrame()
 
     def test_framer_tls_process(self):
         """Framer tls process."""
 
         class MockResult:  # pylint: disable=too-few-public-methods
             """Mock result."""
@@ -503,27 +503,24 @@
         result = MockResult(0x01)
         self._tls.decoder.decode = mock.MagicMock(return_value=result)
         with pytest.raises(InvalidMessageReceivedException):
             self._tls._process(  # pylint: disable=protected-access
                 mock_callback, error=True
             )
         self._tls._process(mock_callback)  # pylint: disable=protected-access
-        assert not self._tls.getRawFrame()
+        assert not self._tls._buffer  # pylint: disable=protected-access
 
     def test_framer_tls_framer_populate(self):
         """Test a tls frame packet build"""
         ModbusRequest()
         msg = b"\x01\x12\x34\x00\x08"
-        self._tls.addToFrame(msg)
+        self._tls._buffer = msg  # pylint: disable=protected-access
         assert self._tls.checkFrame()
         actual = ModbusRequest()
-        result = self._tls.populateResult(  # pylint: disable=assignment-from-none
-            actual
-        )
-        assert not result
+        self._tls.populateResult(actual)
         self._tls.advanceFrame()
 
     def test_framer_tls_framer_packet(self):
         """Test a tls frame packet build"""
         old_encode = ModbusRequest.encode
         ModbusRequest.encode = lambda self: b""
         message = ModbusRequest()
@@ -537,50 +534,50 @@
     # RTU tests
     # ----------------------------------------------------------------------- #
     def test_rtu_framer_transaction_ready(self):
         """Test if the checks for a complete frame work"""
         assert not self._rtu.isFrameReady()
 
         msg_parts = [b"\x00\x01\x00", b"\x00\x00\x01\xfc\x1b"]
-        self._rtu.addToFrame(msg_parts[0])
+        self._rtu._buffer = msg_parts[0]  # pylint: disable=protected-access
         assert not self._rtu.isFrameReady()
         assert not self._rtu.checkFrame()
 
-        self._rtu.addToFrame(msg_parts[1])
+        self._rtu._buffer += msg_parts[1]
         assert self._rtu.isFrameReady()
         assert self._rtu.checkFrame()
 
     def test_rtu_framer_transaction_full(self):
         """Test a full rtu frame transaction"""
         msg = b"\x00\x01\x00\x00\x00\x01\xfc\x1b"
         stripped_msg = msg[1:-2]
-        self._rtu.addToFrame(msg)
+        self._rtu._buffer = msg  # pylint: disable=protected-access
         assert self._rtu.checkFrame()
         result = self._rtu.getFrame()
         assert stripped_msg == result
         self._rtu.advanceFrame()
 
     def test_rtu_framer_transaction_half(self):
         """Test a half completed rtu frame transaction"""
         msg_parts = [b"\x00\x01\x00", b"\x00\x00\x01\xfc\x1b"]
         stripped_msg = b"".join(msg_parts)[1:-2]
-        self._rtu.addToFrame(msg_parts[0])
+        self._rtu._buffer = msg_parts[0]  # pylint: disable=protected-access
         assert not self._rtu.checkFrame()
-        self._rtu.addToFrame(msg_parts[1])
+        self._rtu._buffer += msg_parts[1]
         assert self._rtu.isFrameReady()
         assert self._rtu.checkFrame()
         result = self._rtu.getFrame()
         assert stripped_msg == result
         self._rtu.advanceFrame()
 
     def test_rtu_framer_populate(self):
         """Test a rtu frame packet build"""
         request = ModbusRequest()
         msg = b"\x00\x01\x00\x00\x00\x01\xfc\x1b"
-        self._rtu.addToFrame(msg)
+        self._rtu._buffer = msg  # pylint: disable=protected-access
         self._rtu.populateHeader()
         self._rtu.populateResult(request)
 
         header_dict = self._rtu._header  # pylint: disable=protected-access
         assert len(msg) == header_dict["len"]
         assert int(msg[0]) == header_dict["uid"]
         assert msg[-2:] == header_dict["crc"]
@@ -597,15 +594,15 @@
         actual = self._rtu.buildPacket(message)
         assert expected == actual
         ModbusRequest.encode = old_encode
 
     def test_rtu_decode_exception(self):
         """Test that the RTU framer can decode errors"""
         message = b"\x00\x90\x02\x9c\x01"
-        self._rtu.addToFrame(message)
+        self._rtu._buffer = message  # pylint: disable=protected-access
         result = self._rtu.checkFrame()
         assert result
 
     def test_process(self):
         """Test process."""
 
         class MockResult:  # pylint: disable=too-few-public-methods
@@ -614,15 +611,15 @@
             def __init__(self, code):
                 self.function_code = code
 
         def mock_callback(_arg):
             """Mock callback."""
 
         mock_result = MockResult(code=0)
-        self._rtu.getRawFrame = self._rtu.getFrame = mock.MagicMock()
+        self._rtu.getFrame = mock.MagicMock()
         self._rtu.decoder = mock.MagicMock()
         self._rtu.decoder.decode = mock.MagicMock(return_value=mock_result)
         self._rtu.populateResult = mock.MagicMock()
         self._rtu.advanceFrame = mock.MagicMock()
 
         self._rtu._process(mock_callback)  # pylint: disable=protected-access
         self._rtu.populateResult.assert_called_with(mock_result)
@@ -638,57 +635,57 @@
         """Test rtu process incoming packets."""
         mock_data = b"\x00\x01\x00\x00\x00\x01\xfc\x1b"
         slave = 0x00
 
         def mock_callback():
             """Mock callback."""
 
-        self._rtu.addToFrame = mock.MagicMock()
+        self._rtu._buffer = mock.MagicMock()  # pylint: disable=protected-access
         self._rtu._process = mock.MagicMock()  # pylint: disable=protected-access
         self._rtu.isFrameReady = mock.MagicMock(return_value=False)
         self._rtu._buffer = mock_data  # pylint: disable=protected-access
 
         self._rtu.processIncomingPacket(mock_data, mock_callback, slave)
 
     # ----------------------------------------------------------------------- #
     # ASCII tests
     # ----------------------------------------------------------------------- #
     def test_ascii_framer_transaction_ready(self):
         """Test a ascii frame transaction"""
         msg = b":F7031389000A60\r\n"
         assert not self._ascii.isFrameReady()
         assert not self._ascii.checkFrame()
-        self._ascii.addToFrame(msg)
+        self._ascii._buffer = msg  # pylint: disable=protected-access
         assert self._ascii.isFrameReady()
         assert self._ascii.checkFrame()
         self._ascii.advanceFrame()
         assert not self._ascii.isFrameReady()
         assert not self._ascii.checkFrame()
         assert not self._ascii.getFrame()
 
     def test_ascii_framer_transaction_full(self):
         """Test a full ascii frame transaction"""
         msg = b"sss:F7031389000A60\r\n"
         pack = a2b_hex(msg[6:-4])
-        self._ascii.addToFrame(msg)
+        self._ascii._buffer = msg  # pylint: disable=protected-access
         assert self._ascii.checkFrame()
         result = self._ascii.getFrame()
         assert pack == result
         self._ascii.advanceFrame()
 
     def test_ascii_framer_transaction_half(self):
         """Test a half completed ascii frame transaction"""
         msg1 = b"sss:F7031389"
         msg2 = b"000A60\r\n"
         pack = a2b_hex(msg1[6:] + msg2[:-4])
-        self._ascii.addToFrame(msg1)
+        self._ascii._buffer = msg1  # pylint: disable=protected-access
         assert not self._ascii.checkFrame()
         result = self._ascii.getFrame()
         assert not result
-        self._ascii.addToFrame(msg2)
+        self._ascii._buffer += msg2
         assert self._ascii.checkFrame()
         result = self._ascii.getFrame()
         assert pack == result
         self._ascii.advanceFrame()
 
     def test_ascii_framer_populate(self):
         """Test a ascii frame packet build"""
@@ -726,42 +723,43 @@
     # Binary tests
     # ----------------------------------------------------------------------- #
     def test_binary_framer_transaction_ready(self):
         """Test a binary frame transaction"""
         msg = TEST_MESSAGE
         assert not self._binary.isFrameReady()
         assert not self._binary.checkFrame()
-        self._binary.addToFrame(msg)
+        self._binary._buffer = msg  # pylint: disable=protected-access
         assert self._binary.isFrameReady()
         assert self._binary.checkFrame()
         self._binary.advanceFrame()
         assert not self._binary.isFrameReady()
         assert not self._binary.checkFrame()
         assert not self._binary.getFrame()
 
     def test_binary_framer_transaction_full(self):
         """Test a full binary frame transaction"""
         msg = TEST_MESSAGE
         pack = msg[2:-3]
-        self._binary.addToFrame(msg)
+        self._binary._buffer = msg  # pylint: disable=protected-access
         assert self._binary.checkFrame()
         result = self._binary.getFrame()
         assert pack == result
         self._binary.advanceFrame()
 
     def test_binary_framer_transaction_half(self):
         """Test a half completed binary frame transaction"""
         msg1 = b"\x7b\x01\x03\x00"
         msg2 = b"\x00\x00\x05\x85\xC9\x7d"
         pack = msg1[2:] + msg2[:-3]
-        self._binary.addToFrame(msg1)
+        self._binary._buffer = msg1  # pylint: disable=protected-access
         assert not self._binary.checkFrame()
         result = self._binary.getFrame()
         assert not result
-        self._binary.addToFrame(msg2)
+        self._binary._buffer += msg2
+
         assert self._binary.checkFrame()
         result = self._binary.getFrame()
         assert pack == result
         self._binary.advanceFrame()
 
     def test_binary_framer_populate(self):
         """Test a binary frame packet build"""
```

### Comparing `pymodbus-3.3.2/test/test_utilities.py` & `pymodbus-3.4.0/test/test_utilities.py`

 * *Files identical despite different names*

