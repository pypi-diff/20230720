# Comparing `tmp/types-six-1.16.8.tar.gz` & `tmp/types-six-1.16.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-six-1.16.8.tar", last modified: Fri Jan  7 11:32:32 2022, max compression
+gzip compressed data, was "types-six-1.16.9.tar", last modified: Sat Jan  8 15:20:31 2022, max compression
```

## Comparing `types-six-1.16.8.tar` & `types-six-1.16.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.521479 types-six-1.16.8/
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-01-07 11:32:31.000000 types-six-1.16.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:32:31.000000 types-six-1.16.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-07 11:32:32.521479 types-six-1.16.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:32:32.521479 types-six-1.16.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-01-07 11:32:31.000000 types-six-1.16.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.513478 types-six-1.16.8/six-python2-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-07 11:32:31.000000 types-six-1.16.8/six-python2-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.517479 types-six-1.16.8/six-python2-stubs/moves/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/BaseHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/CGIHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/SimpleHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/_dummy_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/cPickle.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/collections_abc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/configparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/copyreg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/email_mime_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/email_mime_multipart.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/email_mime_nonmultipart.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/email_mime_text.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/html_entities.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/html_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/http_client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/http_cookiejar.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/http_cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/queue.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/reprlib.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/socketserver.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.517479 types-six-1.16.8/six-python2-stubs/moves/urllib/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/error.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/parse.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/response.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib/robotparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib_error.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib_parse.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib_request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib_response.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/urllib_robotparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-07 11:27:57.000000 types-six-1.16.8/six-python2-stubs/moves/xmlrpc_client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.517479 types-six-1.16.8/six-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-07 11:32:31.000000 types-six-1.16.8/six-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.521479 types-six-1.16.8/six-stubs/moves/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/BaseHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/CGIHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/SimpleHTTPServer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/_dummy_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/cPickle.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/collections_abc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/configparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/copyreg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/email_mime_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/email_mime_multipart.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/email_mime_nonmultipart.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/email_mime_text.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/html_entities.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/html_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/http_client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/http_cookiejar.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/http_cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/queue.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/reprlib.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/socketserver.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_commondialog.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_constants.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_dialog.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_filedialog.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_tkfiledialog.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/tkinter_ttk.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.521479 types-six-1.16.8/six-stubs/moves/urllib/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/error.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/parse.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/response.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib/robotparser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib_error.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib_parse.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib_request.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib_response.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-07 11:27:57.000000 types-six-1.16.8/six-stubs/moves/urllib_robotparser.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:32:32.521479 types-six-1.16.8/types_six.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-07 11:32:32.000000 types-six-1.16.8/types_six.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-01-07 11:32:32.000000 types-six-1.16.8/types_six.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 11:32:32.000000 types-six-1.16.8/types_six.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-07 11:32:32.000000 types-six-1.16.8/types_six.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.075377 types-six-1.16.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-01-08 15:20:30.000000 types-six-1.16.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:20:30.000000 types-six-1.16.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-08 15:20:31.075377 types-six-1.16.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-08 15:20:31.075377 types-six-1.16.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-01-08 15:20:30.000000 types-six-1.16.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.063377 types-six-1.16.9/six-python2-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-08 15:20:30.000000 types-six-1.16.9/six-python2-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.067377 types-six-1.16.9/six-python2-stubs/moves/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/BaseHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/CGIHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/SimpleHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/_dummy_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/cPickle.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/collections_abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/configparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/copyreg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/email_mime_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/email_mime_multipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/email_mime_nonmultipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/email_mime_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/html_entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/html_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/http_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/http_cookiejar.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/http_cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/reprlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/socketserver.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.067377 types-six-1.16.9/six-python2-stubs/moves/urllib/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib/robotparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib_parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/urllib_robotparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-08 15:18:10.000000 types-six-1.16.9/six-python2-stubs/moves/xmlrpc_client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.067377 types-six-1.16.9/six-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-08 15:20:30.000000 types-six-1.16.9/six-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.075377 types-six-1.16.9/six-stubs/moves/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/BaseHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/CGIHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/SimpleHTTPServer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/_dummy_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/cPickle.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/collections_abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/configparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/copyreg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/email_mime_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/email_mime_multipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/email_mime_nonmultipart.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/email_mime_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/html_entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/html_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/http_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/http_cookiejar.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/http_cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/reprlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/socketserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_commondialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_dialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_filedialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_tkfiledialog.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/tkinter_ttk.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.075377 types-six-1.16.9/six-stubs/moves/urllib/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib/robotparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib_parse.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-08 15:18:10.000000 types-six-1.16.9/six-stubs/moves/urllib_robotparser.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:31.075377 types-six-1.16.9/types_six.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-08 15:20:30.000000 types-six-1.16.9/types_six.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-01-08 15:20:30.000000 types-six-1.16.9/types_six.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-08 15:20:30.000000 types-six-1.16.9/types_six.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-08 15:20:30.000000 types-six-1.16.9/types_six.egg-info/top_level.txt
```

### Comparing `types-six-1.16.8/PKG-INFO` & `types-six-1.16.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-six
-Version: 1.16.8
+Version: 1.16.9
 Summary: Typing stubs for six
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `six` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `six`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/six. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
```

### Comparing `types-six-1.16.8/setup.py` & `types-six-1.16.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `six` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `six`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/six. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.16.8",
+      version="1.16.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=[],
       packages=['six-stubs', 'six-python2-stubs'],
       package_data={'six-stubs': ['__init__.pyi', 'moves/BaseHTTPServer.pyi', 'moves/CGIHTTPServer.pyi', 'moves/SimpleHTTPServer.pyi', 'moves/__init__.pyi', 'moves/_dummy_thread.pyi', 'moves/_thread.pyi', 'moves/builtins.pyi', 'moves/cPickle.pyi', 'moves/collections_abc.pyi', 'moves/configparser.pyi', 'moves/copyreg.pyi', 'moves/email_mime_base.pyi', 'moves/email_mime_multipart.pyi', 'moves/email_mime_nonmultipart.pyi', 'moves/email_mime_text.pyi', 'moves/html_entities.pyi', 'moves/html_parser.pyi', 'moves/http_client.pyi', 'moves/http_cookiejar.pyi', 'moves/http_cookies.pyi', 'moves/queue.pyi', 'moves/reprlib.pyi', 'moves/socketserver.pyi', 'moves/tkinter.pyi', 'moves/tkinter_commondialog.pyi', 'moves/tkinter_constants.pyi', 'moves/tkinter_dialog.pyi', 'moves/tkinter_filedialog.pyi', 'moves/tkinter_tkfiledialog.pyi', 'moves/tkinter_ttk.pyi', 'moves/urllib/__init__.pyi', 'moves/urllib/error.pyi', 'moves/urllib/parse.pyi', 'moves/urllib/request.pyi', 'moves/urllib/response.pyi', 'moves/urllib/robotparser.pyi', 'moves/urllib_error.pyi', 'moves/urllib_parse.pyi', 'moves/urllib_request.pyi', 'moves/urllib_response.pyi', 'moves/urllib_robotparser.pyi', 'METADATA.toml'], 'six-python2-stubs': ['__init__.pyi', 'moves/BaseHTTPServer.pyi', 'moves/CGIHTTPServer.pyi', 'moves/SimpleHTTPServer.pyi', 'moves/__init__.pyi', 'moves/_dummy_thread.pyi', 'moves/_thread.pyi', 'moves/cPickle.pyi', 'moves/collections_abc.pyi', 'moves/configparser.pyi', 'moves/copyreg.pyi', 'moves/email_mime_base.pyi', 'moves/email_mime_multipart.pyi', 'moves/email_mime_nonmultipart.pyi', 'moves/email_mime_text.pyi', 'moves/html_entities.pyi', 'moves/html_parser.pyi', 'moves/http_client.pyi', 'moves/http_cookiejar.pyi', 'moves/http_cookies.pyi', 'moves/queue.pyi', 'moves/reprlib.pyi', 'moves/socketserver.pyi', 'moves/urllib/__init__.pyi', 'moves/urllib/error.pyi', 'moves/urllib/parse.pyi', 'moves/urllib/request.pyi', 'moves/urllib/response.pyi', 'moves/urllib/robotparser.pyi', 'moves/urllib_error.pyi', 'moves/urllib_parse.pyi', 'moves/urllib_request.pyi', 'moves/urllib_response.pyi', 'moves/urllib_robotparser.pyi', 'moves/xmlrpc_client.pyi', 'METADATA.toml']},
