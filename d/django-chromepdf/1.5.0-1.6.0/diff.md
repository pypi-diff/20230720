# Comparing `tmp/django-chromepdf-1.5.0.tar.gz` & `tmp/django-chromepdf-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-chromepdf-1.5.0.tar", last modified: Wed Feb 22 16:05:23 2023, max compression
+gzip compressed data, was "dist/django-chromepdf-1.6.0.tar", last modified: Thu Jul 20 15:25:58 2023, max compression
```

## Comparing `django-chromepdf-1.5.0.tar` & `django-chromepdf-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.522157 django-chromepdf-1.5.0/
--rw-r--r--   0 kukwaa    (1078) ims        (100)      121 2022-06-07 14:51:55.000000 django-chromepdf-1.5.0/MANIFEST.in
--rw-r--r--   0 kukwaa    (1078) ims        (100)    11184 2023-02-22 16:05:23.521157 django-chromepdf-1.5.0/PKG-INFO
--rw-r--r--   0 kukwaa    (1078) ims        (100)     8494 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/README.md
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.459154 django-chromepdf-1.5.0/chromepdf/
--rw-r--r--   0 kukwaa    (1078) ims        (100)      296 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/__init__.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)      466 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/__main__.py
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.488157 django-chromepdf-1.5.0/chromepdf/chromedrivers/
--rw-r--r--   0 kukwaa    (1078) ims        (100)       93 2022-06-07 14:51:55.000000 django-chromepdf-1.5.0/chromepdf/chromedrivers/blank.txt
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.384153 django-chromepdf-1.5.0/chromepdf/chromesession/
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.493158 django-chromepdf-1.5.0/chromepdf/chromesession/users/
--rw-r--r--   0 kukwaa    (1078) ims        (100)       83 2022-06-07 14:51:55.000000 django-chromepdf-1.5.0/chromepdf/chromesession/users/blank.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)     2274 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/conf.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)      141 2022-06-07 14:51:55.000000 django-chromepdf-1.5.0/chromepdf/exceptions.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3878 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/maker.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     8853 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/pdfconf.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     4397 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/run.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     2413 2022-06-07 14:51:55.000000 django-chromepdf-1.5.0/chromepdf/shortcuts.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3108 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/sizes.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)    14375 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/chromepdf/webdrivers.py
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-02-22 16:05:23.516155 django-chromepdf-1.5.0/django_chromepdf.egg-info/
--rw-r--r--   0 kukwaa    (1078) ims        (100)    11184 2023-02-22 16:05:21.000000 django-chromepdf-1.5.0/django_chromepdf.egg-info/PKG-INFO
--rw-r--r--   0 kukwaa    (1078) ims        (100)      512 2023-02-22 16:05:21.000000 django-chromepdf-1.5.0/django_chromepdf.egg-info/SOURCES.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)        1 2023-02-22 16:05:21.000000 django-chromepdf-1.5.0/django_chromepdf.egg-info/dependency_links.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)       15 2023-02-22 16:05:21.000000 django-chromepdf-1.5.0/django_chromepdf.egg-info/requires.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)       10 2023-02-22 16:05:21.000000 django-chromepdf-1.5.0/django_chromepdf.egg-info/top_level.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)       38 2023-02-22 16:05:23.523157 django-chromepdf-1.5.0/setup.cfg
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3932 2023-02-22 16:02:22.000000 django-chromepdf-1.5.0/setup.py
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/chromepdf/
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/chromepdf/chromedrivers/
+-rw-r--r--   0 kukwaa    (1078) ims        (100)       93 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/chromedrivers/blank.txt
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:57.000000 django-chromepdf-1.6.0/chromepdf/chromesession/
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/chromepdf/chromesession/users/
+-rw-r--r--   0 kukwaa    (1078) ims        (100)       83 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/chromesession/users/blank.txt
+-rw-r--r--   0 kukwaa    (1078) ims        (100)      296 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/__init__.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)      466 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/__main__.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     2276 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/conf.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)      141 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/exceptions.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     3532 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/maker.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     8853 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/pdfconf.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     4685 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/run.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     2309 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/shortcuts.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     3108 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/chromepdf/sizes.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     9230 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/webdrivermakers.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)    16995 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/chromepdf/webdrivers.py
+drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/
+-rw-r--r--   0 kukwaa    (1078) ims        (100)    11184 2023-07-20 15:25:56.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/PKG-INFO
+-rw-r--r--   0 kukwaa    (1078) ims        (100)      541 2023-07-20 15:25:56.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 kukwaa    (1078) ims        (100)        1 2023-07-20 15:25:56.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 kukwaa    (1078) ims        (100)       15 2023-07-20 15:25:56.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/requires.txt
+-rw-r--r--   0 kukwaa    (1078) ims        (100)       10 2023-07-20 15:25:56.000000 django-chromepdf-1.6.0/django_chromepdf.egg-info/top_level.txt
+-rw-r--r--   0 kukwaa    (1078) ims        (100)      121 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/MANIFEST.in
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     8494 2023-07-20 15:23:11.000000 django-chromepdf-1.6.0/README.md
+-rw-r--r--   0 kukwaa    (1078) ims        (100)     3932 2023-07-20 15:22:57.000000 django-chromepdf-1.6.0/setup.py
+-rw-r--r--   0 kukwaa    (1078) ims        (100)    11184 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/PKG-INFO
+-rw-r--r--   0 kukwaa    (1078) ims        (100)       38 2023-07-20 15:25:58.000000 django-chromepdf-1.6.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-chromepdf-1.5.0/PKG-INFO` & `django-chromepdf-1.6.0/django_chromepdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-chromepdf
-Version: 1.5.0
+Version: 1.6.0
 Summary: A small Python 3 library that uses Selenium and Google Chrome to convert HTML into a PDF.
 Home-page: https://github.com/imsweb/django-chromepdf
 Author: Andrew Kukwa
 Author-email: kukwaa@imsweb.com
 License: BSD
 Project-URL: Source, https://github.com/imsweb/django-chromepdf
 Project-URL: Changelog, https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md
