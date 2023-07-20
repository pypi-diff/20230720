# Comparing `tmp/cubicweb-signedrequest-2.1.0.tar.gz` & `tmp/cubicweb-signedrequest-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-signedrequest-2.1.0.tar", last modified: Tue Feb 21 18:44:23 2023, max compression
+gzip compressed data, was "cubicweb-signedrequest-3.0.0.tar", last modified: Thu Jul 20 08:18:42 2023, max compression
```

## Comparing `cubicweb-signedrequest-2.1.0.tar` & `cubicweb-signedrequest-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.596967 cubicweb-signedrequest-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2529 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2077 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.588967 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/authplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/doc/
--rw-rw-rw-   0 root         (0) root         (0)     3869 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/doc/sreq_example.py
--rw-rw-rw-   0 root         (0) root         (0)     2245 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)     2155 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/migration/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/migration/0.2.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/migration/0.3.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/migration/2.1.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/pconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2529 2023-02-21 18:44:21.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1124 2023-02-21 18:44:23.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 18:44:21.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-02-21 18:44:22.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 18:44:21.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-21 18:44:22.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-21 18:44:23.000000 cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 18:44:23.596967 cubicweb-signedrequest-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2639 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/test/
--rw-rw-rw-   0 root         (0) root         (0)    11886 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 18:44:23.592967 cubicweb-signedrequest-2.1.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/test_pyramid.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/test_signedrequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/unittest_authenticate.py
--rw-rw-rw-   0 root         (0) root         (0)     5574 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/test/unittest_security.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-02-21 18:43:46.000000 cubicweb-signedrequest-2.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.427081 cubicweb-signedrequest-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-20 08:18:42.427081 cubicweb-signedrequest-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.415080 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/authplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.419081 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-07-20 08:18:21.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/doc/sreq_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2245 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.419081 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.423081 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/migration/2.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/pconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7828 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.415080 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 08:18:42.000000 cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 08:18:42.427081 cubicweb-signedrequest-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.427081 cubicweb-signedrequest-3.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)    11886 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:18:42.427081 cubicweb-signedrequest-3.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2802 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/test_pyramid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/test_signedrequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/unittest_authenticate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5574 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-20 08:18:22.000000 cubicweb-signedrequest-3.0.0/tox.ini
```

### Comparing `cubicweb-signedrequest-2.1.0/MANIFEST.in` & `cubicweb-signedrequest-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/PKG-INFO` & `cubicweb-signedrequest-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-signedrequest
-Version: 2.1.0
+Version: 3.0.0
 Summary: rest api for cubicweb
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-signedrequest
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -61,9 +60,7 @@
 
 Please read the documentation of cwclientlib_ for examples of how it
 can be used.
 
 .. _cubicweb-rqlcontroller: https://www.cubicweb.org/project/cubicweb-rqlcontroller
 .. _cubicweb-signedrequest: https://www.cubicweb.org/project/cubicweb-signedrequest
 .. _cwclientlib: https://www.cubicweb.org/project/cwclientlib