```

### Comparing `types-six-1.16.8/six-python2-stubs/__init__.pyi` & `types-six-1.16.9/six-python2-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-python2-stubs/moves/__init__.pyi` & `types-six-1.16.9/six-python2-stubs/moves/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-python2-stubs/moves/urllib/parse.pyi` & `types-six-1.16.9/six-python2-stubs/moves/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-python2-stubs/moves/urllib/request.pyi` & `types-six-1.16.9/six-python2-stubs/moves/urllib/request.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-stubs/__init__.pyi` & `types-six-1.16.9/six-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import types
 import unittest
 from builtins import next as next
 from collections.abc import Callable, ItemsView, Iterable, Iterator as _Iterator, KeysView, Mapping, ValuesView
 from functools import wraps as wraps
 from importlib.util import spec_from_loader as spec_from_loader
 from io import BytesIO as BytesIO, StringIO as StringIO
-from typing import Any, AnyStr, NoReturn, Pattern, Type, TypeVar, overload
+from typing import Any, AnyStr, NoReturn, Pattern, TypeVar, overload
 from typing_extensions import Literal
 
 from . import moves as moves
 
 _T = TypeVar("_T")
 _K = TypeVar("_K")
 _V = TypeVar("_V")
@@ -20,17 +20,17 @@
 __author__: str
 __version__: str
 
 PY2: Literal[False]
 PY3: Literal[True]
 PY34: Literal[True]
 
