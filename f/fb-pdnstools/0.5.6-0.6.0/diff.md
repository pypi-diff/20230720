# Comparing `tmp/fb_pdnstools-0.5.6.tar.gz` & `tmp/fb_pdnstools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_pdnstools-0.5.6.tar", last modified: Fri Dec 30 14:55:48 2022, max compression
+gzip compressed data, was "fb_pdnstools-0.6.0.tar", last modified: Thu Jul 20 12:39:56 2023, max compression
```

## Comparing `fb_pdnstools-0.5.6.tar` & `fb_pdnstools-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.011466 fb_pdnstools-0.5.6/
--rw-r--r--   0 root         (0) root         (0)     7652 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       89 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1130 2022-12-30 14:55:48.011466 fb_pdnstools-0.5.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       53 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.003466 fb_pdnstools-0.5.6/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1576 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/bin/pdns-bulk-remove
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.003466 fb_pdnstools-0.5.6/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.007466 fb_pdnstools-0.5.6/lib/fb_pdnstools/
--rw-r--r--   0 root         (0) root         (0)    17398 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24077 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/bulk_rm_app.py
--rw-r--r--   0 root         (0) root         (0)     4488 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/bulk_rm_cfg.py
--rw-r--r--   0 root         (0) root         (0)     3852 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/errors.py
--rw-r--r--   0 root         (0) root         (0)      438 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    42405 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/record.py
--rw-r--r--   0 root         (0) root         (0)     7813 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/server.py
--rw-r--r--   0 root         (0) root         (0)     2977 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/xlate.py
--rw-r--r--   0 root         (0) root         (0)    52857 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.007466 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1130 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      763 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-12-30 14:55:47.000000 fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1183 2022-12-30 14:55:48.011466 fb_pdnstools-0.5.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6491 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 14:55:48.011466 fb_pdnstools-0.5.6/test/
--rw-r--r--   0 root         (0) root         (0)     7126 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/general.py
--rw-r--r--   0 root         (0) root         (0)      280 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/rrset-a-with-comment.js
--rw-r--r--   0 root         (0) root         (0)      171 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/rrset-a.js
--rw-r--r--   0 root         (0) root         (0)      253 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/rrset-mx.js
--rw-r--r--   0 root         (0) root         (0)      230 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/rrset-soa.js
--rwxr-xr-x   0 root         (0) root         (0)     6938 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/test_00_fb_pdnstools.py
--rwxr-xr-x   0 root         (0) root         (0)    15794 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/test_10_record.py
--rwxr-xr-x   0 root         (0) root         (0)     7054 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/test_20_zone.py
--rwxr-xr-x   0 root         (0) root         (0)     5422 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/test_30_server.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/zone-rev.js
--rw-r--r--   0 root         (0) root         (0)     2862 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/zone.js
--rw-r--r--   0 root         (0) root         (0)      683 2022-12-30 14:54:52.000000 fb_pdnstools-0.5.6/test/zones.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.250612 fb_pdnstools-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-20 12:39:56.250612 fb_pdnstools-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.246612 fb_pdnstools-0.6.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1913 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/bin/pdns-bulk-remove
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.246612 fb_pdnstools-0.6.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.246612 fb_pdnstools-0.6.0/lib/fb_pdnstools/
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17887 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/base_handler.py
+-rw-r--r--   0 root         (0) root         (0)    24656 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/bulk_rm_app.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/bulk_rm_cfg.py
+-rw-r--r--   0 root         (0) root         (0)     3209 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/common.py
+-rw-r--r--   0 root         (0) root         (0)     5075 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/errors.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    48900 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/record.py
+-rw-r--r--   0 root         (0) root         (0)     8240 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/server.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/xlate.py
+-rw-r--r--   0 root         (0) root         (0)    56055 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.246612 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 12:39:56.000000 fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-20 12:39:56.250612 fb_pdnstools-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6915 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:39:56.250612 fb_pdnstools-0.6.0/test/
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/general.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/rrset-a-with-comment.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/rrset-a.js
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/rrset-mx.js
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/rrset-soa.js
+-rwxr-xr-x   0 root         (0) root         (0)     6569 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_00_fb_pdnstools.py
+-rwxr-xr-x   0 root         (0) root         (0)     5540 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     3927 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_10_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    16575 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_20_record.py
+-rwxr-xr-x   0 root         (0) root         (0)     7496 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_30_zone.py
+-rwxr-xr-x   0 root         (0) root         (0)     5905 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/test_40_server.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/zone-rev.js
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/zone.js
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-20 12:38:58.000000 fb_pdnstools-0.6.0/test/zones.js
```

### Comparing `fb_pdnstools-0.5.6/LICENSE` & `fb_pdnstools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_pdnstools-0.5.6/PKG-INFO` & `fb_pdnstools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_pdnstools
-Version: 0.5.6
+Version: 0.6.0
 Summary: Modules for handling the PowerDNS API
 Home-page: https://github.com/fbrehm/fb-pdnstools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fb_pdnstools-0.5.6/bin/pdns-bulk-remove` & `fb_pdnstools-0.6.0/bin/pdns-bulk-remove`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+@summary: Removes the given addresses completety from PowerDNS.
+
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
+"""
 
 from __future__ import print_function
 
+import locale
+import os
 import sys
 
-if sys.version_info[0] != 3:
-    print("This script is intended to use with Python3.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+MIN_PYTHON_MAJOR = 3
+MIN_PYTHON_MINOR = 6
+
+if sys.version_info[0] != MIN_PYTHON_MAJOR:
+    print(
+        'This script is intended to use with Python{}.'.format(MIN_PYTHON_MAJOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-if sys.version_info[1] < 6:
-    print("A minimal Python version of 3.6 is necessary to execute this script.", file=sys.stderr)
-    print("You are using Python: {0}.{1}.{2}-{3}-{4}.\n".format(
+if sys.version_info[1] < MIN_PYTHON_MAJOR and sys.version_info[1] < MIN_PYTHON_MINOR:
+    print(
+        'A minimal Python version of {}.{} is necessary to execute this script.'.format(
+            MIN_PYTHON_MAJOR, MIN_PYTHON_MINOR), file=sys.stderr)
+    print('You are using Python: {0}.{1}.{2}-{3}-{4}.\n'.format(
         *sys.version_info), file=sys.stderr)
     sys.exit(1)
 
-import os
-import logging
-import locale
-
 # own modules:
 cur_dir = os.getcwd()
 base_dir = cur_dir
 
 if sys.argv[0] != '' and sys.argv[0] != '-c':
     bin_dir = os.path.dirname(os.path.realpath(sys.argv[0]))
 else:
@@ -33,27 +44,25 @@
 lib_dir = os.path.join(base_dir, 'lib')
 module_dir = os.path.join(lib_dir, 'fb_pdnstools')
 if os.path.exists(module_dir):
     sys.path.insert(0, lib_dir)
 
 from fb_pdnstools.bulk_rm_app import PdnsBulkRmApp
 
-log = logging.getLogger(__name__)
-
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
-__copyright__ = '(C) 2021 by Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 appname = os.path.basename(sys.argv[0])
 
 locale.setlocale(locale.LC_ALL, '')
 
 app = PdnsBulkRmApp(appname=appname, base_dir=base_dir)
 app.initialized = True
 
 if app.verbose > 2:
-    print("{c}-Object:\n{a}".format(c=app.__class__.__name__, a=app))
+    print('{c}-Object:\n{a}'.format(c=app.__class__.__name__, a=app))
 
 app()
 
 sys.exit(0)
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/__init__.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/base_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a base PowerDNS handler object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2022 Frank Brehm, Berlin
-@summary: The module for a base PowerDNS handler object.
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import os
+import copy
+import ipaddress
+import json
 import logging
+import os
 import re
-import json
-import copy
 import socket
-import ipaddress
-
 from abc import ABCMeta
-
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 # Third party modules
+from fb_tools.common import RE_DOT_AT_END
+from fb_tools.common import pp
+from fb_tools.common import reverse_pointer
+from fb_tools.common import to_bool
+from fb_tools.common import to_str
+from fb_tools.handling_obj import HandlingObject
+
 import requests
-import urllib3
 
 import six
 from six import add_metaclass
 
-# Own modules
-from fb_tools.common import pp, to_bool, RE_DOT_AT_END, reverse_pointer, to_str
-
-from fb_tools.handling_obj import HandlingObject
+import urllib3
 
+# Own modules
+from . import DEFAULT_API_PREFIX
+from . import DEFAULT_PORT
+from . import DEFAULT_TIMEOUT
+from . import DEFAULT_USE_HTTPS
+from . import LIBRARY_NAME
+from . import MAX_PORT_NUMBER
+from . import VALID_RRSET_TYPES
+from .errors import PDNSApiError
+from .errors import PDNSApiNotAuthorizedError
+from .errors import PDNSApiNotFoundError
+from .errors import PDNSApiRateLimitExceededError
+from .errors import PDNSApiValidationError
+from .errors import PowerDNSHandlerError
 from .xlate import XLATOR
 
-from .errors import PowerDNSHandlerError, PDNSApiError, PDNSApiNotAuthorizedError
-from .errors import PDNSApiNotFoundError, PDNSApiValidationError, PDNSApiRateLimitExceededError
 
-__version__ = '0.5.6'
+__version__ = '0.6.1'
 LOG = logging.getLogger(__name__)
-LIBRARY_NAME = "fb-pdns-api-client"
 
 LOGLEVEL_REQUESTS_SET = False
 
-DEFAULT_PORT = 8081
-DEFAULT_TIMEOUT = 20
-DEFAULT_API_PREFIX = '/api/v1'
-DEFAULT_USE_HTTPS = False
-
-FQDN_REGEX = re.compile(r'^((?!-)[-A-Z\d]{1,62}(?<!-)\.)+[A-Z]{1,62}\.?$', re.IGNORECASE)
-
-VALID_RRSET_TYPES = [
-    'SOA', 'A', 'AAAA', 'AFSDB', 'APL', 'CAA', 'CDNSKEY', 'CDS', 'CERT', 'CNAME', 'DHCID',
-    'DLV', 'DNAME', 'DNSKEY', 'DS', 'HIP', 'HINFO', 'IPSECKEY', 'ISDN', 'KEY', 'KX', 'LOC',
-    'MB', 'MINFO', 'MX', 'NAPTR', 'NS', 'NSAP', 'NSEC', 'NSEC3', 'NSEC3PARAM', 'OPT', 'PTR',
-    'RP', 'RRSIG', 'SIG', 'SPF', 'SRV', 'SSHFP', 'TA', 'TKEY', 'TLSA', 'TSIG', 'TXT', 'URI',
-    'WKS', 'X25'
-]
-
 _ = XLATOR.gettext
 
 
 # =============================================================================
 @add_metaclass(ABCMeta)
 class BasePowerDNSHandler(HandlingObject):
     """
     Base class for a PowerDNS handler object.
-    May not be instantiated.
+
+    Must not be instantiated directly.
     """
 
     show_simulate_option = True
 
     default_port = DEFAULT_PORT
     default_timeout = DEFAULT_TIMEOUT
-    default_api_servername = "localhost"
+    default_api_servername = 'localhost'
 
     loglevel_requests_set = False
 
     re_request_id = re.compile(r'/requests/([-a-f0-9]+)/', re.IGNORECASE)
 
     # -------------------------------------------------------------------------
     def __init__(
-        self, appname=None, verbose=0, version=__version__, base_dir=None,
-            master_server=None, port=DEFAULT_PORT, key=None, use_https=False, timeout=None,
+        self, appname=None, verbose=0, version=__version__, base_dir=None, master_server=None,
+            port=DEFAULT_PORT, key=None, use_https=DEFAULT_USE_HTTPS, timeout=None,
             path_prefix=DEFAULT_API_PREFIX, simulate=None, force=None, terminal_has_colors=False,
             initialized=False,):
-
+        """Initialize a BasePowerDNSHandler object."""
         self._master_server = master_server
         self._port = self.default_port
         self._key = key
         self._use_https = False
         self._path_prefix = path_prefix
         self._timeout = self.default_timeout
         self._user_agent = '{}/{}'.format(LIBRARY_NAME, __version__)
@@ -110,18 +109,18 @@
         self.use_https = use_https
         self.port = port
         self.timeout = timeout
 
         global LOGLEVEL_REQUESTS_SET
 
         if not LOGLEVEL_REQUESTS_SET:
-            msg = _("Setting Loglevel of the {m} module to {ll}.").format(
+            msg = _('Setting loglevel of the {m} module to {ll}.').format(
                 m='requests', ll='WARNING')
             LOG.debug(msg)
-            logging.getLogger("requests").setLevel(logging.WARNING)
+            logging.getLogger('requests').setLevel(logging.WARNING)
             LOGLEVEL_REQUESTS_SET = True
 
         self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def master_server(self):
@@ -149,19 +148,18 @@
     @port.setter
     def port(self, value):
         if value is None:
             self._port = self.default_port
             return
         val = int(value)
         err_msg = _(
-            "Invalid port number {!r} for the PowerDNS API, "
-            "must be 0 < PORT < 65536.")
-        if val <= 0 or val > 65536:
-            msg = err_msg.format(value)
-            raise ValueError(msg)
+            'Invalid port number {port!r} for the PowerDNS API, must be greater than zero '
+            'and less than {max}.').format(port=value, max=(MAX_PORT_NUMBER + 1))
+        if val <= 0 or val >= MAX_PORT_NUMBER:
+            raise ValueError(err_msg)
         self._port = val
 
     # -----------------------------------------------------------
     @property
     def key(self):
         """The key used to authenticate against the PowerDNS API."""
         return self._key
@@ -177,15 +175,15 @@
             self._key = None
         else:
             self._key = val
 
     # -----------------------------------------------------------
     @property
     def use_https(self):
-        """Should be HTTPS used to communicate with the API?"""
+        """Return, whether to use HTTPS to communicate with the API."""
         if self.mocked:
             return False
         return self._use_https
 
     @use_https.setter
     def use_https(self, value):
         self._use_https = to_bool(value)
@@ -213,15 +211,15 @@
             return
 
         val = str(value).strip()
         if val == '':
             self._path_prefix = None
         else:
             if not os.path.isabs(val):
-                msg = _("The path prefix {!r} must be an absolute path.").format(value)
+                msg = _('The path prefix {!r} must be an absolute path.').format(value)
                 raise ValueError(msg)
             self._path_prefix = val
 
     # -----------------------------------------------------------
     @property
     def timeout(self):
         """The timeout in seconds for requesting the PowerDNS API."""
@@ -230,57 +228,56 @@
     @timeout.setter
     def timeout(self, value):
         if value is None:
             self._timeout = self.default_timeout
             return
         val = int(value)
         err_msg = _(
-            "Invalid timeout {!r} for requesting the PowerDNS API, "
-            "must be 0 < SECONDS < 3600.")
+            'Invalid timeout {!r} for requesting the PowerDNS API, must be greater than zero and '
+            'less or equal to  3600.')
         if val <= 0 or val > 3600:
             msg = err_msg.format(value)
             raise ValueError(msg)
         self._timeout = val
 
     # -----------------------------------------------------------
     @property
     def user_agent(self):
-        "The name of the user agent used in API calls."
+        """The name of the user agent used in API calls."""
         return self._user_agent
 
     @user_agent.setter
     def user_agent(self, value):
         if value is None or str(value).strip() == '':
-            raise PowerDNSHandlerError(_("Invalid user agent {!r} given.").format(value))
+            raise PowerDNSHandlerError(_('Invalid user agent {!r} given.').format(value))
         self._user_agent = str(value).strip()
 
     # -----------------------------------------------------------
     @property
     def api_servername(self):
-        "The (virtual) name of the PowerDNS server used in API calls."
+        """The (virtual) name of the PowerDNS server used in API calls."""
         return self._api_servername
 
     @api_servername.setter
     def api_servername(self, value):
         if value is None or str(value).strip() == '':
-            raise PowerDNSHandlerError(_("Invalid API server name {!r} given.").format(value))
+            raise PowerDNSHandlerError(_('Invalid API server name {!r} given.').format(value))
         self._api_servername = str(value).strip()
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(BasePowerDNSHandler, self).as_dict(short=short)
         res['default_port'] = self.default_port
         res['default_timeout'] = self.default_timeout
         res['default_api_servername'] = self.default_api_servername
         res['master_server'] = self.master_server
         res['port'] = self.port
         res['mocked'] = self.mocked
@@ -314,15 +311,15 @@
                 loc)
             raise PowerDNSHandlerError(msg)
 
     # -------------------------------------------------------------------------
     def _build_url(self, path, no_prefix=False):
 
         if not os.path.isabs(path):
-            msg = _("The path {!r} must be an absolute path.").format(path)
+            msg = _('The path {!r} must be an absolute path.').format(path)
             raise ValueError(msg)
 
         url = 'http://{}'.format(self.master_server)
         if self.mocked:
             url = 'mock://{}'.format(self.master_server)
         elif self.use_https:
             url = 'https://{}'.format(self.master_server)
@@ -334,85 +331,84 @@
 
         if self.path_prefix and not no_prefix:
             url += self.path_prefix
 
         url += path
 
         if self.verbose > 1:
-            LOG.debug(_("Used URL: {!r}").format(url))
+            LOG.debug(_('Used URL: {!r}').format(url))
         return url
 
     # -------------------------------------------------------------------------
     def perform_request(
         self, path, no_prefix=False, method='GET',
             data=None, headers=None, may_simulate=False):
-        """Performing the underlying API request."""
-
+        """Perform the underlying API request."""
         if headers is None:
-            headers = dict()
+            headers = {}
         if self.key:
             headers['X-API-Key'] = self.key
 
         url = self._build_url(path, no_prefix=no_prefix)
         if self.verbose > 1:
-            LOG.debug(_("Request method: {!r}").format(method))
+            LOG.debug(_('Request method: {!r}').format(method))
         if data and self.verbose > 1:
-            data_out = "{!r}".format(data)
+            data_out = '{!r}'.format(data)
             try:
                 data_out = json.loads(data)
             except ValueError:
                 pass
             else:
                 data_out = pp(data_out)
-            LOG.debug("Data:\n{}".format(data_out))
+            LOG.debug('Data:\n{}'.format(data_out))
             if self.verbose > 2:
-                LOG.debug("RAW data:\n{}".format(data))
+                LOG.debug('RAW data:\n{}'.format(data))
 
         headers.update({'User-Agent': self.user_agent})
         headers.update({'Content-Type': 'application/json'})
         if self.verbose > 1:
             head_out = copy.copy(headers)
             if 'X-API-Key' in head_out and self.verbose <= 4:
                 head_out['X-API-Key'] = '******'
-            LOG.debug("Headers:\n{}".format(pp(head_out)))
+            LOG.debug('Headers:\n{}'.format(pp(head_out)))
 
         if may_simulate and self.simulate:
-            LOG.debug(_("Simulation mode, Request will not be sent."))
+            LOG.debug(_('Simulation mode, Request will not be sent.'))
             return ''
 
         try:
 
             session = requests.Session()
             if self.mocked:
                 self.start_mocking(session)
             response = session.request(
                 method, url, data=data, headers=headers, timeout=self.timeout)
 
         except (
                 socket.timeout, urllib3.exceptions.ConnectTimeoutError,
                 urllib3.exceptions.MaxRetryError,
                 requests.exceptions.ConnectTimeout) as e:
-            msg = _("Got a {c} on connecting to {h!r}: {e}.").format(
+            msg = _('Got a {c} on connecting to {h!r}: {e}.').format(
                 c=e.__class__.__name__, h=self.master_server, e=e)
             raise PowerDNSHandlerError(msg)
 
         try:
             self._eval_response(url, response)
 
         except ValueError:
             raise PDNSApiError(_('Failed to parse the response'), response.text)
 
         if self.verbose > 3:
-            LOG.debug("RAW response: {!r}.".format(response.text))
+            LOG.debug('RAW response: {!r}.'.format(response.text))
         if not response.text:
             return ''
 
         json_response = response.json()
         if self.verbose > 3:
-            LOG.debug("JSON response:\n{}".format(pp(json_response)))
+            LOG.debug('JSON response:\n{}'.format(pp(json_response)))
 
         if 'location' in response.headers:
             json_response['requestId'] = self._request_id(response.headers)
 
         return json_response
 
     # -------------------------------------------------------------------------
@@ -420,120 +416,126 @@
 
         if response.ok:
             return
 
         err = response.json()
         code = response.status_code
         msg = err['error']
-        LOG.debug(_("Got an error response code {code}: {msg}").format(code=code, msg=msg))
+        LOG.debug(_('Got an error response code {code}: {msg}').format(code=code, msg=msg))
         if response.status_code == 401:
             raise PDNSApiNotAuthorizedError(code, msg, url)
         if response.status_code == 404:
             raise PDNSApiNotFoundError(code, msg, url)
         if response.status_code == 422:
             raise PDNSApiValidationError(code, msg, url)
         if response.status_code == 429:
             raise PDNSApiRateLimitExceededError(code, msg, url)
         else:
             raise PDNSApiError(code, msg, url)
 
     # -------------------------------------------------------------------------
     def canon_name(self, name):
-
+        """Canonize the DNS name, that means ensure a dot at the end of the name."""
         ret = RE_DOT_AT_END.sub('.', name, 1)
         return ret
 
     # -------------------------------------------------------------------------
     def name2fqdn(self, name, is_fqdn=False):
+        """
+        Transform the given name into a canonized FQDN.
 
+        If an IP address as name is given (and the parameter 'is_fqdn' is False), then
+        this name will be transformed into a reverse pointer address
+        (e.g. '4.3.2.1..in-addr.arpa.').
+        """
         fqdn = name
 
         if not is_fqdn:
             try:
                 address = ipaddress.ip_address(name)
                 fqdn = reverse_pointer(address)
                 is_fqdn = False
             except ValueError:
                 if self.verbose > 3:
-                    LOG.debug(_("Name {!r} is not a valid IP address.").format(name))
+                    LOG.debug(_('Name {!r} is not a valid IP address.').format(name))
                 is_fqdn = True
                 fqdn = name
 
         if ':' in fqdn:
-            LOG.error(_("Invalid FQDN {!r}.").format(fqdn))
+            LOG.error(_('Invalid FQDN {!r}.').format(fqdn))
             return None
 
         return self.canon_name(fqdn)
 
     # -------------------------------------------------------------------------
     def decanon_name(self, name):
-
+        """Decanonize the FQDN - removing possible dots at the end of the name."""
         ret = RE_DOT_AT_END.sub('', name)
         return ret
 
     # -------------------------------------------------------------------------
     def verify_rrset_type(self, rtype, raise_on_error=True):
-
+        """Verify, that the given name is a valid RRset type name."""
         if not isinstance(rtype, six.string_types):
-            msg = _("A rrset type must be a string type, but is {!r} instead.").format(rtype)
+            msg = _('A rrset type must be a string type, but is {!r} instead.').format(rtype)
             if raise_on_error:
                 raise TypeError(msg)
             LOG.error(msg)
             return None
 
         type_used = to_str(rtype).strip().upper()
         if not type_used:
-            msg = _("Invalid, empty rrset type {!r} given.").format(rtype)
+            msg = _('Invalid, empty rrset type {!r} given.').format(rtype)
             if raise_on_error:
                 raise ValueError(msg)
             LOG.error(msg)
             return None
 
         if type_used not in VALID_RRSET_TYPES:
-            msg = _("Invalid rrset type {!r} given.").format(rtype)
+            msg = _('Invalid rrset type {!r} given.').format(rtype)
             if raise_on_error:
                 raise ValueError(msg)
             LOG.error(msg)
             return None
 
         return type_used
 
     # -------------------------------------------------------------------------
     def start_mocking(self, session):
-
+        """Start mocking mode of this class for unit testing."""
         if not self.mocked:
             return
 
-        LOG.debug(_("Preparing mocking ..."))
+        LOG.debug(_('Preparing mocking ...'))
 
         import requests_mock
 
         adapter = requests_mock.Adapter()
         session.mount('mock', adapter)
 
         for path in self.mocking_paths:
 
             if not isinstance(path, MutableMapping):
                 msg = _(
-                    "Mocking path {p!r} is not a dictionary object, but a "
-                    "{c} object instead.").format(p=path, c=path.__class__.__name__)
+                    'Mocking path {p!r} is not a dictionary object, but a '
+                    '{c} object instead.').format(p=path, c=path.__class__.__name__)
                 raise PowerDNSHandlerError(msg)
 
             for key in ('method', 'url'):
                 if key not in path:
-                    msg = _("Mocking path has no {!r} key defined:").format(key)
+                    msg = _('Mocking path has no {!r} key defined:').format(key)
                     msg += '\n' + pp(path)
                     raise PowerDNSHandlerError(msg)
 
             if self.verbose > 2:
-                LOG.debug(_("Adding mocking path:") + '\n' + pp(path))
+                LOG.debug(_('Adding mocking path:') + '\n' + pp(path))
             adapter.register_uri(**path)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/bulk_rm_app.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/bulk_rm_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,77 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for the 'pdns-bulk-remove' application object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 by Frank Brehm, Berlin
-@summary: The module for the 'pdns-bulk-remove' application object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
+import copy
+import ipaddress
 import logging
-import pathlib
-import sys
 import os
+import pathlib
 import re
-import ipaddress
-import copy
-
+import sys
 from functools import cmp_to_key
 
 # Third party modules
-
-# Own modules
-from fb_tools.errors import FbAppError
-
-from fb_tools.common import pp, compare_fqdn, to_bool, reverse_pointer, to_str
-
 from fb_tools.app import BaseApplication
-
+from fb_tools.common import compare_fqdn
+from fb_tools.common import pp
+from fb_tools.common import reverse_pointer
+from fb_tools.common import to_bool
+from fb_tools.common import to_str
 from fb_tools.config import CfgFileOptionAction
+from fb_tools.errors import FbAppError
 
+# Own modules
+from . import DEFAULT_API_PREFIX
+from . import DEFAULT_PORT
 from . import __version__ as GLOBAL_VERSION
-
-from .xlate import XLATOR
-
 from .bulk_rm_cfg import PdnsBulkRmCfg
-
-from . import DEFAULT_PORT, DEFAULT_API_PREFIX
-
 from .server import PowerDNSServer
+from .xlate import XLATOR
 
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class PdnsBulkRmError(FbAppError):
-    """ Base exception class for all exceptions in this application."""
+    """Base exception class for all exceptions in this application."""
+
     pass
 
 
 # =============================================================================
 class PdnsBulkRmApp(BaseApplication):
-    """
-    Class for the application object.
-    """
+    """Class for the application object of the pdns-bulk-remove application."""
 
     show_simulate_option = True
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=GLOBAL_VERSION, base_dir=None,
             initialized=False, usage=None, description=None,
             argparse_epilog=None, argparse_prefix_chars='-', env_prefix=None):
-
+        """Initialize the PdnsBulkRmApp object."""
         desc = _(
-            "Removes the given addresses (A-, AAAA- or CNAME-Records) completety from "
-            "PowerDNS. If there are multiple entries to a DNS-Name, all appropriate "
-            "records are removed. Additionally all appropriate reverse entries (PTR-records) "
-            "were also removed, if they are pointing back to the given A- or AAAA-record.")
+            'Removes the given addresses (A-, AAAA- or CNAME-Records) completety from '
+            'PowerDNS. If there are multiple entries to a DNS-Name, all appropriate '
+            'records are removed. Additionally all appropriate reverse entries (PTR-records) '
+            'were also removed, if they are pointing back to the given A- or AAAA-record.')
 
         self._cfg_file = None
         self.config = None
         self.pdns = None
         self._rm_reverse = True
 
         self.address_file = None
@@ -90,59 +86,56 @@
         )
 
         self.initialized = True
 
     # -------------------------------------------------------------------------
     @property
     def cfg_file(self):
-        """Configuration file."""
+        """Return the onfiguration file."""
         return self._cfg_file
 
     # -------------------------------------------------------------------------
     @property
     def rm_reverse(self):
-        """Flag indicating, that the reverse DNS entries (PTR records)
-            should not be removed."""
+        """Return, whether the reverse DNS entries (PTR records) should not be removed."""
         return self._rm_reverse
 
     @rm_reverse.setter
     def rm_reverse(self, value):
         self._rm_reverse = to_bool(value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(PdnsBulkRmApp, self).as_dict(short=short)
         res['cfg_file'] = self.cfg_file
         res['rm_reverse'] = self.rm_reverse
 
         return res
 
     # -------------------------------------------------------------------------
     def post_init(self):
         """
