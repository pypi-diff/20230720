# Comparing `tmp/nobuco-0.5.8.tar.gz` & `tmp/nobuco-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.8.tar", last modified: Tue Jul 11 12:48:10 2023, max compression
+gzip compressed data, was "nobuco-0.6.0.tar", last modified: Thu Jul 20 18:31:09 2023, max compression
```

## Comparing `nobuco-0.5.8.tar` & `nobuco-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.211155 nobuco-0.5.8/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.8/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-11 12:48:10.211155 nobuco-0.5.8/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.5.8/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.5.8/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.8/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.8/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.8/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.211155 nobuco-0.5.8/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14555 2023-07-11 12:33:40.000000 nobuco-0.5.8/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.5.8/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-07-11 12:35:48.000000 nobuco-0.5.8/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.211155 nobuco-0.5.8/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-07-01 10:07:17.000000 nobuco-0.5.8/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.211155 nobuco-0.5.8/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.8/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 12:48:10.207155 nobuco-0.5.8/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-11 12:48:10.000000 nobuco-0.5.8/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-11 12:48:10.000000 nobuco-0.5.8/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 12:48:10.000000 nobuco-0.5.8/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-11 12:48:10.000000 nobuco-0.5.8/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-11 12:48:10.000000 nobuco-0.5.8/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-11 12:39:33.000000 nobuco-0.5.8/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-11 12:48:10.211155 nobuco-0.5.8/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.457288 nobuco-0.6.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-20 18:31:09.457288 nobuco-0.6.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.6.0/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.0/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.0/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1360 2023-07-20 18:20:30.000000 nobuco-0.6.0/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.6.0/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.0/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.453288 nobuco-0.6.0/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14555 2023-07-11 12:33:40.000000 nobuco-0.6.0/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.0/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-07-11 12:35:48.000000 nobuco-0.6.0/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.453288 nobuco-0.6.0/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.0/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-20 10:14:17.000000 nobuco-0.6.0/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.457288 nobuco-0.6.0/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.0/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 18:31:09.449288 nobuco-0.6.0/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-20 18:31:09.000000 nobuco-0.6.0/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-20 18:26:47.000000 nobuco-0.6.0/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-20 18:31:09.457288 nobuco-0.6.0/setup.cfg
```

### Comparing `nobuco-0.5.8/LICENSE` & `nobuco-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/PKG-INFO` & `nobuco-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.8
+Version: 0.6.0
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.5.8/README.md` & `nobuco-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/__init__.py` & `nobuco-0.6.0/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/commons.py` & `nobuco-0.6.0/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/convert.py` & `nobuco-0.6.0/nobuco/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import time
 import traceback
 import warnings
 from typing import Callable, Dict, Collection, Optional, List, Union, Tuple
 
 import torch
 from nobuco.converters.tensor import permute_pytorch2keras
@@ -240,25 +242,25 @@
 
 
 def pytorch_to_keras(
         module: nn.Module,
         args: List[object] = None,
         kwargs: Dict[str, object] = None,
         input_shapes: Dict[torch.Tensor, Collection[Optional[int]]] = None,
-        inputs_channel_order: Union[ChannelOrder, Dict[torch.Tensor, ChannelOrder]] = ChannelOrder.TENSORFLOW,
-        outputs_channel_order: Union[ChannelOrder, Dict[int, ChannelOrder]] = None,
+        inputs_channel_order: ChannelOrder | Dict[torch.Tensor, ChannelOrder] = ChannelOrder.TENSORFLOW,
+        outputs_channel_order: ChannelOrder | Dict[int, ChannelOrder] = None,
         converter_dict=CONVERTER_DICT,
         trace_shape: bool = False,
         constants_to_variables: bool = True,
         full_validation: bool = True,
         validation_tolerance=1e-4,
         save_trace_html: bool = False,
         return_outputs_pt: bool = False,
         debug_traces: TraceLevel = TraceLevel.DEFAULT,
-) -> Union[keras.Model, Tuple[keras.Model, object]]:
+) -> keras.Model | Tuple[keras.Model, object]:
 
     if args is None:
         args = []
 
     if kwargs is None:
         kwargs = {}