-string_types: tuple[Type[str]]
-integer_types: tuple[Type[int]]
-class_types: tuple[Type[Type[Any]]]
+string_types: tuple[type[str]]
+integer_types: tuple[type[int]]
+class_types: tuple[type[type[Any]]]
 text_type = str
 binary_type = bytes
 
 MAXSIZE: int
 
 callable = builtins.callable
 
@@ -73,16 +73,16 @@
 def assertRaisesRegex(self: unittest.TestCase, callable_obj: Callable[..., Any], *args: Any, **kwargs: Any) -> Any: ...
 def assertRegex(
     self: unittest.TestCase, text: AnyStr, expected_regex: AnyStr | Pattern[AnyStr], msg: str | None = ...
 ) -> None: ...
 
 exec_ = exec
 
-def reraise(tp: Type[BaseException] | None, value: BaseException | None, tb: types.TracebackType | None = ...) -> NoReturn: ...
-def raise_from(value: BaseException | Type[BaseException], from_value: BaseException | None) -> NoReturn: ...
+def reraise(tp: type[BaseException] | None, value: BaseException | None, tb: types.TracebackType | None = ...) -> NoReturn: ...
+def raise_from(value: BaseException | type[BaseException], from_value: BaseException | None) -> NoReturn: ...
 
 print_ = print
 
 def with_metaclass(meta: type, *bases: type) -> type: ...
 def add_metaclass(metaclass: type) -> Callable[[_T], _T]: ...
 def ensure_binary(s: bytes | str, encoding: str = ..., errors: str = ...) -> bytes: ...
 def ensure_str(s: bytes | str, encoding: str = ..., errors: str = ...) -> str: ...
```

### Comparing `types-six-1.16.8/six-stubs/moves/__init__.pyi` & `types-six-1.16.9/six-stubs/moves/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-stubs/moves/urllib/parse.pyi` & `types-six-1.16.9/six-stubs/moves/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/six-stubs/moves/urllib/request.pyi` & `types-six-1.16.9/six-stubs/moves/urllib/request.pyi`

 * *Files identical despite different names*

### Comparing `types-six-1.16.8/types_six.egg-info/PKG-INFO` & `types-six-1.16.9/types_six.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-six
-Version: 1.16.8
+Version: 1.16.9
 Summary: Typing stubs for six
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `six` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `six`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/six. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
```

### Comparing `types-six-1.16.8/types_six.egg-info/SOURCES.txt` & `types-six-1.16.9/types_six.egg-info/SOURCES.txt`

 * *Files identical despite different names*