-        Method to execute before calling run(). Here could be done some
-        finishing actions after reading in commandline parameters,
-        configuration a.s.o.
+        Execute this method before calling run().
+
+        Here could be done some finishing actions after reading in commandline
+        parameters, configuration a.s.o.
 
         This method could be overwritten by descendant classes, these
         methhods should allways include a call to post_init() of the
         parent class.
-
         """
-
         self.initialized = False
 
         self.init_logging()
 
         self.perform_arg_parser()
 
         self.config = PdnsBulkRmCfg(
@@ -151,23 +144,23 @@
 
         self.config.read()
         if self.config.verbose > self.verbose:
             self.verbose = self.config.verbose
         self.config.initialized = True
 
         if self.verbose > 3:
-            LOG.debug("Read configuration:\n{}".format(pp(self.config.as_dict())))
+            LOG.debug('Read configuration:\n{}'.format(pp(self.config.as_dict())))
 
         self.perform_arg_parser_pdns()
 
         if self.address_file:
             self.read_address_file()
 
         if not self.addresses:
-            LOG.error(_("No addresses to remove given."))
+            LOG.error(_('No addresses to remove given.'))
             self.exit(1)
 
         self.pdns = PowerDNSServer(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             master_server=self.config.pdns_master, port=self.config.pdns_api_port,
             key=self.config.pdns_api_key, use_https=self.config.pdns_api_https,
             path_prefix=self.config.pdns_api_prefix,
@@ -175,118 +168,111 @@
         )
 
         self.pdns.initialized = True
         self.initialized = True
 
     # -------------------------------------------------------------------------
     def init_arg_parser(self):
-        """
-        Public available method to initiate the argument parser.
-        """
-
+        """Public available method to initiate the argument parser."""
         super(PdnsBulkRmApp, self).init_arg_parser()
 
         default_cfg_file = self.base_dir.joinpath('etc').joinpath(self.appname + '.ini')
 
         self.arg_parser.add_argument(
             '-c', '--config', '--config-file', dest='cfg_file', metavar=_('FILE'),
             action=CfgFileOptionAction,
-            help=_("Configuration file (default: {!r})").format(default_cfg_file)
+            help=_('Configuration file (default: {!r})').format(default_cfg_file)
         )
 
         pdns_group = self.arg_parser.add_argument_group(_('PowerDNS options'))
 
         pdns_group.add_argument(
             '-H', '--host', dest='host', metavar=_('HOST'),
             help=_(
-                "Address or hostname of the PowerDNS server providing "
-                "the API (Default: {!r}).").format(PdnsBulkRmCfg.default_pdns_master)
+                'Address or hostname of the PowerDNS server providing '
+                'the API (Default: {!r}).').format(PdnsBulkRmCfg.default_pdns_master)
         )
 
         pdns_group.add_argument(
             '-P', '--port', dest='port', type=int, metavar=_('PORT'),
-            help=_("Port on PowerDNS server for API on (Default: {}).").format(DEFAULT_PORT))
+            help=_('Port on PowerDNS server for API on (Default: {}).').format(DEFAULT_PORT))
 
         pdns_group.add_argument(
             '-K', '--key', '--api-key', metavar='KEY', dest='api_key',
-            help=_("The API key for accessing the PowerDNS API.")
+            help=_('The API key for accessing the PowerDNS API.')
         )
 
         pdns_group.add_argument(
-            '--https', action="store_true", dest='https',
-            help=_("Use HTTPS to access the PowerDNS API (Default: {}).").format(
+            '--https', action='store_true', dest='https',
+            help=_('Use HTTPS to access the PowerDNS API (Default: {}).').format(
                 PdnsBulkRmCfg.default_pdns_api_https),
         )
 
         pdns_group.add_argument(
             '--prefix', dest='api_path_prefix',
             help=_(
-                "The global prefix for all paths for accessing the PowerDNS API "
-                "(Default: {!r}).").format(DEFAULT_API_PREFIX)
+                'The global prefix for all paths for accessing the PowerDNS API '
+                '(Default: {!r}).').format(DEFAULT_API_PREFIX)
         )
 
         # Source of the addresses - file or cmdline arguments
         # source_group = self.arg_parser.add_mutually_exclusive_group()
 
         self.arg_parser.add_argument(
-            '-N', '--no-reverse', action="store_true", dest='no_reverse',
+            '-N', '--no-reverse', action='store_true', dest='no_reverse',
             help=_(
                 "Don't remove reverse DNS entries (PTR records) to the given addresses. "
-                "(Default: False - reverse entries will be removed).")
+                '(Default: False - reverse entries will be removed).')
         )
 
         self.arg_parser.add_argument(
             '-F', '--file', metavar=_('FILE'), dest='addr_file', type=pathlib.Path,
             help=_(
-                "File containing the addresses to remove. The addresses must be "
-                "whitespace separeted, lines may be commented out by prepending them "
+                'File containing the addresses to remove. The addresses must be '
+                'whitespace separeted, lines may be commented out by prepending them '
                 "with a hash sign '#'. This option is mutually exclusive with "
-                "giving the addresses as command line arguments.")
+                'giving the addresses as command line arguments.')
         )
 
         self.arg_parser.add_argument(
             'addresses', metavar=_('ADDRESS'), type=str, nargs='*',
             help=_(
-                "Addresses to remove. This option is mutually exclusive with "
-                "the {!r} option.").format('-F/--file'),
+                'Addresses to remove. This option is mutually exclusive with '
+                'the {!r} option.').format('-F/--file'),
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
-
+        """Parse the command line options."""
         if self.args.cfg_file:
             self._cfg_file = self.args.cfg_file
 
     # -------------------------------------------------------------------------
     def perform_arg_parser_pdns(self):
-        """
-        Public available method to execute some actions after parsing
-        the command line parameters.
-        """
-
+        """Execute some actions after parsing the command line parameters."""
         if self.args.addr_file and self.args.addresses:
             msg = _(
-                "The option {!r} is mutually exclusive with giving the addresses "
-                "as command line arguments.").format('-F/--file')
+                'The option {!r} is mutually exclusive with giving the addresses '
+                'as command line arguments.').format('-F/--file')
             LOG.error(msg)
             self.arg_parser.print_usage(sys.stderr)
             self.exit(1)
 
         if self.args.addr_file:
             afile = self.args.addr_file
             if not afile.exists():
-                msg = _("File {!r} does not exists.").format(str(afile))
+                msg = _('File {!r} does not exists.').format(str(afile))
                 LOG.error(msg)
                 self.exit(1)
             if not afile.is_file():
-                msg = _("File {!r} is not a regular file.").format(str(afile))
+                msg = _('File {!r} is not a regular file.').format(str(afile))
                 LOG.error(msg)
                 self.exit(1)
             if not os.access(str(afile), os.R_OK):
-                msg = _("No read access to file {!r}.").format(str(afile))
+                msg = _('No read access to file {!r}.').format(str(afile))
                 LOG.error(msg)
                 self.exit(1)
             self.address_file = afile
 
         if self.args.host:
             self.config.pdns_master = self.args.host
         if self.args.port:
@@ -305,18 +291,18 @@
             for address in self.args.addresses:
                 addr = address.strip().lower()
                 if addr != '' and addr not in self.addresses:
                     self.addresses.append(addr)
 
     # -------------------------------------------------------------------------
     def read_address_file(self):
-
+        """Read the file containing all addresses to remove."""
         content = self.read_file(self.address_file)
         if self.verbose > 2:
-            LOG.debug("Content of {f!r}:\n{c}".format(f=str(self.address_file), c=content))
+            LOG.debug(_('Content of {!r}:').format(str(self.address_file)) + '\n' + content)
 
         re_comment = re.compile(r'\s*#.*')
         re_whitespace = re.compile(r'\s+')
 
         addresses = []
         for line in content.splitlines():
             line_stripped = re_comment.sub('', line).strip()
@@ -327,29 +313,28 @@
                 if addr != '' and addr not in addresses:
                     addresses.append(addr)
 
         if addresses:
             self.addresses = addresses
 
         if not self.addresses:
-            LOG.error(_("No addresses to remove found in {!r}.").format(str(self.address_file)))
+            LOG.error(_('No addresses to remove found in {!r}.').format(str(self.address_file)))
             self.exit(1)
 
     # -------------------------------------------------------------------------
     def __del__(self):
         """Destructor."""
-
         if self.pdns:
             self.pdns = None
 
     # -------------------------------------------------------------------------
     def _run(self):
 
         print()
-        LOG.debug("Starting {a!r}, version {v!r} ...".format(
+        LOG.debug('Starting {a!r}, version {v!r} ...'.format(
             a=self.appname, v=self.version))
 
         ret = 0
         try:
             self.pdns.get_api_zones()
             ret = self.verify_addresses(copy.copy(self.addresses))
             if self.rm_reverse and not ret:
@@ -363,23 +348,23 @@
             # Aufräumen ...
             self.pdns = None
 
         self.exit_value = ret
 
     # -------------------------------------------------------------------------
     def show_simulation(self):
-
+        """Display the informotion to t screen about simulation mode."""
         if not self.simulate:
             return
-        print(self.colored(_("Simulation mode - nothing will be removed in real."), 'YELLOW'))
+        print(self.colored(_('Simulation mode - nothing will be removed in real.'), 'YELLOW'))
         print()
 
     # -------------------------------------------------------------------------
     def do_remove(self):
-
+        """Remove finally all addresses in DNS."""
         for zone_name in sorted(
                 self.records2remove.keys(), key=lambda x: cmp_to_key(compare_fqdn)(x)):
             print()
             zone = self.pdns.zones[zone_name]
             rrsets_rm = []
             for rrset in self.records2remove[zone_name]:
                 zone.add_rrset_for_remove(rrset['fqdn'], rrset['type'], rrsets_rm)
@@ -387,66 +372,66 @@
 
         print()
 
     # -------------------------------------------------------------------------
     def _canon_addresses(self, addresses):
 
         if self.verbose > 1:
-            LOG.debug("Canonizing all given addresses.")
+            LOG.debug(_('Canonizing all given addresses.'))
         all_fqdns = []
 
         for addr in addresses:
 
             fqdn = self.pdns.name2fqdn(addr)
             if not fqdn:
-                LOG.warning(_("Address {!r} could not interpreted as a FQDN.").format(addr))
+                LOG.warning(_('Address {!r} could not interpreted as a FQDN.').format(addr))
                 continue
             if fqdn not in all_fqdns:
                 all_fqdns.append(fqdn)
 
         if self.verbose > 2:
-            LOG.debug("Canonized addresses:\n{}".format(pp(all_fqdns)))
+            LOG.debug(_('Canonized addresses:') + '\n' + pp(all_fqdns))
         return all_fqdns
 
     # -------------------------------------------------------------------------
     def _get_zones_of_addresses(self, fqdns):
 
         if self.verbose > 1:
-            LOG.debug("Retrieve zones for canonized addresses.")
+            LOG.debug(_('Retrieve zones for canonized addresses.'))
         zones_of_records = {}
 
         for fqdn in fqdns:
 
             zones = self.pdns.get_all_zones_for_item(fqdn)
             if not zones:
-                LOG.warning(_("Did not found an appropriate zone for address {!r}.").format(fqdn))
+                LOG.warning(_('Did not found an appropriate zone for address {!r}.').format(fqdn))
                 continue
 
             for zone_name in zones:
                 if zone_name not in zones_of_records:
                     zones_of_records[zone_name] = {}
                 zones_of_records[zone_name][fqdn] = {}
 
         if self.verbose > 2:
-            LOG.debug("Zones of addresses:\n{}".format(pp(zones_of_records)))
+            LOG.debug(_('Zones of addresses:') + '\n' + pp(zones_of_records))
         return zones_of_records
 
     # -------------------------------------------------------------------------
     def _verify_fqdns_in_pdns_zones(self, zone_name, zones_of_records, fqdns_found=None):
 
         if self.verbose > 1:
-            LOG.debug("Verifying FQDNs for zone {!r}.".format(zone_name))
+            LOG.debug(_('Verifying FQDNs for zone {!r}.').format(zone_name))
 
         if fqdns_found is None:
             fqdns_found = []
 
         zone = self.pdns.zones[zone_name]
         zone.update()
         if self.verbose > 1:
-            LOG.debug("Found {c} resource record sets (RRSET) for zone {z!r}.".format(
+            LOG.debug(_('Found {c} resource record sets (RRSET) for zone {z!r}.').format(
                 c=len(zone.rrsets), z=zone_name))
 
         for fqdn in zones_of_records[zone_name]:
             fqdns_in_zone_found = self._verify_fqdn_in_pdns_zone(zone_name, fqdn)
             if fqdns_in_zone_found:
                 fqdns_found += fqdns_in_zone_found
 
@@ -457,18 +442,18 @@
 
         zone = self.pdns.zones[zone_name]
         fqdns_in_zone_found = []
 
         fqdn_puny = to_str(fqdn.encode('idna'))
         if self.verbose > 1:
             if fqdn != fqdn_puny:
-                LOG.debug("Searching {f!r} ({p!r}) in zone {z!r} ...".format(
+                LOG.debug(_('Searching {f!r} ({p!r}) in zone {z!r} ...').format(
                     f=fqdn, p=fqdn_puny, z=zone_name))
             else:
-                LOG.debug("Searching {f!r} in zone {z!r} ...".format(f=fqdn, z=zone_name))
+                LOG.debug(_('Searching {f!r} in zone {z!r} ...').format(f=fqdn, z=zone_name))
 
         for rrset in zone.rrsets:
 
             if rrset.name != fqdn:
                 if fqdn == fqdn_puny:
                     continue
                 if rrset.name != fqdn_puny:
@@ -488,130 +473,132 @@
             for record in rrset.records:
                 if zone.reverse_zone and rrset.type.upper() == 'PTR':
                     if self.expected_ptr is not None and fqdn_puny in self.expected_ptr:
                         ptr = self.pdns.decanon_name(fqdn_puny)
                         exp = self.pdns.decanon_name(self.expected_ptr[fqdn_puny])
                         addr = self.pdns.decanon_name(record.content)
                         if self.verbose > 1:
-                            LOG.debug("Expexted PTR: {p!r} => {a!r}.".format(p=ptr, a=exp))
+                            LOG.debug(_('Expexted PTR: {p!r} => {a!r}.').format(p=ptr, a=exp))
                         if record.content != self.expected_ptr[fqdn_puny]:
                             LOG.warning(_(
-                                "PTR {p!r} does not pointing to expected {e!r}, "
-                                "but to {c!r} instead, ignoring for deletion.").format(
+                                'PTR {p!r} does not pointing to expected {e!r}, '
+                                'but to {c!r} instead, ignoring for deletion.').format(
                                 p=ptr, e=exp, c=addr))
                             continue
                 record2remove = {'content': record.content, 'disabled': record.disabled}
                 rrset2remove['records'].append(record2remove)
             if zone_name not in self.records2remove:
                 self.records2remove[zone_name] = []
             self.records2remove[zone_name].append(rrset2remove)
             if fqdn_puny not in fqdns_in_zone_found:
                 fqdns_in_zone_found.append(fqdn_puny)
 
         return fqdns_in_zone_found
 
     # -------------------------------------------------------------------------
     def verify_addresses(self, addresses):
-
-        LOG.debug("Verifying all given DNS addresses.")
+        """Verify all given DNS addresses."""
+        LOG.debug(_('Verifying all given DNS addresses.'))
 
         fqdns_found = []
 
         all_fqdns = self._canon_addresses(addresses)
         zones_of_records = self._get_zones_of_addresses(all_fqdns)
 
         if not zones_of_records:
-            msg = _("Did not found any addresses with an appropriate zone in PowerDNS.")
+            msg = _('Did not found any addresses with an appropriate zone in PowerDNS.')
             LOG.error(msg)
             return 1
 
         if self.verbose > 1:
-            LOG.debug("Found zones for addresses:\n{}".format(pp(zones_of_records)))
+            LOG.debug(_('Found zones for addresses:') + '\n' + pp(zones_of_records))
 
         for zone_name in zones_of_records:
             fqdns_found = self._verify_fqdns_in_pdns_zones(
                 zone_name, zones_of_records, fqdns_found)
         if self.verbose > 2:
-            LOG.debug("The following FQDNs were found:\n{}".format(pp(fqdns_found)))
+            LOG.debug(_('The following FQDNs were found:') + '\n' + pp(fqdns_found))
 
         fqdns_not_found = []
         for fqdn in all_fqdns:
             if fqdn not in fqdns_found:
                 fqdns_not_found.append(fqdn)
         if fqdns_not_found:
-            msg = _("The following addresses (FQDNs) are not found:")
+            msg = _('The following addresses (FQDNs) are not found:')
             for fqdn in fqdns_not_found:
                 msg += '\n  * {!r}'.format(fqdn)
             LOG.warning(msg)
 
         if not self.records2remove:
             return 1
 
         if self.verbose > 2:
-            LOG.debug("Found resource record sets to remove:\n{}".format(pp(self.records2remove)))
+            msg = _('Found resource record sets to remove:')
+            msg += '\n' + pp(self.records2remove)
+            LOG.debug(msg)
 
         return 0
 
     # -------------------------------------------------------------------------
     def get_reverse_records(self):
-
-        LOG.debug("Retrieving reverse records of A and AAAA records.")
+        """Evaluate reverse PTR records of A and AAAA records."""
+        LOG.debug(_('Evaluating reverse PTR records of A and AAAA records.'))
 
         addresses = []
         self.expected_ptr = {}
 
         for zone_name in self.records2remove:
 
             for rrset in self.records2remove[zone_name]:
 
                 if rrset['type'] not in ('A', 'AAAA'):
                     continue
 
                 for record in rrset['records']:
                     addr_str = record['content']
-                    LOG.debug("Trying to get reverse address of {!r} ...".format(addr_str))
+                    LOG.debug(_('Try to get reverse address of {!r} ...').format(addr_str))
                     addr = None
                     fqdn = None
 
                     try:
                         addr = ipaddress.ip_address(addr_str)
                         fqdn = self.pdns.canon_name(reverse_pointer(addr))
                     except ValueError:
-                        msg = _("IP address {!r} seems not to be a valid IP address.").format(
+                        msg = _('IP address {!r} seems not to be a valid IP address.').format(
                             addr_str)
                         LOG.error(msg)
                         continue
-                    LOG.debug("Found reverse address {!r}.".format(fqdn))
+                    LOG.debug(_('Found reverse address {!r}.').format(fqdn))
                     if fqdn not in addresses:
                         addresses.append(fqdn)
                     self.expected_ptr[fqdn] = rrset['fqdn']
 
         if not addresses:
             return 0
 
         if self.verbose > 1:
-            LOG.debug("Expected PTR records:\n{}".format(pp(self.expected_ptr)))
+            LOG.debug(_('Expected PTR records:') + '\n' + pp(self.expected_ptr))
 
         return self.verify_addresses(addresses)
 
     # -------------------------------------------------------------------------
     def show_records(self):
-
-        title = _("All DNS records to remove")
+        """Display all DNS records to remove on screen."""
+        title = _('All DNS records to remove')
         print()
         print(title)
-        print("=" * len(title))
+        print('=' * len(title))
         print()
 
         disabled = _('Disabled.')
         headers = {
-            'fqdn': _("Name"),
+            'fqdn': _('Name'),
             'z': _('Zone'),
-            'type': _("Type"),
-            'rec': _("Record"),
+            'type': _('Type'),
+            'rec': _('Record'),
             'dis': '',
         }
         lengths = {
             'fqdn': len(headers['fqdn']),
             'z': len(headers['z']),
             'type': len(headers['type']),
             'rec': len(headers['rec']),
@@ -633,19 +620,19 @@
                     lengths['type'] = len(rr_type)
                 for record in rrset['records']:
                     count += 1
                     content = self.pdns.decanon_name(record['content'])
                     if len(content) > lengths['rec']:
                         lengths['rec'] = len(content)
 
-        tpl = "{{fqdn:<{}}}  ".format(lengths['fqdn'])
-        tpl += "{{z:<{}}}  ".format(lengths['z'])
-        tpl += "{{type:<{}}}  ".format(lengths['type'])
-        tpl += "{{rec:<{}}}  ".format(lengths['rec'])
-        tpl += "{{dis:<{}}}".format(lengths['dis'])
+        tpl = '{{fqdn:<{}}}  '.format(lengths['fqdn'])
+        tpl += '{{z:<{}}}  '.format(lengths['z'])
+        tpl += '{{type:<{}}}  '.format(lengths['type'])
+        tpl += '{{rec:<{}}}  '.format(lengths['rec'])
+        tpl += '{{dis:<{}}}'.format(lengths['dis'])
 
         header = tpl.format(**headers)
         print(header)
         print('-' * len(header))
 
         for zone_name in sorted(
                 self.records2remove.keys(), key=lambda x: cmp_to_key(compare_fqdn)(x)):
@@ -659,20 +646,20 @@
                     out['rec'] = content
                     if record['disabled']:
                         out['dis'] = disabled
                     else:
                         out['dis'] = ''
                     print(tpl.format(**out))
         print()
-        msg = ngettext("Total one DNS record to remove.", "Total {} DNS records to remove.", count)
+        msg = ngettext('Total one DNS record to remove.', 'Total {} DNS records to remove.', count)
         print(msg.format(count))
         print()
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/bulk_rm_cfg.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/bulk_rm_cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: A module for providing a configuration for the pdns-bulk-remove application.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 by Frank Brehm, Berlin
-@summary: A module for providing a configuration for the pdns-bulk-remove application
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard module
 import logging
 import re
 
 # Third party modules
-
-# Own modules
 from fb_tools.common import to_bool
+from fb_tools.config import BaseConfiguration
+from fb_tools.config import ConfigError
 
-from fb_tools.config import ConfigError, BaseConfiguration
-
-from . import DEFAULT_PORT, DEFAULT_API_PREFIX
+# Own modules
+from . import DEFAULT_API_PREFIX
+from . import DEFAULT_PORT
+from .xlate import XLATOR
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 LOG = logging.getLogger(__name__)
 
+_ = XLATOR.gettext
+ngettext = XLATOR.ngettext
+
 
 # =============================================================================
 class PdnsBulkRmConfigError(ConfigError):
-    """Base error class for all exceptions happened during
-    execution this configured application"""
+    """Error class for all exceptions reading configuration of the pdns-bulk-remove app."""
 
     pass
 
 
 # =============================================================================
 class PdnsBulkRmCfg(BaseConfiguration):
-    """
-    A class for providing a configuration for the GetVmApplication class
-    and methods to read it from configuration files.
-    """
+    """A class for providing a configuration for the GetVmApplication class."""
 
     default_pdns_master = 'master.pp-dns.com'
     default_pdns_api_port = DEFAULT_PORT
     default_pdns_api_https = False
     default_pdns_api_prefix = DEFAULT_API_PREFIX
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             encoding=None, config_dir=None, config_file=None, initialized=False):
-
+        """Initialize the PdnsBulkRmCfg object."""
         self.pdns_master = self.default_pdns_master
         self.pdns_api_port = self.default_pdns_api_port
         self.pdns_api_key = None
         self.pdns_api_https = self.default_pdns_api_https
         self.pdns_api_prefix = self.default_pdns_api_prefix
 
         super(PdnsBulkRmCfg, self).__init__(
@@ -63,51 +64,50 @@
 
         if initialized:
             self.initialized = True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(PdnsBulkRmCfg, self).as_dict(short=short)
 
         res['pdns_api_key'] = None
         if self.pdns_api_key:
             if self.verbose > 4:
                 res['pdns_api_key'] = self.pdns_api_key
             else:
                 res['pdns_api_key'] = '*******'
 
         return res
 
     # -------------------------------------------------------------------------
     def eval_config_section(self, config, section_name):
-
+        """Evaluate configuration in the section with the given name."""
         super(PdnsBulkRmCfg, self).eval_config_section(config, section_name)
 
         if section_name.lower() in ('pdns', 'powerdns'):
             self._eval_config_pdns(config, section_name)
             return
 
         if self.verbose > 1:
-            LOG.debug("Unhandled configuration section {!r}.".format(section_name))
+            LOG.debug(_('Unhandled configuration section {!r}.').format(section_name))
 
     # -------------------------------------------------------------------------
     def _eval_config_pdns(self, config, section_name):
 
         if self.verbose > 1:
-            LOG.debug("Checking config section {!r} ...".format(section_name))
+            LOG.debug(_('Checking config section {!r} ...').format(section_name))
 
         re_api_key = re.compile(r'^\s*(?:api[_-]?)?key\s*', re.IGNORECASE)
         re_api_prefix = re.compile(r'^\s*(?:api[_-]?)?prefix\s*', re.IGNORECASE)
 
         for (key, value) in config.items(section_name):
 
             if key.lower() == 'master':
@@ -126,14 +126,14 @@
                 self.pdns_api_prefix = str(value).strip()
 
         return
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/errors.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,165 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+summary: The module for special error classes on PowerDNS API operations.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
-@summary: The module for special error classes on PowerDNS API operations.
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 
 # Own modules
 from fb_tools.errors import FbHandlerError
 
 from .xlate import XLATOR
 
 _ = XLATOR.gettext
 
-__version__ = '0.2.4'
+__version__ = '0.3.1'
 
 
 # =============================================================================
 class PowerDNSHandlerError(FbHandlerError):
     """Base class for all exception belonging to PowerDNS."""
+
     pass
 
 
 # =============================================================================
 class PowerDNSZoneError(PowerDNSHandlerError):
+    """Exception class for errors in DNS zones handling."""
+
     pass
 
 
 # =============================================================================
+class PDNSNoRecordsToRemove(PowerDNSZoneError):
+    """Special exception for the case, that there are no more Records left to remove."""
+
+    # -------------------------------------------------------------------------
+    def __init__(self, zone_name):
+        """Initialize the PDNSNoRecordsToRemove object."""
+        self.zone_name = zone_name
+
+    # -------------------------------------------------------------------------
+    def __str__(self):
+        """Typecast into a string."""
+        msg = _('No Resource Record Sets found to remove from zone {!r}.').format(
+            self.zone_name)
+        return msg
+
+
+# =============================================================================
 class PowerDNSRecordError(PowerDNSHandlerError):
+    """Exception class for errors in DNS records handling."""
+
     pass
 
 
 # =============================================================================
 class PowerDNSWrongRecordTypeError(PowerDNSRecordError, TypeError):
+    """Special exception in case of a wrong DNS record type."""
+
     pass
 
 
 # =============================================================================
 class PowerDNSRecordSetError(PowerDNSHandlerError):
+    """Exception class for errors in DNS record sets handling."""
+
     pass
 
 
 # =============================================================================
 class PowerDNSWrongSoaDataError(PowerDNSRecordSetError):
+    """Special exception in case of wrong DNS SOA record data."""
 
     # -------------------------------------------------------------------------
     def __init__(self, data):
+        """Initialize the PowerDNSWrongSoaDataError object."""
         self.data = str(data)
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
-        msg = _("Could not interprete SOA data: {!r}.").format(self.data)
+        """Typecast into a string."""
+        msg = _('Could not interprete SOA data: {!r}.').format(self.data)
         return msg
 
 
 # =============================================================================
 class PDNSApiError(PowerDNSHandlerError):
-    """Base class for more complex exceptions"""
+    """Base class for more complex exceptions."""
 
     # -------------------------------------------------------------------------
     def __init__(self, code, msg, uri=None):
+        """Initialize the PDNSApiError object."""
         self.code = code
         self.msg = msg
         self.uri = uri
 
     # -------------------------------------------------------------------------
     def __str__(self):
-
+        """Typecast into a string."""
         if self.uri:
-            msg = _("Got a {code} error code from {uri!r}: {msg}").format(
+            msg = _('Got a {code} error code from {uri!r}: {msg}').format(
                 code=self.code, uri=self.uri, msg=self.msg)
         else:
-            msg = _("Got a {code} error code: {msg}").format(code=self.code, msg=self.msg)
+            msg = _('Got a {code} error code: {msg}').format(code=self.code, msg=self.msg)
 
         return msg
 
 
 # =============================================================================
 class PDNSApiNotAuthorizedError(PDNSApiError):
-    """The authorization information provided is not correct"""
+    """The authorization information provided is not correct."""
+
     pass
 
 
 # =============================================================================
 class PDNSApiNotFoundError(PDNSApiError):
-    """The ProfitBricks entity was not found"""
+    """The ProfitBricks entity was not found."""
+
     pass
 
 
 # =============================================================================
 class PDNSApiValidationError(PDNSApiError):
-    """The HTTP data provided is not valid"""
+    """The HTTP data provided is not valid."""
+
     pass
 
 
 # =============================================================================
 class PDNSApiRateLimitExceededError(PDNSApiError):
-    """The number of requests sent have exceeded the allowed API rate limit"""
+    """The number of requests sent have exceeded the allowed API rate limit."""
+
     pass
 
 
 # =============================================================================
 class PDNSApiRequestError(PDNSApiError):
-    """Base error for request failures"""
+    """Base error for request failures."""
+
     pass
 
 
 # =============================================================================
 class PDNSApiTimeoutError(PDNSApiRequestError):
     """Raised when a request does not finish in the given time span."""
+
     pass
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/record.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/record.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: An encapsulation class for a DNS record object by PowerDNS API.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
-@summary: An encapsulation class for a DNS record object by PowerDNS API
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
 import copy
-import re
 import datetime
+import logging
+import re
 import time
-
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # Third party modules
-import six
-
-# Own modules
-from fb_tools.common import pp, compare_fqdn, to_utf8, to_str
-
+from fb_tools.common import compare_fqdn
+from fb_tools.common import pp
+from fb_tools.common import to_str
+from fb_tools.common import to_utf8
 from fb_tools.obj import FbBaseObject
 
-from .xlate import XLATOR
+import six
 
-from . import BasePowerDNSHandler, DEFAULT_PORT, DEFAULT_API_PREFIX
+# Own modules
 
+from . import DEFAULT_API_PREFIX, DEFAULT_PORT
+from .base_handler import BasePowerDNSHandler
+from .common import seconds2human
+from .errors import PowerDNSRecordSetError
 from .errors import PowerDNSWrongRecordTypeError
-from .errors import PowerDNSRecordSetError, PowerDNSWrongSoaDataError
+from .errors import PowerDNSWrongSoaDataError
+from .xlate import XLATOR
 
-__version__ = '0.6.3'
+__version__ = '0.7.0'
 
 LOG = logging.getLogger(__name__)
 
 TYPE_ORDER = {
     'SOA': 0,
     'NS': 1,
     'MX': 2,
@@ -53,22 +57,22 @@
 }
 
 _ = XLATOR.gettext
 
 
 # =============================================================================
 def compare_rrsets(x, y):
-
+    """Compare two DNS record sets - thich function can be used for sorting record set lists."""
     if not isinstance(x, PowerDNSRecordSet):
-        raise TypeError(_("Argument {a} {v!r} must be a {o} object.").format(
+        raise TypeError(_('Argument {a} {v!r} must be a {o} object.').format(
             a='x', v=x, o='PowerDNSRecordSet'))
 
     if not isinstance(y, PowerDNSRecordSet):
-        raise TypeError(_("Argument {a} {v!r} must be a {o} object.").format(
-            a='y', v=x, o='PowerDNSRecordSet'))
+        raise TypeError(_('Argument {a} {v!r} must be a {o} object.').format(
+            a='y', v=y, o='PowerDNSRecordSet'))
 
     ret = compare_fqdn(x.name, y.name)
     if ret:
         return ret
 
     xt = 99
     yt = 99
@@ -82,20 +86,21 @@
     if xt > yt:
         return 1
     return 0
 
 
 # =============================================================================
 class PowerDNSRecord(FbBaseObject):
+    """Encapsulation class of a DNS record (part of a DNS record set) in PowerDNS."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             content=None, disabled=False):
-
+        """Initialize a PowerDNSRecord record."""
         self._content = None
         if content:
             self._content = to_str(str(content))
         self._disabled = False
         self.disabled = disabled
 
         super(PowerDNSRecord, self).__init__(
@@ -103,31 +108,31 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def content(self):
-        "The underlying content of this record."
+        """Give the underlying content of this record."""
         return self._content
 
     # -----------------------------------------------------------
     @property
     def disabled(self):
-        "Flag, whether the record is disabled or not."
+        """Flag, whether the record is disabled or not."""
         return self._disabled
 
     @disabled.setter
     def disabled(self, value):
         self._disabled = bool(value)
 
     # -----------------------------------------------------------
     @property
     def enabled(self):
-        "Flag, whether the record is enabled or not."
+        """Flag, whether the record is enabled or not."""
         if self.disabled:
             return False
         return True
 
     @enabled.setter
     def enabled(self, value):
         v = bool(value)
@@ -135,25 +140,24 @@
             self._disabled = False
         else:
             self._disabled = True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, minimal=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param minimal: Generate a minimal dict, which can be used for the PDNS API
         @type minimal: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if minimal:
             return {
                 'content': self.content,
                 'disabled': self.disabled,
             }
 
         res = super(PowerDNSRecord, self).as_dict(short=short)
@@ -161,52 +165,49 @@
         res['disabled'] = self.disabled
         res['enabled'] = self.enabled
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSRecord as a deep copy of the current object."""
         return PowerDNSRecord(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized, content=self.content, disabled=self.disabled)
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(short=True))
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecast into a string for reproduction."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("content={!r}".format(self.content))
-        fields.append("disabled={!r}".format(self.disabled))
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("version={!r}".format(self.version))
+        fields.append('content={!r}'.format(self.content))
+        fields.append('disabled={!r}'.format(self.disabled))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('version={!r}'.format(self.version))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing equality of {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing equality of {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, PowerDNSRecord):
             return False
 
         if self.content is None:
             if other.content is None:
                 return True
@@ -218,21 +219,20 @@
         if self.content.lower() != other.content.lower():
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def __lt__(self, other):
-        """ The '<' operator. """
-
+        """Magic method for using it as the '<'-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing less than of {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing less than of {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, PowerDNSRecord):
-            msg = _("Wrong type {cls} of other parameter {other!r} for comparision.").format(
+            msg = _('Wrong type {cls} of other parameter {other!r} for comparision.').format(
                 cls=other.__class__.__name__, other=other)
             raise PowerDNSWrongRecordTypeError(msg)
 
         if self == other:
             return False
 
         if self.content is None:
@@ -241,22 +241,21 @@
         if other.content is None:
             return False
 
         return self.content.lower() < other.content.lower()
 
     # -------------------------------------------------------------------------
     def __gt__(self, other):
-        """ The '>' operator. """
-
+        """Magic method for using it as the '>'-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing greater than of {} objects ...").format(
+            LOG.debug(_('Comparing greater than of {} objects ...').format(
                 self.__class__.__name__))
 
         if not isinstance(other, PowerDNSRecord):
-            msg = _("Wrong type {cls} of other parameter {other!r} for comparision.").format(
+            msg = _('Wrong type {cls} of other parameter {other!r} for comparision.').format(
                 cls=other.__class__.__name__, other=other)
             raise PowerDNSWrongRecordTypeError(msg)
 
         if self == other:
             return False
 
         if self.content is None:
@@ -266,24 +265,25 @@
             return True
 
         return self.content.lower() > other.content.lower()
 
 
 # =============================================================================
 class PowerDnsSOAData(FbBaseObject):
+    """Encapsulation class of a SOA (Start of authority) DNS record."""
 
     re_soa_data = re.compile(r'^\s*(\S+)\s+(\S+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s*$')
     re_ws = re.compile(r'\s+')
 
     # -------------------------------------------------------------------------
     def __init__(
         self, primary=None, email=None, serial=None, refresh=None, retry=None, expire=None,
             ttl=None, appname=None, verbose=0, version=__version__,
             base_dir=None):
-
+        """Initialize a PowerDnsSOAData record."""
         self._primary = None
         self._email = None
         self._serial = None
         self._refresh = None
         self._retry = None
         self._expire = None
         self._ttl = None
@@ -305,172 +305,248 @@
             self.initialized = True
         else:
             self.initialized = False
 
     # -----------------------------------------------------------
     @property
     def primary(self):
-        "The primary name server of this SOA"
+        """Return the primary name server of this SOA record."""
         return self._primary
 
     @primary.setter
     def primary(self, value):
         if value is None:
             self._primary = None
             return
         self._primary = str(value).strip().lower()
 
     # -----------------------------------------------------------
     @property
     def email(self):
-        "The E-Mail-address of the hostmaster of this zone."
+        """Return the E-Mail-address of the hostmaster of this zone."""
         return self._email
 
     @email.setter
     def email(self, value):
         if value is None:
             self._email = None
             return
         self._email = str(value).strip().lower()
 
     # -----------------------------------------------------------
     @property
     def serial(self):
-        "The serial number of this SOA."
+        """Return the serial number of this SOA record."""
         return self._serial
 
     @serial.setter
     def serial(self, value):
         if value is None:
             self._serial = None
             return
         self._serial = int(value)
 
     # -----------------------------------------------------------
     @property
     def refresh(self):
-        "The time in seconds when slaves should ask master for changes."
+        """Return the time in seconds when slaves should ask master for changes."""
         return self._refresh
 
     @refresh.setter
     def refresh(self, value):
         if value is None:
             self._refresh = None
             return
         self._refresh = int(value)
 
     # -----------------------------------------------------------
     @property
+    def refresh_human(self):
+        """Return the refresh time in a human readable format."""
+        if self._refresh is None:
+            return None
+        return seconds2human(self._refresh)
+
+    # -----------------------------------------------------------
+    @property
     def retry(self):
-        """The time in seconds when slaves should retry getting changes from master,
-            if an attemt to get it was not successful."""
+        """
+        Return the retry time in seconds.
+
+        The time in seconds when slaves should retry getting changes from master,
+        if an attemt to get it was not successful.
+        """
         return self._retry
 
     @retry.setter
     def retry(self, value):
         if value is None:
             self._retry = None
             return
         self._retry = int(value)
 
     # -----------------------------------------------------------
     @property
+    def retry_human(self):
+        """Return the retry time in a human readable format."""
+        if self._retry is None:
+            return None
+        return seconds2human(self._retry)
+
+    # -----------------------------------------------------------
+    @property
     def expire(self):
-        """The time in seconds when slaves should expiring the zone,
-            if an attemt to get it was not successful."""
+        """
+        Retrun the expire time of the zone.
+
+        This is the time in seconds when slaves should expiring the zone,
+        if an attemt to get it was not successful.
+        """
         return self._expire
 
     @expire.setter
     def expire(self, value):
         if value is None:
             self._expire = None
             return
         self._expire = int(value)
 
     # -----------------------------------------------------------
     @property
+    def expire_human(self):
+        """Return the expire time in a human readable format."""
+        if self._expire is None:
+            return None
+        return seconds2human(self._expire)
+
+    # -----------------------------------------------------------
+    @property
     def ttl(self):
-        "The defaul TTL of this zone."
+        """Return the default TTL of this zone."""
         return self._ttl
 
     @ttl.setter
     def ttl(self, value):
         if value is None:
             self._ttl = None
             return
         self._ttl = int(value)
 
     # -----------------------------------------------------------
     @property
+    def ttl_human(self):
+        """Return the ttl of the zone in a human readable format."""
+        if self._ttl is None:
+            return None
+        return seconds2human(self._ttl)
+
+    # -----------------------------------------------------------
+    @property
     def data(self):
-        "String representation of SOA data."
-        if self.primary and self.email and self.serial is not None and self.refresh and \
-                self.retry and self.expire and self.ttl:
-            return "{_primary} {_email} {_serial} {_refresh} {_retry} {_expire} {_ttl}".format(
-                **self.__dict__)
-        else:
+        """Return a string representation of SOA data."""
+        if not self.primary:
+            return None
+        if not self.email:
             return None
+        if self.serial is None:
+            return None
+        if not self.refresh:
+            return None
+        if not self.retry:
+            return None
+        if not self.expire:
+            return None
+        if not self.ttl:
+            return None
+        return '{_primary} {_email} {_serial} {_refresh} {_retry} {_expire} {_ttl}'.format(
+            **self.__dict__)
+
+    # -----------------------------------------------------------
+    @property
+    def data_human(self):
+        """Return a string representation of SOA data in a human readable format."""
+        if not self.primary:
+            return None
+        if not self.email:
+            return None
+        if self.serial is None:
+            return None
+        if not self.refresh:
+            return None
+        if not self.retry:
+            return None
+        if not self.expire:
+            return None
+        if not self.ttl:
+            return None
+        return '{primary} {email} {serial} {refresh!r} {retry!r} {expire!r} {ttl!r}'.format(
+            primary=self.primary, email=self.email, serial=self.serial, refresh=self.refresh_human,
+            retry=self.retry_human, expire=self.expire_human, ttl=self.ttl_human)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(PowerDnsSOAData, self).as_dict(short=short)
         res['primary'] = self.primary
         res['email'] = self.email
         res['serial'] = self.serial
         res['refresh'] = self.refresh
+        res['refresh_human'] = self.refresh_human
         res['retry'] = self.retry
+        res['retry_human'] = self.retry_human
         res['expire'] = self.expire
+        res['expire_human'] = self.expire_human
         res['ttl'] = self.ttl
+        res['ttl_human'] = self.ttl_human
         res['data'] = self.data
+        res['data_human'] = self.data_human
 
         return res
 
     # -------------------------------------------------------------------------
     @classmethod
     def init_from_data(cls, data, appname=None, verbose=0, base_dir=None):
-
+        """Create a PowerDnsSOAData on base of the SOA data given from DNS."""
         line = cls.re_ws.sub(' ', to_str(data))
         match = cls.re_soa_data.match(line)
         if not match:
             raise PowerDNSWrongSoaDataError(data)
 
         soa = cls(
             primary=match.group(1), email=match.group(2), serial=match.group(3),
             refresh=match.group(4), retry=match.group(5), expire=match.group(6),
             ttl=match.group(7), appname=appname, verbose=verbose, base_dir=base_dir)
 
         return soa
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDnsSOAData as a deep copy of the current object."""
         if self.verbose > 4:
-            LOG.debug(_("Copying current {}-object in a new one.").format(self.__class__.__name__))
+            LOG.debug(_('Copying current {}-object in a new one.').format(self.__class__.__name__))
 
         soa = PowerDnsSOAData(
             primary=self.primary, email=self.email, serial=self.serial, refresh=self.refresh,
             retry=self.retry, expire=self.expire, ttl=self.ttl, appname=self.appname,
             version=self.version, base_dir=self.base_dir)
         return soa
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, PowerDnsSOAData):
             return False
 
         if self.primary != other.primary:
             return False
         if self.email != other.email:
@@ -486,15 +562,15 @@
         if self.ttl != other.ttl:
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def increase_serial(self):
-
+        """Increase the serial number in current SOA to the current date + sequential number."""
         i = 0
         tpl = '{year:4d}{month:02d}{day:02d}{nr:02d}'
         curdate = datetime.date.today()
         new_serial = 0
 
         params = {
             'year': curdate.year,
@@ -506,48 +582,46 @@
         while new_serial <= self.serial:
             new_serial = int(tpl.format(**params))
             if new_serial > self.serial:
                 break
             i += 1
             if i > 99:
                 msg = _(
-                    "Serial overflow - old serial {o} is in future, new serial {n} "
-                    "has reached its maximum value.").format(o=self.serial, n=new_serial)
+                    'Serial overflow - old serial {o} is in future, new serial {n} '
+                    'has reached its maximum value.').format(o=self.serial, n=new_serial)
                 raise ValueError(msg)
             params['nr'] = i
 
         self.serial = new_serial
         return new_serial
 
 
 # =============================================================================
 class PowerDNSRecordList(MutableSequence):
-    """
-    A list containing Power DNS Records (as parts of a Record Set).
-    """
+    """A list containing Power DNS Records (as parts of a Record Set)."""
 
-    msg_no_pdns_record = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_pdns_record = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(self, *records):
-
+        """Initialize a PowerDNSRecordList object."""
         self._list = []
 
         for record in records:
             self.append(record)
 
     # -------------------------------------------------------------------------
     def index(self, record, *args):
-
+        """Return the numeric index of the given record in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -577,20 +651,20 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == record:
                 return index
 
-        msg = _("Record {!r} is not in Record list.").format(record.content)
+        msg = _('Record {!r} is not in Record list.').format(record.content)
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, record):
-
+        """Return whether the given record is contained in current list."""
         if not isinstance(record, PowerDNSRecord):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=record.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecord'))
 
         if not self._list:
             return False
 
@@ -598,15 +672,15 @@
             if item == record:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, record):
-
+        """Return the number of records which are equal to the given one in current list."""
         if not isinstance(record, PowerDNSRecord):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=record.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecord'))
 
         if not self._list:
             return 0
 
@@ -614,86 +688,87 @@
         for item in self._list:
             if item == record:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of records in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a record from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the records in list in place."""
         return reversed(self._list)
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, record):
-
+        """Replace the record at the given numeric index by the given one."""
         if not isinstance(record, PowerDNSRecord):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=record.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecord'))
 
         self._list.__setitem__(key, record)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the record at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, record):