```

### Comparing `nobuco-0.5.8/nobuco/converters/channel_ordering.py` & `nobuco-0.6.0/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/converters/node_converter.py` & `nobuco-0.6.0/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/converters/tensor.py` & `nobuco-0.6.0/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/converters/type_cast.py` & `nobuco-0.6.0/nobuco/converters/type_cast.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 import tensorflow as tf
 
 from nobuco.commons import TF_TENSOR_CLASSES
 from nobuco.util import collect_recursively, replace_recursively_func
 
 TF_TYPE_PRIORITY_LIST = [
+    tf.complex128,
+    tf.complex64,
+
     tf.float64,
     tf.float32,
     # tf.float16,
     tf.int32,
     tf.int64,
     # tf.int16,
     # tf.int8,
```

### Comparing `nobuco-0.5.8/nobuco/converters/validation.py` & `nobuco-0.6.0/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/entity/keras.py` & `nobuco-0.6.0/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/entity/pytorch.py` & `nobuco-0.6.0/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/funcs.py` & `nobuco-0.6.0/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/layers/channel_order.py` & `nobuco-0.6.0/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/layers/container.py` & `nobuco-0.6.0/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/locate/link.py` & `nobuco-0.6.0/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/locate/locate.py` & `nobuco-0.6.0/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/activation.py` & `nobuco-0.6.0/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/attention.py` & `nobuco-0.6.0/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/boolean.py` & `nobuco-0.6.0/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/boolean_mask.py` & `nobuco-0.6.0/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/comparison.py` & `nobuco-0.6.0/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/convolution.py` & `nobuco-0.6.0/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/dropout.py` & `nobuco-0.6.0/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/interpolation.py` & `nobuco-0.6.0/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/linear.py` & `nobuco-0.6.0/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/math.py` & `nobuco-0.6.0/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/misc.py` & `nobuco-0.6.0/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/normalization.py` & `nobuco-0.6.0/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/padding.py` & `nobuco-0.6.0/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/pooling.py` & `nobuco-0.6.0/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/recurrent.py` & `nobuco-0.6.0/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/slice.py` & `nobuco-0.6.0/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/tensor_cast.py` & `nobuco-0.6.0/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/tensor_creation.py` & `nobuco-0.6.0/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.6.0/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/trace/tensor_storage.py` & `nobuco-0.6.0/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/trace/trace.py` & `nobuco-0.6.0/nobuco/trace/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import inspect
 import traceback
 import types
 from copy import deepcopy
 from typing import List, Collection, Callable, Union
 
 import torch
@@ -201,15 +203,15 @@
 
         for op_cls, op in Tracer.op_whitelist:
             if not Tracer.is_decorated(op):
                 decorated = Tracer.op_tracing_decorator(op, op_cls, is_whitelist_op=True)
                 setattr(op_cls, op.__name__, decorated)
 
     @staticmethod
-    def trace(module_or_function: Union[nn.Module, Callable], trace_shape: bool, args, kwargs) -> PytorchNodeHierarchy:
+    def trace(module_or_function: nn.Module | Callable, trace_shape: bool, args, kwargs) -> PytorchNodeHierarchy:
         Tracer._trace_shape = trace_shape
 
         ### Module tracing routines
         def apply_module_tracing_recursively(module):
             for child in module.children():
                 apply_module_tracing_recursively(child)
```

### Comparing `nobuco-0.5.8/nobuco/util.py` & `nobuco-0.6.0/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/vis/console_stylizer.py` & `nobuco-0.6.0/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco/vis/html_stylizer.py` & `nobuco-0.6.0/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/nobuco.egg-info/PKG-INFO` & `nobuco-0.6.0/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.8
+Version: 0.6.0
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.5.8/nobuco.egg-info/SOURCES.txt` & `nobuco-0.6.0/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.8/pyproject.toml` & `nobuco-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.8"
+version = "0.6.0"
 description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

