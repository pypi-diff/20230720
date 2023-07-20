# Comparing `tmp/micropython_hints-0.0.6.tar.gz` & `tmp/micropython_hints-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_hints-0.0.6.tar", last modified: Thu Jul 20 12:35:47 2023, max compression
+gzip compressed data, was "micropython_hints-0.0.7.tar", last modified: Thu Jul 20 12:38:20 2023, max compression
```

## Comparing `micropython_hints-0.0.6.tar` & `micropython_hints-0.0.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:35:47.506344 micropython_hints-0.0.6/
--rw-r--r--   0 meo       (1000) meo       (1000)      720 2023-07-20 12:35:47.506344 micropython_hints-0.0.6/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      297 2023-07-20 12:31:43.000000 micropython_hints-0.0.6/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:35:47.506344 micropython_hints-0.0.6/micropython_hints/
--rw-r--r--   0 meo       (1000) meo       (1000)     1818 2023-07-20 12:27:28.000000 micropython_hints-0.0.6/micropython_hints/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      697 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/_thread.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/array.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/binascii.py
--rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/bluetooth.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8754 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/btree.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1976 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/cmath.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/collections.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/cryptolib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/errno.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8518 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/esp.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18158 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/esp32.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8369 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/framebuf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3948 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/gc.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/hashlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/heapq.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/json.py
--rw-r--r--   0 meo       (1000) meo       (1000)    21847 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/lcd160cr.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4002 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/machine.ADCWiPy.py
--rw-r--r--   0 meo       (1000) meo       (1000)    12210 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/machine.TimerWiPy.py
--rw-r--r--   0 meo       (1000) meo       (1000)   102731 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/machine.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5209 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/math.py
--rw-r--r--   0 meo       (1000) meo       (1000)    11660 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/micropython.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2552 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/neopixel.py
--rw-r--r--   0 meo       (1000) meo       (1000)    35185 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/network.py
--rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/os.py
--rw-r--r--   0 meo       (1000) meo       (1000)   183891 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/pyb.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4298 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/random.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/re.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/select.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/socket.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ssl.py
--rw-r--r--   0 meo       (1000) meo       (1000)     7730 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/stm.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/struct.py
--rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/sys.py
--rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/time.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uarray.py
--rw-r--r--   0 meo       (1000) meo       (1000)    12303 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uasyncio.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ubinascii.py
--rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ubluetooth.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ucollections.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ucryptolib.py
--rw-r--r--   0 meo       (1000) meo       (1000)    11686 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uctypes.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uerrno.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uhashlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uheapq.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uio.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ujson.py
--rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uos.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ure.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uselect.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/usocket.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ussl.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/ustruct.py
--rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/usys.py
--rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/utime.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/uzlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)      993 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/wipy.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-20 11:50:39.000000 micropython_hints-0.0.6/micropython_hints/zlib.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:35:47.506344 micropython_hints-0.0.6/micropython_hints.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      720 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)     1958 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       94 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/entry_points.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       17 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       18 2023-07-20 12:35:47.000000 micropython_hints-0.0.6/micropython_hints.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-20 12:35:47.506344 micropython_hints-0.0.6/setup.cfg
--rw-r--r--   0 meo       (1000) meo       (1000)     1366 2023-07-20 12:33:13.000000 micropython_hints-0.0.6/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:38:20.792169 micropython_hints-0.0.7/
+-rw-r--r--   0 meo       (1000) meo       (1000)      720 2023-07-20 12:38:20.792169 micropython_hints-0.0.7/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      297 2023-07-20 12:31:43.000000 micropython_hints-0.0.7/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:38:20.788836 micropython_hints-0.0.7/micropython_hints/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1818 2023-07-20 12:27:28.000000 micropython_hints-0.0.7/micropython_hints/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      697 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/_thread.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/array.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/binascii.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/bluetooth.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8754 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/btree.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1976 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/cmath.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/collections.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/cryptolib.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/errno.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8518 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/esp.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    18158 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/esp32.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8369 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/framebuf.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3948 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/gc.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/hashlib.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/heapq.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/json.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    21847 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/lcd160cr.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     4002 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/machine.ADCWiPy.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    12210 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/machine.TimerWiPy.py
+-rw-r--r--   0 meo       (1000) meo       (1000)   102731 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/machine.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5209 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/math.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    11660 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/micropython.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2552 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/neopixel.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    35185 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/network.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/os.py
+-rw-r--r--   0 meo       (1000) meo       (1000)   183891 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/pyb.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     4298 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/random.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/re.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/select.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/socket.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ssl.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     7730 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/stm.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/struct.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/sys.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/time.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uarray.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    12303 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uasyncio.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ubinascii.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ubluetooth.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ucollections.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ucryptolib.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    11686 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uctypes.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uerrno.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uhashlib.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uheapq.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uio.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ujson.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uos.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ure.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uselect.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/usocket.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ussl.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/ustruct.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/usys.py
+-rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/utime.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/uzlib.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      993 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/wipy.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-20 11:50:39.000000 micropython_hints-0.0.7/micropython_hints/zlib.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-20 12:38:20.792169 micropython_hints-0.0.7/micropython_hints.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      720 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)     1958 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       94 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/entry_points.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       17 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       18 2023-07-20 12:38:20.000000 micropython_hints-0.0.7/micropython_hints.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-20 12:38:20.792169 micropython_hints-0.0.7/setup.cfg
+-rw-r--r--   0 meo       (1000) meo       (1000)     1366 2023-07-20 12:38:13.000000 micropython_hints-0.0.7/setup.py
```

### Comparing `micropython_hints-0.0.6/PKG-INFO` & `micropython_hints-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: micropython_hints
-Version: 0.0.6
+Version: 0.0.7
 Summary: MicroPython type hints