-
+        """Append the given record to the current list."""
         if not isinstance(record, PowerDNSRecord):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=record.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecord'))
 
         self._list.append(record)
 
     # -------------------------------------------------------------------------
     def insert(self, index, record):
-
+        """Insert the given record in current list at given index."""
         if not isinstance(record, PowerDNSRecord):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=record.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecord'))
 
         self._list.insert(index, record)
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSRecordList as a deep copy of the current object."""
         new_list = self.__class__()
         for record in self._list:
             new_list.append(copy.copy(record))
         return new_list
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the PowerDNSRecordList."
-
+        """Remove all items from the PowerDNSRecordList."""
         self._list = []
 
     # -------------------------------------------------------------------------
     def clean(self):
-        "Wrapper for clear()"
-
+        """Do exactly the same like clear() (wrapper for it)."""
         return self.clear()
 
 
 # =============================================================================
 class PowerDNSRecordSetComment(FbBaseObject):
+    """This class encapsulates a comment to a DNS Record set."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None, initialized=None,
             account=None, content='', modified_at=None):
-
+        """Initialize a PowerDNSRecordSetComment object."""
         self._account = None
         self._content = ''
         self._modified_at = int(time.time() + 0.5)
 
         super(PowerDNSRecordSetComment, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir)
 
@@ -703,15 +778,15 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -------------------------------------------------------------------------
     @property
     def account(self):
-        "The name of the account, who has created this comment"
+        """Give the name of the account, who has created this comment."""
         return self._account
 
     @account.setter
     def account(self, value):
         if value is None:
             self._account = None
             return
@@ -720,80 +795,78 @@
             self._account = None
             return
         self._account = v
 
     # -------------------------------------------------------------------------
     @property
     def content(self):
-        "The underlying content of this comment"
+        """Give the underlying content of this comment."""
         return self._content
 
     @content.setter
     def content(self, value):
         if value is None:
             self._content = ''
             return
         v = str(value).strip()
         self._content = v
 
     # -------------------------------------------------------------------------
     @property
     def modified_at(self):
-        "The UNIX time stamp of the last modification of this comment."
+        """Give the UNIX time stamp of the last modification of this comment."""
         return self._modified_at
 
     @modified_at.setter
     def modified_at(self, value):
         if value is None:
             self._modified_at = int(time.time() + 0.5)
             return
         try:
             v = int(value)
         except ValueError as e:
             msg = (_(
-                "Invalid value for {w} of a {c} object - ").format(
+                'Invalid value for {w} of a {c} object - ').format(
                 w='modified_at', c=self.__class__.__name__) + str(e))
             raise ValueError(msg)
         if v < 0:
             msg = _(
-                "Invalid value for {w} {v!r} of a {c} object - "
-                "must be greater than or equal to zero.").format(
+                'Invalid value for {w} {v!r} of a {c} object - '
+                'must be greater than or equal to zero.').format(
                 w='modified_at', c=self.__class__.__name__, v=value)
             raise ValueError(msg)
         self._modified_at = v
 
     # -------------------------------------------------------------------------
     @property
     def modified_date(self):