-
-
```

### Comparing `cubicweb-signedrequest-2.1.0/README.rst` & `cubicweb-signedrequest-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/__init__.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/__pkginfo__.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/__pkginfo__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-signedrequest application packaging information"""
 
 modname = "signedrequest"
 distname = "cubicweb-signedrequest"
 
-numversion = (2, 1, 0)
+numversion = (3, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "rest api for cubicweb"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    "cubicweb": ">= 3.38.0, < 3.39.0",
+    "cubicweb": ">= 4.0.0, < 5.0.0",
 }
 
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
```

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/authplugin.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/authplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/doc/sreq_example.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/doc/sreq_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,15 @@
     def __init__(self, token_id, secret):
         self.token_id = token_id
         self.secret = secret
 
     def __call__(self, r):
         if r.method in ("PUT", "POST"):
             r.headers["Content-SHA512"] = sha512(r.body or "")
-        r.headers["Authorization"] = "Cubicweb {}:{}".format(
-            self.token_id,
-            sign(r, self.secret),
-        )
+        r.headers["Authorization"] = f"Cubicweb {self.token_id}:{sign(r, self.secret)}"
         return r
 
 
 def get(url, token_id, token):
     auth = SignedRequestAuth(token_id, token)
     resp = requests.get(
         url,
```

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/hooks.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/en.po` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/es.po` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/i18n/fr.po` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/pconfig.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/pconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/schema.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/site_cubicweb.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/tools.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         raise AuthenticationError()
     delta = abs(datetime.utcnow() - date)
     if delta > timedelta(0, 300):
         log.error("SIGNED REQUEST: date delta error")
         raise AuthenticationError()
     try:
         id, signature = credentials.split(":", 1)
-        log.debug("SIGNED REQUEST: encoding info for %s" % id)
+        log.debug(f"SIGNED REQUEST: encoding info for {id}")
         return credentials
     except ValueError:
         log.exception("HTTP REST authenticator failed")
         raise AuthenticationError()
 
 
 def build_string_to_sign(request, url=None, headers=None):
```

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest/views.py` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 
 
 class AuthTestSuccess(Controller):
     __regid__ = "authtest"
     __select__ = ~anonymous_user()
 
     def publish(self, rset=None):
-        return "you are properly authenticated as %s" % self._cw.user.login
+        return f"you are properly authenticated as {self._cw.user.login}"
```

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/PKG-INFO` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-signedrequest
-Version: 2.1.0
+Version: 3.0.0
 Summary: rest api for cubicweb
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-signedrequest
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -61,9 +60,7 @@
 
 Please read the documentation of cwclientlib_ for examples of how it
 can be used.
 
 .. _cubicweb-rqlcontroller: https://www.cubicweb.org/project/cubicweb-rqlcontroller
 .. _cubicweb-signedrequest: https://www.cubicweb.org/project/cubicweb-signedrequest
 .. _cwclientlib: https://www.cubicweb.org/project/cwclientlib
-
-
```

### Comparing `cubicweb-signedrequest-2.1.0/cubicweb_signedrequest.egg-info/SOURCES.txt` & `cubicweb-signedrequest-3.0.0/cubicweb_signedrequest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/setup.py` & `cubicweb-signedrequest-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = [
-    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-signedrequest-2.1.0/test/__init__.py` & `cubicweb-signedrequest-3.0.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/test/pytestconf.py` & `cubicweb-signedrequest-3.0.0/test/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/test/test_pyramid.py` & `cubicweb-signedrequest-3.0.0/test/test_pyramid.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,28 +11,24 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from operator import itemgetter
-import webtest
 
-from cubicweb.pyramid.test import PyramidCWTest
+from webtest import TestRequest
 
 from cubicweb_signedrequest import includeme
 from cubicweb_signedrequest.tools import HEADERS_TO_SIGN
+from cubicweb_web.devtools.testlib import PyramidWebCWTC
 from test import TestController, SignedRequestBaseTC
 
 
-class PyramidSignedRequestTC(SignedRequestBaseTC, PyramidCWTest):
-    settings = {
-        "cubicweb.bwcompat": True,
-    }
-
+class PyramidSignedRequestTC(SignedRequestBaseTC, PyramidWebCWTC):
     def includeme(self, config):
         includeme(config)
 
     def _assert_auth_failed(self, req, result):
         self.assertEqual(b"INVALID", result)
 
     def _assert_auth(self, req, result):
@@ -55,15 +51,15 @@
         content=None,
         url="/testauth",
         **params,
     ):
         if headers is None:
             headers = {}
         headers = self.get_valid_authdata(headers)
-        req = webtest.TestRequest.blank(
+        req = TestRequest.blank(
             url,
             base_url=self.config["base-url"].rstrip("/"),
             method=method,
             headers=headers,
             **params,
         )
         if http_method == "POST":
@@ -72,15 +68,15 @@
         if content:
             req.body = content
 
         if signature is None:
             string_to_sign = self._build_string_to_sign(req)
             signature = self._build_signature(token_id, string_to_sign)
 
-        req.headers["Authorization"] = "{} {}:{}".format(method, token_id, signature)
+        req.headers["Authorization"] = f"{method} {token_id}:{signature}"
         with self.temporary_appobjects(TestController):
             resp = self.webapp.do_request(req)
         return resp.body, resp
 
 
 if __name__ == "__main__":
     import unittest
```

### Comparing `cubicweb-signedrequest-2.1.0/test/test_signedrequest.py` & `cubicweb-signedrequest-3.0.0/test/test_signedrequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,18 @@
             '''only test views for entities of the returned types'''
             return set(('My', 'Cube', 'Entity', 'Types'))
 
         def list_startup_views(self):
             '''only test startup views of the returned identifiers'''
             return ('some', 'startup', 'views')
 """
+from cubicweb_web.devtools.testlib import AutomaticWebTest
 
-from cubicweb.devtools import testlib
 
-
-class AutomaticWebTest(testlib.AutomaticWebTest):
+class AutomaticWebTest(AutomaticWebTest):
     def to_test_etypes(self):
         return {"AuthToken"}
 
     def test_one_each_config(self):
         self.skipTest("cubiweb.devtools.fill does not know about tzdatetime")
 
     def test_ten_each_config(self):
```

### Comparing `cubicweb-signedrequest-2.1.0/test/unittest_authenticate.py` & `cubicweb-signedrequest-3.0.0/test/unittest_authenticate.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 "cubicweb-signedrequest automatic tests for authentication"
 
 from io import BytesIO
 
-from cubicweb.devtools.testlib import CubicWebTC, real_error_handling
+from cubicweb.devtools.testlib import real_error_handling
+from cubicweb_web.devtools.testlib import WebCWTC
 
 from cubicweb_signedrequest.tools import HEADERS_TO_SIGN
 from test import TestController, SignedRequestBaseTC
 
 
-class SignedRequestTC(SignedRequestBaseTC, CubicWebTC):
+class SignedRequestTC(SignedRequestBaseTC, WebCWTC):
     def _assert_auth(self, req, result):
         self.assertEqual(200, req.status_out)
         self.assertEqual(b"VALID", result)
 
     def _assert_auth_failed(self, req, result):
         if req.status_out == 200:
             self.assertEqual(b"INVALID", result)
@@ -68,15 +69,15 @@
             for name, value in headers.items():
                 req.set_request_header(name, value, raw=True)
             if signature is None:
                 string_to_sign = self._build_string_to_sign(req)
                 signature = self._build_signature(token_id, string_to_sign)
             req.set_request_header(
                 "Authorization",
-                "{} {}:{}".format(method, token_id, signature),
+                f"{method} {token_id}:{signature}",
                 raw=True,
             )
             with real_error_handling(self.app):
                 result = self.app.handle_request(req)
         return result, req
```

### Comparing `cubicweb-signedrequest-2.1.0/test/unittest_security.py` & `cubicweb-signedrequest-3.0.0/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-signedrequest-2.1.0/tox.ini` & `cubicweb-signedrequest-3.0.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tox]
 envlist = py3,flake8,black,check-manifest,yamllint
 
 [testenv]
 deps =
   webtest
   pytest
+  cubicweb-web>=1.0.0,<2.0.0
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs:--verbose}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
@@ -46,15 +47,15 @@
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
```