@@ -36,15 +36,15 @@
         
         **1. Install ChromePDF via pip.**
         
         The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
         
         You may view the [Changelog](https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
         ```
-        pip install django-chromepdf~=1.5.0
+        pip install django-chromepdf~=1.6.0
         ```
         
         **2. Set the location of your Chrome executable.** This can be done in one of two ways:
         
         * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
         * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
```

### Comparing `django-chromepdf-1.5.0/README.md` & `django-chromepdf-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 **1. Install ChromePDF via pip.**
 
 The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
 
 You may view the [Changelog](CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
 ```
-pip install django-chromepdf~=1.5.0
+pip install django-chromepdf~=1.6.0
 ```
 
 **2. Set the location of your Chrome executable.** This can be done in one of two ways:
 
 * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
 * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
```

### Comparing `django-chromepdf-1.5.0/chromepdf/conf.py` & `django-chromepdf-1.6.0/chromepdf/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 DEFAULT_SETTINGS = {
     'CHROME_PATH': None,
     'CHROMEDRIVER_PATH': None,
     'CHROMEDRIVER_DOWNLOADS': True,
     # also, PDF_KWARGS, but it's handled differently
     'CHROME_ARGS': [],
+    'USE_SELENIUM': None,
 }
 
 
 def get_chromepdf_settings_dict():
     """
     Return a Django's settings.CHROMEPDF dict. Return empty dict if not found or Django not installed.
     For our sanity, this should be the ONLY place within the chromepdf app that we import from Django.
     This way, the library should work even if Django is not installed (except with its settings ignored).
     """
     try:
         from django.conf import settings
         return getattr(settings, 'CHROMEPDF', {})
     except Exception:
-        # catches ImportError and ModuleNotFoundError, and potentially Django's ImproperlyConfigured.
+        # catches ImportError, and potentially Django's ImproperlyConfigured.
         # But we can't explitly name that here since Django might not be installed. So, use a general Exception.
         return {}
 
 
 def parse_settings(**overrides):
     """
     Return a dict of lowercased DEFAULT_SETTINGS based on combination of defaults, Django settings, and overrides.
```

### Comparing `django-chromepdf-1.5.0/chromepdf/pdfconf.py` & `django-chromepdf-1.6.0/chromepdf/pdfconf.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.5.0/chromepdf/run.py` & `django-chromepdf-1.6.0/chromepdf/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     # Other sub-commands may be added in the future
     genpdf_parser = subparsers.add_parser('generate-pdf', help='Generate a PDF file. Followed by one or two args: The part to the input HTML file, and path to the output PDF file. EG: "generate-pdf path/to/file.html path/to/file.pdf"')
     genpdf_parser.add_argument('paths', nargs='*')
     genpdf_parser.add_argument("--pdf-kwargs-json", help="Path to a JSON file whose contents can decode to a pdf_kwargs dict.")
     genpdf_parser.add_argument("--chrome-path", help="Path to Chrome executable")
     genpdf_parser.add_argument("--chromedriver-path", help="Path to Chrome executable")
     genpdf_parser.add_argument("--chromedriver-downloads", type=int, choices=(0, 1), help='1 or 0, to indicate whether to use Chromedriver downloads or not.')
+    genpdf_parser.add_argument("--use-selenium", type=int, choices=(0, 1, -1), help='1=yes, 2=no, -1=use Selenium if present, else do not.')
     genpdf_parser.add_argument("--chrome-args", help='A string of all arguments to pass to Chrome, separated by spaces.')
 
     return parser
 
 
 def _command_generate_pdf(parser, namespace):
     """Call the generate_pdf() function using command-line arguments."""
@@ -63,14 +64,16 @@
     kwargs = {}
     if namespace.chrome_path is not None:
         kwargs['chrome_path'] = namespace.chrome_path
     if namespace.chromedriver_path is not None:
         kwargs['chromedriver_path'] = namespace.chromedriver_path
     if namespace.chromedriver_downloads is not None:
         kwargs['chromedriver_downloads'] = bool(namespace.chromedriver_downloads)
+    if namespace.use_selenium is not None:
+        kwargs['use_selenium'] = None if namespace.use_selenium == -1 else bool(namespace.use_selenium)
     if namespace.chrome_args is not None:
         kwargs['chrome_args'] = namespace.chrome_args.strip().split()
 
     pdf_kwargs = None
     if namespace.pdf_kwargs_json is not None:
         if not os.path.exists(namespace.pdf_kwargs_json):
             parser.error(f'generate-pdf: could not find input pdf-kwargs-json file: "{namespace.pdf_kwargs_json}"')
```

### Comparing `django-chromepdf-1.5.0/chromepdf/shortcuts.py` & `django-chromepdf-1.6.0/chromepdf/shortcuts.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,10 +52,8 @@
 
     with open("myfile.pdf", 'wb') as file:
         file.write(pdfbytes)
 
 
     """
 
-    warnings.warn("generate_pdf_url() is deprecated, use generate_pdf() instead.", DeprecationWarning)
-
     return ChromePdfMaker(**kwargs).generate_pdf_url(url, pdf_kwargs)
```

### Comparing `django-chromepdf-1.5.0/chromepdf/sizes.py` & `django-chromepdf-1.6.0/chromepdf/sizes.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.5.0/chromepdf/webdrivers.py` & `django-chromepdf-1.6.0/chromepdf/webdrivers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 import subprocess
 import warnings
 import zipfile
 from contextlib import contextmanager
 from subprocess import PIPE
 from urllib import request as urllib_request
 
-import selenium
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-
 from chromepdf.exceptions import ChromePdfException
 
 
-_IS_SELENIUM_3 = selenium.__version__.split('.')[0] == '3'
-
-
 def _version_to_tuple(version):
     """
     Shortcut function that converts version string to tuple, for allowing deprecated behavior.
     In ChromePDF 2.0, this should no longer be needed. Tuple support will no longer exist.
     """
     return tuple(int(i) for i in version.split('.'))
 
@@ -36,14 +29,26 @@
     """
     if isinstance(version, tuple):
         warnings.warn("Support for versions as tuples is now deprecated. Pass a string instead.", DeprecationWarning)
         return '.'.join(str(i) for i in version)
     return version
 
 
+_CHROME_PATHS = ('chrome', 'chrome.exe', 'Google Chrome')
+
+
+def find_chrome():
+    "Mimic Selenium's ability to find Google Chrome on PATH, for its default executable names for each OS."
+    for path in _CHROME_PATHS:
+        fullpath = shutil.which(path)
+        if fullpath is not None:
+            return fullpath
+    return None
+
+
 def _get_chrome_version_str(path):
     """
     Return a string containing the version number of the Chrome binary exe, EG for Chrome 85: '85.0.4183.121'
     raise ChromePdfException otherwise (EG if path not found)
     """
 
     is_windows = (platform.system() == 'Windows')
@@ -127,30 +132,47 @@
     """
 
     version = _force_version_str(version)
 
     # Google's API for the latest release takes only the first 3 parts of the version
     version_first3parts = version.rsplit('.', maxsplit=1)[0]  # EG, "85.0.4183"
 
-    # This url returns a 4-part version string of the latest compatible chromedriver for your Chrome version.
-    # This might be DIFFERENT than the version of your Chrome executable.
-    url = f'https://chromedriver.storage.googleapis.com/LATEST_RELEASE_{version_first3parts}'
-    with urllib_request.urlopen(url) as f:
-        contents = f.read()
-    chromedriver_version = contents.decode('utf8')  # EG "85.0.4183.87"
+    version_major = int(version.split('.')[0])
+    if version_major >= 115:
+        # Starting with version 115, use new endpoint
+        # https://groups.google.com/g/chromedriver-users/c/clpipqvOGjE
+        url = 'https://googlechromelabs.github.io/chrome-for-testing/latest-patch-versions-per-build.json'
+        with urllib_request.urlopen(url) as f:
+            contents = json.loads(f.read().decode('utf8'))
+        chromedriver_version = contents['builds'][version_first3parts]['version']
+
+    else:
+        # This url returns a 4-part version string of the latest compatible chromedriver for your Chrome version.
+        # This might be DIFFERENT than the version of your Chrome executable.
+        url = f'https://chromedriver.storage.googleapis.com/LATEST_RELEASE_{version_first3parts}'
+        with urllib_request.urlopen(url) as f:
+            contents = f.read()
+        chromedriver_version = contents.decode('utf8')  # EG "85.0.4183.87"
+
     return chromedriver_version
 
 
 def _get_chromedriver_zip_url(chromedriver_version):
     """
-    Get the chromedriver zip download url for our particular OS+Processor.
+    Get the chromedriver zip download url for our particular OS+Processor for chrome versions 114 and earlier.
     The possible urls are taken from the chromedriver release files list, here:
     https://chromedriver.chromium.org/downloads
     """
 
+    version_major = int(chromedriver_version.split('.')[0])
+    if version_major >= 115:
+        # Starting with version 115, all chrome releases will get a "correspondingly-versioned" chromedriver release.
+        # https://groups.google.com/g/chromedriver-users/c/clpipqvOGjE
+        return _get_chromedriver_zip_url_v115_and_later(chromedriver_version)
+
     is_windows = (platform.system() == 'Windows')
     is_mac = (platform.system() == 'Darwin')
     is_mac_m1 = (is_mac and platform.processor() == 'arm')
 
     if is_windows:
         os_plus_numbits = 'win32'
     elif is_mac_m1:
@@ -160,14 +182,40 @@
     else:
         os_plus_numbits = 'linux64'
     filename = f'chromedriver_{os_plus_numbits}.zip'
 
     return f'https://chromedriver.storage.googleapis.com/{chromedriver_version}/{filename}'
 
 
+def _get_chromedriver_zip_url_v115_and_later(chromedriver_version):
+    """
+    Get the chromedriver zip url for chromedriver versions 115 and up.
+    """
+
+    is_windows = (platform.system() == 'Windows')
+    is_mac = (platform.system() == 'Darwin')
+    is_mac_m1 = (is_mac and platform.processor() == 'arm')
+
+    if is_windows:
+        os_plus_numbits = 'win32'
+    elif is_mac_m1:
+        os_plus_numbits = 'mac-arm64'
+    elif is_mac:
+        os_plus_numbits = 'mac-x64'
+    else:
+        os_plus_numbits = 'linux64'
+
+    # Official code is using the following endpoint for all downloads:
+    # https://github.com/GoogleChromeLabs/chrome-for-testing/blob/dc9fb4537e7f07352431c0fdf308825d2f77bc72/url-utils.mjs#L33
+    filename = f'chromedriver-{os_plus_numbits}.zip'
+    url = f'https://edgedl.me.gvt1.com/edgedl/chrome/chrome-for-testing/{chromedriver_version}/{os_plus_numbits}/{filename}'
+
+    return url
+
+
 def _fetch_chromedriver_zip_bytes(chromedriver_version):
     """
     Return the bytes of the chromedriver zip file for the given chromedriver version, for our OS.
     """
 
     url = _get_chromedriver_zip_url(chromedriver_version)
     with urllib_request.urlopen(url) as f:
@@ -198,17 +246,18 @@
     # chromedrivers have their own version strings. fetch the one for our chrome version.
     chromedriver_version = _fetch_chromedriver_version_for_chrome_version(version)
 
     # Download the zip file containing our chromedriver
     zip_bytes = _fetch_chromedriver_zip_bytes(chromedriver_version)
 
     # Open the zip file, find the chromedriver, and save it to the specified path.
+    # Be advised: pre-115 zip files contain no subfolders, but 115+ contains one subfolder with the chromedriver.
     with zipfile.ZipFile(io.BytesIO(zip_bytes), "r") as zf:
         for name in zf.namelist():
-            if 'chromedriver' in name:
+            if 'chromedriver' in name and not '.chromedriver' in name:  # get "chromedriver[.exe]" but not "LICENSE.chromedriver"
                 with zf.open(name) as chromedriver_file:
                     with open(chromedriver_download_path, 'wb') as f:
                         f.write(chromedriver_file.read())
                         os.chmod(chromedriver_download_path, 0o764)  # grant execute permission
                         return chromedriver_download_path
 
     raise ChromePdfException('Failed to download the chromedriver file.')
@@ -225,93 +274,115 @@
     * chrome_args: List of options to pass to Chrome.
 
     with get_chrome_webdriver(...) as driver:
         # call commands...
     # driver is automatically closed
     """
 
-    chrome_webdriver_kwargs = _get_chrome_webdriver_kwargs(chrome_path, chromedriver_path, **kwargs)
+    warnings.warn("get_chrome_webdriver() is deprecated. Use get_webdriver_maker() instead.", DeprecationWarning)
 
     # contextmanager.__enter__
+
+    from selenium import webdriver
+    chrome_webdriver_kwargs = _get_chrome_webdriver_kwargs(chrome_path, chromedriver_path, **kwargs)
     try:
         driver = webdriver.Chrome(**chrome_webdriver_kwargs)
+
     except Exception as ex:
         if chrome_path and not os.path.exists(chrome_path):
             raise ChromePdfException(f'Could not find a chrome_path path at: {chrome_path}') from ex
         elif chromedriver_path and not os.path.exists(chromedriver_path):
             raise ChromePdfException(f'Could not find a chromedriver_path at: {chromedriver_path}') from ex
         else:
             raise ex
 
     yield driver
 
     # contextmanager.__exit__
     driver.quit()  # quits the entire driver (driver.close() only closes the current window)
 
 
-def _get_chrome_webdriver_kwargs(chrome_path, chromedriver_path, **kwargs):
-    """Return the kwargs needed to pass to webdriver.Chrome(), given the CHROMEPDF settings."""
+def _get_chrome_webdriver_args(**kwargs):
+    """
+    Return arguments to pass to Chrome when starting.
+    This function should not use Selenium, since it is also needed by the no-Selenium driver maker.
+    """
 
-    # at one point "-disable-gpu" was required for headless Chrome. Keep it here just in case.
-    # https://bugs.chromium.org/p/chromium/issues/detail?id=737678
-    options = webdriver.ChromeOptions()
-    options.add_argument("--headless")
-    options.add_argument("--disable-gpu")
+    args = []
+
+    args.append("--headless")
+    args.append("--disable-gpu")
 
-    options.add_argument("--log-level=3")  # silence logging
+    args.append("--log-level=3")  # silence logging
 
     # disables the creation of the crash-dumps-dir.
     # will work even if --crash-dumps-dir is provided.
     # keep both as fallbacks. either is preferable to the global default.
-    options.add_argument('--disable-crash-reporter')
+    args.append('--disable-crash-reporter')
 
     # incognito mode lets us run chrome without creating and storing a user profile to disk.
     # this lets us generate PDFs in a thread- and process-safe way since they will not be
     # fighting over reading/writing the same files in the --user-data-dir
     # passing --incognito AND --user-data-dir= WILL cause the user-data-dir folder to be populated, so don't.
-    options.add_argument("--incognito")
+    args.append("--incognito")
 
     temp_dir = kwargs.get('_chromesession_temp_dir')
     if temp_dir is not None:
         crash_dumps_dir = os.path.join(temp_dir, 'crash-dumps-dir')
-        options.add_argument(f"--crash-dumps-dir={crash_dumps_dir}")
+        args.append(f"--crash-dumps-dir={crash_dumps_dir}")
 
     # add extra chrome args
     chrome_args = kwargs.get('chrome_args', [])
     for argv in chrome_args:
-        options.add_argument(argv)
+        args.append(argv)
+
+    return args
+
+
+def _get_chrome_webdriver_kwargs(chrome_path, chromedriver_path, **kwargs):
+    """Return the kwargs needed to pass to webdriver.Chrome(), given the CHROMEPDF settings."""
+
+    import selenium
+    from selenium import webdriver
+    from selenium.webdriver.chrome.service import Service
+    is_selenium_3 = selenium.__version__.split('.')[0] == '3'
+
+    options = webdriver.ChromeOptions()
+
+    args = _get_chrome_webdriver_args(**kwargs)
+    for arg in args:
+        options.add_argument(arg)
 
     # silence the "DevTools started" message on windows
     # https://bugs.chromium.org/p/chromedriver/issues/detail?id=2907#c3
     options.add_experimental_option('excludeSwitches', ['enable-logging'])
 
     # In Selenium 4, we must tell the driver to ignore any os.environ['http_proxy'/'https_proxy'] values.
     # Calling this function preserves Selenium 3 behavior, which did not check them at all.
     # This function does not exist in Selenium 3, so we must check if it exists to preserve Selenium 3 compatibility.
-    # https://github.com/SeleniumHQ/selenium/issues/8768
     if hasattr(options, 'ignore_local_proxy_environment_variables') and callable(options.ignore_local_proxy_environment_variables):
         options.ignore_local_proxy_environment_variables()
 
     if chrome_path is not None:
         options.binary_location = chrome_path  # Selenium API
 
     chrome_kwargs = {'options': options}
     if chromedriver_path is not None:
-        if _IS_SELENIUM_3:
+        if is_selenium_3:
             chrome_kwargs['executable_path'] = chromedriver_path
         else:
             # executable_path is deprecated in Selenium 4.1.0 - start using Service() instead.
             chrome_kwargs['service'] = Service(chromedriver_path)  # Selenium API
 
     return chrome_kwargs
 
 
 def devtool_command(driver, cmd, params=None):
     """
-    Send a command to Chrome via the web driver.
+    Send a command to Chrome via the Selenium web driver.
     Example:
         result = devtool_command(driver, "Page.printToPDF", pdf_kwargs)
     """
 
     if params is None:
         params = {}
     resource = f"/session/{driver.session_id}/chromium/send_command_and_get_result"
```

### Comparing `django-chromepdf-1.5.0/django_chromepdf.egg-info/PKG-INFO` & `django-chromepdf-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-chromepdf
-Version: 1.5.0
+Version: 1.6.0
 Summary: A small Python 3 library that uses Selenium and Google Chrome to convert HTML into a PDF.
 Home-page: https://github.com/imsweb/django-chromepdf
 Author: Andrew Kukwa
 Author-email: kukwaa@imsweb.com
 License: BSD
 Project-URL: Source, https://github.com/imsweb/django-chromepdf
 Project-URL: Changelog, https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md
@@ -36,15 +36,15 @@
         
         **1. Install ChromePDF via pip.**
         
         The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
         
         You may view the [Changelog](https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
         ```
-        pip install django-chromepdf~=1.5.0
+        pip install django-chromepdf~=1.6.0
         ```
         
         **2. Set the location of your Chrome executable.** This can be done in one of two ways:
         
         * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
         * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
```

### Comparing `django-chromepdf-1.5.0/django_chromepdf.egg-info/SOURCES.txt` & `django-chromepdf-1.6.0/django_chromepdf.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 chromepdf/conf.py
 chromepdf/exceptions.py
 chromepdf/maker.py
 chromepdf/pdfconf.py
 chromepdf/run.py
 chromepdf/shortcuts.py
 chromepdf/sizes.py
+chromepdf/webdrivermakers.py
 chromepdf/webdrivers.py
 chromepdf/chromedrivers/blank.txt
 chromepdf/chromesession/users/blank.txt
 django_chromepdf.egg-info/PKG-INFO
 django_chromepdf.egg-info/SOURCES.txt
 django_chromepdf.egg-info/dependency_links.txt
 django_chromepdf.egg-info/requires.txt
```

### Comparing `django-chromepdf-1.5.0/setup.py` & `django-chromepdf-1.6.0/setup.py`

 * *Files identical despite different names*