-        "The modification of this comment as a datetime object."
-
+        """Give the modification of this comment as a datetime object."""
         return datetime.datetime.utcfromtimestamp(self.modified_at)
 
     # -------------------------------------------------------------------------
     @property
     def valid(self):
-        "Is this a valid comment or not."
+        """Is this a valid comment or not."""
         if self.account is None or self.modified_at is None:
             return False
         return True
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, minimal=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param minimal: Generate a minimal dict, which can be used for the PDNS API
         @type minimal: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if minimal:
             return {
                 'account': self.account,
                 'content': self.content,
                 'modified_at': self.modified_at,
             }
 
@@ -804,54 +877,51 @@
         res['modified_date'] = self.modified_date
         res['valid'] = self.valid
 
         return res
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSRecordSetComment as a deep copy of the current object."""
         return PowerDNSRecordSetComment(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             initialized=self.initialized,
             account=self.account, content=self.content, modified_at=self.modified_at)
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast for translating object structure into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(minimal=True))
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecast into a string for reproduction."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("account={!r}".format(self.account))
-        fields.append("content={!r}".format(self.content))
-        fields.append("modified_at={!r}".format(self.modified_at))
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("version={!r}".format(self.version))
+        fields.append('account={!r}'.format(self.account))
+        fields.append('content={!r}'.format(self.content))
+        fields.append('modified_at={!r}'.format(self.modified_at))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('version={!r}'.format(self.version))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, PowerDNSRecordSetComment):
             return False
 
         if self.account != other.account:
             return False
 
@@ -862,30 +932,30 @@
             return False
 
         return True
 
 
 # =============================================================================
 class PowerDNSRecordSet(BasePowerDNSHandler):
+    """Encapsulates a set of DNS records wth the same name and the same type."""
 
     default_ttl = 3600
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             master_server=None, port=DEFAULT_PORT, key=None, use_https=False,
             timeout=None, path_prefix=DEFAULT_API_PREFIX, simulate=None, force=None,
             terminal_has_colors=False, initialized=None):
-
+        """Initialize a PowerDNSRecordSet object."""
         # {   'comments': [],
         #     'name': 'www.bmwi.tv.',
         #     'records': [{'content': '77.74.236.5', 'disabled': False}],
         #     'ttl': 3600,
         #     'type': 'A'},
-
         self.comments = []
         self._name = None
         self.ttl = self.default_ttl
         self._type = None
         self.records = PowerDNSRecordList()
 
         super(PowerDNSRecordSet, self).__init__(
@@ -897,84 +967,92 @@
 
         if initialized is not None:
             self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def name(self):
-        "The name of this record set."
+        """Give the name of this record set."""
         return self._name
 
     @name.setter
     def name(self, value):
         if not isinstance(value, six.string_types):
-            msg = _("A {w} must be a string type, but is {v!r} instead.").format(
+            msg = _('A {w} must be a string type, but is {v!r} instead.').format(
                 w='PowerDNSRecordSet.name', v=value)
             raise TypeError(msg)
         v = to_str(value).strip().lower()
         if v == '':
-            msg = _("A {w} may not be empty: {v!r}.").format(
+            msg = _('A {w} may not be empty: {v!r}.').format(
                 w='PowerDNSRecordSet.name', v=value)
             raise ValueError(msg)
         self._name = v
 
     # -----------------------------------------------------------
     @property
     def name_unicode(self):
-        """The name of the resource record set in unicode, if it is an IDNA encoded zone."""
+        """Give the name of the resource record set in unicode, if it is an IDNA encoded zone."""
         n = getattr(self, '_name', None)
         if n is None:
             return None
         if 'xn--' in n:
             return to_utf8(n).decode('idna')
         return n
 
     # -----------------------------------------------------------
     @property
-    def type(self):
-        "The type of this record set."
+    def type(self):                                                                 # noqa: A003
+        """Give the type of this record set."""
         return self._type
 
     @type.setter
-    def type(self, value):
+    def type(self, value):                                                          # noqa: A003
         if not isinstance(value, six.string_types):
-            msg = _("A {w} must be a string type, but is {v!r} instead.").format(
+            msg = _('A {w} must be a string type, but is {v!r} instead.').format(
                 w='PowerDNSRecordSet.type', v=value)
             raise TypeError(msg)
         v = to_str(value).strip().upper()
         if v == '':
-            msg = _("A {w} may not be empty: {v!r}.").format(
+            msg = _('A {w} may not be empty: {v!r}.').format(
                 w='PowerDNSRecordSet.type', v=value)
             raise ValueError(msg)
         v = self.verify_rrset_type(v)
         self._type = v
 
     # -----------------------------------------------------------
     @property
     def ttl(self):
-        "The TTL of this record set."
+        """Return the TTL of this record set."""
         return self._ttl
 
     @ttl.setter
     def ttl(self, value):
         self._ttl = int(value)
 
+    # -----------------------------------------------------------
+    @property
+    def ttl_human(self):
+        """Return the ttl of the record set in a human readable format."""
+        if self._ttl is None:
+            return None
+        return seconds2human(self._ttl)
+
     # -------------------------------------------------------------------------
     @classmethod
     def init_from_dict(
         cls, data, appname=None, verbose=0, version=__version__, base_dir=None,
             master_server=None, port=DEFAULT_PORT, key=None, use_https=False, timeout=None,
             path_prefix=DEFAULT_API_PREFIX, simulate=None, force=None,
             terminal_has_colors=False, initialized=None):
-
+        """Create a new PowerDNSRecordSet object based on a given dict."""
         if not isinstance(data, dict):
-            raise PowerDNSRecordSetError(_("Given data {!r} is not a dict object.").format(data))
+            raise PowerDNSRecordSetError(_('Given data {!r} is not a dict object.').format(data))
 
         if verbose > 3:
-            LOG.debug(_("Creating {} object from data:").format(cls.__name__) + '\n' + pp(data))
+            LOG.debug(_('Creating {} object from data:').format(cls.__name__) + '\n' + pp(data))
 
         params = {
             'appname': appname,
             'verbose': verbose,
             'version': version,
             'base_dir': base_dir,
             'master_server': master_server,
@@ -1027,15 +1105,15 @@
 
         rrset.initialized = True
 
         return rrset
 
     # -------------------------------------------------------------------------
     def name_relative(self, reference):
-
+        """Extract the name from the current set name relative to the given reference."""
         # current name must be an absolute name
         if not self.name.endswith('.'):
             return self.name
 
         # reference name must be an absolute name
         if not reference.endswith('.'):
             return self.name
@@ -1043,43 +1121,43 @@
         ref_escaped = r'\.' + re.escape(reference) + r'$'
         rel_name = re.sub(ref_escaped, '', self.name)
         return rel_name
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True, minimal=False):
         """
-        Transforms the elements of the object into a dict
+        Transform the element of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
         @param minimal: Generate a minimal dict, which can be used for the PDNS API
         @type minimal: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         if minimal:
             ret = {
-                "comments": [],
-                "name": self.name,
-                "records": [],
-                "ttl": self.ttl,
-                "type": self.type,
+                'comments': [],
+                'name': self.name,
+                'records': [],
+                'ttl': self.ttl,
+                'type': self.type,
             }
             for comment in self.comments:
                 ret['comments'].append(comment.as_dict(minimal=True))
             for record in self.records:
                 ret['records'].append(record.as_dict(minimal=True))
             return ret
 
         res = super(PowerDNSRecordSet, self).as_dict(short=short)
         res['name'] = self.name
         res['type'] = self.type
         res['ttl'] = self.ttl
+        res['ttl_human'] = self.ttl_human
         res['name_unicode'] = self.name_unicode
         res['comments'] = []
         res['records'] = []
 
         for record in self.records:
             res['records'].append(record.as_dict(short))
 
@@ -1087,26 +1165,24 @@
             res['comments'].append(comment.as_dict(short=short))
 
         return res
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast for translating object structure into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(short=True))
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSRecordSet as a deep copy of the current object."""
         rrset = PowerDNSRecordSet(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             master_server=self.master_server, port=self.port, key=self.key,
             use_https=self.use_https, timeout=self.timeout, path_prefix=self.path_prefix,
             simulate=self.simulate, force=self.force,
             terminal_has_colors=self.terminal_has_colors, initialized=False)
 
@@ -1117,75 +1193,72 @@
         rrset.records = copy.copy(self.records)
 
         rrset.initialized = True
         return rrset
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if self.verbose > 4:
-            LOG.debug(_("Comparing {} objects ...").format(self.__class__.__name__))
+            LOG.debug(_('Comparing {} objects ...').format(self.__class__.__name__))
 
         if not isinstance(other, PowerDNSRecordSet):
             return False
 
         if self.name != other.name:
             return False
 
         if self.type != other.type:
             return False
 
         return True
 
     # -------------------------------------------------------------------------
     def get_soa_data(self):
-
+        """Extract a PowerDnsSOAData object from record content, if current type is SOA."""
         if self.type != 'SOA':
-            msg = (_("Cannot create {o} from record set:") + "\n{rs}").format(
-                o='PowerDnsSOAData', rs=pp(self.as_dict()))
+            msg = _('Cannot create {o} from record set:').format(
+                o='PowerDnsSOAData') + '\n' + pp(self.as_dict())
             raise PowerDNSRecordSetError(msg)
 
         if not self.records:
-            msg = (_("RecordSet has no records:") + "\n{}").format(
-                pp(self.as_dict()))
+            msg = _('RecordSet has no records:') + '\n' + pp(self.as_dict())
             raise PowerDNSRecordSetError(msg)
 
         record = self.records[0]
         soa = PowerDnsSOAData.init_from_data(
             record.content, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir)
         if self.verbose > 3:
-            LOG.debug((_("Got SOA:") + "\n{}").format(pp(soa.as_dict())))
+            LOG.debug(_('Got SOA:') + '\n' + pp(soa.as_dict()))
         return soa
 
 
 # =============================================================================
 class PowerDNSRecordSetList(MutableSequence):
-    """
-    A list containing Power DNS Record Sets (of a zone).
-    """
+    """A list containing Power DNS Record Sets (of a zone)."""
 
-    msg_no_pdns_rrset = _("Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.")
+    msg_no_pdns_rrset = _('Invalid type {t!r} as an item of a {c}, only {o} objects are allowed.')
 
     # -------------------------------------------------------------------------
     def __init__(self, *rrsets):
-
+        """Initialize a PowerDNSRecordSetList object."""
         self._list = []
 
         for rrset in rrsets:
             self.append(rrset)
 
     # -------------------------------------------------------------------------
     def index(self, rrset, *args):
-
+        """Return the numeric index of the given record set in current list."""
         i = None
         j = None
 
         if len(args) > 0:
             if len(args) > 2:
-                raise TypeError(_("{m} takes at most {max} arguments ({n} given).").format(
+                raise TypeError(_('{m} takes at most {max} arguments ({n} given).').format(
                     m='index()', max=3, n=len(args) + 1))
             i = int(args[0])
             if len(args) > 1:
                 j = int(args[1])
 
         index = 0
         start = 0
@@ -1215,21 +1288,21 @@
             for index in list(range(len(self._list))):
                 item = self._list[index]
                 if index >= end:
                     break
             if item == rrset:
                 return index
 
-        msg = _("RecordSet {n!r} ({n}) is not in RecordSet list.").format(
+        msg = _('RecordSet {n!r} ({n}) is not in RecordSet list.').format(
             n=rrset.name, t=rrset.type)
         raise ValueError(msg)
 
     # -------------------------------------------------------------------------
     def __contains__(self, rrset):
-
+        """Return whether the given record set is contained in current list."""
         if not isinstance(rrset, PowerDNSRecordSet):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=rrset.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecordSet'))
 
         if not self._list:
             return False
 
@@ -1237,15 +1310,15 @@
             if item == rrset:
                 return True
 
         return False
 
     # -------------------------------------------------------------------------
     def count(self, rrset):
-
+        """Return the number of record sets which are equal to the given one in current list."""
         if not isinstance(rrset, PowerDNSRecordSet):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=rrset.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecordSet'))
 
         if not self._list:
             return 0
 
@@ -1253,74 +1326,75 @@
         for item in self._list:
             if item == rrset:
                 num += 1
         return num
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of record sets in current list."""
         return len(self._list)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a record set from current list by the given numeric index."""
         return self._list.__getitem__(key)
 
     # -------------------------------------------------------------------------
     def __reversed__(self):
-
+        """Reverse the record sets in list in place."""
         return reversed(self._list)
 
     # -------------------------------------------------------------------------
     def __setitem__(self, key, rrset):
-
+        """Replace the record set at the given numeric index by the given one."""
         if not isinstance(rrset, PowerDNSRecordSet):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=rrset.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecordSet'))
 
         self._list.__setitem__(key, rrset)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
-
+        """Remove the record set at the given numeric index from list."""
         del self._list[key]
 
     # -------------------------------------------------------------------------
     def append(self, rrset):
-
+        """Append the given record set to the current list."""
         if not isinstance(rrset, PowerDNSRecordSet):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=rrset.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecordSet'))
 
         self._list.append(rrset)
 
     # -------------------------------------------------------------------------
     def insert(self, index, rrset):
-
+        """Insert the given record set in current list at given index."""
         if not isinstance(rrset, PowerDNSRecordSet):
             raise TypeError(self.msg_no_pdns_record.format(
                 t=rrset.__class__.__name__, c=self.__class__.__name__, o='PowerDNSRecordSet'))
 
         self._list.insert(index, rrset)
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSRecordSetList as a deep copy of the current object."""
         new_list = self.__class__()
         for rrset in self._list:
             new_list.append(copy.copy(rrset))
         return new_list
 
     # -------------------------------------------------------------------------
     def clear(self):
-        "Remove all items from the PowerDNSRecordSetList."
-
+        """Remove all items from the PowerDNSRecordSetList."""
         self._list = []
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/server.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: The module for a PowerDNS server handler object.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 by Frank Brehm, Berlin
-@summary: The module for a PowerDNS server handler object.
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
 import logging
 import re
 
 # Third party modules
 
-# Own modules
 from fb_tools.common import pp, to_bool, to_str
-
 from fb_tools.handling_obj import HandlingObject
 
-from .xlate import XLATOR
-
-from . import BasePowerDNSHandler, DEFAULT_PORT, DEFAULT_API_PREFIX
-
+# Own modules
+from . import DEFAULT_API_PREFIX
+from . import DEFAULT_PORT
+from .base_handler import BasePowerDNSHandler
 from .errors import PDNSApiNotFoundError, PDNSApiValidationError
-
+from .xlate import XLATOR
 from .zone import PowerDNSZone, PowerDNSZoneDict
 
-__version__ = '0.8.0'
+__version__ = '0.8.2'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class PowerDNSServer(BasePowerDNSHandler):
-    """
-    Class for a PowerDNS server handler.
-    """
+    """Class for a PowerDNS server handler."""
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
             master_server=None, port=DEFAULT_PORT, key=None, use_https=False,
             path_prefix=DEFAULT_API_PREFIX, simulate=None, force=None,
             terminal_has_colors=False, initialized=False):
-
+        """Initialize a PowerDNSServer record."""
         self._api_servername = self.default_api_servername
         self._api_server_version = 'unknown'
         self.zones = None
 
         super(PowerDNSServer, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
             master_server=master_server, port=port, key=key, use_https=use_https,
@@ -59,164 +56,164 @@
         )
 
         self.initialized = initialized
 
     # -----------------------------------------------------------
     @property
     def api_server_version(self):
-        "The version of the PowerDNS server, how provided by API."
+        """Geet the version of the PowerDNS server, how provided by API."""
         return self._api_server_version
 
     # -----------------------------------------------------------
     @HandlingObject.simulate.setter
     def simulate(self, value):
+        """Override the setter of the simulate property."""
         self._simulate = to_bool(value)
 
         if self.initialized:
-            LOG.debug(_("Setting simulate of all subsequent objects to {!r} ...").format(
+            LOG.debug(_('Setting simulate of all subsequent objects to {!r} ...').format(
                 self.simulate))
 
         if self.zones:
             for zone_name in self.zones:
                 self.zones[zone_name].simulate = self.simulate
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(PowerDNSServer, self).as_dict(short=short)
         res['api_server_version'] = self.api_server_version
 
         return res
 
     # -------------------------------------------------------------------------
     def get_api_server_version(self):
-
-        path = "/servers/{}".format(self.api_servername)
+        """Retreive from PowerDNS API their server version."""
+        path = '/servers/{}'.format(self.api_servername)
         try:
             json_response = self.perform_request(path)
         except (PDNSApiNotFoundError, PDNSApiValidationError):
-            LOG.error(_("Could not found server info."))
+            LOG.error(_('Could not found server info.'))
             return None
         if self.verbose > 2:
-            LOG.debug(_("Got a response:") + '\n' + pp(json_response))
+            LOG.debug(_('Got a response:') + '\n' + pp(json_response))
 
         if 'version' in json_response:
             self._api_server_version = to_str(json_response['version'])
-            LOG.info(_("PowerDNS server version {!r}.").format(self.api_server_version))
+            LOG.info(_('PowerDNS server version {!r}.').format(self.api_server_version))
             return self.api_server_version
-        LOG.error(_("Did not found version info in server info:") + "\n" + pp(json_response))
+        LOG.error(_('Did not found version info in server info:') + '\n' + pp(json_response))
         return None
 
     # -------------------------------------------------------------------------
     def get_api_zones(self):
+        """Pull from PowerDNS API a list of all zones and return them as a PowerDNSZoneDict."""
+        LOG.debug(_('Trying to get all zones from PDNS API ...'))
 
-        LOG.debug(_("Trying to get all zones from PDNS API ..."))
-
-        path = "/servers/{}/zones".format(self.api_servername)
+        path = '/servers/{}/zones'.format(self.api_servername)
         json_response = self.perform_request(path)
         if self.verbose > 3:
-            LOG.debug(_("Got a response:") + '\n' + pp(json_response))
+            LOG.debug(_('Got a response:') + '\n' + pp(json_response))
 
         self.zones = PowerDNSZoneDict()
 
         for data in json_response:
             zone = PowerDNSZone.init_from_dict(
                 data, appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
                 master_server=self.master_server, port=self.port, key=self.key,
                 use_https=self.use_https, timeout=self.timeout, path_prefix=self.path_prefix,
                 simulate=self.simulate, force=self.force, initialized=True)
             self.zones.append(zone)
             if self.verbose > 3:
-                print("{!r}".format(zone))
+                print('{!r}'.format(zone))
 
         if self.verbose > 1:
-            msg = ngettext("Found a zone.", "Found {n} zones.", len(self.zones))
+            msg = ngettext('Found a zone.', 'Found {n} zones.', len(self.zones))
             LOG.debug(msg.format(n=len(self.zones)))
 
         if self.verbose > 2:
             if self.verbose > 3:
-                LOG.debug(_("Zones:") + '\n' + pp(self.zones.as_list()))
+                LOG.debug(_('Zones:') + '\n' + pp(self.zones.as_list()))
             else:
-                LOG.debug(_("Zones:") + '\n' + pp(list(self.zones.keys())))
+                LOG.debug(_('Zones:') + '\n' + pp(list(self.zones.keys())))
 
         return self.zones
 
     # -------------------------------------------------------------------------
     def get_zone_for_item(self, item, is_fqdn=False):
-
+        """Search for the best fitting zone for the given FQDN."""
         if not len(self.zones):
             self.get_api_zones()
 
         fqdn = self.name2fqdn(item, is_fqdn=is_fqdn)
         if not fqdn:
             return None
 
         if self.verbose > 2:
-            LOG.debug(_("Searching an appropriate zone for item {i!r} - FQDN {f!r} ...").format(
+            LOG.debug(_('Searching an appropriate zone for item {i!r} - FQDN {f!r} ...').format(
                 i=item, f=fqdn))
 
         for zone_name in reversed(self.zones.keys()):
             pattern = r'\.' + re.escape(zone_name) + '$'
             if self.verbose > 3:
-                LOG.debug(_("Search pattern: {}").format(pattern))
+                LOG.debug(_('Search pattern: {}').format(pattern))
             if re.search(pattern, fqdn):
                 return zone_name
             zone = self.zones[zone_name]
             if zone_name != zone.name_unicode:
                 pattern = r'\.' + re.escape(zone.name_unicode) + '$'
                 if self.verbose > 3:
-                    LOG.debug(_("Search pattern Unicode: {}").format(pattern))
+                    LOG.debug(_('Search pattern Unicode: {}').format(pattern))
                 if re.search(pattern, fqdn):
                     return zone_name
 
         return None
 
     # -------------------------------------------------------------------------
     def get_all_zones_for_item(self, item, is_fqdn=False):
-
+        """Search for all fitting zones for the given FQDN."""
         if not len(self.zones):
             self.get_api_zones()
 
         fqdn = self.name2fqdn(item, is_fqdn=is_fqdn)
         if not fqdn:
             return []
 
         if self.verbose > 2:
-            LOG.debug(_("Searching all appropriate zones for item {i!r} - FQDN {f!r} ...").format(
+            LOG.debug(_('Searching all appropriate zones for item {i!r} - FQDN {f!r} ...').format(
                 i=item, f=fqdn))
         zones = []
 
         for zone_name in self.zones.keys():
             pattern = r'\.' + re.escape(zone_name) + '$'
             if self.verbose > 3:
-                LOG.debug(_("Search pattern: {}").format(pattern))
+                LOG.debug(_('Search pattern: {}').format(pattern))
             if re.search(pattern, fqdn):
                 zones.append(zone_name)
                 continue
             zone = self.zones[zone_name]
             if zone_name != zone.name_unicode:
                 pattern = r'\.' + re.escape(zone.name_unicode) + '$'
                 if self.verbose > 3:
-                    LOG.debug(_("Search pattern Unicode: {}").format(pattern))
+                    LOG.debug(_('Search pattern Unicode: {}').format(pattern))
                 if re.search(pattern, fqdn):
                     zones.append(zone_name)
 
         return zones
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/xlate.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/xlate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-@author: Frank Brehm
-@contact: frank@brehm-online.com
-@copyright: © 2021 by Frank Brehm, Berlin
 @summary: The module for i18n.
+
           It provides translation object, usable from all other
           modules in this package.
+@author: Frank Brehm
+@contact: frank@brehm-online.com
+@copyright: © 2023 by Frank Brehm, Berlin
 """
 from __future__ import absolute_import, print_function
 
 # Standard modules
-import logging
-import gettext
 import copy
+import gettext
+import logging
 import sys
-
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
-
 try:
     from packaging.version import Version
 except ImportError:
     from distutils.version import LooseVersion as Version
 
 # Third party modules
 import babel
 import babel.lists
 from babel.support import Translations
 
 DOMAIN = 'fb_pdnstools'
 
 LOG = logging.getLogger(__name__)
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 __me__ = Path(__file__).resolve()
 __module_dir__ = __me__.parent
 __lib_dir__ = __module_dir__.parent
 __base_dir__ = __lib_dir__.parent
 LOCALE_DIR = __base_dir__.joinpath('locale')
 if LOCALE_DIR.is_dir():
@@ -77,14 +76,15 @@
 _ = XLATOR.gettext
 
 
 # =============================================================================
 def format_list(lst, do_repr=False, style='standard', locale=DEFAULT_LOCALE):
     """
     Format the items in `lst` as a list.
+
     :param lst: a sequence of items to format in to a list
     :param locale: the locale
     """
     if not lst:
         return ''
 
     my_list = copy.copy(lst)
@@ -96,18 +96,18 @@
     if CUR_BABEL_VERSION < NEWER_BABEL_VERSION:
         return babel.lists.format_list(my_list, locale=locale)
     return babel.lists.format_list(my_list, style=style, locale=locale)
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
-    print(_("Module directory: {!r}").format(__module_dir__))
-    print(_("Base directory: {!r}").format(__base_dir__))
-    print(_("Locale directory: {!r}").format(LOCALE_DIR))
-    print(_("Locale domain: {!r}").format(DOMAIN))
-    print(_("Found .mo-file: {!r}").format(__mo_file__))
+    print(_('Module directory: {!r}').format(__module_dir__))
+    print(_('Base directory: {!r}').format(__base_dir__))
+    print(_('Locale directory: {!r}').format(LOCALE_DIR))
+    print(_('Locale domain: {!r}').format(DOMAIN))
+    print(_('Found .mo-file: {!r}').format(__mo_file__))
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools/zone.py` & `fb_pdnstools-0.6.0/lib/fb_pdnstools/zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,94 +1,86 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: An encapsulation class for zone objects by PowerDNS API.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
-@summary: An encapsulation class for zone objects by PowerDNS API
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import absolute_import
 
 # Standard modules
-import logging
 import copy
-import re
 import ipaddress
 import json
-
+import logging
+import re
 from functools import cmp_to_key
-
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 
 # Third party modules
-import six
-
-# Own modules
-from fb_tools.common import pp, to_utf8, to_bool, compare_fqdn, RE_DOT, to_str
-from fb_tools.common import to_unicode, is_sequence
-
+from fb_tools.common import RE_DOT
+from fb_tools.common import compare_fqdn
+from fb_tools.common import is_sequence
+from fb_tools.common import pp
+from fb_tools.common import to_bool
+from fb_tools.common import to_str
+from fb_tools.common import to_unicode
+from fb_tools.common import to_utf8
 from fb_tools.obj import FbBaseObject
 
-from .xlate import XLATOR
-
-from . import BasePowerDNSHandler, DEFAULT_PORT, DEFAULT_API_PREFIX, FQDN_REGEX
+import six
 
+# Own modules
+from . import DEFAULT_API_PREFIX
+from . import DEFAULT_PORT
+from . import FQDN_REGEX
+from .base_handler import BasePowerDNSHandler
+from .errors import PDNSNoRecordsToRemove
 from .errors import PowerDNSZoneError
-
-from .record import PowerDnsSOAData, PowerDNSRecord
+from .record import PowerDNSRecord
+from .record import PowerDNSRecordSet
 from .record import PowerDNSRecordSetComment
-from .record import PowerDNSRecordSet, PowerDNSRecordSetList
+from .record import PowerDNSRecordSetList
+from .record import PowerDnsSOAData
+from .xlate import XLATOR
 
-__version__ = '0.11.2'
+__version__ = '0.11.6'
 
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 
 # =============================================================================
-class PDNSNoRecordsToRemove(PowerDNSZoneError):
-
-    # -------------------------------------------------------------------------
-    def __init__(self, zone_name):
-        self.zone_name = zone_name
-
-    # -------------------------------------------------------------------------
-    def __str__(self):
-
-        msg = _("No Resource Record Sets found to remove from zone {!r}.").format(
-            self.zone_name)
-        return msg
-
-
-# =============================================================================
 class PowerDNSZone(BasePowerDNSHandler):
-    """An encapsulation class for zone objects by PowerDNS API"""
+    """An encapsulation class for zone objects by PowerDNS API."""
 
     re_rev_ipv4 = re.compile(r'^((?:\d+\.)*\d+)\.in-addr\.arpa\.?$', re.IGNORECASE)
     re_rev_ipv6 = re.compile(r'^((?:[0-9a-f]\.)*[0-9a-f])\.ip6.arpa.?$', re.IGNORECASE)
 
     warn_on_unknown_property = False
 
     # -------------------------------------------------------------------------
     def __init__(
         self, appname=None, verbose=0, version=__version__, base_dir=None,
-            account=None, dnssec=False, edited_serial=None, id=None, kind=None,
+            account=None, dnssec=False, edited_serial=None, id=None, kind=None,     # noqa: A002
             last_check=None, master_tsig_key_ids=None, slave_tsig_key_ids=None,
             masters=None, name=None, notified_serial=None, serial=None, url=None,
             soa_edit=None, soa_edit_api=None, nsec3narrow=None, nsec3param=None,
             presigned=None, api_rectify=None, master_server=None, port=DEFAULT_PORT,
             key=None, use_https=False, timeout=None, path_prefix=DEFAULT_API_PREFIX,
             simulate=None, force=None, terminal_has_colors=False, initialized=None,
             **kwargs):
-
+        """Initialize a PowerDNSZone record."""
         self._account = account
         self._dnssec = dnssec
         self._id = id
         self._kind = kind
         self._last_check = last_check
         self.masters = []
         if masters:
@@ -126,15 +118,15 @@
 
         self._soa_edit = soa_edit
         self._soa_edit_api = soa_edit_api
 
         self._add_keys = {}
         if kwargs:
             self._add_keys = copy.copy(kwargs)
-            msg = _("Got unknown init parameters:") + '\n' + pp(self._add_keys)
+            msg = _('Got unknown init parameters:') + '\n' + pp(self._add_keys)
             if self.warn_on_unknown_property:
                 LOG.warn(msg)
             else:
                 LOG.debug(msg)
 
         super(PowerDNSZone, self).__init__(
             appname=appname, verbose=verbose, version=version, base_dir=base_dir,
@@ -151,17 +143,17 @@
     @classmethod
     def init_from_dict(
         cls, data,
             appname=None, verbose=0, version=__version__, base_dir=None,
             master_server=None, port=DEFAULT_PORT, key=None, use_https=False,
             timeout=None, path_prefix=DEFAULT_API_PREFIX,
             simulate=None, force=None, terminal_has_colors=False, initialized=None):
-
+        """Create a new PowerDNSZone object based on a given dict."""
         if not isinstance(data, dict):
-            raise PowerDNSZoneError(_("Given data {!r} is not a dict object.").format(data))
+            raise PowerDNSZoneError(_('Given data {!r} is not a dict object.').format(data))
 
         # {   'account': 'local',
         #     'api_rectify': False,
         #     'dnssec': False,
         #     'id': 'bla.ai.',
         #     'kind': 'Master',
         #     'last_check': 0,
@@ -218,15 +210,15 @@
         params.update(new_data)
 
         if verbose > 3:
             pout = copy.copy(params)
             pout['key'] = None
             if key:
                 pout['key'] = '******'
-            LOG.debug(_("Params initialisation:") + '\n' + pp(pout))
+            LOG.debug(_('Params initialisation:') + '\n' + pp(pout))
 
         zone = cls(**params)
 
         if rrsets:
             for single_rrset in rrsets:
                 rrset = PowerDNSRecordSet.init_from_dict(
                     single_rrset, appname=appname, verbose=verbose, base_dir=base_dir,
@@ -238,16 +230,19 @@
         zone.initialized = True
 
         return zone
 
     # -----------------------------------------------------------
     @property
     def account(self):
-        """The name of the owning account of the zone, internal used
-            to differ local visible zones from all other zones."""
+        """
+        Gives the name of the owning account of the zone.
+
+        Using `internal` to differ local visible zones from all other zones.
+        """
         return getattr(self, '_account', None)
 
     @account.setter
     def account(self, value):
         if value:
             v = to_str(str(value).strip())
             if v:
@@ -265,33 +260,33 @@
 
     @dnssec.setter
     def dnssec(self, value):
         self._dnssec = bool(value)
 
     # -----------------------------------------------------------
     @property
-    def id(self):
-        """The unique idendity of the zone."""
+    def id(self):                                                                   # noqa: A003
+        """Gives the unique idendity of the zone."""
         return getattr(self, '_id', None)
 
     @id.setter
-    def id(self, value):
+    def id(self, value):                                                            # noqa: A003
         if value:
             v = to_str(str(value).strip())
             if v:
                 self._id = v
             else:
                 self._id = None
         else:
             self._id = None
 
     # -----------------------------------------------------------
     @property
     def kind(self):
-        """The kind or type of the zone."""
+        """Gives the kind or type of the zone."""
         return getattr(self, '_kind', None)
 
     @kind.setter
     def kind(self, value):
         if value:
             v = to_str(str(value).strip())
             if v:
@@ -300,21 +295,21 @@
                 self._kind = None
         else:
             self._kind = None
 
     # -----------------------------------------------------------
     @property
     def last_check(self):
-        """The timestamp of the last check of the zone"""
+        """Gives the timestamp of the last check of the zone."""
         return getattr(self, '_last_check', None)
 
     # -----------------------------------------------------------
     @property
     def name(self):
-        """The name of the zone."""
+        """Gives the name of the zone."""
         return getattr(self, '_name', None)
 
     @name.setter
     def name(self, value):
         if value:
             v = to_str(str(value).strip())
             if v:
@@ -339,107 +334,109 @@
             self._name = None
             self._reverse_zone = False
             self._reverse_net = None
 
     # -----------------------------------------------------------
     @property
     def reverse_zone(self):
-        """Is this a reverse zone?"""
+        """Return, whether this is a reverse zone."""
         return self._reverse_zone
 
     # -----------------------------------------------------------
     @property
     def reverse_net(self):
-        """An IP network object representing the network, for which
-            this is the reverse zone."""
+        """Gives an IP network object for the network, for which this is the reverse zone."""
         return self._reverse_net
 
     # -----------------------------------------------------------
     @property
     def name_unicode(self):
-        """The name of the zone in unicode, if it is an IDNA encoded zone."""
+        """Gives name of the zone in unicode, if it is an IDNA encoded zone."""
         n = getattr(self, '_name', None)
         if n is None:
             return None
         if 'xn--' in n:
             return to_utf8(n).decode('idna')
         return n
 
     # -----------------------------------------------------------
     @property
     def notified_serial(self):
-        """The notified serial number of the zone"""
+        """Gives the notified serial number of the zone."""
         return getattr(self, '_notified_serial', None)
 
     # -----------------------------------------------------------
     @property
     def serial(self):
-        """The serial number of the zone"""
+        """Gives the serial number of the zone."""
         return getattr(self, '_serial', None)
 
     # -----------------------------------------------------------
     @property
     def edited_serial(self):
-        """The SOA serial as seen in query responses.
+        """
+        Gives the SOA serial as seen in query responses.
+
         Calculated using the SOA-EDIT metadata, default-soa-edit and
-        default-soa-edit-signed settings."""
+        default-soa-edit-signed settings.
+        """
         return getattr(self, '_edited_serial', None)
 
     # -----------------------------------------------------------
     @property
     def url(self):
-        """The URL in the API to get the zone object."""
+        """Gives the URL in the API to get the zone object."""
         return getattr(self, '_url', None)
 
     # -----------------------------------------------------------
     @property
     def soa_edit(self):
-        """The SOA edit property of the zone object."""
+        """Gives the SOA edit property of the zone object."""
         return getattr(self, '_soa_edit', None)
 
     # -----------------------------------------------------------
     @property
     def soa_edit_api(self):
-        """The SOA edit property (API) of the zone object."""
+        """Gives the SOA edit property (API) of the zone object."""
         return getattr(self, '_soa_edit_api', None)
 
     # -----------------------------------------------------------
     @property
     def nsec3narrow(self):
-        """Some stuff belonging to DNSSEC."""
+        """Gives some stuff belonging to DNSSEC."""
         return getattr(self, '_nsec3narrow', None)
 
     # -----------------------------------------------------------
     @property
     def nsec3param(self):
-        """Some stuff belonging to DNSSEC."""
+        """Gives some stuff belonging to DNSSEC."""
         return getattr(self, '_nsec3param', None)
 
     # -----------------------------------------------------------
     @property
     def presigned(self):
-        """Some stuff belonging to PowerDNS >= 4.1."""
+        """Gives some stuff belonging to PowerDNS >= 4.1."""
         return getattr(self, '_presigned', None)
 
     # -----------------------------------------------------------
     @property
     def api_rectify(self):
-        """Some stuff belonging to PowerDNS >= 4.1."""
+        """Gives some stuff belonging to PowerDNS >= 4.1."""
         return getattr(self, '_api_rectify', None)
 
     # -----------------------------------------------------------
     @property
     def add_keys(self):
-        """Additional, unexpected keys on initialisation."""
+        """Gives additional, unexpected keys on initialisation."""
         return copy.copy(self._add_keys)
 
     # -----------------------------------------------------------
     @property
     def master_tsig_key_ids(self):
-        """The id of the TSIG keys used for master operation in this zone."""
+        """Gives the id of the TSIG keys used for master operation in this zone."""
         return copy.copy(self._master_tsig_key_ids)
 
     @master_tsig_key_ids.setter
     def master_tsig_key_ids(self, key_ids):
         self._master_tsig_key_ids = []
         if key_ids:
             if is_sequence(key_ids):
@@ -463,24 +460,24 @@
                     self._slave_tsig_key_ids.append(key_id)
             else:
                 self._slave_tsig_key_ids.append(key_ids)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
         """
-        Transforms the elements of the object into a dict
+        Transform the elements of the object into a dict.
 
         @param short: don't include local properties in resulting dict.
         @type short: bool
 
         @return: structure as dict
         @rtype:  dict
         """
-
         res = super(PowerDNSZone, self).as_dict(short=short)
+
         res['account'] = self.account
         res['dnssec'] = copy.copy(self.dnssec)
         res['id'] = self.id
         res['kind'] = self.kind
         res['last_check'] = self.last_check
         res['masters'] = copy.copy(self.masters)
         res['name'] = self.name
@@ -509,27 +506,25 @@
                 res['rrsets'].append(rrset)
 
         return res
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """
-        Typecasting function for translating object structure
-        into a string
+        Typecast for translating object structure into a string.
 
         @return: structure as string
         @rtype:  str
         """
-
         return pp(self.as_dict(short=True))
 
     # -------------------------------------------------------------------------
     @classmethod
     def ipv4_nw_from_tuples(cls, tuples):
-
+        """Create ip_network-object from number tuples of the name of a reverse IPv4 zone."""
         bitmask = 0
         tokens = []
         for part in reversed(RE_DOT.split(tuples)):
             tokens.append(part)
 
         if len(tokens) == 3:
             tokens.append('0')
@@ -540,26 +535,26 @@
             bitmask = 16
         elif len(tokens) == 1:
             tokens.append('0')
             tokens.append('0')
             tokens.append('0')
             bitmask = 8
         else:
-            msg = _("Invalid source tuples for detecting IPv4-network: {!r}.").format(tuples)
+            msg = _('Invalid source tuples for detecting IPv4-network: {!r}.').format(tuples)
             raise ValueError(msg)
 
         ip_str = to_unicode('.'.join(tokens) + '/{}'.format(bitmask))
         net = ipaddress.ip_network(ip_str)
 
         return net
 
     # -------------------------------------------------------------------------
     @classmethod
     def ipv6_nw_from_tuples(cls, tuples):
-
+        """Create ip_network-object from hexnumber tuples of the name of a reverse IPv6 zone."""
         parts = RE_DOT.split(tuples)
         bitmask = 0
         tokens = []
         token = ''
         i = 0
 
         for part in reversed(parts):
@@ -583,39 +578,38 @@
         ip_str += to_unicode('/{}'.format(bitmask))
         net = ipaddress.ip_network(ip_str)
 
         return net
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        """Typecasting into a string for reproduction."""
-
-        out = "<%s(" % (self.__class__.__name__)
+        """Typecast into a string for reproduction."""
+        out = '<%s(' % (self.__class__.__name__)
 
         fields = []
-        fields.append("name={!r}".format(self.name))
-        fields.append("url={!r}".format(self.url))
-        fields.append("reverse_zone={!r}".format(self.reverse_zone))
-        fields.append("reverse_net={!r}".format(self.reverse_net))
-        fields.append("kind={!r}".format(self.kind))
-        fields.append("serial={!r}".format(self.serial))
-        fields.append("dnssec={!r}".format(self.dnssec))
-        fields.append("account={!r}".format(self.account))
-        fields.append("appname={!r}".format(self.appname))
-        fields.append("verbose={!r}".format(self.verbose))
-        fields.append("version={!r}".format(self.version))
+        fields.append('name={!r}'.format(self.name))
+        fields.append('url={!r}'.format(self.url))
+        fields.append('reverse_zone={!r}'.format(self.reverse_zone))
+        fields.append('reverse_net={!r}'.format(self.reverse_net))
+        fields.append('kind={!r}'.format(self.kind))
+        fields.append('serial={!r}'.format(self.serial))
+        fields.append('dnssec={!r}'.format(self.dnssec))
+        fields.append('account={!r}'.format(self.account))
+        fields.append('appname={!r}'.format(self.appname))
+        fields.append('verbose={!r}'.format(self.verbose))
+        fields.append('version={!r}'.format(self.version))
 
-        out += ", ".join(fields) + ")>"
+        out += ', '.join(fields) + ')>'
         return out
 
     # -------------------------------------------------------------------------
     def __copy__(self):
-
+        """Return a new PowerDNSZone as a deep copy of the current object."""
         if self.verbose > 3:
-            LOG.debug(_("Copying current {}-object into a new one.").format(
+            LOG.debug(_('Copying current {}-object into a new one.').format(
                 self.__class__.__name__))
 
         zone = self.__class__(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             account=self.account, dnssec=self.dnssec, edited_serial=self.edited_serial,
             id=self.id, kind=self.kind, last_check=self.last_check, masters=self.masters,
             name=self.name, notified_serial=self.notified_serial, serial=self.serial,
@@ -629,20 +623,20 @@
         zone.rrsets = copy.copy(self.rrsets)
 
         zone.initialized = True
         return zone
 
     # -------------------------------------------------------------------------
     def update(self):
-
+        """Update the records in the zone by requesting the API."""
         if not self.url:
-            msg = _("Cannot update zone {!r}, no API URL defined.").format(self.name)
+            msg = _('Cannot update zone {!r}, no API URL defined.').format(self.name)
             raise PowerDNSZoneError(msg)
 
-        LOG.debug(_("Updating data of zone {n!r} from API path {u!r} ...").format(
+        LOG.debug(_('Updating data of zone {n!r} from API path {u!r} ...').format(
             n=self.name, u=self.url))
         json_response = self.perform_request(self.url)
 
         if 'account' in json_response:
             self.account = json_response['account']
         else:
             self.account = None
@@ -724,33 +718,32 @@
                     path_prefix=self.path_prefix, simulate=self.simulate, force=self.force,
                     initialized=True)
                 self.rrsets.append(rrset)
 
     # -------------------------------------------------------------------------
     def perform_request(
             self, path, no_prefix=True, method='GET', data=None, headers=None, may_simulate=False):
-        """Performing the underlying API request."""
-
+        """Perform the underlying API request."""
         return super(PowerDNSZone, self).perform_request(
             path=path, no_prefix=no_prefix, method=method, data=data,
             headers=copy.copy(headers), may_simulate=may_simulate)
 
     # -------------------------------------------------------------------------
     def patch(self, payload):
-
+        """Perform a PATCH request with given payload to current zone."""
         if self.verbose > 1:
-            LOG.debug(_("Patching zone {!r} ...").format(self.name))
+            LOG.debug(_('Patching zone {!r} ...').format(self.name))
 
         return self.perform_request(
             self.url, method='PATCH',
             data=json.dumps(payload), may_simulate=True)
 
     # -------------------------------------------------------------------------
     def get_soa(self):
-
+        """Return a PowerDnsSOAData object created from the SOA record of this zone."""
         rrset = self.get_soa_rrset()
         if not rrset:
             return None
         return rrset.get_soa_data()
 
     # -------------------------------------------------------------------------
     def _generate_comments_list(self, comments=None):
@@ -766,95 +759,94 @@
         for cmt in comment_list_raw:
             if not cmt:
                 continue
             if isinstance(cmt, PowerDNSRecordSetComment):
                 if cmt.valid:
                     comment_list.append(copy.copy(cmt))
                 else:
-                    LOG.warn(_("Found invalid comment {!r}.").format(str(cmt)))
+                    LOG.warn(_('Found invalid comment {!r}.').format(str(cmt)))
             else:
                 cmt = str(cmt).strip()
                 comment = PowerDNSRecordSetComment(
                     appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
                     account='unknown', content=cmt, initialized=True)
                 comment_list.append(comment)
 
         return comment_list
 
     # -------------------------------------------------------------------------
     def update_soa(self, new_soa, comments=None, ttl=None):
-
+        """Update the SOA of the zone on the PowerDNS server."""
         if not isinstance(new_soa, PowerDnsSOAData):
-            msg = _("New SOA must be of type {e}, given {t}: {s!r}").format(
+            msg = _('New SOA must be of type {e}, given {t}: {s!r}').format(
                 e='PowerDnsSOAData', t=new_soa.__class__.__name__, s=new_soa)
             raise TypeError(msg)
 
         if ttl:
             ttl = int(ttl)
         else:
             if not len(self.rrsets):
                 self.update()
             cur_soa_rrset = self.get_soa()
             if not cur_soa_rrset:
-                raise RuntimeError(_("Got no SOA for zone {!r}.").format(self.name))
+                raise RuntimeError(_('Got no SOA for zone {!r}.').format(self.name))
             ttl = cur_soa_rrset.ttl
 
         comment_list = []
         for comment in new_soa.comments:
             if comment.content:
                 comment_list.append(comment)
 
         for comment in self._generate_comments_list(comments):
             if comment.content:
                 comment_list.append(comment)
 
         rrset = new_soa.as_dict(minimal=True)
-        rrset["comments"] = comment_list
-        rrset["changetype"] = 'REPLACE'
-        for record in rrset["records"]:
-            record["set-ptr"] = False
+        rrset['comments'] = comment_list
+        rrset['changetype'] = 'REPLACE'
+        for record in rrset['records']:
+            record['set-ptr'] = False
 
-        payload = {"rrsets": [rrset]}
+        payload = {'rrsets': [rrset]}
 
         if self.verbose > 1:
-            LOG.debug(_("Setting new SOA {s!r} for zone {z!r}, TTL {t} ...").format(
+            LOG.debug(_('Setting new SOA {s!r} for zone {z!r}, TTL {t} ...').format(
                 s=new_soa.data, z=self.name, t=ttl))
 
         self.patch(payload)
 
     # -------------------------------------------------------------------------
     def increase_serial(self):
-        "Increasing the serial number of current zone."
-
+        """Increase the serial number of current zone."""
         self.update()
 
         soa_rrset = self.get_soa_rrset()
         soa = soa_rrset.get_soa_data()
 
         old_serial = soa.serial
         new_serial = soa.increase_serial()
 
-        LOG.debug(_("Increasing serial of zone {z!r} from {o} => {n}.").format(
+        LOG.debug(_('Increasing serial of zone {z!r} from {o} => {n}.').format(
             z=self.name, o=old_serial, n=new_serial))
 
         new_soa_record = PowerDNSRecord(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             content=soa.data, disabled=False, initialized=True)
 
         soa_rrset.records.clear()
         soa_rrset.records.append(new_soa_record)
         self.replace_rrset(soa_rrset)
 
         # self.update_soa(soa)
 
     # -------------------------------------------------------------------------
     def generate_new_comment_list(self, rrset, comment=None, account=None, append_comments=True):
-
+        """Create a list of rrset comments from given PowerDNSRecordSet object and update it."""
         if not isinstance(rrset, PowerDNSRecordSet):
-            msg = _("Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.").format(
+            msg = _('Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.').format(
                 w='rrset', a=rrset, e='PowerDNSRecordSet', c=rrset.__class__.__name__)
             raise TypeError(msg)
 
         comment_list = []
         if append_comments:
             for cmt in rrset.comments:
                 if cmt.valid and cmt.content:
@@ -873,85 +865,85 @@
             comment_list.append(cmt)
 
         return comment_list
 
     # -------------------------------------------------------------------------
     def replace_rrset(
             self, rrset, set_ptr=False, comment=None, account=None, append_comments=True):
-
+        """Replace the recordset on the PDNS server."""
         if not isinstance(rrset, PowerDNSRecordSet):
-            msg = _("Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.").format(
+            msg = _('Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.').format(
                 w='rrset', a=rrset, e='PowerDNSRecordSet', c=rrset.__class__.__name__)
             raise TypeError(msg)
 
         comment_list = self.generate_new_comment_list(
             rrset, comment=comment, account=account, append_comments=append_comments)
         rrset.comments = comment_list
 
         rrset_dict = rrset.as_dict(minimal=True)
-        rrset_dict["changetype"] = 'REPLACE'
-        for record in rrset_dict["records"]:
-            record["set-ptr"] = bool(set_ptr)
+        rrset_dict['changetype'] = 'REPLACE'
+        for record in rrset_dict['records']:
+            record['set-ptr'] = bool(set_ptr)
 
-        payload = {"rrsets": [rrset_dict]}
-        LOG.debug(_("Replacing record set in zone {!r}.").format(self.name))
+        payload = {'rrsets': [rrset_dict]}
+        LOG.debug(_('Replacing record set in zone {!r}.').format(self.name))
 
         self.patch(payload)
 
     # -------------------------------------------------------------------------
     def delete_rrset(self, rrset):
-
+        """Delete the given recordset on the PDNS server."""
         if not isinstance(rrset, PowerDNSRecordSet):
-            msg = _("Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.").format(
+            msg = _('Parameter {w!r} {a!r} is not a {e} object, but a {c} object instead.').format(
                 w='rrset', a=rrset, e='PowerDNSRecordSet', c=rrset.__class__.__name__)
             raise TypeError(msg)
 
         rrset_dict = {
             'name': rrset.name,
-            "type": rrset.type,
-            "changetype": 'DELETE',
-            "records": [],
-            "comments": [],
+            'type': rrset.type,
+            'changetype': 'DELETE',
+            'records': [],
+            'comments': [],
         }
 
-        payload = {"rrsets": [rrset_dict]}
-        LOG.debug(_("Deleting record set in zone {!r}.").format(self.name))
+        payload = {'rrsets': [rrset_dict]}
+        LOG.debug(_('Deleting record set in zone {!r}.').format(self.name))
 
         self.patch(payload)
 
     # -------------------------------------------------------------------------
     def add_record_to_recordset(
         self, fqdn, rrset_type, content, ttl=None, disabled=False, set_ptr=False,
             comment=None, account=None, append_comments=True):
-
+        """Add a record to the given recordset on the PDNS server."""
         fqdn_used = self.verify_fqdn(fqdn)
         if not fqdn_used:
             return None
         rtype = self.verify_rrset_type(rrset_type)
         if not rtype:
             return None
         if self.verbose > 2:
-            msg = _("Adding FQDN: {f!r}, type {t!r}, content: {c!r}.").format(
+            msg = _('Adding FQDN: {f!r}, type {t!r}, content: {c!r}.').format(
                 f=fqdn_used, t=rtype, c=content)
             LOG.debug(msg)
 
         if ttl:
             ttl = int(ttl)
 
         rrset = self.get_rrset(fqdn, rrset_type)
         if rrset:
             if self.verbose > 1:
-                msg = _("Got an existing rrset for FQDN {f!r}, type {t!r}.").format(
+                msg = _('Got an existing rrset for FQDN {f!r}, type {t!r}.').format(
                     f=fqdn_used, t=rtype)
                 LOG.debug(msg)
             if ttl:
                 rrset.ttl = ttl
         else:
             if self.verbose > 1:
-                msg = _("Got no existing rrset for FQDN {f!r}, type {t!r}.").format(
+                msg = _('Got no existing rrset for FQDN {f!r}, type {t!r}.').format(
                     f=fqdn_used, t=rtype)
                 LOG.debug(msg)
             rrset = PowerDNSRecordSet(
                 appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
                 initialized=False)
             rrset.name = fqdn_used
             rrset.type = rrset_type
@@ -961,55 +953,55 @@
                 soa = self.get_soa()
                 rrset.ttl = soa.ttl
 
         record = PowerDNSRecord(
             appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
             content=content, disabled=bool(disabled), initialized=True)
         if record in rrset.records:
-            msg = _("Record {c!r} already contained in record set {f!r} type {t}.").format(
+            msg = _('Record {c!r} already contained in record set {f!r} type {t}.').format(
                 c=content, f=rrset.name, t=rrset.type)
             LOG.warn(msg)
             return
         rrset.records.append(record)
 
         self.replace_rrset(
             rrset, set_ptr=set_ptr, comment=comment, account=account,
             append_comments=bool(append_comments))
 
     # -------------------------------------------------------------------------
     def replace_record_in_recordset(
         self, fqdn, rrset_type, content, ttl=None, disabled=False, set_ptr=False,
             comment=None, account=None, append_comments=True):
-
+        """Replace a record in the given recordset on the PDNS server."""
         fqdn_used = self.verify_fqdn(fqdn)
         if not fqdn_used:
             return None
         rtype = self.verify_rrset_type(rrset_type)
         if not rtype:
             return None
         if self.verbose > 2:
-            msg = _("Replacing FQDN: {f!r}, type {t!r} by content: {c!r}.").format(
+            msg = _('Replacing FQDN: {f!r}, type {t!r} by content: {c!r}.').format(
                 f=fqdn_used, t=rtype, c=content)
             LOG.debug(msg)
 
         if ttl:
             ttl = int(ttl)
 
         rrset = self.get_rrset(fqdn, rrset_type)
         if rrset:
             if self.verbose > 1:
-                msg = _("Got an existing rrset for FQDN {f!r}, type {t!r}.").format(
+                msg = _('Got an existing rrset for FQDN {f!r}, type {t!r}.').format(
                     f=fqdn_used, t=rtype)
                 LOG.debug(msg)
             rrset.records.clear()
             if ttl:
                 rrset.ttl = ttl
         else:
             if self.verbose > 1:
-                msg = _("Got no existing rrset for FQDN {f!r}, type {t!r}.").format(
+                msg = _('Got no existing rrset for FQDN {f!r}, type {t!r}.').format(
                     f=fqdn_used, t=rtype)
                 LOG.debug(msg)
             rrset = PowerDNSRecordSet(
                 appname=self.appname, verbose=self.verbose, base_dir=self.base_dir,
                 initialized=False)
             rrset.name = fqdn_used
             rrset.type = rrset_type
@@ -1029,25 +1021,25 @@
             rrset, set_ptr=set_ptr, comment=comment, account=account,
             append_comments=bool(append_comments))
 
     # -------------------------------------------------------------------------
     def add_address_record(
         self, fqdn, address, ttl=None, disabled=False, set_ptr=True,
             comment=None, account=None, append_comments=False):
-
+        """Add a PTR record to the current (revertse) zone on the PDNS server."""
         if not isinstance(address, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
             msg = _(
-                "Parameter address {a!r} is not an IPv4Address or IPv6Address object, "
-                "but a {c} object instead.").format(a=address, c=address.__class__.__name__)
+                'Parameter address {a!r} is not an IPv4Address or IPv6Address object, '
+                'but a {c} object instead.').format(a=address, c=address.__class__.__name__)
             raise TypeError(msg)
 
         record_type = 'A'
         if address.version == 6:
             record_type = 'AAAA'
-        LOG.debug(_("Trying to create {t}-record {f!r} => {a!r}.").format(
+        LOG.debug(_('Trying to create {t}-record {f!r} => {a!r}.').format(
             t=record_type, f=fqdn, a=str(address)))
 
         canon_fqdn = self.canon_name(fqdn)
 
         self.add_record_to_recordset(
             fqdn=canon_fqdn, rrset_type=record_type, content=str(address),
             ttl=ttl, disabled=disabled, set_ptr=set_ptr,
@@ -1055,25 +1047,25 @@
 
         return True
 
     # -------------------------------------------------------------------------
     def set_address_record(
         self, fqdn, address, ttl=None, disabled=False, set_ptr=True,
             comment=None, account=None, append_comments=False):
-
+        """Replace a PTR record on the current (revertse) zone on the PDNS server."""
         if not isinstance(address, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
             msg = _(
-                "Parameter address {a!r} is not an IPv4Address or IPv6Address object, "
-                "but a {c} object instead.").format(a=address, c=address.__class__.__name__)
+                'Parameter address {a!r} is not an IPv4Address or IPv6Address object, '
+                'but a {c} object instead.').format(a=address, c=address.__class__.__name__)
             raise TypeError(msg)
 
         record_type = 'A'
         if address.version == 6:
             record_type = 'AAAA'
-        LOG.debug(_("Trying to create {t}-record {f!r} => {a!r}.").format(
+        LOG.debug(_('Trying to create {t}-record {f!r} => {a!r}.').format(
             t=record_type, f=fqdn, a=str(address)))
 
         canon_fqdn = self.canon_name(fqdn)
 
         self.replace_record_in_recordset(
             fqdn=canon_fqdn, rrset_type=record_type, content=str(address),
             ttl=ttl, disabled=disabled, set_ptr=set_ptr,
@@ -1081,202 +1073,203 @@
 
         return True
 
     # -------------------------------------------------------------------------
     def add_ptr_record(
         self, pointer, fqdn, ttl=None, disabled=False,
             comment=None, account=None, append_comments=False):
-
+        """Add a PTR record to the current (revertse) zone on the PDNS server."""
         canon_fqdn = self.canon_name(fqdn)
-        LOG.debug(_("Trying to create {t}-record {f!r} => {a!r}.").format(
+        LOG.debug(_('Trying to create {t}-record {f!r} => {a!r}.').format(
             t='PTR', f=pointer, a=canon_fqdn))
 
         self.replace_record_in_recordset(
             fqdn=pointer, rrset_type='PTR', content=canon_fqdn, ttl=ttl, disabled=disabled,
             set_ptr=False, comment=comment, account=account, append_comments=append_comments)
 
         return True
 
     # -------------------------------------------------------------------------
     def add_rrset_for_remove(self, fqdn, rr_type, rrsets=None):
-
+        """Append a dict for removing a recordset to a list."""
         if rrsets is None:
             rrsets = []
 
         rrset = {
-            "name": self.canon_name(fqdn),
-            "type": rr_type.upper(),
-            "records": [],
-            "comments": [],
-            "changetype": "DELETE",
+            'name': self.canon_name(fqdn),
+            'type': rr_type.upper(),
+            'records': [],
+            'comments': [],
+            'changetype': 'DELETE',
         }
         rrsets.append(rrset)
         return rrsets
 
     # -------------------------------------------------------------------------
     def del_rrsets(self, rrsets):
-
+        """Remove the recordsets in the given list fron PDNS server´."""
         if not rrsets:
             raise PDNSNoRecordsToRemove(self.name_unicode)
 
         self.update()
         if self.verbose > 3:
-            LOG.debug(_("Current zone:") + '\n' + pp(self.as_dict()))
+            LOG.debug(_('Current zone:') + '\n' + pp(self.as_dict()))
 
         rrsets_rm = []
 
         for rrset in rrsets:
             found = False
             for item in self.rrsets:
-                if item.name == rrset["name"] and item.type == rrset["type"]:
+                if item.name == rrset['name'] and item.type == rrset['type']:
                     found = True
                     break
             if not found:
-                msg = _("DNS {t!r}-record {n!r} is already deleted.").format(
-                    t=rrset["type"], n=rrset["name"])
+                msg = _('DNS {t!r}-record {n!r} is already deleted.').format(
+                    t=rrset['type'], n=rrset['name'])
                 LOG.warning(msg)
                 continue
             rrsets_rm.append(rrset)
         if not rrsets_rm:
             raise PDNSNoRecordsToRemove(self.name_unicode)
 
-        payload = {"rrsets": rrsets_rm}
+        payload = {'rrsets': rrsets_rm}
         count = len(rrsets_rm)
         msg = ngettext(
-            "Removing one resource record set from zone {z!r}.",
-            "Removing {c} resource record sets from zone {z!r}.", count).format(
+            'Removing one resource record set from zone {z!r}.',
+            'Removing {c} resource record sets from zone {z!r}.', count).format(
             c=count, z=self.name_unicode)
         LOG.info(msg)
         if self.verbose > 1:
-            LOG.debug(_("Resorce record sets:") + '\n' + pp(payload))
+            LOG.debug(_('Resorce record sets:') + '\n' + pp(payload))
 
         self.patch(payload)
-        LOG.info(_("Done."))
+        LOG.info(_('Done.'))
 
         return True
 
     # -------------------------------------------------------------------------
     def notify(self):
-
-        LOG.info(_("Notifying slave servers of zone {!r} ...").format(self.name))
+        """Initiate a notify of all secondary servers of current zone."""
+        LOG.info(_('Notifying slave servers of zone {!r} ...').format(self.name))
         path = self.url + '/notify'
         return self.perform_request(path, method='PUT', may_simulate=True)
 
     # -------------------------------------------------------------------------
     def verify_fqdn(self, fqdn, raise_on_error=True):
-
+        """Verify syntax of the given FQDN, and whether it fits into current zone."""
         if not isinstance(fqdn, six.string_types):
-            msg = _("A {w} must be a string type, but is {v!r} instead.").format(
+            msg = _('A {w} must be a string type, but is {v!r} instead.').format(
                 w='FQDN', v=fqdn)
             if raise_on_error:
                 raise TypeError(msg)
             LOG.error(msg)
             return None
 
         fqdn_used = to_str(fqdn).strip().lower()
         if not fqdn_used:
-            msg = _("Invalid, empty FQDN {!r} given.").format(fqdn)
+            msg = _('Invalid, empty FQDN {!r} given.').format(fqdn)
             if raise_on_error:
                 raise ValueError(msg)
             LOG.error(msg)
             return None
 
         if fqdn_used == '@':
             return self.name
 
         if fqdn_used == self.name:
             return self.name
 
         tail = '.' + self.name
         if self.verbose > 2:
-            LOG.debug(_("Checking FQDN {f!r} for ending on {t!r}.").format(
+            LOG.debug(_('Checking FQDN {f!r} for ending on {t!r}.').format(
                 f=fqdn_used, t=tail))
         if not fqdn_used.endswith(tail):
-            msg = _("Invalid FQDN {f!r}, it must end up with {t!r}.").format(
+            msg = _('Invalid FQDN {f!r}, it must end up with {t!r}.').format(
                 f=fqdn, t=tail)
             if raise_on_error:
                 raise ValueError(msg)
             LOG.error(msg)
             return None
 
         idx = fqdn_used.rfind(tail)
         head = fqdn_used[:idx]
         if self.verbose > 2:
-            LOG.debug(_("Basename of FQDN {f!r} is {h!r}.").format(
+            LOG.debug(_('Basename of FQDN {f!r} is {h!r}.').format(
                 f=fqdn_used, h=head))
 
         if not FQDN_REGEX.match(fqdn_used):
-            msg = _("Invalid FQDN {!r}.").format(fqdn)
+            msg = _('Invalid FQDN {!r}.').format(fqdn)
             if raise_on_error:
                 raise ValueError(msg)
             LOG.error(msg)
             return None
 
         return fqdn_used
 
     # -------------------------------------------------------------------------
     def get_rrset(self, fqdn, rrset_type, raise_on_error=True):
-
+        """Searching a record set by given name and type."""
         fqdn_used = self.verify_fqdn(fqdn, raise_on_error=raise_on_error)
         if not fqdn_used:
             return None
         rtype = self.verify_rrset_type(rrset_type, raise_on_error=raise_on_error)
         if not rtype:
             return None
 
-        LOG.debug(_("Searching for RecordSet {f!r} of type {t!r} in zone {z!r}.").format(
+        LOG.debug(_('Searching for RecordSet {f!r} of type {t!r} in zone {z!r}.').format(
             f=fqdn_used, t=rtype, z=self.name))
 
         if not len(self.rrsets):
             self.update()
 
         for rrset in self.rrsets:
             if rrset.name == fqdn_used and rrset.type == rtype:
                 if self.verbose > 2:
-                    msg = _("Found {} RecordSet:").format(rtype)
+                    msg = _('Found {} RecordSet:').format(rtype)
                     msg += '\n' + pp(rrset.as_dict(minimal=True))
                     LOG.debug(msg)
                 return rrset
 
-        LOG.debug(_("Did not found RecordSet {f!r} of type {t!r}.".format(
+        LOG.debug(_('Did not found RecordSet {f!r} of type {t!r}.'.format(
             f=fqdn_used, t=rtype)))
         return None
 
     # -------------------------------------------------------------------------
     def get_soa_rrset(self, raise_on_error=True):
-
+        """Searching for the SOA record set of current zone."""
         rrset = self.get_rrset(fqdn=self.name, rrset_type='SOA', raise_on_error=raise_on_error)
         if not rrset:
-            LOG.warning(_("Did not get SOA for zone {!r}.").format(self.name))
+            LOG.warning(_('Did not get SOA for zone {!r}.').format(self.name))
         return rrset
 
 
 # =============================================================================
 class PowerDNSZoneDict(MutableMapping):
     """
     A dictionary containing PDNS Zone objects.
+
     It works like a dict.
     i.e.:
     zones = PowerDNSZoneDict(PowerDNSZone(name='pp.com', ...))
     and
     zones['pp.com'] returns a PowerDNSZone object for zone 'pp.com'
     """
 
-    msg_invalid_zone_type = _("Invalid item type {{!r}} to set, only {} allowed.").format(
+    msg_invalid_zone_type = _('Invalid item type {{!r}} to set, only {} allowed.').format(
         'PowerDNSZone')
-    msg_key_not_name = _("The key {k!r} must be equal to the zone name {n!r}.")
-    msg_none_type_error = _("None type as key is not allowed.")
-    msg_empty_key_error = _("Empty key {!r} is not allowed.")
-    msg_no_zone_dict = _("Object {o!r} is not a {e} object.")
+    msg_key_not_name = _('The key {k!r} must be equal to the zone name {n!r}.')
+    msg_none_type_error = _('None type as key is not allowed.')
+    msg_empty_key_error = _('Empty key {!r} is not allowed.')
+    msg_no_zone_dict = _('Object {o!r} is not a {e} object.')
 
     # -------------------------------------------------------------------------
     # __init__() method required to create instance from class.
     def __init__(self, *args, **kwargs):
-        '''Use the object dict'''
-        self._map = dict()
+        """Initialize a PowerDNSZoneDict object."""
+        self._map = {}
 
         for arg in args:
             self.append(arg)
 
     # -------------------------------------------------------------------------
     def _set_item(self, key, zone):
 
@@ -1287,15 +1280,15 @@
         if zone_name != key.lower():
             raise KeyError(self.msg_key_not_name.format(k=key, n=zone_name))
 
         self._map[zone_name] = zone
 
     # -------------------------------------------------------------------------
     def append(self, zone):
-
+        """Append the given zone to the current dict."""
         if not isinstance(zone, PowerDNSZone):
             raise TypeError(self.msg_invalid_zone_type.format(zone.__class__.__name__))
         self._set_item(zone.name, zone)
 
     # -------------------------------------------------------------------------
     def _get_item(self, key):
 
@@ -1306,14 +1299,15 @@
         if zone_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map[zone_name]
 
     # -------------------------------------------------------------------------
     def get(self, key):
+        """Get a zone from current dict by its zone name as key."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def _del_item(self, key, strict=True):
 
         if key is None:
             raise TypeError(self.msg_none_type_error)
@@ -1326,130 +1320,140 @@
             return
 
         del self._map[zone_name]
 
     # -------------------------------------------------------------------------
     # The next five methods are requirements of the ABC.
     def __setitem__(self, key, value):
+        """Set a zone in current dict by its zone name as key."""
         self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def __getitem__(self, key):
+        """Get a zone from current dict by its zone name as key."""
         return self._get_item(key)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, key):
+        """Remove the zone in dict with the given zone name as key."""
         self._del_item(key)
 
     # -------------------------------------------------------------------------
     def __iter__(self):
-
+        """Iterate through all zone names in current dict."""
         for zone_name in self.keys():
             yield zone_name
 
     # -------------------------------------------------------------------------
     def __len__(self):
+        """Return the number of zones in current dict."""
         return len(self._map)
 
     # -------------------------------------------------------------------------
     # The next methods aren't required, but nice for different purposes:
     def __str__(self):
-        '''returns simple dict representation of the mapping'''
+        """Return simple dict representation of the mapping."""
         return str(self._map)
 
     # -------------------------------------------------------------------------
     def __repr__(self):
-        '''echoes class, id, & reproducible representation in the REPL'''
+        """Echoes class, id, & reproducible representation in the REPL."""
         return '{}, {}({})'.format(
             super(PowerDNSZoneDict, self).__repr__(),
             self.__class__.__name__,
             self._map)
 
     # -------------------------------------------------------------------------
     def __contains__(self, key):
+        """Return whether the given zone name is contained in current dict."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         zone_name = str(key).lower().strip()
         if zone_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return zone_name in self._map
 
     # -------------------------------------------------------------------------
     def keys(self):
-
+        """Return a sorted list of all zone names in this dict."""
         return sorted(
             self._map.keys(),
             key=lambda x: cmp_to_key(compare_fqdn)(self._map[x].name_unicode))
 
     # -------------------------------------------------------------------------
     def items(self):
-
+        """Return tuples (zone name + object as tuple) of this dict in a sorted manner."""
         item_list = []
 
         for zone_name in self.keys():
             item_list.append((zone_name, self._map[zone_name]))
 
         return item_list
 
     # -------------------------------------------------------------------------
     def values(self):
-
+        """Return all zone objects in this dict."""
         value_list = []
         for zone_name in self.keys():
             value_list.append(self._map[zone_name])
         return value_list
 
     # -------------------------------------------------------------------------
     def __eq__(self, other):
-
+        """Magic method for using it as the '=='-operator."""
         if not isinstance(other, PowerDNSZoneDict):
             raise TypeError(self.msg_no_zone_dict.format(o=other, e='PowerDNSZoneDict'))
 
         return self._map == other._map
 
     # -------------------------------------------------------------------------
     def __ne__(self, other):
-
+        """Magic method for using it as the '!='-operator."""
         if not isinstance(other, PowerDNSZoneDict):
             raise TypeError(self.msg_no_zone_dict.format(o=other, e='PowerDNSZoneDict'))
 
         return self._map != other._map
 
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
-
+        """Get and return the zone by its name and remove it in dict."""
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         zone_name = str(key).lower().strip()
         if zone_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
         return self._map.pop(zone_name, *args)
 
     # -------------------------------------------------------------------------
     def popitem(self):
-
+        """Remove and return a arbitrary (zone name and object) pair from the dictionary."""
         if not len(self._map):
             return None
 
         zone_name = self.keys()[0]
         zone = self._map[zone_name]
         del self._map[zone_name]
         return (zone_name, zone)
 
     # -------------------------------------------------------------------------
     def clear(self):
-        self._map = dict()
+        """Remove all items from the dictionary."""
+        self._map = {}
 
     # -------------------------------------------------------------------------
     def setdefault(self, key, default):
+        """
+        Return the zone, if the key is in dict.
 
+        If not, insert key with a value of default and return default.
+        """
         if key is None:
             raise TypeError(self.msg_none_type_error)
 
         zone_name = str(key).lower().strip()
         if zone_name == '':
             raise ValueError(self.msg_empty_key_error.format(key))
 
@@ -1460,44 +1464,44 @@
             return self._map[zone_name]
 
         self._set_item(zone_name, default)
         return default
 
     # -------------------------------------------------------------------------
     def update(self, other):
-
+        """Update the dict with the key/value pairs from other, overwriting existing keys."""
         if isinstance(other, PowerDNSZoneDict) or isinstance(other, dict):
             for zone_name in other.keys():
                 self._set_item(zone_name, other[zone_name])
             return
 
         for tokens in other:
             key = tokens[0]
             value = tokens[1]
             self._set_item(key, value)
 
     # -------------------------------------------------------------------------
     def as_dict(self, short=True):
-
+        """Transform the elements of the object into a dict."""
         res = {}
         for zone_name in self._map:
             res[zone_name] = self._map[zone_name].as_dict(short)
         return res
 
     # -------------------------------------------------------------------------
     def as_list(self, short=True):
-
+        """Return a list with all zones transformed to a dict."""
         res = []
         for zone_name in self.keys():
             res.append(self._map[zone_name].as_dict(short))
         return res
 
 
 # =============================================================================
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 list
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/PKG-INFO` & `fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-pdnstools
-Version: 0.5.6
+Version: 0.6.0
 Summary: Modules for handling the PowerDNS API
 Home-page: https://github.com/fbrehm/fb-pdnstools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fb_pdnstools-0.5.6/lib/fb_pdnstools.egg-info/SOURCES.txt` & `fb_pdnstools-0.6.0/lib/fb_pdnstools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 bin/pdns-bulk-remove
 lib/fb_pdnstools/__init__.py
+lib/fb_pdnstools/base_handler.py
 lib/fb_pdnstools/bulk_rm_app.py
 lib/fb_pdnstools/bulk_rm_cfg.py
+lib/fb_pdnstools/common.py
 lib/fb_pdnstools/errors.py
 lib/fb_pdnstools/local_version.py
 lib/fb_pdnstools/record.py
 lib/fb_pdnstools/server.py
 lib/fb_pdnstools/xlate.py
 lib/fb_pdnstools/zone.py
 lib/fb_pdnstools.egg-info/PKG-INFO
@@ -20,13 +22,15 @@
 lib/fb_pdnstools.egg-info/top_level.txt
 test/general.py
 test/rrset-a-with-comment.js
 test/rrset-a.js
 test/rrset-mx.js
 test/rrset-soa.js
 test/test_00_fb_pdnstools.py
-test/test_10_record.py
-test/test_20_zone.py
-test/test_30_server.py
+test/test_05_common.py
+test/test_10_base_handler.py
+test/test_20_record.py
+test/test_30_zone.py
+test/test_40_server.py
 test/zone-rev.js
 test/zone.js
 test/zones.js
```

### Comparing `fb_pdnstools-0.5.6/setup.cfg` & `fb_pdnstools-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
 
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
-ignore = E226,E302,E41,E402
+ignore = E226,E302,E41,E402,D401
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fb_pdnstools-0.5.6/setup.py` & `fb_pdnstools-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
 """
+@summary: Modules for handling the PowerDNS API.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
 @license: LGPL3+
-@copyright: © 2018 Frank Brehm, Berlin
-@summary: Modules for handling the PowerDNS API
+@copyright: © 2023 Frank Brehm, Berlin
 """
 from __future__ import print_function
 
-import os
-import sys
-import re
-import pprint
 import datetime
-import textwrap
 import glob
+import os
 import pathlib
+import pprint
+import re
 import subprocess
-
-# Third party modules
-from setuptools import setup
+import sys
+import textwrap
 
 # own modules:
 __base_dir__ = os.path.abspath(os.path.dirname(__file__))
 __bin_dir__ = os.path.join(__base_dir__, 'bin')
 __lib_dir__ = os.path.join(__base_dir__, 'lib')
 __module_dir__ = os.path.join(__lib_dir__, 'fb_pdnstools')
 __init_py__ = os.path.join(__module_dir__, '__init__.py')
@@ -36,76 +33,82 @@
     '__lib_dir__': __lib_dir__,
     '__module_dir__': __module_dir__,
     '__init_py__': __init_py__,
 }
 
 # -----------------------------------
 def pp(obj):
+    """Human friendly output of data structures."""
     pprinter = pprint.PrettyPrinter(indent=4)
     return pprinter.pformat(obj)
 
 # print("Paths:\n{}".format(pp(PATHS)))
 
 
 if os.path.exists(__module_dir__) and os.path.isfile(__init_py__):
     sys.path.insert(0, os.path.abspath(__lib_dir__))
 
+# Third party modules
 import fb_tools
 
+from setuptools import setup
+
 # from fb_tools.common import pp
 
-ENCODING = "utf-8"
+ENCODING = 'utf-8'
 
 __packet_version__ = fb_tools.__version__
 
 __packet_name__ = 'fb_pdnstools'
 __debian_pkg_name__ = 'fb-pdnstools'
 
 __author__ = 'Frank Brehm'
 __contact__ = 'frank@brehm-online.com'
-__copyright__ = '(C) 2018 Frank Brehm, Berlin'
+__copyright__ = '(C) 2023 Frank Brehm, Berlin'
 __license__ = 'LGPL3+'
 __url__ = 'https://github.com/fbrehm/fb-pdnstools'
 
 
 __open_args__ = {}
 if sys.version_info[0] < 3:
     __open_args__ = {'encoding': ENCODING, 'errors': 'surrogateescape'}
 
 # -----------------------------------
 def read(fname):
-
+    """Read the given file and return its content."""
     content = None
 
     if sys.version_info[0] < 3:
         with open(fname, 'r') as fh:
             content = fh.read()
     else:
         with open(fname, 'r', **__open_args__) as fh:
             content = fh.read()
 
     return content
 
 
 # -----------------------------------
 def is_python_file(filename):
+    """Return, whether the given file seems to be a Python source file."""
     if filename.endswith('.py'):
         return True
     else:
         return False
 
 
 # -----------------------------------
 __debian_dir__ = os.path.join(__base_dir__, 'debian')
 __changelog_file__ = os.path.join(__debian_dir__, 'changelog')
 __readme_file__ = os.path.join(__base_dir__, 'README.txt')
 
 
 # -----------------------------------
 def get_debian_version():
+    """Return the latest package version fron Debian changelog file."""
     if not os.path.isfile(__changelog_file__):
         return None
     changelog = read(__changelog_file__)
     first_row = changelog.splitlines()[0].strip()
     if not first_row:
         return None
     pattern = r'^' + re.escape(__debian_pkg_name__) + r'\s+\(([^\)]+)\)'
@@ -118,24 +121,25 @@
 __debian_version__ = get_debian_version()
 
 if __debian_version__ is not None and __debian_version__ != '':
     __packet_version__ = __debian_version__
 
 # -----------------------------------
 def write_local_version():
-
+    """Write the local version file."""
     local_version_file = os.path.join(__module_dir__, 'local_version.py')
     local_version_file_content = textwrap.dedent('''\
         #!/usr/bin/python
         # -*- coding: utf-8 -*-
         """
+        @summary: Modules for handling the PowerDNS API.
+
         @author: {author}
         @contact: {contact}
         @copyright: © {cur_year} by {author}, Berlin
-        @summary: Modules for handling the PowerDNS API.
         """
 
         __author__ = '{author} <{contact}>'
         __copyright__ = '(C) {cur_year} by {author}, Berlin'
         __contact__ = {contact!r}
         __version__ = {version!r}
         __license__ = {license!r}
@@ -165,15 +169,15 @@
     'argparse',
     'fb_tools',
     'six'
 ]
 
 # -----------------------------------
 def read_requirements():
-
+    """Read the requiremments.txt file."""
     req_file = os.path.join(__base_dir__, 'requirements.txt')
     if not os.path.isfile(req_file):
         return
 
     f_content = read(req_file)
     if not f_content:
         return
@@ -198,15 +202,15 @@
 
 read_requirements()
 
 # -----------------------------------
 __scripts__ = []
 
 def get_scripts():
-
+    """Collect binary script files from bin/."""
     fpattern = os.path.join(__bin_dir__, '*')
     for fname in glob.glob(fpattern):
         script_name = os.path.relpath(fname, __base_dir__)
         if not os.path.isfile(fname):
             continue
         if not os.access(fname, os.X_OK):
             continue
@@ -220,14 +224,15 @@
 get_scripts()
 
 # -----------------------------------
 MO_FILES = 'locale/*/LC_MESSAGES/*.mo'
 PO_FILES = 'locale/*/LC_MESSAGES/*.po'
 
 def create_mo_files():
+    """Compile the translation files."""
     mo_files = []
     for po_path in glob.glob(PO_FILES):
         mo = pathlib.Path(po_path.replace('.po', '.mo'))
         if not mo.exists():
             subprocess.call(['msgfmt', '-o', str(mo), po_path])
         mo_files.append(str(mo))
```

### Comparing `fb_pdnstools-0.5.6/test/general.py` & `fb_pdnstools-0.6.0/test/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
+@summary: general used functions an objects used for unit tests on the pdnstools python modules.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: GPL3
-@summary: general used functions an objects used for unit tests on
-          the pdnstools python modules
 """
 
-import os
-import sys
-import logging
 import argparse
 import json
-
+import logging
+import os
+import sys
 from pathlib import Path
-
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
+# Third party modules
+from fb_logging.colored import ColoredFormatter
+
 import six
 
 # Own modules
-from fb_logging.colored import ColoredFormatter
 
 # =============================================================================
 
 LOG = logging.getLogger(__name__)
 
 
 # =============================================================================
 def get_arg_verbose():
-
+    """Get the verbose level from command line attributes."""
     arg_parser = argparse.ArgumentParser()
 
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument(
-        "-v", "--verbose", action="count",
+        '-v', '--verbose', action='count',
         dest='verbose', help='Increase the verbosity level')
     args = arg_parser.parse_args()
 
     return args.verbose
 
 
 # =============================================================================
 def init_root_logger(verbose=0):
+    """
+    Initialize the root logger object.
 
+    It creates a colored loghandler with all output to STDERR.
+    """
     root_log = logging.getLogger()
     root_log.setLevel(logging.WARNING)
     if verbose:
         root_log.setLevel(logging.INFO)
         if verbose > 1:
             root_log.setLevel(logging.DEBUG)
 
@@ -76,18 +80,19 @@
     lh_console.setFormatter(formatter)
 
     root_log.addHandler(lh_console)
 
 
 # =============================================================================
 class FbPdnsToolsTestcase(unittest.TestCase):
+    """A base testcase class for all test scripts."""
 
     # -------------------------------------------------------------------------
     def __init__(self, methodName='runTest', verbose=0):
-
+        """Initialize a FbPdnsToolsTestcase object."""
         self._verbose = int(verbose)
 
         appname = os.path.basename(sys.argv[0]).replace('.py', '')
         self._appname = appname
 
         super(FbPdnsToolsTestcase, self).__init__(methodName)
 
@@ -108,21 +113,21 @@
             self.open_args['encoding'] = 'utf-8'
             self.open_args['errors'] = 'surrogateescape'
 
         self.server_version = '4.1.10-mocked'
 
         self.server_list_data = [
             {
-                "config_url": "/api/v1/servers/localhost/config{/config_setting}",
-                "daemon_type": "authoritative",
-                "id": "localhost",
-                "type": "Server",
-                "url": "/api/v1/servers/localhost",
-                "version": "{}".format(self.server_version),
-                "zones_url": "/api/v1/servers/localhost/zones{/zone}"
+                'config_url': '/api/v1/servers/localhost/config{/config_setting}',
+                'daemon_type': 'authoritative',
+                'id': 'localhost',
+                'type': 'Server',
+                'url': '/api/v1/servers/localhost',
+                'version': '{}'.format(self.server_version),
+                'zones_url': '/api/v1/servers/localhost/zones{/zone}'
             }
         ]
 
     # -------------------------------------------------------------------------
     @property
     def verbose(self):
         """The verbosity level."""
@@ -132,86 +137,88 @@
     @property
     def appname(self):
         """The name of the current running application."""
         return self._appname
 
     # -------------------------------------------------------------------------
     def setUp(self):
+        """Overridable hook for setup actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def tearDown(self):
+        """Overridable hook for finishing actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def get_js_a_rrset(self):
-
+        """Return data of an A-record from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.a_rrset_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.a_rrset_file)))
         with self.a_rrset_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_a_rrset_comment(self):
-
+        """Return comment data of an A-record from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.a_rrset_file_comment)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.a_rrset_file_comment)))
         with self.a_rrset_file_comment.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_mx_rrset(self):
-
+        """Return data of a MX-record from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.mx_rrset_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.mx_rrset_file)))
         with self.mx_rrset_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_soa_rrset(self):
-
+        """Return data of a SOA-record from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.soa_rrset_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.soa_rrset_file)))
         with self.soa_rrset_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_zone(self):
