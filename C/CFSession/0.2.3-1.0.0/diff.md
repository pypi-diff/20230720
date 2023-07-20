# Comparing `tmp/CFSession-0.2.3.tar.gz` & `tmp/CFSession-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CFSession-0.2.3.tar", last modified: Fri Apr 21 13:19:48 2023, max compression
+gzip compressed data, was "dist\CFSession-1.0.0.tar", last modified: Thu Jul 20 08:28:40 2023, max compression
```

## Comparing `CFSession-0.2.3.tar` & `CFSession-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession/
--rw-rw-rw-   0        0        0      472 2022-11-30 08:50:37.000000 CFSession-0.2.3/CFSession/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-04-02 08:05:39.000000 CFSession-0.2.3/CFSession/cf.py
--rw-rw-rw-   0        0        0    11568 2023-04-21 13:07:00.000000 CFSession-0.2.3/CFSession/cfbrowser.py
--rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-0.2.3/CFSession/cfcookie.py
--rw-rw-rw-   0        0        0     1738 2023-04-02 08:05:39.000000 CFSession-0.2.3/CFSession/cfdefaults.py
--rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-0.2.3/CFSession/cfdirmodel.py
--rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-0.2.3/CFSession/cfexception.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/
--rw-rw-rw-   0        0        0     3664 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3664 2023-04-21 13:19:48.000000 CFSession-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2022-12-18 07:13:04.000000 CFSession-0.2.3/README.md
--rw-rw-rw-   0        0        0       86 2023-04-21 13:19:48.000000 CFSession-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-04-21 13:18:38.000000 CFSession-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession/
+-rw-rw-rw-   0        0        0      472 2022-11-30 08:50:37.000000 CFSession-1.0.0/CFSession/__init__.py
+-rw-rw-rw-   0        0        0     8147 2023-07-19 22:02:31.000000 CFSession-1.0.0/CFSession/cf.py
+-rw-rw-rw-   0        0        0    12589 2023-07-20 06:57:53.000000 CFSession-1.0.0/CFSession/cfbrowser.py
+-rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-1.0.0/CFSession/cfcookie.py
+-rw-rw-rw-   0        0        0     1807 2023-07-19 17:41:30.000000 CFSession-1.0.0/CFSession/cfdefaults.py
+-rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-1.0.0/CFSession/cfdirmodel.py
+-rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-1.0.0/CFSession/cfexception.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/
+-rw-rw-rw-   0        0        0     3664 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3664 2023-07-20 08:28:40.000000 CFSession-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2023-07-19 19:15:56.000000 CFSession-1.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-20 08:28:40.000000 CFSession-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-14 17:12:54.000000 CFSession-1.0.0/setup.py
```

### Comparing `CFSession-0.2.3/CFSession/cf.py` & `CFSession-1.0.0/CFSession/cf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
+#UC
 import undetected_chromedriver as uc
+#Sel
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
+from selenium.common.exceptions import StaleElementReferenceException
 from selenium.common.exceptions import WebDriverException
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+
+#Modules
 from .cfdefaults import Required_defaults
 from pathlib import Path
 import typing
 import time
 import sys
 import json
+import threading
 
 #Not a constant. CAPITAL for more readable syntax
 #If constant is ever declared we will use CONST_VARIABLE_NAME
 IGNORE_WARN = True
 STDOUT = False
 DEBUG = False
 DUMMY = False
 
 def de_print(text: str):
     if DEBUG:
-        text = text.encode('ascii', 'ignore')
         try:
             print(text)
         except UnicodeEncodeError:
-            print("Unicode error occured cannot print")
+            print("Uni Err, ascii md")
+            text = text.encode('ascii', 'ignore')
+            print(text)
         except Exception as e:
             print("[warn] Error occured on a debugger de", e)
     
     
 def norm_print(text):
     if STDOUT or DEBUG:
         text = text.encode('ascii', 'ignore')
@@ -45,25 +55,56 @@
         print("-"*20)
         print("You received this warning as it might be critical to the processs of the program")
         print*("Ignore this warning by using CFSession.cf.IGNORE_WARN = True")
     elif level <= acceptable:
         print(f"[WARN] {text}")
 
 class CFBypass:
-    def __init__(self, driver, directory, target = ["Just a moment...","Please Wait..."]) -> None:
+    def __init__(self, driver: uc.Chrome, directory, target = ["Just a moment...","Please Wait..."], timeout: int = 40, bypass_mode: bool = True) -> None:
         self.TARGET_NAME = target
         self.driver = driver
+        self.website = driver.current_url
         self.directory = directory
-        self.timeout = 40
+        self.timeout = timeout
+        self.bypass_mode = bypass_mode
     
     def start(self):
         return self._main_process()
-
+    
+    def find_element(self, element, max_attempts=3):
+        attempt = 1
+        while True:
+            de_print(f"Finding element: {element}")
+            try:
+                return self.driver.find_element(*element)
+            except StaleElementReferenceException as e:
+                de_print(f"Error element stale {attempt}/{max_attempts} {e}")
+                if attempt == max_attempts:
+                    raise
+                attempt += 1
+
+    def init_bypass(self):
+        WaitFor = lambda i: WebDriverWait(self.driver, 10).until(
+            EC.visibility_of(
+            self.find_element(
+            (By.TAG_NAME, 'body'),
+            ))) and time.sleep(i)
+        self.driver.execute_script(f'window.open("{self.website}","_blank");')
+        WaitFor(5)
+        self.driver.switch_to.window(window_name=self.driver.window_handles[0])
+        self.driver.close() # close first tab
+        self.driver.switch_to.window(window_name=self.driver.window_handles[0]) 
+        WaitFor(2)
+        self.driver.get("https://google.com")
+        WaitFor(2)
+        self.driver.get(self.website)
+        
     def _main_process(self):
         timeout = 0
+        if self.bypass_mode: self.init_bypass()
         while any(ext in self.driver.title for ext in self.TARGET_NAME):
             timeout += 1
             if timeout >= self.timeout:
                 break
             norm_print("Waiting for cloudflare...")
             de_print(f"cur: {self.driver.title}")
             time.sleep(1)
@@ -87,25 +128,27 @@
             dummy = [{"domain": ".nowsecure.nl", "expiry": 1690714605, "httpOnly": True, "name": "cf_clearance", "path": "/", "sameSite": "None", "secure": True, "value": "IOt5_jFk89BojBTV0NWAPj8zh4xq_zSxxt.2scnbY.4-1659175005-0-150"}]
             self.save_cookie(dummy , open(self.directory.cookie_path(),"w"))
         else:
             self.save_cookie(self.driver.get_cookies(), open(self.directory.cookie_path(),"w"))
             de_print("Cookies Saved")
 
 class SiteBrowserProcess:
-    def __init__(self, destination: str, directory: str, ignore_defaults: bool = False, defaults: typing.Union[Required_defaults, bool] = Required_defaults(), *args, **kwargs) -> None:
+    def __init__(self, destination: str, directory: str, headless_mode: bool = False, ignore_defaults: bool = False, defaults: typing.Union[Required_defaults, bool] = Required_defaults(), process_timeout: int = 40, bypass_mode: bool = True, *args, **kwargs) -> None:
         self.args = args
         self.kwargs = kwargs
         self.defaults = defaults
         self.ignore_defaults = ignore_defaults
         self.destination = destination
         self.directory = directory
         self.process_done = False
-        self.isheadless = False
+        self.isheadless = headless_mode
+        self.bypass_mode = bypass_mode
         self.exception = None
         self.has_started = False
+        self.p_timeout = process_timeout
         Path(self.directory.cache_path()).mkdir(parents=True, exist_ok=True) 
 
     def close(self):
         try:
             self.driver.quit()
             self.proc_done = True
         except AttributeError:
@@ -121,24 +164,25 @@
         if self.ignore_defaults and not self.defaults:
             warn_print("You are overriding default arguments without cfdefaults, these may be important to work properly.\nIt is recommended to use 'CFSession.cfdefaults.RequiredDefaults' to modify changes",1)
             return self._init_chromedriver_manual()
         options = self.defaults.options_default()
         desired_cap = self.defaults.desired_capabilites_default()
         cdriver_path = self.directory.chromedriver_path() #the function will return None(default), or a str path
         try:
-            self.driver =  uc.Chrome(desired_capabilities=desired_cap,options=options,driver_executable_path=cdriver_path,*self.args, **self.kwargs)
+            self.driver =  uc.Chrome(desired_capabilities=desired_cap,options=options,driver_executable_path=cdriver_path,headless=self.isheadless,*self.args, **self.kwargs)
         except RuntimeError: #Catch if the objects were reused
             self.defaults.reset_objects()
             options = self.defaults.options_default()
             desired_cap = self.defaults.desired_capabilites_default()
             self.driver =  uc.Chrome(desired_capabilities=desired_cap,options=options,driver_executable_path=cdriver_path,*self.args, **self.kwargs)
         norm_print("Driver initialized")
         
     def init_cf(self,CFobj: CFBypass = CFBypass):
-        return CFobj(self.driver, self.directory)
+        de_print(f"Bypass mode enabled: {self.bypass_mode}")
+        return CFobj(self.driver, self.directory, timeout = self.p_timeout, bypass_mode = self.bypass_mode)
 
     def load_cf(self):
         self.driver.get(self.destination) 
         de_print(self.driver.title)
         cloud = self.init_cf()
         return cloud.start()
```

### Comparing `CFSession-0.2.3/CFSession/cfbrowser.py` & `CFSession-1.0.0/CFSession/cfbrowser.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,24 +25,42 @@
       >>> s = CFSession.cfSession()
       >>> s.get('https://httpbin.org/get')
       <Response [200]>
     Or as a context manager::
       >>> with CFSession.cfSession() as s:
       ...     s.get('https://httpbin.org/get')
       <Response [200]>