-Home-page: https://github.com/miaobuao/micropython_hints
+Home-page: https://github.com/ITA-ZUFE/micropython_hints
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `micropython_hints-0.0.6/micropython_hints/__init__.py` & `micropython_hints-0.0.7/micropython_hints/__init__.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/_thread.py` & `micropython_hints-0.0.7/micropython_hints/_thread.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/array.py` & `micropython_hints-0.0.7/micropython_hints/array.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/binascii.py` & `micropython_hints-0.0.7/micropython_hints/binascii.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/bluetooth.py` & `micropython_hints-0.0.7/micropython_hints/bluetooth.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/btree.py` & `micropython_hints-0.0.7/micropython_hints/btree.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/cmath.py` & `micropython_hints-0.0.7/micropython_hints/cmath.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/collections.py` & `micropython_hints-0.0.7/micropython_hints/collections.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/cryptolib.py` & `micropython_hints-0.0.7/micropython_hints/cryptolib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/errno.py` & `micropython_hints-0.0.7/micropython_hints/errno.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/esp.py` & `micropython_hints-0.0.7/micropython_hints/esp.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/esp32.py` & `micropython_hints-0.0.7/micropython_hints/esp32.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/framebuf.py` & `micropython_hints-0.0.7/micropython_hints/framebuf.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/gc.py` & `micropython_hints-0.0.7/micropython_hints/gc.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/hashlib.py` & `micropython_hints-0.0.7/micropython_hints/hashlib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/heapq.py` & `micropython_hints-0.0.7/micropython_hints/heapq.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/io.py` & `micropython_hints-0.0.7/micropython_hints/io.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/json.py` & `micropython_hints-0.0.7/micropython_hints/json.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/lcd160cr.py` & `micropython_hints-0.0.7/micropython_hints/lcd160cr.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/machine.ADCWiPy.py` & `micropython_hints-0.0.7/micropython_hints/machine.ADCWiPy.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/machine.TimerWiPy.py` & `micropython_hints-0.0.7/micropython_hints/machine.TimerWiPy.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/machine.py` & `micropython_hints-0.0.7/micropython_hints/machine.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/math.py` & `micropython_hints-0.0.7/micropython_hints/math.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/micropython.py` & `micropython_hints-0.0.7/micropython_hints/micropython.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/neopixel.py` & `micropython_hints-0.0.7/micropython_hints/neopixel.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/network.py` & `micropython_hints-0.0.7/micropython_hints/network.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/os.py` & `micropython_hints-0.0.7/micropython_hints/os.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/pyb.py` & `micropython_hints-0.0.7/micropython_hints/pyb.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/random.py` & `micropython_hints-0.0.7/micropython_hints/random.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/re.py` & `micropython_hints-0.0.7/micropython_hints/re.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/select.py` & `micropython_hints-0.0.7/micropython_hints/select.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/socket.py` & `micropython_hints-0.0.7/micropython_hints/socket.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ssl.py` & `micropython_hints-0.0.7/micropython_hints/ssl.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/stm.py` & `micropython_hints-0.0.7/micropython_hints/stm.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/struct.py` & `micropython_hints-0.0.7/micropython_hints/struct.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/sys.py` & `micropython_hints-0.0.7/micropython_hints/sys.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/time.py` & `micropython_hints-0.0.7/micropython_hints/time.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uarray.py` & `micropython_hints-0.0.7/micropython_hints/uarray.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uasyncio.py` & `micropython_hints-0.0.7/micropython_hints/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ubinascii.py` & `micropython_hints-0.0.7/micropython_hints/ubinascii.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ubluetooth.py` & `micropython_hints-0.0.7/micropython_hints/ubluetooth.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ucollections.py` & `micropython_hints-0.0.7/micropython_hints/ucollections.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ucryptolib.py` & `micropython_hints-0.0.7/micropython_hints/ucryptolib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uctypes.py` & `micropython_hints-0.0.7/micropython_hints/uctypes.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uerrno.py` & `micropython_hints-0.0.7/micropython_hints/uerrno.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uhashlib.py` & `micropython_hints-0.0.7/micropython_hints/uhashlib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uheapq.py` & `micropython_hints-0.0.7/micropython_hints/uheapq.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uio.py` & `micropython_hints-0.0.7/micropython_hints/uio.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ujson.py` & `micropython_hints-0.0.7/micropython_hints/ujson.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uos.py` & `micropython_hints-0.0.7/micropython_hints/uos.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ure.py` & `micropython_hints-0.0.7/micropython_hints/ure.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uselect.py` & `micropython_hints-0.0.7/micropython_hints/uselect.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/usocket.py` & `micropython_hints-0.0.7/micropython_hints/usocket.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ussl.py` & `micropython_hints-0.0.7/micropython_hints/ussl.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/ustruct.py` & `micropython_hints-0.0.7/micropython_hints/ustruct.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/usys.py` & `micropython_hints-0.0.7/micropython_hints/usys.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/utime.py` & `micropython_hints-0.0.7/micropython_hints/utime.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/uzlib.py` & `micropython_hints-0.0.7/micropython_hints/uzlib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/wipy.py` & `micropython_hints-0.0.7/micropython_hints/wipy.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints/zlib.py` & `micropython_hints-0.0.7/micropython_hints/zlib.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/micropython_hints.egg-info/PKG-INFO` & `micropython_hints-0.0.7/micropython_hints.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: micropython-hints
-Version: 0.0.6
+Version: 0.0.7
 Summary: MicroPython type hints
-Home-page: https://github.com/miaobuao/micropython_hints
+Home-page: https://github.com/ITA-ZUFE/micropython_hints
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `micropython_hints-0.0.6/micropython_hints.egg-info/SOURCES.txt` & `micropython_hints-0.0.7/micropython_hints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.6/setup.py` & `micropython_hints-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 if os.path.isdir(path):
     print("INFO DEL DIR ", path)
     shutil.rmtree(path)
 
 with open(os.path.join(CUR_PATH, "README.md"), 'r+', encoding='utf8') as f:
     long_description = f.read()
 
-URL = f"https://github.com/miaobuao/{PROJ_NAME}"
+URL = f"https://github.com/ITA-ZUFE/{PROJ_NAME}"
 
 setup(
     name         = PROJ_NAME,
     author       =  "miaobuao",
     url          =  URL,
     description  =  "MicroPython type hints",
-    version      =  "0.0.6",
+    version      =  "0.0.7",
     license      =  "MIT License",
     author_email =  "miaobuao@outlook.com",
     long_description     = long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