-
+        """Return data of a complete forward zone from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.zone_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.zone_file)))
         with self.zone_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_zone_rev(self):
-
+        """Return data of a complete reverse zone from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.zone_rev_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.zone_rev_file)))
         with self.zone_rev_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_zones(self):
-
+        """Return a list of zones without record sets from a test json file."""
         ret = None
-        LOG.debug("Loading file {!r} ...".format(str(self.zones_file)))
+        LOG.debug('Loading file {!r} ...'.format(str(self.zones_file)))
         with self.zones_file.open('r', **self.open_args) as fh:
             ret = json.load(fh)
         return ret
 
     # -------------------------------------------------------------------------
     def get_js_serverlist(self, index=None):
-
+        """Return a list with API server data from a test json file."""
         import json
 
         if index is None:
             data = self.server_list_data
         else:
             data = self.server_list_data[index]
```

### Comparing `fb_pdnstools-0.5.6/test/test_00_fb_pdnstools.py` & `fb_pdnstools-0.6.0/test/test_00_fb_pdnstools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,176 +1,160 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-'''
+"""
+@summary: Test script (and module) for unit tests on fb-pdnstools base classes.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: LGPL3
-@summary: test script (and module) for unit tests on fb-pdnstools base classes
-'''
+"""
 
-import os
-import sys
 import logging
 import logging.handlers
-
+import os
+import sys
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 libdir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'lib'))
 sys.path.insert(0, libdir)
 
-from fb_tools.common import pp
+# Third party modules
+# from fb_tools.common import pp
 
+# Own modules
 from general import FbPdnsToolsTestcase, get_arg_verbose, init_root_logger
 
 LOG = logging.getLogger('test_fb_pdnstools')
 
 
 # =============================================================================
 class TestPdnsToolsBase(FbPdnsToolsTestcase):
+    """Testcase for tests on fb_pdnstools/__init__.py and fb_pdnstools.errors."""
 
     # -------------------------------------------------------------------------
     def test_import_modules(self):
+        """Testing import of modules fb_pdnstools/__init__.py and fb_pdnstools.errors ..."""
+        LOG.info('Test importing main module ...')
 
-        LOG.info("Test importing main module ...")
-
-        LOG.debug("Importing fb_pdnstools ...")
+        LOG.debug('Importing fb_pdnstools ...')
         import fb_pdnstools
 
-        LOG.debug("Version of fb_pdnstools: {!r}.".format(fb_pdnstools.__version__))
+        LOG.debug('Version of fb_pdnstools: {!r}.'.format(fb_pdnstools.__version__))
 
-        LOG.debug("Importing fb_pdnstools.errors ...")
+        LOG.debug('Importing fb_pdnstools.errors ...')
         import fb_pdnstools.errors
-        LOG.debug("Version of fb_pdnstools.errors: {!r}.".format(
+        LOG.debug('Version of fb_pdnstools.errors: {!r}.'.format(
             fb_pdnstools.errors.__version__))
 
     # -------------------------------------------------------------------------
-    def test_base_class(self):
-
-        LOG.info("Testing base class BasePowerDNSHandler ...")
-
-        from fb_pdnstools import BasePowerDNSHandler
-
-        LOG.debug("Creating dummy PDNS handler on base of BasePowerDNSHandler ...")
-
-        # Creating dummy class
-        class DummyPowerDNSHandler(BasePowerDNSHandler):
-            pass
-
-        test_handler = DummyPowerDNSHandler(
-            appname=self.appname, verbose=self.verbose)
-
-        LOG.debug("Dummy PDNS handler:\n{}".format(pp(test_handler.as_dict())))
-
-    # -------------------------------------------------------------------------
     def test_error_classes(self):
+        """Test instantiating of different exception classes in fb_pdnstools.errors."""
+        LOG.info('Testing loading and function of different error handler classes ...')
 
-        LOG.info("Testing loading and function of different error handler classes ...")
-
-        LOG.debug("Testing PowerDNSHandlerError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PowerDNSHandlerError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PowerDNSHandlerError
         with self.assertRaises(PowerDNSHandlerError) as cm:
             raise PowerDNSHandlerError('bla')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PowerDNSZoneError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PowerDNSZoneError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PowerDNSZoneError
         with self.assertRaises(PowerDNSZoneError) as cm:
             raise PowerDNSZoneError('bla')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PowerDNSRecordError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PowerDNSRecordError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PowerDNSRecordError
         with self.assertRaises(PowerDNSRecordError) as cm:
             raise PowerDNSRecordError('bla')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PowerDNSRecordSetError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PowerDNSRecordSetError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PowerDNSRecordSetError
         with self.assertRaises(PowerDNSRecordSetError) as cm:
             raise PowerDNSRecordSetError('bla')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PowerDNSWrongSoaDataError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PowerDNSWrongSoaDataError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PowerDNSWrongSoaDataError
         with self.assertRaises(PowerDNSWrongSoaDataError) as cm:
             raise PowerDNSWrongSoaDataError({'uhu': 'banane'})
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        msg = "Undfined test error"
+        msg = 'Undfined test error'
 
-        LOG.debug("Testing PDNSApiError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiError
         uris = (None, 'https://pdnsmaster.uhu-banane.eu')
         code = 404
         for uri in uris:
             with self.assertRaises(PDNSApiError) as cm:
                 raise PDNSApiError(code, msg, uri)
             e = cm.exception
-            LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+            LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PDNSApiNotAuthorizedError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiNotAuthorizedError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiNotAuthorizedError
         with self.assertRaises(PDNSApiNotAuthorizedError) as cm:
             raise PDNSApiNotAuthorizedError(401, msg)
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PDNSApiNotFoundError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiNotFoundError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiNotFoundError
         with self.assertRaises(PDNSApiNotFoundError) as cm:
             raise PDNSApiNotFoundError(404, msg)
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PDNSApiValidationError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiValidationError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiValidationError
         with self.assertRaises(PDNSApiValidationError) as cm:
             raise PDNSApiValidationError(422, msg, 'https://pdnsmaster.uhu-banane.eu')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PDNSApiRateLimitExceededError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiRateLimitExceededError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiRateLimitExceededError
         with self.assertRaises(PDNSApiRateLimitExceededError) as cm:
             raise PDNSApiRateLimitExceededError(429, msg)
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
-        LOG.debug("Testing PDNSApiRequestError from fb_pdnstools.errors ...")
+        LOG.debug('Testing PDNSApiRequestError from fb_pdnstools.errors ...')
         from fb_pdnstools.errors import PDNSApiRequestError
         with self.assertRaises(PDNSApiRequestError) as cm:
             raise PDNSApiRequestError(419, 'I am not a tea pot.')
         e = cm.exception
-        LOG.debug("Got a {c}: {e}".format(c=e.__class__.__name__, e=e))
+        LOG.debug('Got a {c}: {e}'.format(c=e.__class__.__name__, e=e))
 
 
 # =============================================================================
 if __name__ == '__main__':
 
     verbose = get_arg_verbose()
     if verbose is None:
         verbose = 0
     init_root_logger(verbose)
 
-    LOG.info("Starting tests ...")
+    LOG.info('Starting tests ...')
 
     loader = unittest.TestLoader()
     suite = unittest.TestSuite()
 
     suite.addTest(TestPdnsToolsBase('test_import_modules', verbose))
-    suite.addTest(TestPdnsToolsBase('test_base_class', verbose))
     suite.addTest(TestPdnsToolsBase('test_error_classes', verbose))
 
     runner = unittest.TextTestRunner(verbosity=verbose)
 
     result = runner.run(suite)
```

### Comparing `fb_pdnstools-0.5.6/test/test_10_record.py` & `fb_pdnstools-0.6.0/test/test_20_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,121 +1,126 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-'''
+"""
+@summary: Test script (and module) for unit tests record classes.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: LGPL3
-@summary: test script (and module) for unit tests record classes
-'''
+"""
 
-import os
-import sys
+import datetime
 import logging
 import logging.handlers
-import datetime
-
+import os
+import sys
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 libdir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'lib'))
 sys.path.insert(0, libdir)
 
+# Third party modules
 from fb_tools.common import pp
 
+# Own modules
 from general import FbPdnsToolsTestcase, get_arg_verbose, init_root_logger
 
 LOG = logging.getLogger('test_record')
 
 
 # =============================================================================
 class TestPdnsRecord(FbPdnsToolsTestcase):
+    """Testcase for tests on fb_pdnstools.record."""
 
     # -------------------------------------------------------------------------
     def setUp(self):
+        """Hook for setup actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def tearDown(self):
+        """Hook for finishing actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def test_import_modules(self):
-
+        """Testing import of module fb_pdnstools.record ..."""
         if self.verbose:
             print()
-        LOG.info("Test importing record module ...")
+        LOG.info('Test importing record module ...')
 
-        LOG.debug("Importing fb_pdnstools.record ...")
+        LOG.debug('Importing fb_pdnstools.record ...')
         import fb_pdnstools.record
 
-        LOG.debug("Version of fb_pdnstools.record: {!r}.".format(fb_pdnstools.record.__version__))
+        LOG.debug('Version of fb_pdnstools.record: {!r}.'.format(fb_pdnstools.record.__version__))
 
-        LOG.info("Testing import of PowerDNSRecord from fb_pdnstools.record ...")
+        LOG.info('Testing import of PowerDNSRecord from fb_pdnstools.record ...')
         from fb_pdnstools.record import PowerDNSRecord
 
         record = PowerDNSRecord(appname=self.appname, verbose=self.verbose)
-        LOG.debug("Empty PowerDNSRecord:\n{}".format(record))
+        LOG.debug('Empty PowerDNSRecord:\n{}'.format(record))
 
     # -------------------------------------------------------------------------
     def test_pdns_record(self):
-
+        """Test instantiating of class PowerDNSRecord with different parameters."""
         if self.verbose:
             print()
-        LOG.info("Testing class PowerDNSRecord ...")
+        LOG.info('Testing class PowerDNSRecord ...')
 
-        test_content = "www.testing.com."
+        test_content = 'www.testing.com.'
 
         from fb_pdnstools.record import PowerDNSRecord
 
-        LOG.debug("Creating an empty record.")
+        LOG.debug('Creating an empty record.')
         record = PowerDNSRecord(
             appname=self.appname, verbose=self.verbose)
-        LOG.debug("Record: %%r: {!r}".format(record))
+        LOG.debug('Record: %%r: {!r}'.format(record))
         if self.verbose > 1:
-            LOG.debug("Record: %%s: {}".format(record))
-            LOG.debug("record.as_dict():\n{}".format(pp(record.as_dict())))
+            LOG.debug('Record: %%s: {}'.format(record))
+            LOG.debug('record.as_dict():\n{}'.format(pp(record.as_dict())))
         self.assertIsNone(record.content)
         self.assertIsInstance(record.disabled, bool)
         self.assertFalse(record.disabled)
 
-        LOG.debug("Creating an enabled record.")
+        LOG.debug('Creating an enabled record.')
         record = PowerDNSRecord(
             appname=self.appname, verbose=self.verbose, content=test_content)
-        LOG.debug("Record: %%r: {!r}".format(record))
+        LOG.debug('Record: %%r: {!r}'.format(record))
         if self.verbose > 1:
-            LOG.debug("Record: %%s: {}".format(record))
-            LOG.debug("record.as_dict():\n{}".format(pp(record.as_dict())))
+            LOG.debug('Record: %%s: {}'.format(record))
+            LOG.debug('record.as_dict():\n{}'.format(pp(record.as_dict())))
         self.assertEqual(record.content, test_content)
         self.assertIsInstance(record.disabled, bool)
         self.assertFalse(record.disabled)
 
-        LOG.debug("Creating a disabled record.")
+        LOG.debug('Creating a disabled record.')
         record = PowerDNSRecord(
             appname=self.appname, verbose=self.verbose, content=test_content, disabled=True)
-        LOG.debug("Record: %%r: {!r}".format(record))
-        LOG.debug("Record: %%s: {}".format(record))
+        LOG.debug('Record: %%r: {!r}'.format(record))
+        LOG.debug('Record: %%s: {}'.format(record))
         if self.verbose > 1:
-            LOG.debug("record.as_dict():\n{}".format(pp(record.as_dict())))
+            LOG.debug('record.as_dict():\n{}'.format(pp(record.as_dict())))
         self.assertEqual(record.content, test_content)
         self.assertIsInstance(record.disabled, bool)
         self.assertTrue(record.disabled)
 
     # -------------------------------------------------------------------------
     def test_pdns_record_equality(self):
-
+        """Testing equal operator of class PowerDNSRecord."""
         if self.verbose:
             print()
-        LOG.info("Testing equal operator of class PowerDNSRecord ...")
+        LOG.info('Testing equal operator of class PowerDNSRecord ...')
 
-        test_content = "www.testing.com."
-        test_content2 = "www.uhu-banane.com."
-        test_content3 = "www.Testing.com."
+        test_content = 'www.testing.com.'
+        test_content2 = 'www.uhu-banane.com.'
+        test_content3 = 'www.Testing.com.'
 
         from fb_pdnstools.record import PowerDNSRecord
 
         test_matrix = (
             (None, None, True),
             (test_content, None, False),
             (None, test_content, False),
@@ -124,53 +129,53 @@
             (test_content, test_content3, True),
         )
         for test_set in test_matrix:
             rec1 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[0])
             rec2 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[1])
             expected = test_set[2]
             LOG.debug(
-                "Comparing equality of record {r1!r} and record {r2!r}, expected: {ex}.".format(
+                'Comparing equality of record {r1!r} and record {r2!r}, expected: {ex}.'.format(
                     r1=rec1.content, r2=rec2.content, ex=expected))
             if rec1 == rec2:
                 result = True
             else:
                 result = False
-            LOG.debug("Result: {}".format(result))
+            LOG.debug('Result: {}'.format(result))
             if expected:
                 self.assertTrue(result)
             else:
                 self.assertFalse(result)
 
     # -------------------------------------------------------------------------
     def test_pdns_record_gt(self):
-
+        """Testing the greater than operator of class PowerDNSRecord."""
         if self.verbose:
             print()
-        LOG.info("Testing the greater than operator of class PowerDNSRecord ...")
+        LOG.info('Testing the greater than operator of class PowerDNSRecord ...')
 
-        test_content = "www.1testing.com."
-        test_content2 = "www.2uhu-banane.com."
-        test_content3 = "www.1Testing.com."
+        test_content = 'www.1testing.com.'
+        test_content2 = 'www.2uhu-banane.com.'
+        test_content3 = 'www.1Testing.com.'
 
         from fb_pdnstools.record import PowerDNSRecord
 
-        LOG.debug("Testing the greater than operator with wrong argument ...")
+        LOG.debug('Testing the greater than operator with wrong argument ...')
         record = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_content)
         test_matrix = (
             (record, 'uhu'),
             (88, record)
         )
         for test_set in test_matrix:
             with self.assertRaises(TypeError) as cm:
-                LOG.debug("Comparing {r1!r} with {r2!r} ...".format(
+                LOG.debug('Comparing {r1!r} with {r2!r} ...'.format(
                     r1=test_set[0], r2=test_set[1]))
                 if test_set[0] > test_set[1]:
-                    print("This should not be visible!")
+                    print('This should not be visible!')
             e = cm.exception
-            LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+            LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
         test_matrix = (
             (None, None, False),
             (test_content, None, True),
             (None, test_content, False),
             (test_content, test_content, False),
             (test_content, test_content2, False),
@@ -179,53 +184,53 @@
         )
 
         for test_set in test_matrix:
             rec1 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[0])
             rec2 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[1])
             expected = test_set[2]
             LOG.debug(
-                "Comparing record {r1!r} > record {r2!r}, expected: {ex}.".format(
+                'Comparing record {r1!r} > record {r2!r}, expected: {ex}.'.format(
                     r1=rec1.content, r2=rec2.content, ex=expected))
             if rec1 > rec2:
                 result = True
             else:
                 result = False
-            LOG.debug("Result: {}".format(result))
+            LOG.debug('Result: {}'.format(result))
             if expected:
                 self.assertTrue(result)
             else:
                 self.assertFalse(result)
 
     # -------------------------------------------------------------------------
     def test_pdns_record_lt(self):
-
+        """Testing the less than operator of class PowerDNSRecord."""
         if self.verbose:
             print()
-        LOG.info("Testing the less than operator of class PowerDNSRecord ...")
+        LOG.info('Testing the less than operator of class PowerDNSRecord ...')
 
-        test_content = "www.1testing.com."
-        test_content2 = "www.2uhu-banane.com."
-        test_content3 = "www.1Testing.com."
+        test_content = 'www.1testing.com.'
+        test_content2 = 'www.2uhu-banane.com.'
+        test_content3 = 'www.1Testing.com.'
 
         from fb_pdnstools.record import PowerDNSRecord
 
-        LOG.debug("Testing the less than operator with wrong argument ...")
+        LOG.debug('Testing the less than operator with wrong argument ...')
         record = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_content)
         test_matrix = (
             (record, 'uhu'),
             (88, record)
         )
         for test_set in test_matrix:
             with self.assertRaises(TypeError) as cm:
-                LOG.debug("Comparing {r1!r} with {r2!r} ...".format(
+                LOG.debug('Comparing {r1!r} with {r2!r} ...'.format(
                     r1=test_set[0], r2=test_set[1]))
                 if test_set[0] < test_set[1]:
-                    print("This should not be visible!")
+                    print('This should not be visible!')
             e = cm.exception
-            LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+            LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
         test_matrix = (
             (None, None, False),
             (test_content, None, False),
             (None, test_content, True),
             (test_content, test_content, False),
             (test_content, test_content2, True),
@@ -234,151 +239,151 @@
         )
 
         for test_set in test_matrix:
             rec1 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[0])
             rec2 = PowerDNSRecord(appname=self.appname, verbose=self.verbose, content=test_set[1])
             expected = test_set[2]
             LOG.debug(
-                "Comparing record {r1!r} < record {r2!r}, expected: {ex}.".format(
+                'Comparing record {r1!r} < record {r2!r}, expected: {ex}.'.format(
                     r1=rec1.content, r2=rec2.content, ex=expected))
             if rec1 < rec2:
                 result = True
             else:
                 result = False
-            LOG.debug("Result: {}".format(result))
+            LOG.debug('Result: {}'.format(result))
             if expected:
                 self.assertTrue(result)
             else:
                 self.assertFalse(result)
 
     # -------------------------------------------------------------------------
     def test_pdns_recordset_comment(self):
-
+        """Test instantiating of class PowerDNSRecordSetComment."""
         if self.verbose:
             print()
-        LOG.info("Testing class PowerDNSRecordSetComment ...")
+        LOG.info('Testing class PowerDNSRecordSetComment ...')
 
         test_account = 'tester'
-        test_content = "Test comment"
+        test_content = 'Test comment'
         test_modified_at = 1000 * 24 * 60 * 60
 
         from fb_pdnstools.record import PowerDNSRecordSetComment
 
-        LOG.debug("Creating an empty, invalid comment.")
+        LOG.debug('Creating an empty, invalid comment.')
         empty_comment = PowerDNSRecordSetComment(
             appname=self.appname, verbose=self.verbose)
-        LOG.debug("Empty comment: %%r: {!r}".format(empty_comment))
-        LOG.debug("Empty comment: %%s: {}".format(empty_comment))
+        LOG.debug('Empty comment: %%r: {!r}'.format(empty_comment))
+        LOG.debug('Empty comment: %%s: {}'.format(empty_comment))
         if self.verbose > 1:
-            LOG.debug("Empty comment.as_dict():\n{}".format(pp(empty_comment.as_dict())))
-        LOG.debug("Empty comment.as_dict(minimal=True): {}".format(
+            LOG.debug('Empty comment.as_dict():\n{}'.format(pp(empty_comment.as_dict())))
+        LOG.debug('Empty comment.as_dict(minimal=True): {}'.format(
             pp(empty_comment.as_dict(minimal=True))))
         self.assertIsNone(empty_comment.account)
         self.assertEqual(empty_comment.content, '')
         self.assertIsInstance(empty_comment.modified_at, int)
         self.assertGreaterEqual(empty_comment.modified_at, 0)
         self.assertIsInstance(empty_comment.modified_date, datetime.datetime)
         self.assertFalse(empty_comment.valid)
         del empty_comment
 
-        LOG.debug("Creating an non empty, valid comment.")
+        LOG.debug('Creating an non empty, valid comment.')
         comment = PowerDNSRecordSetComment(
             appname=self.appname, verbose=self.verbose, account=test_account, content=test_content)
-        LOG.debug("Comment: %%r: {!r}".format(comment))
-        LOG.debug("Comment: %%s: {}".format(comment))
+        LOG.debug('Comment: %%r: {!r}'.format(comment))
+        LOG.debug('Comment: %%s: {}'.format(comment))
         if self.verbose > 1:
-            LOG.debug("Comment.as_dict():\n{}".format(pp(comment.as_dict())))
-        LOG.debug("Comment.as_dict(minimal=True): {}".format(
+            LOG.debug('Comment.as_dict():\n{}'.format(pp(comment.as_dict())))
+        LOG.debug('Comment.as_dict(minimal=True): {}'.format(
             pp(comment.as_dict(minimal=True))))
         self.assertEqual(comment.account, test_account)
         self.assertEqual(comment.content, test_content)
         self.assertIsInstance(comment.modified_at, int)
         self.assertGreaterEqual(comment.modified_at, 0)
         self.assertIsInstance(comment.modified_date, datetime.datetime)
         self.assertTrue(comment.valid)
 
-        LOG.debug("Creating a comment with a defined modified_at property.")
+        LOG.debug('Creating a comment with a defined modified_at property.')
         comment = PowerDNSRecordSetComment(
             appname=self.appname, verbose=self.verbose,
             account=test_account, content=test_content, modified_at=test_modified_at)
-        LOG.debug("Comment: %%s: {}".format(comment))
+        LOG.debug('Comment: %%s: {}'.format(comment))
         if self.verbose > 1:
-            LOG.debug("Comment: %%r: {!r}".format(comment))
+            LOG.debug('Comment: %%r: {!r}'.format(comment))
         if self.verbose > 2:
-            LOG.debug("Ccomment.as_dict():\n{}".format(pp(comment.as_dict())))
+            LOG.debug('Comment.as_dict():\n{}'.format(pp(comment.as_dict())))
         self.assertIsInstance(comment.modified_at, int)
         self.assertEqual(comment.modified_at, test_modified_at)
         self.assertIsInstance(comment.modified_date, datetime.datetime)
 
-        LOG.debug("Testing raising errors on wrong (String) modified_at property.")
+        LOG.debug('Testing raising errors on wrong (String) modified_at property.')
         with self.assertRaises(ValueError) as cm:
             comment = PowerDNSRecordSetComment(
                 appname=self.appname, verbose=self.verbose,
                 account=test_account, content=test_content, modified_at='bla')
         e = cm.exception
-        LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+        LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
-        LOG.debug("Testing raising errors on wrong (negative) modified_at property.")
+        LOG.debug('Testing raising errors on wrong (negative) modified_at property.')
         with self.assertRaises(ValueError) as cm:
             comment = PowerDNSRecordSetComment(
                 appname=self.appname, verbose=self.verbose,
                 account=test_account, content=test_content, modified_at=-100)
         e = cm.exception
-        LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+        LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
     # -------------------------------------------------------------------------
     def test_pdns_recordset_simple(self):
-
+        """Test instantiating of a simple PowerDNSRecordSet object."""
         if self.verbose:
             print()
-        LOG.info("Testing class PowerDNSRecordSet ...")
+        LOG.info('Testing class PowerDNSRecordSet ...')
 
         from fb_pdnstools.record import PowerDNSRecordSet
 
         js_rrset = self.get_js_a_rrset()
 
         rrset = PowerDNSRecordSet.init_from_dict(
             js_rrset, appname=self.appname, verbose=self.verbose)
-        LOG.debug("RecordSet: %%r: {!r}".format(rrset))
+        LOG.debug('RecordSet: %%r: {!r}'.format(rrset))
         if self.verbose > 1:
-            LOG.debug("RecordSet: %%s: {}".format(rrset))
-            LOG.debug("rrset.as_dict():\n{}".format(pp(rrset.as_dict())))
-        LOG.debug("RecordSet.as_dict(minimal=True): {}".format(
+            LOG.debug('RecordSet: %%s: {}'.format(rrset))
+            LOG.debug('rrset.as_dict():\n{}'.format(pp(rrset.as_dict())))
+        LOG.debug('RecordSet.as_dict(minimal=True): {}'.format(
             pp(rrset.as_dict(minimal=True))))
 
     # -------------------------------------------------------------------------
     def test_pdns_recordset_with_comment(self):
-
+        """Test instantiating of a PowerDNSRecordSet object with a comment."""
         if self.verbose:
             print()
-        LOG.info("Testing class PowerDNSRecordSet with comments ...")
+        LOG.info('Testing class PowerDNSRecordSet with comments ...')
 
         from fb_pdnstools.record import PowerDNSRecordSet
 
         js_rrset = self.get_js_a_rrset_comment()
 
         rrset = PowerDNSRecordSet.init_from_dict(
             js_rrset, appname=self.appname, verbose=self.verbose)
-        LOG.debug("RecordSet: %%r: {!r}".format(rrset))
+        LOG.debug('RecordSet: %%r: {!r}'.format(rrset))
         if self.verbose > 1:
-            LOG.debug("RecordSet: %%s: {}".format(rrset))
-            LOG.debug("rrset.as_dict():\n{}".format(pp(rrset.as_dict())))
-        LOG.debug("RecordSet.as_dict(minimal=True): {}".format(
+            LOG.debug('RecordSet: %%s: {}'.format(rrset))
+            LOG.debug('rrset.as_dict():\n{}'.format(pp(rrset.as_dict())))
+        LOG.debug('RecordSet.as_dict(minimal=True): {}'.format(
             pp(rrset.as_dict(minimal=True))))
 
 
 # =============================================================================
 if __name__ == '__main__':
 
     verbose = get_arg_verbose()
     if verbose is None:
         verbose = 0
     init_root_logger(verbose)
 
-    LOG.info("Starting tests ...")
+    LOG.info('Starting tests ...')
 
     loader = unittest.TestLoader()
     suite = unittest.TestSuite()
 
     suite.addTest(TestPdnsRecord('test_import_modules', verbose))
     suite.addTest(TestPdnsRecord('test_pdns_record', verbose))
     suite.addTest(TestPdnsRecord('test_pdns_record_equality', verbose))
```

### Comparing `fb_pdnstools-0.5.6/test/test_20_zone.py` & `fb_pdnstools-0.6.0/test/test_30_zone.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-'''
+"""
+@summary: Test script (and module) for unit tests on zone classes.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: LGPL3
-@summary: test script (and module) for unit tests on zone classes
-'''
+"""
 