+    
+    Parameters:
+        - directory (cfDirectory, optional): An instance of cfDirectory representing the directory to use. 
+                If not provided, a new cfDirectory instance will be created.
+
+        - headless_mode (bool, optional): Whether to run in headless mode (without a graphical user interface). 
+            Default is False.
+
+        - tries (int, optional): The number of tries or attempts to bypass cf without human intervention. Default is 3.
+                If cf bypass fails, it will automatically revert to providing data from the original, un-bypassed site.
+
+        - *cfarg: Pass arguments to SiteBrowserProcess class (non-keyword arguments).
+
+        - **cfkwarg: Pass keyword arguments to SiteBrowserProcess class.
     """
 
-    def __init__(self,directory: cfDirectory = cfDirectory(),*cfarg, **cfkwarg):
+    
+
+    def __init__(self,directory: cfDirectory = cfDirectory(), headless_mode: bool = False, tries: int = 3,*cfarg, **cfkwarg):
         self.session = requests.Session()
         self.arg = cfarg
         self.kwarg = cfkwarg
+        self.headless = headless_mode
         self.directory = directory
         self.cookieChecker = cfSessionHandler(self.directory)
         self._setcookies_status = self.set_cookies()
         self.cf_proccache = None
+        self.tries = tries
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
@@ -127,15 +145,15 @@
     def _handle_equalfunc(self):
         if not self._setcookies_status:
             self.reload_token(self.url)
             self.set_cookies()
 
     def request(self,method,url,**kwargs) -> requests.Response:
         content = None
-        for t in range(0,2):
+        for t in range(0,self.tries):
             try:
                 if method == "GET":
                     content = self.session.get(url, **kwargs)
                 elif method == "POST":
                     content = self.session.post(url, **kwargs)
                 elif method == "PATCH":
                     content = self.session.patch(url, **kwargs)
@@ -190,16 +208,16 @@
 
     def _response_hook_raiseforstatus(self, objself: CFException):
         """Raises `CFException` if an error has occured"""
         if isinstance(self.exception,CFException):
                 raise self.exception
 
     def _class_initialize(self,site_requested,directory,*args,**kwargs):
-        return SiteBrowserProcess(site_requested,directory=directory,*args,**kwargs)
-
+        return SiteBrowserProcess(site_requested,directory=directory,headless_mode=self.headless,*args,**kwargs)
+    
     def close(self):
         self.session.close()
         if self.cf_proccache:
             self.cf_proccache.close()
             del self.cf_proccache
 
     def __repr__(self):
@@ -250,24 +268,25 @@
 
 class cfSimulacrum(cfSession):
     def __init__(self, *aer, **res):
         super().__init__(*aer,**res)
         self.cdriver = None
         self.cfinder = None
         self.site = None
+        self.bypass_mode = False
         
     def copen(self, site_requested, *aer, **res) -> SiteBrowserProcess: # returns SiteBrowserProcess
         self.site = site_requested
-        self.cdriver = self._class_initialize(site_requested,directory=self.directory, *aer, **res)
+        self.cdriver = self._class_initialize(site_requested,directory=self.directory, bypass_mode=self.bypass_mode, *aer, **res)
         self.cdriver._init_chromedriver_manual() 
         self.cdriver.driver.get(self.site)
         return self.cdriver
 
     def find(self) -> CFBypass: #returns CFBypass
-        self.cfinder = CFBypass(self.cdriver.driver, self.directory)
+        self.cfinder = CFBypass(self.cdriver.driver, self.directory, bypass_mode=self.bypass_mode)
         return self.cfinder
 
     def search(self,target_title: Union[str, list] = None):
         if not self.cfinder:
             self.cfinder = CFBypass(self.cdriver.driver, self.directory)
         self.cfinder.TARGET_NAME = target_title if target_title != None else self.cfinder.TARGET_NAME
         self.cfinder.start()
```

### Comparing `CFSession-0.2.3/CFSession/cfcookie.py` & `CFSession-1.0.0/CFSession/cfcookie.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.3/CFSession/cfdefaults.py` & `CFSession-1.0.0/CFSession/cfdefaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         self.dcp = DesiredCapabilities().CHROME
 
     def options_default(self) -> uc.ChromeOptions():
         try:
             self.options.use_chromium=True
             self.options.add_argument("--disable-renderer-backgrounding")
             self.options.add_argument("--disable-backgrounding-occluded-windows")
+            self.options.add_argument("--disable-popup-blocking")
+
         except AttributeError:
             self.reset_objects()
             return self.options_default()
         return self.options
 
     def desired_capabilites_default(self) -> DesiredCapabilities:
         self.dcp["pageLoadStrategy"] = "eager"
```

### Comparing `CFSession-0.2.3/CFSession/cfdirmodel.py` & `CFSession-1.0.0/CFSession/cfdirmodel.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.3/CFSession/cfexception.py` & `CFSession-1.0.0/CFSession/cfexception.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.3/CFSession.egg-info/PKG-INFO` & `CFSession-1.0.0/CFSession.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 0.2.3
+Version: 1.0.0
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,15 @@
 <a href="https://pypi.org/project/CFSession"><img src="https://github.com/Kinuseka/CFSession/actions/workflows/python-package.yml/badge.svg" alt="Build Test"></a>
 
 
 
 
 ## How it works
 It relies on a modified selenium (undetected-chromedriver) to cloak on sites that block selenium based sessions. 
-When a program is able to pass through the IAUM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
+When a program is able to pass through the IUAM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
 
 The library wraps around requests library.
 
 **Tested request types:**
 * GET
 * POST
```

### Comparing `CFSession-0.2.3/LICENSE` & `CFSession-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.3/PKG-INFO` & `CFSession-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 0.2.3
+Version: 1.0.0
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,15 @@
 <a href="https://pypi.org/project/CFSession"><img src="https://github.com/Kinuseka/CFSession/actions/workflows/python-package.yml/badge.svg" alt="Build Test"></a>
 
 
 
 
 ## How it works
 It relies on a modified selenium (undetected-chromedriver) to cloak on sites that block selenium based sessions. 
-When a program is able to pass through the IAUM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
+When a program is able to pass through the IUAM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
 
 The library wraps around requests library.
 
 **Tested request types:**
 * GET
 * POST
```

### Comparing `CFSession-0.2.3/README.md` & `CFSession-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <a href="https://pypi.org/project/CFSession"><img src="https://github.com/Kinuseka/CFSession/actions/workflows/python-package.yml/badge.svg" alt="Build Test"></a>
 
 
 
 
 ## How it works
 It relies on a modified selenium (undetected-chromedriver) to cloak on sites that block selenium based sessions. 
-When a program is able to pass through the IAUM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
+When a program is able to pass through the IUAM or Captcha verification the program immedietely saves the session token to cache to be able to access to the site right away without needing to verify again when program closes(until the token expires).
 
 The library wraps around requests library.
 
 **Tested request types:**
 * GET
 * POST
```

### Comparing `CFSession-0.2.3/setup.py` & `CFSession-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setup(
     name='CFSession',
-    version='0.2.3',
+    version='1.0.0',
     author='Kinuseka',
     author_email='realkingseeker1089@gmail.com',
     description='A Cloudflare IUAM session grabber',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Kinuseka/CFSession',
     classifiers=[
```