-import os
-import sys
 import logging
 import logging.handlers
-
+import os
+import sys
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 libdir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'lib'))
 sys.path.insert(0, libdir)
 
+# Third party modules
 from fb_tools.common import pp
 
+# Own modules
 from general import FbPdnsToolsTestcase, get_arg_verbose, init_root_logger
 
 LOG = logging.getLogger('test_zone')
 
 
 # =============================================================================
 class TestPdnsZone(FbPdnsToolsTestcase):
+    """Testcase for tests on fb_pdnstools.zone."""
 
     # -------------------------------------------------------------------------
     def setUp(self):
+        """Hook for setup actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def tearDown(self):
+        """Hook for finishing actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def test_import_modules(self):
-
+        """Testing import of module fb_pdnstools.zone ..."""
         if self.verbose:
             print()
-        LOG.info("Test importing record module ...")
+        LOG.info('Test importing record module ...')
 
-        LOG.debug("Importing fb_pdnstools.zone ...")
+        LOG.debug('Importing fb_pdnstools.zone ...')
         import fb_pdnstools.zone
 
-        LOG.debug("Version of fb_pdnstools.zone: {!r}.".format(fb_pdnstools.zone.__version__))
+        LOG.debug('Version of fb_pdnstools.zone: {!r}.'.format(fb_pdnstools.zone.__version__))
 
-        LOG.info("Testing import of PowerDNSRecord from fb_pdnstools.record ...")
+        LOG.info('Testing import of PowerDNSZone from fb_pdnstools.zone ...')
         from fb_pdnstools.zone import PowerDNSZone
 
         zone = PowerDNSZone(appname=self.appname, verbose=self.verbose)
-        LOG.debug("Empty PowerDNSZone:\n{}".format(zone))
+        LOG.debug('Empty PowerDNSZone:\n{}'.format(zone))
 
-        LOG.info("Testing import of PowerDNSZoneDict from fb_pdnstools.record ...")
+        LOG.info('Testing import of PowerDNSZoneDict from fb_pdnstools.zone ...')
         from fb_pdnstools.zone import PowerDNSZoneDict
 
         zone_map = PowerDNSZoneDict()
-        LOG.debug("Empty PowerDNSZoneDict: {}".format(zone_map))
+        LOG.debug('Empty PowerDNSZoneDict: {}'.format(zone_map))
 
     # -------------------------------------------------------------------------
     def test_verify_fqdn(self):
-
+        """Test verifying a FQDN."""
         if self.verbose:
             print()
-        LOG.info("Testing PowerDNSZone.verify_fqdn() ...")
+        LOG.info('Testing PowerDNSZone.verify_fqdn() ...')
 
         valid_fqdns = [
             '@', 'testing.com.', 'uhu.testing.com.', ' uhu.testing.com.',
             'uhu.banane.testing.com.', 'UHU.TESTING.COM.']
         invalid_fqdns_type = [None, 33, True]
         invalid_fqdns_value = [
             '', '.', 'bla.@', 'testing.com', 'test.com.', '.testing.com', '.testing.com.',
@@ -81,87 +86,87 @@
         from fb_pdnstools.zone import PowerDNSZone
 
         js_zone = self.get_js_zone()
 
         zone = PowerDNSZone.init_from_dict(
             js_zone, appname=self.appname, verbose=self.verbose)
         if self.verbose > 1:
-            LOG.debug("Zone: %%r: {!r}".format(zone))
+            LOG.debug('Zone: %%r: {!r}'.format(zone))
         if self.verbose > 2:
-            LOG.debug("zone.as_dict():\n{}".format(pp(zone.as_dict())))
+            LOG.debug('zone.as_dict():\n{}'.format(pp(zone.as_dict())))
 
         for fqdn in valid_fqdns:
-            LOG.debug("Testing FQDN {f!r} for zone {z!r} ...".format(f=fqdn, z=zone.name))
+            LOG.debug('Testing FQDN {f!r} for zone {z!r} ...'.format(f=fqdn, z=zone.name))
             got_fqdn = zone.verify_fqdn(fqdn)
-            LOG.debug("Got verified FQDN {!r}.".format(got_fqdn))
+            LOG.debug('Got verified FQDN {!r}.'.format(got_fqdn))
             self.assertIsNotNone(got_fqdn)
 
         for fqdn in invalid_fqdns_type:
-            LOG.debug("Testing raise on FQDN {f!r} for zone {z!r} ...".format(f=fqdn, z=zone.name))
+            LOG.debug('Testing raise on FQDN {f!r} for zone {z!r} ...'.format(f=fqdn, z=zone.name))
             with self.assertRaises(TypeError) as cm:
                 got_fqdn = zone.verify_fqdn(fqdn)
-                LOG.error("This FQDN {!r} should never be visible.".format(got_fqdn))
+                LOG.error('This FQDN {!r} should never be visible.'.format(got_fqdn))
             e = cm.exception
-            LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+            LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
-            LOG.debug("Testing returning None on FQDN {f!r} for zone {z!r} ...".format(
+            LOG.debug('Testing returning None on FQDN {f!r} for zone {z!r} ...'.format(
                 f=fqdn, z=zone.name))
             got_fqdn = zone.verify_fqdn(fqdn, raise_on_error=False)
-            LOG.debug("Got back {!r}.".format(got_fqdn))
+            LOG.debug('Got back {!r}.'.format(got_fqdn))
             self.assertIsNone(got_fqdn)
 
         for fqdn in invalid_fqdns_value:
-            LOG.debug("Testing raise on FQDN {f!r} for zone {z!r} ...".format(f=fqdn, z=zone.name))
+            LOG.debug('Testing raise on FQDN {f!r} for zone {z!r} ...'.format(f=fqdn, z=zone.name))
             with self.assertRaises(ValueError) as cm:
                 got_fqdn = zone.verify_fqdn(fqdn)
-                LOG.error("This FQDN {!r} should never be visible.".format(got_fqdn))
+                LOG.error('This FQDN {!r} should never be visible.'.format(got_fqdn))
             e = cm.exception
-            LOG.debug("{} raised: {}".format(e.__class__.__name__, e))
+            LOG.debug('{} raised: {}'.format(e.__class__.__name__, e))
 
-            LOG.debug("Testing returning None on FQDN {f!r} for zone {z!r} ...".format(
+            LOG.debug('Testing returning None on FQDN {f!r} for zone {z!r} ...'.format(
                 f=fqdn, z=zone.name))
             got_fqdn = zone.verify_fqdn(fqdn, raise_on_error=False)
-            LOG.debug("Got back {!r}.".format(got_fqdn))
+            LOG.debug('Got back {!r}.'.format(got_fqdn))
             self.assertIsNone(got_fqdn)
 
     # -------------------------------------------------------------------------
     def test_zone_simple(self):
-
-        LOG.info("Testing class PowerDNSZone ...")
+        """Test instantiating of a simple PowerDNSZone object."""
+        LOG.info('Testing class PowerDNSZone ...')
 
         from fb_pdnstools.zone import PowerDNSZone
 
         js_zone = self.get_js_zone()
 
         PowerDNSZone.warn_on_unknown_property = True
         zone = PowerDNSZone.init_from_dict(
             js_zone, appname=self.appname, verbose=self.verbose)
-        LOG.debug("Zone: %%r: {!r}".format(zone))
+        LOG.debug('Zone: %%r: {!r}'.format(zone))
         if self.verbose > 1:
-            LOG.debug("Zone: %%s: {}".format(zone))
-            LOG.debug("zone.as_dict():\n{}".format(pp(zone.as_dict())))
+            LOG.debug('Zone: %%s: {}'.format(zone))
+            LOG.debug('zone.as_dict():\n{}'.format(pp(zone.as_dict())))
 
     # -------------------------------------------------------------------------
     def test_zone_get_soa(self):
-
-        LOG.info("Testing class PowerDNSZone.get_soa() ...")
+        """Test getting the SOA record from a PowerDNSZone object."""
+        LOG.info('Testing class PowerDNSZone.get_soa() ...')
 
         from fb_pdnstools.zone import PowerDNSZone
 
         js_zone = self.get_js_zone()
 
         PowerDNSZone.warn_on_unknown_property = True
         zone = PowerDNSZone.init_from_dict(
             js_zone, appname=self.appname, verbose=self.verbose)
         if self.verbose > 1:
-            LOG.debug("Zone: %%r: {!r}".format(zone))
+            LOG.debug('Zone: %%r: {!r}'.format(zone))
 
         soa = zone.get_soa()
         if self.verbose > 2:
-            LOG.debug("Got SOA object:\n{}".format(pp(soa.as_dict())))
+            LOG.debug('Got SOA object:\n{}'.format(pp(soa.as_dict())))
         self.assertIsNotNone(soa)
         self.assertEqual(soa.primary, 'ns1.example.com.')
         self.assertEqual(soa.email, 'hostmaster.example.com.')
         self.assertEqual(soa.serial, 2018061201)
         self.assertEqual(soa.refresh, 10800)
         self.assertEqual(soa.retry, 1800)
         self.assertEqual(soa.expire, 604800)
@@ -172,15 +177,15 @@
 if __name__ == '__main__':
 
     verbose = get_arg_verbose()
     if verbose is None:
         verbose = 0
     init_root_logger(verbose)
 
-    LOG.info("Starting tests ...")
+    LOG.info('Starting tests ...')
 
     loader = unittest.TestLoader()
     suite = unittest.TestSuite()
 
     suite.addTest(TestPdnsZone('test_import_modules', verbose))
     suite.addTest(TestPdnsZone('test_verify_fqdn', verbose))
     suite.addTest(TestPdnsZone('test_zone_simple', verbose))
```

### Comparing `fb_pdnstools-0.5.6/test/test_30_server.py` & `fb_pdnstools-0.6.0/test/test_40_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-'''
+"""
+@summary: Test script (and module) for unit tests on PDNS server class.
+
 @author: Frank Brehm
 @contact: frank@brehm-online.com
-@copyright: © 2021 Frank Brehm, Berlin
+@copyright: © 2023 Frank Brehm, Berlin
 @license: LGPL3
-@summary: test script (and module) for unit tests on PDNS server class
-'''
+"""
 
-import os
-import sys
+import json
 import logging
 import logging.handlers
-import json
-
+import os
+import sys
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
-import requests
-import requests_mock
-
 libdir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'lib'))
 sys.path.insert(0, libdir)
 
+# Third party modules
 from fb_tools.common import pp
 
 from general import FbPdnsToolsTestcase, get_arg_verbose, init_root_logger
 
+import requests
+
+import requests_mock
+
 LOG = logging.getLogger('test_server')
 
 
 # =============================================================================
 class TestPdnsServer(FbPdnsToolsTestcase):
+    """Testcase for tests on fb_pdnstools.server."""
 
     # -------------------------------------------------------------------------
     def setUp(self):
+        """Hook for setup actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def tearDown(self):
+        """Hook for finishing actions on each test method call."""
         pass
 
     # -------------------------------------------------------------------------
     def test_import_modules(self):
-
+        """Testing import of module fb_pdnstools.server ..."""
         if self.verbose:
             print()
-        LOG.info("Test importing server module ...")
+        LOG.info('Test importing server module ...')
 
-        LOG.debug("Importing fb_pdnstools.server ...")
+        LOG.debug('Importing fb_pdnstools.server ...')
         import fb_pdnstools.server
 
-        LOG.debug("Version of fb_pdnstools.server: {!r}.".format(fb_pdnstools.zone.__version__))
+        LOG.debug('Version of fb_pdnstools.server: {!r}.'.format(fb_pdnstools.zone.__version__))
 
-        LOG.info("Testing import of PowerDNSServer from fb_pdnstools.server ...")
+        LOG.info('Testing import of PowerDNSServer from fb_pdnstools.server ...')
         from fb_pdnstools.server import PowerDNSServer
 
         server = PowerDNSServer(appname=self.appname, verbose=self.verbose)
-        LOG.debug("Empty PowerDNSServer:\n{}".format(server))
+        LOG.debug('Empty PowerDNSServer:\n{}'.format(server))
 
     # -------------------------------------------------------------------------
     def set_mocking(self, obj):
+        """
+        Setting mocking mode in the given server object.
 
-        from fb_pdnstools import BasePowerDNSHandler
+        Also responses for some HTTP requests are prepared.
+        """
+        from fb_pdnstools.base_handler import BasePowerDNSHandler
 
         if not isinstance(obj, BasePowerDNSHandler):
-            msg = "Given object is not a BasePowerDNSHandler object, but a {} instead.".format(
+            msg = 'Given object is not a BasePowerDNSHandler object, but a {} instead.'.format(
                 obj.__class__.__name__)
             raise TypeError(msg)
 
         obj.mocked = True
 
         slist = self.get_js_serverlist()
         obj.mocking_paths.append({
@@ -94,65 +103,65 @@
         js_zone_rev = self.get_js_zone_rev()
         obj.mocking_paths.append({
             'method': 'GET', 'url': '/api/v1/servers/localhost/zones/222.40.10.in-addr.arpa.',
             'text': json.dumps(js_zone_rev)})
 
     # -------------------------------------------------------------------------
     def test_get_zone(self):
-
-        LOG.info("Testing getting a zone from a mocked PDNS API ...")
+        """Testing getting a zone from a mocked PDNS API."""
+        LOG.info('Testing getting a zone from a mocked PDNS API ...')
 
         adapter = requests_mock.Adapter()
         session = requests.Session()
         session.mount('mock', adapter)
 
         from fb_pdnstools.server import PowerDNSServer
         from fb_pdnstools.zone import PowerDNSZone, PowerDNSZoneDict
 
         pdns = PowerDNSServer(
             appname=self.appname, verbose=self.verbose, master_server=self.server_name,
             key=self.api_key, use_https=False)
         self.set_mocking(pdns)
 
-        LOG.debug("PowerDNSServer  %%r: {!r}".format(pdns))
+        LOG.debug('PowerDNSServer  %%r: {!r}'.format(pdns))
         if self.verbose > 1:
-            LOG.debug("PowerDNSServer: %%s: {}".format(pdns))
+            LOG.debug('PowerDNSServer: %%s: {}'.format(pdns))
         if self.verbose > 2:
-            LOG.debug("pdns.as_dict():\n{}".format(pp(pdns.as_dict())))
+            LOG.debug('pdns.as_dict():\n{}'.format(pp(pdns.as_dict())))
 
         api_version = pdns.get_api_server_version()
         self.assertEqual(api_version, self.server_version)
 
-        LOG.debug("Retreiving all zones ...")
+        LOG.debug('Retreiving all zones ...')
         zones = pdns.get_api_zones()
         self.assertIsInstance(zones, PowerDNSZoneDict)
-        self.assertIn("testing.com.", zones)
+        self.assertIn('testing.com.', zones)
 
-        LOG.debug("Retreiving zone {!r} ...".format("testing.com."))
-        zone = zones["testing.com."]
+        LOG.debug('Retreiving zone {!r} ...'.format('testing.com.'))
+        zone = zones['testing.com.']
         self.assertIsInstance(zone, PowerDNSZone)
         self.set_mocking(zone)
-        LOG.debug("Updating zone {!r} ...".format("testing.com."))
+        LOG.debug('Updating zone {!r} ...'.format('testing.com.'))
         zone.update()
-        LOG.debug("Zone: %%r: {!r}".format(zone))
+        LOG.debug('Zone: %%r: {!r}'.format(zone))
         if self.verbose > 1:
-            LOG.debug("Zone: %%s: {}".format(zone))
+            LOG.debug('Zone: %%s: {}'.format(zone))
         if self.verbose > 2:
-            LOG.debug("zone.as_dict: {}".format(pp(zone.as_dict())))
+            LOG.debug('zone.as_dict: {}'.format(pp(zone.as_dict())))
 
 
 # =============================================================================
 if __name__ == '__main__':
 
     verbose = get_arg_verbose()
     if verbose is None:
         verbose = 0
     init_root_logger(verbose)
 
-    LOG.info("Starting tests ...")
+    LOG.info('Starting tests ...')
 
     loader = unittest.TestLoader()
     suite = unittest.TestSuite()
 
     suite.addTest(TestPdnsServer('test_import_modules', verbose))
     suite.addTest(TestPdnsServer('test_get_zone', verbose))
```

### Comparing `fb_pdnstools-0.5.6/test/zone-rev.js` & `fb_pdnstools-0.6.0/test/zone-rev.js`

 * *Files identical despite different names*

### Comparing `fb_pdnstools-0.5.6/test/zone.js` & `fb_pdnstools-0.6.0/test/zone.js`

 * *Files identical despite different names*

### Comparing `fb_pdnstools-0.5.6/test/zones.js` & `fb_pdnstools-0.6.0/test/zones.js`

 * *Files identical despite different names*

